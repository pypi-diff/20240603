# Comparing `tmp/voxylstats-1.0.0.tar.gz` & `tmp/voxylstats-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voxylstats-1.0.0.tar", last modified: Mon Jun  3 03:49:11 2024, max compression
+gzip compressed data, was "voxylstats-1.0.1.tar", last modified: Mon Jun  3 03:59:27 2024, max compression
```

## Comparing `voxylstats-1.0.0.tar` & `voxylstats-1.0.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-06-03 03:49:11.204909 voxylstats-1.0.0/
--rw-rw-rw-   0        0        0     1087 2022-03-13 03:26:53.000000 voxylstats-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      513 2024-06-03 03:49:11.203909 voxylstats-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      330 2024-06-03 03:43:19.000000 voxylstats-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2024-06-03 03:49:11.205909 voxylstats-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      379 2024-06-03 03:45:19.000000 voxylstats-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-06-03 03:49:11.110908 voxylstats-1.0.0/voxyl/
--rw-rw-rw-   0        0        0      276 2024-06-02 23:06:11.000000 voxylstats-1.0.0/voxyl/__init__.py
--rw-rw-rw-   0        0        0    14754 2024-06-03 03:35:43.000000 voxylstats-1.0.0/voxyl/client.py
--rw-rw-rw-   0        0        0     6377 2024-06-03 03:02:06.000000 voxylstats-1.0.0/voxyl/constants.py
--rw-rw-rw-   0        0        0     2110 2024-06-03 03:39:26.000000 voxylstats-1.0.0/voxyl/errors.py
-drwxrwxrwx   0        0        0        0 2024-06-03 03:49:11.127910 voxylstats-1.0.0/voxyl/models/
--rw-rw-rw-   0        0        0      122 2024-06-02 23:39:56.000000 voxylstats-1.0.0/voxyl/models/__init__.py
--rw-rw-rw-   0        0        0      460 2024-06-02 23:54:27.000000 voxylstats-1.0.0/voxyl/models/achievements.py
-drwxrwxrwx   0        0        0        0 2024-06-03 03:49:11.191910 voxylstats-1.0.0/voxyl/models/games/
--rw-rw-rw-   0        0        0      658 2024-06-02 01:02:55.000000 voxylstats-1.0.0/voxyl/models/games/__init__.py
--rw-rw-rw-   0        0        0      529 2024-06-03 02:30:24.000000 voxylstats-1.0.0/voxyl/models/games/bed_rush.py
--rw-rw-rw-   0        0        0      186 2024-06-02 01:03:11.000000 voxylstats-1.0.0/voxyl/models/games/bedwalls.py
--rw-rw-rw-   0        0        0      723 2024-06-03 02:31:24.000000 voxylstats-1.0.0/voxyl/models/games/bedwars_late.py
--rw-rw-rw-   0        0        0      721 2024-06-03 02:31:24.000000 voxylstats-1.0.0/voxyl/models/games/bedwars_mega.py
--rw-rw-rw-   0        0        0      737 2024-06-03 02:31:24.000000 voxylstats-1.0.0/voxyl/models/games/bedwars_normal.py
--rw-rw-rw-   0        0        0      721 2024-06-03 02:31:24.000000 voxylstats-1.0.0/voxyl/models/games/bedwars_rush.py
--rw-rw-rw-   0        0        0      539 2024-06-03 02:30:58.000000 voxylstats-1.0.0/voxyl/models/games/bow_fight.py
--rw-rw-rw-   0        0        0      919 2024-06-03 02:31:24.000000 voxylstats-1.0.0/voxyl/models/games/bridge_fight.py
--rw-rw-rw-   0        0        0      347 2024-06-01 22:59:15.000000 voxylstats-1.0.0/voxyl/models/games/default_game_structure.py
--rw-rw-rw-   0        0        0      547 2024-06-03 02:30:58.000000 voxylstats-1.0.0/voxyl/models/games/flat_fight.py
--rw-rw-rw-   0        0        0      196 2024-06-02 01:03:11.000000 voxylstats-1.0.0/voxyl/models/games/four_way_bridges.py
--rw-rw-rw-   0        0        0      721 2024-06-03 02:31:24.000000 voxylstats-1.0.0/voxyl/models/games/ground_fight.py
--rw-rw-rw-   0        0        0      721 2024-06-03 02:31:24.000000 voxylstats-1.0.0/voxyl/models/games/ladder_fight.py
--rw-rw-rw-   0        0        0      697 2024-06-03 02:31:24.000000 voxylstats-1.0.0/voxyl/models/games/mini_wars.py
--rw-rw-rw-   0        0        0      123 2024-06-02 01:03:11.000000 voxylstats-1.0.0/voxyl/models/games/obstacles.py
--rw-rw-rw-   0        0        0      124 2024-06-02 01:03:11.000000 voxylstats-1.0.0/voxyl/models/games/party_games.py
--rw-rw-rw-   0        0        0      553 2024-06-03 02:30:58.000000 voxylstats-1.0.0/voxyl/models/games/pearl_fight.py
--rw-rw-rw-   0        0        0      208 2024-06-02 01:03:11.000000 voxylstats-1.0.0/voxyl/models/games/ranked_fours_practice.py
--rw-rw-rw-   0        0        0      593 2024-06-03 02:30:58.000000 voxylstats-1.0.0/voxyl/models/games/resource_collect.py
--rw-rw-rw-   0        0        0      617 2024-06-03 02:30:58.000000 voxylstats-1.0.0/voxyl/models/games/resource_old_collect.py
--rw-rw-rw-   0        0        0      553 2024-06-03 02:30:58.000000 voxylstats-1.0.0/voxyl/models/games/stick_fight.py
--rw-rw-rw-   0        0        0      517 2024-06-03 02:30:58.000000 voxylstats-1.0.0/voxyl/models/games/sumo.py
--rw-rw-rw-   0        0        0      547 2024-06-03 02:30:58.000000 voxylstats-1.0.0/voxyl/models/games/sumo_duels.py
--rw-rw-rw-   0        0        0      705 2024-06-03 02:31:24.000000 voxylstats-1.0.0/voxyl/models/games/void_fight.py
--rw-rw-rw-   0        0        0     3504 2024-06-03 03:39:52.000000 voxylstats-1.0.0/voxyl/models/guild.py
--rw-rw-rw-   0        0        0     1882 2024-06-03 01:56:26.000000 voxylstats-1.0.0/voxyl/models/leaderboard.py
--rw-rw-rw-   0        0        0     9246 2024-06-03 02:18:25.000000 voxylstats-1.0.0/voxyl/models/player.py
--rw-rw-rw-   0        0        0    10778 2024-06-03 02:29:30.000000 voxylstats-1.0.0/voxyl/models/utils.py
-drwxrwxrwx   0        0        0        0 2024-06-03 03:49:11.200945 voxylstats-1.0.0/voxylstats.egg-info/
--rw-rw-rw-   0        0        0      513 2024-06-03 03:49:10.000000 voxylstats-1.0.0/voxylstats.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1254 2024-06-03 03:49:11.000000 voxylstats-1.0.0/voxylstats.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-03 03:49:10.000000 voxylstats-1.0.0/voxylstats.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-06-03 03:49:10.000000 voxylstats-1.0.0/voxylstats.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-03 03:59:27.245829 voxylstats-1.0.1/
+-rw-rw-rw-   0        0        0     1087 2022-03-13 03:26:53.000000 voxylstats-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      517 2024-06-03 03:59:27.244858 voxylstats-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      334 2024-06-03 03:58:42.000000 voxylstats-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-06-03 03:59:27.245829 voxylstats-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      379 2024-06-03 03:59:23.000000 voxylstats-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 03:59:27.150830 voxylstats-1.0.1/voxyl/
+-rw-rw-rw-   0        0        0      276 2024-06-02 23:06:11.000000 voxylstats-1.0.1/voxyl/__init__.py
+-rw-rw-rw-   0        0        0    14754 2024-06-03 03:49:52.000000 voxylstats-1.0.1/voxyl/client.py
+-rw-rw-rw-   0        0        0     6377 2024-06-03 03:02:06.000000 voxylstats-1.0.1/voxyl/constants.py
+-rw-rw-rw-   0        0        0     2110 2024-06-03 03:39:26.000000 voxylstats-1.0.1/voxyl/errors.py
+drwxrwxrwx   0        0        0        0 2024-06-03 03:59:27.167868 voxylstats-1.0.1/voxyl/models/
+-rw-rw-rw-   0        0        0      122 2024-06-02 23:39:56.000000 voxylstats-1.0.1/voxyl/models/__init__.py
+-rw-rw-rw-   0        0        0      460 2024-06-02 23:54:27.000000 voxylstats-1.0.1/voxyl/models/achievements.py
+drwxrwxrwx   0        0        0        0 2024-06-03 03:59:27.230857 voxylstats-1.0.1/voxyl/models/games/
+-rw-rw-rw-   0        0        0      658 2024-06-02 01:02:55.000000 voxylstats-1.0.1/voxyl/models/games/__init__.py
+-rw-rw-rw-   0        0        0      529 2024-06-03 02:30:24.000000 voxylstats-1.0.1/voxyl/models/games/bed_rush.py
+-rw-rw-rw-   0        0        0      186 2024-06-02 01:03:11.000000 voxylstats-1.0.1/voxyl/models/games/bedwalls.py
+-rw-rw-rw-   0        0        0      723 2024-06-03 02:31:24.000000 voxylstats-1.0.1/voxyl/models/games/bedwars_late.py
+-rw-rw-rw-   0        0        0      721 2024-06-03 02:31:24.000000 voxylstats-1.0.1/voxyl/models/games/bedwars_mega.py
+-rw-rw-rw-   0        0        0      737 2024-06-03 02:31:24.000000 voxylstats-1.0.1/voxyl/models/games/bedwars_normal.py
+-rw-rw-rw-   0        0        0      721 2024-06-03 02:31:24.000000 voxylstats-1.0.1/voxyl/models/games/bedwars_rush.py
+-rw-rw-rw-   0        0        0      539 2024-06-03 02:30:58.000000 voxylstats-1.0.1/voxyl/models/games/bow_fight.py
+-rw-rw-rw-   0        0        0      919 2024-06-03 02:31:24.000000 voxylstats-1.0.1/voxyl/models/games/bridge_fight.py
+-rw-rw-rw-   0        0        0      347 2024-06-01 22:59:15.000000 voxylstats-1.0.1/voxyl/models/games/default_game_structure.py
+-rw-rw-rw-   0        0        0      547 2024-06-03 02:30:58.000000 voxylstats-1.0.1/voxyl/models/games/flat_fight.py
+-rw-rw-rw-   0        0        0      196 2024-06-02 01:03:11.000000 voxylstats-1.0.1/voxyl/models/games/four_way_bridges.py
+-rw-rw-rw-   0        0        0      721 2024-06-03 02:31:24.000000 voxylstats-1.0.1/voxyl/models/games/ground_fight.py
+-rw-rw-rw-   0        0        0      721 2024-06-03 02:31:24.000000 voxylstats-1.0.1/voxyl/models/games/ladder_fight.py
+-rw-rw-rw-   0        0        0      697 2024-06-03 02:31:24.000000 voxylstats-1.0.1/voxyl/models/games/mini_wars.py
+-rw-rw-rw-   0        0        0      123 2024-06-02 01:03:11.000000 voxylstats-1.0.1/voxyl/models/games/obstacles.py
+-rw-rw-rw-   0        0        0      124 2024-06-02 01:03:11.000000 voxylstats-1.0.1/voxyl/models/games/party_games.py
+-rw-rw-rw-   0        0        0      553 2024-06-03 02:30:58.000000 voxylstats-1.0.1/voxyl/models/games/pearl_fight.py
+-rw-rw-rw-   0        0        0      208 2024-06-02 01:03:11.000000 voxylstats-1.0.1/voxyl/models/games/ranked_fours_practice.py
+-rw-rw-rw-   0        0        0      593 2024-06-03 02:30:58.000000 voxylstats-1.0.1/voxyl/models/games/resource_collect.py
+-rw-rw-rw-   0        0        0      617 2024-06-03 02:30:58.000000 voxylstats-1.0.1/voxyl/models/games/resource_old_collect.py
+-rw-rw-rw-   0        0        0      553 2024-06-03 02:30:58.000000 voxylstats-1.0.1/voxyl/models/games/stick_fight.py
+-rw-rw-rw-   0        0        0      517 2024-06-03 02:30:58.000000 voxylstats-1.0.1/voxyl/models/games/sumo.py
+-rw-rw-rw-   0        0        0      547 2024-06-03 02:30:58.000000 voxylstats-1.0.1/voxyl/models/games/sumo_duels.py
+-rw-rw-rw-   0        0        0      705 2024-06-03 02:31:24.000000 voxylstats-1.0.1/voxyl/models/games/void_fight.py
+-rw-rw-rw-   0        0        0     3504 2024-06-03 03:39:52.000000 voxylstats-1.0.1/voxyl/models/guild.py
+-rw-rw-rw-   0        0        0     1882 2024-06-03 01:56:26.000000 voxylstats-1.0.1/voxyl/models/leaderboard.py
+-rw-rw-rw-   0        0        0     9246 2024-06-03 02:18:25.000000 voxylstats-1.0.1/voxyl/models/player.py
+-rw-rw-rw-   0        0        0    10778 2024-06-03 02:29:30.000000 voxylstats-1.0.1/voxyl/models/utils.py
+drwxrwxrwx   0        0        0        0 2024-06-03 03:59:27.241863 voxylstats-1.0.1/voxylstats.egg-info/
+-rw-rw-rw-   0        0        0      517 2024-06-03 03:59:26.000000 voxylstats-1.0.1/voxylstats.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1254 2024-06-03 03:59:27.000000 voxylstats-1.0.1/voxylstats.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 03:59:26.000000 voxylstats-1.0.1/voxylstats.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-06-03 03:59:26.000000 voxylstats-1.0.1/voxylstats.egg-info/top_level.txt
```

### Comparing `voxylstats-1.0.0/LICENSE` & `voxylstats-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `voxylstats-1.0.0/PKG-INFO` & `voxylstats-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: voxylstats
-Version: 1.0.0
+Version: 1.0.1
 Summary: A simple python wrapper for the Voxyl API
 Author: _lightninq & firestarad
 License: MIT
 License-File: LICENSE
 
 # Python-API-Wrapper
 
 This is a simple api wrapper written in python for the Minecraft Server, bedwarspractice.club. It is part of the Voxyl Network.
-This wrapper provides access to all data in the Voxyl API. If there is an error, please contact [FirestarAD](mailto:contact.firestarad@gmail.com?subject=[Voxyl API Wrapper] Bug)
+This wrapper provides access to all data in the Voxyl API. If there is an error, please contact [FirestarAD](mailto:contact.firestarad@gmail.com?subject=Voxyl%20API%20Wrapper%20Bug)
```

