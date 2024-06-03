# Comparing `tmp/byron-0.8a1.dev8.tar.gz` & `tmp/byron-0.8a1.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "byron-0.8a1.dev8.tar", max compression
+gzip compressed data, was "byron-0.8a1.dev9.tar", max compression
```

## Comparing `byron-0.8a1.dev8.tar` & `byron-0.8a1.dev9.tar`

### file list

```diff
@@ -1,70 +1,70 @@
--rw-r--r--   0        0        0    11357 2023-08-16 06:13:19.244265 byron-0.8a1.dev8/LICENSE
--rw-r--r--   0        0        0     5881 2023-08-21 14:40:56.870439 byron-0.8a1.dev8/byron/__init__.py
--rw-r--r--   0        0        0     1720 2023-08-16 11:28:02.728112 byron-0.8a1.dev8/byron/classes/__init__.py
--rw-r--r--   0        0        0    10551 2023-08-18 18:14:10.097768 byron-0.8a1.dev8/byron/classes/_individual_as.py
--rw-r--r--   0        0        0     2469 2023-08-16 11:28:02.728353 byron-0.8a1.dev8/byron/classes/byron.py
--rw-r--r--   0        0        0     1350 2023-08-16 11:28:02.728552 byron-0.8a1.dev8/byron/classes/dump.py
--rw-r--r--   0        0        0    27164 2023-08-21 18:01:55.909248 byron-0.8a1.dev8/byron/classes/evaluator.py
--rw-r--r--   0        0        0     5013 2023-08-16 11:28:02.729164 byron-0.8a1.dev8/byron/classes/fitness.py
--rw-r--r--   0        0        0     2900 2023-08-21 17:47:57.435389 byron-0.8a1.dev8/byron/classes/frame.py
--rw-r--r--   0        0        0     1663 2023-08-16 11:28:02.729566 byron-0.8a1.dev8/byron/classes/identifiable.py
--rw-r--r--   0        0        0    23217 2023-08-21 18:00:08.721370 byron-0.8a1.dev8/byron/classes/individual.py
--rw-r--r--   0        0        0     3537 2023-08-21 14:35:44.113498 byron-0.8a1.dev8/byron/classes/macro.py
--rw-r--r--   0        0        0     2833 2023-08-16 11:28:02.730377 byron-0.8a1.dev8/byron/classes/monitor.py
--rw-r--r--   0        0        0     1581 2023-08-16 11:28:02.730552 byron-0.8a1.dev8/byron/classes/node_reference.py
--rw-r--r--   0        0        0     6020 2023-08-21 17:28:14.869166 byron-0.8a1.dev8/byron/classes/node_view.py
--rw-r--r--   0        0        0     5436 2023-08-21 14:17:18.270798 byron-0.8a1.dev8/byron/classes/parameter.py
--rw-r--r--   0        0        0     2227 2023-08-16 11:28:02.731176 byron-0.8a1.dev8/byron/classes/paranoid.py
--rw-r--r--   0        0        0     6447 2023-08-21 15:31:42.723298 byron-0.8a1.dev8/byron/classes/population.py
--rw-r--r--   0        0        0     1576 2023-08-16 11:28:02.731588 byron-0.8a1.dev8/byron/classes/readymade_frames.py
--rw-r--r--   0        0        0     2720 2023-08-21 14:37:40.146288 byron-0.8a1.dev8/byron/classes/readymade_macros.py
--rw-r--r--   0        0        0     3797 2023-08-21 14:37:40.153256 byron-0.8a1.dev8/byron/classes/selement.py
--rw-r--r--   0        0        0     1306 2023-08-16 11:28:02.732233 byron-0.8a1.dev8/byron/classes/shared.py
--rw-r--r--   0        0        0     5655 2023-08-16 11:28:02.732405 byron-0.8a1.dev8/byron/classes/value_bag.py
--rw-r--r--   0        0        0     1373 2023-08-16 11:28:02.732586 byron-0.8a1.dev8/byron/ea/__init__.py
--rw-r--r--   0        0        0     1899 2023-08-16 11:28:02.732764 byron-0.8a1.dev8/byron/ea/check.py
--rw-r--r--   0        0        0     1288 2023-08-16 11:28:02.732928 byron-0.8a1.dev8/byron/ea/common.py
--rw-r--r--   0        0        0     2860 2023-08-16 11:28:02.733117 byron-0.8a1.dev8/byron/ea/parametric.py
--rw-r--r--   0        0        0     1865 2023-08-16 11:28:02.733289 byron-0.8a1.dev8/byron/ea/selection.py
--rw-r--r--   0        0        0     5955 2023-08-21 15:02:46.543019 byron-0.8a1.dev8/byron/ea/vanilla.py
--rw-r--r--   0        0        0     1353 2023-08-16 11:28:02.733639 byron-0.8a1.dev8/byron/evaluator_.py
--rw-r--r--   0        0        0     1317 2023-08-16 11:28:02.733813 byron-0.8a1.dev8/byron/fitness/__init__.py
--rw-r--r--   0        0        0     6651 2023-08-16 11:28:02.733999 byron-0.8a1.dev8/byron/fitness/basic.py
--rw-r--r--   0        0        0     2586 2023-08-16 11:28:02.734167 byron-0.8a1.dev8/byron/fitness/reverse.py
--rw-r--r--   0        0        0     1346 2023-08-16 11:28:02.734330 byron-0.8a1.dev8/byron/fitness_.py
--rw-r--r--   0        0        0      436 2023-08-16 06:13:19.247310 byron-0.8a1.dev8/byron/fitness_log.py
--rw-r--r--   0        0        0     1928 2023-08-18 18:14:10.099225 byron-0.8a1.dev8/byron/framework/__init__.py
--rw-r--r--   0        0        0     4655 2023-08-16 16:48:21.228009 byron-0.8a1.dev8/byron/framework/bnf.py
--rw-r--r--   0        0        0     3484 2023-08-16 06:13:19.247583 byron-0.8a1.dev8/byron/framework/defaults.py
--rw-r--r--   0        0        0     7995 2023-08-21 17:22:35.955315 byron-0.8a1.dev8/byron/framework/framework.py
--rw-r--r--   0        0        0     3749 2023-08-16 11:28:02.735107 byron-0.8a1.dev8/byron/framework/macro.py
--rw-r--r--   0        0        0     9772 2023-08-20 12:33:27.203699 byron-0.8a1.dev8/byron/framework/parameter.py
--rw-r--r--   0        0        0     5669 2023-08-20 12:33:27.204566 byron-0.8a1.dev8/byron/framework/parameter_structural_global.py
--rw-r--r--   0        0        0     3376 2023-08-20 12:33:27.204748 byron-0.8a1.dev8/byron/framework/parameter_structural_local.py
--rw-r--r--   0        0        0     2518 2023-08-21 14:17:18.272743 byron-0.8a1.dev8/byron/framework/shared.py
--rw-r--r--   0        0        0     4274 2023-08-18 18:14:10.099661 byron-0.8a1.dev8/byron/framework/show_element.py
--rw-r--r--   0        0        0     2132 2023-08-16 11:28:02.736359 byron-0.8a1.dev8/byron/framework/utilities.py
--rw-r--r--   0        0        0     2328 2023-08-16 11:28:02.736608 byron-0.8a1.dev8/byron/functions.py
--rw-r--r--   0        0        0     4546 2023-08-21 18:04:09.538047 byron-0.8a1.dev8/byron/global_symbols.py
--rw-r--r--   0        0        0     1396 2023-08-20 12:33:27.205056 byron-0.8a1.dev8/byron/operators/__init__.py
--rw-r--r--   0        0        0     3493 2023-08-18 18:14:10.100258 byron-0.8a1.dev8/byron/operators/_graph_crossover.py
--rw-r--r--   0        0        0     1902 2023-08-16 11:28:02.737263 byron-0.8a1.dev8/byron/operators/initializers.py
--rw-r--r--   0        0        0     4200 2023-08-20 12:33:27.205204 byron-0.8a1.dev8/byron/operators/mutation.py
--rw-r--r--   0        0        0     2522 2023-08-20 18:09:23.615445 byron-0.8a1.dev8/byron/operators/parameter_crossover.py
--rw-r--r--   0        0        0     4897 2023-08-21 14:17:18.272961 byron-0.8a1.dev8/byron/operators/tools.py
--rw-r--r--   0        0        0     5106 2023-08-21 14:17:18.273203 byron-0.8a1.dev8/byron/operators/unroll.py
--rw-r--r--   0        0        0     1516 2023-08-20 12:33:27.205549 byron-0.8a1.dev8/byron/randy/__init__.py
--rw-r--r--   0        0        0     6787 2023-08-21 18:01:55.916073 byron-0.8a1.dev8/byron/randy/main.py
--rw-r--r--   0        0        0     7467 2023-08-21 18:01:55.893992 byron-0.8a1.dev8/byron/registry.py
--rw-r--r--   0        0        0     4368 2023-08-21 14:17:18.273533 byron-0.8a1.dev8/byron/sys.py
--rw-r--r--   0        0        0     2298 2023-08-21 15:30:05.364211 byron-0.8a1.dev8/byron/tools/entropy.py
--rw-r--r--   0        0        0     7322 2023-08-18 18:14:10.101269 byron-0.8a1.dev8/byron/tools/graph.py
--rw-r--r--   0        0        0     4295 2023-08-21 18:01:55.897656 byron-0.8a1.dev8/byron/tools/names.py
--rw-r--r--   0        0        0     2040 2023-08-21 17:59:43.278828 byron-0.8a1.dev8/byron/tools/node_to_string.py
--rw-r--r--   0        0        0     1402 2023-08-16 11:28:02.738656 byron-0.8a1.dev8/byron/user_messages/__init__.py
--rw-r--r--   0        0        0     4593 2023-08-21 18:01:55.901255 byron-0.8a1.dev8/byron/user_messages/checks.py
--rw-r--r--   0        0        0     1731 2023-08-16 11:28:02.738976 byron-0.8a1.dev8/byron/user_messages/exception.py
--rw-r--r--   0        0        0     5780 2023-08-19 14:19:17.877429 byron-0.8a1.dev8/byron/user_messages/messaging.py
--rw-r--r--   0        0        0     2486 2023-08-18 18:14:10.101774 byron-0.8a1.dev8/docs/pypi.md
--rw-r--r--   0        0        0     3390 2023-08-21 18:04:09.536976 byron-0.8a1.dev8/pyproject.toml
--rw-r--r--   0        0        0     3983 1970-01-01 00:00:00.000000 byron-0.8a1.dev8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-08-16 06:13:19.244265 byron-0.8a1.dev9/LICENSE
+-rw-r--r--   0        0        0     5553 2023-08-22 16:17:32.113145 byron-0.8a1.dev9/byron/__init__.py
+-rw-r--r--   0        0        0     1720 2023-08-22 15:03:51.021909 byron-0.8a1.dev9/byron/classes/__init__.py
+-rw-r--r--   0        0        0    10551 2023-08-22 15:03:50.941520 byron-0.8a1.dev9/byron/classes/_individual_as.py
+-rw-r--r--   0        0        0     2469 2023-08-22 15:03:51.159144 byron-0.8a1.dev9/byron/classes/byron.py
+-rw-r--r--   0        0        0     1350 2023-08-22 15:03:51.044000 byron-0.8a1.dev9/byron/classes/dump.py
+-rw-r--r--   0        0        0    27164 2023-08-22 15:52:09.835724 byron-0.8a1.dev9/byron/classes/evaluator.py
+-rw-r--r--   0        0        0     4965 2023-08-22 15:52:09.829630 byron-0.8a1.dev9/byron/classes/fitness.py
+-rw-r--r--   0        0        0     2900 2023-08-22 15:03:51.091772 byron-0.8a1.dev9/byron/classes/frame.py
+-rw-r--r--   0        0        0     1663 2023-08-22 15:03:51.019407 byron-0.8a1.dev9/byron/classes/identifiable.py
+-rw-r--r--   0        0        0    23343 2023-08-22 15:52:09.842381 byron-0.8a1.dev9/byron/classes/individual.py
+-rw-r--r--   0        0        0     2805 2023-08-22 15:03:51.101340 byron-0.8a1.dev9/byron/classes/macro.py
+-rw-r--r--   0        0        0     2833 2023-08-22 15:03:51.018670 byron-0.8a1.dev9/byron/classes/monitor.py
+-rw-r--r--   0        0        0     1581 2023-08-22 15:03:51.154469 byron-0.8a1.dev9/byron/classes/node_reference.py
+-rw-r--r--   0        0        0     6020 2023-08-22 15:03:51.030343 byron-0.8a1.dev9/byron/classes/node_view.py
+-rw-r--r--   0        0        0     5436 2023-08-22 15:52:09.833851 byron-0.8a1.dev9/byron/classes/parameter.py
+-rw-r--r--   0        0        0     2227 2023-08-22 15:03:50.919063 byron-0.8a1.dev9/byron/classes/paranoid.py
+-rw-r--r--   0        0        0     6447 2023-08-22 15:03:51.135500 byron-0.8a1.dev9/byron/classes/population.py
+-rw-r--r--   0        0        0     1452 2023-08-22 16:07:48.446955 byron-0.8a1.dev9/byron/classes/readymade_frames.py
+-rw-r--r--   0        0        0     2454 2023-08-22 15:03:51.080700 byron-0.8a1.dev9/byron/classes/readymade_macros.py
+-rw-r--r--   0        0        0     6463 2023-08-22 16:07:32.664254 byron-0.8a1.dev9/byron/classes/selement.py
+-rw-r--r--   0        0        0     1306 2023-08-22 15:03:51.041682 byron-0.8a1.dev9/byron/classes/shared.py
+-rw-r--r--   0        0        0     5655 2023-08-22 15:03:51.011856 byron-0.8a1.dev9/byron/classes/value_bag.py
+-rw-r--r--   0        0        0     1373 2023-08-22 15:03:50.948258 byron-0.8a1.dev9/byron/ea/__init__.py
+-rw-r--r--   0        0        0     1899 2023-08-22 15:03:51.161598 byron-0.8a1.dev9/byron/ea/check.py
+-rw-r--r--   0        0        0     1288 2023-08-22 15:03:51.045071 byron-0.8a1.dev9/byron/ea/common.py
+-rw-r--r--   0        0        0     2860 2023-08-22 15:03:50.990857 byron-0.8a1.dev9/byron/ea/parametric.py
+-rw-r--r--   0        0        0     1865 2023-08-22 15:03:51.034314 byron-0.8a1.dev9/byron/ea/selection.py
+-rw-r--r--   0        0        0     5955 2023-08-22 15:03:51.183000 byron-0.8a1.dev9/byron/ea/vanilla.py
+-rw-r--r--   0        0        0     1353 2023-08-22 15:03:51.017822 byron-0.8a1.dev9/byron/evaluator_.py
+-rw-r--r--   0        0        0     1317 2023-08-22 15:03:51.015396 byron-0.8a1.dev9/byron/fitness/__init__.py
+-rw-r--r--   0        0        0     6077 2023-08-22 16:17:18.540408 byron-0.8a1.dev9/byron/fitness/basic.py
+-rw-r--r--   0        0        0     2459 2023-08-22 16:17:00.532340 byron-0.8a1.dev9/byron/fitness/reverse.py
+-rw-r--r--   0        0        0     1346 2023-08-22 15:03:51.027249 byron-0.8a1.dev9/byron/fitness_.py
+-rw-r--r--   0        0        0      436 2023-08-16 06:13:19.247310 byron-0.8a1.dev9/byron/fitness_log.py
+-rw-r--r--   0        0        0     1928 2023-08-22 15:03:19.230621 byron-0.8a1.dev9/byron/framework/__init__.py
+-rw-r--r--   0        0        0     4451 2023-08-22 16:10:04.465663 byron-0.8a1.dev9/byron/framework/bnf.py
+-rw-r--r--   0        0        0     3484 2023-08-22 15:52:09.830833 byron-0.8a1.dev9/byron/framework/defaults.py
+-rw-r--r--   0        0        0     7534 2023-08-22 16:08:05.063013 byron-0.8a1.dev9/byron/framework/framework.py
+-rw-r--r--   0        0        0     3551 2023-08-22 15:03:19.228294 byron-0.8a1.dev9/byron/framework/macro.py
+-rw-r--r--   0        0        0     9612 2023-08-22 15:03:19.233473 byron-0.8a1.dev9/byron/framework/parameter.py
+-rw-r--r--   0        0        0     5457 2023-08-22 15:52:09.844521 byron-0.8a1.dev9/byron/framework/parameter_structural_global.py
+-rw-r--r--   0        0        0     3274 2023-08-22 15:03:19.219743 byron-0.8a1.dev9/byron/framework/parameter_structural_local.py
+-rw-r--r--   0        0        0     2451 2023-08-22 15:03:19.226971 byron-0.8a1.dev9/byron/framework/shared.py
+-rw-r--r--   0        0        0     4274 2023-08-22 15:11:26.896894 byron-0.8a1.dev9/byron/framework/show_element.py
+-rw-r--r--   0        0        0     2132 2023-08-22 15:03:19.224809 byron-0.8a1.dev9/byron/framework/utilities.py
+-rw-r--r--   0        0        0     2328 2023-08-22 15:03:50.930643 byron-0.8a1.dev9/byron/functions.py
+-rw-r--r--   0        0        0     4546 2023-08-22 16:25:29.368422 byron-0.8a1.dev9/byron/global_symbols.py
+-rw-r--r--   0        0        0     1396 2023-08-22 15:03:51.012860 byron-0.8a1.dev9/byron/operators/__init__.py
+-rw-r--r--   0        0        0     3493 2023-08-22 15:03:51.033069 byron-0.8a1.dev9/byron/operators/_graph_crossover.py
+-rw-r--r--   0        0        0     1902 2023-08-22 15:03:51.008376 byron-0.8a1.dev9/byron/operators/initializers.py
+-rw-r--r--   0        0        0     4200 2023-08-22 15:03:50.886214 byron-0.8a1.dev9/byron/operators/mutation.py
+-rw-r--r--   0        0        0     2522 2023-08-22 15:03:51.002299 byron-0.8a1.dev9/byron/operators/parameter_crossover.py
+-rw-r--r--   0        0        0     4897 2023-08-22 15:03:51.007485 byron-0.8a1.dev9/byron/operators/tools.py
+-rw-r--r--   0        0        0     5106 2023-08-22 15:52:09.845507 byron-0.8a1.dev9/byron/operators/unroll.py
+-rw-r--r--   0        0        0     1516 2023-08-22 15:03:51.167314 byron-0.8a1.dev9/byron/randy/__init__.py
+-rw-r--r--   0        0        0     6787 2023-08-21 18:04:56.671683 byron-0.8a1.dev9/byron/randy/main.py
+-rw-r--r--   0        0        0     7368 2023-08-22 15:12:45.475725 byron-0.8a1.dev9/byron/registry.py
+-rw-r--r--   0        0        0     4367 2023-08-22 15:03:51.097070 byron-0.8a1.dev9/byron/sys.py
+-rw-r--r--   0        0        0     2298 2023-08-22 15:03:50.994038 byron-0.8a1.dev9/byron/tools/entropy.py
+-rw-r--r--   0        0        0     7322 2023-08-22 15:52:09.832247 byron-0.8a1.dev9/byron/tools/graph.py
+-rw-r--r--   0        0        0     1882 2023-08-22 16:03:59.649047 byron-0.8a1.dev9/byron/tools/names.py
+-rw-r--r--   0        0        0     2040 2023-08-22 15:03:50.906090 byron-0.8a1.dev9/byron/tools/node_to_string.py
+-rw-r--r--   0        0        0     1402 2023-08-22 15:03:51.086861 byron-0.8a1.dev9/byron/user_messages/__init__.py
+-rw-r--r--   0        0        0     4593 2023-08-22 15:03:51.171730 byron-0.8a1.dev9/byron/user_messages/checks.py
+-rw-r--r--   0        0        0     1731 2023-08-22 15:03:51.022708 byron-0.8a1.dev9/byron/user_messages/exception.py
+-rw-r--r--   0        0        0     5780 2023-08-22 15:03:50.986334 byron-0.8a1.dev9/byron/user_messages/messaging.py
+-rw-r--r--   0        0        0     2486 2023-08-18 18:14:10.101774 byron-0.8a1.dev9/docs/pypi.md
+-rw-r--r--   0        0        0     3390 2023-08-22 16:25:29.367091 byron-0.8a1.dev9/pyproject.toml
+-rw-r--r--   0        0        0     3983 1970-01-01 00:00:00.000000 byron-0.8a1.dev9/PKG-INFO
```

### Comparing `byron-0.8a1.dev8/LICENSE` & `byron-0.8a1.dev9/LICENSE`

 * *Files identical despite different names*

### Comparing `byron-0.8a1.dev8/byron/__init__.py` & `byron-0.8a1.dev9/byron/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #################################|###|#####################################
 #  __                            |   |                                    #
-# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.1    #
+# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.8    #
 # |  _  |  |  |   _|  _  |     | |___| An evolutionary optimizer & fuzzer #
 # |_____|___  |__| |_____|__|__|  ).(  https://pypi.org/project/byron/    #
 #       |_____|                   \|/                                     #
 ################################## ' ######################################
 
 # Copyright 2023 Giovanni Squillero and Alberto Tonda
 #
@@ -100,23 +100,14 @@
 from byron.tools.entropy import *
 
 
 #############################################################################
 # Patch names to ease debugging and visualization
 
 # noinspection PyUnresolvedReferences
-from byron.tools.names import _patch_class_info
-
-for name in sorted(dir()):
-    item = globals()[name]
-    if isinstance(item, type) and item.__name__.endswith("ABC"):
-        _patch_class_info(item, item.__name__, tag="abc")
-    elif isinstance(item, type):
-        _patch_class_info(item, item.__name__)
-del _patch_class_info
 
 #############################################################################
 # Welcome!
 
 # __welcome__ = (
 #     f'This is Byron v{__version__} "{__codename__}"\n' + f"(c) 2023 G. Squillero & A. Tonda — Licensed under Apache-2.0"
 # )
```

### Comparing `byron-0.8a1.dev8/byron/classes/__init__.py` & `byron-0.8a1.dev9/byron/classes/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #################################|###|#####################################
 #  __                            |   |                                    #
-# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.1    #
+# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.8    #
 # |  _  |  |  |   _|  _  |     | |___| An evolutionary optimizer & fuzzer #
 # |_____|___  |__| |_____|__|__|  ).(  https://pypi.org/project/byron/    #
 #       |_____|                   \|/                                     #
 ################################## ' ######################################
 
 # Copyright 2023 Giovanni Squillero and Alberto Tonda
 #
```

### Comparing `byron-0.8a1.dev8/byron/classes/_individual_as.py` & `byron-0.8a1.dev9/byron/classes/_individual_as.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #################################|###|#####################################
 #  __                            |   |                                    #
-# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.1    #
+# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.8    #
 # |  _  |  |  |   _|  _  |     | |___| An evolutionary optimizer & fuzzer #
 # |_____|___  |__| |_____|__|__|  ).(  https://pypi.org/project/byron/    #
 #       |_____|                   \|/                                     #
 ################################## ' ######################################
 
 # Copyright 2023 Giovanni Squillero and Alberto Tonda
 #
```

### Comparing `byron-0.8a1.dev8/byron/classes/byron.py` & `byron-0.8a1.dev9/byron/classes/byron.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #################################|###|#####################################
 #  __                            |   |                                    #
-# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.1    #
+# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.8    #
 # |  _  |  |  |   _|  _  |     | |___| An evolutionary optimizer & fuzzer #
 # |_____|___  |__| |_____|__|__|  ).(  https://pypi.org/project/byron/    #
 #       |_____|                   \|/                                     #
 ################################## ' ######################################
 
 # Copyright 2023 Giovanni Squillero and Alberto Tonda
 #
```

### Comparing `byron-0.8a1.dev8/byron/classes/dump.py` & `byron-0.8a1.dev9/byron/classes/dump.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #################################|###|#####################################
 #  __                            |   |                                    #
-# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.1    #
+# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.8    #
 # |  _  |  |  |   _|  _  |     | |___| An evolutionary optimizer & fuzzer #
 # |_____|___  |__| |_____|__|__|  ).(  https://pypi.org/project/byron/    #
 #       |_____|                   \|/                                     #
 ################################## ' ######################################
 
 # Copyright 2023 Giovanni Squillero and Alberto Tonda
 #
```

### Comparing `byron-0.8a1.dev8/byron/classes/evaluator.py` & `byron-0.8a1.dev9/byron/classes/evaluator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #################################|###|#####################################
 #  __                            |   |                                    #
-# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.1    #
+# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.8    #
 # |  _  |  |  |   _|  _  |     | |___| An evolutionary optimizer & fuzzer #
 # |_____|___  |__| |_____|__|__|  ).(  https://pypi.org/project/byron/    #
 #       |_____|                   \|/                                     #
 ################################## ' ######################################
 
 # Copyright 2023 Giovanni Squillero and Alberto Tonda
 #
