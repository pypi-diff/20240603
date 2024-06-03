# Comparing `tmp/math_spec_mapping-0.3.4.tar.gz` & `tmp/math_spec_mapping-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "math_spec_mapping-0.3.4.tar", last modified: Fri May 17 04:40:05 2024, max compression
+gzip compressed data, was "math_spec_mapping-0.3.5.tar", last modified: Mon Jun  3 13:55:29 2024, max compression
```

## Comparing `math_spec_mapping-0.3.4.tar` & `math_spec_mapping-0.3.5.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-05-17 04:40:05.897089 math_spec_mapping-0.3.4/
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1069 2023-12-10 00:44:46.000000 math_spec_mapping-0.3.4/LICENSE
--rw-r--r--   0 seanmcowen   (501) staff       (20)     6009 2024-05-17 04:40:05.896818 math_spec_mapping-0.3.4/PKG-INFO
--rw-r--r--   0 seanmcowen   (501) staff       (20)     5511 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.4/README.md
--rw-r--r--   0 seanmcowen   (501) staff       (20)      747 2024-05-17 04:30:03.000000 math_spec_mapping-0.3.4/pyproject.toml
--rw-r--r--   0 seanmcowen   (501) staff       (20)       38 2024-05-17 04:40:05.897134 math_spec_mapping-0.3.4/setup.cfg
-drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-05-17 04:40:05.886456 math_spec_mapping-0.3.4/src/
-drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-05-17 04:40:05.887733 math_spec_mapping-0.3.4/src/math_spec_mapping/
-drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-05-17 04:40:05.890972 math_spec_mapping-0.3.4/src/math_spec_mapping/Classes/
--rw-r--r--   0 seanmcowen   (501) staff       (20)      246 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Classes/ActionTransmissionChannel.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)    17437 2024-05-15 18:36:04.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Classes/Block.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      593 2024-05-17 03:51:16.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Classes/BoundaryAction.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      526 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Classes/ControlAction.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1226 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Classes/Entity.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)    32143 2024-05-17 04:00:15.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Classes/MathSpec.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      379 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Classes/Mechanism.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      581 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Classes/Metric.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1237 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Classes/Parameter.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      530 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Classes/Policy.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      472 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Classes/Space.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1599 2024-05-15 18:36:04.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Classes/State.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      257 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Classes/StateUpdateTransmissionChannel.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      749 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Classes/StatefulMetric.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      289 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Classes/Type.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      761 2024-03-31 21:59:52.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Classes/__init__.py
-drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-05-17 04:40:05.891408 math_spec_mapping-0.3.4/src/math_spec_mapping/Convenience/
--rw-r--r--   0 seanmcowen   (501) staff       (20)      112 2024-05-06 21:48:04.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Convenience/__init__.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1625 2024-05-06 21:48:04.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Convenience/documentation.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)    11010 2024-05-06 21:48:04.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Convenience/starter.py
-drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-05-17 04:40:05.894121 math_spec_mapping-0.3.4/src/math_spec_mapping/Load/
--rw-r--r--   0 seanmcowen   (501) staff       (20)       33 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Load/__init__.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     2561 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Load/action_transmission_channel.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     2625 2024-05-17 03:54:01.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Load/boundary_actions.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     2042 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Load/control_actions.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      480 2024-05-17 02:56:05.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Load/displays.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1289 2024-05-15 18:36:04.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Load/entities.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     4463 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Load/general.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      395 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Load/implementations.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     2484 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Load/load.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     2037 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Load/mechanism.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     3434 2024-04-17 18:04:23.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Load/metrics.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1393 2024-05-06 21:48:04.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Load/parameters.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     2444 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Load/policy.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1116 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Load/spaces.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     2238 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Load/state_update_transmission_channels.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1977 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Load/stateful_metrics.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1365 2024-05-17 00:59:42.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Load/states.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     4356 2024-05-06 21:48:04.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Load/type.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     3083 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Load/wiring.py
-drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-05-17 04:40:05.896332 math_spec_mapping-0.3.4/src/math_spec_mapping/Reports/
--rw-r--r--   0 seanmcowen   (501) staff       (20)      933 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Reports/__init__.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1410 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Reports/boundary_actions.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1216 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Reports/control_actions.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1610 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Reports/general.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     9007 2024-04-17 18:04:23.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Reports/html.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)    22871 2024-05-16 16:23:01.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Reports/markdown.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1322 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Reports/mechanisms.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     3129 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Reports/node_map.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      535 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Reports/parameters.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1814 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Reports/policies.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      579 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Reports/spaces.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     2321 2024-04-17 18:04:23.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Reports/state.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1505 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Reports/tables.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1618 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Reports/wiring.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      961 2024-05-06 21:48:04.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/__init__.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      233 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/schema.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)    30916 2024-05-16 16:43:09.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/schema.schema.json
-drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-05-17 04:40:05.896571 math_spec_mapping-0.3.4/src/math_spec_mapping.egg-info/
--rw-r--r--   0 seanmcowen   (501) staff       (20)     6009 2024-05-17 04:40:05.000000 math_spec_mapping-0.3.4/src/math_spec_mapping.egg-info/PKG-INFO
--rw-r--r--   0 seanmcowen   (501) staff       (20)     2610 2024-05-17 04:40:05.000000 math_spec_mapping-0.3.4/src/math_spec_mapping.egg-info/SOURCES.txt
--rw-r--r--   0 seanmcowen   (501) staff       (20)        1 2024-05-17 04:40:05.000000 math_spec_mapping-0.3.4/src/math_spec_mapping.egg-info/dependency_links.txt
--rw-r--r--   0 seanmcowen   (501) staff       (20)       44 2024-05-17 04:40:05.000000 math_spec_mapping-0.3.4/src/math_spec_mapping.egg-info/requires.txt
--rw-r--r--   0 seanmcowen   (501) staff       (20)       18 2024-05-17 04:40:05.000000 math_spec_mapping-0.3.4/src/math_spec_mapping.egg-info/top_level.txt
+drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-06-03 13:55:29.289541 math_spec_mapping-0.3.5/
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1069 2023-12-10 00:44:46.000000 math_spec_mapping-0.3.5/LICENSE
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     6009 2024-06-03 13:55:29.289318 math_spec_mapping-0.3.5/PKG-INFO
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     5511 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.5/README.md
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      747 2024-05-17 04:58:58.000000 math_spec_mapping-0.3.5/pyproject.toml
+-rw-r--r--   0 seanmcowen   (501) staff       (20)       38 2024-06-03 13:55:29.289580 math_spec_mapping-0.3.5/setup.cfg
+drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-06-03 13:55:29.277983 math_spec_mapping-0.3.5/src/
+drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-06-03 13:55:29.279213 math_spec_mapping-0.3.5/src/math_spec_mapping/
+drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-06-03 13:55:29.283110 math_spec_mapping-0.3.5/src/math_spec_mapping/Classes/
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      246 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.5/src/math_spec_mapping/Classes/ActionTransmissionChannel.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)    17437 2024-05-15 18:36:04.000000 math_spec_mapping-0.3.5/src/math_spec_mapping/Classes/Block.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      593 2024-05-17 04:55:49.000000 math_spec_mapping-0.3.5/src/math_spec_mapping/Classes/BoundaryAction.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      526 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.5/src/math_spec_mapping/Classes/ControlAction.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1226 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.5/src/math_spec_mapping/Classes/Entity.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)    33257 2024-06-03 03:53:20.000000 math_spec_mapping-0.3.5/src/math_spec_mapping/Classes/MathSpec.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      379 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.5/src/math_spec_mapping/Classes/Mechanism.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      581 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.5/src/math_spec_mapping/Classes/Metric.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1237 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.5/src/math_spec_mapping/Classes/Parameter.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      530 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.5/src/math_spec_mapping/Classes/Policy.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      472 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.5/src/math_spec_mapping/Classes/Space.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1599 2024-05-15 18:36:04.000000 math_spec_mapping-0.3.5/src/math_spec_mapping/Classes/State.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      257 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.5/src/math_spec_mapping/Classes/StateUpdateTransmissionChannel.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      749 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.5/src/math_spec_mapping/Classes/StatefulMetric.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      289 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.5/src/math_spec_mapping/Classes/Type.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      761 2024-03-31 21:59:52.000000 math_spec_mapping-0.3.5/src/math_spec_mapping/Classes/__init__.py
+drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-06-03 13:55:29.283566 math_spec_mapping-0.3.5/src/math_spec_mapping/Convenience/
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      112 2024-05-06 21:48:04.000000 math_spec_mapping-0.3.5/src/math_spec_mapping/Convenience/__init__.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1625 2024-05-06 21:48:04.000000 math_spec_mapping-0.3.5/src/math_spec_mapping/Convenience/documentation.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)    11010 2024-05-06 21:48:04.000000 math_spec_mapping-0.3.5/src/math_spec_mapping/Convenience/starter.py
+drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-06-03 13:55:29.286807 math_spec_mapping-0.3.5/src/math_spec_mapping/Load/
+-rw-r--r--   0 seanmcowen   (501) staff       (20)       33 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.5/src/math_spec_mapping/Load/__init__.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     2561 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.5/src/math_spec_mapping/Load/action_transmission_channel.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     2625 2024-05-17 04:55:49.000000 math_spec_mapping-0.3.5/src/math_spec_mapping/Load/boundary_actions.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     2042 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.5/src/math_spec_mapping/Load/control_actions.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      480 2024-05-17 04:55:49.000000 math_spec_mapping-0.3.5/src/math_spec_mapping/Load/displays.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1289 2024-05-15 18:36:04.000000 math_spec_mapping-0.3.5/src/math_spec_mapping/Load/entities.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     4463 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.5/src/math_spec_mapping/Load/general.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      395 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.5/src/math_spec_mapping/Load/implementations.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     2484 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.5/src/math_spec_mapping/Load/load.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     2037 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.5/src/math_spec_mapping/Load/mechanism.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     3434 2024-04-17 18:04:23.000000 math_spec_mapping-0.3.5/src/math_spec_mapping/Load/metrics.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1393 2024-05-06 21:48:04.000000 math_spec_mapping-0.3.5/src/math_spec_mapping/Load/parameters.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     2444 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.5/src/math_spec_mapping/Load/policy.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1116 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.5/src/math_spec_mapping/Load/spaces.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     2238 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.5/src/math_spec_mapping/Load/state_update_transmission_channels.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1977 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.5/src/math_spec_mapping/Load/stateful_metrics.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1365 2024-05-17 04:55:49.000000 math_spec_mapping-0.3.5/src/math_spec_mapping/Load/states.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     4356 2024-05-06 21:48:04.000000 math_spec_mapping-0.3.5/src/math_spec_mapping/Load/type.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     3083 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.5/src/math_spec_mapping/Load/wiring.py
+drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-06-03 13:55:29.288894 math_spec_mapping-0.3.5/src/math_spec_mapping/Reports/
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      933 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.5/src/math_spec_mapping/Reports/__init__.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1410 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.5/src/math_spec_mapping/Reports/boundary_actions.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1216 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.5/src/math_spec_mapping/Reports/control_actions.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1610 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.5/src/math_spec_mapping/Reports/general.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     9220 2024-06-03 02:52:31.000000 math_spec_mapping-0.3.5/src/math_spec_mapping/Reports/html.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)    22871 2024-05-17 04:55:49.000000 math_spec_mapping-0.3.5/src/math_spec_mapping/Reports/markdown.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1322 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.5/src/math_spec_mapping/Reports/mechanisms.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     3129 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.5/src/math_spec_mapping/Reports/node_map.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      535 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.5/src/math_spec_mapping/Reports/parameters.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1814 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.5/src/math_spec_mapping/Reports/policies.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      579 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.5/src/math_spec_mapping/Reports/spaces.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     2321 2024-04-17 18:04:23.000000 math_spec_mapping-0.3.5/src/math_spec_mapping/Reports/state.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1505 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.5/src/math_spec_mapping/Reports/tables.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1618 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.5/src/math_spec_mapping/Reports/wiring.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      961 2024-05-06 21:48:04.000000 math_spec_mapping-0.3.5/src/math_spec_mapping/__init__.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      233 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.5/src/math_spec_mapping/schema.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)    30916 2024-05-17 04:55:49.000000 math_spec_mapping-0.3.5/src/math_spec_mapping/schema.schema.json
+drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-06-03 13:55:29.289086 math_spec_mapping-0.3.5/src/math_spec_mapping.egg-info/
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     6009 2024-06-03 13:55:29.000000 math_spec_mapping-0.3.5/src/math_spec_mapping.egg-info/PKG-INFO
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     2610 2024-06-03 13:55:29.000000 math_spec_mapping-0.3.5/src/math_spec_mapping.egg-info/SOURCES.txt
+-rw-r--r--   0 seanmcowen   (501) staff       (20)        1 2024-06-03 13:55:29.000000 math_spec_mapping-0.3.5/src/math_spec_mapping.egg-info/dependency_links.txt
+-rw-r--r--   0 seanmcowen   (501) staff       (20)       44 2024-06-03 13:55:29.000000 math_spec_mapping-0.3.5/src/math_spec_mapping.egg-info/requires.txt
+-rw-r--r--   0 seanmcowen   (501) staff       (20)       18 2024-06-03 13:55:29.000000 math_spec_mapping-0.3.5/src/math_spec_mapping.egg-info/top_level.txt
```

### Comparing `math_spec_mapping-0.3.4/LICENSE` & `math_spec_mapping-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.4/PKG-INFO` & `math_spec_mapping-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: math-spec-mapping
-Version: 0.3.4
+Version: 0.3.5
 Summary: A library for easy mapping of mathematical specifications.
 Author-email: Sean McOwen <Sean@Block.Science>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `math_spec_mapping-0.3.4/README.md` & `math_spec_mapping-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.4/pyproject.toml` & `math_spec_mapping-0.3.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "math-spec-mapping"
-version = "0.3.4"
+version = "0.3.5"
 authors = [
   { name="Sean McOwen", email="Sean@Block.Science" },
 ]
 description = "A library for easy mapping of mathematical specifications."
 dependencies = [
   "graphviz>=0.20.1",
   "ipython>=7.7.0",
```