### Comparing `voxylstats-1.0.0/voxyl/client.py` & `voxylstats-1.0.1/voxyl/client.py`

 * *Files identical despite different names*

### Comparing `voxylstats-1.0.0/voxyl/constants.py` & `voxylstats-1.0.1/voxyl/constants.py`

 * *Files identical despite different names*

### Comparing `voxylstats-1.0.0/voxyl/errors.py` & `voxylstats-1.0.1/voxyl/errors.py`

 * *Files identical despite different names*

### Comparing `voxylstats-1.0.0/voxyl/models/games/__init__.py` & `voxylstats-1.0.1/voxyl/models/games/__init__.py`

 * *Files identical despite different names*

### Comparing `voxylstats-1.0.0/voxyl/models/games/bed_rush.py` & `voxylstats-1.0.1/voxyl/models/games/bed_rush.py`

 * *Files identical despite different names*

### Comparing `voxylstats-1.0.0/voxyl/models/games/bedwars_late.py` & `voxylstats-1.0.1/voxyl/models/games/bedwars_late.py`

 * *Files identical despite different names*

### Comparing `voxylstats-1.0.0/voxyl/models/games/bedwars_mega.py` & `voxylstats-1.0.1/voxyl/models/games/bedwars_mega.py`

 * *Files identical despite different names*