@@ -493,15 +493,15 @@
             raise RuntimeError("Process failed (returned None)")
         elif not result.stdout:
             raise RuntimeError(f"Process returned empty stdout (stderr: '{result.stderr}')")
         else:
             results = list(filter(lambda s: bool(s), result.stdout.split("\n")))
             assert len(results) == len(
                 individuals
-            ), f"{PARANOIA_VALUE_ERROR}: number of results and number of individual mismatch: found {len(results)} expected {len(individuals)}"
+            ), f"{PARANOIA_VALUE_ERROR}: Number of results and number of individual mismatch: found {len(results)} expected {len(individuals)}"
             for ind, line in zip_longest(individuals, results):
                 value = [float(r) for r in line.split()]
                 if len(value) == 1:
                     value = value[0]
                 fitness = make_fitness(value)
                 ind[1].fitness = fitness
```

### Comparing `byron-0.8a1.dev8/byron/classes/fitness.py` & `byron-0.8a1.dev9/byron/classes/fitness.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #################################|###|#####################################
 #  __                            |   |                                    #
-# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.1    #
+# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.8    #
 # |  _  |  |  |   _|  _  |     | |___| An evolutionary optimizer & fuzzer #
 # |_____|___  |__| |_____|__|__|  ).(  https://pypi.org/project/byron/    #
 #       |_____|                   \|/                                     #
 ################################## ' ######################################
 
 # Copyright 2023 Giovanni Squillero and Alberto Tonda
 #
@@ -29,15 +29,14 @@
 
 from abc import ABC, abstractmethod
 from functools import wraps, cache
 
 # from byron.classes.paranoid import Paranoid
 from byron.global_symbols import *
 from byron.user_messages import *