### Comparing `math_spec_mapping-0.3.4/src/math_spec_mapping/Classes/Block.py` & `math_spec_mapping-0.3.5/src/math_spec_mapping/Classes/Block.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.4/src/math_spec_mapping/Classes/BoundaryAction.py` & `math_spec_mapping-0.3.5/src/math_spec_mapping/Classes/BoundaryAction.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.4/src/math_spec_mapping/Classes/ControlAction.py` & `math_spec_mapping-0.3.5/src/math_spec_mapping/Classes/ControlAction.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.4/src/math_spec_mapping/Classes/Entity.py` & `math_spec_mapping-0.3.5/src/math_spec_mapping/Classes/Entity.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.4/src/math_spec_mapping/Classes/MathSpec.py` & `math_spec_mapping-0.3.5/src/math_spec_mapping/Classes/MathSpec.py`

 * *Files 6% similar despite different names*

```diff
@@ -367,15 +367,15 @@
                 (x, x.boundary_action_options)
                 for x in self.boundary_actions.values()
                 if len(x.boundary_action_options) > 1
             ]
         )
         opts.extend(
             [
-                (x, x.control_actions)
+                (x, x.control_action_options)
                 for x in self.control_actions.values()
                 if len(x.control_action_options) > 1
             ]
         )
         self.functional_parameters = {}
         for x in opts:
             x, y = x
@@ -725,15 +725,15 @@
             else:
                 if len(opts) == 1:
                     opt = opts[0]
                 else:
                     assert (
                         "FP {}".format(ba.name) in self.params
                     ), "No functional parameterization for {}. To fix this error, add {} to the parameters passed to ms.build_implementation. Option can be: {}".format(
-                        ba.name, ba.name, [x.name for x in opts]
+                        ba.name, "FP " + ba.name, [x.name for x in opts]
                     )
 
                     opt = self.ms.functional_parameters["FP {}".format(ba.name)][
                         self.params["FP {}".format(ba.name)]
                     ]
 
                 if "python" not in opt.implementations:
@@ -802,15 +802,15 @@
             else:
                 if len(opts) == 1:
                     opt = opts[0]
                 else:
                     assert (
                         "FP {}".format(p.name) in self.params
                     ), "No functional parameterization for {}. To fix this error, add {} to the parameters passed to ms.build_implementation. Option can be: {}".format(
-                        p.name, p.name, [x.name for x in opts]
+                        p.name, "FP " + p.name, [x.name for x in opts]
                     )
                     opt = self.ms.functional_parameters["FP {}".format(p.name)][
                         self.params["FP {}".format(p.name)]
                     ]
 
                 if "python" not in opt.implementations:
                     print(
@@ -853,7 +853,35 @@
 
                 else:
                     hold.append(w)
             wiring = hold
         if len(wiring) > 0:
             wiring = [x.name for x in wiring]
             print("The following wirings were not loading: {}".format(wiring))
+
+    def validate_state_and_params(self, state, parameters):
+
+        k1 = state.keys()
+        k2 = [x.name for x in self.ms.state["Global State"].variables]
+
+        not_in_state = [x for x in k2 if x not in k1]
+        shouldnt_be_in_state = [x for x in k1 if x not in k2]
+        assert (
+            len(not_in_state) == 0
+        ), "The following state variables are missing: {}".format(not_in_state)
+        assert (
+            len(shouldnt_be_in_state) == 0
+        ), "The following state variables are extra: {}".format(shouldnt_be_in_state)
+
+        k1 = parameters.keys()
+        k2 = self.ms.parameters.all_parameters + list(
+            self.ms.functional_parameters.keys()
+        )
+
+        not_in_params = [x for x in k2 if x not in k1]
+        shouldnt_be_in_params = [x for x in k1 if x not in k2]
+        assert (
+            len(not_in_params) == 0
+        ), "The following parameters are missing: {}".format(not_in_params)
+        assert (
+            len(shouldnt_be_in_params) == 0
+        ), "The following parameters are extra: {}".format(shouldnt_be_in_params)
```