### Comparing `voxylstats-1.0.0/voxyl/models/games/bedwars_normal.py` & `voxylstats-1.0.1/voxyl/models/games/bedwars_normal.py`

 * *Files identical despite different names*

### Comparing `voxylstats-1.0.0/voxyl/models/games/bedwars_rush.py` & `voxylstats-1.0.1/voxyl/models/games/bedwars_rush.py`

 * *Files identical despite different names*

### Comparing `voxylstats-1.0.0/voxyl/models/games/bow_fight.py` & `voxylstats-1.0.1/voxyl/models/games/bow_fight.py`

 * *Files identical despite different names*

### Comparing `voxylstats-1.0.0/voxyl/models/games/bridge_fight.py` & `voxylstats-1.0.1/voxyl/models/games/bridge_fight.py`

 * *Files identical despite different names*

### Comparing `voxylstats-1.0.0/voxyl/models/games/flat_fight.py` & `voxylstats-1.0.1/voxyl/models/games/flat_fight.py`

 * *Files identical despite different names*

### Comparing `voxylstats-1.0.0/voxyl/models/games/ground_fight.py` & `voxylstats-1.0.1/voxyl/models/games/ground_fight.py`

 * *Files identical despite different names*

### Comparing `voxylstats-1.0.0/voxyl/models/games/ladder_fight.py` & `voxylstats-1.0.1/voxyl/models/games/ladder_fight.py`

 * *Files identical despite different names*