-from byron.tools.names import _patch_class_info
 
 
 # class FitnessABC(Paranoid, ABC):
 class FitnessABC(ABC):
     """Fitness of a phenotype, handle multiple formats (eg. scalar, tuple).
 
     The class also redefines the relational operator in order to handle different types of optimization
@@ -74,15 +73,15 @@
         """Check whether some differences from the other Fitness may be perceived."""
         assert self.check_comparable(other)
         return super().__ne__(other)
 
     def check_comparable(self, other: "FitnessABC"):
         assert (
             self.__class__ == other.__class__
-        ), f"{PARANOIA_TYPE_ERROR}: different Fitness types: {self.__class__} and {other.__class__}."
+        ), f"{PARANOIA_TYPE_ERROR}: Different Fitness types: {self.__class__} and {other.__class__}."
         return True
 
     def _decorate(self) -> str:
         """Represent the individual fitness value with a nice string."""
         return f"{super().__str__()}"
 
     # FINAL/WARNINGS
```

### Comparing `byron-0.8a1.dev8/byron/classes/frame.py` & `byron-0.8a1.dev9/byron/classes/frame.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #################################|###|#####################################
 #  __                            |   |                                    #
-# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.1    #
+# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.8    #
 # |  _  |  |  |   _|  _  |     | |___| An evolutionary optimizer & fuzzer #
 # |_____|___  |__| |_____|__|__|  ).(  https://pypi.org/project/byron/    #
 #       |_____|                   \|/                                     #
 ################################## ' ######################################
 
 # Copyright 2023 Giovanni Squillero and Alberto Tonda
 #
```

### Comparing `byron-0.8a1.dev8/byron/classes/identifiable.py` & `byron-0.8a1.dev9/byron/classes/identifiable.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #################################|###|#####################################
 #  __                            |   |                                    #
-# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.1    #
+# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.8    #
 # |  _  |  |  |   _|  _  |     | |___| An evolutionary optimizer & fuzzer #
 # |_____|___  |__| |_____|__|__|  ).(  https://pypi.org/project/byron/    #
 #       |_____|                   \|/                                     #
 ################################## ' ######################################
 
 # Copyright 2023 Giovanni Squillero and Alberto Tonda
 #
```

### Comparing `byron-0.8a1.dev8/byron/classes/individual.py` & `byron-0.8a1.dev9/byron/classes/individual.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #################################|###|#####################################
 #  __                            |   |                                    #
-# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.1    #
+# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.8    #
 # |  _  |  |  |   _|  _  |     | |___| An evolutionary optimizer & fuzzer #
 # |_____|___  |__| |_____|__|__|  ).(  https://pypi.org/project/byron/    #
 #       |_____|                   \|/                                     #
 ################################## ' ######################################
 
 # Copyright 2023 Giovanni Squillero and Alberto Tonda
 #
@@ -321,30 +321,30 @@
         # ==[check genome (structural)]======================================
         assert self.genome == self._genome, f"{PARANOIA_VALUE_ERROR}: Panic!"
         assert self.genome == self.G, f"{PARANOIA_VALUE_ERROR}: Panic!"
 
         assert self.genome == self._genome, f"{PARANOIA_VALUE_ERROR}: Panic: genome != _genome"
         assert nx.is_weakly_connected(
             self._genome
-        ), f"{PARANOIA_VALUE_ERROR}: genome of {self!r} is not a connected graph"
+        ), f"{PARANOIA_VALUE_ERROR}: Genome of {self!r} is not a connected graph"
 
         G = nx.MultiDiGraph()
         G.add_edges_from(self.G.edges)
         G.remove_node(NODE_ZERO)
         assert (
             sum(1 for _ in nx.weakly_connected_components(G)) == 1
-        ), f"{PARANOIA_TYPE_ERROR}: individual is not a weakly connected graph"
+        ), f"{PARANOIA_TYPE_ERROR}: Individual is not a weakly connected graph"
 
         assert nx.is_branching(self.structure_tree) and nx.is_weakly_connected(
             self.structure_tree
-        ), f"{PARANOIA_VALUE_ERROR}: structure_tree of {self!r} is not a tree"
+        ), f"{PARANOIA_VALUE_ERROR}: Structure_tree of {self!r} is not a tree"
 
         assert set(self.genome.nodes) == set(
             self.structure_tree.nodes
-        ), f"{PARANOIA_VALUE_ERROR}: node mismatch with structure tree: {set(self.genome.nodes) ^ set(self.structure_tree.nodes)}"
+        ), f"{PARANOIA_VALUE_ERROR}: Node mismatch with structure tree: {set(self.genome.nodes) ^ set(self.structure_tree.nodes)}"
 
         # ==[check genome (fitness)]=========================================
         assert (self._fitness is None and not self.is_finalized) or (
             self._fitness is not None and self.is_finalized
         ), f"Value Error (paranoia check): Mismatch fitness and is_finalized"
 
         # ==[check edges (semantic)]=========================================
@@ -355,47 +355,47 @@
         ), "ValueError (paranoia check): unknown attribute in tree edge"
         tree_edges = [(u, v) for u, v, k, d in edges if d["_type"] == FRAMEWORK]
         assert len(tree_edges) == len(set(tree_edges)), "ValueError (paranoia check): duplicated framework edge"
 
         # ==[check nodes (semantic)]=========================================
         assert all(
             n < self._genome.graph["node_count"] for n in self._genome
-        ), f"{PARANOIA_VALUE_ERROR}: invalid 'node_count' attribute ({self._genome.graph['node_count']})"
+        ), f"{PARANOIA_VALUE_ERROR}: Invalid 'node_count' attribute ({self._genome.graph['node_count']})"
 
         assert all(
             '_selement' in d for n, d in self._genome.nodes(data=True)
-        ), f"{PARANOIA_VALUE_ERROR}: missing '_selement'"
+        ), f"{PARANOIA_VALUE_ERROR}: Missing '_selement'"
         assert all(
             (isinstance(d['_selement'], Macro) and d['_type'] == 'macro')
             or (isinstance(d['_selement'], FrameABC) and d['_type'] == 'frame')
             for n, d in self._genome.nodes(data=True)
         )
-        assert isinstance(self._genome.nodes[0]['_selement'], MacroZero), f"{PARANOIA_TYPE_ERROR}: incorrect NodeZero"
+        assert isinstance(self._genome.nodes[0]['_selement'], MacroZero), f"{PARANOIA_TYPE_ERROR}: Incorrect NodeZero"
 
         # ==[check structural parameter]=====================================
         assert all(
             p._node_reference == NodeReference(self._genome, n)
             for n in self._genome
             for p in self._genome.nodes[n].values()
             if isinstance(p, ParameterStructuralABC)
         ), f"{PARANOIA_VALUE_ERROR}: Incorrect node_reference in structural parameter"
 
         structural_edges = [(u, v, k) for u, v, k, d in self._genome.edges(data='_type', keys=True) if d == LINK]
         assert len(structural_edges) == len(set(k for u, v, k in structural_edges)), (
-            f"{PARANOIA_VALUE_ERROR}: found duplicated keys in structural edges: "
+            f"{PARANOIA_VALUE_ERROR}: Found duplicated keys in structural edges: "
             + f"{set(x for i, x in enumerate(list(k for u, v, k in structural_edges)) if i != list(k for u, v, k in structural_edges).index(x))}"
         )
         structural_parameters = [p for p in self.parameters if isinstance(p, ParameterStructuralABC)]
         assert len(structural_edges) == len(structural_parameters), (
-            f"{PARANOIA_VALUE_ERROR}: inconsistent number of structural edges: "
+            f"{PARANOIA_VALUE_ERROR}: Inconsistent number of structural edges: "
             + f"found {len(structural_edges)}, expecting {len(structural_parameters)}"
         )
         assert set(k for u, v, k in structural_edges) == set(
             p._key for p in structural_parameters
-        ), f"{PARANOIA_VALUE_ERROR}: inconsistent keys in structural edges"
+        ), f"{PARANOIA_VALUE_ERROR}: Inconsistent keys in structural edges"
 
         return True
 
     def describe(
         self,
         *,
         include_fitness: bool = True,
@@ -495,20 +495,22 @@
                 node_str += bag['_label'].format(**bag)
             if nr.graph.nodes[nr.node]['_type'] == MACRO_NODE:
                 node_str += '{_text_before_macro}'.format(**bag)
                 node_str += nr.graph.nodes[nr.node]['_selement'].dump(bag)
                 if bag['$dump_node_info'] and nr.node != NODE_ZERO:
                     if node_str:
                         node_str += '  '
-                    node_str += '{_comment} 🖋 {_node.path_string} ➜ {_node.selement}'.format(**bag)
+                    node_str += '{_comment} 🖋 {_node.path_string} ➜ {_node.selement.__class__}'.format(**bag)
                 node_str += '{_text_after_macro}'.format(**bag)
             elif nr.graph.nodes[nr.node]["_type"] == FRAME_NODE:
                 node_str += '{_text_before_frame}'.format(**bag)
                 if bag['$dump_node_info']:
-                    node_str += '{_comment} 🖋 {_node.path_string} ➜ {_node.selement}{_text_after_macro}'.format(**bag)
+                    node_str += (
+                        '{_comment} 🖋 {_node.path_string} ➜ {_node.selement.__class__}{_text_after_macro}'.format(**bag)
+                    )
                 node_str += '{_text_after_frame}'.format(**bag)
             node_str += '{_text_after_node}'.format(**bag)
             # ---------------------------------------------------------------
 
             if not bag['$omit_from_dump']:
                 phenotype += node_str
         # ===================================================================
@@ -541,20 +543,22 @@
         node_str = '{_text_before_node}'.format(**bag)
         if nr.graph.in_degree(nr.node) > 1:
             node_str += bag['_label'].format(**bag)
         if nr.graph.nodes[nr.node]['_type'] == MACRO_NODE:
             node_str += '{_text_before_macro}'.format(**bag)
             node_str += nr.graph.nodes[nr.node]['_selement'].dump(bag)
             if bag['$dump_node_info']:
-                node_str += '  {_comment} 🖋 {_node.path_string} ➜ {_node.selement}'.format(**bag)
+                node_str += '  {_comment} 🖋 {_node.path_string} ➜ {_node.selement.__class__}'.format(**bag)
             node_str += '{_text_after_macro}'.format(**bag)
         elif nr.graph.nodes[nr.node]['_type'] == FRAME_NODE:
             node_str += '{_text_before_frame}'.format(**bag)
             if bag['$dump_node_info']:
-                node_str += '{_comment} 🖋 {_node.path_string} ➜ {_node.selement}{_text_after_macro}'.format(**bag)
+                node_str += '{_comment} 🖋 {_node.path_string} ➜ {_node.selement.__class__}{_text_after_macro}'.format(
+                    **bag
+                )
             node_str += '{_text_after_frame}'.format(**bag)
         node_str += '{_text_after_node}'.format(**bag)
         # ====================================================================
 
         dump += node_str
         for n in [v for u, v in T.out_edges(nr.node)]:
             dump = Individual._dump_node_recursive(NodeReference(nr.graph, n), T, local_parameters, dump)
```

### Comparing `byron-0.8a1.dev8/byron/classes/monitor.py` & `byron-0.8a1.dev9/byron/classes/monitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #################################|###|#####################################
 #  __                            |   |                                    #
-# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.1    #
+# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.8    #
 # |  _  |  |  |   _|  _  |     | |___| An evolutionary optimizer & fuzzer #
 # |_____|___  |__| |_____|__|__|  ).(  https://pypi.org/project/byron/    #
 #       |_____|                   \|/                                     #
 ################################## ' ######################################
 
 # Copyright 2023 Giovanni Squillero and Alberto Tonda
 #
```

### Comparing `byron-0.8a1.dev8/byron/classes/node_reference.py` & `byron-0.8a1.dev9/byron/classes/node_reference.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #################################|###|#####################################
 #  __                            |   |                                    #
-# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.1    #
+# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.8    #
 # |  _  |  |  |   _|  _  |     | |___| An evolutionary optimizer & fuzzer #
 # |_____|___  |__| |_____|__|__|  ).(  https://pypi.org/project/byron/    #
 #       |_____|                   \|/                                     #
 ################################## ' ######################################
 
 # Copyright 2023 Giovanni Squillero and Alberto Tonda
 #
```

### Comparing `byron-0.8a1.dev8/byron/classes/node_view.py` & `byron-0.8a1.dev9/byron/classes/node_view.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #################################|###|#####################################
 #  __                            |   |                                    #
-# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.1    #
+# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.8    #
 # |  _  |  |  |   _|  _  |     | |___| An evolutionary optimizer & fuzzer #
 # |_____|___  |__| |_____|__|__|  ).(  https://pypi.org/project/byron/    #
 #       |_____|                   \|/                                     #
 ################################## ' ######################################
 
 # Copyright 2023 Giovanni Squillero and Alberto Tonda
 #
```

### Comparing `byron-0.8a1.dev8/byron/classes/parameter.py` & `byron-0.8a1.dev9/byron/classes/parameter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #################################|###|#####################################
 #  __                            |   |                                    #
-# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.1    #
+# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.8    #
 # |  _  |  |  |   _|  _  |     | |___| An evolutionary optimizer & fuzzer #
 # |_____|___  |__| |_____|__|__|  ).(  https://pypi.org/project/byron/    #
 #       |_____|                   \|/                                     #
 ################################## ' ######################################
 
 # Copyright 2023 Giovanni Squillero and Alberto Tonda
 #
@@ -35,15 +35,15 @@
 from byron.global_symbols import *
 from byron.user_messages import *
 from byron.classes.selement import SElement
 from byron.classes.paranoid import Paranoid
 from byron.classes.node_reference import NodeReference
 
 
-class ParameterABC(Paranoid, ABC):
+class ParameterABC(SElement, Paranoid):
     """Generic class for storing a Macro parameter"""
 
     __slots__ = []  # Preventing the automatic creation of __dict__
 
     COUNTER = 0
 
     def __init__(self):
@@ -72,15 +72,15 @@
 
     @property
     def value(self):
         return self._value
 
     @value.setter
     def value(self, new_value):
-        assert self.is_correct(new_value), f"{PARANOIA_VALUE_ERROR}: invalid value: {new_value}"
+        assert self.is_correct(new_value), f"{PARANOIA_VALUE_ERROR}: Invalid value: {new_value}"
         self._value = new_value
 
     @abstractmethod
     def mutate(self, strength: float = 1.0) -> None:
         pass
 
 
@@ -92,15 +92,15 @@
     pass
 
 
 class ParameterSharedABC(ParameterABC):
     pass
 
 
-class ParameterStructuralABC(ParameterABC, ABC):
+class ParameterStructuralABC(ParameterABC):
     """Generic class for storing a Macro structural parameter"""
 
     __slots__ = []  # Preventing the automatic creation of __dict__
 
     _node_reference: NodeReference | None
 
     def __init__(self):
@@ -115,31 +115,31 @@
         self._node_reference = node_reference
 
     def unfasten(self):
         self._node_reference = None
 
     @property
     def graph(self):
-        assert self.is_fastened, f"{PARANOIA_VALUE_ERROR}: structural parameter is not fastened"
+        assert self.is_fastened, f"{PARANOIA_VALUE_ERROR}: Structural parameter is not fastened"
         return self._node_reference.graph
 
     @property
     def node(self):
-        assert self.is_fastened, f"{PARANOIA_VALUE_ERROR}: structural parameter is not fastened"
+        assert self.is_fastened, f"{PARANOIA_VALUE_ERROR}: Structural parameter is not fastened"
         return self._node_reference.node
 
     @property
     def is_fastened(self) -> bool:
         return self._node_reference is not None
 
     @property
     def value(self):
         assert (
             self.is_fastened
-        ), f"{PARANOIA_VALUE_ERROR}: attempt to retrieve the value of an unfastened structural parameter"
+        ), f"{PARANOIA_VALUE_ERROR}: Attempt to retrieve the value of an unfastened structural parameter"
         if self._node_reference is None:
             return None
         return next(
             (v for u, v, k in self._node_reference.graph.edges(self._node_reference.node, keys=True) if k == self.key),
             None,
         )
```

### Comparing `byron-0.8a1.dev8/byron/classes/paranoid.py` & `byron-0.8a1.dev9/byron/classes/paranoid.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #################################|###|#####################################
 #  __                            |   |                                    #
-# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.1    #
+# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.8    #
 # |  _  |  |  |   _|  _  |     | |___| An evolutionary optimizer & fuzzer #
 # |_____|___  |__| |_____|__|__|  ).(  https://pypi.org/project/byron/    #
 #       |_____|                   \|/                                     #
 ################################## ' ######################################
 
 # Copyright 2023 Giovanni Squillero and Alberto Tonda
 #
```

### Comparing `byron-0.8a1.dev8/byron/classes/population.py` & `byron-0.8a1.dev9/byron/classes/population.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #################################|###|#####################################
 #  __                            |   |                                    #
-# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.1    #
+# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.8    #
 # |  _  |  |  |   _|  _  |     | |___| An evolutionary optimizer & fuzzer #
 # |_____|___  |__| |_____|__|__|  ).(  https://pypi.org/project/byron/    #
 #       |_____|                   \|/                                     #
 ################################## ' ######################################
 
 # Copyright 2023 Giovanni Squillero and Alberto Tonda
 #
```

### Comparing `byron-0.8a1.dev8/byron/classes/readymade_frames.py` & `byron-0.8a1.dev9/byron/user_messages/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #################################|###|#####################################
 #  __                            |   |                                    #
-# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.1    #
+# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.8    #
 # |  _  |  |  |   _|  _  |     | |___| An evolutionary optimizer & fuzzer #
 # |_____|___  |__| |_____|__|__|  ).(  https://pypi.org/project/byron/    #
 #       |_____|                   \|/                                     #
 ################################## ' ######################################
 
 # Copyright 2023 Giovanni Squillero and Alberto Tonda
 #
@@ -21,20 +21,10 @@
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # =[ HISTORY ]===============================================================
 # v1 / May 2023 / Squillero (GX)
 
-__all__ = ["SELF"]
-
-from .frame import FrameABC
-from byron.tools.names import canonize_name, _patch_class_info
-
-
-class SELF(FrameABC):
-    """Placeholder for the BNF frame."""
-
-    pass
-
-
-_patch_class_info(SELF, canonize_name("SELF", "Frame", make_unique=False, warn_duplicates=False), tag="framework")
+from byron.user_messages.exception import *
+from byron.user_messages.messaging import *
+from byron.user_messages.checks import *
```

### Comparing `byron-0.8a1.dev8/byron/classes/readymade_macros.py` & `byron-0.8a1.dev9/byron/classes/readymade_macros.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #################################|###|#####################################
 #  __                            |   |                                    #
-# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.1    #
+# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.8    #
 # |  _  |  |  |   _|  _  |     | |___| An evolutionary optimizer & fuzzer #
 # |_____|___  |__| |_____|__|__|  ).(  https://pypi.org/project/byron/    #
 #       |_____|                   \|/                                     #
 ################################## ' ######################################
 
 # Copyright 2023 Giovanni Squillero and Alberto Tonda
 #
@@ -31,15 +31,14 @@
 from datetime import datetime
 import platform
 
 import networkx as nx
 
 from byron.classes.macro import Macro
 from byron.global_symbols import *
-from byron.tools.names import canonize_name, _patch_class_info
 from byron.user_messages import *
 
 
 class MacroZero(Macro):
     TEXT = (
         "{_comment}"
         + f""" Automagically written by Byron v{__version__}"""
@@ -74,11 +73,9 @@
         return True
 
     @property
     def shannon(self) -> list[int]:
         return [hash(self.__class__)]
 
 
-_patch_class_info(
-    MacroZero, canonize_name("MacroZero", "Macro", make_unique=False, warn_duplicates=False), tag="framework"
-)
-_patch_class_info(Info, canonize_name("Info", "Macro", make_unique=False, warn_duplicates=False), tag="framework")
+MacroZero._patch_info()
+Info._patch_info()
```

### Comparing `byron-0.8a1.dev8/byron/classes/shared.py` & `byron-0.8a1.dev9/byron/classes/shared.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #################################|###|#####################################
 #  __                            |   |                                    #
-# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.1    #
+# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.8    #
 # |  _  |  |  |   _|  _  |     | |___| An evolutionary optimizer & fuzzer #
 # |_____|___  |__| |_____|__|__|  ).(  https://pypi.org/project/byron/    #
 #       |_____|                   \|/                                     #
 ################################## ' ######################################
 
 # Copyright 2023 Giovanni Squillero and Alberto Tonda
 #
```

### Comparing `byron-0.8a1.dev8/byron/classes/value_bag.py` & `byron-0.8a1.dev9/byron/classes/value_bag.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #################################|###|#####################################
 #  __                            |   |                                    #
-# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.1    #
+# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.8    #
 # |  _  |  |  |   _|  _  |     | |___| An evolutionary optimizer & fuzzer #
 # |_____|___  |__| |_____|__|__|  ).(  https://pypi.org/project/byron/    #
 #       |_____|                   \|/                                     #
 ################################## ' ######################################
 
 # Copyright 2023 Giovanni Squillero and Alberto Tonda
 #
```

### Comparing `byron-0.8a1.dev8/byron/ea/__init__.py` & `byron-0.8a1.dev9/byron/ea/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #################################|###|#####################################
 #  __                            |   |                                    #
-# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.1    #
+# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.8    #
 # |  _  |  |  |   _|  _  |     | |___| An evolutionary optimizer & fuzzer #
 # |_____|___  |__| |_____|__|__|  ).(  https://pypi.org/project/byron/    #
 #       |_____|                   \|/                                     #
 ################################## ' ######################################
 # Copyright 2022-2023 Giovanni Squillero and Alberto Tonda
 #
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
```

### Comparing `byron-0.8a1.dev8/byron/ea/check.py` & `byron-0.8a1.dev9/byron/ea/check.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #################################|###|#####################################
 #  __                            |   |                                    #
-# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.1    #
+# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.8    #
 # |  _  |  |  |   _|  _  |     | |___| An evolutionary optimizer & fuzzer #
 # |_____|___  |__| |_____|__|__|  ).(  https://pypi.org/project/byron/    #
 #       |_____|                   \|/                                     #
 ################################## ' ######################################
 # Copyright 2022-2023 Giovanni Squillero and Alberto Tonda
 #
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
```

### Comparing `byron-0.8a1.dev8/byron/ea/common.py` & `byron-0.8a1.dev9/byron/fitness_.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #################################|###|#####################################
 #  __                            |   |                                    #
-# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.1    #
+# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.8    #
 # |  _  |  |  |   _|  _  |     | |___| An evolutionary optimizer & fuzzer #
 # |_____|___  |__| |_____|__|__|  ).(  https://pypi.org/project/byron/    #
 #       |_____|                   \|/                                     #
 ################################## ' ######################################
 
 # Copyright 2023 Giovanni Squillero and Alberto Tonda
 #
@@ -19,10 +19,11 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # =[ HISTORY ]===============================================================
-# v1 / April 2023 / Squillero (GX)
+# v1 / May 2023 / Squillero (GX)
 
-__all__ = []
+from byron.classes.fitness import FitnessABC
+from byron.fitness import *
```

### Comparing `byron-0.8a1.dev8/byron/ea/parametric.py` & `byron-0.8a1.dev9/byron/ea/parametric.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #################################|###|#####################################
 #  __                            |   |                                    #
-# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.1    #
+# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.8    #
 # |  _  |  |  |   _|  _  |     | |___| An evolutionary optimizer & fuzzer #
 # |_____|___  |__| |_____|__|__|  ).(  https://pypi.org/project/byron/    #
 #       |_____|                   \|/                                     #
 ################################## ' ######################################
 
 # Copyright 2023 Giovanni Squillero and Alberto Tonda
 #
```

### Comparing `byron-0.8a1.dev8/byron/ea/selection.py` & `byron-0.8a1.dev9/byron/ea/selection.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #################################|###|#####################################
 #  __                            |   |                                    #
-# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.1    #
+# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.8    #
 # |  _  |  |  |   _|  _  |     | |___| An evolutionary optimizer & fuzzer #
 # |_____|___  |__| |_____|__|__|  ).(  https://pypi.org/project/byron/    #
 #       |_____|                   \|/                                     #
 ################################## ' ######################################
 # Copyright 2022-2023 Giovanni Squillero and Alberto Tonda
 #
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
```

### Comparing `byron-0.8a1.dev8/byron/ea/vanilla.py` & `byron-0.8a1.dev9/byron/ea/vanilla.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #################################|###|#####################################
 #  __                            |   |                                    #
-# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.1    #
+# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.8    #
 # |  _  |  |  |   _|  _  |     | |___| An evolutionary optimizer & fuzzer #
 # |_____|___  |__| |_____|__|__|  ).(  https://pypi.org/project/byron/    #
 #       |_____|                   \|/                                     #
 ################################## ' ######################################
 
 # Copyright 2023 Giovanni Squillero and Alberto Tonda
 #
```

### Comparing `byron-0.8a1.dev8/byron/evaluator_.py` & `byron-0.8a1.dev9/byron/evaluator_.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #################################|###|#####################################
 #  __                            |   |                                    #
-# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.1    #
+# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.8    #
 # |  _  |  |  |   _|  _  |     | |___| An evolutionary optimizer & fuzzer #
 # |_____|___  |__| |_____|__|__|  ).(  https://pypi.org/project/byron/    #
 #       |_____|                   \|/                                     #
 ################################## ' ######################################
 
 # Copyright 2023 Giovanni Squillero and Alberto Tonda
 #
```

### Comparing `byron-0.8a1.dev8/byron/fitness/__init__.py` & `byron-0.8a1.dev9/byron/fitness/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #################################|###|#####################################
 #  __                            |   |                                    #
-# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.1    #
+# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.8    #
 # |  _  |  |  |   _|  _  |     | |___| An evolutionary optimizer & fuzzer #
 # |_____|___  |__| |_____|__|__|  ).(  https://pypi.org/project/byron/    #
 #       |_____|                   \|/                                     #
 ################################## ' ######################################
 
 # Copyright 2023 Giovanni Squillero and Alberto Tonda
 #
```

### Comparing `byron-0.8a1.dev8/byron/fitness/basic.py` & `byron-0.8a1.dev9/byron/fitness/basic.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #################################|###|#####################################
 #  __                            |   |                                    #
-# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.1    #
+# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.8    #
 # |  _  |  |  |   _|  _  |     | |___| An evolutionary optimizer & fuzzer #
 # |_____|___  |__| |_____|__|__|  ).(  https://pypi.org/project/byron/    #
 #       |_____|                   \|/                                     #
 ################################## ' ######################################
 
 # Copyright 2023 Giovanni Squillero and Alberto Tonda
 #
@@ -82,18 +82,18 @@
         assert self.check_comparable(other)
         return self != other and float(self) > float(other)
 
     def check_comparable(self, other: "Scalar"):
         assert super().check_comparable(other)
         assert (
             not isinstance(other, self.__class__) or self._abs_tol == other._abs_tol
-        ), f"{PARANOIA_VALUE_ERROR}: different absolute tolerance: {float(self)}±{self._abs_tol} vs. {float(other)}±{other._abs_tol}"
+        ), f"{PARANOIA_VALUE_ERROR}: Different absolute tolerance: {float(self)}±{self._abs_tol} vs. {float(other)}±{other._abs_tol}"
         assert (
             not isinstance(other, self.__class__) or self._rel_tol == other._rel_tol
-        ), f"{PARANOIA_VALUE_ERROR}: different relative tolerance: {float(self)}±{self._rel_tol}r vs. {float(other)}±{other._rel_tol}r"
+        ), f"{PARANOIA_VALUE_ERROR}: Different relative tolerance: {float(self)}±{self._rel_tol}r vs. {float(other)}±{other._rel_tol}r"
         return True
 
 
 # VECTORS
 
 
 class Vector(FitnessABC):
@@ -160,19 +160,7 @@
     elif isinstance(data, Sequence):
         logger.warning(f"{data}")
         return Lexicographic(data)
     else:
         assert (
             isinstance(data, Sequence) or isinstance(data, int) or isinstance(data, float)
         ), f"TypeError: Can't convert {data!r} ({type()}) to Fitness"
-
-
-##############################################################################
-# Patch names
-# _patch_class_info(Scalar, 'Scalar', tag='fitness')
-# _patch_class_info(Integer, 'Integer', tag='fitness')
-# _patch_class_info(Float, 'Float', tag='fitness')
-# _patch_class_info(Vector, 'Vector', tag='fitness')
-# _patch_class_info(Lexicographic, 'Vector', tag='fitness')
-# _patch_class_info(ApproximateVector, 'VectorApproximate', tag='fitness')
-# _patch_class_info(IntegerVector, 'VectorInteger', tag='fitness')
-# _patch_class_info(ScalarVector, 'VectorScalar', tag='fitness')
```

### Comparing `byron-0.8a1.dev8/byron/fitness/reverse.py` & `byron-0.8a1.dev9/byron/fitness/reverse.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #################################|###|#####################################
 #  __                            |   |                                    #
-# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.1    #
+# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.8    #
 # |  _  |  |  |   _|  _  |     | |___| An evolutionary optimizer & fuzzer #
 # |_____|___  |__| |_____|__|__|  ).(  https://pypi.org/project/byron/    #
 #       |_____|                   \|/                                     #
 ################################## ' ######################################
 
 # Copyright 2023 Giovanni Squillero and Alberto Tonda
 #
@@ -28,15 +28,14 @@
 __all__ = ["reverse_fitness"]
 
 from abc import ABC, abstractmethod
 from functools import cache
 
 from byron.classes.fitness import FitnessABC
 from byron.user_messages import *
-from byron.tools.names import _patch_class_info
 
 
 @cache
 def reverse_fitness(fitness_class: type[FitnessABC]) -> type[FitnessABC]:
     """Reverse fitness class turning a maximization problem into a minimization one."""
     assert check_valid_type(fitness_class, FitnessABC, subclass=True)
 
@@ -53,10 +52,8 @@
             ), f"TypeError: different types of fitness: '{self.__class__}' and '{other.__class__}'"
             return super(T, other).is_dominant(self)
 
         def _decorate(self) -> str:
             # return 'ᴙ⟦' + fitness_class._decorate(self) + '⟧'
             return "ᴙ" + fitness_class._decorate(self)
 
-    _patch_class_info(T, f"reverse[{fitness_class.__name__}]", tag="fitness")
-
     return T
```

### Comparing `byron-0.8a1.dev8/byron/fitness_.py` & `byron-0.8a1.dev9/byron/randy/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #################################|###|#####################################
 #  __                            |   |                                    #
-# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.1    #
+# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.8    #
 # |  _  |  |  |   _|  _  |     | |___| An evolutionary optimizer & fuzzer #
 # |_____|___  |__| |_____|__|__|  ).(  https://pypi.org/project/byron/    #
 #       |_____|                   \|/                                     #
 ################################## ' ######################################
 
 # Copyright 2023 Giovanni Squillero and Alberto Tonda
 #
@@ -21,9 +21,12 @@
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # =[ HISTORY ]===============================================================
 # v1 / May 2023 / Squillero (GX)
 
-from byron.classes.fitness import FitnessABC
-from byron.fitness import *
+from .main import *
+
+assert "rrandom" not in globals(), f"SystemError (paranoia check): Randy the Random already initialized"
+rrandom = Randy(42)
+assert "rrandom" in globals(), f"SystemError (paranoia check): Randy the Random not initialized"
```

### Comparing `byron-0.8a1.dev8/byron/framework/__init__.py` & `byron-0.8a1.dev9/byron/framework/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #################################|###|#####################################
 #  __                            |   |                                    #
-# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.1    #
+# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.8    #
 # |  _  |  |  |   _|  _  |     | |___| An evolutionary optimizer & fuzzer #
 # |_____|___  |__| |_____|__|__|  ).(  https://pypi.org/project/byron/    #
 #       |_____|                   \|/                                     #
 ################################## ' ######################################
 
 # Copyright 2023 Giovanni Squillero and Alberto Tonda
 #
```

### Comparing `byron-0.8a1.dev8/byron/framework/bnf.py` & `byron-0.8a1.dev9/byron/framework/bnf.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #################################|###|#####################################
 #  __                            |   |                                    #
-# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.1    #
+# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.8    #
 # |  _  |  |  |   _|  _  |     | |___| An evolutionary optimizer & fuzzer #
 # |_____|___  |__| |_____|__|__|  ).(  https://pypi.org/project/byron/    #
 #       |_____|                   \|/                                     #
 ################################## ' ######################################
 
 # Copyright 2023 Giovanni Squillero and Alberto Tonda
 #
@@ -24,20 +24,19 @@
 
 # =[ HISTORY ]===============================================================
 # v1 / May 2023 / Squillero (GX)
 
 __all__ = ["bnf"]
 
 from byron.global_symbols import FRAMEWORK
-from byron.tools.names import _patch_class_info, FRAMEWORK_DIRECTORY
 from byron.classes.frame import FrameABC
 from byron.classes.selement import SElement
 from byron.classes.macro import Macro
 from byron.classes.readymade_frames import SELF
-from byron.tools.names import canonize_name, uncanonize_name
+from byron.tools.names import base_name
 from byron.framework.macro import macro
 
 from .framework import *
 
 
 def bnf(
     production: list[list[type[SElement] | type[Macro] | str]], name: str | None = None, extra_parameters: dict = None
@@ -103,22 +102,22 @@
     References
     ----------
     .. [1] https://en.wikipedia.org/wiki/Backus%E2%80%93Naur_form
     """
     derivations = list()
     for expression in production:
         frame = sequence(expression)
