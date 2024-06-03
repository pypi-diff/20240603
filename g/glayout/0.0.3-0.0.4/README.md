# Comparing `tmp/glayout-0.0.3.tar.gz` & `tmp/glayout-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glayout-0.0.3.tar", last modified: Sat Apr 13 00:03:43 2024, max compression
+gzip compressed data, was "glayout-0.0.4.tar", last modified: Mon Jun  3 08:07:55 2024, max compression
```

## Comparing `glayout-0.0.3.tar` & `glayout-0.0.4.tar`

### file list

```diff
@@ -1,59 +1,80 @@
-drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-04-13 00:03:43.751008 glayout-0.0.3/
--rw-r--r--   0 labtob    (1000) labtob    (1000)    31914 2024-04-13 00:03:43.751008 glayout-0.0.3/PKG-INFO
-drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-04-13 00:03:43.746008 glayout-0.0.3/glayout/
--rw-r--r--   0 labtob    (1000) labtob    (1000)       18 2024-04-06 16:10:51.000000 glayout-0.0.3/glayout/__init__.py
-drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-04-13 00:03:43.748008 glayout-0.0.3/glayout/components/
--rw-r--r--   0 labtob    (1000) labtob    (1000)        0 2024-04-06 16:10:51.000000 glayout-0.0.3/glayout/components/__init__.py
--rw-r--r--   0 labtob    (1000) labtob    (1000)    10577 2024-04-06 16:10:51.000000 glayout-0.0.3/glayout/components/diff_pair.py
--rw-r--r--   0 labtob    (1000) labtob    (1000)     7074 2024-04-06 16:10:51.000000 glayout-0.0.3/glayout/components/diff_pair_cmirrorbias.py
--rw-r--r--   0 labtob    (1000) labtob    (1000)    10713 2024-04-06 16:10:51.000000 glayout-0.0.3/glayout/components/diff_pair_stackedcmirror.py
--rw-r--r--   0 labtob    (1000) labtob    (1000)    12982 2024-04-06 16:10:51.000000 glayout-0.0.3/glayout/components/differential_to_single_ended_converter.py
--rw-r--r--   0 labtob    (1000) labtob    (1000)    10212 2024-04-06 16:10:51.000000 glayout-0.0.3/glayout/components/opamp.py
--rw-r--r--   0 labtob    (1000) labtob    (1000)    15844 2024-04-06 16:10:51.000000 glayout-0.0.3/glayout/components/opamp_twostage.py
--rw-r--r--   0 labtob    (1000) labtob    (1000)     4912 2024-04-06 16:10:51.000000 glayout-0.0.3/glayout/components/row_csamplifier_diff_to_single_ended_converter.py
--rw-r--r--   0 labtob    (1000) labtob    (1000)     3129 2024-04-06 16:10:51.000000 glayout-0.0.3/glayout/components/stacked_current_mirror.py
-drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-04-13 00:03:43.748008 glayout-0.0.3/glayout/pdk/
--rw-r--r--   0 labtob    (1000) labtob    (1000)        0 2024-04-06 16:10:51.000000 glayout-0.0.3/glayout/pdk/__init__.py
-drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-04-13 00:03:43.749008 glayout-0.0.3/glayout/pdk/gf180_mapped/
--rw-r--r--   0 labtob    (1000) labtob    (1000)      150 2024-04-06 16:10:51.000000 glayout-0.0.3/glayout/pdk/gf180_mapped/__init__.py
--rw-r--r--   0 labtob    (1000) labtob    (1000)     1317 2024-04-13 00:03:04.000000 glayout-0.0.3/glayout/pdk/gf180_mapped/gf180_mapped.py
--rw-r--r--   0 labtob    (1000) labtob    (1000)    13625 2024-04-06 16:10:51.000000 glayout-0.0.3/glayout/pdk/gf180_mapped/grules.py
--rw-r--r--   0 labtob    (1000) labtob    (1000)    14510 2024-04-06 16:10:51.000000 glayout-0.0.3/glayout/pdk/mappedpdk.py
-drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-04-13 00:03:43.749008 glayout-0.0.3/glayout/pdk/sky130_mapped/
--rw-r--r--   0 labtob    (1000) labtob    (1000)      155 2024-04-06 16:10:51.000000 glayout-0.0.3/glayout/pdk/sky130_mapped/__init__.py
--rw-r--r--   0 labtob    (1000) labtob    (1000)    13642 2024-04-06 16:10:51.000000 glayout-0.0.3/glayout/pdk/sky130_mapped/grules.py
--rw-r--r--   0 labtob    (1000) labtob    (1000)     2781 2024-04-06 16:10:51.000000 glayout-0.0.3/glayout/pdk/sky130_mapped/sky130_add_npc.py
--rw-r--r--   0 labtob    (1000) labtob    (1000)     1305 2024-04-13 00:03:19.000000 glayout-0.0.3/glayout/pdk/sky130_mapped/sky130_mapped.py
-drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-04-13 00:03:43.750008 glayout-0.0.3/glayout/pdk/util/
--rw-r--r--   0 labtob    (1000) labtob    (1000)        0 2024-04-06 16:10:51.000000 glayout-0.0.3/glayout/pdk/util/__init__.py
--rw-r--r--   0 labtob    (1000) labtob    (1000)    12926 2024-04-06 16:10:51.000000 glayout-0.0.3/glayout/pdk/util/comp_utils.py
--rw-r--r--   0 labtob    (1000) labtob    (1000)     2350 2024-04-06 16:10:51.000000 glayout-0.0.3/glayout/pdk/util/component_array_create.py
--rw-r--r--   0 labtob    (1000) labtob    (1000)    15988 2024-04-06 16:10:51.000000 glayout-0.0.3/glayout/pdk/util/port_utils.py
--rw-r--r--   0 labtob    (1000) labtob    (1000)     5190 2024-04-06 16:10:51.000000 glayout-0.0.3/glayout/pdk/util/print_rules.py
--rw-r--r--   0 labtob    (1000) labtob    (1000)      480 2024-04-06 16:10:51.000000 glayout-0.0.3/glayout/pdk/util/snap_to_grid.py
-drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-04-13 00:03:43.750008 glayout-0.0.3/glayout/placement/
--rw-r--r--   0 labtob    (1000) labtob    (1000)        0 2024-04-06 16:10:51.000000 glayout-0.0.3/glayout/placement/__init__.py
--rw-r--r--   0 labtob    (1000) labtob    (1000)     8520 2024-04-06 16:10:51.000000 glayout-0.0.3/glayout/placement/two_transistor_interdigitized.py
--rw-r--r--   0 labtob    (1000) labtob    (1000)     2241 2024-04-06 16:10:51.000000 glayout-0.0.3/glayout/placement/two_transistor_place.py
-drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-04-13 00:03:43.750008 glayout-0.0.3/glayout/primitives/
--rw-r--r--   0 labtob    (1000) labtob    (1000)        0 2024-04-06 16:10:51.000000 glayout-0.0.3/glayout/primitives/__init__.py
--rw-r--r--   0 labtob    (1000) labtob    (1000)    28362 2024-04-06 16:10:51.000000 glayout-0.0.3/glayout/primitives/fet.py
--rw-r--r--   0 labtob    (1000) labtob    (1000)     5503 2024-04-06 16:10:51.000000 glayout-0.0.3/glayout/primitives/guardring.py
--rw-r--r--   0 labtob    (1000) labtob    (1000)     5182 2024-04-06 16:10:51.000000 glayout-0.0.3/glayout/primitives/mimcap.py
--rw-r--r--   0 labtob    (1000) labtob    (1000)    14335 2024-04-06 16:10:51.000000 glayout-0.0.3/glayout/primitives/via_gen.py
-drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-04-13 00:03:43.751008 glayout-0.0.3/glayout/routing/
--rw-r--r--   0 labtob    (1000) labtob    (1000)     4469 2024-04-06 16:10:51.000000 glayout-0.0.3/glayout/routing/L_route.py
--rw-r--r--   0 labtob    (1000) labtob    (1000)        0 2024-04-06 16:10:51.000000 glayout-0.0.3/glayout/routing/__init__.py
--rw-r--r--   0 labtob    (1000) labtob    (1000)     9611 2024-04-06 16:10:51.000000 glayout-0.0.3/glayout/routing/c_route.py
--rw-r--r--   0 labtob    (1000) labtob    (1000)     4488 2024-04-06 16:10:51.000000 glayout-0.0.3/glayout/routing/straight_route.py
-drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-04-13 00:03:43.751008 glayout-0.0.3/glayout/spice/
--rw-r--r--   0 labtob    (1000) labtob    (1000)       28 2024-04-06 16:10:51.000000 glayout-0.0.3/glayout/spice/__init__.py
--rw-r--r--   0 labtob    (1000) labtob    (1000)    11224 2024-04-06 16:10:51.000000 glayout-0.0.3/glayout/spice/netlist.py
-drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-04-13 00:03:43.747008 glayout-0.0.3/glayout.egg-info/
--rw-r--r--   0 labtob    (1000) labtob    (1000)    31914 2024-04-13 00:03:43.000000 glayout-0.0.3/glayout.egg-info/PKG-INFO
--rw-r--r--   0 labtob    (1000) labtob    (1000)     1624 2024-04-13 00:03:43.000000 glayout-0.0.3/glayout.egg-info/SOURCES.txt
--rw-r--r--   0 labtob    (1000) labtob    (1000)        1 2024-04-13 00:03:43.000000 glayout-0.0.3/glayout.egg-info/dependency_links.txt
--rw-r--r--   0 labtob    (1000) labtob    (1000)       34 2024-04-13 00:03:43.000000 glayout-0.0.3/glayout.egg-info/requires.txt
--rw-r--r--   0 labtob    (1000) labtob    (1000)        8 2024-04-13 00:03:43.000000 glayout-0.0.3/glayout.egg-info/top_level.txt
--rw-r--r--   0 labtob    (1000) labtob    (1000)       38 2024-04-13 00:03:43.751008 glayout-0.0.3/setup.cfg
--rw-r--r--   0 labtob    (1000) labtob    (1000)     1128 2024-04-13 00:03:40.000000 glayout-0.0.3/setup.py
+drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-06-03 08:07:55.665222 glayout-0.0.4/
+-rw-r--r--   0 labtob    (1000) labtob    (1000)    47806 2024-06-03 08:07:55.665222 glayout-0.0.4/PKG-INFO
+-rw-r--r--   0 labtob    (1000) labtob    (1000)    47090 2024-06-03 08:07:22.000000 glayout-0.0.4/README.md
+drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-06-03 08:07:55.659222 glayout-0.0.4/glayout/
+-rw-r--r--   0 labtob    (1000) labtob    (1000)       18 2024-05-31 19:50:08.000000 glayout-0.0.4/glayout/__init__.py
+drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-06-03 08:07:55.660221 glayout-0.0.4/glayout/flow/
+-rw-r--r--   0 labtob    (1000) labtob    (1000)        0 2024-05-31 19:50:08.000000 glayout-0.0.4/glayout/flow/__init__.py
+drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-06-03 08:07:55.661222 glayout-0.0.4/glayout/flow/components/
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     3591 2024-06-01 04:36:26.000000 glayout-0.0.4/glayout/flow/components/CrossCoupledInverters_cell.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)        0 2024-05-31 19:50:08.000000 glayout-0.0.4/glayout/flow/components/__init__.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     5118 2024-05-31 19:50:08.000000 glayout-0.0.4/glayout/flow/components/current_mirror.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)    11298 2024-05-31 19:50:08.000000 glayout-0.0.4/glayout/flow/components/diff_pair.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     7149 2024-05-31 19:50:08.000000 glayout-0.0.4/glayout/flow/components/diff_pair_cmirrorbias.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)    10798 2024-05-31 19:50:08.000000 glayout-0.0.4/glayout/flow/components/diff_pair_stackedcmirror.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)    13052 2024-05-31 19:50:08.000000 glayout-0.0.4/glayout/flow/components/differential_to_single_ended_converter.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)    10292 2024-05-31 19:50:08.000000 glayout-0.0.4/glayout/flow/components/opamp.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)    15018 2024-05-31 19:50:08.000000 glayout-0.0.4/glayout/flow/components/opamp_cell.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)    15944 2024-05-31 19:50:08.000000 glayout-0.0.4/glayout/flow/components/opamp_twostage.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     4982 2024-05-31 19:50:08.000000 glayout-0.0.4/glayout/flow/components/row_csamplifier_diff_to_single_ended_converter.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     3199 2024-05-31 19:50:08.000000 glayout-0.0.4/glayout/flow/components/stacked_current_mirror.py
+drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-06-03 08:07:55.661222 glayout-0.0.4/glayout/flow/pdk/
+-rw-r--r--   0 labtob    (1000) labtob    (1000)        0 2024-05-31 19:50:08.000000 glayout-0.0.4/glayout/flow/pdk/__init__.py
+drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-06-03 08:07:55.661222 glayout-0.0.4/glayout/flow/pdk/gf180_mapped/
+-rw-r--r--   0 labtob    (1000) labtob    (1000)      155 2024-05-31 19:50:08.000000 glayout-0.0.4/glayout/flow/pdk/gf180_mapped/__init__.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     2371 2024-05-31 19:50:08.000000 glayout-0.0.4/glayout/flow/pdk/gf180_mapped/gf180_mapped.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)    13625 2024-05-31 19:50:08.000000 glayout-0.0.4/glayout/flow/pdk/gf180_mapped/grules.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)    41412 2024-05-31 19:50:08.000000 glayout-0.0.4/glayout/flow/pdk/mappedpdk.py
+drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-06-03 08:07:55.662222 glayout-0.0.4/glayout/flow/pdk/sky130_mapped/
+-rw-r--r--   0 labtob    (1000) labtob    (1000)      160 2024-05-31 19:50:08.000000 glayout-0.0.4/glayout/flow/pdk/sky130_mapped/__init__.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)    13642 2024-05-31 19:50:08.000000 glayout-0.0.4/glayout/flow/pdk/sky130_mapped/grules.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     2781 2024-05-31 19:50:08.000000 glayout-0.0.4/glayout/flow/pdk/sky130_mapped/sky130_add_npc.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     2011 2024-05-31 19:50:08.000000 glayout-0.0.4/glayout/flow/pdk/sky130_mapped/sky130_mapped.py
+drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-06-03 08:07:55.662222 glayout-0.0.4/glayout/flow/pdk/util/
+-rw-r--r--   0 labtob    (1000) labtob    (1000)        0 2024-05-31 19:50:08.000000 glayout-0.0.4/glayout/flow/pdk/util/__init__.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)    14235 2024-05-31 19:50:08.000000 glayout-0.0.4/glayout/flow/pdk/util/comp_utils.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     2350 2024-05-31 19:50:08.000000 glayout-0.0.4/glayout/flow/pdk/util/component_array_create.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)    20448 2024-05-31 19:50:08.000000 glayout-0.0.4/glayout/flow/pdk/util/port_utils.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     5190 2024-05-31 19:50:08.000000 glayout-0.0.4/glayout/flow/pdk/util/print_rules.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)      480 2024-05-31 19:50:08.000000 glayout-0.0.4/glayout/flow/pdk/util/snap_to_grid.py
+drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-06-03 08:07:55.663221 glayout-0.0.4/glayout/flow/placement/
+-rw-r--r--   0 labtob    (1000) labtob    (1000)        0 2024-05-31 19:50:08.000000 glayout-0.0.4/glayout/flow/placement/__init__.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)    16267 2024-05-31 19:50:08.000000 glayout-0.0.4/glayout/flow/placement/common_centroid_ab_ba.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     2368 2024-06-01 03:59:21.000000 glayout-0.0.4/glayout/flow/placement/four_transistor_interdigitized.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)    13444 2024-05-31 19:50:08.000000 glayout-0.0.4/glayout/flow/placement/two_transistor_interdigitized.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     2256 2024-05-31 19:50:08.000000 glayout-0.0.4/glayout/flow/placement/two_transistor_place.py
+drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-06-03 08:07:55.663221 glayout-0.0.4/glayout/flow/primitives/
+-rw-r--r--   0 labtob    (1000) labtob    (1000)        0 2024-05-31 19:50:08.000000 glayout-0.0.4/glayout/flow/primitives/__init__.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)    28775 2024-05-31 19:50:08.000000 glayout-0.0.4/glayout/flow/primitives/fet.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     5534 2024-05-31 19:50:08.000000 glayout-0.0.4/glayout/flow/primitives/guardring.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     5214 2024-05-31 19:50:08.000000 glayout-0.0.4/glayout/flow/primitives/mimcap.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     8004 2024-05-31 19:50:08.000000 glayout-0.0.4/glayout/flow/primitives/resistor.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)    14355 2024-05-31 19:50:08.000000 glayout-0.0.4/glayout/flow/primitives/via_gen.py
+drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-06-03 08:07:55.664222 glayout-0.0.4/glayout/flow/routing/
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     4489 2024-05-31 19:50:08.000000 glayout-0.0.4/glayout/flow/routing/L_route.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)        0 2024-05-31 19:50:08.000000 glayout-0.0.4/glayout/flow/routing/__init__.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)    10790 2024-05-31 19:50:08.000000 glayout-0.0.4/glayout/flow/routing/c_route.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)    18533 2024-05-31 19:50:08.000000 glayout-0.0.4/glayout/flow/routing/smart_route.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     4508 2024-05-31 19:50:08.000000 glayout-0.0.4/glayout/flow/routing/straight_route.py
+drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-06-03 08:07:55.664222 glayout-0.0.4/glayout/flow/spice/
+-rw-r--r--   0 labtob    (1000) labtob    (1000)       28 2024-05-31 19:50:08.000000 glayout-0.0.4/glayout/flow/spice/__init__.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)    11224 2024-05-31 19:50:08.000000 glayout-0.0.4/glayout/flow/spice/netlist.py
+drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-06-03 08:07:55.664222 glayout-0.0.4/glayout/llm/
+-rw-r--r--   0 labtob    (1000) labtob    (1000)        0 2024-05-31 19:50:08.000000 glayout-0.0.4/glayout/llm/__init__.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)    13786 2024-06-01 19:06:49.000000 glayout-0.0.4/glayout/llm/manage_data.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)    12531 2024-06-01 20:47:53.000000 glayout-0.0.4/glayout/llm/train_and_run.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     1899 2024-05-31 19:50:08.000000 glayout-0.0.4/glayout/llm/validate_synthetic_data.py
+drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-06-03 08:07:55.665222 glayout-0.0.4/glayout/syntaxer/
+-rw-r--r--   0 labtob    (1000) labtob    (1000)        1 2024-05-31 19:50:08.000000 glayout-0.0.4/glayout/syntaxer/__init__.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     8269 2024-05-31 19:50:08.000000 glayout-0.0.4/glayout/syntaxer/dynamic_load.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)      512 2024-05-31 19:50:08.000000 glayout-0.0.4/glayout/syntaxer/nltk_init_deps.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)    17326 2024-05-31 19:50:08.000000 glayout-0.0.4/glayout/syntaxer/process_input.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)    45589 2024-05-31 19:50:08.000000 glayout-0.0.4/glayout/syntaxer/relational.py
+drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-06-03 08:07:55.660221 glayout-0.0.4/glayout.egg-info/
+-rw-r--r--   0 labtob    (1000) labtob    (1000)    47806 2024-06-03 08:07:55.000000 glayout-0.0.4/glayout.egg-info/PKG-INFO
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     2353 2024-06-03 08:07:55.000000 glayout-0.0.4/glayout.egg-info/SOURCES.txt
+-rw-r--r--   0 labtob    (1000) labtob    (1000)        1 2024-06-03 08:07:55.000000 glayout-0.0.4/glayout.egg-info/dependency_links.txt
+-rw-r--r--   0 labtob    (1000) labtob    (1000)      260 2024-06-03 08:07:55.000000 glayout-0.0.4/glayout.egg-info/requires.txt
+-rw-r--r--   0 labtob    (1000) labtob    (1000)        8 2024-06-03 08:07:55.000000 glayout-0.0.4/glayout.egg-info/top_level.txt
+-rw-r--r--   0 labtob    (1000) labtob    (1000)       38 2024-06-03 08:07:55.665222 glayout-0.0.4/setup.cfg
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     1583 2024-05-31 19:50:08.000000 glayout-0.0.4/setup.py
```

### Comparing `glayout-0.0.3/PKG-INFO` & `glayout-0.0.4/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: glayout
-Version: 0.0.3
-Summary: Fully Open-Source Autonomous SoC Synthesis using Customizable Cell-Based Synthesizable Analog Circuits
-Home-page: https://github.com/idea-fasoc/OpenFASOC
-Author:  msaligane
-Author-email: mehdi@umich.edu
-License: MIT
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
+Version: 0.0.4
+Summary: A human language to analog layout API with support for different technologies.
+Home-page: https://github.com/idea-fasoc/OpenFASOC/tree/main/openfasoc/generators/glayout
+Author: Ali Hammoud, Harsh Khandeparkar, Vijay Shankar, Chetanya Goyal, Sakib Pathen, Arlene Dai, Ryan Wans, Mehdi Saligane
+Author-email: alibilal@umich.edu, Harsh, vijayshankar.renganathan@analog.com, Chetanya, spathen@umich.edu, arlendai@umich.edu, Ryan, mehdi@umich.edu
 Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 All functions, classes, etc have a help docustring. See python help() for specific questions
 
 - [Installation](#installation)
 - [Glayout](#glayout)
@@ -35,14 +33,30 @@
       - [PortTree](#porttree)
     - [Snap to 2x grid](#snap-to-2x-grid)
     - [Mimcaps Implementation](#mimcaps-implementation)
     - [DRC](#drc)
     - [LVS, and Labeling Issues](#lvs-and-labeling-issues)
     - [Addressing Complicated Requirments with Default Decorators](#addressing-complicated-requirments-with-default-decorators)
   - [API overview](#api-overview)
+- [Natural Language Processing](#natural-language-processing)
+  - [Standard Components](#standard-components)
+    - [NMOS](#nmos)
+    - [PMOS](#pmos)
+    - [MIMCAP](#mimcap)
+    - [MIMCAP Array](#mimcap-array)
+    - [Differential Pair](#differential-pair)
+  - [Strict Syntax Commands](#strict-syntax-commands)
+    - [Import Command](#import-command)
+    - [Create Parameters Command](#create-parameters-command)
+    - [Place Command](#place-command)
+    - [Move Command](#move-command)
+    - [Route Command](#route-command)
+  - [Non-Standard Components Which can be Imported](#non-standard-components-which-can-be-imported)
+    - [CrossCoupledInverters](#crosscoupledinverters)
+  - [StrictSyntax Style Guide](#strictsyntax-style-guide)
 
 # Installation
 You must be running python3.10 or later. 
 - Run `python3 -m pip install -r requirements.txt` in the gdsfactory-gen directory
 - open Klayout
   - go to Tools -> Manage Packages
   - under "Install New Packages" search for "klive"
@@ -58,20 +72,20 @@
 ### Generic Layers
 Almost all CMOS technologies have some version of basically the same layers, some of which are: “active/diffusion”, ”metal contact”, “metal 1”, “via1”, …etc. The layer description format of tuple(integer, integer) is standard. The idea of a generic layer is to map the standard layer names to a specific tuple(integer, integer) depending on the technology. For example, a generic layer present in most technologies is “metal 2”. The sky130 version of “metal 2” is the integer tuple (68, 20). The gf180 version of “metal 2” is the integer tuple (34,0). Importantly, the designer does not use or care about the value of the integer tuple. The designer only cares about the layer it represents, which they can always access in python from the generic name.  
 MappedPDK provides the designer with all the generic layers necessary, some of which are: “diffusion”, “dnwell”, “nwell”, “pwell”, “p+s/d”, “n+s/d”, “mcon”...etc. MappedPDK guarantees that regardless of which technology is represented ‘under the hood’ and what the value of the tuple(integer, integer), these layers will be accessible by the same names. The designer can access generic layers using the following syntax (for example):  
 `MappedPDK.get_glayer(“metal 2”)`  
 This “get_glayer” instance method of the MappedPDK takes the generic layer name and returns the tuple(integer, integer) specific to the technology. A MappedPDK object supports mappings for all design layers necessary. The BEOL generic layers support a metal stack met1-met5. Because metal stacks and some layers are technology dependent, the MappedPDK contains the “MappedPDK.verify_glayers()” method for verifying the presence of layers. For example, if a technology BEOL contains met1-met2, but a cell requires met3, it is possible for the cell generator to verify at runtime that the technology contains met3.
 
 **BEOL Example Generic Layer Mappings**
-| Generic Layer Name | sky130 | gf180 |
-| :-: | :-: | :-: |
-|mcon| (66,44) | (33,0) |
-|met1| (67,20) | (34,0) |
-|via1| (67,44) | (35,0) |
-|met2| (68,20) | (36,0) |
+| Generic Layer Name | sky130  | gf180  |
+| :----------------: | :-----: | :----: |
+|        mcon        | (66,44) | (33,0) |
+|        met1        | (67,20) | (34,0) |
+|        via1        | (67,44) | (35,0) |
+|        met2        | (68,20) | (36,0) |
 
 
 ### Generic Rule Guide
 Almost all CMOS technologies have some version of basically the same three rules: “min_separation”, “min_enclosure”, and “min_width” (or “width” for via layers). Hundreds of rules arise by prescribing one of these three rules between combinations of layers. For example, there may be a rule which requires a “min_enclosure” between “via1” and “metal 2”. There can also be “self rules” or rules describing a requirement between a layer and itself; most “min_width” rules are self rules. An example of a “self rule” between “metal 2” and “metal 2” would be the “min_width” rule.  
 The description of CMOS rules provided in the above paragraph fits very well within a mathematical graph. Layers can be thought of as vertices in the graph. Rules describe relationships between layers; rules can be thought of as edges in the graph. A “self rule” can be thought of as a “self edge” in the graph (an edge connecting a vertex to itself). This graph can be described mathematically as an undirected graph.  
 **figure here of example rule graph**  
 To greatly simplify the rule graph, context dependent rules (sometimes referred to as lambda rules) are eliminated by taking the worst case value for each rule. This allows the designer to lookup rules without providing any additional context of surrounding layer geometry (usually required for dependent rules).  
@@ -91,34 +105,34 @@
 `from gdsfactory.cell import cell`   
 The MappedPDK.get_glayer and MappedPDK.get_grule methods enable the construction of DRC clean layouts programmatically. However, it is the responsibility of the Cell factory programmer to ensure that the proper rules and layer checks are executed. **The quality of the programmer is the quality of the cell.**
 ### Via Stack Generator
 The only stand alone cell (cell factory which does not call other cell factories) in the glayout package is the via stack. Cell factories generally follow a similar programming procedure, so via stack provides a good introduction to the cell factory structure.  
 Like all cells, via stack takes as the first argument a MappedPDK object. There are two other required arguments which specify the generic layers to create the via stack between; the order in which these “glayers” (another name for generic layers) are provided does not matter. There are also several optional arguments providing more specific layout control. To explain this cell, the following function call will be assumed:  
 `via_stack(GF180_MappedPDK, “active”, “metal 3”)` OR  `via_stack(GF180_MappedPDK, “metal 3”, “active”)`  
 Most cells start by running layer error checking. The via stack must verify that the provided MappedPDK contains both glayers provided and both glayers provided can be routed between. For example, it is usually not possible to route from “nwell” without an “n+s/d” implant, so if one of the layers provided is “nwell”, via stack raises an exception. Additionally, via stack must verify that all layers in between the provided glayers are available in the pdk. In this case, the required glayers are: “active”, “metal contact”, “metal 1”, “via 1”, “metal 2”, via 2”, and “metal 3”. For the passed MappedPDK (GF180), all required glayers are present, but in the case that a glayer is not present, via stack raises an exception.  
-layer error checking is done with [`pdk.has_required_glayers(glayers_list)`](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/pdk/mappedpdk.py#L142).  
+layer error checking is done with [`pdk.has_required_glayers(glayers_list)`](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/flow//pdk/mappedpdk.py#L142).  
 The via stack then loops through these layers, placing them one at a time. To legally size and place each layer, via stack must consider “min_enclosure” and “width” rules for vias and metals. For example, to lay the “active” layer, the “metal contact” “width” and the “metal contact” to “active” “min_enclosure” rules must be considered. To lay the “metal 1” layer, the “min_enclosure” and “width” rules of both the via above and the via below “metal 1” must be considered. The programmer of the generic cells must consider all relevant rules to produce a legal layout. Rules are accessed in cell code using the `MappedPDK.get_grule` method.
 ### Routing
 Routing utilities are required to create complicated hierarchical designs. At the backend of routing is the gdsfactory “Port” object. Fundamentally, ports describe a polygon edge. Ports include center, width, and orientation of the edge, along with other attributes and utility methods. The glayout routing functions operate to create paths between ports.  
 As described with the via stack example above, the checks and sizings necessary for legal layout are executed in the cell generator. Glayout routing functions do not need to understand cell context; for this reason, routing functions are called “dumb routes”. There are three “dumb route” utilities: straight route, L route, and C route. Dumb routes are simple, but contain optional arguments which allow for precise control over created paths. The default path behavior is easy to predict and will generally make the most reasonable decisions if no direction is provided.   
 For example, Straight route creates a straight path directly between two ports. If the two provided ports are not collinear or have different orientations, the function will by default route from the first port to the imaginary line stretching perpendicularly from the second port. By default, the route will begin on the same layer as the first port and will lay a via stack if necessary at the second port. If two ports are parallel, Straight route will raise an exception.
 
 **Straight Route Default Behavoir:**
 ![straight route default behavoir](docs/straight_route_def_beh.png)  
 
 L route and C route also create simple paths. L route creates an L shaped route (two straight paths perpendicular) and C route creates a C shaped route (two parallel paths connected by a straight path).  
 ### PDK Agnostic Hierarchical Cells
 All cells other than the via stack contain hierarchy. Combining hierarchy and careful routing allows for clean layouts while increasing complexity. 
-#### Example 1: [via_array](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/primitives/via_gen.py#L180)
-The most basic hierarchical cell is the [via_array](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/primitives/via_gen.py#L180). Via array is composed of via stacks and has a similar interface to the via stack generator, but additionally accepts a size argument. The array spacing computation is another example of the programmers role in creating DRC clean layout. After error checking, the via array program creates the via stack single element that will be copied to create the array. Then, the generator loops through each layer and uses the gdsfactory component.extract method to get the dimension of that layer in the via stack; The min spacing for that layer is `pdk.get_grule(layer)["min_separation"] + 2*layer_dim`. After looping through the entire array, The maximum seperation is the correct spacing to use.  
-#### Example 2: [tapring](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/primitives/guardring.py)
-tapring produces a substrate / well tap rectanglular ring that legally enclose a rectangular shape. `gdsfactory.component.rectangular_ring` is used along with glayout [via_array](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/primitives/via_gen.py#L180). The ring is always of minimum width and legalizing the ring is easy because via_array does most of the work. Special care is taken at the corners to ensure min spacing between adjacent metal layers is not below min_separation. Although not currently implemented, error checking for this ring should check the size is not too small (separation between edges is not legal).  
+#### Example 1: [via_array](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/flow/primitives/via_gen.py#L180)
+The most basic hierarchical cell is the [via_array](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/flow/primitives/via_gen.py#L180). Via array is composed of via stacks and has a similar interface to the via stack generator, but additionally accepts a size argument. The array spacing computation is another example of the programmers role in creating DRC clean layout. After error checking, the via array program creates the via stack single element that will be copied to create the array. Then, the generator loops through each layer and uses the gdsfactory component.extract method to get the dimension of that layer in the via stack; The min spacing for that layer is `pdk.get_grule(layer)["min_separation"] + 2*layer_dim`. After looping through the entire array, The maximum seperation is the correct spacing to use.  
+#### Example 2: [tapring](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/flow/primitives/guardring.py)
+tapring produces a substrate / well tap rectanglular ring that legally enclose a rectangular shape. `gdsfactory.component.rectangular_ring` is used along with glayout [via_array](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/flow/primitives/via_gen.py#L180). The ring is always of minimum width and legalizing the ring is easy because via_array does most of the work. Special care is taken at the corners to ensure min spacing between adjacent metal layers is not below min_separation. Although not currently implemented, error checking for this ring should check the size is not too small (separation between edges is not legal).  
 Generators should be made as generic as possible. In this case, tapring can produce either a p-tap or n-tap ring. Glayers are just strings and they can be passed to functions as arguments. Also, you glayer variables can be passed directly to `pdk.get_grule(glayer_var)`.
-#### Example 3: [fet](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/primitives/fet.py)
-The most important component factory in glayout is the [multiplier](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/primitives/fet.py#L61) because it handles the difficult task of creating legal transistors. By passing the source/drain layer (either "p+s/d" or "n+s/d") multiplier code is reused to create nmos and pmos transistors. arrays of multipliers can be created to allow for transistors with several multipliers. read the help docustring for all functions in [fet.py](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/primitives/fet.py)
+#### Example 3: [fet](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/flow/primitives/fet.py)
+The most important component factory in glayout is the [multiplier](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/flow/primitives/fet.py#L61) because it handles the difficult task of creating legal transistors. By passing the source/drain layer (either "p+s/d" or "n+s/d") multiplier code is reused to create nmos and pmos transistors. arrays of multipliers can be created to allow for transistors with several multipliers. read the help docustring for all functions in [fet.py](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/flow/primitives/fet.py)
 
 ## Advanced Topics
 The following topics are only neccessary if you want to code with glayout, but are not neccessary for a basic understanding of glayout.
 ### Cells and PDK.activate()
 All cell factories should be decorated with the `@cell` decorator which can be imported from gdsfactory with `from gdsfactory.cell import cell`. You must also call pdk.activate() for cells to correctly work. This is related to caching, gds/oasis write settings, default decorators, etc.
 ### Important GDSFactory Notes and Glayout Utilities
 The GDSFactory API is extremely versatile and there are many useful features. It takes some experience to learn about all features and identify the most useful tools from GDSFactory. GDSFactory serves as the backend GDS manipulation library and as an object oriented tool kit with several useful classes including: Components, Component References, and Ports. There are also common shapes as Components in GDSFactory such as rectangles, circles, rectangular_rings, etc. To automate common tasks that do not fit into GDSFactory, Glayout includes many utility functions. The most important of these functions are also addressed here.  
@@ -133,63 +147,63 @@
 	- Component booleans: see the gdsfactory documentation for how to run boolean operations of components.
 	- Component.write_gds(): write the gds to disk
 	- Component.bbox: return bounding box of the component (xmin,ymin),(xmax,ymax). Glayout has an evaluate_bbox function which return the x and y dimensions of the bbox
 	- insertion operator: `ref = Component << Component_to_add`
 	- Component.add(): add an one of several types to a Component. (more flexible than << operator)
 	- Component.ref()/.ref_center(): return a reference to a component
 
-It is not possible to move Components in GDSFactory. GDSFactory has a Component cache, so moving a component may invalidate the cache, but there are situations where you want to move a component; For these situations, use the glayout [move](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/pdk/util/comp_utils.py#L24), [movex](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/pdk/util/comp_utils.py#L63), [movey](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/pdk/util/comp_utils.py#L73) functions.
+It is not possible to move Components in GDSFactory. GDSFactory has a Component cache, so moving a component may invalidate the cache, but there are situations where you want to move a component; For these situations, use the glayout [move](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/flow/pdk/util/comp_utils.py#L24), [movex](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/flow/pdk/util/comp_utils.py#L63), [movey](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/flow/pdk/util/comp_utils.py#L73) functions.
 
 - Component references are pointers to components. They have many of the same methods as Components with some additions.
 	- ComponentReference.parent: the Component which this component reference points to
 	- ComponentReference.movex, movey, move: you can move ComponentReferences
 	- ComponentReference.get_ports_list(): get a list of ports in the component.
 Ports are edge descriptions.
 
 To add a ComponentReference to a Component, you cannot use the insertion operator. Use the Component.add() method.
 
 - A port describes a single edge of a polygon. The most useful port attributes are **width, center tuple(x,y), orientation (degrees), and layer of the edge**. 
     - For example, the rectangle cell factory provided in gdsfactory.components.rectangle returns a Component type with the following port names: e1, e2, e3, e4.
     	- e1=West, e2=North, e3=East, e4=South. The default naming scheme of ports in GDSFactory is not descriptive
-    	- use glayout [rename_ports_by_orientation](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/pdk/util/port_utils.py#L67), [rename_ports_by_list](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/pdk/util/port_utils.py#L91) functions and see below for port naming best practices guide
-    	- glayout [get_orientation](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/pdk/util/port_utils.py#L124): returns the letter (N,E,S,W) or degrees of orientation of port.  by default returns the one you do not have. see help.
-    	- glayout [assert_port_manhattan](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/pdk/util/port_utils.py#L159): assert that a port or list or ports have orientation N, E, S, or W
-    	- glayout [assert_ports_perpindicular](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/pdk/util/port_utils.py#L181): assert two ports are perpindicular
-    	- glayout [set_port_orientation](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/pdk/util/port_utils.py#L181): return new port which is copy of old port but with new orientation
-    	- glayout [set_port_width](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/pdk/util/port_utils.py#L202): return a new port which is a copy of the old one, but with new width
+    	- use glayout [rename_ports_by_orientation](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/flow/pdk/util/port_utils.py#L67), [rename_ports_by_list](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/flow/pdk/util/port_utils.py#L91) functions and see below for port naming best practices guide
+    	- glayout [get_orientation](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/flow/pdk/util/port_utils.py#L124): returns the letter (N,E,S,W) or degrees of orientation of port.  by default returns the one you do not have. see help.
+    	- glayout [assert_port_manhattan](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/flow/pdk/util/port_utils.py#L159): assert that a port or list or ports have orientation N, E, S, or W
+    	- glayout [assert_ports_perpindicular](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/flow/pdk/util/port_utils.py#L181): assert two ports are perpindicular
+    	- glayout [set_port_orientation](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/flow/pdk/util/port_utils.py#L181): return new port which is copy of old port but with new orientation
+    	- glayout [set_port_width](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/flow/pdk/util/port_utils.py#L202): return a new port which is a copy of the old one, but with new width
 
-A very important utility is [align_comp_to_port](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/pdk/util/comp_utils.py#L83): pass a component or componentReference and a port, and align the component to any edge of the port.
+A very important utility is [align_comp_to_port](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/flow/pdk/util/comp_utils.py#L83): pass a component or componentReference and a port, and align the component to any edge of the port.
 
 ### Port Naming Best Practices Guide
 As previously pointed out, the default naming of ports in GDSFactory is not descriptive. By default gdsfactory.components.rectangle returns ports e1 (West port), e2 (North port), e3 (East port), e4 (South port). Additionally, complicated hiearchies can result in thousands of ports, so organizing ports is a neccessity. The below best practices guide should be used to organize ports
 - Ports use the "\_" syntax. Think of this like a directory tree for files. Each time you introduce a new level of hiearchy, you should add a prefix + "\_" describing the cell. 
 	- For example, adding a via_array to the edge of a tapring, you should call
 `tapring.add_ports(via_array.get_ports_list(),prefix="topviaarray_")`
 	- The port rename functions look for the "\_" syntax. You can NOT use the port rename functions without this syntax.
 - The last 2 characters of a port name should "\_" followed by the orientation (N, E, S, or W)
-	- you can easily achieve this by calling glayout [`rename_ports_by_orientation`](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/pdk/util/port_utils.py#L67) before returning a component (just the names end with "\_" before calling this function)
+	- you can easily achieve this by calling glayout [`rename_ports_by_orientation`](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/flow/pdk/util/port_utils.py#L67) before returning a component (just the names end with "\_" before calling this function)
 - **USE PORTS**: be sure to correctly add and label ports to components you make because you do not know when they will be used in other cells. 
 
 #### PortTree
-The [PortTree](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/pdk/util/port_utils.py#L232) class is designed to assist in finding ports and understanding port structure. Initialize a PortTree by calling [`PortTree(Component or ComponentReference)`](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/pdk/util/port_utils.py#L245). The PortTree will internally construct a directory tree structure from the Component's ports. You can use [`PortTree.print()`](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/pdk/util/port_utils.py#L304) to print this whole structure for a nice figure explaining a Component's ports. See the example print output from a via_stack component below:
+The [PortTree](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/flow/pdk/util/port_utils.py#L232) class is designed to assist in finding ports and understanding port structure. Initialize a PortTree by calling [`PortTree(Component or ComponentReference)`](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/flow/pdk/util/port_utils.py#L245). The PortTree will internally construct a directory tree structure from the Component's ports. You can use [`PortTree.print()`](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/flow/pdk/util/port_utils.py#L304) to print this whole structure for a nice figure explaining a Component's ports. See the example print output from a via_stack component below:
 
 **PortTree of a via_stack:**
 ![PortTree example](docs/PortTreeExample.png)
 
 ### Snap to 2x grid
 All rules (when creating a MappedPDK) and all user provided float arguments must be snapped to 2*grid size. This is because it is possible to center a component. Centering a component which has a dimension on grid may result in off grid polygons. You can snap floating point values to grid easily by calling `pdk.snap_to_2x_grid()`. You should also take care to snap to 2xgrid whenever you see it is neccessary while writing generator code. For example, most generators which take a size(xdim: float, ydim: float) argument should snap to 2xgrid.
 ### Mimcaps Implementation
 Although many technolgies have 2 or more mimcap options, there is currently only 1 mimcap option supported. When creating a mapped pdk, you specify the cap metal layer as a generic layer, but you specify the metal above and metal below the cap met as part of the DRC rule set for `pdk.get_grule("capmet")`. You can access the metal above capmet with `pdk.get_grule(capmet)["capmettop"]`.
 ### DRC
 If the system has klayout installed and you provide a klayout lydrc script for your MappedPDK, you can run DRC from python by calling pdk.drc(Component or GDS). The return value is a boolean (legal or not legal) and a lyrdb (xml format) file is written describing each DRC error. This file can be opened graphically in klayout with the following syntax `klayout layout.gds -m drc.lyrdb`
 ### LVS, and Labeling Issues
 There are no glayers for labeling or pins, all cells are generated without any labels. You can easily add pins to your component manually after glayout write the gds, or by using ports, you can write a function for adding labels and pins. See [sky130_nist_tapeout example function](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/tapeout_and_RL/sky130_nist_tapeout.py#L97). 
 ### Addressing Complicated Requirments with Default Decorators
 A python decorator is a function (the decorator) is a function which is called on another function. It can be used to enhance the features of a function. With GDSFactory Pdk (and MappedPDK objects) you can define a default decorator which runs on any cell factory (cell factories must be decorated with the `@cell` decorator). The default decorator you define runs in addition to the `@cell` decorator. The defined default_decorator should accept as argument a Component and return a Component.  
-This should be used when dealing with PDK specfic requirments that do not fit into the MappedPDK framework. For example, sky130 has a NPC (nitride poly cut) layer which **must** be used wherever licon (local interconnect contact) is laid over poly. It does not make sense to modify MappedPDK to add a generic NPC layer AND modify all cell factories; sky130 is unqiue in this requirment, so modifying MappedPDK/all cell factories would make glayout less generic. Instead, we define a default_decorator [`sky130_add_npc(Component) -> Component`](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/pdk/sky130_mapped/sky130_add_npc.py). This function uses booleans to add npc anywhere licon is laid over poly (it also joins NPC polygons if they are closer than the NPC min separation rule). Layers and rules in this technology specific function are hard coded because this decorator will only run for sky130 is the active pdk (this is one reason why you must be sure that pdk is activated).
+This should be used when dealing with PDK specfic requirments that do not fit into the MappedPDK framework. For example, sky130 has a NPC (nitride poly cut) layer which **must** be used wherever licon (local interconnect contact) is laid over poly. It does not make sense to modify MappedPDK to add a generic NPC layer AND modify all cell factories; sky130 is unqiue in this requirment, so modifying MappedPDK/all cell factories would make glayout less generic. Instead, we define a default_decorator [`sky130_add_npc(Component) -> Component`](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/flow/pdk/sky130_mapped/sky130_add_npc.py). This function uses booleans to add npc anywhere licon is laid over poly (it also joins NPC polygons if they are closer than the NPC min separation rule). Layers and rules in this technology specific function are hard coded because this decorator will only run for sky130 is the active pdk (this is one reason why you must be sure that pdk is activated).
 
 ## API overview
 This section provides a high-level overview of all functions in glayout. See **docs** (TODO) printed docustrings of all files.
 
 
 - glayout: 
   - generators
@@ -234,9 +248,167 @@
           - get_padding_points_cc: get points of a rectangle which pads (with some extra space optionally) a component. (e.g. lay p+s/d over diffusion with padding=0.2um)
           - to_decimal: convert a float or list of float (or decimal) to python decimal
           - to_float: convert decimal or list of decimal (or float) to python float
         - port_utils.py
         - print_rules.py
         - snap_to_grid.py
         - component_array_create.py
+# Natural Language Processing
+In addition to python code, there is also natural language capabilities within Glayout. Glayout strictsyntax is a command language for producing analog circuit layout. Component placement in Analog layout is drawing the geometric shapes representing various Components. Routing is the process of connecting these Components by drawing metal lines between them. Glayout strictsyntax allows the designer to place, move, and connect circuit Components without needing to draw them, rather with strictsyntax the designer can describe them in simple words and with simple commands. The Glayout runtime interprets these commands and will automatically place, move, and route the final layout.
+
+To get started with the glayout runtime, you can create a basic run.py script using the following:
+```
+import argparse
+from glayout.syntaxer.dynamic_load import run_session
+from pathlib import Path
+
+if __name__ == "__main__":
+    parser = argparse.ArgumentParser(description="Manage, interact, and run conversation sessions.")
+    parser.add_argument(
+        "-l",
+        "--load_conversation",
+        type=Path,
+        help="Specify the file path to load a previous conversation",
+    )
+    parser.add_argument(
+        "-r",
+        "--restore_and_exit",
+        action='store_true',
+        help="Restore the conversation state and exit",
+    )
+    args = parser.parse_args()
+    run_session(args.load_conversation, args.restore_and_exit)
+```
+By entering `python run.py` with no arguments to the above script you can begin creating layout with the strictsyntax.
+
+Components are predesigned circuits which can be used as building blocks to create larger circuits. Components are highly modular and have many parameters which can be configured when they are placed. Placing a Component is also known as instantiating the Component. Instances must be given a name. The instance name is called the ComponentRef. Components are also hierarchical, meaning that a Component can be made up of many sub-Components. Also, after making a circuit with Glayout, it can be used in the future as a Component in a larger circuit.
+
+Components can be connected together through a process called routing. Components include several Ports. Ports serve as nodes on Components. Ports are used to create connections (also known as routes) between different Components in a circuit. Ports represent the input or output nodes for Components in the layout and act like an interface to the Component. In the geometry of the layout, Ports correspond to edges of nodes. 
+Ports are accessed through an organized naming syntax. The names correspond to the function of the Port. For example, MOS Field-Effect Transistors (MOSFETs) have three main nodes: drain, gate, and source. Remember, each Port corresponds to an edge in layout, so they always end with a direction indicator. Direction indicators are North (N), East (E), South (S), or West (W). Indicators N, E, S, W are for specifying which edge of the node we are referring to. For example, if we want to refer to the west edge of the drain node, we would use the port name “ComponentRef_drain_W”, replacing ComponentRef with the name of the Component instance.
+
+## Standard Components
+There are several existing components which are part of the Glayout runtime. These components are described below and do not require any imports. Note that it is also possible to import other Components.
+
+### NMOS
+Nmos is an n-type mosfet transistor. It is also referred to as nmos, n-type, or nfet. It has the following parameters which are configurable when you place the component: 
+length: a float parameter specifying the transistor length
+width: a float parameter specifying the width of a single transistor
+fingers: an integer parameter which multiplies the width. For example, if fingers is 3, then the size will be 3 times the width.
+multipliers: An integer parameter specifying how many rows of fingers to place. Each row is equivalent to width*fingers in size, so that the total size is multipliers*width*fingers. Default is 1.
+with_tie: True or False, specifies if a bulk tie is required. Set this true unless the designer specifies otherwise.
+with_substrate_tap: True or False. If True, then add a substrate tap on the very outside perimeter of nmos. Set this to False unless the designer specifies otherwise.
+with_dummy: When True, specifies dummy devices should be added to the edges of the transistor. You should set this to True unless the designer specifies otherwise. 
+with_dnwell: boolean parameter specifying to use deep nwell if True. You should usually set this to False unless the designer specifies otherwise.
+rmult: make metal connections within the nmos component wider. Specify this as 1 unless the designer asks to make routing wider or use wider metals.
+
+The main nmos ports correspond to source, gate, and drain nodes. Each underscore in a port name represents a level of hierarchy. For example, we start with the ComponentRef which is the name of the nmos Component instance. Then we specify one of the nodes from drain, gate, or source. Lastly we specify a direction indicator from N, E, S, W. The following are just some examples of the valid nmos ports:
+ComponentRef_source_N
+ComponentRef_drain_W
+ComponentRef_source_E
+ComponentRef_gate_S
+
+### PMOS
+Pmos is a p-type mosfet transistor. It is also referred to as pmos, pfet or p-type. It has the following parameters which are configurable when you place the component: 
+length: a float parameter specifying the transistor length
+width: a float parameter specifying the width of a single transistor
+fingers: an integer parameter which multiplies the width. For example, if fingers is 3, then the size will be 3 times the width.
+multipliers: An integer parameter specifying how many rows of fingers to place. Each row is equivalent to width*fingers in size, so that the total size is multipliers*width*fingers. Default is 1.
+with_tie: True or False, specifies if a bulk tie is required. Set this true unless the designer specifies otherwise.
+with_substrate_tap: True or False. If True, then add a substrate tap on the very outside perimeter of nmos. Set this to False unless the designer specifies otherwise.
+with_dummy: When True, specifies dummy devices should be added to the edges of the transistor. You should set this to True unless the designer specifies otherwise. 
+dnwell: Note that this is different from the nmos “width_dnwell” argument, but it serves a similar purpose. When dnwell is set to True it adds a deep nwell to the pmos transistor. You should set this to False unless the designer specifies otherwise. The designer may say they want triple well isolation, in which case you should set this as True.
+rmult: make metal connections within the pmos component wider. Specify this as 1 unless the designer asks to make routing wider or use wider metals.
+
+Here are just some examples of the valid pmos ports:
+ComponentRef_gate_S 
+ComponentRef_source_E
+ComponentRef_drain_W
+
+### MIMCAP
+The mimcap is a capacitor. The mimcap takes only one argument which can be configured when the component is placed:
+size: a tuple of floating point numbers like (2.1, 3.7) denoting the x and y dimension of the capacitor. The default size is (5.0, 5.0)
+
+The mimcap has the following 4 ports:
+ComponentRef_top_met_N
+ComponentRef_top_met_E
+ComponentRef_top_met_S
+ComponentRef_top_met_W
+
+### MIMCAP Array
+There is also a mimcap_array (also written as mimcap array) which automatically places and routes several mimcaps together. The mimcap_array takes the following parameters:
+size: a tuple of floating point numbers denoting the x and y dimension of the capacitor.
+columns: the number of columns in the array
+rows: the number of rows in the array
+
+
+### Differential Pair
+A differential pair is available, which is referred to as diff_pair or diff pair. The diff_pair is a differential pair Component which is created using 2 nfet Components. The nfet Components are referred to as “A” and “B” respectively. The diff pair has the following configurable parameters:
+length: a float parameter specifying the length of all transistor Components part of the diff pair.
+width: a float parameter specifying the width of all transistor Components part of the diff pair.
+fingers: an integer parameter which modifies the number of fingers in all transistor Components which are part of the diff pair.
+
+The following are just some examples of the valid ports for diff_pair:
+ComponentRef_A_source_S
+ComponentRef_A_drain_N
+ComponentRef_B_source_S
+ComponentRef_A_gate_E
+ComponentRef_B_drain_W
+ComponentRef_B_gate_E
+
+## Strict Syntax Commands
+Strict syntax supports the commands listed below. Note I have left square brackets [] around places where specific command calls should fill in information.
+### Import Command
+Sometimes you want to use Components which are not included in the Glayout runtime. You do this using the import command. The import command automatically searches for the Component path, so you do not need to specify a path. All you need is to specify the Component you want. The general syntax for importing a Component is:
+import [Component]
+For example, to import a CrossCoupledInvereters, the user could do the following:
+import CrossCoupledInverters
+### Create Parameters Command
+You generally want to make the Components as parameterized as possible so that they are highly modular and customizable. To do this you need to create parameters. You can create parameters with the following general command syntax:
+create a [Type] parameter called [ParameterName]
+Here are some examples using the create parameter command:
+create a float parameter called device_width 
+create a int parameter called device_fingers
+### Place Command
+The general syntax for the place command is below. I have left square brackets around names of Components or ComponentRefs or parameters that should be inserted when using the command. When you insert parameters, you can specify them as a comma separated list.
+place a [Component] called [ComponentRef] with [parameters]
+An example of using the place command is as follows:
+place a nmos called m1 with width 1.0, length 2.0, fingers 2, rmult 1, multipliers 3, with_substrate_tap False, with_tie True, with_dummy True, with_dnwell False
+The parameter list also supports passing existing parameter names instead of values.
+### Move Command
+By default all placed Components are centered at the origin. Obviously, if we place more than one ComponentRef we need to move some of them so that they are not overlapping. To emphasize, if more than one ComponentRef is placed, at least one ComponentRef must be moved to avoid overlapping. To do this, use the move command. The move command allows you to specify relative movements relative to other placed ComponentRefs.
+The general relative move syntax is as follows:
+move [ComponentRef we are moving] [relative direction] [relative to ComponentRef]
+Directions include above, below, right, or left.
+Here is an example of using relative move (say we have a ComponentRef called m1 and another called m2):
+move m1 below m2
+### Route Command
+Routes are connections between 2 Ports. There are 4 types of routes: straight_route, c_route, L_route, and smart_route. Unless you are very confident, always use smart_route. Only under special circumstances you can specifcy a different route type, but in almost all cases smart_route is the best option. smart_route can almost always optimally route between two ports. There are also some rules you can use to determine the Port orientations. If you are routing between ComponentRefs which are left or right of each other, then select Ports which are on the adjacent sides. If you are routing between ComponentRefs above or below each other, then select Ports that are both on the East side or both on the West side. The general route syntax is as follows:
+route between [Port1] and [Port2] using [route_type]
+For example, if we have a nmos ComponentRef called m1 which is to the west of a pmos ComponentRef called m2, an example route command to connect the sources of both would be as follows:
+route between m1_source_E and m2_source_W using smart_route
+Note that the first part of the portname is the ComponentRef name. Also, notice why the E and W ports were chosen. The nmos ComponentRef called m1 is to the left of the pmos ComponentRef called m2, so the sides adjacent to each other are the east side of m1 and west side of m2. If m1 was above m2, then I could have selected both East Ports or both West Ports as follows:
+route between m1_source_E and m2_source_E using smart_route
+or
+route between m1_source_W and m2_source_W using smart_route
+
+## Non-Standard Components Which can be Imported
+### CrossCoupledInverters
+CrossCoupledInverters is available to use and can be imported with:
+import CrossCoupledInverters
+The cell is made up of 4 transistor Components. The top two transistors are pfets and the bottom two transistors are nfets. 
+This cell implements the following prepackage circuit for easy import:
+CrossCoupledInverters includes two inverters. Inverters are composed of an nfet and pfet with their gates shorted with each other (the input of an inverter) and their drains shorted with each other (the output of an inverter). The inputs of the inverters are also shorted, with the sources of the nfets shorted with each other and the drains of the pfets shorted with each other. Importing the cell allows for it to be placed without any extra work. The CrossCoupledInverters has the following parameters:
+pfet_width: A float parameter specifying the width of the pmos Components
+nfet_width: A float parameter specifying the width of the nmos Components
+length: A float parameter specifying the length of all transistor Components
+numfingers: An int parameter specifying the number of fingers in all transistor Components
+
+The west (or left) inverter generally has the following port naming conventions:
+ComponentRef_top,bottom_A_source,drain,gate_N,E,S,W
+The west (or right) inverter generally has the following port naming conventions:
+ComponentRef_top,bottom_B_source,drain,gate_N,E,S,W
+Where top refers to the inverter’s pmos Component and bottom refers to the inverters nmos Component. A or B refers to the inverter, with A representing the west inverter and B representing the east inverter.
+
+## StrictSyntax Style Guide
+You should always follow this order of commands when creating a Component with strictsyntax: Start by importing any required Components, then create any required parameters, then place all required ComponentRefs with their respective parameters, then move all ComponentRefs to their final positions relative to one another, and lastly route between ComponentRefs.
```

### Comparing `glayout-0.0.3/glayout/components/diff_pair.py` & `glayout-0.0.4/glayout/flow/components/diff_pair.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,45 @@
+from typing import Optional, Union
+
 from gdsfactory.cell import cell
 from gdsfactory.component import Component, copy
 from gdsfactory.components.rectangle import rectangle
-from glayout.primitives.fet import nmos, pmos
-from glayout.pdk.mappedpdk import MappedPDK
-from typing import Optional, Union
 from gdsfactory.routing.route_quad import route_quad
 from gdsfactory.routing.route_sharp import route_sharp
-from glayout.routing.c_route import c_route
-from glayout.routing.straight_route import straight_route
-from glayout.pdk.util.comp_utils import movex, movey, evaluate_bbox, align_comp_to_port
-from glayout.pdk.util.port_utils import rename_ports_by_orientation, rename_ports_by_list, add_ports_perimeter, print_ports, get_orientation, set_port_orientation
-from glayout.primitives.via_gen import via_stack
-from glayout.primitives.guardring import tapring
-from glayout.pdk.util.snap_to_grid import component_snap_to_grid
-from glayout.spice import Netlist
+from glayout.flow.pdk.mappedpdk import MappedPDK
+from glayout.flow.pdk.util.comp_utils import align_comp_to_port, evaluate_bbox, movex, movey
+from glayout.flow.pdk.util.port_utils import (
+    add_ports_perimeter,
+    get_orientation,
+    print_ports,
+    rename_ports_by_list,
+    rename_ports_by_orientation,
+    set_port_orientation,
+)
+from glayout.flow.pdk.util.snap_to_grid import component_snap_to_grid
+from glayout.flow.placement.common_centroid_ab_ba import common_centroid_ab_ba
+from glayout.flow.primitives.fet import nmos, pmos
+from glayout.flow.primitives.guardring import tapring
+from glayout.flow.primitives.via_gen import via_stack
+from glayout.flow.routing.c_route import c_route
+from glayout.flow.routing.smart_route import smart_route
+from glayout.flow.routing.straight_route import straight_route
+from glayout.flow.spice import Netlist
+
 
 def diff_pair_netlist(fetL: Component, fetR: Component) -> Netlist:
 	diff_pair_netlist = Netlist(circuit_name='DIFF_PAIR', nodes=['VP', 'VN', 'VDD1', 'VDD2', 'VTAIL', 'B'])
 	diff_pair_netlist.connect_netlist(
 		fetL.info['netlist'],
 		[('D', 'VDD1'), ('G', 'VP'), ('S', 'VTAIL'), ('B', 'B')]
 	)
 	diff_pair_netlist.connect_netlist(
 		fetR.info['netlist'],
 		[('D', 'VDD2'), ('G', 'VN'), ('S', 'VTAIL'), ('B', 'B')]
 	)
-
 	return diff_pair_netlist
 
 @cell
 def diff_pair(
 	pdk: MappedPDK,
 	width: float = 3,
 	fingers: int = 4,
@@ -129,15 +139,15 @@
 	# cross gate route top with c_route. bar_minus ABOVE bar_plus
 	get_left_extension = lambda bar, a_topl=a_topl, diffpair=diffpair, pdk=pdk : (abs(diffpair.xmin-min(a_topl.ports["multiplier_0_gate_W"].center[0],bar.ports["e1"].center[0])) + pdk.get_grule("met2")["min_separation"])
 	get_right_extension = lambda bar, b_topr=b_topr, diffpair=diffpair, pdk=pdk : (abs(diffpair.xmax-max(b_topr.ports["multiplier_0_gate_E"].center[0],bar.ports["e3"].center[0])) + pdk.get_grule("met2")["min_separation"])
 	# lay bar plus and PLUSgate_routeW
 	bar_comp = rectangle(centered=True,size=(abs(b_topr.xmax-a_topl.xmin), b_topr.ports["multiplier_0_gate_E"].width),layer=pdk.get_glayer("met2"))
 	bar_plus = (diffpair << bar_comp).movey(diffpair.ymax + bar_comp.ymax + pdk.get_grule("met2")["min_separation"])
 	PLUSgate_routeW = diffpair << c_route(pdk, a_topl.ports["multiplier_0_gate_W"], bar_plus.ports["e1"], extension=get_left_extension(bar_plus))
-	#lay bar minus and MINUSgate_routeE
+	# lay bar minus and MINUSgate_routeE
 	plus_minus_seperation = max(pdk.get_grule("met2")["min_separation"], plus_minus_seperation)
 	bar_minus = (diffpair << bar_comp).movey(diffpair.ymax +bar_comp.ymax + plus_minus_seperation)
 	MINUSgate_routeE = diffpair << c_route(pdk, b_topr.ports["multiplier_0_gate_E"], bar_minus.ports["e3"], extension=get_right_extension(bar_minus))
 	# lay MINUSgate_routeW and PLUSgate_routeE
 	MINUSgate_routeW = diffpair << c_route(pdk, set_port_orientation(b_botl.ports["multiplier_0_gate_E"],"W"), bar_minus.ports["e1"], extension=get_left_extension(bar_minus))
 	PLUSgate_routeE = diffpair << c_route(pdk, set_port_orientation(a_botr.ports["multiplier_0_gate_W"],"E"), bar_plus.ports["e3"], extension=get_right_extension(bar_plus))
 	# correct pwell place, add ports, flatten, and return
@@ -158,8 +168,22 @@
 	component = component_snap_to_grid(rename_ports_by_orientation(diffpair))
 
 	component.info['netlist'] = diff_pair_netlist(fetL, fetR)
 	return component
 
 
 
-
+@cell
+def diff_pair_generic(
+	pdk: MappedPDK,
+	width: float = 3,
+	fingers: int = 4,
+	length: Optional[float] = None,
+	n_or_p_fet: bool = True,
+	plus_minus_seperation: float = 0,
+	rmult: int = 1,
+	dummy: Union[bool, tuple[bool, bool]] = True,
+	substrate_tap: bool=True
+) -> Component:
+	diffpair = common_centroid_ab_ba(pdk,width,fingers,length,n_or_p_fet,rmult,dummy,substrate_tap)
+	diffpair << smart_route(pdk,diffpair.ports["A_source_E"],diffpair.ports["B_source_E"],diffpair, diffpair)
+	return diffpair
```

### Comparing `glayout-0.0.3/glayout/components/diff_pair_cmirrorbias.py` & `glayout-0.0.4/glayout/flow/components/diff_pair_cmirrorbias.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 from gdsfactory.cell import cell, clear_cache
 from gdsfactory.component import Component, copy
 from gdsfactory.component_reference import ComponentReference
 from gdsfactory.components.rectangle import rectangle
-from glayout.pdk.mappedpdk import MappedPDK
+from glayout.flow.pdk.mappedpdk import MappedPDK
 from typing import Optional, Union
-from glayout.primitives.fet import nmos, pmos, multiplier
-from glayout.components.diff_pair import diff_pair
-from glayout.primitives.guardring import tapring
-from glayout.primitives.mimcap import mimcap_array, mimcap
-from glayout.routing.L_route import L_route
-from glayout.routing.c_route import c_route
-from glayout.primitives.via_gen import via_stack, via_array
+from glayout.flow.primitives.fet import nmos, pmos, multiplier
+from glayout.flow.components.diff_pair import diff_pair
+from glayout.flow.primitives.guardring import tapring
+from glayout.flow.primitives.mimcap import mimcap_array, mimcap
+from glayout.flow.routing.L_route import L_route
+from glayout.flow.routing.c_route import c_route
+from glayout.flow.primitives.via_gen import via_stack, via_array
 from gdsfactory.routing.route_quad import route_quad
-from glayout.pdk.util.comp_utils import (
+from glayout.flow.pdk.util.comp_utils import (
     evaluate_bbox,
     prec_ref_center,
     movex,
     movey,
     to_decimal,
     to_float,
     move,
     align_comp_to_port,
     get_padding_points_cc,
 )
-from glayout.pdk.util.port_utils import (
+from glayout.flow.pdk.util.port_utils import (
     rename_ports_by_orientation,
     rename_ports_by_list,
     add_ports_perimeter,
     print_ports,
     set_port_orientation,
     rename_component_ports,
 )
-from glayout.routing.straight_route import straight_route
-from glayout.pdk.util.snap_to_grid import component_snap_to_grid
+from glayout.flow.routing.straight_route import straight_route
+from glayout.flow.pdk.util.snap_to_grid import component_snap_to_grid
 from pydantic import validate_arguments
-from glayout.placement.two_transistor_interdigitized import two_nfet_interdigitized
-from glayout.spice import Netlist
-from glayout.components.stacked_current_mirror import current_mirror_netlist
+from glayout.flow.placement.two_transistor_interdigitized import two_nfet_interdigitized
+from glayout.flow.spice import Netlist
+from glayout.flow.components.stacked_current_mirror import current_mirror_netlist
 
 def diff_pair_ibias_netlist(center_diffpair: Component, current_mirror: Component, antenna_diode: Component) -> Netlist:
     netlist = Netlist(
         circuit_name="DIFFPAIR_CMIRROR_BIAS",
         nodes=['VP', 'VN', 'VDD1', 'VDD2', 'IBIAS', 'VSS', 'B']
     )
```

### Comparing `glayout-0.0.3/glayout/components/diff_pair_stackedcmirror.py` & `glayout-0.0.4/glayout/flow/components/diff_pair_stackedcmirror.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 from gdsfactory.cell import cell, clear_cache
 from gdsfactory.component import Component, copy
 from gdsfactory.component_reference import ComponentReference
 from gdsfactory.components.rectangle import rectangle
-from glayout.pdk.mappedpdk import MappedPDK
+from glayout.flow.pdk.mappedpdk import MappedPDK
 from typing import Optional, Union
-from glayout.primitives.fet import nmos, pmos, multiplier
-from glayout.components.diff_pair import diff_pair
-from glayout.primitives.guardring import tapring
-from glayout.primitives.mimcap import mimcap_array, mimcap
-from glayout.routing.L_route import L_route
-from glayout.routing.c_route import c_route
-from glayout.primitives.via_gen import via_stack, via_array
+from glayout.flow.primitives.fet import nmos, pmos, multiplier
+from glayout.flow.components.diff_pair import diff_pair
+from glayout.flow.primitives.guardring import tapring
+from glayout.flow.primitives.mimcap import mimcap_array, mimcap
+from glayout.flow.routing.L_route import L_route
+from glayout.flow.routing.c_route import c_route
+from glayout.flow.primitives.via_gen import via_stack, via_array
 from gdsfactory.routing.route_quad import route_quad
-from glayout.pdk.util.comp_utils import evaluate_bbox, prec_ref_center, movex, movey, to_decimal, to_float, move, align_comp_to_port, get_padding_points_cc
-from glayout.pdk.util.port_utils import rename_ports_by_orientation, rename_ports_by_list, add_ports_perimeter, print_ports, set_port_orientation, rename_component_ports
-from glayout.routing.straight_route import straight_route
-from glayout.pdk.util.snap_to_grid import component_snap_to_grid
+from glayout.flow.pdk.util.comp_utils import evaluate_bbox, prec_ref_center, movex, movey, to_decimal, to_float, move, align_comp_to_port, get_padding_points_cc
+from glayout.flow.pdk.util.port_utils import rename_ports_by_orientation, rename_ports_by_list, add_ports_perimeter, print_ports, set_port_orientation, rename_component_ports
+from glayout.flow.routing.straight_route import straight_route
+from glayout.flow.pdk.util.snap_to_grid import component_snap_to_grid
 from pydantic import validate_arguments
-from glayout.placement.two_transistor_interdigitized import two_nfet_interdigitized
+from glayout.flow.placement.two_transistor_interdigitized import two_nfet_interdigitized
 
-from glayout.components.diff_pair_cmirrorbias import diff_pair_ibias
-from glayout.components.stacked_current_mirror import stacked_nfet_current_mirror
-from glayout.components.differential_to_single_ended_converter import differential_to_single_ended_converter
-from glayout.components.row_csamplifier_diff_to_single_ended_converter import row_csamplifier_diff_to_single_ended_converter
+from glayout.flow.components.diff_pair_cmirrorbias import diff_pair_ibias
+from glayout.flow.components.stacked_current_mirror import stacked_nfet_current_mirror
+from glayout.flow.components.differential_to_single_ended_converter import differential_to_single_ended_converter
+from glayout.flow.components.row_csamplifier_diff_to_single_ended_converter import row_csamplifier_diff_to_single_ended_converter
 
 
 @validate_arguments
 def __add_diff_pair_and_bias(pdk: MappedPDK, toplevel_stacked: Component, half_diffpair_params: tuple[float, float, int], diffpair_bias: tuple[float, float, int], rmult: int, with_antenna_diode_on_diffinputs: int) -> Component:
     clear_cache()
     diffpair_i_ref = diff_pair_ibias(pdk, half_diffpair_params, diffpair_bias, rmult, with_antenna_diode_on_diffinputs)
     toplevel_stacked.add(diffpair_i_ref)
```

### Comparing `glayout-0.0.3/glayout/components/differential_to_single_ended_converter.py` & `glayout-0.0.4/glayout/flow/components/differential_to_single_ended_converter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from gdsfactory.cell import cell, clear_cache
 from gdsfactory.component import Component, copy
 from gdsfactory.component_reference import ComponentReference
 from gdsfactory.components.rectangle import rectangle
-from glayout.pdk.mappedpdk import MappedPDK
+from glayout.flow.pdk.mappedpdk import MappedPDK
 from typing import Optional, Union
-from glayout.primitives.fet import nmos, pmos, multiplier
-from glayout.components.diff_pair import diff_pair
-from glayout.primitives.guardring import tapring
-from glayout.primitives.mimcap import mimcap_array, mimcap
-from glayout.routing.L_route import L_route
-from glayout.routing.c_route import c_route
-from glayout.primitives.via_gen import via_stack, via_array
+from glayout.flow.primitives.fet import nmos, pmos, multiplier
+from glayout.flow.components.diff_pair import diff_pair
+from glayout.flow.primitives.guardring import tapring
+from glayout.flow.primitives.mimcap import mimcap_array, mimcap
+from glayout.flow.routing.L_route import L_route
+from glayout.flow.routing.c_route import c_route
+from glayout.flow.primitives.via_gen import via_stack, via_array
 from gdsfactory.routing.route_quad import route_quad
-from glayout.pdk.util.comp_utils import evaluate_bbox, prec_ref_center, movex, movey, to_decimal, to_float, move, align_comp_to_port, get_padding_points_cc
-from glayout.pdk.util.port_utils import rename_ports_by_orientation, rename_ports_by_list, add_ports_perimeter, print_ports, set_port_orientation, rename_component_ports
-from glayout.routing.straight_route import straight_route
-from glayout.pdk.util.snap_to_grid import component_snap_to_grid
+from glayout.flow.pdk.util.comp_utils import evaluate_bbox, prec_ref_center, movex, movey, to_decimal, to_float, move, align_comp_to_port, get_padding_points_cc
+from glayout.flow.pdk.util.port_utils import rename_ports_by_orientation, rename_ports_by_list, add_ports_perimeter, print_ports, set_port_orientation, rename_component_ports
+from glayout.flow.routing.straight_route import straight_route
+from glayout.flow.pdk.util.snap_to_grid import component_snap_to_grid
 from pydantic import validate_arguments
-from glayout.placement.two_transistor_interdigitized import two_nfet_interdigitized
-from glayout.spice import Netlist
+from glayout.flow.placement.two_transistor_interdigitized import two_nfet_interdigitized
+from glayout.flow.spice import Netlist
 
 
 
 @validate_arguments
 def __create_sharedgatecomps(pdk: MappedPDK, rmult: int, half_pload: tuple[float,float,int]) -> tuple:
     # add diffpair current mirror loads (this is a pmos current mirror split into 2 for better matching/compensation)
     shared_gate_comps = Component("shared gate components")
```

### Comparing `glayout-0.0.3/glayout/components/opamp.py` & `glayout-0.0.4/glayout/flow/components/opamp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from gdsfactory.cell import cell, clear_cache
 from gdsfactory.component import Component, copy
 from gdsfactory.component_reference import ComponentReference
 from gdsfactory.components.rectangle import rectangle
-from glayout.pdk.mappedpdk import MappedPDK
+from glayout.flow.pdk.mappedpdk import MappedPDK
 from typing import Optional, Union
-from glayout.primitives.fet import nmos, pmos, multiplier
-from glayout.components.diff_pair import diff_pair
-from glayout.primitives.guardring import tapring
-from glayout.primitives.mimcap import mimcap_array, mimcap
-from glayout.routing.L_route import L_route
-from glayout.routing.c_route import c_route
-from glayout.primitives.via_gen import via_stack, via_array
+from glayout.flow.primitives.fet import nmos, pmos, multiplier
+from glayout.flow.components.diff_pair import diff_pair
+from glayout.flow.primitives.guardring import tapring
+from glayout.flow.primitives.mimcap import mimcap_array, mimcap
+from glayout.flow.routing.L_route import L_route
+from glayout.flow.routing.c_route import c_route
+from glayout.flow.primitives.via_gen import via_stack, via_array
 from gdsfactory.routing.route_quad import route_quad
-from glayout.pdk.util.comp_utils import evaluate_bbox, prec_ref_center, movex, movey, to_decimal, to_float, move, align_comp_to_port, get_padding_points_cc
-from glayout.pdk.util.port_utils import rename_ports_by_orientation, rename_ports_by_list, add_ports_perimeter, print_ports, set_port_orientation, rename_component_ports
-from glayout.routing.straight_route import straight_route
-from glayout.pdk.util.snap_to_grid import component_snap_to_grid
+from glayout.flow.pdk.util.comp_utils import evaluate_bbox, prec_ref_center, movex, movey, to_decimal, to_float, move, align_comp_to_port, get_padding_points_cc
+from glayout.flow.pdk.util.port_utils import rename_ports_by_orientation, rename_ports_by_list, add_ports_perimeter, print_ports, set_port_orientation, rename_component_ports
+from glayout.flow.routing.straight_route import straight_route
+from glayout.flow.pdk.util.snap_to_grid import component_snap_to_grid
 from pydantic import validate_arguments
-from glayout.placement.two_transistor_interdigitized import two_nfet_interdigitized
-from glayout.spice import Netlist
+from glayout.flow.placement.two_transistor_interdigitized import two_nfet_interdigitized
+from glayout.flow.spice import Netlist
 
-from glayout.components.opamp_twostage import opamp_twostage
-from glayout.components.stacked_current_mirror import current_mirror_netlist
+from glayout.flow.components.opamp_twostage import opamp_twostage
+from glayout.flow.components.stacked_current_mirror import current_mirror_netlist
 
 def opamp_output_stage_netlist(pdk: MappedPDK, output_amp_fet_ref: ComponentReference, biasParams: list) -> Netlist:
     bias_netlist = current_mirror_netlist(pdk, biasParams[0], biasParams[1], biasParams[2])
 
     output_stage_netlist = Netlist(
         circuit_name="OUTPUT_STAGE",
         nodes=['VDD', 'GND', 'IBIAS', 'VIN', 'VOUT']
```

### Comparing `glayout-0.0.3/glayout/components/opamp_twostage.py` & `glayout-0.0.4/glayout/flow/components/opamp_twostage.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 from gdsfactory.cell import cell, clear_cache
 from gdsfactory.component import Component, copy
 from gdsfactory.component_reference import ComponentReference
 from gdsfactory.components.rectangle import rectangle
-from glayout.pdk.mappedpdk import MappedPDK
+from glayout.flow.pdk.mappedpdk import MappedPDK
 from typing import Optional, Union
-from glayout.primitives.fet import nmos, pmos, multiplier
-from glayout.components.diff_pair import diff_pair
-from glayout.primitives.guardring import tapring
-from glayout.primitives.mimcap import mimcap_array, mimcap
-from glayout.routing.L_route import L_route
-from glayout.routing.c_route import c_route
-from glayout.primitives.via_gen import via_stack, via_array
+from glayout.flow.primitives.fet import nmos, pmos, multiplier
+from glayout.flow.components.diff_pair import diff_pair
+from glayout.flow.primitives.guardring import tapring
+from glayout.flow.primitives.mimcap import mimcap_array, mimcap
+from glayout.flow.routing.L_route import L_route
+from glayout.flow.routing.c_route import c_route
+from glayout.flow.primitives.via_gen import via_stack, via_array
 from gdsfactory.routing.route_quad import route_quad
-from glayout.pdk.util.comp_utils import evaluate_bbox, prec_ref_center, movex, movey, to_decimal, to_float, move, align_comp_to_port, get_padding_points_cc
-from glayout.pdk.util.port_utils import rename_ports_by_orientation, rename_ports_by_list, add_ports_perimeter, print_ports, set_port_orientation, rename_component_ports
-from glayout.routing.straight_route import straight_route
-from glayout.pdk.util.snap_to_grid import component_snap_to_grid
+from glayout.flow.pdk.util.comp_utils import evaluate_bbox, prec_ref_center, movex, movey, to_decimal, to_float, move, align_comp_to_port, get_padding_points_cc
+from glayout.flow.pdk.util.port_utils import rename_ports_by_orientation, rename_ports_by_list, add_ports_perimeter, print_ports, set_port_orientation, rename_component_ports
+from glayout.flow.routing.straight_route import straight_route
+from glayout.flow.pdk.util.snap_to_grid import component_snap_to_grid
 from pydantic import validate_arguments
-from glayout.placement.two_transistor_interdigitized import two_nfet_interdigitized
+from glayout.flow.placement.two_transistor_interdigitized import two_nfet_interdigitized
 
-from glayout.components.diff_pair_cmirrorbias import diff_pair_ibias
-from glayout.components.stacked_current_mirror import stacked_nfet_current_mirror
-from glayout.components.differential_to_single_ended_converter import differential_to_single_ended_converter
-from glayout.components.row_csamplifier_diff_to_single_ended_converter import row_csamplifier_diff_to_single_ended_converter
-from glayout.components.diff_pair_stackedcmirror import diff_pair_stackedcmirror
-from glayout.spice import Netlist
-from glayout.components.stacked_current_mirror import current_mirror_netlist
+from glayout.flow.components.diff_pair_cmirrorbias import diff_pair_ibias
+from glayout.flow.components.stacked_current_mirror import stacked_nfet_current_mirror
+from glayout.flow.components.differential_to_single_ended_converter import differential_to_single_ended_converter
+from glayout.flow.components.row_csamplifier_diff_to_single_ended_converter import row_csamplifier_diff_to_single_ended_converter
+from glayout.flow.components.diff_pair_stackedcmirror import diff_pair_stackedcmirror
+from glayout.flow.spice import Netlist
+from glayout.flow.components.stacked_current_mirror import current_mirror_netlist
 
 @validate_arguments
 def __create_and_route_pins(
     pdk: MappedPDK,
     opamp_top: Component,
     pmos_comps_ref: ComponentReference,
     halfmultn_drain_routeref: ComponentReference,
```

### Comparing `glayout-0.0.3/glayout/components/row_csamplifier_diff_to_single_ended_converter.py` & `glayout-0.0.4/glayout/flow/components/row_csamplifier_diff_to_single_ended_converter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from gdsfactory.cell import cell, clear_cache
 from gdsfactory.component import Component, copy
 from gdsfactory.component_reference import ComponentReference
 from gdsfactory.components.rectangle import rectangle
-from glayout.pdk.mappedpdk import MappedPDK
+from glayout.flow.pdk.mappedpdk import MappedPDK
 from typing import Optional, Union
-from glayout.primitives.fet import nmos, pmos, multiplier
-from glayout.components.diff_pair import diff_pair
-from glayout.primitives.guardring import tapring
-from glayout.primitives.mimcap import mimcap_array, mimcap
-from glayout.routing.L_route import L_route
-from glayout.routing.c_route import c_route
-from glayout.primitives.via_gen import via_stack, via_array
+from glayout.flow.primitives.fet import nmos, pmos, multiplier
+from glayout.flow.components.diff_pair import diff_pair
+from glayout.flow.primitives.guardring import tapring
+from glayout.flow.primitives.mimcap import mimcap_array, mimcap
+from glayout.flow.routing.L_route import L_route
+from glayout.flow.routing.c_route import c_route
+from glayout.flow.primitives.via_gen import via_stack, via_array
 from gdsfactory.routing.route_quad import route_quad
-from glayout.pdk.util.comp_utils import evaluate_bbox, prec_ref_center, movex, movey, to_decimal, to_float, move, align_comp_to_port, get_padding_points_cc
-from glayout.pdk.util.port_utils import rename_ports_by_orientation, rename_ports_by_list, add_ports_perimeter, print_ports, set_port_orientation, rename_component_ports
-from glayout.routing.straight_route import straight_route
-from glayout.pdk.util.snap_to_grid import component_snap_to_grid
+from glayout.flow.pdk.util.comp_utils import evaluate_bbox, prec_ref_center, movex, movey, to_decimal, to_float, move, align_comp_to_port, get_padding_points_cc
+from glayout.flow.pdk.util.port_utils import rename_ports_by_orientation, rename_ports_by_list, add_ports_perimeter, print_ports, set_port_orientation, rename_component_ports
+from glayout.flow.routing.straight_route import straight_route
+from glayout.flow.pdk.util.snap_to_grid import component_snap_to_grid
 from pydantic import validate_arguments
-from glayout.placement.two_transistor_interdigitized import two_nfet_interdigitized
-from glayout.spice import Netlist
+from glayout.flow.placement.two_transistor_interdigitized import two_nfet_interdigitized
+from glayout.flow.spice import Netlist
 
 def row_csamplifier_diff_to_single_ended_converter_netlist(diff_to_single: Component) -> Netlist:
     overall_netlist = Netlist(
         circuit_name="DIFF_TO_SINGLE_CS",
         nodes=['VIN1', 'VIN2', 'VOUT', 'VSS', 'VSS2']
     )
```

### Comparing `glayout-0.0.3/glayout/components/stacked_current_mirror.py` & `glayout-0.0.4/glayout/flow/components/stacked_current_mirror.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from gdsfactory.cell import cell, clear_cache
 from gdsfactory.component import Component, copy
 from gdsfactory.component_reference import ComponentReference
 from gdsfactory.components.rectangle import rectangle
-from glayout.pdk.mappedpdk import MappedPDK
+from glayout.flow.pdk.mappedpdk import MappedPDK
 from typing import Optional, Union
-from glayout.primitives.fet import nmos, pmos, multiplier
-from glayout.components.diff_pair import diff_pair
-from glayout.primitives.guardring import tapring
-from glayout.primitives.mimcap import mimcap_array, mimcap
-from glayout.routing.L_route import L_route
-from glayout.routing.c_route import c_route
-from glayout.primitives.via_gen import via_stack, via_array
+from glayout.flow.primitives.fet import nmos, pmos, multiplier
+from glayout.flow.components.diff_pair import diff_pair
+from glayout.flow.primitives.guardring import tapring
+from glayout.flow.primitives.mimcap import mimcap_array, mimcap
+from glayout.flow.routing.L_route import L_route
+from glayout.flow.routing.c_route import c_route
+from glayout.flow.primitives.via_gen import via_stack, via_array
 from gdsfactory.routing.route_quad import route_quad
-from glayout.pdk.util.comp_utils import evaluate_bbox, prec_ref_center, movex, movey, to_decimal, to_float, move, align_comp_to_port, get_padding_points_cc
-from glayout.pdk.util.port_utils import rename_ports_by_orientation, rename_ports_by_list, add_ports_perimeter, print_ports, set_port_orientation, rename_component_ports
-from glayout.routing.straight_route import straight_route
-from glayout.pdk.util.snap_to_grid import component_snap_to_grid
+from glayout.flow.pdk.util.comp_utils import evaluate_bbox, prec_ref_center, movex, movey, to_decimal, to_float, move, align_comp_to_port, get_padding_points_cc
+from glayout.flow.pdk.util.port_utils import rename_ports_by_orientation, rename_ports_by_list, add_ports_perimeter, print_ports, set_port_orientation, rename_component_ports
+from glayout.flow.routing.straight_route import straight_route
+from glayout.flow.pdk.util.snap_to_grid import component_snap_to_grid
 from pydantic import validate_arguments
-from glayout.placement.two_transistor_interdigitized import two_nfet_interdigitized
-from glayout.spice import Netlist
+from glayout.flow.placement.two_transistor_interdigitized import two_nfet_interdigitized
+from glayout.flow.spice import Netlist
 
 def current_mirror_netlist(pdk: MappedPDK, width: float, length: float, multipliers: int) -> Netlist:
     return Netlist(
         circuit_name='CURRENT_MIRROR',
         nodes=['VREF', 'VCOPY', 'VSS'],
         source_netlist=""".subckt {circuit_name} {nodes} l=1 w=1 m=1
 XREF VREF VREF VSS VSS {model} l={{l}} w={{w}} m={{m}}
```

### Comparing `glayout-0.0.3/glayout/pdk/gf180_mapped/gf180_mapped.py` & `glayout-0.0.4/glayout/flow/pdk/gf180_mapped/gf180_mapped.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,37 @@
 """
 usage: from gf180_mapped import gf180_mapped_pdk
 """
 
-from gf180.layers import LAYER  # , LAYER_VIEWS
 from ..gf180_mapped.grules import grulesobj
-from ..mappedpdk import MappedPDK
+from ..mappedpdk import MappedPDK, SetupPDKFiles
 from pathlib import Path
 
-LAYER = LAYER.dict()
+
 #LAYER["fusetop"]=(75, 0)
-LAYER["CAP_MK"] = (117,5)
+LAYER = {
+    "metal5": (81, 0),
+    "via4": (41, 0),
+    "metal4": (46, 0),
+    "via3": (40, 0),
+    "metal3": (42, 0),
+    "via2": (38, 0),
+    "metal2": (36, 0),
+    "via1": (35, 0),
+    "metal1": (34, 0),
+    "contact": (33, 0),
+    "poly2": (30, 0),
+    "comp": (22, 0),
+    "nplus": (32, 0),
+    "pplus": (31, 0),
+    "nwell": (21, 0),
+    "lvpwell": (204, 0),
+    "dnwell": (12, 0),
+    "CAP_MK": (117, 5)
+}
 
 gf180_glayer_mapping = {
     "met5": "metal5",
     "via4": "via4",
     "met4": "metal4",
     "via3": "via3",
     "met3": "metal3",
@@ -33,24 +51,41 @@
     "capmet": "CAP_MK"
 }
 
 # note for DRC, there is mim_option 'A'. This is the one configured for use
 
 gf180_lydrc_file_path = Path(__file__).resolve().parent / "gf180mcu_drc.lydrc"
 
+openfasoc_dir = Path(__file__).resolve().parent.parent.parent.parent.parent.parent.parent
+pdk_root = Path('/usr/bin/miniconda3/share/pdk/')
+lvs_schematic_ref_file = openfasoc_dir / "common" / "platforms" / "gf180osu9t" / "cdl" / "gf180mcu_osu_sc_9T.spice"
+magic_drc_file = pdk_root / "gf180mcuC" / "libs.tech" / "magic" / "gf180mcuC.magicrc"
+lvs_setup_tcl_file = pdk_root / "gf180mcuC" / "libs.tech" / "netgen" / "gf180mcuC_setup.tcl"
+temp_dir = None
+
+
+pdk_files = SetupPDKFiles(
+    pdk_root=pdk_root,
+    klayout_drc_file=gf180_lydrc_file_path,
+    lvs_schematic_ref_file=lvs_schematic_ref_file,
+    lvs_setup_tcl_file=lvs_setup_tcl_file,
+    magic_drc_file=magic_drc_file,
+    temp_dir=temp_dir,
+    pdk='gf180'
+).return_dict_of_files()
 
 gf180_mapped_pdk = MappedPDK(
     name="gf180",
     glayers=gf180_glayer_mapping,
 	models={
         'nfet': 'nfet_03v3',
 		'pfet': 'pfet_03v3',
 		'mimcap': 'mimcap_1p0fF'
     },
     layers=LAYER,
-    #klayout_lydrc_file=gf180_lydrc_file_path,
+    pdk_files=pdk_files,
     grules=grulesobj,
 )
 
 # configure the grid size and other settings
 gf180_mapped_pdk.gds_write_settings.precision = 5*10**-9
 gf180_mapped_pdk.cell_decorator_settings.cache=False
```

### Comparing `glayout-0.0.3/glayout/pdk/gf180_mapped/grules.py` & `glayout-0.0.4/glayout/flow/pdk/gf180_mapped/grules.py`

 * *Files identical despite different names*

### Comparing `glayout-0.0.3/glayout/pdk/sky130_mapped/grules.py` & `glayout-0.0.4/glayout/flow/pdk/sky130_mapped/grules.py`

 * *Files identical despite different names*

### Comparing `glayout-0.0.3/glayout/pdk/sky130_mapped/sky130_add_npc.py` & `glayout-0.0.4/glayout/flow/pdk/sky130_mapped/sky130_add_npc.py`

 * *Files identical despite different names*

### Comparing `glayout-0.0.3/glayout/pdk/util/comp_utils.py` & `glayout-0.0.4/glayout/flow/pdk/util/comp_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,31 +3,57 @@
 from gdsfactory.typings import Component, ComponentReference
 from gdsfactory.components.rectangle import rectangle
 from gdsfactory.port import Port
 from typing import Callable, Union, Optional, Iterable
 from decimal import Decimal
 from gdsfactory.functions import transformed
 from gdsfactory.functions import move as __gf_move
-from glayout.pdk.mappedpdk import MappedPDK
+from glayout.flow.pdk.mappedpdk import MappedPDK
 from gdstk import rectangle as primitive_rectangle
-from .port_utils import add_ports_perimeter, rename_ports_by_list
+from .port_utils import add_ports_perimeter, rename_ports_by_list, parse_direction
 
 
 @validate_arguments
 def evaluate_bbox(custom_comp: Union[Component, ComponentReference], return_decimal: Optional[bool]=False, padding: float=0) -> tuple[Union[float,Decimal],Union[float,Decimal]]:
 	"""returns the length and height of a component like object"""
 	compbbox = custom_comp.bbox
 	width = abs(Decimal(str(compbbox[1][0])) - Decimal(str(compbbox[0][0]))) + 2*Decimal(str(padding))
 	height = abs(Decimal(str(compbbox[1][1])) - Decimal(str(compbbox[0][1]))) + 2*Decimal(str(padding))
 	if return_decimal:
 		return (width,height)
 	return (float(width),float(height))
 
 
 @validate_arguments
+def center_to_edge_distance(custom_comp: Union[Component, ComponentReference], direction: Union[str,int]) -> float:
+	"""specifies the distance between the center of custom_comp and a specified edge given by the direction argument
+	the component is considerd a rectangle (using the bounding box), such there are 4 edges
+	Args:
+		custom_comp (Component | ComponentReference): Component we want the center of
+		direction (str | int): the edge we are interested in
+	Returns:
+		float: absolute distance between custom_comp center and N,S,E, or W edge
+	"""
+	compbbox = custom_comp.bbox
+	#center = prec_center(custom_comp)
+	center = custom_comp.center
+	direction = parse_direction(direction)
+	if direction==1:# West edge
+		distance = center[0] - compbbox[0][0]
+	elif direction==2:# North edge
+		distance = center[1] - compbbox[1][1]
+	elif direction==3:# East edge
+		distance = center[0] - compbbox[1][0]
+	elif direction==4:# South edge
+		distance = center[1] - compbbox[0][1]
+	else:
+		raise ValueError("unknown error with direction in function center_to_edge_distance (comp_utils)")
+	return snap_to_grid(abs(distance),2)
+
+@validate_arguments
 def move(custom_comp: Union[Port, ComponentReference, Component], offsetxy: tuple[float,float] = (0,0), destination: Optional[tuple[Optional[float],Optional[float]]]=None, layer: Optional[tuple[int,int]]=None) -> Union[Port, ComponentReference, Component]:
 	"""moves custom_comp
 	moves by offset[0]=x offset, offset[1]=y offset
 	destination (x,y) if not none overrides offset option
 	layer if specfied will move based on a layer (only relevant for destination option)
 	returns the modified custom_comp
 	"""
@@ -130,39 +156,39 @@
 			yalign = "b"
 		elif round(align_to.orientation) == 90:#facing north
 			xalign = "c"
 			yalign = "t"
 		else:
 			raise ValueError("port must be vertical or horizontal")
 	else:
-		xalign = (alignment[0] or "none").lower()
-		yalign = (alignment[1] or "none").lower()
+		xalign = (alignment[0] or "none").lower().strip()
+		yalign = (alignment[1] or "none").lower().strip()
 	# compute translation x amount for x alignment
 	x_movcenter = align_to.center[0] - ccenter[0]
 	x_mov_lr = abs(xdim/2 if is_EW else (width-xdim)/2)
 	if "none" in xalign:
 		xmov = 0
-	elif "l" in xalign:
+	elif "l" in xalign[0]:
 		xmov = x_movcenter - x_mov_lr
-	elif "r" in xalign:
-		xmov = x_movcenter + x_mov_lr
-	elif "c" in xalign:
+	elif "c" in xalign[0]:
 		xmov = x_movcenter
+	elif "r" in xalign[0]:
+		xmov = x_movcenter + x_mov_lr
 	else:
 		raise ValueError("please specify valid x alignment of l/r/c/None")
 	# compute translation y amount for y alignment
 	y_movcenter = align_to.center[1] - ccenter[1]
 	y_move_updown = abs((width-ydim)/2 if is_EW else ydim/2)
 	if "none" in yalign:
 		ymov = 0
-	elif "t" in yalign:
-		ymov = y_movcenter + y_move_updown
-	elif "b" in yalign:
+	elif "b" in yalign[0]:
 		ymov = y_movcenter - y_move_updown
-	elif "c" in yalign:
+	elif "t" in yalign[0]:
+		ymov = y_movcenter + y_move_updown
+	elif "c" in yalign[0]:
 		ymov = y_movcenter
 	else:
 		raise ValueError("please specify valid y alignment of t/b/c/None")
 	# make reference type, execute move
 	if isinstance(custom_comp, Component):
 		comp_ref = custom_comp.ref()
 	else:
@@ -242,27 +268,30 @@
 	currentmax = to_decimal((custom_comp.xmax,custom_comp.ymax))
 	correctionxy = [correctmax[i] - currentmax[i] for i in range(2)]
 	if return_decimal:
 		return correctionxy
 	return to_float(correctionxy)
 
 @validate_arguments
-def prec_ref_center(custom_comp: Union[Component,ComponentReference], destination: Optional[tuple[float,float]]=None) -> ComponentReference:
+def prec_ref_center(custom_comp: Union[Component,ComponentReference], destination: Optional[tuple[float,float]]=None, snapmov2grid: bool=False) -> ComponentReference:
 	"""instead of using component.ref_center() to get a ref to center at origin,
 	use this function which will return a centered ref
 	you can then run component.add(prec_ref_center(custom_comp)) to add the reference to your component
 	you can optionally specify a destination = tuple(x,y), by default, the destination is 0,0
 	returns component reference
 	"""
 	compref = custom_comp if isinstance(custom_comp, ComponentReference) else custom_comp.ref()
 	xcor, ycor = prec_center(compref, False)
 	if destination is not None:
 		xcor += destination[0]
 		ycor += destination[1]
-	return compref.movex(xcor).movey(ycor)
+	if snapmov2grid:
+		compref.movex(snap_to_grid(xcor,2)).movey(snap_to_grid(ycor,2))
+	else:
+		return compref.movex(xcor).movey(ycor)
 
 
 
 def get_padding_points_cc(
 	custom_comp: Union[ComponentReference, Component, list],
 	default: float = 50.0,
 	top: Optional[float]=None,
```

### Comparing `glayout-0.0.3/glayout/pdk/util/component_array_create.py` & `glayout-0.0.4/glayout/flow/pdk/util/component_array_create.py`

 * *Files identical despite different names*

### Comparing `glayout-0.0.3/glayout/pdk/util/port_utils.py` & `glayout-0.0.4/glayout/flow/pdk/util/port_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,34 +3,126 @@
 from gdsfactory.components.rectangle import rectangle
 from gdsfactory.port import Port
 from typing import Callable, Union, Optional
 from decimal import Decimal
 from pathlib import Path
 import pickle
 from PrettyPrint import PrettyPrintTree
+import math
 
 
 @validate_arguments
-def rename_component_ports(custom_comp: Component, rename_function: Callable[[str, Port], str]) -> Component:
+def parse_direction(direction: Union[int, str]) -> int:
+	"""returns 1,2,3,4 (W,N,E,S)
+
+	Args:
+		direction (int | str): a direction description either string or int
+		****direction descrption could be north/south/east/west or left/right/up/down, etc.
+
+	Returns:
+		int: 1=W, 2=N, 3=E, 4=S
+	"""
+	if isinstance(direction, int):
+		if direction<1 or direction>4:
+			raise ValueError(f"direction was specified as int {direction}, but int directions are 1,2,3, or 4")
+		else:
+			return direction
+	else:# direction is a string
+		cmp = direction.strip().lower()[0]
+		if cmp=="l" or cmp=="w" or cmp=="1":
+			return 1
+		elif cmp=="u" or cmp=="n" or cmp=="2":
+			return 2
+		elif cmp=="r" or cmp=="e" or cmp=="3":
+			return 3
+		elif cmp=="d" or cmp=="s" or cmp=="4":
+			return 4
+		else:
+			raise ValueError(f"failed to parse direction string {direction}")
+
+
+def proc_angle(angle: float) -> int:
+	"""round an angle in degrees to nearest int and converts to an angle [-180,180]
+
+	Args:
+		angle (float): angle in degrees
+
+	Returns:
+		float: angle in degrees [-180,180]
+	"""
+	angle = round(angle)
+	angle = angle % 360
+	if angle > 180:
+	    angle -= 360
+	return angle
+
+
+@validate_arguments
+def ports_parallel(edge1: Port, edge2: Port) -> bool:
+	"""returns True if the provided ports are parralel (same or 180degree opposite directions)
+	Requires ports are manhattan
+	Args:
+		edge1 (Port)
+		edge2 (Port)
+	Returns:
+		bool: True if the provided ports are parralel
+	"""
+	assert_port_manhattan([edge1,edge2])
+	e1orientation = abs(proc_angle(edge1.orientation))
+	e2orientation = abs(proc_angle(edge2.orientation))
+	if e1orientation==e2orientation:
+		return True
+	if (e1orientation==180 and e2orientation==0) or (e1orientation==0 and e2orientation==180):
+		return True
+	return False
+
+
+@validate_arguments
+def ports_inline(edge1: Port, edge2: Port, abstolerance: float=0.1) -> bool:
+	"""Check if two ports are inline within a tolerance.
+
+	Args:
+		edge1 (Port): The first port.
+		edge2 (Port): The second port.
+		abstolerance (float, optional): The absolute tolerance for inline check.. Defaults to 0.1.
+
+	Returns:
+		bool: True if the ports are inline within the given tolerance.
+	"""
+	# trivial cases and error checking
+	assert_port_manhattan([edge1, edge2])
+	if not(ports_parallel(edge1, edge2)):
+		return False
+	# given ports are parallel, determine coordinates of value
+	e1orientation = abs(proc_angle(edge1.orientation))
+	if e1orientation == 90:
+		centers = sorted([edge1.center[0], edge2.center[0]])
+	else:
+		centers = sorted([edge1.center[1], edge2.center[1]])
+	# determine if ports are inline within tolerance bounds
+	return not(centers[0] < (centers[1] - abstolerance))
+
+
+
+@validate_arguments
+def rename_component_ports(custom_comp: Union[Component, ComponentReference], rename_function: Callable[[str, Port], str]) -> Union[Component, ComponentReference]:
     """uses rename_function(str, Port) -> str to decide which ports to rename.
     rename_function accepts the current port name (string) and current port (Port) then returns the new port name
     rename_function can return new name = current port name, in which case the name will not change
     rename_function should raise error if custom requirments for rename are not met
     if you want to pass additional args to rename_function, implement a functor
     custom_comp is the components to modify. the modified component is returned
     """
     names_to_modify = list()
     # find ports and get new names
     for pname, pobj in custom_comp.ports.items():
         # error checking
         if not pname == pobj.name:
             raise ValueError("component may have an invalid ports dict")
-        
         new_name = rename_function(pname, pobj)
-        
         names_to_modify.append((pname,new_name))
     # modify names
     for namepair in names_to_modify:
         if namepair[0] in custom_comp.ports.keys():
             portobj = custom_comp.ports.pop(namepair[0])
             portobj.name = namepair[1]
             custom_comp.ports[namepair[1]] = portobj
@@ -63,15 +155,15 @@
 	# construct new name
 	old_str_split = old_name.rsplit("_", 1)
 	old_str_split[1] = new_suffix
 	new_name = "_".join(old_str_split)
 	return new_name
 
 @validate_arguments
-def rename_ports_by_orientation(custom_comp: Component) -> Component:
+def rename_ports_by_orientation(custom_comp: Union[Component, ComponentReference]) -> Union[Component, ComponentReference]:
     """replaces the last part of the port name 
     (after the last underscore, unless name is e1/2/3/4) with a direction
     direction is one of N,E,S,W
     returns the modified component
     """
     return rename_component_ports(custom_comp, rename_ports_by_orientation__call)
 
@@ -240,16 +332,40 @@
     for key,val in custom_comp.ports.items():
         print(key)
         if not names_only:
             print(val)
             print()
 
 
+def create_private_ports(custom_comp: Union[Component, ComponentReference], port_paths: Optional[Union[str,list[str]]] = None) -> list[Port]:
+	"""returns a list with a copy ports for children of the port_paths specified
+	the ports have _private appended
+	Args:
+		custom_comp (Component): comp to consider PortTree for
+		port_paths (str, list[str], optional): path along the PortTree to consider. Defaults to None (all ports are copied)
+		****NOTE: if a list is provided, then it will consider all paths in the list
+	Returns:
+		list[Port]: copies of all ports along port_path, these ports end with _private
+	"""
+	# arg setup
+	bypass = port_paths is None
+	if bypass:
+		port_paths = []
+	else:
+		if isinstance(port_paths, str):
+			port_paths = [port_paths]
+	# find all matching ports
+	ports_to_add = list()
+	for port in custom_comp.get_ports_list():
+		if any([port.name.startswith(port_path) for port_path in port_paths]) or bypass:
+			ports_to_add.append(port.copy(name=port.name+"_private"))
+	return ports_to_add
+
 class PortTree:
-	"""PortTree helps a glayout programmer visualize the ports in a component
+	"""PortTree helps a glayout.flow.programmer visualize the ports in a component
 	\"_\" should represent a level of hiearchy (much like a directory). think of this like psuedo directories
 	Initialize a PortTree from a Component or ComponentReference
 	then use self.ls to list all ports/subdirectories in a directory
 	you can use self.print to prettyprint a port tree (uses pypi prettyprinttree package)
 
 	You should not need to access the internal dictionary for the tree, but if you do:
 	PortTree internally uses tuple[str, dict] = name:children as the node type
@@ -312,20 +428,38 @@
 		return node_dict.items()
 		
 	
 	def get_val(self, node: tuple[str, dict]) -> str:
 		"""returns value of a node, (node might be a PortTree)"""
 		return node[0] if isinstance(node, tuple) else self.name
 	
+	def get_node(self, port_path: Optional[str] = None) -> tuple[str, dict]:
+		"""get a node name and children from a port_path
+		Args:
+			port_path (str, optional): psuedo path to a node in this PortTree. Defaults to None (returns root of the tree)
+		Returns:
+			list[tuple[str, dict]]: name and children of the specified node
+		"""
+		if port_path is None:
+			return self.name, self.tree
+		else:
+			current_children = self.tree
+			current_name = self.name
+			for node in port_path.split("_"):
+				current_children = current_children[node]
+				current_name = node
+		return current_name, current_children
+
+	
 	def print(self, savetofile: bool=True, default_opts: bool=True, depth: Optional[int]=None, outfile_name: Optional[str]=None, **kwargs):
 		"""prints output to terminal directly using prettyprinttree pypi package
 		args:
 		depth = max depth to print. this is a kwarg but since it so common, it should be specfied from depth arg
 		savetofile = saves print output to a txt file rather than printing to terminal (easier to view, but without nice formatting)
-		default_opts = bool=True results in using glayout recommended default print arguments
+		default_opts = bool=True results in using glayout.flow.recommended default print arguments
 		kwargs -> kwargs are prettyprint options passed directly to prettyprint.
 		****NOTE: kwargs override all other options
 		"""
 		depth = int(depth) if (depth is not None and depth>0) else -1
 		extra_kwargs = {}
 		if default_opts:
 			extra_kwargs.update({"default_orientation": True})
@@ -337,28 +471,28 @@
 		if rtrstr:
 			outfile_name = "outputtree.txt" if outfile_name is None else outfile_name
 			with open(outfile_name,"w") as outputfile:
 				outputfile.write(rtrstr)
 
 
 def print_port_tree_all_cells() -> list:
-	"""print the PortTree for most of the glayout cells and save as a text file.
+	"""print the PortTree for most of the glayout.flow.cells and save as a text file.
 	returns a list of components
 	"""
-	from glayout.primitives.via_gen import via_stack, via_array
-	from glayout.opamp import opamp
-	from glayout.primitives.mimcap import mimcap
-	from glayout.primitives.mimcap import mimcap_array
-	from glayout.primitives.guardring import tapring
-	from glayout.primitives.fet import multiplier, nmos, pmos
-	from glayout.diff_pair import diff_pair
-	from glayout.routing.straight_route import straight_route
-	from glayout.routing.c_route import c_route
-	from glayout.routing.L_route import L_route
-	from glayout.pdk.sky130_mapped import sky130_mapped_pdk as pdk
+	from glayout.flow.primitives.via_gen import via_stack, via_array
+	from glayout.flow.opamp import opamp
+	from glayout.flow.primitives.mimcap import mimcap
+	from glayout.flow.primitives.mimcap import mimcap_array
+	from glayout.flow.primitives.guardring import tapring
+	from glayout.flow.primitives.fet import multiplier, nmos, pmos
+	from glayout.flow.diff_pair import diff_pair
+	from glayout.flow.routing.straight_route import straight_route
+	from glayout.flow.routing.c_route import c_route
+	from glayout.flow.routing.L_route import L_route
+	from glayout.flow.pdk.sky130_mapped import sky130_mapped_pdk as pdk
 	from gdsfactory.port import Port
 	print("saving via_stack, via_array, opamp, mimcap, mimcap_array, tapring, multiplier, nmos, pmos, diff_pair, straight_route, c_route, L_route Ports to txt files")
 	celllist = list()
 	celllist.append(["via_stack",via_stack(pdk, "active_diff","met5")])
 	celllist.append(["viaarray", via_array(pdk, "active_diff","met5", num_vias=(2,3))])
 	celllist.append(["mimcap",mimcap(pdk)])
 	celllist.append(["mimcap_array",mimcap_array(pdk, 2, 3)])
@@ -371,11 +505,11 @@
 	psuedo_portb = Port("top",0,(5,10),2.5,layer=pdk.get_glayer("met5"))
 	psuedo_porta = Port("right",90,(10,10),2,layer=pdk.get_glayer("met2"))
 	celllist.append(["straight_route",straight_route(pdk,psuedo_porta,psuedo_portb)])
 	celllist.append(["L_route",L_route(pdk, psuedo_porta, psuedo_portb)])
 	celllist.append(["c_route",c_route(pdk, psuedo_porta, psuedo_porta,extension=2)])
 	celllist.append(["opamp",opamp(pdk)])
 	for name, py_cell in celllist:
-		from glayout import __version__ as glayoutvinfo
-		glayoutv = str(glayoutvinfo)
-		PortTree(py_cell,name=name).print(depth=5,outfile_name=name+"_v"+glayoutv+"_tree.txt",default_orientation=True)
+		from glayout import __version__ as glayoutinfo
+		vglayout = str(glayoutinfo)
+		PortTree(py_cell,name=name).print(depth=5,outfile_name=name+"_v"+vglayout+"_tree.txt",default_orientation=True)
 	return celllist
```

### Comparing `glayout-0.0.3/glayout/pdk/util/print_rules.py` & `glayout-0.0.4/glayout/flow/pdk/util/print_rules.py`

 * *Files identical despite different names*

### Comparing `glayout-0.0.3/glayout/placement/two_transistor_interdigitized.py` & `glayout-0.0.4/glayout/flow/placement/two_transistor_interdigitized.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from glayout.pdk.mappedpdk import MappedPDK
+from glayout.flow.pdk.mappedpdk import MappedPDK
 from pydantic import validate_arguments
 from gdsfactory.component import Component
-from glayout.primitives.fet import nmos, pmos, multiplier
-from glayout.pdk.util.comp_utils import evaluate_bbox
+from glayout.flow.primitives.fet import nmos, pmos, multiplier
+from glayout.flow.pdk.util.comp_utils import evaluate_bbox
 from typing import Literal, Union
-from glayout.pdk.util.port_utils import rename_ports_by_orientation, rename_ports_by_list
-from glayout.pdk.util.comp_utils import prec_ref_center
-from glayout.routing.straight_route import straight_route
+from glayout.flow.pdk.util.port_utils import rename_ports_by_orientation, rename_ports_by_list, create_private_ports
+from glayout.flow.pdk.util.comp_utils import prec_ref_center
+from glayout.flow.routing.straight_route import straight_route
 from gdsfactory.functions import transformed
-from glayout.primitives.guardring import tapring
-from glayout.pdk.util.port_utils import add_ports_perimeter
+from glayout.flow.primitives.guardring import tapring
+from glayout.flow.pdk.util.port_utils import add_ports_perimeter
 from gdsfactory.cell import clear_cache
+from typing import Literal
 
-
-#from glayout.placement.two_transistor_interdigitized import two_nfet_interdigitized; from glayout.pdk.sky130_mapped import sky130_mapped_pdk as pdk; biasParams=[6,2,4]; rmult=2
+#from glayout.flow.placement.two_transistor_interdigitized import two_nfet_interdigitized; from glayout.flow.pdk.sky130_mapped import sky130_mapped_pdk as pdk; biasParams=[6,2,4]; rmult=2
 
 @validate_arguments
-def two_transistor_interdigitized(
+def macro_two_transistor_interdigitized(
     pdk: MappedPDK,
     numcols: int,
     deviceA_and_B: Literal["nfet", "pfet"],
     dummy: Union[bool, tuple[bool, bool]] = True,
     **kwargs
 ) -> Component:
     """place two transistors in a single row with interdigitized placement
@@ -28,15 +28,15 @@
     Place follows an ABABAB... pattern
     args:
     pdk = MappedPDK to use
     numcols = a single col is actually one col for both transistors (so AB). 2 cols = ABAB ... so on
     deviceA_and_B = the device to place for both transistors (either nfet or pfet)
     dummy = place dummy at the edges of the interdigitized place (true by default). you can specify tuple to place only on one side
     kwargs = key word arguments for device. 
-    ****NOTE: These are the same as glayout.primitives.fet.multiplier arguments EXCLUDING dummy, sd_route_extension, and pdk options
+    ****NOTE: These are the same as glayout.flow.primitives.fet.multiplier arguments EXCLUDING dummy, sd_route_extension, and pdk options
     """
     if isinstance(dummy, bool):
         dummy = (dummy, dummy)
     # override kwargs for needed options
     kwargs["sd_route_extension"] = 0
     kwargs["gate_route_extension"] = 0
     kwargs["sdlayer"] = "n+s/d" if deviceA_and_B == "nfet" else "p+s/d"
@@ -67,15 +67,22 @@
             refs.append(idplace << center_devB)
         else: # not i%2 == i is even (so device A)
             refs.append(idplace << center_devA)
         refs[-1].movex(i*(xdisp))
         devletter = "B" if i%2 else "A"
         prefix=devletter+"_"+str(int(i/2))+"_"
         idplace.add_ports(refs[-1].get_ports_list(), prefix=prefix)
-    #issue somehwere before line 89
+    # extend poly layer for equal parasitics
+    for i in range(2*numcols):
+        desired_end_layer = pdk.layer_to_glayer(refs[i].ports["row0_col0_rightsd_top_met_N"].layer)
+        idplace << straight_route(pdk, refs[i].ports["row0_col0_rightsd_top_met_N"],refs[-1].ports["drain_E"],glayer2=desired_end_layer)
+        idplace << straight_route(pdk, refs[i].ports["leftsd_top_met_N"],refs[-1].ports["drain_E"],glayer2=desired_end_layer)
+        if not i%2:
+            desired_gate_end_layer = "poly"
+            idplace << straight_route(pdk, refs[i].ports["row0_col0_gate_S"], refs[-1].ports["gate_E"],glayer2=desired_gate_end_layer)
     # merge s/d layer for all transistors
     idplace << straight_route(pdk, refs[0].ports["plusdoped_W"],refs[-1].ports["plusdoped_E"])
     # create s/d/gate connections extending over entire row
     A_src = idplace << rename_ports_by_orientation(rename_ports_by_list(straight_route(pdk, refs[0].ports["source_W"], refs[-1].ports["source_E"]), [("route_","_")]))
     B_src = idplace << rename_ports_by_orientation(rename_ports_by_list(straight_route(pdk, refs[-1].ports["source_E"], refs[0].ports["source_W"]), [("route_","_")]))
     A_drain = idplace << rename_ports_by_orientation(rename_ports_by_list(straight_route(pdk, refs[0].ports["drain_W"], refs[-1].ports["drain_E"]), [("route_","_")]))
     B_drain = idplace << rename_ports_by_orientation(rename_ports_by_list(straight_route(pdk, refs[-1].ports["drain_E"], refs[0].ports["drain_W"]), [("route_","_")]))
@@ -83,14 +90,15 @@
     B_gate = idplace << rename_ports_by_orientation(rename_ports_by_list(straight_route(pdk, refs[-1].ports["gate_E"], refs[0].ports["gate_W"]), [("route_","_")]))
     # add route ports and return
     prefixes = ["A_source","B_source","A_drain","B_drain","A_gate","B_gate"]
     for i, ref in enumerate([A_src, B_src, A_drain, B_drain, A_gate, B_gate]):
         idplace.add_ports(ref.get_ports_list(),prefix=prefixes[i])
     idplace = transformed(prec_ref_center(idplace))
     idplace.unlock()
+    idplace.add_ports(create_private_ports(idplace, prefixes))
     return idplace
 
 
 @validate_arguments
 def two_nfet_interdigitized(
     pdk: MappedPDK,
     numcols: int,
@@ -103,18 +111,18 @@
     """Currently only supports two of the same nfet instances. does NOT support multipliers (currently)
     Place follows an ABABAB... pattern
     args:
     pdk = MappedPDK to use
     numcols = a single col is actually one col for both nfets (so AB). 2 cols = ABAB ... so on
     dummy = place dummy at the edges of the interdigitized place (true by default). you can specify tuple to place only on one side
     kwargs = key word arguments for multiplier. 
-    ****NOTE: These are the same as glayout.primitives.fet.multiplier arguments EXCLUDING dummy, sd_route_extension, and pdk options
+    ****NOTE: These are the same as glayout.flow.primitives.fet.multiplier arguments EXCLUDING dummy, sd_route_extension, and pdk options
     tie_layers: tuple[str,str] specifying (horizontal glayer, vertical glayer) or well tie ring. default=("met2","met1")
     """
-    base_multiplier = two_transistor_interdigitized(pdk, numcols, "nfet", dummy, **kwargs)
+    base_multiplier = macro_two_transistor_interdigitized(pdk, numcols, "nfet", dummy, **kwargs)
     # tie
     if with_tie:
         tap_separation = max(
             pdk.util_max_metal_seperation(),
             pdk.get_grule("active_diff", "active_tap")["min_separation"],
         )
         tap_separation += pdk.get_grule("p+s/d", "active_tap")["min_enclosure"]
@@ -159,8 +167,107 @@
             enclosed_rectangle=substrate_tap_encloses,
             sdlayer="p+s/d",
             horizontal_glayer="met2",
             vertical_glayer="met1",
         )
         tapring_ref = base_multiplier << ringtoadd
         base_multiplier.add_ports(tapring_ref.get_ports_list(),prefix="substratetap_")
+    base_multiplier.info["route_genid"] = "two_transistor_interdigitized"
     return base_multiplier
+
+
+
+@validate_arguments
+def two_pfet_interdigitized(
+    pdk: MappedPDK,
+    numcols: int,
+    dummy: Union[bool, tuple[bool, bool]] = True,
+    with_substrate_tap: bool = True,
+    with_tie: bool = True,
+    tie_layers: tuple[str,str]=("met2","met1"),
+    **kwargs
+) -> Component:
+    """Currently only supports two of the same nfet instances. does NOT support multipliers (currently)
+    Place follows an ABABAB... pattern
+    args:
+    pdk = MappedPDK to use
+    numcols = a single col is actually one col for both nfets (so AB). 2 cols = ABAB ... so on
+    dummy = place dummy at the edges of the interdigitized place (true by default). you can specify tuple to place only on one side
+    kwargs = key word arguments for multiplier. 
+    ****NOTE: These are the same as glayout.flow.primitives.fet.multiplier arguments EXCLUDING dummy, sd_route_extension, and pdk options
+    tie_layers: tuple[str,str] specifying (horizontal glayer, vertical glayer) or well tie ring. default=("met2","met1")
+    """
+    base_multiplier = macro_two_transistor_interdigitized(pdk, numcols, "pfet", dummy, **kwargs)
+    # tie
+    if with_tie:
+        tap_separation = max(
+            pdk.util_max_metal_seperation(),
+            pdk.get_grule("active_diff", "active_tap")["min_separation"],
+        )
+        tap_separation += pdk.get_grule("n+s/d", "active_tap")["min_enclosure"]
+        tap_encloses = (
+            2 * (tap_separation + base_multiplier.xmax),
+            2 * (tap_separation + base_multiplier.ymax),
+        )
+        tiering_ref = base_multiplier << tapring(
+            pdk,
+            enclosed_rectangle=tap_encloses,
+            sdlayer="n+s/d",
+            horizontal_glayer=tie_layers[0],
+            vertical_glayer=tie_layers[1],
+        )
+        base_multiplier.add_ports(tiering_ref.get_ports_list(), prefix="welltie_")
+        try:
+            base_multiplier<<straight_route(pdk,base_multiplier.ports["A_0_dummy_L_gsdcon_top_met_W"],base_multiplier.ports["welltie_W_top_met_W"],glayer2="met1")
+        except KeyError:
+            pass
+        try:
+            base_multiplier<<straight_route(pdk,base_multiplier.ports[f"B_{numcols-1}_dummy_R_gsdcon_top_met_E"],base_multiplier.ports["welltie_E_top_met_E"],glayer2="met1")
+        except KeyError:
+            pass
+    # add pwell
+    base_multiplier.add_padding(
+        layers=(pdk.get_glayer("nwell"),),
+        default=pdk.get_grule("nwell", "active_tap")["min_enclosure"],
+    )
+    # add substrate tap
+    base_multiplier = add_ports_perimeter(base_multiplier,layer=pdk.get_glayer("nwell"),prefix="well_")
+    # add substrate tap if with_substrate_tap
+    if with_substrate_tap:
+        substrate_tap_separation = pdk.get_grule("dnwell", "active_tap")[
+            "min_separation"
+        ]
+        substrate_tap_encloses = (
+            2 * (substrate_tap_separation + base_multiplier.xmax),
+            2 * (substrate_tap_separation + base_multiplier.ymax),
+        )
+        ringtoadd = tapring(
+            pdk,
+            enclosed_rectangle=substrate_tap_encloses,
+            sdlayer="p+s/d",
+            horizontal_glayer="met2",
+            vertical_glayer="met1",
+        )
+        tapring_ref = base_multiplier << ringtoadd
+        base_multiplier.add_ports(tapring_ref.get_ports_list(),prefix="substratetap_")
+    base_multiplier.info["route_genid"] = "two_transistor_interdigitized"
+    return base_multiplier
+
+
+
+
+def two_transistor_interdigitized(
+    pdk: MappedPDK,
+    device: Literal["nfet","pfet"],
+    numcols: int,
+    dummy: Union[bool, tuple[bool, bool]] = True,
+    with_substrate_tap: bool = True,
+    with_tie: bool = True,
+    tie_layers: tuple[str,str]=("met2","met1"),
+    **kwargs
+) -> Component:
+    if device=="nfet":
+        return two_nfet_interdigitized(pdk=pdk,numcols=numcols,dummy=dummy,with_substrate_tap=with_substrate_tap,with_tie=with_tie,tie_layers=tie_layers,**kwargs)
+    else:
+        return two_pfet_interdigitized(pdk=pdk,numcols=numcols,dummy=dummy,with_substrate_tap=with_substrate_tap,with_tie=with_tie,tie_layers=tie_layers,**kwargs)
+
+
```

### Comparing `glayout-0.0.3/glayout/placement/two_transistor_place.py` & `glayout-0.0.4/glayout/flow/placement/two_transistor_place.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from glayout.pdk.mappedpdk import MappedPDK
+from glayout.flow.pdk.mappedpdk import MappedPDK
 from pydantic import validate_arguments
 from gdsfactory.component import Component
 from typing import Callable
-from glayout.primitives.fet import nmos, pmos
-from glayout.pdk.util.comp_utils import evaluate_bbox
+from glayout.flow.primitives.fet import nmos, pmos
+from glayout.flow.pdk.util.comp_utils import evaluate_bbox
 
 @validate_arguments
 def two_transistor_place(pdk: MappedPDK, pattern: str, deviceA: tuple[Callable, dict], deviceB: tuple[Callable, dict]) -> Component:
     """Place two transitors according to the patter provided
     args:
     pdk = MappedPDK to use
     pattern = placement pattern. This string must contain only white space, the char a, the char b.
```

### Comparing `glayout-0.0.3/glayout/primitives/fet.py` & `glayout-0.0.4/glayout/flow/primitives/fet.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from gdsfactory.grid import grid
 from gdsfactory.cell import cell
 from gdsfactory.component import Component, copy
 from gdsfactory.components.rectangle import rectangle
-from glayout.pdk.mappedpdk import MappedPDK
+from glayout.flow.pdk.mappedpdk import MappedPDK
 from typing import Optional, Union
-from glayout.primitives.via_gen import via_array, via_stack
-from glayout.primitives.guardring import tapring
+from glayout.flow.primitives.via_gen import via_array, via_stack
+from glayout.flow.primitives.guardring import tapring
 from pydantic import validate_arguments
-from glayout.pdk.util.comp_utils import evaluate_bbox, to_float, to_decimal, prec_array, prec_center, prec_ref_center, movey, align_comp_to_port
-from glayout.pdk.util.port_utils import rename_ports_by_orientation, rename_ports_by_list, add_ports_perimeter, print_ports
-from glayout.routing.c_route import c_route
-from glayout.routing.L_route import L_route
-from glayout.pdk.util.snap_to_grid import component_snap_to_grid
+from glayout.flow.pdk.util.comp_utils import evaluate_bbox, to_float, to_decimal, prec_array, prec_center, prec_ref_center, movey, align_comp_to_port
+from glayout.flow.pdk.util.port_utils import rename_ports_by_orientation, rename_ports_by_list, add_ports_perimeter, print_ports
+from glayout.flow.routing.c_route import c_route
+from glayout.flow.routing.L_route import L_route
+from glayout.flow.pdk.util.snap_to_grid import component_snap_to_grid
 from decimal import Decimal
-from glayout.routing.straight_route import straight_route
-from glayout.spice import Netlist
+from glayout.flow.routing.straight_route import straight_route
+from glayout.flow.spice import Netlist
 
 
 @validate_arguments
 def __gen_fingers_macro(pdk: MappedPDK, rmult: int, fingers: int, length: float, width: float, poly_height: float, sdlayer: str, inter_finger_topmet: str) -> Component:
     """internal use: returns an array of fingers"""
     length = pdk.snap_to_2xgrid(length)
     width = pdk.snap_to_2xgrid(width)
@@ -98,14 +98,15 @@
             'length': length,
             'width': width,
             'mult': fingers * multipliers,
             'dummy_mult': multipliers
         }
     )
 
+# drain is above source
 @cell
 def multiplier(
     pdk: MappedPDK,
     sdlayer: str,
     width: Optional[float] = 3,
     length: Optional[float] = None,
     fingers: int = 1,
@@ -321,24 +322,30 @@
             # route gates right
             gatepfx = thismult + "gate_"
             this_gate = multiplier_arr.ports[gatepfx+gate_side]
             next_gate = multiplier_arr.ports[nextmult + "gate_"+gate_side]
             gate_ref = multiplier_arr << c_route(pdk, this_gate, next_gate, viaoffset=(True,False), extension=to_float(src_extension))
             multiplier_arr.add_ports(gate_ref.get_ports_list(), prefix=gatepfx)
     multiplier_arr = component_snap_to_grid(rename_ports_by_orientation(multiplier_arr))
+    # add port redirects for shortcut names (source,drain,gate N,E,S,W)
+    for pin in ["source","drain","gate"]:
+        for side in ["N","E","S","W"]:
+            aliasport = pin + "_" + side
+            actualport = "multiplier_0_" + aliasport
+            multiplier_arr.add_port(port=multiplier_arr.ports[actualport],name=aliasport)
     # recenter
     final_arr = Component()
     marrref = final_arr << multiplier_arr
     correctionxy = prec_center(marrref)
     marrref.movex(correctionxy[0]).movey(correctionxy[1])
     final_arr.add_ports(marrref.get_ports_list())
     return component_snap_to_grid(rename_ports_by_orientation(final_arr))
 
 
-@cell
+#@cell
 def nmos(
     pdk,
     width: float = 3,
     fingers: Optional[int] = 1,
     multipliers: Optional[int] = 1,
     with_tie: bool = True,
     with_dummy: Union[bool, tuple[bool, bool]] = True,
@@ -474,15 +481,15 @@
         multipliers=multipliers,
         with_dummy=with_dummy
     )
 
     return component
 
 
-@cell
+#@cell
 def pmos(
     pdk,
     width: float = 3,
     fingers: Optional[int] = 1,
     multipliers: Optional[int] = 1,
     with_tie: Optional[bool] = True,
     dnwell: Optional[bool] = False,
```

### Comparing `glayout-0.0.3/glayout/primitives/guardring.py` & `glayout-0.0.4/glayout/flow/primitives/guardring.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from glayout.pdk.mappedpdk import MappedPDK
+from glayout.flow.pdk.mappedpdk import MappedPDK
 from gdsfactory.cell import cell
 from gdsfactory.component import Component
 from gdsfactory.components.rectangle import rectangle
 from gdsfactory.components.rectangular_ring import rectangular_ring
-from glayout.primitives.via_gen import via_array, via_stack
+from glayout.flow.primitives.via_gen import via_array, via_stack
 from typing import Optional
-from glayout.pdk.util.comp_utils import to_decimal, to_float, evaluate_bbox
-from glayout.pdk.util.port_utils import print_ports
-from glayout.pdk.util.snap_to_grid import component_snap_to_grid
-from glayout.routing.L_route import L_route
+from glayout.flow.pdk.util.comp_utils import to_decimal, to_float, evaluate_bbox
+from glayout.flow.pdk.util.port_utils import print_ports
+from glayout.flow.pdk.util.snap_to_grid import component_snap_to_grid
+from glayout.flow.routing.L_route import L_route
 
 
-@cell
+#@cell
 def tapring(
     pdk: MappedPDK,
     enclosed_rectangle=(2.0, 4.0),
     sdlayer: str = "p+s/d",
     horizontal_glayer: str = "met2",
     vertical_glayer: str = "met1",
     sides: tuple[bool,bool,bool,bool] = (True,True,True,True)
```

### Comparing `glayout-0.0.3/glayout/primitives/mimcap.py` & `glayout-0.0.4/glayout/flow/primitives/mimcap.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from gdsfactory.cell import cell
 from gdsfactory.component import Component
 from gdsfactory.components.rectangle import rectangle
-from glayout.pdk.mappedpdk import MappedPDK
+from glayout.flow.pdk.mappedpdk import MappedPDK
 from typing import Optional
-from glayout.primitives.via_gen import via_array
-from glayout.pdk.util.comp_utils import prec_array, to_decimal, to_float
-from glayout.pdk.util.port_utils import rename_ports_by_orientation, add_ports_perimeter, print_ports
+from glayout.flow.primitives.via_gen import via_array
+from glayout.flow.pdk.util.comp_utils import prec_array, to_decimal, to_float
+from glayout.flow.pdk.util.port_utils import rename_ports_by_orientation, add_ports_perimeter, print_ports
 from pydantic import validate_arguments
-from glayout.routing.straight_route import straight_route
+from glayout.flow.routing.straight_route import straight_route
 from decimal import ROUND_UP, Decimal
-from glayout.spice import Netlist
+from glayout.flow.spice import Netlist
 
 @validate_arguments
 def __get_mimcap_layerconstruction_info(pdk: MappedPDK) -> tuple[str,str]:
 	"""returns the glayer metal below and glayer metal above capmet
 	args: pdk
 	"""
 	capmettop = pdk.layer_to_glayer(pdk.get_grule("capmet")["capmettop"])
@@ -47,15 +47,15 @@
 		arr_netlist.connect_netlist(
 			mimcap_netlist,
 			[]
 		)
 
 	return arr_netlist
 
-@cell
+#@cell
 def mimcap(
     pdk: MappedPDK, size: tuple[float,float]=(5.0, 5.0)
 ) -> Component:
     """create a mimcap
     args:
     pdk=pdk to use
     size=tuple(float,float) size of cap
@@ -82,15 +82,15 @@
     component = rename_ports_by_orientation(mim_cap).flatten()
 
     # netlist generation
     component.info['netlist'] = __generate_mimcap_netlist(pdk, size)
 
     return component
 
-@cell
+#@cell
 def mimcap_array(pdk: MappedPDK, rows: int, columns: int, size: tuple[float,float] = (5.0,5.0), rmult: Optional[int]=1) -> Component:
 	"""create mimcap array
 	args:
 	pdk to use
 	size = tuple(float,float) size of a single cap
 	****Note: size is the size of the capmet layer
 	ports:
```

### Comparing `glayout-0.0.3/glayout/primitives/via_gen.py` & `glayout-0.0.4/glayout/flow/primitives/via_gen.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from gdsfactory.cell import cell
 from gdsfactory.component import Component
 from gdsfactory.components.rectangle import rectangle
 from pydantic import validate_arguments
-from glayout.pdk.mappedpdk import MappedPDK
+from glayout.flow.pdk.mappedpdk import MappedPDK
 from math import floor
 from typing import Optional, Union
-from glayout.pdk.util.comp_utils import evaluate_bbox, prec_array, to_float, move, prec_ref_center, to_decimal
-from glayout.pdk.util.port_utils import rename_ports_by_orientation, print_ports
-from glayout.pdk.util.snap_to_grid import component_snap_to_grid
+from glayout.flow.pdk.util.comp_utils import evaluate_bbox, prec_array, to_float, move, prec_ref_center, to_decimal
+from glayout.flow.pdk.util.port_utils import rename_ports_by_orientation, print_ports
+from glayout.flow.pdk.util.snap_to_grid import component_snap_to_grid
 from decimal import Decimal
 from typing import Literal
 
 
 @validate_arguments
 def __error_check_order_layers(
     pdk: MappedPDK, glayer1: str, glayer2: str
```

### Comparing `glayout-0.0.3/glayout/routing/L_route.py` & `glayout-0.0.4/glayout/flow/routing/L_route.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from gdsfactory.cell import cell
 from gdsfactory.component import Component
 from gdsfactory.port import Port
-from glayout.pdk.mappedpdk import MappedPDK
+from glayout.flow.pdk.mappedpdk import MappedPDK
 from typing import Optional, Union
-from glayout.primitives.via_gen import via_stack, via_array
-from glayout.pdk.util.comp_utils import evaluate_bbox, align_comp_to_port, to_decimal, to_float, prec_ref_center, get_primitive_rectangle
-from glayout.pdk.util.port_utils import rename_ports_by_orientation, rename_ports_by_list, print_ports, assert_port_manhattan, assert_ports_perpindicular
+from glayout.flow.primitives.via_gen import via_stack, via_array
+from glayout.flow.pdk.util.comp_utils import evaluate_bbox, align_comp_to_port, to_decimal, to_float, prec_ref_center, get_primitive_rectangle
+from glayout.flow.pdk.util.port_utils import rename_ports_by_orientation, rename_ports_by_list, print_ports, assert_port_manhattan, assert_ports_perpindicular
 from decimal import Decimal
 
 
 @cell
 def L_route(
 	pdk: MappedPDK,
 	edge1: Port,
```

### Comparing `glayout-0.0.3/glayout/routing/c_route.py` & `glayout-0.0.4/glayout/flow/routing/c_route.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 from gdsfactory.cell import cell
 from gdsfactory.component import Component
 from gdsfactory.port import Port
-from glayout.pdk.mappedpdk import MappedPDK
+from glayout.flow.pdk.mappedpdk import MappedPDK
 from typing import Optional, Union
 from math import isclose
-from glayout.primitives.via_gen import via_stack
-from gdsfactory.routing.route_quad import route_quad
+from glayout.flow.primitives.via_gen import via_stack
+from glayout.flow.routing.straight_route import straight_route
 from gdsfactory.components.rectangle import rectangle
-from glayout.pdk.util.comp_utils import evaluate_bbox, get_primitive_rectangle
-from glayout.pdk.util.port_utils import add_ports_perimeter, rename_ports_by_orientation, rename_ports_by_list, print_ports, set_port_width, set_port_orientation, get_orientation
+from glayout.flow.pdk.util.comp_utils import evaluate_bbox, get_primitive_rectangle
+from glayout.flow.pdk.util.port_utils import add_ports_perimeter, rename_ports_by_orientation, rename_ports_by_list, print_ports, set_port_width, set_port_orientation, get_orientation
 from pydantic import validate_arguments
 from gdsfactory.snap import snap_to_grid
 
 
 @validate_arguments
-def __fill_empty_viastack__macro(pdk: MappedPDK, glayer: str, size: tuple[float,float]) -> Component:
-	"""returns a rectangle with ports that pretend to be viastack ports"""
+def __fill_empty_viastack__macro(pdk: MappedPDK, glayer: str, size: Optional[tuple[float,float]]=None) -> Component:
+	"""returns a rectangle with ports that pretend to be viastack ports
+	by default creates a rectangle with size double the min width of the glayer"""
+	if size is None:
+		size = pdk.snap_to_2xgrid([2*pdk.get_grule(glayer)["min_width"],2*pdk.get_grule(glayer)["min_width"]])
 	comp = rectangle(size=size,layer=pdk.get_glayer(glayer),centered=True)
 	return rename_ports_by_orientation(rename_ports_by_list(comp,replace_list=[("e","top_met_")])).flatten()
 
 @cell
 def c_route(
 	pdk: MappedPDK, 
 	edge1: Port, 
@@ -28,15 +31,16 @@
 	width1: Optional[float] = None, 
 	width2: Optional[float] = None,
 	cwidth: Optional[float] = None,
 	e1glayer: Optional[str] = None, 
 	e2glayer: Optional[str] = None, 
 	cglayer: Optional[str] = None, 
 	viaoffset: Optional[Union[bool,tuple[Optional[bool],Optional[bool]]]]=(True,True),
-	fullbottom: Optional[bool] = False
+	fullbottom: Optional[bool] = False,
+	debug=False
 ) -> Component:
 	"""creates a C shaped route between two Ports.
 	
 	edge1--|
 	       |
 	edge2--|
 	
@@ -53,14 +57,17 @@
 	cglayer = glayer for the connection part (part that goes through a via) defaults to e1glayer met+1
 	viaoffset = offsets the via so that it is flush with the cglayer (may be needed for drc) i.e. -| vs _|
 	- True offsets via towards the other via
 	- False offsets via away from the other via
 	- None means center (no offset)
 	****NOTE: viaoffset pushes both vias towards each other slightly
 	"""
+	if debug:
+		pass
+		#import pdb; pdb.set_trace()
 	# error checking and figure out args
 	if round(edge1.orientation) % 90 or round(edge2.orientation) % 90:
 		raise ValueError("Ports must be vertical or horizontal")
 	if not isclose(edge1.orientation,edge2.orientation):
 		raise ValueError("Ports must be parralel and have same orientation")
 	width1 = width1 if width1 else edge1.width
 	width2 = width2 if width2 else edge1.width
@@ -76,16 +83,17 @@
 	pdk.has_required_glayers([e1glayer,e2glayer,cglayer])
 	pdk.activate()
 	extension = snap_to_grid(extension)
 	# create route
 	croute = Component()
 	viastack1 = via_stack(pdk,e1glayer,cglayer,fullbottom=fullbottom,assume_bottom_via=True)
 	viastack2 = via_stack(pdk,e2glayer,cglayer,fullbottom=fullbottom,assume_bottom_via=True)
-	if e1glayer == e2glayer:
-		pass
+	if e1glayer==cglayer and e2glayer==cglayer:
+		viastack1 = __fill_empty_viastack__macro(pdk,e1glayer)
+		viastack2 = __fill_empty_viastack__macro(pdk,e2glayer)
 	elif e1glayer == cglayer:
 		viastack1 = __fill_empty_viastack__macro(pdk,e1glayer,size=evaluate_bbox(viastack2))
 	elif e2glayer == cglayer:
 		viastack2 = __fill_empty_viastack__macro(pdk,e2glayer,size=evaluate_bbox(viastack1))
 	# find extension
 	e1_length = snap_to_grid(extension + evaluate_bbox(viastack1)[0])
 	e2_length = snap_to_grid(extension + evaluate_bbox(viastack2)[0])
@@ -159,44 +167,59 @@
 		me1.move(destination=e1_extension.ports["e_E"].center)
 		me2.move(destination=e2_extension.ports["e_E"].center)
 		via_flush *= 1 if me1.ymax > me2.ymax else -1
 		me1.movex(0-viastack1.xmax).movey(0-via_flush1)
 		me2.movex(0-viastack2.xmax).movey(via_flush2)
 		me1, me2 = (me1, me2) if (me1.origin[1] > me2.origin[1]) else (me2, me1)
 		route_ports = [me1.ports["top_met_N"],me2.ports["top_met_S"]]
+		fix_connection_direction = "E"
+		fix_ports = [me1.ports["top_met_E"],me2.ports["top_met_E"]]
 	elif round(edge1.orientation) == 180:# facing west
 		me1.move(destination=e1_extension.ports["e_W"].center)
 		me2.move(destination=e2_extension.ports["e_W"].center)
 		via_flush *= 1 if me1.ymax > me2.ymax else -1
 		me1.movex(viastack1.xmax).movey(0-via_flush1)
 		me2.movex(viastack2.xmax).movey(via_flush2)
 		me1, me2 = (me1, me2) if (me1.origin[1] > me2.origin[1]) else (me2, me1)
 		route_ports = [me1.ports["top_met_N"],me2.ports["top_met_S"]]
+		fix_connection_direction = "E"
+		fix_ports = [me1.ports["top_met_E"],me2.ports["top_met_E"]]
 	elif round(edge1.orientation) == 270:# facing south
 		me1.move(destination=e1_extension.ports["e_S"].center)
 		me2.move(destination=e2_extension.ports["e_S"].center)
 		via_flush *= 1 if me1.xmax > me2.xmax else -1
 		me1.movey(viastack1.xmax).movex(0-via_flush1)
 		me2.movey(viastack2.xmax).movex(via_flush2)
 		me1, me2 = (me1, me2) if (me1.origin[0] > me2.origin[0]) else (me2, me1)
 		route_ports = [me1.ports["top_met_E"],me2.ports["top_met_W"]]
+		fix_connection_direction = "N"
+		fix_ports = [me1.ports["top_met_N"],me2.ports["top_met_N"]]
 	else:#facing north
 		me1.move(destination=e1_extension.ports["e_N"].center)
 		me2.move(destination=e2_extension.ports["e_N"].center)
 		via_flush *= 1 if me1.xmax > me2.xmax else -1
 		me1.movey(0-viastack1.xmax).movex(0-via_flush1)
 		me2.movey(0-viastack2.xmax).movex(via_flush2)
 		me1, me2 = (me1, me2) if (me1.origin[0] > me2.origin[0]) else (me2, me1)
 		route_ports = [me1.ports["top_met_E"],me2.ports["top_met_W"]]
+		fix_connection_direction = "N"
+		fix_ports = [me1.ports["top_met_N"],me2.ports["top_met_N"]]
 	# connect extensions, add ports, return
 	croute << e1_extension_comp
 	croute << e2_extension_comp
 	if cwidth:
 		route_ports = [set_port_width(port_,cwidth) for port_ in route_ports]
 	route_ports[0].width = route_ports[1].width = max(route_ports[0].width, route_ports[1].width)
-	cconnection = croute << route_quad(route_ports[0],route_ports[1],layer=pdk.get_glayer(cglayer))
+	route_port0 = route_ports[0].copy()
+	route_port1 = route_ports[1].copy()
+	route_port0.layer = route_port1.layer = pdk.get_glayer(cglayer)
+	cconnection = croute << straight_route(pdk, route_port0,route_port1,glayer1=cglayer,glayer2=cglayer)
+	for _port in fix_ports:
+		port2 = cconnection.ports["route_"+fix_connection_direction]
+		port2.layer = _port.layer = pdk.get_glayer(cglayer)
+		croute << straight_route(pdk, _port, port2, glayer1=cglayer,glayer2=cglayer)
 	for i,port_to_add in enumerate(route_ports):
 		orta = get_orientation(port_to_add.orientation)
 		route_ports[i] = set_port_orientation(port_to_add, orta)
 	croute.add_ports(route_ports,prefix="con_")
 	return rename_ports_by_orientation(rename_ports_by_list(croute.flatten(), [("con_","con_")]))
```

### Comparing `glayout-0.0.3/glayout/routing/straight_route.py` & `glayout-0.0.4/glayout/flow/routing/straight_route.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from gdsfactory.cell import cell
 from gdsfactory.component import Component
 from gdsfactory.port import Port
-from glayout.pdk.mappedpdk import MappedPDK
+from glayout.flow.pdk.mappedpdk import MappedPDK
 from typing import Optional
-from glayout.primitives.via_gen import via_stack, via_array
+from glayout.flow.primitives.via_gen import via_stack, via_array
 from gdsfactory.components.rectangle import rectangle
-from glayout.pdk.util.comp_utils import evaluate_bbox, align_comp_to_port
-from glayout.pdk.util.port_utils import assert_port_manhattan, set_port_orientation, add_ports_perimeter
+from glayout.flow.pdk.util.comp_utils import evaluate_bbox, align_comp_to_port
+from glayout.flow.pdk.util.port_utils import assert_port_manhattan, set_port_orientation, add_ports_perimeter
 from gdstk import rectangle as primitive_rectangle
 
 
 @cell
 def straight_route(
 	pdk: MappedPDK,
 	edge1: Port,
```

### Comparing `glayout-0.0.3/glayout/spice/netlist.py` & `glayout-0.0.4/glayout/flow/spice/netlist.py`

 * *Files identical despite different names*

### Comparing `glayout-0.0.3/glayout.egg-info/PKG-INFO` & `glayout-0.0.4/glayout.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: glayout
-Version: 0.0.3
-Summary: Fully Open-Source Autonomous SoC Synthesis using Customizable Cell-Based Synthesizable Analog Circuits
-Home-page: https://github.com/idea-fasoc/OpenFASOC
-Author:  msaligane
-Author-email: mehdi@umich.edu
-License: MIT
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
+Version: 0.0.4
+Summary: A human language to analog layout API with support for different technologies.
+Home-page: https://github.com/idea-fasoc/OpenFASOC/tree/main/openfasoc/generators/glayout
+Author: Ali Hammoud, Harsh Khandeparkar, Vijay Shankar, Chetanya Goyal, Sakib Pathen, Arlene Dai, Ryan Wans, Mehdi Saligane
+Author-email: alibilal@umich.edu, Harsh, vijayshankar.renganathan@analog.com, Chetanya, spathen@umich.edu, arlendai@umich.edu, Ryan, mehdi@umich.edu
 Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 All functions, classes, etc have a help docustring. See python help() for specific questions
 
 - [Installation](#installation)
 - [Glayout](#glayout)
@@ -35,14 +33,30 @@
       - [PortTree](#porttree)
     - [Snap to 2x grid](#snap-to-2x-grid)
     - [Mimcaps Implementation](#mimcaps-implementation)
     - [DRC](#drc)
     - [LVS, and Labeling Issues](#lvs-and-labeling-issues)
     - [Addressing Complicated Requirments with Default Decorators](#addressing-complicated-requirments-with-default-decorators)
   - [API overview](#api-overview)
+- [Natural Language Processing](#natural-language-processing)
+  - [Standard Components](#standard-components)
+    - [NMOS](#nmos)
+    - [PMOS](#pmos)
+    - [MIMCAP](#mimcap)
+    - [MIMCAP Array](#mimcap-array)
+    - [Differential Pair](#differential-pair)
+  - [Strict Syntax Commands](#strict-syntax-commands)
+    - [Import Command](#import-command)
+    - [Create Parameters Command](#create-parameters-command)
+    - [Place Command](#place-command)
+    - [Move Command](#move-command)
+    - [Route Command](#route-command)
+  - [Non-Standard Components Which can be Imported](#non-standard-components-which-can-be-imported)
+    - [CrossCoupledInverters](#crosscoupledinverters)
+  - [StrictSyntax Style Guide](#strictsyntax-style-guide)
 
 # Installation
 You must be running python3.10 or later. 
 - Run `python3 -m pip install -r requirements.txt` in the gdsfactory-gen directory
 - open Klayout
   - go to Tools -> Manage Packages
   - under "Install New Packages" search for "klive"
@@ -58,20 +72,20 @@
 ### Generic Layers
 Almost all CMOS technologies have some version of basically the same layers, some of which are: “active/diffusion”, ”metal contact”, “metal 1”, “via1”, …etc. The layer description format of tuple(integer, integer) is standard. The idea of a generic layer is to map the standard layer names to a specific tuple(integer, integer) depending on the technology. For example, a generic layer present in most technologies is “metal 2”. The sky130 version of “metal 2” is the integer tuple (68, 20). The gf180 version of “metal 2” is the integer tuple (34,0). Importantly, the designer does not use or care about the value of the integer tuple. The designer only cares about the layer it represents, which they can always access in python from the generic name.  
 MappedPDK provides the designer with all the generic layers necessary, some of which are: “diffusion”, “dnwell”, “nwell”, “pwell”, “p+s/d”, “n+s/d”, “mcon”...etc. MappedPDK guarantees that regardless of which technology is represented ‘under the hood’ and what the value of the tuple(integer, integer), these layers will be accessible by the same names. The designer can access generic layers using the following syntax (for example):  
 `MappedPDK.get_glayer(“metal 2”)`  
 This “get_glayer” instance method of the MappedPDK takes the generic layer name and returns the tuple(integer, integer) specific to the technology. A MappedPDK object supports mappings for all design layers necessary. The BEOL generic layers support a metal stack met1-met5. Because metal stacks and some layers are technology dependent, the MappedPDK contains the “MappedPDK.verify_glayers()” method for verifying the presence of layers. For example, if a technology BEOL contains met1-met2, but a cell requires met3, it is possible for the cell generator to verify at runtime that the technology contains met3.
 
 **BEOL Example Generic Layer Mappings**
-| Generic Layer Name | sky130 | gf180 |
-| :-: | :-: | :-: |
-|mcon| (66,44) | (33,0) |
-|met1| (67,20) | (34,0) |
-|via1| (67,44) | (35,0) |
-|met2| (68,20) | (36,0) |
+| Generic Layer Name | sky130  | gf180  |
+| :----------------: | :-----: | :----: |
+|        mcon        | (66,44) | (33,0) |
+|        met1        | (67,20) | (34,0) |
+|        via1        | (67,44) | (35,0) |
+|        met2        | (68,20) | (36,0) |
 
 
 ### Generic Rule Guide
 Almost all CMOS technologies have some version of basically the same three rules: “min_separation”, “min_enclosure”, and “min_width” (or “width” for via layers). Hundreds of rules arise by prescribing one of these three rules between combinations of layers. For example, there may be a rule which requires a “min_enclosure” between “via1” and “metal 2”. There can also be “self rules” or rules describing a requirement between a layer and itself; most “min_width” rules are self rules. An example of a “self rule” between “metal 2” and “metal 2” would be the “min_width” rule.  
 The description of CMOS rules provided in the above paragraph fits very well within a mathematical graph. Layers can be thought of as vertices in the graph. Rules describe relationships between layers; rules can be thought of as edges in the graph. A “self rule” can be thought of as a “self edge” in the graph (an edge connecting a vertex to itself). This graph can be described mathematically as an undirected graph.  
 **figure here of example rule graph**  
 To greatly simplify the rule graph, context dependent rules (sometimes referred to as lambda rules) are eliminated by taking the worst case value for each rule. This allows the designer to lookup rules without providing any additional context of surrounding layer geometry (usually required for dependent rules).  
@@ -91,34 +105,34 @@
 `from gdsfactory.cell import cell`   
 The MappedPDK.get_glayer and MappedPDK.get_grule methods enable the construction of DRC clean layouts programmatically. However, it is the responsibility of the Cell factory programmer to ensure that the proper rules and layer checks are executed. **The quality of the programmer is the quality of the cell.**
 ### Via Stack Generator
 The only stand alone cell (cell factory which does not call other cell factories) in the glayout package is the via stack. Cell factories generally follow a similar programming procedure, so via stack provides a good introduction to the cell factory structure.  
 Like all cells, via stack takes as the first argument a MappedPDK object. There are two other required arguments which specify the generic layers to create the via stack between; the order in which these “glayers” (another name for generic layers) are provided does not matter. There are also several optional arguments providing more specific layout control. To explain this cell, the following function call will be assumed:  
 `via_stack(GF180_MappedPDK, “active”, “metal 3”)` OR  `via_stack(GF180_MappedPDK, “metal 3”, “active”)`  
 Most cells start by running layer error checking. The via stack must verify that the provided MappedPDK contains both glayers provided and both glayers provided can be routed between. For example, it is usually not possible to route from “nwell” without an “n+s/d” implant, so if one of the layers provided is “nwell”, via stack raises an exception. Additionally, via stack must verify that all layers in between the provided glayers are available in the pdk. In this case, the required glayers are: “active”, “metal contact”, “metal 1”, “via 1”, “metal 2”, via 2”, and “metal 3”. For the passed MappedPDK (GF180), all required glayers are present, but in the case that a glayer is not present, via stack raises an exception.  
-layer error checking is done with [`pdk.has_required_glayers(glayers_list)`](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/pdk/mappedpdk.py#L142).  
+layer error checking is done with [`pdk.has_required_glayers(glayers_list)`](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/flow//pdk/mappedpdk.py#L142).  
 The via stack then loops through these layers, placing them one at a time. To legally size and place each layer, via stack must consider “min_enclosure” and “width” rules for vias and metals. For example, to lay the “active” layer, the “metal contact” “width” and the “metal contact” to “active” “min_enclosure” rules must be considered. To lay the “metal 1” layer, the “min_enclosure” and “width” rules of both the via above and the via below “metal 1” must be considered. The programmer of the generic cells must consider all relevant rules to produce a legal layout. Rules are accessed in cell code using the `MappedPDK.get_grule` method.
 ### Routing
 Routing utilities are required to create complicated hierarchical designs. At the backend of routing is the gdsfactory “Port” object. Fundamentally, ports describe a polygon edge. Ports include center, width, and orientation of the edge, along with other attributes and utility methods. The glayout routing functions operate to create paths between ports.  
 As described with the via stack example above, the checks and sizings necessary for legal layout are executed in the cell generator. Glayout routing functions do not need to understand cell context; for this reason, routing functions are called “dumb routes”. There are three “dumb route” utilities: straight route, L route, and C route. Dumb routes are simple, but contain optional arguments which allow for precise control over created paths. The default path behavior is easy to predict and will generally make the most reasonable decisions if no direction is provided.   
 For example, Straight route creates a straight path directly between two ports. If the two provided ports are not collinear or have different orientations, the function will by default route from the first port to the imaginary line stretching perpendicularly from the second port. By default, the route will begin on the same layer as the first port and will lay a via stack if necessary at the second port. If two ports are parallel, Straight route will raise an exception.
 
 **Straight Route Default Behavoir:**
 ![straight route default behavoir](docs/straight_route_def_beh.png)  
 
 L route and C route also create simple paths. L route creates an L shaped route (two straight paths perpendicular) and C route creates a C shaped route (two parallel paths connected by a straight path).  
 ### PDK Agnostic Hierarchical Cells
 All cells other than the via stack contain hierarchy. Combining hierarchy and careful routing allows for clean layouts while increasing complexity. 
-#### Example 1: [via_array](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/primitives/via_gen.py#L180)
-The most basic hierarchical cell is the [via_array](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/primitives/via_gen.py#L180). Via array is composed of via stacks and has a similar interface to the via stack generator, but additionally accepts a size argument. The array spacing computation is another example of the programmers role in creating DRC clean layout. After error checking, the via array program creates the via stack single element that will be copied to create the array. Then, the generator loops through each layer and uses the gdsfactory component.extract method to get the dimension of that layer in the via stack; The min spacing for that layer is `pdk.get_grule(layer)["min_separation"] + 2*layer_dim`. After looping through the entire array, The maximum seperation is the correct spacing to use.  
-#### Example 2: [tapring](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/primitives/guardring.py)
-tapring produces a substrate / well tap rectanglular ring that legally enclose a rectangular shape. `gdsfactory.component.rectangular_ring` is used along with glayout [via_array](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/primitives/via_gen.py#L180). The ring is always of minimum width and legalizing the ring is easy because via_array does most of the work. Special care is taken at the corners to ensure min spacing between adjacent metal layers is not below min_separation. Although not currently implemented, error checking for this ring should check the size is not too small (separation between edges is not legal).  
+#### Example 1: [via_array](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/flow/primitives/via_gen.py#L180)
+The most basic hierarchical cell is the [via_array](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/flow/primitives/via_gen.py#L180). Via array is composed of via stacks and has a similar interface to the via stack generator, but additionally accepts a size argument. The array spacing computation is another example of the programmers role in creating DRC clean layout. After error checking, the via array program creates the via stack single element that will be copied to create the array. Then, the generator loops through each layer and uses the gdsfactory component.extract method to get the dimension of that layer in the via stack; The min spacing for that layer is `pdk.get_grule(layer)["min_separation"] + 2*layer_dim`. After looping through the entire array, The maximum seperation is the correct spacing to use.  
+#### Example 2: [tapring](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/flow/primitives/guardring.py)
+tapring produces a substrate / well tap rectanglular ring that legally enclose a rectangular shape. `gdsfactory.component.rectangular_ring` is used along with glayout [via_array](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/flow/primitives/via_gen.py#L180). The ring is always of minimum width and legalizing the ring is easy because via_array does most of the work. Special care is taken at the corners to ensure min spacing between adjacent metal layers is not below min_separation. Although not currently implemented, error checking for this ring should check the size is not too small (separation between edges is not legal).  
 Generators should be made as generic as possible. In this case, tapring can produce either a p-tap or n-tap ring. Glayers are just strings and they can be passed to functions as arguments. Also, you glayer variables can be passed directly to `pdk.get_grule(glayer_var)`.
-#### Example 3: [fet](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/primitives/fet.py)
-The most important component factory in glayout is the [multiplier](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/primitives/fet.py#L61) because it handles the difficult task of creating legal transistors. By passing the source/drain layer (either "p+s/d" or "n+s/d") multiplier code is reused to create nmos and pmos transistors. arrays of multipliers can be created to allow for transistors with several multipliers. read the help docustring for all functions in [fet.py](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/primitives/fet.py)
+#### Example 3: [fet](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/flow/primitives/fet.py)
+The most important component factory in glayout is the [multiplier](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/flow/primitives/fet.py#L61) because it handles the difficult task of creating legal transistors. By passing the source/drain layer (either "p+s/d" or "n+s/d") multiplier code is reused to create nmos and pmos transistors. arrays of multipliers can be created to allow for transistors with several multipliers. read the help docustring for all functions in [fet.py](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/flow/primitives/fet.py)
 
 ## Advanced Topics
 The following topics are only neccessary if you want to code with glayout, but are not neccessary for a basic understanding of glayout.
 ### Cells and PDK.activate()
 All cell factories should be decorated with the `@cell` decorator which can be imported from gdsfactory with `from gdsfactory.cell import cell`. You must also call pdk.activate() for cells to correctly work. This is related to caching, gds/oasis write settings, default decorators, etc.
 ### Important GDSFactory Notes and Glayout Utilities
 The GDSFactory API is extremely versatile and there are many useful features. It takes some experience to learn about all features and identify the most useful tools from GDSFactory. GDSFactory serves as the backend GDS manipulation library and as an object oriented tool kit with several useful classes including: Components, Component References, and Ports. There are also common shapes as Components in GDSFactory such as rectangles, circles, rectangular_rings, etc. To automate common tasks that do not fit into GDSFactory, Glayout includes many utility functions. The most important of these functions are also addressed here.  
@@ -133,63 +147,63 @@
 	- Component booleans: see the gdsfactory documentation for how to run boolean operations of components.
 	- Component.write_gds(): write the gds to disk
 	- Component.bbox: return bounding box of the component (xmin,ymin),(xmax,ymax). Glayout has an evaluate_bbox function which return the x and y dimensions of the bbox
 	- insertion operator: `ref = Component << Component_to_add`
 	- Component.add(): add an one of several types to a Component. (more flexible than << operator)
 	- Component.ref()/.ref_center(): return a reference to a component
 
-It is not possible to move Components in GDSFactory. GDSFactory has a Component cache, so moving a component may invalidate the cache, but there are situations where you want to move a component; For these situations, use the glayout [move](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/pdk/util/comp_utils.py#L24), [movex](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/pdk/util/comp_utils.py#L63), [movey](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/pdk/util/comp_utils.py#L73) functions.
+It is not possible to move Components in GDSFactory. GDSFactory has a Component cache, so moving a component may invalidate the cache, but there are situations where you want to move a component; For these situations, use the glayout [move](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/flow/pdk/util/comp_utils.py#L24), [movex](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/flow/pdk/util/comp_utils.py#L63), [movey](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/flow/pdk/util/comp_utils.py#L73) functions.
 
 - Component references are pointers to components. They have many of the same methods as Components with some additions.
 	- ComponentReference.parent: the Component which this component reference points to
 	- ComponentReference.movex, movey, move: you can move ComponentReferences
 	- ComponentReference.get_ports_list(): get a list of ports in the component.
 Ports are edge descriptions.
 
 To add a ComponentReference to a Component, you cannot use the insertion operator. Use the Component.add() method.
 
 - A port describes a single edge of a polygon. The most useful port attributes are **width, center tuple(x,y), orientation (degrees), and layer of the edge**. 
     - For example, the rectangle cell factory provided in gdsfactory.components.rectangle returns a Component type with the following port names: e1, e2, e3, e4.
     	- e1=West, e2=North, e3=East, e4=South. The default naming scheme of ports in GDSFactory is not descriptive
-    	- use glayout [rename_ports_by_orientation](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/pdk/util/port_utils.py#L67), [rename_ports_by_list](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/pdk/util/port_utils.py#L91) functions and see below for port naming best practices guide
-    	- glayout [get_orientation](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/pdk/util/port_utils.py#L124): returns the letter (N,E,S,W) or degrees of orientation of port.  by default returns the one you do not have. see help.
-    	- glayout [assert_port_manhattan](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/pdk/util/port_utils.py#L159): assert that a port or list or ports have orientation N, E, S, or W
-    	- glayout [assert_ports_perpindicular](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/pdk/util/port_utils.py#L181): assert two ports are perpindicular
-    	- glayout [set_port_orientation](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/pdk/util/port_utils.py#L181): return new port which is copy of old port but with new orientation
-    	- glayout [set_port_width](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/pdk/util/port_utils.py#L202): return a new port which is a copy of the old one, but with new width
+    	- use glayout [rename_ports_by_orientation](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/flow/pdk/util/port_utils.py#L67), [rename_ports_by_list](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/flow/pdk/util/port_utils.py#L91) functions and see below for port naming best practices guide
+    	- glayout [get_orientation](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/flow/pdk/util/port_utils.py#L124): returns the letter (N,E,S,W) or degrees of orientation of port.  by default returns the one you do not have. see help.
+    	- glayout [assert_port_manhattan](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/flow/pdk/util/port_utils.py#L159): assert that a port or list or ports have orientation N, E, S, or W
+    	- glayout [assert_ports_perpindicular](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/flow/pdk/util/port_utils.py#L181): assert two ports are perpindicular
+    	- glayout [set_port_orientation](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/flow/pdk/util/port_utils.py#L181): return new port which is copy of old port but with new orientation
+    	- glayout [set_port_width](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/flow/pdk/util/port_utils.py#L202): return a new port which is a copy of the old one, but with new width
 
-A very important utility is [align_comp_to_port](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/pdk/util/comp_utils.py#L83): pass a component or componentReference and a port, and align the component to any edge of the port.
+A very important utility is [align_comp_to_port](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/flow/pdk/util/comp_utils.py#L83): pass a component or componentReference and a port, and align the component to any edge of the port.
 
 ### Port Naming Best Practices Guide
 As previously pointed out, the default naming of ports in GDSFactory is not descriptive. By default gdsfactory.components.rectangle returns ports e1 (West port), e2 (North port), e3 (East port), e4 (South port). Additionally, complicated hiearchies can result in thousands of ports, so organizing ports is a neccessity. The below best practices guide should be used to organize ports
 - Ports use the "\_" syntax. Think of this like a directory tree for files. Each time you introduce a new level of hiearchy, you should add a prefix + "\_" describing the cell. 
 	- For example, adding a via_array to the edge of a tapring, you should call
 `tapring.add_ports(via_array.get_ports_list(),prefix="topviaarray_")`
 	- The port rename functions look for the "\_" syntax. You can NOT use the port rename functions without this syntax.
 - The last 2 characters of a port name should "\_" followed by the orientation (N, E, S, or W)
-	- you can easily achieve this by calling glayout [`rename_ports_by_orientation`](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/pdk/util/port_utils.py#L67) before returning a component (just the names end with "\_" before calling this function)
+	- you can easily achieve this by calling glayout [`rename_ports_by_orientation`](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/flow/pdk/util/port_utils.py#L67) before returning a component (just the names end with "\_" before calling this function)
 - **USE PORTS**: be sure to correctly add and label ports to components you make because you do not know when they will be used in other cells. 
 
 #### PortTree
-The [PortTree](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/pdk/util/port_utils.py#L232) class is designed to assist in finding ports and understanding port structure. Initialize a PortTree by calling [`PortTree(Component or ComponentReference)`](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/pdk/util/port_utils.py#L245). The PortTree will internally construct a directory tree structure from the Component's ports. You can use [`PortTree.print()`](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/pdk/util/port_utils.py#L304) to print this whole structure for a nice figure explaining a Component's ports. See the example print output from a via_stack component below:
+The [PortTree](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/flow/pdk/util/port_utils.py#L232) class is designed to assist in finding ports and understanding port structure. Initialize a PortTree by calling [`PortTree(Component or ComponentReference)`](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/flow/pdk/util/port_utils.py#L245). The PortTree will internally construct a directory tree structure from the Component's ports. You can use [`PortTree.print()`](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/flow/pdk/util/port_utils.py#L304) to print this whole structure for a nice figure explaining a Component's ports. See the example print output from a via_stack component below:
 
 **PortTree of a via_stack:**
 ![PortTree example](docs/PortTreeExample.png)
 
 ### Snap to 2x grid
 All rules (when creating a MappedPDK) and all user provided float arguments must be snapped to 2*grid size. This is because it is possible to center a component. Centering a component which has a dimension on grid may result in off grid polygons. You can snap floating point values to grid easily by calling `pdk.snap_to_2x_grid()`. You should also take care to snap to 2xgrid whenever you see it is neccessary while writing generator code. For example, most generators which take a size(xdim: float, ydim: float) argument should snap to 2xgrid.
 ### Mimcaps Implementation
 Although many technolgies have 2 or more mimcap options, there is currently only 1 mimcap option supported. When creating a mapped pdk, you specify the cap metal layer as a generic layer, but you specify the metal above and metal below the cap met as part of the DRC rule set for `pdk.get_grule("capmet")`. You can access the metal above capmet with `pdk.get_grule(capmet)["capmettop"]`.
 ### DRC
 If the system has klayout installed and you provide a klayout lydrc script for your MappedPDK, you can run DRC from python by calling pdk.drc(Component or GDS). The return value is a boolean (legal or not legal) and a lyrdb (xml format) file is written describing each DRC error. This file can be opened graphically in klayout with the following syntax `klayout layout.gds -m drc.lyrdb`
 ### LVS, and Labeling Issues
 There are no glayers for labeling or pins, all cells are generated without any labels. You can easily add pins to your component manually after glayout write the gds, or by using ports, you can write a function for adding labels and pins. See [sky130_nist_tapeout example function](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/tapeout_and_RL/sky130_nist_tapeout.py#L97). 
 ### Addressing Complicated Requirments with Default Decorators
 A python decorator is a function (the decorator) is a function which is called on another function. It can be used to enhance the features of a function. With GDSFactory Pdk (and MappedPDK objects) you can define a default decorator which runs on any cell factory (cell factories must be decorated with the `@cell` decorator). The default decorator you define runs in addition to the `@cell` decorator. The defined default_decorator should accept as argument a Component and return a Component.  
-This should be used when dealing with PDK specfic requirments that do not fit into the MappedPDK framework. For example, sky130 has a NPC (nitride poly cut) layer which **must** be used wherever licon (local interconnect contact) is laid over poly. It does not make sense to modify MappedPDK to add a generic NPC layer AND modify all cell factories; sky130 is unqiue in this requirment, so modifying MappedPDK/all cell factories would make glayout less generic. Instead, we define a default_decorator [`sky130_add_npc(Component) -> Component`](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/pdk/sky130_mapped/sky130_add_npc.py). This function uses booleans to add npc anywhere licon is laid over poly (it also joins NPC polygons if they are closer than the NPC min separation rule). Layers and rules in this technology specific function are hard coded because this decorator will only run for sky130 is the active pdk (this is one reason why you must be sure that pdk is activated).
+This should be used when dealing with PDK specfic requirments that do not fit into the MappedPDK framework. For example, sky130 has a NPC (nitride poly cut) layer which **must** be used wherever licon (local interconnect contact) is laid over poly. It does not make sense to modify MappedPDK to add a generic NPC layer AND modify all cell factories; sky130 is unqiue in this requirment, so modifying MappedPDK/all cell factories would make glayout less generic. Instead, we define a default_decorator [`sky130_add_npc(Component) -> Component`](https://github.com/alibillalhammoud/OpenFASOC/blob/main/openfasoc/generators/gdsfactory-gen/glayout/flow/pdk/sky130_mapped/sky130_add_npc.py). This function uses booleans to add npc anywhere licon is laid over poly (it also joins NPC polygons if they are closer than the NPC min separation rule). Layers and rules in this technology specific function are hard coded because this decorator will only run for sky130 is the active pdk (this is one reason why you must be sure that pdk is activated).
 
 ## API overview
 This section provides a high-level overview of all functions in glayout. See **docs** (TODO) printed docustrings of all files.
 
 
 - glayout: 
   - generators
@@ -234,9 +248,167 @@
           - get_padding_points_cc: get points of a rectangle which pads (with some extra space optionally) a component. (e.g. lay p+s/d over diffusion with padding=0.2um)
           - to_decimal: convert a float or list of float (or decimal) to python decimal
           - to_float: convert decimal or list of decimal (or float) to python float
         - port_utils.py
         - print_rules.py
         - snap_to_grid.py
         - component_array_create.py
+# Natural Language Processing
+In addition to python code, there is also natural language capabilities within Glayout. Glayout strictsyntax is a command language for producing analog circuit layout. Component placement in Analog layout is drawing the geometric shapes representing various Components. Routing is the process of connecting these Components by drawing metal lines between them. Glayout strictsyntax allows the designer to place, move, and connect circuit Components without needing to draw them, rather with strictsyntax the designer can describe them in simple words and with simple commands. The Glayout runtime interprets these commands and will automatically place, move, and route the final layout.
+
+To get started with the glayout runtime, you can create a basic run.py script using the following:
+```
+import argparse
+from glayout.syntaxer.dynamic_load import run_session
+from pathlib import Path
+
+if __name__ == "__main__":
+    parser = argparse.ArgumentParser(description="Manage, interact, and run conversation sessions.")
+    parser.add_argument(
+        "-l",
+        "--load_conversation",
+        type=Path,
+        help="Specify the file path to load a previous conversation",
+    )
+    parser.add_argument(
+        "-r",
+        "--restore_and_exit",
+        action='store_true',
+        help="Restore the conversation state and exit",
+    )
+    args = parser.parse_args()
+    run_session(args.load_conversation, args.restore_and_exit)
+```
+By entering `python run.py` with no arguments to the above script you can begin creating layout with the strictsyntax.
+
+Components are predesigned circuits which can be used as building blocks to create larger circuits. Components are highly modular and have many parameters which can be configured when they are placed. Placing a Component is also known as instantiating the Component. Instances must be given a name. The instance name is called the ComponentRef. Components are also hierarchical, meaning that a Component can be made up of many sub-Components. Also, after making a circuit with Glayout, it can be used in the future as a Component in a larger circuit.
+
+Components can be connected together through a process called routing. Components include several Ports. Ports serve as nodes on Components. Ports are used to create connections (also known as routes) between different Components in a circuit. Ports represent the input or output nodes for Components in the layout and act like an interface to the Component. In the geometry of the layout, Ports correspond to edges of nodes. 
+Ports are accessed through an organized naming syntax. The names correspond to the function of the Port. For example, MOS Field-Effect Transistors (MOSFETs) have three main nodes: drain, gate, and source. Remember, each Port corresponds to an edge in layout, so they always end with a direction indicator. Direction indicators are North (N), East (E), South (S), or West (W). Indicators N, E, S, W are for specifying which edge of the node we are referring to. For example, if we want to refer to the west edge of the drain node, we would use the port name “ComponentRef_drain_W”, replacing ComponentRef with the name of the Component instance.
+
+## Standard Components
+There are several existing components which are part of the Glayout runtime. These components are described below and do not require any imports. Note that it is also possible to import other Components.
+
+### NMOS
+Nmos is an n-type mosfet transistor. It is also referred to as nmos, n-type, or nfet. It has the following parameters which are configurable when you place the component: 
+length: a float parameter specifying the transistor length
+width: a float parameter specifying the width of a single transistor
+fingers: an integer parameter which multiplies the width. For example, if fingers is 3, then the size will be 3 times the width.
+multipliers: An integer parameter specifying how many rows of fingers to place. Each row is equivalent to width*fingers in size, so that the total size is multipliers*width*fingers. Default is 1.
+with_tie: True or False, specifies if a bulk tie is required. Set this true unless the designer specifies otherwise.
+with_substrate_tap: True or False. If True, then add a substrate tap on the very outside perimeter of nmos. Set this to False unless the designer specifies otherwise.
+with_dummy: When True, specifies dummy devices should be added to the edges of the transistor. You should set this to True unless the designer specifies otherwise. 
+with_dnwell: boolean parameter specifying to use deep nwell if True. You should usually set this to False unless the designer specifies otherwise.
+rmult: make metal connections within the nmos component wider. Specify this as 1 unless the designer asks to make routing wider or use wider metals.
+
+The main nmos ports correspond to source, gate, and drain nodes. Each underscore in a port name represents a level of hierarchy. For example, we start with the ComponentRef which is the name of the nmos Component instance. Then we specify one of the nodes from drain, gate, or source. Lastly we specify a direction indicator from N, E, S, W. The following are just some examples of the valid nmos ports:
+ComponentRef_source_N
+ComponentRef_drain_W
+ComponentRef_source_E
+ComponentRef_gate_S
+
+### PMOS
+Pmos is a p-type mosfet transistor. It is also referred to as pmos, pfet or p-type. It has the following parameters which are configurable when you place the component: 
+length: a float parameter specifying the transistor length
+width: a float parameter specifying the width of a single transistor
+fingers: an integer parameter which multiplies the width. For example, if fingers is 3, then the size will be 3 times the width.
+multipliers: An integer parameter specifying how many rows of fingers to place. Each row is equivalent to width*fingers in size, so that the total size is multipliers*width*fingers. Default is 1.
+with_tie: True or False, specifies if a bulk tie is required. Set this true unless the designer specifies otherwise.
+with_substrate_tap: True or False. If True, then add a substrate tap on the very outside perimeter of nmos. Set this to False unless the designer specifies otherwise.
+with_dummy: When True, specifies dummy devices should be added to the edges of the transistor. You should set this to True unless the designer specifies otherwise. 
+dnwell: Note that this is different from the nmos “width_dnwell” argument, but it serves a similar purpose. When dnwell is set to True it adds a deep nwell to the pmos transistor. You should set this to False unless the designer specifies otherwise. The designer may say they want triple well isolation, in which case you should set this as True.
+rmult: make metal connections within the pmos component wider. Specify this as 1 unless the designer asks to make routing wider or use wider metals.
+
+Here are just some examples of the valid pmos ports:
+ComponentRef_gate_S 
+ComponentRef_source_E
+ComponentRef_drain_W
+
+### MIMCAP
+The mimcap is a capacitor. The mimcap takes only one argument which can be configured when the component is placed:
+size: a tuple of floating point numbers like (2.1, 3.7) denoting the x and y dimension of the capacitor. The default size is (5.0, 5.0)
+
+The mimcap has the following 4 ports:
+ComponentRef_top_met_N
+ComponentRef_top_met_E
+ComponentRef_top_met_S
+ComponentRef_top_met_W
+
+### MIMCAP Array
+There is also a mimcap_array (also written as mimcap array) which automatically places and routes several mimcaps together. The mimcap_array takes the following parameters:
+size: a tuple of floating point numbers denoting the x and y dimension of the capacitor.
+columns: the number of columns in the array
+rows: the number of rows in the array
+
+
+### Differential Pair
+A differential pair is available, which is referred to as diff_pair or diff pair. The diff_pair is a differential pair Component which is created using 2 nfet Components. The nfet Components are referred to as “A” and “B” respectively. The diff pair has the following configurable parameters:
+length: a float parameter specifying the length of all transistor Components part of the diff pair.
+width: a float parameter specifying the width of all transistor Components part of the diff pair.
+fingers: an integer parameter which modifies the number of fingers in all transistor Components which are part of the diff pair.
+
+The following are just some examples of the valid ports for diff_pair:
+ComponentRef_A_source_S
+ComponentRef_A_drain_N
+ComponentRef_B_source_S
+ComponentRef_A_gate_E
+ComponentRef_B_drain_W
+ComponentRef_B_gate_E
+
+## Strict Syntax Commands
+Strict syntax supports the commands listed below. Note I have left square brackets [] around places where specific command calls should fill in information.
+### Import Command
+Sometimes you want to use Components which are not included in the Glayout runtime. You do this using the import command. The import command automatically searches for the Component path, so you do not need to specify a path. All you need is to specify the Component you want. The general syntax for importing a Component is:
+import [Component]
+For example, to import a CrossCoupledInvereters, the user could do the following:
+import CrossCoupledInverters
+### Create Parameters Command
+You generally want to make the Components as parameterized as possible so that they are highly modular and customizable. To do this you need to create parameters. You can create parameters with the following general command syntax:
+create a [Type] parameter called [ParameterName]
+Here are some examples using the create parameter command:
+create a float parameter called device_width 
+create a int parameter called device_fingers
+### Place Command
+The general syntax for the place command is below. I have left square brackets around names of Components or ComponentRefs or parameters that should be inserted when using the command. When you insert parameters, you can specify them as a comma separated list.
+place a [Component] called [ComponentRef] with [parameters]
+An example of using the place command is as follows:
+place a nmos called m1 with width 1.0, length 2.0, fingers 2, rmult 1, multipliers 3, with_substrate_tap False, with_tie True, with_dummy True, with_dnwell False
+The parameter list also supports passing existing parameter names instead of values.
+### Move Command
+By default all placed Components are centered at the origin. Obviously, if we place more than one ComponentRef we need to move some of them so that they are not overlapping. To emphasize, if more than one ComponentRef is placed, at least one ComponentRef must be moved to avoid overlapping. To do this, use the move command. The move command allows you to specify relative movements relative to other placed ComponentRefs.
+The general relative move syntax is as follows:
+move [ComponentRef we are moving] [relative direction] [relative to ComponentRef]
+Directions include above, below, right, or left.
+Here is an example of using relative move (say we have a ComponentRef called m1 and another called m2):
+move m1 below m2
+### Route Command
+Routes are connections between 2 Ports. There are 4 types of routes: straight_route, c_route, L_route, and smart_route. Unless you are very confident, always use smart_route. Only under special circumstances you can specifcy a different route type, but in almost all cases smart_route is the best option. smart_route can almost always optimally route between two ports. There are also some rules you can use to determine the Port orientations. If you are routing between ComponentRefs which are left or right of each other, then select Ports which are on the adjacent sides. If you are routing between ComponentRefs above or below each other, then select Ports that are both on the East side or both on the West side. The general route syntax is as follows:
+route between [Port1] and [Port2] using [route_type]
+For example, if we have a nmos ComponentRef called m1 which is to the west of a pmos ComponentRef called m2, an example route command to connect the sources of both would be as follows:
+route between m1_source_E and m2_source_W using smart_route
+Note that the first part of the portname is the ComponentRef name. Also, notice why the E and W ports were chosen. The nmos ComponentRef called m1 is to the left of the pmos ComponentRef called m2, so the sides adjacent to each other are the east side of m1 and west side of m2. If m1 was above m2, then I could have selected both East Ports or both West Ports as follows:
+route between m1_source_E and m2_source_E using smart_route
+or
+route between m1_source_W and m2_source_W using smart_route
+
+## Non-Standard Components Which can be Imported
+### CrossCoupledInverters
+CrossCoupledInverters is available to use and can be imported with:
+import CrossCoupledInverters
+The cell is made up of 4 transistor Components. The top two transistors are pfets and the bottom two transistors are nfets. 
+This cell implements the following prepackage circuit for easy import:
+CrossCoupledInverters includes two inverters. Inverters are composed of an nfet and pfet with their gates shorted with each other (the input of an inverter) and their drains shorted with each other (the output of an inverter). The inputs of the inverters are also shorted, with the sources of the nfets shorted with each other and the drains of the pfets shorted with each other. Importing the cell allows for it to be placed without any extra work. The CrossCoupledInverters has the following parameters:
+pfet_width: A float parameter specifying the width of the pmos Components
+nfet_width: A float parameter specifying the width of the nmos Components
+length: A float parameter specifying the length of all transistor Components
+numfingers: An int parameter specifying the number of fingers in all transistor Components
+
+The west (or left) inverter generally has the following port naming conventions:
+ComponentRef_top,bottom_A_source,drain,gate_N,E,S,W
+The west (or right) inverter generally has the following port naming conventions:
+ComponentRef_top,bottom_B_source,drain,gate_N,E,S,W
+Where top refers to the inverter’s pmos Component and bottom refers to the inverters nmos Component. A or B refers to the inverter, with A representing the west inverter and B representing the east inverter.
+
+## StrictSyntax Style Guide
+You should always follow this order of commands when creating a Component with strictsyntax: Start by importing any required Components, then create any required parameters, then place all required ComponentRefs with their respective parameters, then move all ComponentRefs to their final positions relative to one another, and lastly route between ComponentRefs.
```

### Comparing `glayout-0.0.3/setup.py` & `glayout-0.0.4/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,50 @@
-from setuptools import find_packages
-from setuptools import setup
-
-
-with open("glayout/README.md") as f:
-    LONG_DESCRIPTION = f.read()
-
-
-def get_install_requires():
-    with open("glayout/requirements.txt", "r") as f:
-        return [line.strip() for line in f.readlines() if not line.startswith("-")]
+from setuptools import setup, find_packages
 
 
 setup(
-    name="glayout",
-    version="0.0.3",
-    url="https://github.com/idea-fasoc/OpenFASOC",
-    license="MIT",
-    author=" msaligane",
-    author_email="mehdi@umich.edu",
-    description="Fully Open-Source Autonomous SoC Synthesis using Customizable Cell-Based Synthesizable Analog Circuits",
-    long_description=LONG_DESCRIPTION,
-    long_description_content_type="text/markdown",
-    packages=find_packages(exclude=("tests",)),
-    package_dir={"":"./"},
-    package_data={'glayout' :[]},
-    include_package_data=True,
-    install_requires=get_install_requires(),
-    python_requires=">=3.10",
+    name='glayout',
+    version='0.0.4',
+    author='Ali Hammoud, Harsh Khandeparkar, Vijay Shankar, Chetanya Goyal, Sakib Pathen, Arlene Dai, Ryan Wans, Mehdi Saligane',
+    author_email='alibilal@umich.edu, Harsh, vijayshankar.renganathan@analog.com, Chetanya, spathen@umich.edu, arlendai@umich.edu, Ryan, mehdi@umich.edu',
+    description='A human language to analog layout API with support for different technologies.',
+    long_description=open('README.md').read(),
+    long_description_content_type='text/markdown',
+    url='https://github.com/idea-fasoc/OpenFASOC/tree/main/openfasoc/generators/glayout',
+    packages=find_packages(),
     classifiers=[
-        "Development Status :: 2 - Pre-Alpha",
-        "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python",
-        "Programming Language :: Python :: 3.10",
+        'Programming Language :: Python :: 3.10',
+        'License :: OSI Approved :: MIT License',
+        'Operating System :: OS Independent',
+    ],
+    python_requires='>=3.10',
+    install_requires=[
+        "gdsfactory==7.7.0",
+        "prettyprint",
+        "prettyprinttree",
+        "nltk",
+        "torch",
+        "transformers",
+        "langchain",
+        "langchain_community",
+        "chromadb",
+        "ollama",
+        "unstructured",
+        "unstructured[md]",
+        "sentence-transformers",
+        "peft",
+        "accelerate",
+        "bitsandbytes",
+        "safetensors",
+        "requests",
+        "datasets",
+        "auto-gptq",
+        "optimum",
+        "trl",
+        "flash-attn"
     ],
+    entry_points={
+        'console_scripts': [
+            #"glayout = something:run"# Define any command line scripts here
+        ],
+    },
 )
```

