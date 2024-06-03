# Comparing `tmp/tui_dsmt-202406030834.tar.gz` & `tmp/tui_dsmt-202406031350.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tui_dsmt-202406030834.tar", last modified: Mon Jun  3 08:34:10 2024, max compression
+gzip compressed data, was "tui_dsmt-202406031350.tar", last modified: Mon Jun  3 13:50:23 2024, max compression
```

## Comparing `tui_dsmt-202406030834.tar` & `tui_dsmt-202406031350.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 08:34:10.642183 tui_dsmt-202406030834/
--rw-r--r--   0 root         (0) root         (0)      897 2024-06-03 08:34:10.642183 tui_dsmt-202406030834/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2024-06-03 08:34:10.642183 tui_dsmt-202406030834/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1355 2024-06-01 15:59:19.000000 tui_dsmt-202406030834/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 08:34:10.618183 tui_dsmt-202406030834/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 08:34:10.618183 tui_dsmt-202406030834/src/tui_dsmt/
--rw-rw-rw-   0 root         (0) root         (0)     1115 2024-06-01 16:21:07.000000 tui_dsmt-202406030834/src/tui_dsmt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 08:34:10.622183 tui_dsmt-202406030834/src/tui_dsmt/clustering/
--rw-rw-rw-   0 root         (0) root         (0)     5223 2024-05-18 09:15:33.000000 tui_dsmt-202406030834/src/tui_dsmt/clustering/PAM.py
--rw-rw-rw-   0 root         (0) root         (0)      309 2024-05-18 09:15:33.000000 tui_dsmt-202406030834/src/tui_dsmt/clustering/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2691 2024-05-18 09:15:33.000000 tui_dsmt-202406030834/src/tui_dsmt/clustering/animation.py
--rw-rw-rw-   0 root         (0) root         (0)    19467 2024-05-18 09:15:33.000000 tui_dsmt-202406030834/src/tui_dsmt/clustering/datasets.py
--rw-rw-rw-   0 root         (0) root         (0)      260 2024-05-18 09:15:33.000000 tui_dsmt-202406030834/src/tui_dsmt/clustering/draw.py
--rw-rw-rw-   0 root         (0) root         (0)     2141 2024-05-18 09:15:33.000000 tui_dsmt-202406030834/src/tui_dsmt/clustering/evaluation.py
--rw-rw-rw-   0 root         (0) root         (0)     4488 2024-05-18 09:15:33.000000 tui_dsmt-202406030834/src/tui_dsmt/clustering/hierarchical.py
--rw-rw-rw-   0 root         (0) root         (0)      945 2024-05-18 09:15:33.000000 tui_dsmt-202406030834/src/tui_dsmt/clustering/interactive.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 08:34:10.622183 tui_dsmt-202406030834/src/tui_dsmt/fpm/
--rw-rw-rw-   0 root         (0) root         (0)    14098 2024-05-18 09:15:33.000000 tui_dsmt-202406030834/src/tui_dsmt/fpm/BruteForceFI.py
--rw-rw-rw-   0 root         (0) root         (0)     4055 2024-05-18 09:15:33.000000 tui_dsmt-202406030834/src/tui_dsmt/fpm/ConditionalFPTree.py
--rw-rw-rw-   0 root         (0) root         (0)     5936 2024-06-01 15:59:19.000000 tui_dsmt-202406030834/src/tui_dsmt/fpm/ConditionalPatternBase.py
--rw-rw-rw-   0 root         (0) root         (0)    11873 2024-06-01 15:59:19.000000 tui_dsmt-202406030834/src/tui_dsmt/fpm/FPTree.py
--rw-rw-rw-   0 root         (0) root         (0)    19208 2024-06-01 15:59:19.000000 tui_dsmt-202406030834/src/tui_dsmt/fpm/HashTree.py
--rw-rw-rw-   0 root         (0) root         (0)     1462 2024-05-18 09:15:33.000000 tui_dsmt-202406030834/src/tui_dsmt/fpm/Itemset.py
--rw-rw-rw-   0 root         (0) root         (0)     3036 2024-05-18 09:15:33.000000 tui_dsmt-202406030834/src/tui_dsmt/fpm/ItemsetGrid.py
--rw-rw-rw-   0 root         (0) root         (0)     5942 2024-05-18 09:15:33.000000 tui_dsmt-202406030834/src/tui_dsmt/fpm/ItemsetGridApriori.py
--rw-rw-rw-   0 root         (0) root         (0)     5865 2024-05-18 09:15:33.000000 tui_dsmt-202406030834/src/tui_dsmt/fpm/ItemsetGridECLAT.py
--rw-rw-rw-   0 root         (0) root         (0)     1309 2024-05-18 09:15:33.000000 tui_dsmt-202406030834/src/tui_dsmt/fpm/SequentialDatabase.py
--rw-rw-rw-   0 root         (0) root         (0)     1139 2024-06-01 15:59:19.000000 tui_dsmt-202406030834/src/tui_dsmt/fpm/SequentialItemset.py
--rw-rw-rw-   0 root         (0) root         (0)     1181 2024-05-18 09:15:33.000000 tui_dsmt-202406030834/src/tui_dsmt/fpm/TransactionDatabase.py
--rw-rw-rw-   0 root         (0) root         (0)     2691 2024-06-01 15:59:19.000000 tui_dsmt-202406030834/src/tui_dsmt/fpm/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1067 2024-06-01 15:59:19.000000 tui_dsmt-202406030834/src/tui_dsmt/fpm/datasets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 08:34:10.622183 tui_dsmt-202406030834/src/tui_dsmt/fpm/resources/
--rw-rw-rw-   0 root         (0) root         (0)    52516 2024-06-01 15:59:19.000000 tui_dsmt-202406030834/src/tui_dsmt/fpm/resources/website_tracking.csv
--rw-rw-rw-   0 root         (0) root         (0)   125202 2024-06-01 15:59:19.000000 tui_dsmt-202406030834/src/tui_dsmt/fpm/resources/website_tracking2.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 08:34:10.626183 tui_dsmt-202406030834/src/tui_dsmt/graph/
--rw-rw-rw-   0 root         (0) root         (0)     3894 2024-05-18 09:15:33.000000 tui_dsmt-202406030834/src/tui_dsmt/graph/BFS.py
--rw-rw-rw-   0 root         (0) root         (0)     1585 2024-05-18 09:15:33.000000 tui_dsmt-202406030834/src/tui_dsmt/graph/BipartiteFlow.py
--rw-rw-rw-   0 root         (0) root         (0)     3038 2024-06-01 15:59:19.000000 tui_dsmt-202406030834/src/tui_dsmt/graph/BronKerbosch.py
--rw-rw-rw-   0 root         (0) root         (0)     3478 2024-05-18 09:15:33.000000 tui_dsmt-202406030834/src/tui_dsmt/graph/DFS.py
--rw-rw-rw-   0 root         (0) root         (0)     5843 2024-05-18 09:15:33.000000 tui_dsmt-202406030834/src/tui_dsmt/graph/Dijkstra.py
--rw-rw-rw-   0 root         (0) root         (0)      175 2024-05-18 09:15:33.000000 tui_dsmt-202406030834/src/tui_dsmt/graph/EdmondsKarp.py
--rw-rw-rw-   0 root         (0) root         (0)     4747 2024-05-18 09:15:33.000000 tui_dsmt-202406030834/src/tui_dsmt/graph/FordFulkerson.py
--rw-rw-rw-   0 root         (0) root         (0)     4860 2024-05-18 09:15:33.000000 tui_dsmt-202406030834/src/tui_dsmt/graph/FruchtermanReingold.py
--rw-rw-rw-   0 root         (0) root         (0)     4461 2024-05-18 09:15:33.000000 tui_dsmt-202406030834/src/tui_dsmt/graph/Hall.py
--rw-rw-rw-   0 root         (0) root         (0)     2095 2024-05-18 09:15:33.000000 tui_dsmt-202406030834/src/tui_dsmt/graph/InteractiveGraph.py
--rw-rw-rw-   0 root         (0) root         (0)     3142 2024-05-18 09:15:33.000000 tui_dsmt-202406030834/src/tui_dsmt/graph/Kruskal.py
--rw-rw-rw-   0 root         (0) root         (0)     4877 2024-05-18 09:15:33.000000 tui_dsmt-202406030834/src/tui_dsmt/graph/LabelPropagation.py
--rw-rw-rw-   0 root         (0) root         (0)       39 2024-05-18 09:15:33.000000 tui_dsmt-202406030834/src/tui_dsmt/graph/MarkovClusterAlgorithm.py
--rw-rw-rw-   0 root         (0) root         (0)     2234 2024-05-18 09:15:33.000000 tui_dsmt-202406030834/src/tui_dsmt/graph/MaximumFlow.py
--rw-rw-rw-   0 root         (0) root         (0)     2705 2024-05-18 09:15:33.000000 tui_dsmt-202406030834/src/tui_dsmt/graph/RandomWalk.py
--rw-rw-rw-   0 root         (0) root         (0)      684 2024-06-01 19:03:19.000000 tui_dsmt-202406030834/src/tui_dsmt/graph/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6462 2024-06-01 19:03:19.000000 tui_dsmt-202406030834/src/tui_dsmt/graph/datasets.py
--rw-rw-rw-   0 root         (0) root         (0)     5307 2024-06-01 19:11:59.000000 tui_dsmt-202406030834/src/tui_dsmt/graph/game.py
--rw-rw-rw-   0 root         (0) root         (0)     6426 2024-05-18 09:15:33.000000 tui_dsmt-202406030834/src/tui_dsmt/graph/html.py
--rw-rw-rw-   0 root         (0) root         (0)      870 2024-05-18 09:15:33.000000 tui_dsmt-202406030834/src/tui_dsmt/graph/representation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 08:34:10.638183 tui_dsmt-202406030834/src/tui_dsmt/graph/resources/
--rw-rw-rw-   0 root         (0) root         (0)      300 2024-06-01 19:03:19.000000 tui_dsmt-202406030834/src/tui_dsmt/graph/resources/bi_flow.csv
--rw-rw-rw-   0 root         (0) root         (0)       28 2024-06-01 19:03:19.000000 tui_dsmt-202406030834/src/tui_dsmt/graph/resources/bi_small.csv
--rw-rw-rw-   0 root         (0) root         (0)     2807 2024-06-01 19:03:19.000000 tui_dsmt-202406030834/src/tui_dsmt/graph/resources/bipartite_exams.csv
--rw-rw-rw-   0 root         (0) root         (0)       60 2024-06-01 19:03:19.000000 tui_dsmt-202406030834/src/tui_dsmt/graph/resources/cliques_small.csv
--rw-rw-rw-   0 root         (0) root         (0)       99 2024-06-01 19:03:19.000000 tui_dsmt-202406030834/src/tui_dsmt/graph/resources/community_small.csv
--rw-rw-rw-   0 root         (0) root         (0)       28 2024-06-01 19:03:19.000000 tui_dsmt-202406030834/src/tui_dsmt/graph/resources/community_tiny.csv
--rw-rw-rw-   0 root         (0) root         (0)      306 2024-06-01 19:03:19.000000 tui_dsmt-202406030834/src/tui_dsmt/graph/resources/dach_cities.csv
--rw-rw-rw-   0 root         (0) root         (0)  8978701 2024-05-18 09:15:33.000000 tui_dsmt-202406030834/src/tui_dsmt/graph/resources/dewiki_sample.pickle.bz2
--rw-rw-rw-   0 root         (0) root         (0)      100 2024-06-01 19:03:19.000000 tui_dsmt-202406030834/src/tui_dsmt/graph/resources/mf_ex1.csv
--rw-rw-rw-   0 root         (0) root         (0)      108 2024-06-01 19:03:19.000000 tui_dsmt-202406030834/src/tui_dsmt/graph/resources/mf_ex2.csv
--rw-rw-rw-   0 root         (0) root         (0)       60 2024-06-01 16:21:07.000000 tui_dsmt-202406030834/src/tui_dsmt/graph/resources/multiprocessing_small.csv
--rw-rw-rw-   0 root         (0) root         (0)      399 2024-06-01 16:21:07.000000 tui_dsmt-202406030834/src/tui_dsmt/graph/resources/multiprocessing_small_pos.json
--rw-rw-rw-   0 root         (0) root         (0)       60 2024-06-01 16:21:07.000000 tui_dsmt-202406030834/src/tui_dsmt/graph/resources/multiprocessing_small_weights.csv
--rw-rw-rw-   0 root         (0) root         (0)     1115 2024-06-01 19:03:19.000000 tui_dsmt-202406030834/src/tui_dsmt/graph/resources/tw.csv
--rw-rw-rw-   0 root         (0) root         (0)     1272 2024-06-01 19:03:19.000000 tui_dsmt-202406030834/src/tui_dsmt/graph/resources/tw_pos.json
--rw-rw-rw-   0 root         (0) root         (0)   229164 2024-06-01 19:03:19.000000 tui_dsmt-202406030834/src/tui_dsmt/graph/resources/wiki_it.tsv
--rw-rw-rw-   0 root         (0) root         (0)    57082 2024-06-01 19:03:19.000000 tui_dsmt-202406030834/src/tui_dsmt/graph/resources/wiki_it_pos.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 08:34:10.638183 tui_dsmt-202406030834/src/tui_dsmt/jpanim/
--rw-rw-rw-   0 root         (0) root         (0)     2935 2024-05-18 09:15:33.000000 tui_dsmt-202406030834/src/tui_dsmt/jpanim/JupyterAnimation.py
--rw-rw-rw-   0 root         (0) root         (0)       47 2024-05-18 09:15:33.000000 tui_dsmt-202406030834/src/tui_dsmt/jpanim/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 08:34:10.638183 tui_dsmt-202406030834/src/tui_dsmt/jpanim/resources/
--rw-rw-rw-   0 root         (0) root         (0)     2002 2024-05-18 09:15:33.000000 tui_dsmt-202406030834/src/tui_dsmt/jpanim/resources/controls-ff.html
--rw-rw-rw-   0 root         (0) root         (0)      797 2024-05-18 09:15:33.000000 tui_dsmt-202406030834/src/tui_dsmt/jpanim/resources/controls.html
--rw-rw-rw-   0 root         (0) root         (0)      743 2024-05-18 09:15:33.000000 tui_dsmt-202406030834/src/tui_dsmt/jpanim/resources/script.js
--rw-rw-rw-   0 root         (0) root         (0)      193 2024-05-18 09:15:33.000000 tui_dsmt-202406030834/src/tui_dsmt/jpanim/resources/style.css
--rw-rw-rw-   0 root         (0) root         (0)   147897 2024-05-18 09:15:33.000000 tui_dsmt-202406030834/src/tui_dsmt/jpanim/resources/vue-3.4.24.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 08:34:10.642183 tui_dsmt-202406030834/src/tui_dsmt/util/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-18 09:15:33.000000 tui_dsmt-202406030834/src/tui_dsmt/util/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 08:34:10.642183 tui_dsmt-202406030834/src/tui_dsmt.egg-info/
--rw-r--r--   0 root         (0) root         (0)      897 2024-06-03 08:34:10.000000 tui_dsmt-202406030834/src/tui_dsmt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2860 2024-06-03 08:34:10.000000 tui_dsmt-202406030834/src/tui_dsmt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-06-03 08:34:10.000000 tui_dsmt-202406030834/src/tui_dsmt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      194 2024-06-03 08:34:10.000000 tui_dsmt-202406030834/src/tui_dsmt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-06-03 08:34:10.000000 tui_dsmt-202406030834/src/tui_dsmt.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:50:23.368699 tui_dsmt-202406031350/
+-rw-r--r--   0 root         (0) root         (0)      897 2024-06-03 13:50:23.368699 tui_dsmt-202406031350/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2024-06-03 13:50:23.368699 tui_dsmt-202406031350/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1355 2024-06-01 15:59:04.000000 tui_dsmt-202406031350/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:50:23.324699 tui_dsmt-202406031350/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:50:23.324699 tui_dsmt-202406031350/src/tui_dsmt/
+-rw-rw-rw-   0 root         (0) root         (0)     1115 2024-06-01 16:20:05.000000 tui_dsmt-202406031350/src/tui_dsmt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:50:23.328698 tui_dsmt-202406031350/src/tui_dsmt/clustering/
+-rw-rw-rw-   0 root         (0) root         (0)     5223 2024-05-18 09:14:58.000000 tui_dsmt-202406031350/src/tui_dsmt/clustering/PAM.py
+-rw-rw-rw-   0 root         (0) root         (0)      309 2024-05-18 09:14:58.000000 tui_dsmt-202406031350/src/tui_dsmt/clustering/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2691 2024-05-18 09:14:58.000000 tui_dsmt-202406031350/src/tui_dsmt/clustering/animation.py
+-rw-rw-rw-   0 root         (0) root         (0)    19467 2024-05-18 09:14:58.000000 tui_dsmt-202406031350/src/tui_dsmt/clustering/datasets.py
+-rw-rw-rw-   0 root         (0) root         (0)      260 2024-05-18 09:14:58.000000 tui_dsmt-202406031350/src/tui_dsmt/clustering/draw.py
+-rw-rw-rw-   0 root         (0) root         (0)     2141 2024-05-18 09:14:58.000000 tui_dsmt-202406031350/src/tui_dsmt/clustering/evaluation.py
+-rw-rw-rw-   0 root         (0) root         (0)     4488 2024-05-18 09:14:58.000000 tui_dsmt-202406031350/src/tui_dsmt/clustering/hierarchical.py
+-rw-rw-rw-   0 root         (0) root         (0)      945 2024-05-18 09:14:58.000000 tui_dsmt-202406031350/src/tui_dsmt/clustering/interactive.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:50:23.332698 tui_dsmt-202406031350/src/tui_dsmt/fpm/
+-rw-rw-rw-   0 root         (0) root         (0)    14098 2024-05-18 09:14:58.000000 tui_dsmt-202406031350/src/tui_dsmt/fpm/BruteForceFI.py
+-rw-rw-rw-   0 root         (0) root         (0)     4055 2024-05-18 09:14:58.000000 tui_dsmt-202406031350/src/tui_dsmt/fpm/ConditionalFPTree.py
+-rw-rw-rw-   0 root         (0) root         (0)     5936 2024-06-01 15:59:04.000000 tui_dsmt-202406031350/src/tui_dsmt/fpm/ConditionalPatternBase.py
+-rw-rw-rw-   0 root         (0) root         (0)    11873 2024-06-01 15:59:04.000000 tui_dsmt-202406031350/src/tui_dsmt/fpm/FPTree.py
+-rw-rw-rw-   0 root         (0) root         (0)    19208 2024-06-01 15:59:04.000000 tui_dsmt-202406031350/src/tui_dsmt/fpm/HashTree.py
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2024-05-18 09:14:58.000000 tui_dsmt-202406031350/src/tui_dsmt/fpm/Itemset.py
+-rw-rw-rw-   0 root         (0) root         (0)     3036 2024-05-18 09:14:58.000000 tui_dsmt-202406031350/src/tui_dsmt/fpm/ItemsetGrid.py
+-rw-rw-rw-   0 root         (0) root         (0)     5942 2024-05-18 09:14:58.000000 tui_dsmt-202406031350/src/tui_dsmt/fpm/ItemsetGridApriori.py
+-rw-rw-rw-   0 root         (0) root         (0)     5865 2024-05-18 09:14:58.000000 tui_dsmt-202406031350/src/tui_dsmt/fpm/ItemsetGridECLAT.py
+-rw-rw-rw-   0 root         (0) root         (0)     1309 2024-05-18 09:14:58.000000 tui_dsmt-202406031350/src/tui_dsmt/fpm/SequentialDatabase.py
+-rw-rw-rw-   0 root         (0) root         (0)     1139 2024-06-01 15:59:04.000000 tui_dsmt-202406031350/src/tui_dsmt/fpm/SequentialItemset.py
+-rw-rw-rw-   0 root         (0) root         (0)     1181 2024-05-18 09:14:58.000000 tui_dsmt-202406031350/src/tui_dsmt/fpm/TransactionDatabase.py
+-rw-rw-rw-   0 root         (0) root         (0)     2691 2024-06-01 15:59:04.000000 tui_dsmt-202406031350/src/tui_dsmt/fpm/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1067 2024-06-01 15:59:04.000000 tui_dsmt-202406031350/src/tui_dsmt/fpm/datasets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:50:23.332698 tui_dsmt-202406031350/src/tui_dsmt/fpm/resources/
+-rw-rw-rw-   0 root         (0) root         (0)    52516 2024-06-01 15:59:04.000000 tui_dsmt-202406031350/src/tui_dsmt/fpm/resources/website_tracking.csv
+-rw-rw-rw-   0 root         (0) root         (0)   125202 2024-06-01 15:59:04.000000 tui_dsmt-202406031350/src/tui_dsmt/fpm/resources/website_tracking2.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:50:23.340699 tui_dsmt-202406031350/src/tui_dsmt/graph/
+-rw-rw-rw-   0 root         (0) root         (0)     3894 2024-05-18 09:14:58.000000 tui_dsmt-202406031350/src/tui_dsmt/graph/BFS.py
+-rw-rw-rw-   0 root         (0) root         (0)     1585 2024-05-18 09:14:58.000000 tui_dsmt-202406031350/src/tui_dsmt/graph/BipartiteFlow.py
+-rw-rw-rw-   0 root         (0) root         (0)     3038 2024-06-01 15:59:04.000000 tui_dsmt-202406031350/src/tui_dsmt/graph/BronKerbosch.py
+-rw-rw-rw-   0 root         (0) root         (0)     3478 2024-05-18 09:14:58.000000 tui_dsmt-202406031350/src/tui_dsmt/graph/DFS.py
+-rw-rw-rw-   0 root         (0) root         (0)     5843 2024-05-18 09:14:58.000000 tui_dsmt-202406031350/src/tui_dsmt/graph/Dijkstra.py
+-rw-rw-rw-   0 root         (0) root         (0)      175 2024-05-18 09:14:58.000000 tui_dsmt-202406031350/src/tui_dsmt/graph/EdmondsKarp.py
+-rw-rw-rw-   0 root         (0) root         (0)     4747 2024-05-18 09:14:58.000000 tui_dsmt-202406031350/src/tui_dsmt/graph/FordFulkerson.py
+-rw-rw-rw-   0 root         (0) root         (0)     4860 2024-05-18 09:14:58.000000 tui_dsmt-202406031350/src/tui_dsmt/graph/FruchtermanReingold.py
+-rw-rw-rw-   0 root         (0) root         (0)     4461 2024-05-18 09:14:58.000000 tui_dsmt-202406031350/src/tui_dsmt/graph/Hall.py
+-rw-rw-rw-   0 root         (0) root         (0)     2095 2024-05-18 09:14:58.000000 tui_dsmt-202406031350/src/tui_dsmt/graph/InteractiveGraph.py
+-rw-rw-rw-   0 root         (0) root         (0)     3142 2024-05-18 09:14:58.000000 tui_dsmt-202406031350/src/tui_dsmt/graph/Kruskal.py
+-rw-rw-rw-   0 root         (0) root         (0)     4877 2024-05-18 09:14:58.000000 tui_dsmt-202406031350/src/tui_dsmt/graph/LabelPropagation.py
+-rw-rw-rw-   0 root         (0) root         (0)       39 2024-05-18 09:14:58.000000 tui_dsmt-202406031350/src/tui_dsmt/graph/MarkovClusterAlgorithm.py
+-rw-rw-rw-   0 root         (0) root         (0)     2234 2024-05-18 09:14:58.000000 tui_dsmt-202406031350/src/tui_dsmt/graph/MaximumFlow.py
+-rw-rw-rw-   0 root         (0) root         (0)     2705 2024-05-18 09:14:58.000000 tui_dsmt-202406031350/src/tui_dsmt/graph/RandomWalk.py
+-rw-rw-rw-   0 root         (0) root         (0)      684 2024-06-01 19:03:19.000000 tui_dsmt-202406031350/src/tui_dsmt/graph/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6462 2024-06-01 19:03:19.000000 tui_dsmt-202406031350/src/tui_dsmt/graph/datasets.py
+-rw-rw-rw-   0 root         (0) root         (0)     5307 2024-06-01 19:11:59.000000 tui_dsmt-202406031350/src/tui_dsmt/graph/game.py
+-rw-rw-rw-   0 root         (0) root         (0)     6426 2024-05-18 09:14:58.000000 tui_dsmt-202406031350/src/tui_dsmt/graph/html.py
+-rw-rw-rw-   0 root         (0) root         (0)      870 2024-05-18 09:14:58.000000 tui_dsmt-202406031350/src/tui_dsmt/graph/representation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:50:23.364699 tui_dsmt-202406031350/src/tui_dsmt/graph/resources/
+-rw-rw-rw-   0 root         (0) root         (0)      300 2024-06-01 19:03:19.000000 tui_dsmt-202406031350/src/tui_dsmt/graph/resources/bi_flow.csv
+-rw-rw-rw-   0 root         (0) root         (0)       28 2024-06-01 19:03:19.000000 tui_dsmt-202406031350/src/tui_dsmt/graph/resources/bi_small.csv
+-rw-rw-rw-   0 root         (0) root         (0)     2807 2024-06-01 19:03:19.000000 tui_dsmt-202406031350/src/tui_dsmt/graph/resources/bipartite_exams.csv
+-rw-rw-rw-   0 root         (0) root         (0)       60 2024-06-01 19:03:19.000000 tui_dsmt-202406031350/src/tui_dsmt/graph/resources/cliques_small.csv
+-rw-rw-rw-   0 root         (0) root         (0)       99 2024-06-01 19:03:19.000000 tui_dsmt-202406031350/src/tui_dsmt/graph/resources/community_small.csv
+-rw-rw-rw-   0 root         (0) root         (0)       28 2024-06-01 19:03:19.000000 tui_dsmt-202406031350/src/tui_dsmt/graph/resources/community_tiny.csv
+-rw-rw-rw-   0 root         (0) root         (0)      306 2024-06-01 19:03:19.000000 tui_dsmt-202406031350/src/tui_dsmt/graph/resources/dach_cities.csv
+-rw-rw-rw-   0 root         (0) root         (0)  8978701 2024-05-18 09:14:58.000000 tui_dsmt-202406031350/src/tui_dsmt/graph/resources/dewiki_sample.pickle.bz2
+-rw-rw-rw-   0 root         (0) root         (0)      100 2024-06-01 19:03:19.000000 tui_dsmt-202406031350/src/tui_dsmt/graph/resources/mf_ex1.csv
+-rw-rw-rw-   0 root         (0) root         (0)      108 2024-06-01 19:03:19.000000 tui_dsmt-202406031350/src/tui_dsmt/graph/resources/mf_ex2.csv
+-rw-rw-rw-   0 root         (0) root         (0)       60 2024-06-01 16:20:05.000000 tui_dsmt-202406031350/src/tui_dsmt/graph/resources/multiprocessing_small.csv
+-rw-rw-rw-   0 root         (0) root         (0)      399 2024-06-01 16:20:05.000000 tui_dsmt-202406031350/src/tui_dsmt/graph/resources/multiprocessing_small_pos.json
+-rw-rw-rw-   0 root         (0) root         (0)       60 2024-06-01 16:20:05.000000 tui_dsmt-202406031350/src/tui_dsmt/graph/resources/multiprocessing_small_weights.csv
+-rw-rw-rw-   0 root         (0) root         (0)     1115 2024-06-01 19:03:19.000000 tui_dsmt-202406031350/src/tui_dsmt/graph/resources/tw.csv
+-rw-rw-rw-   0 root         (0) root         (0)     1272 2024-06-01 19:03:19.000000 tui_dsmt-202406031350/src/tui_dsmt/graph/resources/tw_pos.json
+-rw-rw-rw-   0 root         (0) root         (0)   229164 2024-06-01 19:03:19.000000 tui_dsmt-202406031350/src/tui_dsmt/graph/resources/wiki_it.tsv
+-rw-rw-rw-   0 root         (0) root         (0)    57082 2024-06-01 19:03:19.000000 tui_dsmt-202406031350/src/tui_dsmt/graph/resources/wiki_it_pos.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:50:23.364699 tui_dsmt-202406031350/src/tui_dsmt/jpanim/
+-rw-rw-rw-   0 root         (0) root         (0)     2935 2024-05-18 09:14:58.000000 tui_dsmt-202406031350/src/tui_dsmt/jpanim/JupyterAnimation.py
+-rw-rw-rw-   0 root         (0) root         (0)       47 2024-05-18 09:14:58.000000 tui_dsmt-202406031350/src/tui_dsmt/jpanim/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:50:23.364699 tui_dsmt-202406031350/src/tui_dsmt/jpanim/resources/
+-rw-rw-rw-   0 root         (0) root         (0)     2002 2024-05-18 09:14:58.000000 tui_dsmt-202406031350/src/tui_dsmt/jpanim/resources/controls-ff.html
+-rw-rw-rw-   0 root         (0) root         (0)      797 2024-05-18 09:14:58.000000 tui_dsmt-202406031350/src/tui_dsmt/jpanim/resources/controls.html
+-rw-rw-rw-   0 root         (0) root         (0)      743 2024-05-18 09:14:58.000000 tui_dsmt-202406031350/src/tui_dsmt/jpanim/resources/script.js
+-rw-rw-rw-   0 root         (0) root         (0)      193 2024-05-18 09:14:58.000000 tui_dsmt-202406031350/src/tui_dsmt/jpanim/resources/style.css
+-rw-rw-rw-   0 root         (0) root         (0)   147897 2024-05-18 09:14:58.000000 tui_dsmt-202406031350/src/tui_dsmt/jpanim/resources/vue-3.4.24.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:50:23.368699 tui_dsmt-202406031350/src/tui_dsmt/util/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-18 09:14:58.000000 tui_dsmt-202406031350/src/tui_dsmt/util/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:50:23.368699 tui_dsmt-202406031350/src/tui_dsmt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      897 2024-06-03 13:50:23.000000 tui_dsmt-202406031350/src/tui_dsmt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2860 2024-06-03 13:50:23.000000 tui_dsmt-202406031350/src/tui_dsmt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-06-03 13:50:23.000000 tui_dsmt-202406031350/src/tui_dsmt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      194 2024-06-03 13:50:23.000000 tui_dsmt-202406031350/src/tui_dsmt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-06-03 13:50:23.000000 tui_dsmt-202406031350/src/tui_dsmt.egg-info/top_level.txt
```

### Comparing `tui_dsmt-202406030834/PKG-INFO` & `tui_dsmt-202406031350/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tui_dsmt
-Version: 202406030834
+Version: 202406031350
 Summary: everything you need for our jupyter notebooks
 Home-page: https://dbgit.prakinf.tu-ilmenau.de/lectures/data-science-methoden-und-techniken
 Author: Eric Tröbs
 Author-email: eric.troebs@tu-ilmenau.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tui_dsmt-202406030834/setup.py` & `tui_dsmt-202406031350/setup.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202406030834/src/tui_dsmt/__init__.py` & `tui_dsmt-202406031350/src/tui_dsmt/__init__.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202406030834/src/tui_dsmt/clustering/PAM.py` & `tui_dsmt-202406031350/src/tui_dsmt/clustering/PAM.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202406030834/src/tui_dsmt/clustering/animation.py` & `tui_dsmt-202406031350/src/tui_dsmt/clustering/animation.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202406030834/src/tui_dsmt/clustering/datasets.py` & `tui_dsmt-202406031350/src/tui_dsmt/clustering/datasets.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202406030834/src/tui_dsmt/clustering/evaluation.py` & `tui_dsmt-202406031350/src/tui_dsmt/clustering/evaluation.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202406030834/src/tui_dsmt/clustering/hierarchical.py` & `tui_dsmt-202406031350/src/tui_dsmt/clustering/hierarchical.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202406030834/src/tui_dsmt/clustering/interactive.py` & `tui_dsmt-202406031350/src/tui_dsmt/clustering/interactive.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202406030834/src/tui_dsmt/fpm/BruteForceFI.py` & `tui_dsmt-202406031350/src/tui_dsmt/fpm/BruteForceFI.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202406030834/src/tui_dsmt/fpm/ConditionalFPTree.py` & `tui_dsmt-202406031350/src/tui_dsmt/fpm/ConditionalFPTree.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202406030834/src/tui_dsmt/fpm/ConditionalPatternBase.py` & `tui_dsmt-202406031350/src/tui_dsmt/fpm/ConditionalPatternBase.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202406030834/src/tui_dsmt/fpm/FPTree.py` & `tui_dsmt-202406031350/src/tui_dsmt/fpm/FPTree.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202406030834/src/tui_dsmt/fpm/HashTree.py` & `tui_dsmt-202406031350/src/tui_dsmt/fpm/HashTree.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202406030834/src/tui_dsmt/fpm/Itemset.py` & `tui_dsmt-202406031350/src/tui_dsmt/fpm/Itemset.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202406030834/src/tui_dsmt/fpm/ItemsetGrid.py` & `tui_dsmt-202406031350/src/tui_dsmt/fpm/ItemsetGrid.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202406030834/src/tui_dsmt/fpm/ItemsetGridApriori.py` & `tui_dsmt-202406031350/src/tui_dsmt/fpm/ItemsetGridApriori.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202406030834/src/tui_dsmt/fpm/ItemsetGridECLAT.py` & `tui_dsmt-202406031350/src/tui_dsmt/fpm/ItemsetGridECLAT.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202406030834/src/tui_dsmt/fpm/SequentialDatabase.py` & `tui_dsmt-202406031350/src/tui_dsmt/fpm/SequentialDatabase.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202406030834/src/tui_dsmt/fpm/SequentialItemset.py` & `tui_dsmt-202406031350/src/tui_dsmt/fpm/SequentialItemset.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202406030834/src/tui_dsmt/fpm/TransactionDatabase.py` & `tui_dsmt-202406031350/src/tui_dsmt/fpm/TransactionDatabase.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202406030834/src/tui_dsmt/fpm/__init__.py` & `tui_dsmt-202406031350/src/tui_dsmt/fpm/__init__.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202406030834/src/tui_dsmt/fpm/datasets.py` & `tui_dsmt-202406031350/src/tui_dsmt/fpm/datasets.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202406030834/src/tui_dsmt/fpm/resources/website_tracking.csv` & `tui_dsmt-202406031350/src/tui_dsmt/fpm/resources/website_tracking.csv`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202406030834/src/tui_dsmt/fpm/resources/website_tracking2.json` & `tui_dsmt-202406031350/src/tui_dsmt/fpm/resources/website_tracking2.json`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202406030834/src/tui_dsmt/graph/BFS.py` & `tui_dsmt-202406031350/src/tui_dsmt/graph/BFS.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202406030834/src/tui_dsmt/graph/BipartiteFlow.py` & `tui_dsmt-202406031350/src/tui_dsmt/graph/BipartiteFlow.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202406030834/src/tui_dsmt/graph/BronKerbosch.py` & `tui_dsmt-202406031350/src/tui_dsmt/graph/BronKerbosch.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202406030834/src/tui_dsmt/graph/DFS.py` & `tui_dsmt-202406031350/src/tui_dsmt/graph/DFS.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202406030834/src/tui_dsmt/graph/Dijkstra.py` & `tui_dsmt-202406031350/src/tui_dsmt/graph/Dijkstra.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202406030834/src/tui_dsmt/graph/FordFulkerson.py` & `tui_dsmt-202406031350/src/tui_dsmt/graph/FordFulkerson.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202406030834/src/tui_dsmt/graph/FruchtermanReingold.py` & `tui_dsmt-202406031350/src/tui_dsmt/graph/FruchtermanReingold.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202406030834/src/tui_dsmt/graph/Hall.py` & `tui_dsmt-202406031350/src/tui_dsmt/graph/Hall.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202406030834/src/tui_dsmt/graph/InteractiveGraph.py` & `tui_dsmt-202406031350/src/tui_dsmt/graph/InteractiveGraph.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202406030834/src/tui_dsmt/graph/Kruskal.py` & `tui_dsmt-202406031350/src/tui_dsmt/graph/Kruskal.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202406030834/src/tui_dsmt/graph/LabelPropagation.py` & `tui_dsmt-202406031350/src/tui_dsmt/graph/LabelPropagation.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202406030834/src/tui_dsmt/graph/MaximumFlow.py` & `tui_dsmt-202406031350/src/tui_dsmt/graph/MaximumFlow.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202406030834/src/tui_dsmt/graph/RandomWalk.py` & `tui_dsmt-202406031350/src/tui_dsmt/graph/RandomWalk.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202406030834/src/tui_dsmt/graph/__init__.py` & `tui_dsmt-202406031350/src/tui_dsmt/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202406030834/src/tui_dsmt/graph/datasets.py` & `tui_dsmt-202406031350/src/tui_dsmt/graph/datasets.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202406030834/src/tui_dsmt/graph/game.py` & `tui_dsmt-202406031350/src/tui_dsmt/graph/game.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202406030834/src/tui_dsmt/graph/html.py` & `tui_dsmt-202406031350/src/tui_dsmt/graph/html.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202406030834/src/tui_dsmt/graph/representation.py` & `tui_dsmt-202406031350/src/tui_dsmt/graph/representation.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202406030834/src/tui_dsmt/graph/resources/bipartite_exams.csv` & `tui_dsmt-202406031350/src/tui_dsmt/graph/resources/bipartite_exams.csv`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202406030834/src/tui_dsmt/graph/resources/dewiki_sample.pickle.bz2` & `tui_dsmt-202406031350/src/tui_dsmt/graph/resources/dewiki_sample.pickle.bz2`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202406030834/src/tui_dsmt/graph/resources/tw.csv` & `tui_dsmt-202406031350/src/tui_dsmt/graph/resources/tw.csv`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202406030834/src/tui_dsmt/graph/resources/tw_pos.json` & `tui_dsmt-202406031350/src/tui_dsmt/graph/resources/tw_pos.json`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202406030834/src/tui_dsmt/graph/resources/wiki_it.tsv` & `tui_dsmt-202406031350/src/tui_dsmt/graph/resources/wiki_it.tsv`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202406030834/src/tui_dsmt/graph/resources/wiki_it_pos.json` & `tui_dsmt-202406031350/src/tui_dsmt/graph/resources/wiki_it_pos.json`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202406030834/src/tui_dsmt/jpanim/JupyterAnimation.py` & `tui_dsmt-202406031350/src/tui_dsmt/jpanim/JupyterAnimation.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202406030834/src/tui_dsmt/jpanim/resources/controls-ff.html` & `tui_dsmt-202406031350/src/tui_dsmt/jpanim/resources/controls-ff.html`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202406030834/src/tui_dsmt/jpanim/resources/controls.html` & `tui_dsmt-202406031350/src/tui_dsmt/jpanim/resources/controls.html`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202406030834/src/tui_dsmt/jpanim/resources/script.js` & `tui_dsmt-202406031350/src/tui_dsmt/jpanim/resources/script.js`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202406030834/src/tui_dsmt/jpanim/resources/vue-3.4.24.js` & `tui_dsmt-202406031350/src/tui_dsmt/jpanim/resources/vue-3.4.24.js`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202406030834/src/tui_dsmt.egg-info/PKG-INFO` & `tui_dsmt-202406031350/src/tui_dsmt.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tui_dsmt
-Version: 202406030834
+Version: 202406031350
 Summary: everything you need for our jupyter notebooks
 Home-page: https://dbgit.prakinf.tu-ilmenau.de/lectures/data-science-methoden-und-techniken
 Author: Eric Tröbs
 Author-email: eric.troebs@tu-ilmenau.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tui_dsmt-202406030834/src/tui_dsmt.egg-info/SOURCES.txt` & `tui_dsmt-202406031350/src/tui_dsmt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