-        _patch_class_info(frame, canonize_name("BNF:" + uncanonize_name(frame.__name__), "Frame"), tag=FRAMEWORK)
+        frame._patch_info(name='BNF:' + base_name(frame.BYRON_CLASS_NAME) + '#')
         derivations.append(frame)
 
     root = alternative(derivations, extra_parameters=extra_parameters)
     if name:
-        _patch_class_info(root, canonize_name(name, "Frame", user=True), tag=FRAMEWORK)
+        root._patch_info(custom_class_id=name)
     else:
-        _patch_class_info(root, canonize_name("BNF", "Frame"), tag=FRAMEWORK)
+        root._patch_info(name="BNF#")
 
     # patch derivations to include a self reference
     for derivation in root.ALTERNATIVES:
         if SELF in derivation.SEQUENCE:
             derivation.SEQUENCE = tuple(f if f != SELF else root for f in derivation.SEQUENCE)
 
     return root
```

### Comparing `byron-0.8a1.dev8/byron/framework/defaults.py` & `byron-0.8a1.dev9/byron/framework/defaults.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,23 +51,23 @@
     *   `_text_before_macro`: Dumped before a node that encodes a macro (default ``''``)
     *   `_text_after_macro`: Dumped after a node that encodes a macro (default ``'\n'``)
     *   `_text_before_frame`: Dumped before a node that encodes a frame (default ``''``)
     *   `_text_after_frame`: Dumped after a node that encodes a frame (default ``''``)
 
     See `byron.DEFAULT_EXTRA_PARAMETERS` for the complete list of default parameters.
     """
-    assert re.fullmatch(r'_[a-z_0-9]+', key), f"{PARANOIA_VALUE_ERROR}: invalid key name {key}"
+    assert re.fullmatch(r'_[a-z_0-9]+', key), f"{PARANOIA_VALUE_ERROR}: Invalid key name {key}"
     DEFAULT_EXTRA_PARAMETERS[key] = value
 
 
 def set_option(key: str, value: Any) -> None:
     r"""Set the global default for a framework option
 
     Options name always start with dollar ``$``. They are boolean. The default for options is ``False``.
 
     *   `$dump_node_info`: Dump after each node a valid *line comment* with some information (useful for debug)
 
     See `byron.DEFAULT_OPTIONS` for the complete list of default parameters.
     """
 
-    assert re.fullmatch(r'\$[a-z_0-9]+', key), f"{PARANOIA_VALUE_ERROR}: invalid option name {key}"
+    assert re.fullmatch(r'\$[a-z_0-9]+', key), f"{PARANOIA_VALUE_ERROR}: Invalid option name {key}"
     DEFAULT_OPTIONS[key] = value
```

### Comparing `byron-0.8a1.dev8/byron/framework/framework.py` & `byron-0.8a1.dev9/byron/framework/framework.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #################################|###|#####################################
 #  __                            |   |                                    #
-# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.1    #
+# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.8    #
 # |  _  |  |  |   _|  _  |     | |___| An evolutionary optimizer & fuzzer #
 # |_____|___  |__| |_____|__|__|  ).(  https://pypi.org/project/byron/    #
 #       |_____|                   \|/                                     #
 ################################## ' ######################################
 
 # Copyright 2023 Giovanni Squillero and Alberto Tonda
 #
@@ -28,15 +28,14 @@
 __all__ = ["sequence", "alternative", "bunch"]
 
 from collections import abc
 from typing import Sequence
 
 from byron.global_symbols import *
 from byron.user_messages import *
-from byron.tools.names import canonize_name, _patch_class_info, FRAMEWORK_DIRECTORY
 from byron.classes.selement import SElement
 from byron.classes.frame import *
 from byron.classes.macro import Macro
 from byron.framework.macro import macro
 from byron.framework.utilities import cook_selement_list
 from byron.randy import rrandom
 
@@ -105,20 +104,18 @@
             super().__init__()
 
         @property
         def successors(self):
             return [rrandom.choice(T.ALTERNATIVES)]
 
     if name:
-        _patch_class_info(T, canonize_name(name, "Frame", user=True), tag=FRAMEWORK)
-        T.ID = name
+        T._patch_info(custom_class_id=name)
     else:
-        _patch_class_info(T, canonize_name("FrameAlternative", "Frame"), tag=FRAMEWORK)
+        T._patch_info(name="FrameAlternative#")
 
-    FRAMEWORK_DIRECTORY[T.ID] = T
     return T
 
 
 def sequence(
     seq: abc.Sequence[type[SElement] | str], *, name: str | None = None, extra_parameters: dict = None, **kwargs
 ) -> type[FrameABC]:
     cooked_seq = cook_selement_list(seq)
@@ -131,20 +128,20 @@
             super().__init__()
 
         @property
         def successors(self):
             return T.SEQUENCE
 
     if name:
-        _patch_class_info(T, canonize_name(name, "Frame", user=True), tag=FRAMEWORK)
-        T.ID = name
+        T._patch_info(custom_class_id=name)
+    elif len(cooked_seq) == 1:
+        T._patch_info(name="SingleFrame#")
     else:
-        _patch_class_info(T, canonize_name("FrameSequence", "Frame"), tag=FRAMEWORK)
+        T._patch_info(name="FrameSequence#")
 
-    FRAMEWORK_DIRECTORY[T.ID] = T
     return T
 
 
 def bunch(
     pool: Macro | abc.Collection[type[Macro]],
     size: tuple[int, int] | int = 1,
     *,
@@ -178,22 +175,22 @@
 
     original_size = size
     if isinstance(size, int):
         size = (size, size + 1)
     else:
         size = tuple(size)
         assert len(size) == 2, f"{PARANOIA_VALUE_ERROR}: Not a half open range [min, max)"
-    assert 0 <= size[0] < size[1], f"{PARANOIA_VALUE_ERROR}: min size is {size[0]} and max size is {size[1]-1}"
+    assert 0 <= size[0] < size[1], f"{PARANOIA_VALUE_ERROR}: Min size is {size[0]} and max size is {size[1]-1}"
 
     assert _debug_hints()
 
     if weights is None:
         weights = [1] * len(pool)
     else:
-        assert len(weights) == len(pool), f"{PARANOIA_VALUE_ERROR}: number of weights non coherent with pool size"
+        assert len(weights) == len(pool), f"{PARANOIA_VALUE_ERROR}: Number of weights non coherent with pool size"
 
     class T(FrameMacroBunch, FrameABC):
         SIZE = size
         POOL = tuple(sum(([m] * w for m, w in zip(pool, weights)), start=list()))
         EXTRA_PARAMETERS = dict(extra_parameters) if extra_parameters else dict()
 
         __slots__ = []  # Preventing the automatic creation of __dict__
@@ -209,19 +206,16 @@
     def check_out_degree(n):
         return n.out_degree >= size[0] and n.out_degree < size[1]
 
     T.add_node_check(check_out_degree)
 
     # White parentheses: ⦅ ⦆  (U+2985, U+2986)
     if name:
-        canonic_name = canonize_name(name, "Frame", user=True)
-        T.ID = name
+        T._patch_info(custom_class_id=name)
     elif size == (1, 2):
-        canonic_name = canonize_name("SingleMacro", "Frame")
+        T._patch_info(name='SingleMacro#')
     elif size[1] - size[0] == 1:
-        canonic_name = canonize_name("MacroArray", "Frame")
+        T._patch_info(name='MacroArray#')
     else:
-        canonic_name = canonize_name("MacroBunch", "Frame")
-    _patch_class_info(T, canonic_name, tag=FRAMEWORK)
+        T._patch_info(name='MacroBunch#')
 
-    FRAMEWORK_DIRECTORY[T.ID] = T
     return T
```

### Comparing `byron-0.8a1.dev8/byron/framework/macro.py` & `byron-0.8a1.dev9/byron/framework/macro.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #################################|###|#####################################
 #  __                            |   |                                    #
-# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.1    #
+# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.8    #
 # |  _  |  |  |   _|  _  |     | |___| An evolutionary optimizer & fuzzer #
 # |_____|___  |__| |_____|__|__|  ).(  https://pypi.org/project/byron/    #
 #       |_____|                   \|/                                     #
 ################################## ' ######################################
 
 # Copyright 2023 Giovanni Squillero and Alberto Tonda
 #
@@ -28,15 +28,14 @@
 __all__ = ["macro"]
 
 from functools import cache
 from typing import Any
 
 from byron.global_symbols import FRAMEWORK
 from byron.user_messages import *
-from byron.tools.names import canonize_name, _patch_class_info, FRAMEWORK_DIRECTORY
 from byron.classes.macro import Macro
 from byron.classes.parameter import ParameterABC
 
 
 @cache
 def _macro(
     text: str, macro_parameters: tuple[tuple[str, type[ParameterABC]]], extra_parameters: tuple[tuple[str, Any]]
@@ -45,19 +44,18 @@
         TEXT = text
         PARAMETERS = dict(macro_parameters)
         EXTRA_PARAMETERS = dict(extra_parameters) if extra_parameters else dict()
 
         __slots__ = []  # Preventing the automatic creation of __dict__
 
     if not macro_parameters:
-        _patch_class_info(M, canonize_name('Text', 'Macro'), tag=FRAMEWORK)
+        M._patch_info(name='Text#')
     else:
-        _patch_class_info(M, canonize_name('User', 'Macro'), tag=FRAMEWORK)
+        M._patch_info(name='User#')
 
-    FRAMEWORK_DIRECTORY[M.ID] = M
     return M
 
 
 def macro(text: str, **parameters: type[ParameterABC] | str) -> type[Macro]:
     """Class factory: Returns the class for a specific macro.
 
     A macro is a fragment of text with variable elements, the `parameters`, appearing