### Comparing `math_spec_mapping-0.3.4/src/math_spec_mapping/Classes/Metric.py` & `math_spec_mapping-0.3.5/src/math_spec_mapping/Classes/Metric.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.4/src/math_spec_mapping/Classes/Parameter.py` & `math_spec_mapping-0.3.5/src/math_spec_mapping/Classes/Parameter.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.4/src/math_spec_mapping/Classes/Policy.py` & `math_spec_mapping-0.3.5/src/math_spec_mapping/Classes/Policy.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.4/src/math_spec_mapping/Classes/State.py` & `math_spec_mapping-0.3.5/src/math_spec_mapping/Classes/State.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.4/src/math_spec_mapping/Classes/StatefulMetric.py` & `math_spec_mapping-0.3.5/src/math_spec_mapping/Classes/StatefulMetric.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.4/src/math_spec_mapping/Classes/__init__.py` & `math_spec_mapping-0.3.5/src/math_spec_mapping/Classes/__init__.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.4/src/math_spec_mapping/Convenience/documentation.py` & `math_spec_mapping-0.3.5/src/math_spec_mapping/Convenience/documentation.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.4/src/math_spec_mapping/Convenience/starter.py` & `math_spec_mapping-0.3.5/src/math_spec_mapping/Convenience/starter.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.4/src/math_spec_mapping/Load/action_transmission_channel.py` & `math_spec_mapping-0.3.5/src/math_spec_mapping/Load/action_transmission_channel.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.4/src/math_spec_mapping/Load/boundary_actions.py` & `math_spec_mapping-0.3.5/src/math_spec_mapping/Load/boundary_actions.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.4/src/math_spec_mapping/Load/control_actions.py` & `math_spec_mapping-0.3.5/src/math_spec_mapping/Load/control_actions.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.4/src/math_spec_mapping/Load/entities.py` & `math_spec_mapping-0.3.5/src/math_spec_mapping/Load/entities.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.4/src/math_spec_mapping/Load/general.py` & `math_spec_mapping-0.3.5/src/math_spec_mapping/Load/general.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.4/src/math_spec_mapping/Load/load.py` & `math_spec_mapping-0.3.5/src/math_spec_mapping/Load/load.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.4/src/math_spec_mapping/Load/mechanism.py` & `math_spec_mapping-0.3.5/src/math_spec_mapping/Load/mechanism.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.4/src/math_spec_mapping/Load/metrics.py` & `math_spec_mapping-0.3.5/src/math_spec_mapping/Load/metrics.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.4/src/math_spec_mapping/Load/parameters.py` & `math_spec_mapping-0.3.5/src/math_spec_mapping/Load/parameters.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.4/src/math_spec_mapping/Load/policy.py` & `math_spec_mapping-0.3.5/src/math_spec_mapping/Load/policy.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.4/src/math_spec_mapping/Load/spaces.py` & `math_spec_mapping-0.3.5/src/math_spec_mapping/Load/spaces.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.4/src/math_spec_mapping/Load/state_update_transmission_channels.py` & `math_spec_mapping-0.3.5/src/math_spec_mapping/Load/state_update_transmission_channels.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.4/src/math_spec_mapping/Load/stateful_metrics.py` & `math_spec_mapping-0.3.5/src/math_spec_mapping/Load/stateful_metrics.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.4/src/math_spec_mapping/Load/states.py` & `math_spec_mapping-0.3.5/src/math_spec_mapping/Load/states.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.4/src/math_spec_mapping/Load/type.py` & `math_spec_mapping-0.3.5/src/math_spec_mapping/Load/type.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.4/src/math_spec_mapping/Load/wiring.py` & `math_spec_mapping-0.3.5/src/math_spec_mapping/Load/wiring.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.4/src/math_spec_mapping/Reports/__init__.py` & `math_spec_mapping-0.3.5/src/math_spec_mapping/Reports/__init__.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.4/src/math_spec_mapping/Reports/boundary_actions.py` & `math_spec_mapping-0.3.5/src/math_spec_mapping/Reports/boundary_actions.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.4/src/math_spec_mapping/Reports/control_actions.py` & `math_spec_mapping-0.3.5/src/math_spec_mapping/Reports/control_actions.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.4/src/math_spec_mapping/Reports/general.py` & `math_spec_mapping-0.3.5/src/math_spec_mapping/Reports/general.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.4/src/math_spec_mapping/Reports/html.py` & `math_spec_mapping-0.3.5/src/math_spec_mapping/Reports/html.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,15 +160,18 @@
     out += symbol1 + "**Stateful Metrics**\n"
     for name in ms.stateful_metrics.keys():
         if linking:
             out += symbol2 + "{}".format(name) + "\n"
         else:
             out += symbol2 + name + "\n"
         for var in ms.stateful_metrics[name].metrics:
-            out += symbol3 + "[[{}]]".format(var.name) + "\n"
+            if linking:
+                out += symbol3 + "[[{}]]".format(var.name) + "\n"
+            else:
+                out += symbol3 + "{}".format(var.name) + "\n"
 
     out += symbol1 + "**Types**\n"
     for name in ms.types.keys():
         if linking:
             out += symbol2 + "[[{}]]".format(name) + "\n"
         else:
             out += symbol2 + name + "\n"
@@ -182,15 +185,18 @@
     out += symbol1 + "**Parameters**\n"
     for name in ms.parameters.data.keys():
         if linking:
             out += symbol2 + "{}".format(name) + "\n"
         else:
             out += symbol2 + name + "\n"
         for param in [x.name for x in ms.parameters.data[name].parameters]:
-            out += symbol3 + "[[{}]]".format(param) + "\n"
+            if linking:
+                out += symbol3 + "[[{}]]".format(param) + "\n"
+            else:
+                out += symbol3 + "{}".format(param) + "\n"
 
     out += symbol1 + "**Boundary Actions**\n"
     for name in ms.boundary_actions.keys():
         if linking:
             out += symbol2 + "[[{}]]".format(name) + "\n"
         else:
             out += symbol2 + name + "\n"
```

### Comparing `math_spec_mapping-0.3.4/src/math_spec_mapping/Reports/markdown.py` & `math_spec_mapping-0.3.5/src/math_spec_mapping/Reports/markdown.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.4/src/math_spec_mapping/Reports/mechanisms.py` & `math_spec_mapping-0.3.5/src/math_spec_mapping/Reports/mechanisms.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.4/src/math_spec_mapping/Reports/node_map.py` & `math_spec_mapping-0.3.5/src/math_spec_mapping/Reports/node_map.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.4/src/math_spec_mapping/Reports/parameters.py` & `math_spec_mapping-0.3.5/src/math_spec_mapping/Reports/parameters.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.4/src/math_spec_mapping/Reports/policies.py` & `math_spec_mapping-0.3.5/src/math_spec_mapping/Reports/policies.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.4/src/math_spec_mapping/Reports/spaces.py` & `math_spec_mapping-0.3.5/src/math_spec_mapping/Reports/spaces.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.4/src/math_spec_mapping/Reports/state.py` & `math_spec_mapping-0.3.5/src/math_spec_mapping/Reports/state.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.4/src/math_spec_mapping/Reports/tables.py` & `math_spec_mapping-0.3.5/src/math_spec_mapping/Reports/tables.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.4/src/math_spec_mapping/Reports/wiring.py` & `math_spec_mapping-0.3.5/src/math_spec_mapping/Reports/wiring.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.4/src/math_spec_mapping/__init__.py` & `math_spec_mapping-0.3.5/src/math_spec_mapping/__init__.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.4/src/math_spec_mapping/schema.schema.json` & `math_spec_mapping-0.3.5/src/math_spec_mapping/schema.schema.json`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.4/src/math_spec_mapping.egg-info/PKG-INFO` & `math_spec_mapping-0.3.5/src/math_spec_mapping.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: math-spec-mapping
-Version: 0.3.4
+Version: 0.3.5
 Summary: A library for easy mapping of mathematical specifications.
 Author-email: Sean McOwen <Sean@Block.Science>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `math_spec_mapping-0.3.4/src/math_spec_mapping.egg-info/SOURCES.txt` & `math_spec_mapping-0.3.5/src/math_spec_mapping.egg-info/SOURCES.txt`

 * *Files identical despite different names*