### Comparing `voxylstats-1.0.0/voxyl/models/games/mini_wars.py` & `voxylstats-1.0.1/voxyl/models/games/mini_wars.py`

 * *Files identical despite different names*

### Comparing `voxylstats-1.0.0/voxyl/models/games/pearl_fight.py` & `voxylstats-1.0.1/voxyl/models/games/pearl_fight.py`

 * *Files identical despite different names*

### Comparing `voxylstats-1.0.0/voxyl/models/games/resource_collect.py` & `voxylstats-1.0.1/voxyl/models/games/resource_collect.py`

 * *Files identical despite different names*

### Comparing `voxylstats-1.0.0/voxyl/models/games/resource_old_collect.py` & `voxylstats-1.0.1/voxyl/models/games/resource_old_collect.py`

 * *Files identical despite different names*

### Comparing `voxylstats-1.0.0/voxyl/models/games/stick_fight.py` & `voxylstats-1.0.1/voxyl/models/games/stick_fight.py`

 * *Files identical despite different names*

### Comparing `voxylstats-1.0.0/voxyl/models/games/sumo.py` & `voxylstats-1.0.1/voxyl/models/games/sumo.py`

 * *Files identical despite different names*

### Comparing `voxylstats-1.0.0/voxyl/models/games/sumo_duels.py` & `voxylstats-1.0.1/voxyl/models/games/sumo_duels.py`

 * *Files identical despite different names*