```

### Comparing `byron-0.8a1.dev8/byron/framework/parameter.py` & `byron-0.8a1.dev9/byron/framework/parameter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #################################|###|#####################################
 #  __                            |   |                                    #
-# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.1    #
+# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.8    #
 # |  _  |  |  |   _|  _  |     | |___| An evolutionary optimizer & fuzzer #
 # |_____|___  |__| |_____|__|__|  ).(  https://pypi.org/project/byron/    #
 #       |_____|                   \|/                                     #
 ################################## ' ######################################
 
 # Copyright 2023 Giovanni Squillero and Alberto Tonda
 #
@@ -29,15 +29,14 @@
 
 from collections.abc import Collection
 from functools import cache
 from numbers import Number
 from typing import Any, Hashable, SupportsInt
 
 from byron.user_messages import *
-from byron.tools.names import _patch_class_info
 from byron.classes.parameter import *
 from byron.randy import rrandom
 
 
 @cache
 def _numeric(*, type_, min_, max_):
     class T(ParameterNumericABC):
@@ -72,19 +71,19 @@
                 if strength == 1.0:
                     self.value = rrandom.random_float(min_, max_)
                 else:
                     self.value = rrandom.random_float(min_, max_, loc=self._value, strength=strength)
 
     if type_ == int and min_ == 0 and any(max_ == 2**n for n in range(4, 128 + 1)):
         p = next(n for n in range(4, 128 + 1) if max_ == 2**n)
-        _patch_class_info(T, f'{type_.__name__.title()}[{p}bit]', tag='parameter')
+        T._patch_info(name=f'{type_.__name__.title()}[{p}bit]')
     elif type_ == int:
-        _patch_class_info(T, f'{type_.__name__.title()}[{min_}..{max_-1}]', tag='parameter')
+        T._patch_info(name=f'{type_.__name__.title()}[{min_}..{max_ - 1}]')
     else:
-        _patch_class_info(T, f'{type_.__name__.title()}[{min_}–{max_})', tag='parameter')
+        T._patch_info(name=f'{type_.__name__.title()}[{min_}–{max_})')
     return T
 
 
 def integer_parameter(min_: int, max_: int) -> type[ParameterABC]:
     r"""An Int parameter: an integer number in the half-open range [min_, max_)."""
 
     def check_range():
@@ -147,15 +146,15 @@
         def mutate(self, strength: float = 1.0) -> None:
             if strength == 1.0:
                 self.value = rrandom.choice(alternatives)
             else:
                 self.value = rrandom.choice(alternatives, loc=alternatives.index(self._value), sigma=strength)
 
     # NOTE[GX]: alternative symbol: – (not a minus!)
-    _patch_class_info(T, 'Choice[' + '┊'.join(str(a) for a in alternatives) + ']', tag='parameter')
+    T._patch_info(name='Choice[' + '┊'.join(str(a) for a in alternatives) + ']')
     return T
 
 
 def choice_parameter(alternatives: Collection[Hashable]) -> type[ParameterABC]:
     r"""A Choice parameter: an element from a fixed list of alternatives."""
 
     def check_size():
@@ -206,15 +205,15 @@
         def mutate(self, strength: float = 1.0) -> None:
             if strength == 1:
                 new_value = [rrandom.choice(symbols) for _ in range(length)]
             else:
                 new_value = [rrandom.choice(symbols) if rrandom.boolean(strength) else old for old in self._value]
             self.value = "".join(new_value)
 
-    _patch_class_info(T, "Array[" + "".join(str(a) for a in symbols) + f"ｘ{length}]", tag="parameter")
+    T._patch_info(name="Array[" + "".join(str(a) for a in symbols) + f"ｘ{length}]")
     return T
 
 
 def array_parameter(symbols: Collection[str], length: SupportsInt) -> type[ParameterABC]:
     r"""An Array parameter: a fixed-length array of symbols."""
 
     assert check_valid_type(symbols, Collection)
@@ -242,9 +241,9 @@
         def is_correct(self, obj: Any) -> bool:
             return True
 
         def mutate(self, strength: float = 1.0) -> None:
             T.COUNTER += 1
             self.value = T.COUNTER
 
-    _patch_class_info(T, 'Counter[]', tag='parameter')
+    T._patch_info(name='Counter[]')
     return T
```

### Comparing `byron-0.8a1.dev8/byron/framework/parameter_structural_global.py` & `byron-0.8a1.dev9/byron/framework/parameter_structural_global.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #################################|###|#####################################
 #  __                            |   |                                    #
-# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.1    #
+# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.8    #
 # |  _  |  |  |   _|  _  |     | |___| An evolutionary optimizer & fuzzer #
 # |_____|___  |__| |_____|__|__|  ).(  https://pypi.org/project/byron/    #
 #       |_____|                   \|/                                     #
 ################################## ' ######################################
 
 # Copyright 2023 Giovanni Squillero and Alberto Tonda
 #
@@ -33,19 +33,18 @@
 
 from byron.user_messages import *
 from byron.randy import rrandom
 from byron.global_symbols import *
 
 from byron.classes.parameter import ParameterStructuralABC
 from byron.operators.unroll import *
-from byron.classes.selement import SElement
+from byron.classes.selement import SElement, SElementMeta
 from byron.tools.names import *
 
 from byron.tools.graph import *
-from byron.tools.names import canonize_name, _patch_class_info
 
 __all__ = ["global_reference"]
 
 
 @cache
 def _global_reference(
     *,
@@ -53,25 +52,18 @@
     target_frame: type[SElement] | None = None,
     first_macro: bool = True,
     creative_zeal: Number = 0,
 ) -> type[ParameterStructuralABC]:
     class T(ParameterStructuralABC):
         __slots__ = ["_target_frame"]  # Preventing the automatic creation of __dict__
 
-        if isinstance(target_frame, str):
-
-            def __init__(self):
-                super().__init__()
-                self._target_frame = FRAMEWORK_DIRECTORY[target_frame]
-
-        else:
-
-            def __init__(self):
-                super().__init__()
-                self._target_frame = target_frame
+        def __init__(self):
+            super().__init__()
+            # NOTE[GX] if target_frame is a string it works thanks to selement string magic!
+            self._target_frame = target_frame
 
         def get_potential_targets(self, add_none=True):
             G = self._node_reference.graph
             suitable_frames = [
                 n for n in nx.dfs_preorder_nodes(G) if G.nodes[n]['_selement'].__class__ == self._target_frame
             ]
             if first_macro:
