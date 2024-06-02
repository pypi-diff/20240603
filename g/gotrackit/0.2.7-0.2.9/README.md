# Comparing `tmp/gotrackit-0.2.7.tar.gz` & `tmp/gotrackit-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gotrackit-0.2.7.tar", last modified: Sun May 19 15:34:59 2024, max compression
+gzip compressed data, was "gotrackit-0.2.9.tar", last modified: Sun Jun  2 10:37:25 2024, max compression
```

## Comparing `gotrackit-0.2.7.tar` & `gotrackit-0.2.9.tar`

### file list

```diff
@@ -1,115 +1,116 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 15:34:59.460935 gotrackit-0.2.7/
--rw-rw-rw-   0        0        0     1085 2024-01-01 15:23:01.000000 gotrackit-0.2.7/LICENSE
--rw-rw-rw-   0        0        0     7732 2024-05-19 15:34:59.460935 gotrackit-0.2.7/PKG-INFO
--rw-rw-rw-   0        0        0     6986 2024-05-19 15:33:57.000000 gotrackit-0.2.7/README.md
--rw-rw-rw-   0        0        0      795 2024-05-19 15:34:20.000000 gotrackit-0.2.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-19 15:34:59.460935 gotrackit-0.2.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-19 15:34:59.388550 gotrackit-0.2.7/src/
--rw-rw-rw-   0        0        0      101 2023-12-09 00:21:11.000000 gotrackit-0.2.7/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-19 15:34:59.392539 gotrackit-0.2.7/src/gotrackit/
--rw-rw-rw-   0        0        0    16111 2024-05-19 14:54:43.000000 gotrackit-0.2.7/src/gotrackit/GlobalVal.py
--rw-rw-rw-   0        0        0    17442 2024-05-19 09:31:55.000000 gotrackit-0.2.7/src/gotrackit/MapMatch.py
--rw-rw-rw-   0        0        0      624 2024-05-18 04:36:05.000000 gotrackit-0.2.7/src/gotrackit/WrapsFunc.py
--rw-rw-rw-   0        0        0      102 2024-01-18 03:53:10.000000 gotrackit-0.2.7/src/gotrackit/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-19 15:34:59.396579 gotrackit-0.2.7/src/gotrackit/generation/
--rw-rw-rw-   0        0        0    25084 2024-03-27 15:57:38.000000 gotrackit-0.2.7/src/gotrackit/generation/GpsGen.py
--rw-rw-rw-   0        0        0      103 2023-12-30 07:52:41.000000 gotrackit-0.2.7/src/gotrackit/generation/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-19 15:34:59.400579 gotrackit-0.2.7/src/gotrackit/gps/
--rw-rw-rw-   0        0        0     4241 2024-05-19 13:01:14.000000 gotrackit-0.2.7/src/gotrackit/gps/GpsArray.py
--rw-rw-rw-   0        0        0     8021 2024-05-19 13:01:14.000000 gotrackit-0.2.7/src/gotrackit/gps/GpsTrip.py
--rw-rw-rw-   0        0        0     3896 2024-04-30 05:17:12.000000 gotrackit-0.2.7/src/gotrackit/gps/GpsXfer.py
--rw-rw-rw-   0        0        0    21654 2024-05-19 13:34:52.000000 gotrackit-0.2.7/src/gotrackit/gps/LocGps.py
--rw-rw-rw-   0        0        0      103 2023-12-31 04:37:58.000000 gotrackit-0.2.7/src/gotrackit/gps/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-19 15:34:59.404579 gotrackit-0.2.7/src/gotrackit/map/
--rw-rw-rw-   0        0        0    20406 2024-05-17 07:59:43.000000 gotrackit-0.2.7/src/gotrackit/map/Link.py
--rw-rw-rw-   0        0        0    40402 2024-05-17 08:31:42.000000 gotrackit-0.2.7/src/gotrackit/map/Net.py
--rw-rw-rw-   0        0        0     4848 2024-05-18 04:12:21.000000 gotrackit-0.2.7/src/gotrackit/map/Node.py
--rw-rw-rw-   0        0        0      103 2023-12-31 04:37:58.000000 gotrackit-0.2.7/src/gotrackit/map/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-19 15:34:59.408579 gotrackit-0.2.7/src/gotrackit/model/
--rw-rw-rw-   0        0        0    59726 2024-05-19 15:28:00.000000 gotrackit-0.2.7/src/gotrackit/model/Markov.py
--rw-rw-rw-   0        0        0     2441 2024-05-19 15:08:25.000000 gotrackit-0.2.7/src/gotrackit/model/Para.py
--rw-rw-rw-   0        0        0      103 2023-12-31 04:37:58.000000 gotrackit-0.2.7/src/gotrackit/model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-19 15:34:59.412592 gotrackit-0.2.7/src/gotrackit/netreverse/
--rw-rw-rw-   0        0        0     1657 2024-01-31 02:46:45.000000 gotrackit-0.2.7/src/gotrackit/netreverse/GlobalVal.py
--rw-rw-rw-   0        0        0    27460 2024-05-08 15:05:30.000000 gotrackit-0.2.7/src/gotrackit/netreverse/NetGen.py
-drwxrwxrwx   0        0        0        0 2024-05-19 15:34:59.412592 gotrackit-0.2.7/src/gotrackit/netreverse/Parse/
--rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.7/src/gotrackit/netreverse/Parse/__init__.py
--rw-rw-rw-   0        0        0    19151 2024-04-10 05:04:41.000000 gotrackit-0.2.7/src/gotrackit/netreverse/Parse/gd_car_path.py
-drwxrwxrwx   0        0        0        0 2024-05-19 15:34:59.416579 gotrackit-0.2.7/src/gotrackit/netreverse/PublicTools/
--rw-rw-rw-   0        0        0     3697 2024-01-27 14:10:52.000000 gotrackit-0.2.7/src/gotrackit/netreverse/PublicTools/GeoProcess.py
--rw-rw-rw-   0        0        0     1024 2023-12-16 09:25:56.000000 gotrackit-0.2.7/src/gotrackit/netreverse/PublicTools/GraphAna.py
--rw-rw-rw-   0        0        0     1649 2024-01-28 14:46:20.000000 gotrackit-0.2.7/src/gotrackit/netreverse/PublicTools/IndexAna.py
--rw-rw-rw-   0        0        0      221 2024-01-28 14:46:20.000000 gotrackit-0.2.7/src/gotrackit/netreverse/PublicTools/MapProcess.py
--rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.7/src/gotrackit/netreverse/PublicTools/__init__.py
--rw-rw-rw-   0        0        0     4362 2024-03-07 05:54:15.000000 gotrackit-0.2.7/src/gotrackit/netreverse/PublicTools/od.py
-drwxrwxrwx   0        0        0        0 2024-05-19 15:34:59.420579 gotrackit-0.2.7/src/gotrackit/netreverse/Request/
--rw-rw-rw-   0        0        0        0 2023-12-12 03:03:06.000000 gotrackit-0.2.7/src/gotrackit/netreverse/Request/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-19 15:34:59.420579 gotrackit-0.2.7/src/gotrackit/netreverse/Request/api/
--rw-rw-rw-   0        0        0     3812 2024-01-29 14:05:19.000000 gotrackit-0.2.7/src/gotrackit/netreverse/Request/api/WebApi.py
--rw-rw-rw-   0        0        0      103 2023-12-12 04:05:25.000000 gotrackit-0.2.7/src/gotrackit/netreverse/Request/api/__init__.py
--rw-rw-rw-   0        0        0     3093 2024-01-29 11:43:10.000000 gotrackit-0.2.7/src/gotrackit/netreverse/Request/request_path.py
-drwxrwxrwx   0        0        0        0 2024-05-19 15:34:59.424579 gotrackit-0.2.7/src/gotrackit/netreverse/Request/usage/
--rw-rw-rw-   0        0        0      103 2023-12-12 04:10:22.000000 gotrackit-0.2.7/src/gotrackit/netreverse/Request/usage/__init__.py
--rw-rw-rw-   0        0        0     7809 2024-01-28 14:46:20.000000 gotrackit-0.2.7/src/gotrackit/netreverse/Request/usage/bd_ts.py
--rw-rw-rw-   0        0        0    11231 2024-01-31 07:13:59.000000 gotrackit-0.2.7/src/gotrackit/netreverse/Request/usage/gd_car_path.py
-drwxrwxrwx   0        0        0        0 2024-05-19 15:34:59.428906 gotrackit-0.2.7/src/gotrackit/netreverse/RoadNet/
-drwxrwxrwx   0        0        0        0 2024-05-19 15:34:59.432936 gotrackit-0.2.7/src/gotrackit/netreverse/RoadNet/DupProcess/
--rw-rw-rw-   0        0        0    21741 2024-05-08 08:28:07.000000 gotrackit-0.2.7/src/gotrackit/netreverse/RoadNet/DupProcess/DupLinks.py
--rw-rw-rw-   0        0        0      134 2023-12-16 09:25:56.000000 gotrackit-0.2.7/src/gotrackit/netreverse/RoadNet/DupProcess/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-19 15:34:59.432936 gotrackit-0.2.7/src/gotrackit/netreverse/RoadNet/Merge/
--rw-rw-rw-   0        0        0      103 2023-12-18 12:14:41.000000 gotrackit-0.2.7/src/gotrackit/netreverse/RoadNet/Merge/__init__.py
--rw-rw-rw-   0        0        0     6874 2024-01-27 07:40:20.000000 gotrackit-0.2.7/src/gotrackit/netreverse/RoadNet/Merge/get_merged_link_seq.py
-drwxrwxrwx   0        0        0        0 2024-05-19 15:34:59.436953 gotrackit-0.2.7/src/gotrackit/netreverse/RoadNet/Merge/limit/
--rw-rw-rw-   0        0        0      134 2023-12-16 09:25:56.000000 gotrackit-0.2.7/src/gotrackit/netreverse/RoadNet/Merge/limit/__init__.py
--rw-rw-rw-   0        0        0    18675 2024-01-27 07:25:52.000000 gotrackit-0.2.7/src/gotrackit/netreverse/RoadNet/Merge/limit/attr_limit.py
--rw-rw-rw-   0        0        0    11592 2024-01-31 01:26:21.000000 gotrackit-0.2.7/src/gotrackit/netreverse/RoadNet/Merge/limit/direction_limit.py
--rw-rw-rw-   0        0        0     2865 2024-01-27 07:40:20.000000 gotrackit-0.2.7/src/gotrackit/netreverse/RoadNet/Merge/limit/same_head_tail_limit.py
--rw-rw-rw-   0        0        0     9459 2024-01-27 07:40:20.000000 gotrackit-0.2.7/src/gotrackit/netreverse/RoadNet/Merge/limit/two_degrees_group.py
--rw-rw-rw-   0        0        0    12237 2024-05-08 09:22:18.000000 gotrackit-0.2.7/src/gotrackit/netreverse/RoadNet/Merge/merge_links.py
--rw-rw-rw-   0        0        0    15086 2024-01-27 08:21:05.000000 gotrackit-0.2.7/src/gotrackit/netreverse/RoadNet/Merge/merge_short.py
-drwxrwxrwx   0        0        0        0 2024-05-19 15:34:59.440938 gotrackit-0.2.7/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/
--rw-rw-rw-   0        0        0      102 2024-03-17 11:27:43.000000 gotrackit-0.2.7/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-19 15:34:59.444931 gotrackit-0.2.7/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/
--rw-rw-rw-   0        0        0      134 2023-12-16 09:25:56.000000 gotrackit-0.2.7/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/__init__.py
--rw-rw-rw-   0        0        0    18675 2024-01-27 07:25:52.000000 gotrackit-0.2.7/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/attr_limit.py
--rw-rw-rw-   0        0        0    11592 2024-01-31 01:26:21.000000 gotrackit-0.2.7/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/direction_limit.py
--rw-rw-rw-   0        0        0     2865 2024-01-27 07:40:20.000000 gotrackit-0.2.7/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/same_head_tail_limit.py
--rw-rw-rw-   0        0        0     8948 2024-04-08 05:51:27.000000 gotrackit-0.2.7/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/two_degrees_group.py
--rw-rw-rw-   0        0        0    21567 2024-05-08 09:34:18.000000 gotrackit-0.2.7/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/merge_links_multi.py
-drwxrwxrwx   0        0        0        0 2024-05-19 15:34:59.448936 gotrackit-0.2.7/src/gotrackit/netreverse/RoadNet/SaveStreets/
--rw-rw-rw-   0        0        0      134 2023-12-16 09:25:56.000000 gotrackit-0.2.7/src/gotrackit/netreverse/RoadNet/SaveStreets/__init__.py
--rw-rw-rw-   0        0        0    22373 2024-05-18 04:15:30.000000 gotrackit-0.2.7/src/gotrackit/netreverse/RoadNet/SaveStreets/streets.py
-drwxrwxrwx   0        0        0        0 2024-05-19 15:34:59.448936 gotrackit-0.2.7/src/gotrackit/netreverse/RoadNet/Split/
--rw-rw-rw-   0        0        0     4266 2024-01-29 13:44:04.000000 gotrackit-0.2.7/src/gotrackit/netreverse/RoadNet/Split/SplitPath.py
--rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.7/src/gotrackit/netreverse/RoadNet/Split/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-19 15:34:59.452935 gotrackit-0.2.7/src/gotrackit/netreverse/RoadNet/Tools/
--rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.7/src/gotrackit/netreverse/RoadNet/Tools/__init__.py
--rw-rw-rw-   0        0        0     5745 2024-04-08 08:18:36.000000 gotrackit-0.2.7/src/gotrackit/netreverse/RoadNet/Tools/process.py
--rw-rw-rw-   0        0        0      133 2023-12-16 09:25:56.000000 gotrackit-0.2.7/src/gotrackit/netreverse/RoadNet/__init__.py
--rw-rw-rw-   0        0        0     9629 2024-05-10 08:28:49.000000 gotrackit-0.2.7/src/gotrackit/netreverse/RoadNet/conn.py
--rw-rw-rw-   0        0        0    18855 2024-03-09 13:07:40.000000 gotrackit-0.2.7/src/gotrackit/netreverse/RoadNet/increment.py
--rw-rw-rw-   0        0        0     9043 2024-04-08 07:19:18.000000 gotrackit-0.2.7/src/gotrackit/netreverse/RoadNet/net_reverse.py
--rw-rw-rw-   0        0        0     5790 2024-05-08 09:34:18.000000 gotrackit-0.2.7/src/gotrackit/netreverse/RoadNet/optimize_net.py
--rw-rw-rw-   0        0        0     1188 2024-03-05 08:17:38.000000 gotrackit-0.2.7/src/gotrackit/netreverse/RoadNet/save_file.py
--rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.7/src/gotrackit/netreverse/__init__.py
--rw-rw-rw-   0        0        0     2654 2024-01-29 14:01:55.000000 gotrackit-0.2.7/src/gotrackit/netreverse/book_mark.py
--rw-rw-rw-   0        0        0     1872 2024-05-08 09:34:18.000000 gotrackit-0.2.7/src/gotrackit/netreverse/format_od.py
-drwxrwxrwx   0        0        0        0 2024-05-19 15:34:59.452935 gotrackit-0.2.7/src/gotrackit/netxfer/
--rw-rw-rw-   0        0        0    17197 2024-04-16 10:06:45.000000 gotrackit-0.2.7/src/gotrackit/netxfer/SumoConvert.py
--rw-rw-rw-   0        0        0      101 2024-03-30 00:52:12.000000 gotrackit-0.2.7/src/gotrackit/netxfer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-19 15:34:59.452935 gotrackit-0.2.7/src/gotrackit/solver/
--rw-rw-rw-   0        0        0     9156 2024-05-07 23:25:32.000000 gotrackit-0.2.7/src/gotrackit/solver/Viterbi.py
--rw-rw-rw-   0        0        0      103 2023-12-31 04:37:58.000000 gotrackit-0.2.7/src/gotrackit/solver/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-19 15:34:59.456936 gotrackit-0.2.7/src/gotrackit/tools/
--rw-rw-rw-   0        0        0      102 2024-01-10 02:23:14.000000 gotrackit-0.2.7/src/gotrackit/tools/__init__.py
--rw-rw-rw-   0        0        0    10646 2024-03-05 06:26:07.000000 gotrackit-0.2.7/src/gotrackit/tools/coord_trans.py
--rw-rw-rw-   0        0        0    12569 2024-05-17 05:28:38.000000 gotrackit-0.2.7/src/gotrackit/tools/geo_process.py
--rw-rw-rw-   0        0        0      812 2024-04-12 02:40:08.000000 gotrackit-0.2.7/src/gotrackit/tools/group.py
--rw-rw-rw-   0        0        0     1121 2024-01-31 04:02:14.000000 gotrackit-0.2.7/src/gotrackit/tools/save_file.py
--rw-rw-rw-   0        0        0    10550 2024-05-07 01:39:06.000000 gotrackit-0.2.7/src/gotrackit/visualization.py
-drwxrwxrwx   0        0        0        0 2024-05-19 15:34:59.460935 gotrackit-0.2.7/src/gotrackit.egg-info/
--rw-rw-rw-   0        0        0     7732 2024-05-19 15:34:59.000000 gotrackit-0.2.7/src/gotrackit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3723 2024-05-19 15:34:59.000000 gotrackit-0.2.7/src/gotrackit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 15:34:59.000000 gotrackit-0.2.7/src/gotrackit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-05-19 15:34:59.000000 gotrackit-0.2.7/src/gotrackit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-05-19 15:34:59.000000 gotrackit-0.2.7/src/gotrackit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-02 10:37:25.299133 gotrackit-0.2.9/
+-rw-rw-rw-   0        0        0     1085 2024-01-01 15:23:01.000000 gotrackit-0.2.9/LICENSE
+-rw-rw-rw-   0        0        0     7110 2024-06-02 10:37:25.299133 gotrackit-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     6364 2024-05-31 23:01:01.000000 gotrackit-0.2.9/README.md
+-rw-rw-rw-   0        0        0      795 2024-06-02 10:35:33.000000 gotrackit-0.2.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-06-02 10:37:25.299133 gotrackit-0.2.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-06-02 10:37:25.212759 gotrackit-0.2.9/src/
+-rw-rw-rw-   0        0        0      101 2023-12-09 00:21:11.000000 gotrackit-0.2.9/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-02 10:37:25.221566 gotrackit-0.2.9/src/gotrackit/
+-rw-rw-rw-   0        0        0    16692 2024-05-30 03:58:49.000000 gotrackit-0.2.9/src/gotrackit/GlobalVal.py
+-rw-rw-rw-   0        0        0    17442 2024-05-19 09:31:55.000000 gotrackit-0.2.9/src/gotrackit/MapMatch.py
+-rw-rw-rw-   0        0        0      624 2024-05-18 04:36:05.000000 gotrackit-0.2.9/src/gotrackit/WrapsFunc.py
+-rw-rw-rw-   0        0        0      102 2024-01-18 03:53:10.000000 gotrackit-0.2.9/src/gotrackit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-02 10:37:25.225569 gotrackit-0.2.9/src/gotrackit/generation/
+-rw-rw-rw-   0        0        0    25674 2024-05-26 12:23:18.000000 gotrackit-0.2.9/src/gotrackit/generation/GpsGen.py
+-rw-rw-rw-   0        0        0     4868 2024-06-02 10:21:36.000000 gotrackit-0.2.9/src/gotrackit/generation/SampleTrip.py
+-rw-rw-rw-   0        0        0      103 2023-12-30 07:52:41.000000 gotrackit-0.2.9/src/gotrackit/generation/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-02 10:37:25.233569 gotrackit-0.2.9/src/gotrackit/gps/
+-rw-rw-rw-   0        0        0     4419 2024-05-30 07:06:46.000000 gotrackit-0.2.9/src/gotrackit/gps/GpsArray.py
+-rw-rw-rw-   0        0        0    18921 2024-05-31 01:41:59.000000 gotrackit-0.2.9/src/gotrackit/gps/GpsTrip.py
+-rw-rw-rw-   0        0        0     3896 2024-04-30 05:17:12.000000 gotrackit-0.2.9/src/gotrackit/gps/GpsXfer.py
+-rw-rw-rw-   0        0        0    21654 2024-05-19 13:34:52.000000 gotrackit-0.2.9/src/gotrackit/gps/LocGps.py
+-rw-rw-rw-   0        0        0      103 2023-12-31 04:37:58.000000 gotrackit-0.2.9/src/gotrackit/gps/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-02 10:37:25.235386 gotrackit-0.2.9/src/gotrackit/map/
+-rw-rw-rw-   0        0        0    20406 2024-05-17 07:59:43.000000 gotrackit-0.2.9/src/gotrackit/map/Link.py
+-rw-rw-rw-   0        0        0    40844 2024-06-02 10:28:10.000000 gotrackit-0.2.9/src/gotrackit/map/Net.py
+-rw-rw-rw-   0        0        0     4848 2024-05-18 04:12:21.000000 gotrackit-0.2.9/src/gotrackit/map/Node.py
+-rw-rw-rw-   0        0        0      103 2023-12-31 04:37:58.000000 gotrackit-0.2.9/src/gotrackit/map/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-02 10:37:25.239390 gotrackit-0.2.9/src/gotrackit/model/
+-rw-rw-rw-   0        0        0    59713 2024-05-30 23:51:42.000000 gotrackit-0.2.9/src/gotrackit/model/Markov.py
+-rw-rw-rw-   0        0        0     2441 2024-05-19 15:08:25.000000 gotrackit-0.2.9/src/gotrackit/model/Para.py
+-rw-rw-rw-   0        0        0      103 2023-12-31 04:37:58.000000 gotrackit-0.2.9/src/gotrackit/model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-02 10:37:25.243389 gotrackit-0.2.9/src/gotrackit/netreverse/
+-rw-rw-rw-   0        0        0     1657 2024-01-31 02:46:45.000000 gotrackit-0.2.9/src/gotrackit/netreverse/GlobalVal.py
+-rw-rw-rw-   0        0        0    26548 2024-05-31 03:22:07.000000 gotrackit-0.2.9/src/gotrackit/netreverse/NetGen.py
+drwxrwxrwx   0        0        0        0 2024-06-02 10:37:25.247416 gotrackit-0.2.9/src/gotrackit/netreverse/Parse/
+-rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.9/src/gotrackit/netreverse/Parse/__init__.py
+-rw-rw-rw-   0        0        0    19151 2024-04-10 05:04:41.000000 gotrackit-0.2.9/src/gotrackit/netreverse/Parse/gd_car_path.py
+drwxrwxrwx   0        0        0        0 2024-06-02 10:37:25.251389 gotrackit-0.2.9/src/gotrackit/netreverse/PublicTools/
+-rw-rw-rw-   0        0        0     3697 2024-01-27 14:10:52.000000 gotrackit-0.2.9/src/gotrackit/netreverse/PublicTools/GeoProcess.py
+-rw-rw-rw-   0        0        0     1024 2023-12-16 09:25:56.000000 gotrackit-0.2.9/src/gotrackit/netreverse/PublicTools/GraphAna.py
+-rw-rw-rw-   0        0        0     1649 2024-01-28 14:46:20.000000 gotrackit-0.2.9/src/gotrackit/netreverse/PublicTools/IndexAna.py
+-rw-rw-rw-   0        0        0      221 2024-01-28 14:46:20.000000 gotrackit-0.2.9/src/gotrackit/netreverse/PublicTools/MapProcess.py
+-rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.9/src/gotrackit/netreverse/PublicTools/__init__.py
+-rw-rw-rw-   0        0        0     4362 2024-03-07 05:54:15.000000 gotrackit-0.2.9/src/gotrackit/netreverse/PublicTools/od.py
+drwxrwxrwx   0        0        0        0 2024-06-02 10:37:25.255390 gotrackit-0.2.9/src/gotrackit/netreverse/Request/
+-rw-rw-rw-   0        0        0        0 2023-12-12 03:03:06.000000 gotrackit-0.2.9/src/gotrackit/netreverse/Request/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-02 10:37:25.255390 gotrackit-0.2.9/src/gotrackit/netreverse/Request/api/
+-rw-rw-rw-   0        0        0     3697 2024-05-31 08:43:21.000000 gotrackit-0.2.9/src/gotrackit/netreverse/Request/api/WebApi.py
+-rw-rw-rw-   0        0        0      103 2023-12-12 04:05:25.000000 gotrackit-0.2.9/src/gotrackit/netreverse/Request/api/__init__.py
+-rw-rw-rw-   0        0        0     3240 2024-05-31 07:35:06.000000 gotrackit-0.2.9/src/gotrackit/netreverse/Request/request_path.py
+drwxrwxrwx   0        0        0        0 2024-06-02 10:37:25.259389 gotrackit-0.2.9/src/gotrackit/netreverse/Request/usage/
+-rw-rw-rw-   0        0        0      103 2023-12-12 04:10:22.000000 gotrackit-0.2.9/src/gotrackit/netreverse/Request/usage/__init__.py
+-rw-rw-rw-   0        0        0     7809 2024-01-28 14:46:20.000000 gotrackit-0.2.9/src/gotrackit/netreverse/Request/usage/bd_ts.py
+-rw-rw-rw-   0        0        0    11937 2024-06-01 13:04:54.000000 gotrackit-0.2.9/src/gotrackit/netreverse/Request/usage/gd_car_path.py
+drwxrwxrwx   0        0        0        0 2024-06-02 10:37:25.263389 gotrackit-0.2.9/src/gotrackit/netreverse/RoadNet/
+drwxrwxrwx   0        0        0        0 2024-06-02 10:37:25.267389 gotrackit-0.2.9/src/gotrackit/netreverse/RoadNet/DupProcess/
+-rw-rw-rw-   0        0        0    21741 2024-05-31 04:43:13.000000 gotrackit-0.2.9/src/gotrackit/netreverse/RoadNet/DupProcess/DupLinks.py
+-rw-rw-rw-   0        0        0      134 2023-12-16 09:25:56.000000 gotrackit-0.2.9/src/gotrackit/netreverse/RoadNet/DupProcess/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-02 10:37:25.271389 gotrackit-0.2.9/src/gotrackit/netreverse/RoadNet/Merge/
+-rw-rw-rw-   0        0        0      103 2023-12-18 12:14:41.000000 gotrackit-0.2.9/src/gotrackit/netreverse/RoadNet/Merge/__init__.py
+-rw-rw-rw-   0        0        0     6874 2024-01-27 07:40:20.000000 gotrackit-0.2.9/src/gotrackit/netreverse/RoadNet/Merge/get_merged_link_seq.py
+drwxrwxrwx   0        0        0        0 2024-06-02 10:37:25.275390 gotrackit-0.2.9/src/gotrackit/netreverse/RoadNet/Merge/limit/
+-rw-rw-rw-   0        0        0      134 2023-12-16 09:25:56.000000 gotrackit-0.2.9/src/gotrackit/netreverse/RoadNet/Merge/limit/__init__.py
+-rw-rw-rw-   0        0        0    18675 2024-01-27 07:25:52.000000 gotrackit-0.2.9/src/gotrackit/netreverse/RoadNet/Merge/limit/attr_limit.py
+-rw-rw-rw-   0        0        0    11592 2024-01-31 01:26:21.000000 gotrackit-0.2.9/src/gotrackit/netreverse/RoadNet/Merge/limit/direction_limit.py
+-rw-rw-rw-   0        0        0     2865 2024-01-27 07:40:20.000000 gotrackit-0.2.9/src/gotrackit/netreverse/RoadNet/Merge/limit/same_head_tail_limit.py
+-rw-rw-rw-   0        0        0     9459 2024-01-27 07:40:20.000000 gotrackit-0.2.9/src/gotrackit/netreverse/RoadNet/Merge/limit/two_degrees_group.py
+-rw-rw-rw-   0        0        0    12745 2024-05-31 14:54:02.000000 gotrackit-0.2.9/src/gotrackit/netreverse/RoadNet/Merge/merge_links.py
+-rw-rw-rw-   0        0        0    15086 2024-01-27 08:21:05.000000 gotrackit-0.2.9/src/gotrackit/netreverse/RoadNet/Merge/merge_short.py
+drwxrwxrwx   0        0        0        0 2024-06-02 10:37:25.279389 gotrackit-0.2.9/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/
+-rw-rw-rw-   0        0        0      102 2024-03-17 11:27:43.000000 gotrackit-0.2.9/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-02 10:37:25.284923 gotrackit-0.2.9/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/
+-rw-rw-rw-   0        0        0      134 2023-12-16 09:25:56.000000 gotrackit-0.2.9/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/__init__.py
+-rw-rw-rw-   0        0        0    18675 2024-01-27 07:25:52.000000 gotrackit-0.2.9/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/attr_limit.py
+-rw-rw-rw-   0        0        0    11592 2024-01-31 01:26:21.000000 gotrackit-0.2.9/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/direction_limit.py
+-rw-rw-rw-   0        0        0     2865 2024-01-27 07:40:20.000000 gotrackit-0.2.9/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/same_head_tail_limit.py
+-rw-rw-rw-   0        0        0     8948 2024-04-08 05:51:27.000000 gotrackit-0.2.9/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/two_degrees_group.py
+-rw-rw-rw-   0        0        0    22077 2024-06-02 10:32:57.000000 gotrackit-0.2.9/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/merge_links_multi.py
+drwxrwxrwx   0        0        0        0 2024-06-02 10:37:25.284923 gotrackit-0.2.9/src/gotrackit/netreverse/RoadNet/SaveStreets/
+-rw-rw-rw-   0        0        0      134 2023-12-16 09:25:56.000000 gotrackit-0.2.9/src/gotrackit/netreverse/RoadNet/SaveStreets/__init__.py
+-rw-rw-rw-   0        0        0    22514 2024-05-31 14:54:02.000000 gotrackit-0.2.9/src/gotrackit/netreverse/RoadNet/SaveStreets/streets.py
+drwxrwxrwx   0        0        0        0 2024-06-02 10:37:25.288925 gotrackit-0.2.9/src/gotrackit/netreverse/RoadNet/Split/
+-rw-rw-rw-   0        0        0     4266 2024-01-29 13:44:04.000000 gotrackit-0.2.9/src/gotrackit/netreverse/RoadNet/Split/SplitPath.py
+-rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.9/src/gotrackit/netreverse/RoadNet/Split/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-02 10:37:25.288925 gotrackit-0.2.9/src/gotrackit/netreverse/RoadNet/Tools/
+-rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.9/src/gotrackit/netreverse/RoadNet/Tools/__init__.py
+-rw-rw-rw-   0        0        0     5745 2024-04-08 08:18:36.000000 gotrackit-0.2.9/src/gotrackit/netreverse/RoadNet/Tools/process.py
+-rw-rw-rw-   0        0        0      133 2023-12-16 09:25:56.000000 gotrackit-0.2.9/src/gotrackit/netreverse/RoadNet/__init__.py
+-rw-rw-rw-   0        0        0     9697 2024-06-01 13:18:44.000000 gotrackit-0.2.9/src/gotrackit/netreverse/RoadNet/conn.py
+-rw-rw-rw-   0        0        0    18855 2024-03-09 13:07:40.000000 gotrackit-0.2.9/src/gotrackit/netreverse/RoadNet/increment.py
+-rw-rw-rw-   0        0        0     9315 2024-06-02 09:53:53.000000 gotrackit-0.2.9/src/gotrackit/netreverse/RoadNet/net_reverse.py
+-rw-rw-rw-   0        0        0     5790 2024-05-08 09:34:18.000000 gotrackit-0.2.9/src/gotrackit/netreverse/RoadNet/optimize_net.py
+-rw-rw-rw-   0        0        0     1188 2024-03-05 08:17:38.000000 gotrackit-0.2.9/src/gotrackit/netreverse/RoadNet/save_file.py
+-rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.9/src/gotrackit/netreverse/__init__.py
+-rw-rw-rw-   0        0        0     2654 2024-01-29 14:01:55.000000 gotrackit-0.2.9/src/gotrackit/netreverse/book_mark.py
+-rw-rw-rw-   0        0        0     1872 2024-05-08 09:34:18.000000 gotrackit-0.2.9/src/gotrackit/netreverse/format_od.py
+drwxrwxrwx   0        0        0        0 2024-06-02 10:37:25.293658 gotrackit-0.2.9/src/gotrackit/netxfer/
+-rw-rw-rw-   0        0        0    17197 2024-04-16 10:06:45.000000 gotrackit-0.2.9/src/gotrackit/netxfer/SumoConvert.py
+-rw-rw-rw-   0        0        0      101 2024-03-30 00:52:12.000000 gotrackit-0.2.9/src/gotrackit/netxfer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-02 10:37:25.295131 gotrackit-0.2.9/src/gotrackit/solver/
+-rw-rw-rw-   0        0        0     9156 2024-05-07 23:25:32.000000 gotrackit-0.2.9/src/gotrackit/solver/Viterbi.py
+-rw-rw-rw-   0        0        0      103 2023-12-31 04:37:58.000000 gotrackit-0.2.9/src/gotrackit/solver/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-02 10:37:25.299133 gotrackit-0.2.9/src/gotrackit/tools/
+-rw-rw-rw-   0        0        0      102 2024-01-10 02:23:14.000000 gotrackit-0.2.9/src/gotrackit/tools/__init__.py
+-rw-rw-rw-   0        0        0    10646 2024-03-05 06:26:07.000000 gotrackit-0.2.9/src/gotrackit/tools/coord_trans.py
+-rw-rw-rw-   0        0        0    12802 2024-05-31 14:58:37.000000 gotrackit-0.2.9/src/gotrackit/tools/geo_process.py
+-rw-rw-rw-   0        0        0      812 2024-04-12 02:40:08.000000 gotrackit-0.2.9/src/gotrackit/tools/group.py
+-rw-rw-rw-   0        0        0     1121 2024-01-31 04:02:14.000000 gotrackit-0.2.9/src/gotrackit/tools/save_file.py
+-rw-rw-rw-   0        0        0    10550 2024-05-07 01:39:06.000000 gotrackit-0.2.9/src/gotrackit/visualization.py
+drwxrwxrwx   0        0        0        0 2024-06-02 10:37:25.299133 gotrackit-0.2.9/src/gotrackit.egg-info/
+-rw-rw-rw-   0        0        0     7110 2024-06-02 10:37:25.000000 gotrackit-0.2.9/src/gotrackit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3762 2024-06-02 10:37:25.000000 gotrackit-0.2.9/src/gotrackit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 10:37:25.000000 gotrackit-0.2.9/src/gotrackit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-06-02 10:37:25.000000 gotrackit-0.2.9/src/gotrackit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-06-02 10:37:25.000000 gotrackit-0.2.9/src/gotrackit.egg-info/top_level.txt
```

### Comparing `gotrackit-0.2.7/LICENSE` & `gotrackit-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.7/PKG-INFO` & `gotrackit-0.2.9/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gotrackit
-Version: 0.2.7
+Version: 0.2.9
 Summary: A Python Package for Map Matching Algorithm Based on Hidden Markov Model
 Author-email: Kai Tang <794568794@qq.com>
 License: LICENCE
 Project-URL: Homepage, https://github.com/zdsjjtTLG/TrackIt
 Keywords: HMM,MapMatching,Net,Link,Node,Hidden Markov Model,Algorithm
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -16,83 +16,70 @@
 Requires-Dist: shapely
 Requires-Dist: networkx
 Requires-Dist: pandas
 Requires-Dist: numpy
 Requires-Dist: keplergl
 Requires-Dist: geopy
 