### Comparing `voxylstats-1.0.0/voxyl/models/games/void_fight.py` & `voxylstats-1.0.1/voxyl/models/games/void_fight.py`

 * *Files identical despite different names*

### Comparing `voxylstats-1.0.0/voxyl/models/guild.py` & `voxylstats-1.0.1/voxyl/models/guild.py`

 * *Files identical despite different names*

### Comparing `voxylstats-1.0.0/voxyl/models/leaderboard.py` & `voxylstats-1.0.1/voxyl/models/leaderboard.py`

 * *Files identical despite different names*

### Comparing `voxylstats-1.0.0/voxyl/models/player.py` & `voxylstats-1.0.1/voxyl/models/player.py`

 * *Files identical despite different names*

### Comparing `voxylstats-1.0.0/voxyl/models/utils.py` & `voxylstats-1.0.1/voxyl/models/utils.py`

 * *Files identical despite different names*

### Comparing `voxylstats-1.0.0/voxylstats.egg-info/PKG-INFO` & `voxylstats-1.0.1/voxylstats.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: voxylstats
-Version: 1.0.0
+Version: 1.0.1
 Summary: A simple python wrapper for the Voxyl API
 Author: _lightninq & firestarad
 License: MIT
 License-File: LICENSE
 
 # Python-API-Wrapper
 
 This is a simple api wrapper written in python for the Minecraft Server, bedwarspractice.club. It is part of the Voxyl Network.
-This wrapper provides access to all data in the Voxyl API. If there is an error, please contact [FirestarAD](mailto:contact.firestarad@gmail.com?subject=[Voxyl API Wrapper] Bug)
+This wrapper provides access to all data in the Voxyl API. If there is an error, please contact [FirestarAD](mailto:contact.firestarad@gmail.com?subject=Voxyl%20API%20Wrapper%20Bug)
```

### Comparing `voxylstats-1.0.0/voxylstats.egg-info/SOURCES.txt` & `voxylstats-1.0.1/voxylstats.egg-info/SOURCES.txt`

 * *Files identical despite different names*