@@ -97,15 +89,15 @@
                 targets = [None]
 
             if not targets:
                 raise ByronOperatorFailure
             return targets
 
         def mutate(self, strength: float = 1.0) -> None:
-            assert self.is_fastened, f"{PARANOIA_VALUE_ERROR}: node is unfastened"
+            assert self.is_fastened, f"{PARANOIA_VALUE_ERROR}: Node is unfastened"
 
             # first try
             potential_targets = self.get_potential_targets()
             if strength == 1.0:
                 target = rrandom.choice(potential_targets)
             else:
                 target = rrandom.choice(potential_targets, self.value, sigma=strength)
@@ -127,17 +119,17 @@
                 raise ByronOperatorFailure
             self.value = target
             for ccomp in list(nx.weakly_connected_components(self.graph)):
                 if NODE_ZERO not in ccomp:
                     self.self.graph.remove_nodes_from(ccomp)
 
     if isinstance(target_frame, str):
-        _patch_class_info(T, f"GlobalReference['{target_frame}']", tag="parameter")
+        T._patch_info(name=f"GlobalReference['{target_frame}']")
     else:
-        _patch_class_info(T, f"GlobalReference[{target_frame.__name__}]", tag="parameter")
+        T._patch_info(name=f"GlobalReference[{target_frame}]")
     return T
 
 
 def global_reference(
     target_frame: str | type[SElement], *, creative_zeal=0, first_macro: bool = False
 ) -> type[ParameterStructuralABC]:
     assert (
```

### Comparing `byron-0.8a1.dev8/byron/framework/parameter_structural_local.py` & `byron-0.8a1.dev9/byron/framework/parameter_structural_local.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #################################|###|#####################################
 #  __                            |   |                                    #
-# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.1    #
+# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.8    #
 # |  _  |  |  |   _|  _  |     | |___| An evolutionary optimizer & fuzzer #
 # |_____|___  |__| |_____|__|__|  ).(  https://pypi.org/project/byron/    #
 #       |_____|                   \|/                                     #
 ################################## ' ######################################
 
 # Copyright 2023 Giovanni Squillero and Alberto Tonda
 #
@@ -32,15 +32,14 @@
 from byron.global_symbols import *
 
 from byron.classes.parameter import ParameterStructuralABC
 from byron.classes.node_reference import NodeReference
 from byron.randy import rrandom
 
 from byron.tools.graph import *
-from byron.tools.names import canonize_name, _patch_class_info
 
 __all__ = ["local_reference"]
 
 
 @cache
 def _local_reference(
     backward: bool = True, self_loop: bool = True, forward: bool = True
@@ -84,18 +83,17 @@
                 raise ByronOperatorFailure
 
             if strength == 1 or self.value is None:
                 self.value = rrandom.choice(pt, None)
             else:
                 self.value = rrandom.sigmachoice(pt, pt.index(self.value), strength)
 
-    _patch_class_info(
-        T,
-        f"""LocalReference[{'<' if backward else '≮'}{'=' if self_loop else '≠'}{'>' if forward else '≯'}]""",
-        tag="parameter",
+    T._patch_info(
+        name=f"LocalReference[{'<' if backward else '≮'}{'=' if self_loop else '≠'}{'>' if forward else '≯'}]"
     )
+
     return T
 
 
 def local_reference(backward: bool = True, loop: bool = True, forward: bool = True) -> type[ParameterStructuralABC]:
     # TODO: Add checks
     return _local_reference(bool(backward), bool(loop), bool(forward))
```

### Comparing `byron-0.8a1.dev8/byron/framework/shared.py` & `byron-0.8a1.dev9/byron/framework/shared.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #################################|###|#####################################
 #  __                            |   |                                    #
-# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.1    #
+# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.8    #
 # |  _  |  |  |   _|  _  |     | |___| An evolutionary optimizer & fuzzer #
 # |_____|___  |__| |_____|__|__|  ).(  https://pypi.org/project/byron/    #
 #       |_____|                   \|/                                     #
 ################################## ' ######################################
 
 # Copyright 2023 Giovanni Squillero and Alberto Tonda
 #
@@ -25,15 +25,14 @@
 # =[ HISTORY ]===============================================================
 # v1 / May 2023 / Squillero (GX)
 
 __all__ = ["make_shared_parameter"]
 
 from typing import Any
 from byron.classes.parameter import *
-from byron.tools.names import _patch_class_info
 
 # MAKE KEY (TODO!!!)
 _parameters = set()
 
 
 def make_shared_parameter(parameter: type[ParameterABC]) -> type[ParameterABC]:
     parameter_instance = parameter()
@@ -62,9 +61,9 @@
         def mutate(self, strength: float = 1.0) -> None:
             if self.is_owner:
                 parameter_instance.mutate(strength)
 
         def is_correct(self, obj: Any) -> bool:
             return parameter_instance.is_correct(obj)
 
-    _patch_class_info(T, f"Shared❬{parameter_instance.__class__.__name__}❭", tag="parameter")
+    T._patch_info(name=f"Shared❬{parameter_instance.__class__.__name__}❭")
     return T
```

### Comparing `byron-0.8a1.dev8/byron/framework/show_element.py` & `byron-0.8a1.dev9/byron/framework/show_element.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #################################|###|#####################################
 #  __                            |   |                                    #
-# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.1    #
+# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.8    #
 # |  _  |  |  |   _|  _  |     | |___| An evolutionary optimizer & fuzzer #
 # |_____|___  |__| |_____|__|__|  ).(  https://pypi.org/project/byron/    #
 #       |_____|                   \|/                                     #
 ################################## ' ######################################
 
 # Copyright 2023 Giovanni Squillero and Alberto Tonda
 #
@@ -42,17 +42,15 @@
 def as_text(
     element: type[SElement] | ParameterABC,
     *,
     seed: int | None = 42,
     node_info: bool = True,
     extra_parameters: dict | None = None,
 ):
-    if isinstance(element, type) and issubclass(element, SElement):
-        frame = element
-    elif isinstance(element, type) and issubclass(element, ParameterABC):
+    if isinstance(element, type) and issubclass(element, ParameterABC):
         frame = macro(
             '{p1.__class__}\n'
             + '• {p1}\n'
             + '• {p2}\n'
             + '• {p3}\n'
             + '• {p4}\n'
             + '• {p5}\n'
@@ -65,14 +63,16 @@
             p4=element,
             p5=element,
             p6=element,
             p7=element,
             p8=element,
         )
         node_info = False
+    elif isinstance(element, type) and issubclass(element, SElement):
+        frame = element
     else:
         raise NotImplementedError(f"{__name__}.as_text({element!r})")
     individual = _generate_random_individual(frame, seed=seed)
 
     if extra_parameters is None:
         extra_parameters = dict()
     parameters = DEFAULT_EXTRA_PARAMETERS | DEFAULT_OPTIONS | extra_parameters
```

### Comparing `byron-0.8a1.dev8/byron/framework/utilities.py` & `byron-0.8a1.dev9/byron/framework/utilities.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #################################|###|#####################################
 #  __                            |   |                                    #
-# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.1    #
+# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.8    #
 # |  _  |  |  |   _|  _  |     | |___| An evolutionary optimizer & fuzzer #
 # |_____|___  |__| |_____|__|__|  ).(  https://pypi.org/project/byron/    #
 #       |_____|                   \|/                                     #
 ################################## ' ######################################
 
 # Copyright 2023 Giovanni Squillero and Alberto Tonda
 #
```

### Comparing `byron-0.8a1.dev8/byron/functions.py` & `byron-0.8a1.dev9/byron/functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #################################|###|#####################################
 #  __                            |   |                                    #
-# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.1    #
+# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.8    #
 # |  _  |  |  |   _|  _  |     | |___| An evolutionary optimizer & fuzzer #
 # |_____|___  |__| |_____|__|__|  ).(  https://pypi.org/project/byron/    #
 #       |_____|                   \|/                                     #
 ################################## ' ######################################
 # Copyright 2022-2023 Giovanni Squillero and Alberto Tonda
 #
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
```

### Comparing `byron-0.8a1.dev8/byron/global_symbols.py` & `byron-0.8a1.dev9/byron/global_symbols.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #################################|###|#####################################
 #  __                            |   |                                    #
-# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.1    #
+# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.8    #
 # |  _  |  |  |   _|  _  |     | |___| An evolutionary optimizer & fuzzer #
 # |_____|___  |__| |_____|__|__|  ).(  https://pypi.org/project/byron/    #
 #       |_____|                   \|/                                     #
 ################################## ' ######################################
 
 # Copyright 2023 Giovanni Squillero and Alberto Tonda
 #
@@ -63,16 +63,16 @@
 import sys
 import time
 from collections import defaultdict
 
 import multiprocessing
 import re
 
-__version__ = "0.8a1.dev8"
-__date__ = "21-08-2023"
+__version__ = "0.8a1.dev9"
+__date__ = "22-08-2023"
 __codename__ = "Don Juan"
 __author__ = "Giovanni Squillero and Alberto Tonda"
 __copyright__ = "Copyright (c) 2023 Giovanni Squillero and Alberto Tonda"
 
 #####################################################################################################################
 # Auto-detected "modes"
```

### Comparing `byron-0.8a1.dev8/byron/operators/__init__.py` & `byron-0.8a1.dev9/byron/operators/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #################################|###|#####################################
 #  __                            |   |                                    #
-# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.1    #
+# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.8    #
 # |  _  |  |  |   _|  _  |     | |___| An evolutionary optimizer & fuzzer #
 # |_____|___  |__| |_____|__|__|  ).(  https://pypi.org/project/byron/    #
 #       |_____|                   \|/                                     #
 ################################## ' ######################################
 # Copyright 2022-2023 Giovanni Squillero and Alberto Tonda
 #
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
```

### Comparing `byron-0.8a1.dev8/byron/operators/_graph_crossover.py` & `byron-0.8a1.dev9/byron/operators/_graph_crossover.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #################################|###|#####################################
 #  __                            |   |                                    #
-# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.1    #
+# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.8    #
 # |  _  |  |  |   _|  _  |     | |___| An evolutionary optimizer & fuzzer #
 # |_____|___  |__| |_____|__|__|  ).(  https://pypi.org/project/byron/    #
 #       |_____|                   \|/                                     #
 ################################## ' ######################################
 # Copyright 2022-2023 Giovanni Squillero and Alberto Tonda
 #
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
```

### Comparing `byron-0.8a1.dev8/byron/operators/initializers.py` & `byron-0.8a1.dev9/byron/operators/initializers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #################################|###|#####################################
 #  __                            |   |                                    #
-# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.1    #
+# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.8    #
 # |  _  |  |  |   _|  _  |     | |___| An evolutionary optimizer & fuzzer #
 # |_____|___  |__| |_____|__|__|  ).(  https://pypi.org/project/byron/    #
 #       |_____|                   \|/                                     #
 ################################## ' ######################################
 # Copyright 2022-2023 Giovanni Squillero and Alberto Tonda
 #
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
```

### Comparing `byron-0.8a1.dev8/byron/operators/mutation.py` & `byron-0.8a1.dev9/byron/operators/mutation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #################################|###|#####################################
 #  __                            |   |                                    #
-# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.1    #
+# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.8    #
 # |  _  |  |  |   _|  _  |     | |___| An evolutionary optimizer & fuzzer #
 # |_____|___  |__| |_____|__|__|  ).(  https://pypi.org/project/byron/    #
 #       |_____|                   \|/                                     #
 ################################## ' ######################################
 # Copyright 2022-2023 Giovanni Squillero and Alberto Tonda
 #
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
```

### Comparing `byron-0.8a1.dev8/byron/operators/parameter_crossover.py` & `byron-0.8a1.dev9/byron/operators/parameter_crossover.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #################################|###|#####################################
 #  __                            |   |                                    #
-# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.1    #
+# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.8    #
 # |  _  |  |  |   _|  _  |     | |___| An evolutionary optimizer & fuzzer #
 # |_____|___  |__| |_____|__|__|  ).(  https://github.com/squillero/byron #
 #       |_____|                   \|/                                     #
 ################################## ' ######################################
 
 # Copyright 2023 Giovanni Squillero and Alberto Tonda
 #
```

### Comparing `byron-0.8a1.dev8/byron/operators/tools.py` & `byron-0.8a1.dev9/byron/operators/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #################################|###|#####################################
 #  __                            |   |                                    #
-# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.1    #
+# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.8    #
 # |  _  |  |  |   _|  _  |     | |___| An evolutionary optimizer & fuzzer #
 # |_____|___  |__| |_____|__|__|  ).(  https://github.com/squillero/byron #
 #       |_____|                   \|/                                     #
 ################################## ' ######################################
 
 # Copyright 2023 Giovanni Squillero and Alberto Tonda
 #
```

### Comparing `byron-0.8a1.dev8/byron/operators/unroll.py` & `byron-0.8a1.dev9/byron/operators/unroll.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #################################|###|#####################################
 #  __                            |   |                                    #
-# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.1    #
+# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.8    #
 # |  _  |  |  |   _|  _  |     | |___| An evolutionary optimizer & fuzzer #
 # |_____|___  |__| |_____|__|__|  ).(  https://pypi.org/project/byron/    #
 #       |_____|                   \|/                                     #
 ################################## ' ######################################
 
 # Copyright 2023 Giovanni Squillero and Alberto Tonda
 #
@@ -54,15 +54,15 @@
 
     Returns:
         The root of the new subtree (an int)
     """
 
     assert check_valid_types(individual, Individual)
     assert check_valid_types(top, FrameABC, Macro, subclass=True)
-    assert not individual.is_finalized, f"{PARANOIA_VALUE_ERROR}: individual is finalized"
+    assert not individual.is_finalized, f"{PARANOIA_VALUE_ERROR}: Individual is finalized"
 
     G = individual.genome
     new_node_reference = unroll_selement(top, G)
     if not new_node_reference:
         return None
     G.add_edge(NODE_ZERO, new_node_reference.node, _type=FRAMEWORK)
     initialize_subtree(new_node_reference)
```

### Comparing `byron-0.8a1.dev8/byron/randy/__init__.py` & `byron-0.8a1.dev9/byron/classes/readymade_frames.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #################################|###|#####################################
 #  __                            |   |                                    #
-# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.1    #
+# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.8    #
 # |  _  |  |  |   _|  _  |     | |___| An evolutionary optimizer & fuzzer #
 # |_____|___  |__| |_____|__|__|  ).(  https://pypi.org/project/byron/    #
 #       |_____|                   \|/                                     #
 ################################## ' ######################################
 
 # Copyright 2023 Giovanni Squillero and Alberto Tonda
 #
@@ -21,12 +21,20 @@
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # =[ HISTORY ]===============================================================
 # v1 / May 2023 / Squillero (GX)
 
-from .main import *
+__all__ = ["SELF"]
 
-assert "rrandom" not in globals(), f"SystemError (paranoia check): Randy the Random already initialized"
-rrandom = Randy(42)
-assert "rrandom" in globals(), f"SystemError (paranoia check): Randy the Random not initialized"
+from byron.global_symbols import *
+from .frame import FrameABC
+
+
+class SELF(FrameABC):
+    """Placeholder for the BNF frame."""
+
+    pass
+
+
+SELF._patch_info()
```

### Comparing `byron-0.8a1.dev8/byron/randy/main.py` & `byron-0.8a1.dev9/byron/randy/main.py`

 * *Files identical despite different names*

### Comparing `byron-0.8a1.dev8/byron/registry.py` & `byron-0.8a1.dev9/byron/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #################################|###|#####################################
 #  __                            |   |                                    #
-# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.1    #
+# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.8    #
 # |  _  |  |  |   _|  _  |     | |___| An evolutionary optimizer & fuzzer #
 # |_____|___  |__| |_____|__|__|  ).(  https://pypi.org/project/byron/    #
 #       |_____|                   \|/                                     #
 ################################## ' ######################################
 
 # Copyright 2023 Giovanni Squillero and Alberto Tonda
 #
@@ -156,16 +156,14 @@
                 p.name for p in signature(func).parameters.values()
             ), f"TypeError: invalid signature for a genetic operator '{func.__name__}{signature(func)}'"
 
         @wraps(func)
         def wrapper(*args: Individual, **kwargs):
             wrapper.stats.calls += 1
 
-            logger.debug(f"genetic_operator: {func.__name__}({', '.join(str(_) for _ in args)})")
-
             try:
                 offspring = func(*args, **kwargs)
             except ByronOperatorFailure:
                 offspring = list()
 
             if offspring is None:
                 offspring = []
```

### Comparing `byron-0.8a1.dev8/byron/sys.py` & `byron-0.8a1.dev9/byron/sys.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #################################|###|#####################################
 #  __                            |   |                                    #
-# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.1    #
+# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.8    #
 # |  _  |  |  |   _|  _  |     | |___| An evolutionary optimizer & fuzzer #
 # |_____|___  |__| |_____|__|__|  ).(  https://pypi.org/project/byron/    #
 #       |_____|                   \|/                                     #
 ################################## ' ######################################
 
 # Copyright 2023 Giovanni Squillero and Alberto Tonda
 #
@@ -25,15 +25,15 @@
 # =[ HISTORY ]===============================================================
 # v1 / June 2023 / Squillero (GX)
 
 """Information about the current system.
 Mostly useful in interactive environments such as a Jupyter Notebook.
 """
 
-__all__ = ['get_operators', 'log_operators']
+__all__ = ['get_operators', 'log_operators', 'SYSINFO']
 
 import inspect
 from pprint import pformat
 from byron.operators import *
 
 
 class View:
@@ -120,8 +120,8 @@
     for op in all_ops:
         name = f'{op.__name__} ({descr[op.num_parents]})'
         logger.info(f"[blue]*[/blue] {name:.<50s}: {op.stats}")
 
 
 assert "SYSINFO" not in globals(), f"SystemError (paranoia check): SYSINFO already initialized."
 SYSINFO = SysInfo()
-assert "SYSINFO" in globals(), f"SystemError (paranoia check): FRAMEWORK_DIRECTORY not initialized."
+assert "SYSINFO" in globals(), f"SystemError (paranoia check): SYSINFO not initialized."
```

### Comparing `byron-0.8a1.dev8/byron/tools/entropy.py` & `byron-0.8a1.dev9/byron/tools/entropy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #################################|###|#####################################
 #  __                            |   |                                    #
-# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.1    #
+# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.8    #
 # |  _  |  |  |   _|  _  |     | |___| An evolutionary optimizer & fuzzer #
 # |_____|___  |__| |_____|__|__|  ).(  https://github.com/squillero/byron #
 #       |_____|                   \|/                                     #
 ################################## ' ######################################
 
 # Copyright 2023 Giovanni Squillero and Alberto Tonda
 #
```

### Comparing `byron-0.8a1.dev8/byron/tools/graph.py` & `byron-0.8a1.dev9/byron/tools/graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #################################|###|#####################################
 #  __                            |   |                                    #
-# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.1    #
+# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.8    #
 # |  _  |  |  |   _|  _  |     | |___| An evolutionary optimizer & fuzzer #
 # |_____|___  |__| |_____|__|__|  ).(  https://pypi.org/project/byron/    #
 #       |_____|                   \|/                                     #
 ################################## ' ######################################
 
 # Copyright 2023 Giovanni Squillero and Alberto Tonda
 #
@@ -84,15 +84,15 @@
 def set_successors_order(ref: NodeReference, new_order: Sequence[int]) -> None:
     assert check_valid_type(new_order, Sequence)
     G = ref.graph
     current = list((u, v, k) for u, v, k, d in G.out_edges(ref.node, keys=True, data="_type") if d == FRAMEWORK)
     assert all(k == 0 for u, v, k in current), f"ValueError: Found a FRAMEWORK edge with key != 0."
     assert {v for u, v, k in current} == set(
         new_order
-    ), f"{PARANOIA_VALUE_ERROR}: mismatching new order: {[v for u, v, k in current]} vs. {new_order}."
+    ), f"{PARANOIA_VALUE_ERROR}: Mismatching new order: {[v for u, v, k in current]} vs. {new_order}."
 
     attributes = dict()
     for u, v, k in current:
         attributes[(u, v)] = G.edges[u, v, k]  # save all attributes
         G.remove_edge(u, v, k)
     for v in new_order:
         G.add_edge(ref.node, v, **attributes[(u, v)])  # replace all attributes
```

### Comparing `byron-0.8a1.dev8/byron/tools/node_to_string.py` & `byron-0.8a1.dev9/byron/tools/node_to_string.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #################################|###|#####################################
 #  __                            |   |                                    #
-# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.1    #
+# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.8    #
 # |  _  |  |  |   _|  _  |     | |___| An evolutionary optimizer & fuzzer #
 # |_____|___  |__| |_____|__|__|  ).(  https://github.com/squillero/byron #
 #       |_____|                   \|/                                     #
 ################################## ' ######################################
 
 # Copyright 2023 Giovanni Squillero and Alberto Tonda
 #
```

### Comparing `byron-0.8a1.dev8/byron/user_messages/checks.py` & `byron-0.8a1.dev9/byron/user_messages/checks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #################################|###|#####################################
 #  __                            |   |                                    #
-# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.1    #
+# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.8    #
 # |  _  |  |  |   _|  _  |     | |___| An evolutionary optimizer & fuzzer #
 # |_____|___  |__| |_____|__|__|  ).(  https://pypi.org/project/byron/    #
 #       |_____|                   \|/                                     #
 ################################## ' ######################################
 
 # Copyright 2023 Giovanni Squillero and Alberto Tonda
 #
```

### Comparing `byron-0.8a1.dev8/byron/user_messages/exception.py` & `byron-0.8a1.dev9/byron/user_messages/exception.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #################################|###|#####################################
 #  __                            |   |                                    #
-# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.1    #
+# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.8    #
 # |  _  |  |  |   _|  _  |     | |___| An evolutionary optimizer & fuzzer #
 # |_____|___  |__| |_____|__|__|  ).(  https://pypi.org/project/byron/    #
 #       |_____|                   \|/                                     #
 ################################## ' ######################################
 
 # Copyright 2023 Giovanni Squillero and Alberto Tonda
 #
```

### Comparing `byron-0.8a1.dev8/byron/user_messages/messaging.py` & `byron-0.8a1.dev9/byron/user_messages/messaging.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #################################|###|#####################################
 #  __                            |   |                                    #
-# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.1    #
+# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.8    #
 # |  _  |  |  |   _|  _  |     | |___| An evolutionary optimizer & fuzzer #
 # |_____|___  |__| |_____|__|__|  ).(  https://pypi.org/project/byron/    #
 #       |_____|                   \|/                                     #
 ################################## ' ######################################
 
 # Copyright 2023 Giovanni Squillero and Alberto Tonda
 #
```

### Comparing `byron-0.8a1.dev8/docs/pypi.md` & `byron-0.8a1.dev9/docs/pypi.md`

 * *Files identical despite different names*

### Comparing `byron-0.8a1.dev8/pyproject.toml` & `byron-0.8a1.dev9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #################################|###|#####################################
 #  __                            |   |                                    #
-# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.1    #
+# |  |--.--.--.----.-----.-----. |===| This file is part of Byron v0.8    #
 # |  _  |  |  |   _|  _  |     | |___| An evolutionary optimizer & fuzzer #
 # |_____|___  |__| |_____|__|__|  ).(  https://pypi.org/project/byron/    #
 #       |_____|                   \|/                                     #
 ################################## ' ######################################
 # Copyright 2023 Giovanni Squillero and Alberto Tonda
 # SPDX-License-Identifier: Apache-2.0
 
 [tool.poetry]
 name = "byron"
-version = "0.8a1.dev8"
+version = "0.8a1.dev9"
 description = "Multi-purpose extensible self-adaptive optimizer and fuzzer"
 authors = [
     "Giovanni Squillero <giovanni.squillero@polito.it>",
     "Alberto Tonda <alberto.tonda@inrae.fr>",
 ]
 #maintainers = [
 #    "Giovanni Squillero <giovanni.squillero@polito.it>"
@@ -93,15 +93,15 @@
 inputs = ['byron']
 
 [tool.pylint]
 max-line-length = 120
 source-roots = ['src']
 
 [bumpver]
-current_version = "0.8a1.dev8"
+current_version = "0.8a1.dev9"
 version_pattern = "MAJOR.MINOR[PYTAGNUM].devINC0"
 commit_message = "Bump version to {new_version}"
 commit = false
 push = false
 
 [bumpver.file_patterns]
 "pyproject.toml" = [
```

### Comparing `byron-0.8a1.dev8/PKG-INFO` & `byron-0.8a1.dev9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: byron
-Version: 0.8a1.dev8
+Version: 0.8a1.dev9
 Summary: Multi-purpose extensible self-adaptive optimizer and fuzzer
 Home-page: https://github.com/cad-polito-it/byron
 License: Apache-2.0
 Keywords: Aritificial Intelligence,Evolutionary Computation,Approximate Optimization,Fuzzer
 Author: Giovanni Squillero
 Author-email: giovanni.squillero@polito.it
 Requires-Python: >=3.11,<3.13
```