-
+**Read this in other languages: [Chinese](README.md) or [English](README_EN.md).**
 
 <div align="center">
     <img src="docs/_static/images/gotrackit.png" />
 </div>
 
 <br>
 
 <div align=center>
 
 [![Documentation Status](https://readthedocs.org/projects/gotrackit/badge/?version=latest)](https://gotrackit.readthedocs.io/en/latest/?badge=latest)
 ![PyPI - Version](https://img.shields.io/pypi/v/gotrackit)
 ![GitHub License](https://img.shields.io/github/license/zdsjjtTLG/Trackit)
+[![Downloads](https://static.pepy.tech/badge/gotrackit)](https://pepy.tech/project/gotrackit)
 ![PyPI - Downloads](https://img.shields.io/pypi/dw/gotrackit)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/gotrackit)
+![Static Badge](https://img.shields.io/badge/Model-HMM-9EC231)
+![Static Badge](https://img.shields.io/badge/Optimization-FastMapMatching-blue)
+![Static Badge](https://img.shields.io/badge/Optimization-MultiCoreParallelism-9EC231)
+![Github Created At](https://img.shields.io/github/created-at/zdsjjtTLG/Trackit)
+![GitHub last commit](https://img.shields.io/github/last-commit/zdsjjtTLG/Trackit)
 
-~ 一个包搞定：路网获取、路网优化、宏微观地图匹配、匹配可视化、问题路段快速定位 ~
-
-Developed by Tang Kai, Email: 794568794@qq.com & tangkai@zhechengdata.com
-</div>
-<br>
-
-
-**版本状态：05.19已更新: v0.2.6**
-
-更新命令：pip install --upgrade  -i https://pypi.org/simple/ gotrackit
-
-- 地图匹配接口效率优化, 相较于v0.2.4小幅度提升
+![GitHub User's stars](https://img.shields.io/github/stars/zdsjjtTLG)
+![GitHub forks](https://img.shields.io/github/forks/zdsjjtTLG/Trackit)
 
-- 新增网格参数搜索，帮助用户确定合理的匹配参数
+~ 💪一个包搞定：路网获取、路网优化、宏微观地图匹配、匹配可视化、问题路段快速定位💪 ~
 
-- BUG修复
+👻Developed by Tang Kai, Email: 794568794@qq.com & tangkai@zhechengdata.com👻
 
+🔑gotrackit迭代更新很快，记得关注版本更新信息哦🔑
 
-**不要下载GitHub仓库上的代码来使用!!!  直接pip安装gotrackit为第三方库即可使用**
-
+**❗❗❗不要下载GitHub仓库上的代码来使用!!!  直接pip安装gotrackit为第三方库即可使用❗❗❗**
 
+😆😁👉[gotrackit用户手册](https://gotrackit.readthedocs.io/en/latest/)👈😝😉
+</div>
 <br>
 
-<div align=center>
-~ v0.2.7(相较于0.2.1)效率将大幅度提升, 最高可以提升20倍的性能 !~
-</div>
 
-<br>
+**💬版本状态：06.03即将更新: v0.2.8**
 
-与上一版本对比:
+更新命令：pip install --upgrade  -i https://pypi.org/simple/ gotrackit
 
-| 样例数据           | 有效的GPS点数 | top_k(k邻近候选参数) | gps_buffer(临域半径) | 候选路段条数 | 状态转移次数  | v0.2.1版解算时间 | v0.2.7版解算时间 |
-|----------------|----------|----------------|------------------|---------|------------|-------------|-------------|
-| 1辆车,深圳稀疏轨迹点样例1 | 190      | 60             | 500m             | 10615 | 629788次 | 28秒         | **1.35秒**   |
-| 1辆车,深圳稀疏轨迹点样例2 | 400      | 20             | 120m             | 5137 | 82006次  | 7.8秒        | **0.60秒**   |
+- 样例GPS生成模块：接口简化、BUG修复
 
+- 基于GPS生产OD的接口：效率优化
 
-v0.2.7多核效率对比:
+- 上线GPS行程切分接口
 
-基于上表深圳稀疏轨迹点样例2，我们将他复制150份，进行多核测试，可以看到到6核时, 效率已经不再提升，最快71s解算完150条轨迹，平均每条轨迹0.47s，相较于0.60s再次提升了20%，在车辆数较多时，多核的效率提升很明显。
+- 路网请求模块，Key配额提示优化，动态停用已超配额的Key
 
-| 样例数据                                      | 有效的GPS点数 | top_k | gps_buffer | 候选路段条数 | 状态转移次数 | v0.2.7解算时间 |
-|-------------------------------------------|----------|----------------|------------------|-----|--------|------------|
-| 150辆车的GPS轨迹(单核串行,子图搜索,有构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 226.0秒     | 
-| 150辆车的GPS轨迹(3核并行,子图搜索,有构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 101.6秒     |
-| 150辆车的GPS轨迹(3核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 88.3秒      |
-| 150辆车的GPS轨迹(4核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 75.3秒      | 
-| 150辆车的GPS轨迹(5核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 72.1秒      | 
-| 150辆车的GPS轨迹(6核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 71.5秒      | 
+- 地图匹配接口BUG修复(极小概率BUG、但是影响较大)、路网生产模块BUG修复
 
 
 <br>
 
+
 <div align=center>
 ~ 稀疏轨迹匹配与路径补全 ~
 </div>
 
 <br>
 
 深圳稀疏轨迹点样例1：
@@ -143,28 +130,34 @@
     <img src="docs/_static/images/wxq.jpg" />
 </div>
 
 
 ## 1. 简介
 本地图匹配包基于隐马尔可夫模型(HMM)实现了连续GPS点位的概率建模，利用这个包可以轻松对GPS数据进行地图匹配，本开源包的特点如下:
 
-**数据无忧**
-- 提供路网生产模块以及路网优化接口，您不需要准备任何路网和GPS数据即可玩转地图匹配；
+**😻数据无忧**
+- 提供路网生产模块以及大量路网处理优化工具，您不需要准备任何路网和GPS数据即可玩转地图匹配；
 - 提供GPS样例数据生产模块，解决没有GPS数据的难题；
-- 提供GPS数据清洗接口，包括滑动窗口降噪、数据降频。
+- 提供GPS数据清洗接口，包括行程切分、滑动窗口降噪、数据降频、停留点识别、点位增密。
 
-**文档齐全**
 
+**☑️文档齐全**
 - 中文文档，有详细的操作指引；
 - 算法原理讲解部分不涉及复杂的公式推导，使用动画形式剖析算法原理,简洁明了。
 
-**匹配结果自动优化**
+
+**🚀匹配算法优化**
+- 支持基于路径预存储的FastMapMatching、支持多核并行匹配、支持网格参数搜索；
 - 对基于HMM匹配的初步路径进行了优化，对于不连通的位置会自动搜路补全，对于实际路网不连通的位置会输出警告信息，方便用户回溯问题。
 
 
+**🌈匹配结果支持动画可视化**
+- 匹配结果提供三种输出形式：GPS点匹配结果表(csv)、匹配结果矢量化图层、矢量图层匹配动画(HTML文件)，HTML动画方便用户直观地感受匹配结果，同时可以提高问题排查的效率。
+
+
 
 ### 1.1. 如何安装gotrackit
 
 #### __所需前置依赖__
 
 - geopy(2.4.1)
 - gdal(3.4.3)
@@ -188,25 +181,40 @@
 ```
 
 更新：
 ``` shell
 pip install --upgrade  -i https://pypi.org/simple/ gotrackit
 ```
 
-### 1.2 用户手册与视频教程
+### 1.2 如何使用gotrackit
+
+- [用户手册](https://gotrackit.readthedocs.io/en/latest/)
+
+- [基于隐马尔可夫模型(HMM)的地图匹配算法动画版！学不会你来打我！](https://www.bilibili.com/video/BV1gQ4y1w7dC)
 
-[用户手册](https://gotrackit.readthedocs.io/en/latest/)
+- [一个python包搞定路网获取+地图匹配！](https://www.bilibili.com/video/BV1nC411z7Vg)
 
-[基于隐马尔可夫模型(HMM)的地图匹配算法动画版！学不会你来打我！](https://www.bilibili.com/video/BV1gQ4y1w7dC)
+- [gotrackit地图匹配包参数详解与问题排查](https://www.bilibili.com/video/BV1qK421Y7hV)
+
+- [QGIS路网拓扑显示、底图加载、样式复用、map保存](https://www.bilibili.com/video/BV1Sq421F7QX)
+
+
+### 1.3. 如何引用gotrackit
+
+如果你想在文章中引用gotrackit，请附上以下链接：
+
+``` shell
+https://github.com/zdsjjtTLG/TrackIt
+```
 
-[一个python包搞定路网获取+地图匹配！](https://www.bilibili.com/video/BV1nC411z7Vg)
+### 1.4. BUG提交
 
-[gotrackit地图匹配包参数详解与问题排查](https://www.bilibili.com/video/BV1qK421Y7hV)
+如果确定是BUG，请提交在以下页面：
 
-[QGIS路网拓扑显示、底图加载、样式复用、map保存](https://www.bilibili.com/video/BV1Sq421F7QX)
+[BUG提交页面](https://github.com/zdsjjtTLG/TrackIt/issues)
 
 
 ## 2. 地图匹配问题
 
 ![car_gps.png](docs/_static/images/car_gps.png)
 
 ![where_car.png](docs/_static/images/whereIsCar.png)
```

### Comparing `gotrackit-0.2.7/README.md` & `gotrackit-0.2.9/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,76 +1,63 @@
-
+**Read this in other languages: [Chinese](README.md) or [English](README_EN.md).**
 
 <div align="center">
     <img src="docs/_static/images/gotrackit.png" />
 </div>
 
 <br>
 
 <div align=center>
 
 [![Documentation Status](https://readthedocs.org/projects/gotrackit/badge/?version=latest)](https://gotrackit.readthedocs.io/en/latest/?badge=latest)
 ![PyPI - Version](https://img.shields.io/pypi/v/gotrackit)
 ![GitHub License](https://img.shields.io/github/license/zdsjjtTLG/Trackit)
+[![Downloads](https://static.pepy.tech/badge/gotrackit)](https://pepy.tech/project/gotrackit)
 ![PyPI - Downloads](https://img.shields.io/pypi/dw/gotrackit)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/gotrackit)
+![Static Badge](https://img.shields.io/badge/Model-HMM-9EC231)
+![Static Badge](https://img.shields.io/badge/Optimization-FastMapMatching-blue)
+![Static Badge](https://img.shields.io/badge/Optimization-MultiCoreParallelism-9EC231)
+![Github Created At](https://img.shields.io/github/created-at/zdsjjtTLG/Trackit)
+![GitHub last commit](https://img.shields.io/github/last-commit/zdsjjtTLG/Trackit)
 
-~ 一个包搞定：路网获取、路网优化、宏微观地图匹配、匹配可视化、问题路段快速定位 ~
-
-Developed by Tang Kai, Email: 794568794@qq.com & tangkai@zhechengdata.com
-</div>
-<br>
-
-
-**版本状态：05.19已更新: v0.2.6**
-
-更新命令：pip install --upgrade  -i https://pypi.org/simple/ gotrackit
-
-- 地图匹配接口效率优化, 相较于v0.2.4小幅度提升
+![GitHub User's stars](https://img.shields.io/github/stars/zdsjjtTLG)
+![GitHub forks](https://img.shields.io/github/forks/zdsjjtTLG/Trackit)
 
-- 新增网格参数搜索，帮助用户确定合理的匹配参数
+~ 💪一个包搞定：路网获取、路网优化、宏微观地图匹配、匹配可视化、问题路段快速定位💪 ~
 
-- BUG修复
+👻Developed by Tang Kai, Email: 794568794@qq.com & tangkai@zhechengdata.com👻
 
+🔑gotrackit迭代更新很快，记得关注版本更新信息哦🔑
 
-**不要下载GitHub仓库上的代码来使用!!!  直接pip安装gotrackit为第三方库即可使用**
-
+**❗❗❗不要下载GitHub仓库上的代码来使用!!!  直接pip安装gotrackit为第三方库即可使用❗❗❗**
 
+😆😁👉[gotrackit用户手册](https://gotrackit.readthedocs.io/en/latest/)👈😝😉
+</div>
 <br>
 
-<div align=center>
-~ v0.2.7(相较于0.2.1)效率将大幅度提升, 最高可以提升20倍的性能 !~
-</div>
 
-<br>
+**💬版本状态：06.03即将更新: v0.2.8**
 
-与上一版本对比:
+更新命令：pip install --upgrade  -i https://pypi.org/simple/ gotrackit
 
-| 样例数据           | 有效的GPS点数 | top_k(k邻近候选参数) | gps_buffer(临域半径) | 候选路段条数 | 状态转移次数  | v0.2.1版解算时间 | v0.2.7版解算时间 |
-|----------------|----------|----------------|------------------|---------|------------|-------------|-------------|
-| 1辆车,深圳稀疏轨迹点样例1 | 190      | 60             | 500m             | 10615 | 629788次 | 28秒         | **1.35秒**   |
-| 1辆车,深圳稀疏轨迹点样例2 | 400      | 20             | 120m             | 5137 | 82006次  | 7.8秒        | **0.60秒**   |
+- 样例GPS生成模块：接口简化、BUG修复
 
+- 基于GPS生产OD的接口：效率优化
 
-v0.2.7多核效率对比:
+- 上线GPS行程切分接口
 
-基于上表深圳稀疏轨迹点样例2，我们将他复制150份，进行多核测试，可以看到到6核时, 效率已经不再提升，最快71s解算完150条轨迹，平均每条轨迹0.47s，相较于0.60s再次提升了20%，在车辆数较多时，多核的效率提升很明显。
+- 路网请求模块，Key配额提示优化，动态停用已超配额的Key
 
-| 样例数据                                      | 有效的GPS点数 | top_k | gps_buffer | 候选路段条数 | 状态转移次数 | v0.2.7解算时间 |
-|-------------------------------------------|----------|----------------|------------------|-----|--------|------------|
-| 150辆车的GPS轨迹(单核串行,子图搜索,有构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 226.0秒     | 
-| 150辆车的GPS轨迹(3核并行,子图搜索,有构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 101.6秒     |
-| 150辆车的GPS轨迹(3核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 88.3秒      |
-| 150辆车的GPS轨迹(4核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 75.3秒      | 
-| 150辆车的GPS轨迹(5核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 72.1秒      | 
-| 150辆车的GPS轨迹(6核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 71.5秒      | 
+- 地图匹配接口BUG修复(极小概率BUG、但是影响较大)、路网生产模块BUG修复
 
 
 <br>
 
+
 <div align=center>
 ~ 稀疏轨迹匹配与路径补全 ~
 </div>
 
 <br>
 
 深圳稀疏轨迹点样例1：
@@ -121,28 +108,34 @@
     <img src="docs/_static/images/wxq.jpg" />
 </div>
 
 
 ## 1. 简介
 本地图匹配包基于隐马尔可夫模型(HMM)实现了连续GPS点位的概率建模，利用这个包可以轻松对GPS数据进行地图匹配，本开源包的特点如下:
 
-**数据无忧**
-- 提供路网生产模块以及路网优化接口，您不需要准备任何路网和GPS数据即可玩转地图匹配；
+**😻数据无忧**
+- 提供路网生产模块以及大量路网处理优化工具，您不需要准备任何路网和GPS数据即可玩转地图匹配；
 - 提供GPS样例数据生产模块，解决没有GPS数据的难题；
-- 提供GPS数据清洗接口，包括滑动窗口降噪、数据降频。
+- 提供GPS数据清洗接口，包括行程切分、滑动窗口降噪、数据降频、停留点识别、点位增密。
 
-**文档齐全**
 
+**☑️文档齐全**
 - 中文文档，有详细的操作指引；
 - 算法原理讲解部分不涉及复杂的公式推导，使用动画形式剖析算法原理,简洁明了。
 
-**匹配结果自动优化**
+
+**🚀匹配算法优化**
+- 支持基于路径预存储的FastMapMatching、支持多核并行匹配、支持网格参数搜索；
 - 对基于HMM匹配的初步路径进行了优化，对于不连通的位置会自动搜路补全，对于实际路网不连通的位置会输出警告信息，方便用户回溯问题。
 
 
+**🌈匹配结果支持动画可视化**
+- 匹配结果提供三种输出形式：GPS点匹配结果表(csv)、匹配结果矢量化图层、矢量图层匹配动画(HTML文件)，HTML动画方便用户直观地感受匹配结果，同时可以提高问题排查的效率。
+
+
 
 ### 1.1. 如何安装gotrackit
 
 #### __所需前置依赖__
 
 - geopy(2.4.1)
 - gdal(3.4.3)
@@ -166,25 +159,40 @@
 ```
 
 更新：
 ``` shell
 pip install --upgrade  -i https://pypi.org/simple/ gotrackit
 ```
 
-### 1.2 用户手册与视频教程
+### 1.2 如何使用gotrackit
+
+- [用户手册](https://gotrackit.readthedocs.io/en/latest/)
+
+- [基于隐马尔可夫模型(HMM)的地图匹配算法动画版！学不会你来打我！](https://www.bilibili.com/video/BV1gQ4y1w7dC)
 
-[用户手册](https://gotrackit.readthedocs.io/en/latest/)
+- [一个python包搞定路网获取+地图匹配！](https://www.bilibili.com/video/BV1nC411z7Vg)
 
-[基于隐马尔可夫模型(HMM)的地图匹配算法动画版！学不会你来打我！](https://www.bilibili.com/video/BV1gQ4y1w7dC)
+- [gotrackit地图匹配包参数详解与问题排查](https://www.bilibili.com/video/BV1qK421Y7hV)
+
+- [QGIS路网拓扑显示、底图加载、样式复用、map保存](https://www.bilibili.com/video/BV1Sq421F7QX)
+
+
+### 1.3. 如何引用gotrackit
+
+如果你想在文章中引用gotrackit，请附上以下链接：
+
+``` shell
+https://github.com/zdsjjtTLG/TrackIt
+```
 
-[一个python包搞定路网获取+地图匹配！](https://www.bilibili.com/video/BV1nC411z7Vg)
+### 1.4. BUG提交
 
-[gotrackit地图匹配包参数详解与问题排查](https://www.bilibili.com/video/BV1qK421Y7hV)
+如果确定是BUG，请提交在以下页面：
 
-[QGIS路网拓扑显示、底图加载、样式复用、map保存](https://www.bilibili.com/video/BV1Sq421F7QX)
+[BUG提交页面](https://github.com/zdsjjtTLG/TrackIt/issues)
 
 
 ## 2. 地图匹配问题
 
 ![car_gps.png](docs/_static/images/car_gps.png)
 
 ![where_car.png](docs/_static/images/whereIsCar.png)
```

### Comparing `gotrackit-0.2.7/pyproject.toml` & `gotrackit-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gotrackit"
-version = "0.2.7"
+version = "0.2.9"
 dependencies = ["geopandas>=0.14.1", "shapely", "networkx", "pandas", "numpy", "keplergl", "geopy"]
 requires-python = ">=3.8"
 authors = [
   { name="Kai Tang", email="794568794@qq.com" },
 ]
 description = "A Python Package for Map Matching Algorithm Based on Hidden Markov Model"
 readme = "README.md"
```

### Comparing `gotrackit-0.2.7/src/gotrackit/GlobalVal.py` & `gotrackit-0.2.9/src/gotrackit/GlobalVal.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,40 +36,48 @@
         self.SUB_SEQ_FIELD = 'sub_seq'
         self.ORIGIN_POINT_SEQ_FIELD = 'origin_seq'
         self.TIME_FIELD = 'time'
         self.LNG_FIELD = 'lng'
         self.LAT_FIELD = 'lat'
         self.HEADING_FIELD = 'heading'
         self.AGENT_ID_FIELD = 'agent_id'
+        self.PRE_AGENT_ID_FIELD = 'pre_agent'
+        self.ORIGIN_AGENT_ID_FIELD = 'origin_agent_id'
         self.TYPE_FIELD = 'type'
         self.NEXT_LINK_FIELD = 'next_link'
         self.GEOMETRY_FIELD = 'geometry'
         self.FROM_GPS_SEQ = 'from_seq'
         self.TO_GPS_SEQ = 'to_seq'
 
         self.GROUP_FIELD = 'group'
         self.SUB_GROUP_FIELD = 'sub_group'
         self.NEXT_P = 'next_p'
         self.PRE_P = 'pre_p'
         self.NEXT_SEQ = 'next_seq'
         self.NEXT_TIME = 'next_time'
+        self.PRE_TIME = 'pre_time'
         self.ADJ_TIME_GAP = 'time_gap'
         self.ADJ_DIS = 'gps_adj_dis'
+        self.ADJ_X_DIS = 'gps_adj_xl'
+        self.ADJ_Y_DIS = 'gps_adj_yl'
         self.ADJ_SPEED = 'adj_speed'
 
         self.DENSE_GEO = '__dens_geo__'
         self.N_SEGMENTS = '__n__'
 
         self.X_DIFF = 'gv_dx'
         self.Y_DIFF = 'gv_dy'
         self.VEC_LEN = 'gvl'
 
         self.PLAIN_X = 'prj_x'
         self.PLAIN_Y = 'prj_y'
 
+        self.PRE_PLAIN_X = 'pre_prj_x'
+        self.PRE_PLAIN_Y = 'pre_prj_y'
+
 
 class RouteField(object):
     """"""
     def __init__(self):
         self.PATH_ID_FIELD = 'path_id'
         self.TIME_COST_FIELD = 'time_cost'
         self.SEQ_FIELD = 'seq'
@@ -93,14 +101,25 @@
         self.PRJ_GEO = 'prj_p'
         self.DIS_TO_NEXT = 'dis_to_next'
         self.HEADING_GAP = 'heading_gap'
         self.USED_HEADING_GAP = 'used_heading_gap'
         self.EMISSION_P = 'emission_p'
 
 
+class OdField(object):
+    """路网字段"""
+    def __init__(self):
+        self.OD_ID_FIELD = 'od_id'
+        self.WAYPOINTS_FIELD = 'way_points'
+        self.OX_FIELD = 'o_x'
+        self.OY_FIELD = 'o_y'
+        self.DX_FIELD = 'd_x'
+        self.DY_FIELD = 'd_y'
+
+
 class KeplerConfig(object):
     def __init__(self):
         self.__BASE_CONFIG = {
             'version': 'v1',
             'config': {
                 'visState': {
                     'filters': [
```

### Comparing `gotrackit-0.2.7/src/gotrackit/MapMatch.py` & `gotrackit-0.2.9/src/gotrackit/MapMatch.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.7/src/gotrackit/WrapsFunc.py` & `gotrackit-0.2.9/src/gotrackit/WrapsFunc.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.7/src/gotrackit/generation/GpsGen.py` & `gotrackit-0.2.9/src/gotrackit/generation/GpsGen.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,15 @@
         :param loc_error_sigma: gps定位误差参数, N(μ, σ2)中的σ
         """
         self.time_step = time_step
         self.loc_frequency = loc_frequency
         self.agent_id = agent_id
 
         self.tic_miu = 0
-        self.tic_sigma = loc_frequency * 0.1
+        self.tic_sigma = loc_frequency * 0.06
 
         self.loc_error_miu = loc_error_miu
         self.loc_error_sigma = loc_error_sigma
         self.heading_error_sigma = heading_error_sigma
         self.heading_error_miu = heading_error_miu
 
         # 用于记录定位数据的list
@@ -119,15 +119,15 @@
     def receive_car_loc(self, now_time: datetime.datetime = None, loc: tuple[float, float, float, int, int, int] = None) -> None:
         """
         接收车辆的定位信息, 依据定位频率判断是否记录定位信息
         :param now_time:
         :param loc:
         :return:
         """
-        if not self.__final_loc_gps or (now_time - self.__final_loc_gps[-1][0]).seconds > self.tic_gap:
+        if not self.__final_loc_gps or (now_time - self.__final_loc_gps[-1][0]).total_seconds() > self.tic_gap:
             loc_error = self.loc_error
             device_loc_x, device_loc_y, device_heading = \
                 loc[0] + loc_error[0], loc[1] + loc_error[1], loc[2] + loc_error[2]
             link, f, t = int(loc[3]), int(loc[4]), int(loc[5])
             self.__final_loc_gps.append((now_time, Point(device_loc_x, device_loc_y), round(device_heading, 2),
                                          self.agent_id, link, f, t))
             logging.info(
@@ -337,15 +337,15 @@
     def get_gps_loc_info(self) -> list[tuple[datetime.datetime, Point, float, str, int, int, int]]:
         return self.gps_device.get_gps_loc_info()
 
 
 class RouteInfoCollector(object):
     """真实路径坐标以及GPS坐标收集器"""
     def __init__(self, convert_prj_sys: bool = True, convert_type: str = 'bd-84',
-                 convert_loc: bool = False, from_crs: str = None, to_crs: str = None, crs: str = None):
+                 convert_loc: bool = False, from_crs: str = None, to_crs: str = None, crs: str = None) -> object:
         """
 
         :param convert_prj_sys: 是否转换坐标系(GCJ02、百度、84之间的转化)
         :param convert_type: 'gc-84', 'gc-bd'分别代表GCJ02转化为84, GCJ02转化为百度,
         :param from_crs: str
         :param to_crs: str
         :param crs: str
@@ -371,120 +371,130 @@
     def collect_trajectory(self, trajectory_info: list[tuple[datetime.datetime, Point, float, str]] = None):
         self.trajectory_info_list.extend(trajectory_info)
 
     @staticmethod
     @function_time_cost
     def format_gdf(convert_prj_sys:bool=False, from_crs: str = None, to_crs: str = None, crs: str = None, convert_loc: bool = False,
                    convert_type: str = 'bd-84',
-                   info_list: list = None, attr_name_field_list: list[str] = None) -> gpd.GeoDataFrame:
+                   info_list: list = None, attr_name_field_list: list[str] = None, time_format="%Y-%m-%d %H:%M:%S") -> gpd.GeoDataFrame:
 
         format_df = pd.DataFrame(info_list, columns=attr_name_field_list)
 
         if to_crs is not None:
             used_crs = from_crs
         else:
             used_crs = crs
             to_crs = crs
 
         format_gdf = gpd.GeoDataFrame(format_df, geometry=gps_field.GEOMETRY_FIELD, crs=used_crs)
         format_gdf = format_gdf.to_crs(to_crs)
         format_gdf[gps_field.TIME_FIELD] = format_gdf[gps_field.TIME_FIELD].apply(
-            lambda t: t.strftime("%Y-%m-%d %H:%M:%S"))
+            lambda t: t.strftime(time_format))
 
         if convert_loc:
             con = LngLatTransfer()
             format_gdf[gps_field.GEOMETRY_FIELD] = \
                 format_gdf[gps_field.GEOMETRY_FIELD].apply(
                     lambda geo: con.obj_convert(geo_obj=geo, con_type=convert_type))
         format_gdf[gps_field.LNG_FIELD] = format_gdf[gps_field.GEOMETRY_FIELD].apply(lambda geo: geo.x)
         format_gdf[gps_field.LAT_FIELD] = format_gdf[gps_field.GEOMETRY_FIELD].apply(lambda geo: geo.y)
 
         attr_name_field_list.remove(gps_field.GEOMETRY_FIELD)
         attr_name_field_list.extend([gps_field.LNG_FIELD, gps_field.LAT_FIELD, gps_field.GEOMETRY_FIELD])
         return format_gdf[attr_name_field_list]
 
     @function_time_cost
-    def save_trajectory(self, out_fldr: str = r'./', file_name: str = None, file_type: str = 'csv') -> gpd.GeoDataFrame:
+    def save_trajectory(self, out_fldr: str = r'./', file_name: str = None, file_type: str = 'csv',
+                        time_format="%Y-%m-%d %H:%M:%S") -> gpd.GeoDataFrame:
         """
         存储轨迹信息
         :param out_fldr:
         :param file_name:
         :param file_type:
+        :param time_format:
         :return:
         """
         if self.trajectory_gdf.empty:
             self.trajectory_gdf = self.format_gdf(from_crs=self.from_crs,
                                                   to_crs=self.to_crs,
                                                   crs=self.crs, convert_loc=self.convert_loc,
                                                   convert_type=self.convert_type,
                                                   info_list=self.trajectory_info_list,
                                                   attr_name_field_list=[gps_field.TIME_FIELD, gps_field.GEOMETRY_FIELD,
                                                                         gps_field.HEADING_FIELD,
-                                                                        gps_field.AGENT_ID_FIELD])
+                                                                        gps_field.AGENT_ID_FIELD],
+                                                  time_format=time_format)
         if out_fldr is None:
             pass
         else:
             self.save_file(file_type=file_type, df=self.trajectory_gdf, out_fldr=out_fldr, file_name=file_name)
         return self.trajectory_gdf
 
     @function_time_cost
-    def save_gps_info(self, out_fldr: str = r'./', file_name: str = None, file_type: str = 'csv') -> gpd.GeoDataFrame:
+    def save_gps_info(self, out_fldr: str = r'./', file_name: str = None, file_type: str = 'csv',
+                      time_format="%Y-%m-%d %H:%M:%S") -> gpd.GeoDataFrame:
         """
         存储gps信息
         :param out_fldr:
         :param file_name:
         :param file_type:
+        :param time_format:
         :return:
         """
         if self.gps_gdf.empty:
             self.gps_gdf = self.format_gdf(convert_prj_sys=self.convert_prj_sys, from_crs=self.from_crs,
                                            to_crs=self.to_crs,
                                            crs=self.crs, convert_loc=self.convert_loc, convert_type=self.convert_type,
                                            info_list=self.gps_info_list,
                                            attr_name_field_list=[gps_field.TIME_FIELD, gps_field.GEOMETRY_FIELD,
                                                                  gps_field.HEADING_FIELD, gps_field.AGENT_ID_FIELD,
                                                                  net_field.LINK_ID_FIELD,
-                                                                 net_field.FROM_NODE_FIELD, net_field.TO_NODE_FIELD])
+                                                                 net_field.FROM_NODE_FIELD, net_field.TO_NODE_FIELD],
+                                           time_format=time_format)
         if out_fldr is None:
             pass
         else:
             self.save_file(file_type=file_type, df=self.gps_gdf, out_fldr=out_fldr, file_name=file_name)
         return self.gps_gdf
     @function_time_cost
     def save_mix_info(self, out_fldr: str = r'./', file_name: str = None, convert_prj_sys: bool = True,
                       from_crs: str = None, to_crs: str = None, crs: str = None,
-                      convert_loc: bool = False, convert_type: str = 'bd-84', file_type: str = 'csv') -> gpd.GeoDataFrame:
+                      convert_loc: bool = False, convert_type: str = 'bd-84', file_type: str = 'csv',
+                      time_format="%Y-%m-%d %H:%M:%S") -> gpd.GeoDataFrame:
         """
 
         :param out_fldr:
         :param file_name:
         :param convert_prj_sys:
         :param from_crs:
         :param to_crs:
         :param crs:
         :param convert_loc:
         :param convert_type:
         :param file_type:
+        :param time_format
         :return:
         """
         if self.gps_gdf.empty:
             self.gps_gdf = self.format_gdf(convert_prj_sys=convert_prj_sys, from_crs=from_crs, to_crs=to_crs,
                                            crs=crs, convert_loc=convert_loc, convert_type=convert_type,
                                            info_list=self.gps_info_list,
                                            attr_name_field_list=[gps_field.TIME_FIELD, gps_field.GEOMETRY_FIELD,
                                                                  gps_field.HEADING_FIELD, gps_field.AGENT_ID_FIELD,
                                                                  net_field.LINK_ID_FIELD,
-                                                                 net_field.FROM_NODE_FIELD, net_field.TO_NODE_FIELD])
+                                                                 net_field.FROM_NODE_FIELD, net_field.TO_NODE_FIELD],
+                                           time_format=time_format)
         if self.trajectory_gdf.empty:
             self.trajectory_gdf = self.format_gdf(convert_prj_sys=convert_prj_sys, from_crs=from_crs, to_crs=to_crs,
                                                   crs=crs, convert_loc=convert_loc, convert_type=convert_type,
                                                   info_list=self.trajectory_info_list,
                                                   attr_name_field_list=[gps_field.TIME_FIELD, gps_field.GEOMETRY_FIELD,
                                                                         gps_field.HEADING_FIELD,
-                                                                        gps_field.AGENT_ID_FIELD])
+                                                                        gps_field.AGENT_ID_FIELD],
+                                                  time_format=time_format)
         self.gps_gdf[gps_field.TYPE_FIELD] = 'gps'
         self.trajectory_gdf[gps_field.TYPE_FIELD] = 'trajectory'
         mix_gdf = pd.concat([self.trajectory_gdf, self.gps_gdf])
         mix_gdf.reset_index(inplace=True, drop=True)
         if out_fldr is None:
             pass
         else:
```

### Comparing `gotrackit-0.2.7/src/gotrackit/gps/GpsArray.py` & `gotrackit-0.2.9/src/gotrackit/gps/GpsArray.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,16 +44,17 @@
         try:
             self.gps_points_gdf[gps_field.TIME_FIELD] = \
                 pd.to_datetime(self.gps_points_gdf[gps_field.TIME_FIELD], format=time_format)
         except ValueError:
             print(rf'time column does not match format {time_format}, try using time-unit: {time_unit}')
             self.gps_points_gdf[gps_field.TIME_FIELD] = \
                 pd.to_datetime(self.gps_points_gdf[gps_field.TIME_FIELD], unit=time_unit)
-
-        self.gps_points_gdf.sort_values(by=[gps_field.TIME_FIELD], ascending=[True], inplace=True)
+        self.gps_points_gdf.sort_values(by=[gps_field.AGENT_ID_FIELD, gps_field.TIME_FIELD],
+                                        ascending=[True, True], inplace=True)
+        self.gps_points_gdf.drop_duplicates(subset=[agent_field, time_field], keep='first', inplace=True)
         self.gps_points_gdf.reset_index(inplace=True, drop=True)
         self.to_plane_prj()
 
         # 存储最原始的GPS信息
         self.__source_gps_points_gdf = self.gps_points_gdf.copy()
         self.check()
```

### Comparing `gotrackit-0.2.7/src/gotrackit/gps/GpsXfer.py` & `gotrackit-0.2.9/src/gotrackit/gps/GpsXfer.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.7/src/gotrackit/gps/LocGps.py` & `gotrackit-0.2.9/src/gotrackit/gps/LocGps.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.7/src/gotrackit/map/Link.py` & `gotrackit-0.2.9/src/gotrackit/map/Link.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.7/src/gotrackit/map/Net.py` & `gotrackit-0.2.9/src/gotrackit/map/Net.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
     @function_time_cost
     def __init__(self, link_path: str = None, node_path: str = None, link_gdf: gpd.GeoDataFrame = None,
                  node_gdf: gpd.GeoDataFrame = None, weight_field: str = 'length', init_from_existing: bool = False,
                  is_check: bool = True, create_single: bool = True, search_method: str = 'dijkstra',
                  ft_link_mapping: dict = None, double_single_mapping: dict = None, link_ft_mapping: dict = None,
                  link_t_mapping: dict = None, link_f_mapping: dict = None, link_geo_mapping: dict = None,
-                 not_conn_cost: float = 999.0, cache_path: bool = True, cache_id: bool = True,
+                 not_conn_cost: float = 1000.0, cache_path: bool = True, cache_id: bool = True,
                  is_sub_net: bool = False, fmm_cache: bool = False, cache_cn: int = 2, cache_slice: int = None,
                  fmm_cache_fldr: str = None,
                  cache_name: str = 'cache', recalc_cache: bool = True,
                  cut_off: float = 1200.0, max_cut_off: float = 5000.0, delete_circle: bool = True):
         """
         创建Net类
         :param link_path: link层的路网文件路径, 若指定了该参数, 则直接从磁盘IO创建Net线层
@@ -479,14 +479,27 @@
 
     def drop_dup_ft_road(self):
         self.__link.drop_dup_ft_road()
 
     def merger_double_link(self):
         self.__link.merge_double_link()
 
+    def check_ln_consistency(self):
+        l_node = self.__link.used_node()
+        n_node = self.__node.node_id_set()
+        gap = n_node - l_node
+        # print(rf'1: {gap}')
+        if gap:
+            # 点层中存在线层没有用的点, 直接删掉
+            self.__node.delete_nodes(node_list=list(gap))
+
+        # n_node = self.__node.node_id_set()
+        # gap = l_node - n_node
+        # print(rf'2: {gap}')
+
     def del_short_links(self, l_threshold: float = 0.5) -> None:
         self.__link.del_short_links(l_threshold=l_threshold)
         self.del_zero_degree_nodes()
 
     def del_zero_degree_nodes(self) -> None:
         self.__node.delete_nodes(node_list=list(self.__node.node_id_set() - self.__link.used_node()))
```

### Comparing `gotrackit-0.2.7/src/gotrackit/map/Node.py` & `gotrackit-0.2.9/src/gotrackit/map/Node.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.7/src/gotrackit/model/Markov.py` & `gotrackit-0.2.9/src/gotrackit/model/Markov.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,15 +192,15 @@
                     self.init_warn_info()
 
         return True, match_res
 
     def __calc_emission(self, use_heading_inf: bool = True, omitted_l: float = 6.0, gps_sigma: float = 30.0):
         # 计算每个观测点的生成概率, 这是在计算状态转移概率之后, 已经将关联不到的GPS点删除了
         if use_heading_inf:
-            if gps_field.X_DIFF not in self.__done_prj_df.columns:
+            if not self.gps_points.done_diff_heading:
                 self.gps_points.calc_diff_heading()
                 self.__done_prj_df = pd.merge(self.__done_prj_df, self.gps_points.gps_gdf[[gps_field.POINT_SEQ_FIELD,
                                                                                            gps_field.X_DIFF,
                                                                                            gps_field.Y_DIFF,
                                                                                            gps_field.VEC_LEN]],
                                               how='left',
                                               on=gps_field.POINT_SEQ_FIELD)
```

### Comparing `gotrackit-0.2.7/src/gotrackit/model/Para.py` & `gotrackit-0.2.9/src/gotrackit/model/Para.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.7/src/gotrackit/netreverse/GlobalVal.py` & `gotrackit-0.2.9/src/gotrackit/netreverse/GlobalVal.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.7/src/gotrackit/netreverse/NetGen.py` & `gotrackit-0.2.9/src/gotrackit/netreverse/NetGen.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,32 +7,31 @@
 """生产路网的相关方法"""
 
 import os.path
 import pandas as pd
 import geopandas as gpd
 from ..map.Net import Net
 from .RoadNet.conn import Conn
-from .GlobalVal import NetField
 from .format_od import FormatOD
 from .RoadNet import net_reverse
-from ..gps.GpsTrip import GpsTrip
 from .RoadNet.increment import increment
+from .GlobalVal import NetField, GpsField
 from .RoadNet.save_file import save_file
 from .Request.request_path import CarPath
 from .RoadNet.optimize_net import optimize
 from .Parse.gd_car_path import ParseGdPath
 from .RoadNet.Split.SplitPath import split_path
 from .PublicTools.GeoProcess import generate_region
 from .RoadNet.Split.SplitPath import split_path_main
 from ..tools.geo_process import clean_link_geo, remapping_id
 from .RoadNet.Tools.process import merge_double_link, create_single_link
 from .RoadNet.SaveStreets.streets import generate_node_from_link, modify_minimum
 
-
 net_field = NetField()
+gps_field = GpsField()
 
 class Reverse(object):
     def __init__(self, flag_name: str = '深圳市', plain_prj: str = None, net_out_fldr: str = None,
                  net_file_type: str = 'shp'):
         # overall
         self.flag_name = flag_name
         self.plain_prj = plain_prj
@@ -293,33 +292,34 @@
                      cache_times: int = 300, ignore_hh: bool = True, remove_his: bool = True,
                      log_fldr: str = None, save_log_file: bool = False,
                      min_lng: float = None, min_lat: float = None, w: float = 2000, h: float = 2000,
                      od_num: int = 100, gap_n: int = 1000, min_od_length: float = 1200.0) -> tuple[bool, list[str]]:
         """构造OD -> 请求 -> 二进制存储"""
         assert binary_path_fldr is not None
 
-        assert od_type in ['rand_od', 'region_od', 'diy_od', 'gps_based']
+        assert od_type in ['rand_od', 'region_od', 'diy_od']
         fmod = FormatOD(plain_crs=self.plain_prj)
         if isinstance(region_gdf, gpd.GeoDataFrame) and not region_gdf.empty:
             assert region_gdf.crs.srs.upper() == 'EPSG:4326', '面域文件必须是EPSG:4326"'
         if od_type == 'rand_od':
             if region_gdf is None or region_gdf.empty:
                 region_gdf = generate_region(min_lng=min_lng, min_lat=min_lat, w=w, h=h, plain_crs=self.plain_prj)
 
             od_df = fmod.format_region_rnd_od(region_gdf=region_gdf, flag_name=self.flag_name, od_num=od_num,
                                               gap_n=gap_n, length_limit=min_od_length,
                                               boundary_buffer=boundary_buffer)
             self.__region_gdf = region_gdf
+            od_file_path = None
         elif od_type == 'region_od':
             od_df = fmod.format_region_od(region_gdf=region_gdf)
+            od_file_path = None
         elif od_type == 'diy_od':
             if od_df is None or od_df.empty:
                 od_df = pd.read_csv(od_file_path)
-        elif od_type == 'gps_based':
-            raise ValueError('Sorry! This function is under development! 这个函数正在开发中...')
+                od_file_path = None
 
         self.__od_df = od_df
 
         path_request_obj = CarPath(key_list=key_list, input_file_path=od_file_path, od_df=od_df,
                                    cache_times=cache_times, ignore_hh=ignore_hh, out_fldr=binary_path_fldr,
                                    file_flag=self.flag_name, log_fldr=log_fldr, save_log_file=save_log_file)
 
@@ -473,20 +473,7 @@
         single_link_gdf = create_single_link(link_gdf=link_gdf)
         if self.limit_col_name not in single_link_gdf.columns:
             single_link_gdf[self.limit_col_name] = 'XX路'
         single_link_gdf = split_path(path_gdf=single_link_gdf)
         single_link_gdf.drop(columns=['ft_loc'], axis=1, inplace=True)
         del link_gdf
         self.__generate_net_from_split_path(split_path_gdf=single_link_gdf)
-
-    @staticmethod
-    def generate_od_by_gps(gps_df: pd.DataFrame = None, time_format: str = '%Y-%m-%d %H:%M:%S', time_unit: str = 's',
-                           plain_crs: str = 'EPSG:32650', group_gap_threshold: float = 360.0, n: int = 5,
-                           min_distance_threshold: float = 10.0, way_points_num: int = 5,
-                           dwell_accu_time: float = 60.0) -> tuple[pd.DataFrame, gpd.GeoDataFrame]:
-        gtp = GpsTrip(gps_df=gps_df, time_unit=time_unit, time_format=time_format, plain_crs=plain_crs,
-                      group_gap_threshold=group_gap_threshold, n=n, min_distance_threshold=min_distance_threshold,
-                      way_points_num=way_points_num, dwell_accu_time=dwell_accu_time)
-        gtp.add_main_group()
-        od_df, od_line = gtp.generate_od()
-        return od_df, od_line
-
```

### Comparing `gotrackit-0.2.7/src/gotrackit/netreverse/Parse/gd_car_path.py` & `gotrackit-0.2.9/src/gotrackit/netreverse/Parse/gd_car_path.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.7/src/gotrackit/netreverse/PublicTools/GeoProcess.py` & `gotrackit-0.2.9/src/gotrackit/netreverse/PublicTools/GeoProcess.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.7/src/gotrackit/netreverse/PublicTools/GraphAna.py` & `gotrackit-0.2.9/src/gotrackit/netreverse/PublicTools/GraphAna.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.7/src/gotrackit/netreverse/PublicTools/IndexAna.py` & `gotrackit-0.2.9/src/gotrackit/netreverse/PublicTools/IndexAna.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.7/src/gotrackit/netreverse/PublicTools/od.py` & `gotrackit-0.2.9/src/gotrackit/netreverse/PublicTools/od.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.7/src/gotrackit/netreverse/Request/api/WebApi.py` & `gotrackit-0.2.9/src/gotrackit/netreverse/Request/api/WebApi.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,38 +4,38 @@
 # @Team    : ZheChengData
 
 import json
 import requests
 import numpy as np
 
 class GdRoutePlan(object):
-    def __init__(self, key_list=None, ):
-        self.key_list = key_list
-        assert len(key_list) >= 1, '至少有一个key值'
+    def __init__(self):
+        pass
 
-    def car_route_plan(self, od_id=None, origin=None, destination=None,
+    @staticmethod
+    def car_route_plan(od_id=None, origin=None, destination=None, key: str = None,
                        origin_id=None, destination_id=None,
                        origin_type=None, avoidpolygons=None,
                        waypoints_loc=None, strategy='32', is_rnd_strategy=False):
         """
         # 参数含义见: https://lbs.amap.com/api/webservice/guide/api/newroute
+        :param key:
         :param origin:
         :param destination:
         :param origin_id:
         :param destination_id:
         :param origin_type:
         :param avoidpolygons:
         :param od_id:
         :param waypoints_loc:
         :param strategy:
         :param is_rnd_strategy: 是否启用随机策略
         :return:
         """
         api_url = 'https://restapi.amap.com/v5/direction/driving'
-        key = self.key_list[np.random.randint(0, len(self.key_list))]
         para_dict = {'key': key}
         if is_rnd_strategy:
             strategy_list = ['0', '1', '2', '3', '32', '34', '35', '36', '37', '42']
             strategy = strategy_list[np.random.randint(0, len(strategy_list))]
         else:
             if strategy is None:
                 strategy = '0'
@@ -43,15 +43,15 @@
                      'waypoints_loc', 'strategy']
         para_val = [od_id, origin, destination, origin_id, destination_id, origin_type, avoidpolygons, waypoints_loc,
                     strategy]
         for name, val in zip(para_name, para_val):
             if para_val is not None:
                 para_dict.update({name: val})
         para_dict.update({'show_fields': "cost,navi,tmcs,polyline"})
-        print(para_dict)
+        # print(para_dict)
         # 请求
         try:
             r = requests.get(api_url, params=para_dict, timeout=10)
             json_data = json.loads(r.text)
             info_code = json_data['infocode']
         except:
             return None, None
```

### Comparing `gotrackit-0.2.7/src/gotrackit/netreverse/Request/request_path.py` & `gotrackit-0.2.9/src/gotrackit/netreverse/Request/request_path.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,26 +34,28 @@
         otr = RequestOnTime(key_list=self.key_list,
                             od_df=self.od_df,
                             input_file_path=self.input_file_path)
         if not self.ignore_hh:
             assert hh_field in self.od_df.columns, rf'如果启用了时段限制, 请确保od表中有{hh_field}字段, 否则请将ignore_hh参数设为True'
             self.od_df[hh_field] = self.od_df[hh_field].astype(int)
             assert set(self.od_df[hh_field]).issubset({i for i in range(0, 24)}), rf'{hh_field}字段的值有误!'
+        key_info_dict = {k: 0 for k in self.key_list}
         while True:
             if_end_request, new_file_list = otr.start_request(out_fldr=self.out_fldr,
                                                               cache_times=self.cache_times,
                                                               id_field=od_id_field,
                                                               ignore_hh=self.ignore_hh,
                                                               file_flag=self.file_flag,
                                                               o_x_field=o_x_field,
                                                               o_y_field=o_y_field,
                                                               d_x_field=d_x_field, d_y_field=d_y_field,
                                                               way_points_field=way_points_field,
                                                               request_hh_field=hh_field,
                                                               log_fldr=self.log_fldr,
                                                               remove_his=remove_his,
-                                                              save_log_file=self.save_log_file)
+                                                              save_log_file=self.save_log_file,
+                                                              key_info_dict=key_info_dict)
             if if_end_request:
                 break
             else:
                 pass
         return if_end_request, new_file_list
```

### Comparing `gotrackit-0.2.7/src/gotrackit/netreverse/Request/usage/bd_ts.py` & `gotrackit-0.2.9/src/gotrackit/netreverse/Request/usage/bd_ts.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.7/src/gotrackit/netreverse/Request/usage/gd_car_path.py` & `gotrackit-0.2.9/src/gotrackit/netreverse/Request/usage/gd_car_path.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,26 +11,28 @@
 import datetime
 import numpy as np
 import pandas as pd
 from ..api.WebApi import GdRoutePlan
 
 
 class RequestOnTime(object):
-    def __init__(self, key_list=None, input_file_path=None, od_df: pd.DataFrame = None):
-        self.key_list = key_list
+    def __init__(self, key_list: list[str] = None, input_file_path: str = None, od_df: pd.DataFrame = None):
+        self.key_list = list(set(key_list))
+        self.origin_key_list = self.key_list.copy()
         if input_file_path is None:
             self.od_df = od_df
         else:
             self.od_df = pd.read_csv(input_file_path)
 
-    def start_request(self, out_fldr=None, cache_times=2000, id_field=None,
-                      file_flag=None, o_x_field='o_x', o_y_field='o_y',
-                      d_x_field='d_x', d_y_field='d_y', way_points_field=None,
-                      request_hh_field=None, ignore_hh=False, log_fldr: str = None, save_log_file: bool = False,
-                      remove_his: bool = True):
+    def start_request(self, out_fldr: str = None, cache_times: int = 2000, id_field: str = None,
+                      file_flag: str = None, o_x_field: str = 'o_x', o_y_field: str = 'o_y',
+                      d_x_field: str = 'd_x', d_y_field: str = 'd_y', way_points_field: str = None,
+                      request_hh_field: str = None, ignore_hh: bool = False, log_fldr: str = None,
+                      save_log_file: bool = False,
+                      remove_his: bool = True, key_info_dict: dict[str, int] = None):
         """
         给一个od表, 按照时间进行请求
         :param out_fldr:
         :param cache_times:
         :param id_field:
         :param file_flag:
         :param o_x_field:
@@ -39,30 +41,24 @@
         :param d_y_field:
         :param way_points_field:
         :param request_hh_field:
         :param ignore_hh:
         :param log_fldr:
         :param save_log_file:
         :param remove_his
+        :param key_info_dict:
         :return:
         """
 
-        # 1. 配置日志输出
-        # prj_root_fldr = os.getcwd()
-        # if 'log' not in os.listdir(os.path.join(prj_root_fldr, 'data/output/')):
-        #     os.makedirs(os.path.join(prj_root_fldr, 'data/output/log/'))
-
         console_handler = logging.StreamHandler(sys.stdout)
         console_handler.setFormatter(
             logging.Formatter('[%(asctime)s %(levelname)s] %(message)s', datefmt='%m/%d/%Y %H:%M:%S'))
         console_handler.setLevel(logging.INFO)
 
         if log_fldr is not None and save_log_file:
-            # file_handler = logging.FileHandler(os.path.join(prj_root_fldr, fr'data/output/log/log_request_{file_flag}.log'),
-            #                                    mode='a')
             file_handler = logging.FileHandler(os.path.join(log_fldr, fr'log_request_{file_flag}.log'), mode='a')
 
             file_handler.setFormatter(
                 logging.Formatter('[%(asctime)s %(levelname)s] %(message)s', datefmt='%m/%d/%Y %H:%M:%S'))
             file_handler.setLevel(logging.INFO)
             logging.basicConfig(level=logging.INFO, format='%(asctime)s %(message)s',
                                 handlers=[file_handler, console_handler])
@@ -95,15 +91,15 @@
         except:
             already_request_list = []
 
         logging.info(rf'请求{file_flag}, 第{last_num + 1}个文件...')
         logging.info(rf'already_request_list_len: {len(already_request_list)}')
 
         # 路径规划对象
-        route_plan = GdRoutePlan(self.key_list)
+        route_plan = GdRoutePlan()
 
         # 开始请求数据
         while continue_request:
             # 删除已经请求的和发生联通错误的......
             self.od_df.drop(index=self.od_df[self.od_df[id_field].isin(already_request_list)].index, inplace=True, axis=0)
             self.od_df.reset_index(drop=True, inplace=True)
             logging.info(rf'尚且未请求的有{len(self.od_df)}条')
@@ -129,106 +125,114 @@
             # 开始请求当前时段的
             od_route_dict, done_list, is_end = self.request_hh_df(request_df=request_df, cache_times=cache_times,
                                                                   request_hh=request_hour,
                                                                   id_field=id_field, o_x_field=o_x_field,
                                                                   o_y_field=o_y_field,
                                                                   d_x_field=d_x_field, d_y_field=d_y_field,
                                                                   way_points_field=way_points_field,
-                                                                  route_plan_obj=route_plan, ignore_hh=ignore_hh)
+                                                                  route_plan_obj=route_plan, ignore_hh=ignore_hh,
+                                                                  key_info_dict=key_info_dict,
+                                                                  key_list=self.key_list)
 
             already_request_list.extend(done_list)
-            last_num += 1
-            self.save_file(out_fldr=out_fldr, file_flag=file_prefix, last_num=last_num,
-                           od_route_dict=od_route_dict, already_request_list=already_request_list)
-            new_file_list.append(rf'{file_prefix}_gd_path_{last_num}')
+            if od_route_dict:
+                last_num += 1
+                self.save_file(out_fldr=out_fldr, file_flag=file_prefix, last_num=last_num,
+                               od_route_dict=od_route_dict, already_request_list=already_request_list)
+                new_file_list.append(rf'{file_prefix}_gd_path_{last_num}')
 
             # 配额达到上限
             if is_end:
                 logging.info(rf'开始休眠等待配额恢复...')
                 time.sleep(3600)
+                self.key_list = self.origin_key_list.copy()
+                key_info_dict = {k: 0 for k in self.key_list}
 
     @staticmethod
     def request_hh_df(request_df=None, cache_times=None, request_hh=None,
                       id_field=None, o_x_field='o_x', o_y_field='o_y', d_x_field='d_x', d_y_field='d_y',
-                      way_points_field=None, route_plan_obj=None, ignore_hh=True):
+                      way_points_field=None, route_plan_obj=None, ignore_hh=True, key_info_dict: dict[str, int] = None,
+                      key_list: list[str] = None):
         """请求给定表的od, 每达到cache_times次(或者在规定时段内没有请求完或者提前请求完或者达到配额上限)就返回"""
         _count = 0  # 用于计数
         od_route_dict = dict()  # 用于存储请求结果
         done_list = []  # 用于存储请求成功的od_id
         not_conn_error_num = 0  # 用于记录搜路失败的od数目
         not_conn_error_list = []  # 用于记录搜路失败的od_id
         http_error_num = 0  # 用于记录网络失败的od数目
         http_error_list = []  # 用于记录网络失败的od_id
-        limit_num = 0
         for _, row in request_df.iterrows():
             strategy = None
             is_rnd_strategy = True
             od_id = int(row[id_field])
             o_loc = ','.join([str(np.around(row[o_x_field], decimals=6)), str(np.around(row[o_y_field], 6))])
             d_loc = ','.join([str(np.around(row[d_x_field], decimals=6)), str(np.around(row[d_y_field], 6))])
             if way_points_field in request_df.columns:
                 way_points = row[way_points_field]
                 if way_points not in [None, '', ' ']:
-                    logging.info(rf'启用途径点...')
+                    logging.info(rf'Enable waypoints.')
                     is_rnd_strategy = False
                     strategy = '0'
             else:
                 way_points = None
                 is_rnd_strategy = True
-
-            json_data, info_code = route_plan_obj.car_route_plan(origin=o_loc, destination=d_loc,
+            key = key_list[np.random.randint(0, len(key_list))]
+            json_data, info_code = route_plan_obj.car_route_plan(origin=o_loc, destination=d_loc, key=key,
                                                                  od_id=od_id, waypoints_loc=way_points,
                                                                  is_rnd_strategy=is_rnd_strategy, strategy=strategy)
-            logging.info(rf'info_code: {info_code}, count: {_count}, od: {od_id}')
 
             if info_code is not None:
                 # 请求成功
                 if info_code == 10000:
-                    logging.info(r'请求成功')
+                    logging.info(rf'Success - od: {od_id}, info_code: {info_code}, Request Success, count: {_count}.')
                     od_route_dict[od_id] = json_data
                     done_list.append(od_id)
                     _count += 1
-                elif info_code in [10003]:
-                    limit_num += 1
-                    if limit_num >= 30:
-                        logging.info(r'达到配额上限,结束请求')
+                elif info_code in [10003, 10044, 10014, 10019, 10020, 10021, 10029, 10045]:
+                    logging.info(rf'Failure - od: {od_id}, info_code: {info_code}, Quotas Exceeded, count: {_count}.')
+                    key_info_dict[key] += 1
+                    if key_info_dict[key] >= 30 and key in key_list:
+                        logging.info(rf'A key has reached the quota limit and is abandoned.')
+                        key_list.remove(key)
+                    if not key_list:
+                        logging.info(rf'All keys have reached the quota limit, stop requesting.')
                         return od_route_dict, done_list, True
-                elif info_code in [20003, 20011, 20012, 20800, 20801, 20802, 20803]:
-                    # 其他错误(未知错误, 路径错误......), 这部分不会重复请求
-                    logging.info(r'未知错误, 路径错误...')
+                else:
+                    logging.info(rf'Failure - od: {od_id}, info_code: {info_code}, Planning Error, count: {_count}.')
                     not_conn_error_num += 1
                     not_conn_error_list.append(od_id)
                     done_list.append(od_id)
                     _count += 1
             else:
+                logging.info(rf'Failure - od: {od_id}, info_code: XXXXX, Https Error, count: {_count}.')
                 # 网络错误
                 http_error_num += 1
                 http_error_list.append(od_id)
 
             # 达到请求次数后缓存一次
             if _count >= cache_times:
-                logging.info(rf'达到缓存次数..., 返回')
-                logging.info(rf'路网不连通导致的失败od数: {len(not_conn_error_list)}')
-                logging.info(rf'https网络导致的失败od数: {len(http_error_list)}')
+                logging.info(rf'Reached the cache count, return.')
+                logging.info(rf'Number of failures due to planning errors: {len(not_conn_error_list)}.')
+                logging.info(rf'Number of failures due to http errors: {len(http_error_list)}.')
                 return od_route_dict, done_list, False
 
             if ignore_hh:
                 pass
             else:
                 # 请求完一个后检查时间
                 if datetime.datetime.now().hour != request_hh:
-                    logging.info(rf'时段超限..., 返回')
-                    logging.info(rf'路网不连通导致的失败od数: {len(not_conn_error_list)}')
-                    logging.info(rf'https网络导致的失败od数: {len(http_error_list)}')
+                    logging.info(rf'Time limit exceeded, return.')
+                    logging.info(rf'Number of failures due to planning errors: {len(not_conn_error_list)}.')
+                    logging.info(rf'Number of failures due to http errors: {len(http_error_list)}.')
                     return od_route_dict, done_list, False
 
         # 既没有达到缓存次数也没有时段超限
-        logging.info(rf'od请求完毕, 没有达到配额上限也没有达到缓存次数..., 返回')
-        logging.info(rf'路网不连通导致的失败od数: {len(not_conn_error_list)}')
-        logging.info(rf'https网络导致的失败od数: {len(http_error_list)}')
+        logging.info(rf'od request completed, return.')
+        logging.info(rf'Number of failures due to planning errors: {len(not_conn_error_list)}.')
+        logging.info(rf'Number of failures due to http errors: {len(http_error_list)}.')
         return od_route_dict, done_list, False
 
     @staticmethod
     def save_file(out_fldr=None, file_flag=None, last_num=None,
                   od_route_dict=None, already_request_list=None):
         with open(os.path.join(out_fldr, rf'{file_flag}_gd_path_{last_num}'), 'wb') as f:
             pickle.dump(od_route_dict, f)
```

### Comparing `gotrackit-0.2.7/src/gotrackit/netreverse/RoadNet/DupProcess/DupLinks.py` & `gotrackit-0.2.9/src/gotrackit/netreverse/RoadNet/DupProcess/DupLinks.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.7/src/gotrackit/netreverse/RoadNet/Merge/get_merged_link_seq.py` & `gotrackit-0.2.9/src/gotrackit/netreverse/RoadNet/Merge/get_merged_link_seq.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.7/src/gotrackit/netreverse/RoadNet/Merge/limit/attr_limit.py` & `gotrackit-0.2.9/src/gotrackit/netreverse/RoadNet/Merge/limit/attr_limit.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.7/src/gotrackit/netreverse/RoadNet/Merge/limit/direction_limit.py` & `gotrackit-0.2.9/src/gotrackit/netreverse/RoadNet/Merge/limit/direction_limit.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.7/src/gotrackit/netreverse/RoadNet/Merge/limit/same_head_tail_limit.py` & `gotrackit-0.2.9/src/gotrackit/netreverse/RoadNet/Merge/limit/same_head_tail_limit.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.7/src/gotrackit/netreverse/RoadNet/Merge/limit/two_degrees_group.py` & `gotrackit-0.2.9/src/gotrackit/netreverse/RoadNet/Merge/limit/two_degrees_group.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.7/src/gotrackit/netreverse/RoadNet/Merge/merge_links.py` & `gotrackit-0.2.9/src/gotrackit/netreverse/RoadNet/Merge/merge_links.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     origin_crs = new_link.crs
     if origin_crs == plain_prj:
         pass
     else:
         new_link = new_link.to_crs(plain_prj)
         new_link[length_field] = new_link[geometry_field].apply(lambda x: x.length)
         new_link = new_link.to_crs(origin_crs)
-
+    drop_no_use_nodes(link_gdf=new_link, node_gdf=new_node)
     return new_link, new_node, info_dict
 
 
 # 逻辑子模块, 只记录合并信息, 并不修改传入的数据
 def merge_links(link_gdf=None, node_gdf=None, merge_link_df=None) -> (gpd.GeoDataFrame, gpd.GeoDataFrame, dict):
     """传入可合并的路段组, 直接在线层数据, 点层数据上修改
     :param link_gdf: gpd.GeoDataFrame, 线层数据
@@ -269,7 +269,13 @@
         except ValueError as e:
             # print(r'是平面坐标')
             return linestring_obj.length
     else:
         return linestring_obj.length
 
 
+def drop_no_use_nodes(link_gdf: gpd.GeoDataFrame = None, node_gdf: gpd.GeoDataFrame = None):
+    # 去除没有link连接的节点
+    used_node = set(link_gdf[net_field.FROM_NODE_FIELD]) | set(link_gdf[net_field.TO_NODE_FIELD])
+    node_gdf.reset_index(inplace=True, drop=True)
+    node_gdf.drop(index=node_gdf[~node_gdf[net_field.NODE_ID_FIELD].isin(used_node)].index, inplace=True, axis=1)
+    node_gdf.reset_index(inplace=True, drop=True)
```

### Comparing `gotrackit-0.2.7/src/gotrackit/netreverse/RoadNet/Merge/merge_short.py` & `gotrackit-0.2.9/src/gotrackit/netreverse/RoadNet/Merge/merge_short.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.7/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/attr_limit.py` & `gotrackit-0.2.9/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/attr_limit.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.7/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/direction_limit.py` & `gotrackit-0.2.9/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/direction_limit.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.7/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/same_head_tail_limit.py` & `gotrackit-0.2.9/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/same_head_tail_limit.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.7/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/two_degrees_group.py` & `gotrackit-0.2.9/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/two_degrees_group.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.7/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/merge_links_multi.py` & `gotrackit-0.2.9/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/merge_links_multi.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,23 +69,23 @@
 
     # 初步确定所有的可以合并的group
     connected_components, two_degrees_sub_graph = get_connected_components(ud_graph=ud_graph, d_graph=d_graph)
 
     # 对迭代器切片
     connected_components_group = cut_group(obj_list=connected_components, n=core_num)
     del connected_components
-    print(len(connected_components_group))
+    n = len(connected_components_group)
     # 测试
     # merge_link_df = get_merge_df_main(link_gdf, node_gdf, connected_components_group[0], two_degrees_sub_graph,
     #                                   ud_graph, allow_ring, ignore_dir, judge_col_name, plain_prj, accu_l_threshold,
     #                                   angle_threshold, restrict_length, restrict_angle, min_length)
     print('starting filter group')
-    pool = multiprocessing.Pool(processes=len(connected_components_group))
+    pool = multiprocessing.Pool(processes=n)
     result_list = []
-    for i in range(0, len(connected_components_group)):
+    for i in range(0, n):
         result = pool.apply_async(get_merge_df_main,
                                   args=(link_gdf, node_gdf, connected_components_group[i], two_degrees_sub_graph,
                                         ud_graph, allow_ring, ignore_dir, limit_col_name, plain_prj, accu_l_threshold,
                                         angle_threshold, restrict_length, restrict_angle, min_length))
         result_list.append(result)
     pool.close()
     pool.join()
@@ -94,14 +94,15 @@
     merge_link_df = pd.DataFrame()
     for merge_res in result_list:
         merge_link_df = pd.concat([merge_link_df, merge_res.get()])
     merge_link_df.reset_index(inplace=True, drop=True)
     del result_list
 
     if merge_link_df.empty:
+        drop_no_use_nodes(link_gdf=link_gdf, node_gdf=node_gdf)
         return link_gdf, node_gdf
 
     origin_crs = link_gdf.crs.srs
     link_gdf['sorted_ft'] = link_gdf[[from_node_id_field, to_node_id_field]].apply(lambda x: tuple(sorted(x)), axis=1)
     origin_sorted_ft_list = link_gdf['sorted_ft'].to_list()
 
     # 计算head_node, tail_node, root_node
@@ -158,14 +159,15 @@
     link_gdf.drop(index=target_link_index, inplace=True, axis=0)
     new_link_gdf = gpd.GeoDataFrame(new_link_df, crs=link_gdf.crs.srs, geometry='geometry')
     del new_link_df
 
     link_gdf = pd.concat([link_gdf, new_link_gdf])
     link_gdf.reset_index(inplace=True, drop=True)
     link_gdf.drop(columns=['sorted_ft'], axis=1, inplace=True)
+    drop_no_use_nodes(link_gdf=link_gdf, node_gdf=node_gdf)
     return link_gdf, node_gdf, merge_info_dict
 
 
 def build_graph_from_link(link_df=None, from_col_name='from', to_col_name='to', ignore_dir=False, dir_col='dir'):
     """
     根据路网的from_node, to_node, dir字段建立图
     :param link_df: pd.DataFrame, 路网线层数据
@@ -464,7 +466,13 @@
         except ValueError as e:
             # print(r'是平面坐标')
             return linestring_obj.length
     else:
         return linestring_obj.length
 
 
+def drop_no_use_nodes(link_gdf: gpd.GeoDataFrame = None, node_gdf: gpd.GeoDataFrame = None):
+    # 去除没有link连接的节点
+    used_node = set(link_gdf[net_field.FROM_NODE_FIELD]) | set(link_gdf[net_field.TO_NODE_FIELD])
+    node_gdf.reset_index(inplace=True, drop=True)
+    node_gdf.drop(index=node_gdf[~node_gdf[net_field.NODE_ID_FIELD].isin(used_node)].index, inplace=True, axis=1)
+    node_gdf.reset_index(inplace=True, drop=True)
```

### Comparing `gotrackit-0.2.7/src/gotrackit/netreverse/RoadNet/SaveStreets/streets.py` & `gotrackit-0.2.9/src/gotrackit/netreverse/RoadNet/SaveStreets/streets.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,14 +240,16 @@
         index=join_df[join_df[net_field.NODE_ID_FIELD + '_left'] == join_df[net_field.NODE_ID_FIELD + '_right']].index,
         inplace=True, axis=0)
 
     node_group_status_list = []
     if join_df.empty:
         node_map_dict = dict()
         node_gdf = node_gdf.to_crs(origin_crs)
+        # 去除没有link连接的节点
+        drop_no_use_nodes(link_gdf, node_gdf)
         return link_gdf, node_gdf, gpd.GeoDataFrame()
     else:
         # 建立图
         g = nx.Graph()
         g.add_edges_from([(f, t) for f, t in zip(join_df[net_field.NODE_ID_FIELD + '_left'],
                                                  join_df[net_field.NODE_ID_FIELD + '_right'])])
 
@@ -438,9 +440,10 @@
             node_group_list = list(node_group)
             node_map_dict.update({origin_node: node_group_list[0] for origin_node in node_group_list[1:]})
 
 
 def drop_no_use_nodes(link_gdf: gpd.GeoDataFrame = None, node_gdf: gpd.GeoDataFrame = None):
     # 去除没有link连接的节点
     used_node = set(link_gdf[net_field.FROM_NODE_FIELD]) | set(link_gdf[net_field.TO_NODE_FIELD])
+    node_gdf.reset_index(inplace=True, drop=True)
     node_gdf.drop(index=node_gdf[~node_gdf[net_field.NODE_ID_FIELD].isin(used_node)].index, inplace=True, axis=1)
     node_gdf.reset_index(inplace=True, drop=True)
```

### Comparing `gotrackit-0.2.7/src/gotrackit/netreverse/RoadNet/Split/SplitPath.py` & `gotrackit-0.2.9/src/gotrackit/netreverse/RoadNet/Split/SplitPath.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.7/src/gotrackit/netreverse/RoadNet/Tools/process.py` & `gotrackit-0.2.9/src/gotrackit/netreverse/RoadNet/Tools/process.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.7/src/gotrackit/netreverse/RoadNet/conn.py` & `gotrackit-0.2.9/src/gotrackit/netreverse/RoadNet/conn.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,14 @@
         """"""
         # 遍历
         flag = 0
         if self.not_conn_df is None or self.not_conn_df.empty:
             return None
 
         for split_node, n_link_gdf in self.not_conn_df.groupby(node_id_field):
-            # print(split_node)
             if 'index_right' in n_link_gdf.columns:
                 n_link_gdf.drop(columns='index_right', axis=1, inplace=True)
             if split_node not in self.net.get_node_data()[node_id_field]:
                 continue
             if len(n_link_gdf) == 1:
                 target_link = n_link_gdf[link_id_field].to_list()[0]
                 if target_link in self.done_split_link.keys() and self.done_split_link[target_link] <= 1:
@@ -174,31 +173,34 @@
                                          val_list=[[split_node]])
                 self.net.renew_link_head_geo(link_list=[target_link_id])
             else:
                 to_del_node = self.net.get_link_from_to(target_link_id)[1]
                 self.net.modify_link_gdf(link_id_list=[target_link_id], attr_field_list=[to_node_field],
                                          val_list=[[split_node]])
                 self.net.renew_link_tail_geo(link_list=[target_link_id])
-            try:
-                self.net.del_nodes(node_list=[to_del_node])
-            except KeyError:
-                # this node has already been deleted
-                pass
+            # try:
+            #     print(rf'del {to_del_node}')
+            #     self.net.del_nodes(node_list=[to_del_node])
+            # except KeyError:
+            #     # this node has already been deleted
+            #     pass
 
         self.done_split_link[target_link_id] = 1
 
     def execute(self, out_fldr: str = None, file_name: str = 'space_bookmarks', generate_mark: bool = False,
                 link_name_field: str = 'road_name') -> \
             tuple[gpd.GeoDataFrame, gpd.GeoDataFrame]:
         # check the conn problem
         self.check(out_fldr=out_fldr, file_name=file_name, generate_mark=generate_mark)
 
         # modify conn problem
         self.corrective_conn()
 
+        self.net.check_ln_consistency()
+
         # drop dup road
         self.net.drop_dup_ft_road()
 
         # merger_double_link
         self.net.merger_double_link()
 
         link_gdf, node_gdf = self.net.get_bilateral_link_data(), self.net.get_node_data()
```

### Comparing `gotrackit-0.2.7/src/gotrackit/netreverse/RoadNet/increment.py` & `gotrackit-0.2.9/src/gotrackit/netreverse/RoadNet/increment.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.7/src/gotrackit/netreverse/RoadNet/net_reverse.py` & `gotrackit-0.2.9/src/gotrackit/netreverse/RoadNet/net_reverse.py`

 * *Files 5% similar despite different names*

```diff
@@ -114,15 +114,16 @@
     if modify_conn:
         if conn_period == 'start':
             print(rf'##########   {flag_name} - Repair Road Network Connectivity Before Topology Optimization')
             net = Net(link_gdf=link_gdf, node_gdf=new_node, create_single=False)
             conn = Conn(net=net, check_buffer=conn_buffer)
             # print(net.geo_crs, net.planar_crs)
             link_gdf, new_node = conn.execute(out_fldr=out_fldr, file_name=flag_name + '_conn', generate_mark=True)
-
+            # net.export_net(export_crs='EPSG:4326', out_fldr=out_fldr, file_type='shp',
+            #                flag_name='modifiedConn')
     # 5.拓扑优化
     print(rf'##########   {flag_name} - Topology Optimization')
     final_link, final_node, dup_info_dict = optimize_net.optimize(link_gdf=link_gdf, node_gdf=new_node,
                                                                   ignore_dir=False, limit_col_name=limit_col_name,
                                                                   save_preliminary=save_preliminary,
                                                                   out_fldr=out_fldr,
                                                                   plain_prj=plain_prj,
@@ -145,11 +146,14 @@
     if modify_conn:
         if conn_period == 'final':
             print(rf'##########   {flag_name} - Repair Road Network Connectivity After Topology Optimization')
             net = Net(link_gdf=final_link, node_gdf=final_node, create_single=False)
             # print(net.geo_crs, net.planar_crs)
             conn = Conn(net=net, check_buffer=conn_buffer)
             final_link, final_node = conn.execute(out_fldr=out_fldr, file_name=flag_name + '_conn', generate_mark=True)
-
+    try:
+        final_link.loc[final_link['road_name'] == '路口转向', 'dir'] = 0
+    except Exception as e:
+        pass
     save_file(data_item=final_link, out_fldr=out_fldr, file_name='FinalLink', file_type=net_file_type)
     save_file(data_item=final_node, out_fldr=out_fldr, file_name='FinalNode', file_type=net_file_type)
     generate_book_mark(name_loc_dict=dup_info_dict, prj_name=flag_name, input_fldr=out_fldr)
```

### Comparing `gotrackit-0.2.7/src/gotrackit/netreverse/RoadNet/optimize_net.py` & `gotrackit-0.2.9/src/gotrackit/netreverse/RoadNet/optimize_net.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.7/src/gotrackit/netreverse/RoadNet/save_file.py` & `gotrackit-0.2.9/src/gotrackit/netreverse/RoadNet/save_file.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.7/src/gotrackit/netreverse/book_mark.py` & `gotrackit-0.2.9/src/gotrackit/netreverse/book_mark.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.7/src/gotrackit/netreverse/format_od.py` & `gotrackit-0.2.9/src/gotrackit/netreverse/format_od.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.7/src/gotrackit/netxfer/SumoConvert.py` & `gotrackit-0.2.9/src/gotrackit/netxfer/SumoConvert.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.7/src/gotrackit/solver/Viterbi.py` & `gotrackit-0.2.9/src/gotrackit/solver/Viterbi.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.7/src/gotrackit/tools/coord_trans.py` & `gotrackit-0.2.9/src/gotrackit/tools/coord_trans.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.7/src/gotrackit/tools/geo_process.py` & `gotrackit-0.2.9/src/gotrackit/tools/geo_process.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,22 +98,28 @@
     将直线对象line进行n等分加密, 返回中间的加密点坐标
     :param s_loc
     :param e_loc
     :param n:
     :return:
     """
     # s, e = coord_list[0], coord_list[-1]
-    try:
-        k = (e_loc[1] - s_loc[1]) / (e_loc[0] - s_loc[0])
-    except ZeroDivisionError:
-        gap = np.abs(e_loc[1] - s_loc[1]) / n
+    # try:
+    #     k = (e_loc[1] - s_loc[1]) / (e_loc[0] - s_loc[0])
+    # except ZeroDivisionError:
+    #     gap = np.abs(e_loc[1] - s_loc[1]) / n
+    #     return [(s_loc[0], s_loc[1] + (i + 1) * gap) for i in range(n - 1)]
+    x_diff, y_diff = e_loc[0] - s_loc[0], e_loc[1] - s_loc[1]
+    if np.abs(x_diff) <= 1e-5:
+        gap = y_diff / n
         return [(s_loc[0], s_loc[1] + (i + 1) * gap) for i in range(n - 1)]
+    else:
+        k = y_diff / x_diff
 
     b = e_loc[1] - k * e_loc[0]
-    gap_x = (e_loc[0] - s_loc[0]) / n
+    gap_x = x_diff / n
     sample_x_list = [s_loc[0] + (i + 1) * gap_x for i in range(n - 1)]
     return [(sample_x, k * sample_x + b) for sample_x in sample_x_list]
 
 
 def prj_inf(p: Point = None, line: LineString = None) -> tuple[Point, float, float, float, list[LineString], float, float]:
     """
     # 返回 某point到line的(投影点坐标, 点到投影点的直线距离, 投影点到line拓扑起点的路径距离, line的长度, 投影点打断line后的geo list)
```

### Comparing `gotrackit-0.2.7/src/gotrackit/tools/group.py` & `gotrackit-0.2.9/src/gotrackit/tools/group.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.7/src/gotrackit/tools/save_file.py` & `gotrackit-0.2.9/src/gotrackit/tools/save_file.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.7/src/gotrackit/visualization.py` & `gotrackit-0.2.9/src/gotrackit/visualization.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.7/src/gotrackit.egg-info/PKG-INFO` & `gotrackit-0.2.9/src/gotrackit.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gotrackit
-Version: 0.2.7
+Version: 0.2.9
 Summary: A Python Package for Map Matching Algorithm Based on Hidden Markov Model
 Author-email: Kai Tang <794568794@qq.com>
 License: LICENCE
 Project-URL: Homepage, https://github.com/zdsjjtTLG/TrackIt
 Keywords: HMM,MapMatching,Net,Link,Node,Hidden Markov Model,Algorithm
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -16,83 +16,70 @@
 Requires-Dist: shapely
 Requires-Dist: networkx
 Requires-Dist: pandas
 Requires-Dist: numpy
 Requires-Dist: keplergl
 Requires-Dist: geopy
 
-
+**Read this in other languages: [Chinese](README.md) or [English](README_EN.md).**
 
 <div align="center">
     <img src="docs/_static/images/gotrackit.png" />
 </div>
 
 <br>
 
 <div align=center>
 
 [![Documentation Status](https://readthedocs.org/projects/gotrackit/badge/?version=latest)](https://gotrackit.readthedocs.io/en/latest/?badge=latest)
 ![PyPI - Version](https://img.shields.io/pypi/v/gotrackit)
 ![GitHub License](https://img.shields.io/github/license/zdsjjtTLG/Trackit)
+[![Downloads](https://static.pepy.tech/badge/gotrackit)](https://pepy.tech/project/gotrackit)
 ![PyPI - Downloads](https://img.shields.io/pypi/dw/gotrackit)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/gotrackit)
+![Static Badge](https://img.shields.io/badge/Model-HMM-9EC231)
+![Static Badge](https://img.shields.io/badge/Optimization-FastMapMatching-blue)
+![Static Badge](https://img.shields.io/badge/Optimization-MultiCoreParallelism-9EC231)
+![Github Created At](https://img.shields.io/github/created-at/zdsjjtTLG/Trackit)
+![GitHub last commit](https://img.shields.io/github/last-commit/zdsjjtTLG/Trackit)
 
-~ 一个包搞定：路网获取、路网优化、宏微观地图匹配、匹配可视化、问题路段快速定位 ~
-
-Developed by Tang Kai, Email: 794568794@qq.com & tangkai@zhechengdata.com
-</div>
-<br>
-
-
-**版本状态：05.19已更新: v0.2.6**
-
-更新命令：pip install --upgrade  -i https://pypi.org/simple/ gotrackit
-
-- 地图匹配接口效率优化, 相较于v0.2.4小幅度提升
+![GitHub User's stars](https://img.shields.io/github/stars/zdsjjtTLG)
+![GitHub forks](https://img.shields.io/github/forks/zdsjjtTLG/Trackit)
 
-- 新增网格参数搜索，帮助用户确定合理的匹配参数
+~ 💪一个包搞定：路网获取、路网优化、宏微观地图匹配、匹配可视化、问题路段快速定位💪 ~
 
-- BUG修复
+👻Developed by Tang Kai, Email: 794568794@qq.com & tangkai@zhechengdata.com👻
 
+🔑gotrackit迭代更新很快，记得关注版本更新信息哦🔑
 
-**不要下载GitHub仓库上的代码来使用!!!  直接pip安装gotrackit为第三方库即可使用**
-
+**❗❗❗不要下载GitHub仓库上的代码来使用!!!  直接pip安装gotrackit为第三方库即可使用❗❗❗**
 
+😆😁👉[gotrackit用户手册](https://gotrackit.readthedocs.io/en/latest/)👈😝😉
+</div>
 <br>
 
-<div align=center>
-~ v0.2.7(相较于0.2.1)效率将大幅度提升, 最高可以提升20倍的性能 !~
-</div>
 
-<br>
+**💬版本状态：06.03即将更新: v0.2.8**
 
-与上一版本对比:
+更新命令：pip install --upgrade  -i https://pypi.org/simple/ gotrackit
 
-| 样例数据           | 有效的GPS点数 | top_k(k邻近候选参数) | gps_buffer(临域半径) | 候选路段条数 | 状态转移次数  | v0.2.1版解算时间 | v0.2.7版解算时间 |
-|----------------|----------|----------------|------------------|---------|------------|-------------|-------------|
-| 1辆车,深圳稀疏轨迹点样例1 | 190      | 60             | 500m             | 10615 | 629788次 | 28秒         | **1.35秒**   |
-| 1辆车,深圳稀疏轨迹点样例2 | 400      | 20             | 120m             | 5137 | 82006次  | 7.8秒        | **0.60秒**   |
+- 样例GPS生成模块：接口简化、BUG修复
 
+- 基于GPS生产OD的接口：效率优化
 
-v0.2.7多核效率对比:
+- 上线GPS行程切分接口
 
-基于上表深圳稀疏轨迹点样例2，我们将他复制150份，进行多核测试，可以看到到6核时, 效率已经不再提升，最快71s解算完150条轨迹，平均每条轨迹0.47s，相较于0.60s再次提升了20%，在车辆数较多时，多核的效率提升很明显。
+- 路网请求模块，Key配额提示优化，动态停用已超配额的Key
 
-| 样例数据                                      | 有效的GPS点数 | top_k | gps_buffer | 候选路段条数 | 状态转移次数 | v0.2.7解算时间 |
-|-------------------------------------------|----------|----------------|------------------|-----|--------|------------|
-| 150辆车的GPS轨迹(单核串行,子图搜索,有构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 226.0秒     | 
-| 150辆车的GPS轨迹(3核并行,子图搜索,有构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 101.6秒     |
-| 150辆车的GPS轨迹(3核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 88.3秒      |
-| 150辆车的GPS轨迹(4核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 75.3秒      | 
-| 150辆车的GPS轨迹(5核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 72.1秒      | 
-| 150辆车的GPS轨迹(6核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 71.5秒      | 
+- 地图匹配接口BUG修复(极小概率BUG、但是影响较大)、路网生产模块BUG修复
 
 
 <br>
 
+
 <div align=center>
 ~ 稀疏轨迹匹配与路径补全 ~
 </div>
 
 <br>
 
 深圳稀疏轨迹点样例1：
@@ -143,28 +130,34 @@
     <img src="docs/_static/images/wxq.jpg" />
 </div>
 
 
 ## 1. 简介
 本地图匹配包基于隐马尔可夫模型(HMM)实现了连续GPS点位的概率建模，利用这个包可以轻松对GPS数据进行地图匹配，本开源包的特点如下:
 
-**数据无忧**
-- 提供路网生产模块以及路网优化接口，您不需要准备任何路网和GPS数据即可玩转地图匹配；
+**😻数据无忧**
+- 提供路网生产模块以及大量路网处理优化工具，您不需要准备任何路网和GPS数据即可玩转地图匹配；
 - 提供GPS样例数据生产模块，解决没有GPS数据的难题；
-- 提供GPS数据清洗接口，包括滑动窗口降噪、数据降频。
+- 提供GPS数据清洗接口，包括行程切分、滑动窗口降噪、数据降频、停留点识别、点位增密。
 
-**文档齐全**
 
+**☑️文档齐全**
 - 中文文档，有详细的操作指引；
 - 算法原理讲解部分不涉及复杂的公式推导，使用动画形式剖析算法原理,简洁明了。
 
-**匹配结果自动优化**
+
+**🚀匹配算法优化**
+- 支持基于路径预存储的FastMapMatching、支持多核并行匹配、支持网格参数搜索；
 - 对基于HMM匹配的初步路径进行了优化，对于不连通的位置会自动搜路补全，对于实际路网不连通的位置会输出警告信息，方便用户回溯问题。
 
 
+**🌈匹配结果支持动画可视化**
+- 匹配结果提供三种输出形式：GPS点匹配结果表(csv)、匹配结果矢量化图层、矢量图层匹配动画(HTML文件)，HTML动画方便用户直观地感受匹配结果，同时可以提高问题排查的效率。
+
+
 
 ### 1.1. 如何安装gotrackit
 
 #### __所需前置依赖__
 
 - geopy(2.4.1)
 - gdal(3.4.3)
@@ -188,25 +181,40 @@
 ```
 
 更新：
 ``` shell
 pip install --upgrade  -i https://pypi.org/simple/ gotrackit
 ```
 
-### 1.2 用户手册与视频教程
+### 1.2 如何使用gotrackit
+
+- [用户手册](https://gotrackit.readthedocs.io/en/latest/)
+
+- [基于隐马尔可夫模型(HMM)的地图匹配算法动画版！学不会你来打我！](https://www.bilibili.com/video/BV1gQ4y1w7dC)
 
-[用户手册](https://gotrackit.readthedocs.io/en/latest/)
+- [一个python包搞定路网获取+地图匹配！](https://www.bilibili.com/video/BV1nC411z7Vg)
 
-[基于隐马尔可夫模型(HMM)的地图匹配算法动画版！学不会你来打我！](https://www.bilibili.com/video/BV1gQ4y1w7dC)
+- [gotrackit地图匹配包参数详解与问题排查](https://www.bilibili.com/video/BV1qK421Y7hV)
+
+- [QGIS路网拓扑显示、底图加载、样式复用、map保存](https://www.bilibili.com/video/BV1Sq421F7QX)
+
+
+### 1.3. 如何引用gotrackit
+
+如果你想在文章中引用gotrackit，请附上以下链接：
+
+``` shell
+https://github.com/zdsjjtTLG/TrackIt
+```
 
-[一个python包搞定路网获取+地图匹配！](https://www.bilibili.com/video/BV1nC411z7Vg)
+### 1.4. BUG提交
 
-[gotrackit地图匹配包参数详解与问题排查](https://www.bilibili.com/video/BV1qK421Y7hV)
+如果确定是BUG，请提交在以下页面：
 
-[QGIS路网拓扑显示、底图加载、样式复用、map保存](https://www.bilibili.com/video/BV1Sq421F7QX)
+[BUG提交页面](https://github.com/zdsjjtTLG/TrackIt/issues)
 
 
 ## 2. 地图匹配问题
 
 ![car_gps.png](docs/_static/images/car_gps.png)
 
 ![where_car.png](docs/_static/images/whereIsCar.png)
```

### Comparing `gotrackit-0.2.7/src/gotrackit.egg-info/SOURCES.txt` & `gotrackit-0.2.9/src/gotrackit.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 src/gotrackit/visualization.py
 src/gotrackit.egg-info/PKG-INFO
 src/gotrackit.egg-info/SOURCES.txt
 src/gotrackit.egg-info/dependency_links.txt
 src/gotrackit.egg-info/requires.txt
 src/gotrackit.egg-info/top_level.txt
 src/gotrackit/generation/GpsGen.py
+src/gotrackit/generation/SampleTrip.py
 src/gotrackit/generation/__init__.py
 src/gotrackit/gps/GpsArray.py
 src/gotrackit/gps/GpsTrip.py
 src/gotrackit/gps/GpsXfer.py
 src/gotrackit/gps/LocGps.py
 src/gotrackit/gps/__init__.py
 src/gotrackit/map/Link.py
```

