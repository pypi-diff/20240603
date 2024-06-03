# Comparing `tmp/SNAKES-0.9.32.tar.gz` & `tmp/SNAKES-0.9.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SNAKES-0.9.32.tar", last modified: Mon Oct  2 11:41:24 2023, max compression
+gzip compressed data, was "dist/SNAKES-0.9.33.tar", last modified: Mon Jun  3 11:00:13 2024, max compression
```

## Comparing `SNAKES-0.9.32.tar` & `SNAKES-0.9.33.tar`

### file list

```diff
@@ -1,153 +1,153 @@
-drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-10-02 11:41:24.820441 SNAKES-0.9.32/
--rw-r--r--   0 franck    (1000) franck    (1000)       60 2016-09-20 08:55:14.798269 SNAKES-0.9.32/.gitignore
--rw-r--r--   0 franck    (1000) franck    (1000)      423 2015-03-14 16:15:28.936069 SNAKES-0.9.32/BUGS
--rw-rw-r--   0 franck    (1000) franck    (1000)     7642 2022-05-13 06:38:09.861553 SNAKES-0.9.32/LICENCE.md
--rw-r--r--   0 franck    (1000) franck    (1000)     3747 2023-10-02 11:41:24.812441 SNAKES-0.9.32/MANIFEST
--rw-r--r--   0 franck    (1000) franck    (1000)       95 2016-06-20 09:18:26.643131 SNAKES-0.9.32/MANIFEST.in
--rw-r--r--   0 franck    (1000) franck    (1000)     1133 2020-10-14 14:14:50.647564 SNAKES-0.9.32/Makefile
--rw-rw-r--   0 franck    (1000) franck    (1000)      987 2023-10-02 11:41:24.820441 SNAKES-0.9.32/PKG-INFO
--rw-r--r--   0 franck    (1000) franck    (1000)     2331 2021-06-09 15:58:26.142109 SNAKES-0.9.32/README.md
--rw-r--r--   0 franck    (1000) franck    (1000)        7 2023-10-02 11:41:11.212459 SNAKES-0.9.32/VERSION
-drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-10-02 11:41:24.816441 SNAKES-0.9.32/bin/
--rwxr-xr-x   0 franck    (1000) franck    (1000)       80 2015-03-14 16:15:28.936069 SNAKES-0.9.32/bin/abcd
--rwxr-xr-x   0 franck    (1000) franck    (1000)     4018 2015-03-14 16:15:28.936069 SNAKES-0.9.32/bin/snkc
--rwxr-xr-x   0 franck    (1000) franck    (1000)     1908 2015-03-14 16:15:28.936069 SNAKES-0.9.32/bin/snkd
-drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-10-02 11:41:24.816441 SNAKES-0.9.32/doc/
--rw-r--r--   0 franck    (1000) franck    (1000)     7639 2015-03-14 16:15:28.936069 SNAKES-0.9.32/doc/COPYING
--rw-r--r--   0 franck    (1000) franck    (1000)    13756 2015-03-14 16:15:28.936069 SNAKES-0.9.32/doc/abcd.txt
-drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-10-02 11:41:24.812441 SNAKES-0.9.32/doc/examples/
-drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-10-02 11:41:24.816441 SNAKES-0.9.32/doc/examples/abcd/
--rw-r--r--   0 franck    (1000) franck    (1000)      274 2015-03-14 16:15:28.936069 SNAKES-0.9.32/doc/examples/abcd/README
-drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-10-02 11:41:24.816441 SNAKES-0.9.32/doc/examples/abcd/ns/
--rw-r--r--   0 franck    (1000) franck    (1000)    10652 2015-03-14 16:15:28.936069 SNAKES-0.9.32/doc/examples/abcd/ns/dolev_yao.py
--rw-r--r--   0 franck    (1000) franck    (1000)     1590 2015-03-14 16:15:28.936069 SNAKES-0.9.32/doc/examples/abcd/ns/ns.abcd
--rw-r--r--   0 franck    (1000) franck    (1000)      595 2015-03-14 16:15:28.936069 SNAKES-0.9.32/doc/examples/abcd/ns/ns.py
--rw-r--r--   0 franck    (1000) franck    (1000)      439 2015-03-14 16:15:28.936069 SNAKES-0.9.32/doc/examples/abcd/philo.abcd
--rw-r--r--   0 franck    (1000) franck    (1000)      469 2015-03-14 16:15:28.936069 SNAKES-0.9.32/doc/examples/abcd/prod-cons.abcd
--rw-r--r--   0 franck    (1000) franck    (1000)      878 2015-03-14 16:15:28.936069 SNAKES-0.9.32/doc/examples/abcd/railroad.abcd
--rw-r--r--   0 franck    (1000) franck    (1000)      482 2015-03-14 16:15:28.936069 SNAKES-0.9.32/doc/examples/abcd/railroad.py
--rw-r--r--   0 franck    (1000) franck    (1000)    21394 2015-03-14 16:15:28.936069 SNAKES-0.9.32/doc/queries.txt
--rw-r--r--   0 franck    (1000) franck    (1000)      922 2015-03-14 16:15:28.936069 SNAKES-0.9.32/doc/simple-coloured.pnml
--rw-r--r--   0 franck    (1000) franck    (1000)      805 2015-03-14 16:15:28.936069 SNAKES-0.9.32/doc/simple-pt.pnml
--rw-r--r--   0 franck    (1000) franck    (1000)    19513 2015-03-14 16:15:28.936069 SNAKES-0.9.32/doc/snakes-pnml.txt
--rw-r--r--   0 franck    (1000) franck    (1000)    15652 2015-03-14 16:15:28.936069 SNAKES-0.9.32/doc/tutorial.png
--rw-r--r--   0 franck    (1000) franck    (1000)    51066 2015-03-14 16:15:28.936069 SNAKES-0.9.32/doc/tutorial.txt
--rw-r--r--   0 franck    (1000) franck    (1000)      693 2015-03-14 16:15:28.936069 SNAKES-0.9.32/mklang.py
--rw-r--r--   0 franck    (1000) franck    (1000)     3381 2021-06-09 16:04:05.542667 SNAKES-0.9.32/setup.py
-drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-10-02 11:41:24.816441 SNAKES-0.9.32/snakes/
--rw-rw-r--   0 franck    (1000) franck    (1000)     1603 2023-10-02 11:41:11.216459 SNAKES-0.9.32/snakes/__init__.py
--rw-r--r--   0 franck    (1000) franck    (1000)      537 2017-12-09 15:45:08.326904 SNAKES-0.9.32/snakes/compat.py
--rw-r--r--   0 franck    (1000) franck    (1000)    32205 2015-03-14 16:15:28.936069 SNAKES-0.9.32/snakes/data.py
--rw-r--r--   0 franck    (1000) franck    (1000)    11922 2015-03-14 16:15:28.940069 SNAKES-0.9.32/snakes/hashables.py
-drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-10-02 11:41:24.816441 SNAKES-0.9.32/snakes/lang/
--rw-r--r--   0 franck    (1000) franck    (1000)     6396 2015-03-14 16:15:28.940069 SNAKES-0.9.32/snakes/lang/__init__.py
-drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-10-02 11:41:24.816441 SNAKES-0.9.32/snakes/lang/abcd/
--rw-r--r--   0 franck    (1000) franck    (1000)        0 2015-03-14 16:15:28.940069 SNAKES-0.9.32/snakes/lang/abcd/__init__.py
--rw-r--r--   0 franck    (1000) franck    (1000)    31781 2015-03-14 16:15:28.940069 SNAKES-0.9.32/snakes/lang/abcd/asdl.py
--rw-r--r--   0 franck    (1000) franck    (1000)    37555 2015-03-14 16:15:28.940069 SNAKES-0.9.32/snakes/lang/abcd/parser.py
--rw-r--r--   0 franck    (1000) franck    (1000)   290093 2015-03-14 16:15:28.940069 SNAKES-0.9.32/snakes/lang/abcd/pgen.py
--rw-r--r--   0 franck    (1000) franck    (1000)     9839 2015-03-14 16:15:28.940069 SNAKES-0.9.32/snakes/lang/asdl.py
--rw-r--r--   0 franck    (1000) franck    (1000)    10235 2015-03-14 16:15:28.940069 SNAKES-0.9.32/snakes/lang/astjy25.py
--rw-r--r--   0 franck    (1000) franck    (1000)    11933 2023-10-02 11:39:38.996581 SNAKES-0.9.32/snakes/lang/astpy25.py
--rw-r--r--   0 franck    (1000) franck    (1000)    10324 2015-03-14 16:15:28.940069 SNAKES-0.9.32/snakes/lang/astpypy.py
-drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-10-02 11:41:24.816441 SNAKES-0.9.32/snakes/lang/ctlstar/
--rw-r--r--   0 franck    (1000) franck    (1000)        0 2015-03-14 16:15:28.940069 SNAKES-0.9.32/snakes/lang/ctlstar/__init__.py
--rw-r--r--   0 franck    (1000) franck    (1000)    29069 2015-03-14 16:15:28.940069 SNAKES-0.9.32/snakes/lang/ctlstar/asdl.py
--rw-r--r--   0 franck    (1000) franck    (1000)    27179 2015-03-14 16:15:28.940069 SNAKES-0.9.32/snakes/lang/ctlstar/parser.py
--rw-r--r--   0 franck    (1000) franck    (1000)   286604 2015-03-14 16:15:28.944069 SNAKES-0.9.32/snakes/lang/ctlstar/pgen.py
--rw-r--r--   0 franck    (1000) franck    (1000)    49093 2015-03-14 16:15:28.944069 SNAKES-0.9.32/snakes/lang/pgen.py
-drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-10-02 11:41:24.816441 SNAKES-0.9.32/snakes/lang/pylib/
--rw-r--r--   0 franck    (1000) franck    (1000)        0 2015-03-14 16:15:28.944069 SNAKES-0.9.32/snakes/lang/pylib/__init__.py
--rw-r--r--   0 franck    (1000) franck    (1000)    11630 2015-03-14 16:15:28.944069 SNAKES-0.9.32/snakes/lang/pylib/asdl.py
--rw-r--r--   0 franck    (1000) franck    (1000)    26841 2015-03-14 16:15:28.944069 SNAKES-0.9.32/snakes/lang/pylib/spark.py
--rw-r--r--   0 franck    (1000) franck    (1000)    14022 2015-03-14 16:15:28.944069 SNAKES-0.9.32/snakes/lang/pylib/unparse.py
-drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-10-02 11:41:24.816441 SNAKES-0.9.32/snakes/lang/python/
--rw-r--r--   0 franck    (1000) franck    (1000)        0 2015-03-14 16:15:28.944069 SNAKES-0.9.32/snakes/lang/python/__init__.py
--rw-r--r--   0 franck    (1000) franck    (1000)    22425 2015-03-14 16:15:28.944069 SNAKES-0.9.32/snakes/lang/python/asdl.py
--rw-r--r--   0 franck    (1000) franck    (1000)    97603 2015-03-14 16:15:28.944069 SNAKES-0.9.32/snakes/lang/python/parser.py
--rw-r--r--   0 franck    (1000) franck    (1000)   210533 2015-03-14 16:15:28.948069 SNAKES-0.9.32/snakes/lang/python/pgen.py
--rw-r--r--   0 franck    (1000) franck    (1000)    14221 2015-03-14 16:15:28.948069 SNAKES-0.9.32/snakes/lang/unparse.py
--rw-r--r--   0 franck    (1000) franck    (1000)   158724 2022-10-24 13:00:21.585567 SNAKES-0.9.32/snakes/nets.py
-drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-10-02 11:41:24.816441 SNAKES-0.9.32/snakes/plugins/
--rw-r--r--   0 franck    (1000) franck    (1000)     7731 2023-04-26 13:32:18.999430 SNAKES-0.9.32/snakes/plugins/__init__.py
--rw-r--r--   0 franck    (1000) franck    (1000)     5850 2017-09-12 12:54:19.889129 SNAKES-0.9.32/snakes/plugins/bound.py
--rw-r--r--   0 franck    (1000) franck    (1000)    15116 2023-04-26 13:16:22.245726 SNAKES-0.9.32/snakes/plugins/clusters.py
--rw-r--r--   0 franck    (1000) franck    (1000)    17105 2023-03-16 10:10:42.618753 SNAKES-0.9.32/snakes/plugins/gv.py
--rw-r--r--   0 franck    (1000) franck    (1000)     1022 2015-03-14 16:15:28.948069 SNAKES-0.9.32/snakes/plugins/hello.py
--rw-r--r--   0 franck    (1000) franck    (1000)    11004 2015-03-14 16:15:28.948069 SNAKES-0.9.32/snakes/plugins/labels.py
--rw-r--r--   0 franck    (1000) franck    (1000)     3461 2016-10-10 16:15:27.918489 SNAKES-0.9.32/snakes/plugins/let.py
--rw-r--r--   0 franck    (1000) franck    (1000)     4689 2017-11-05 15:30:00.859886 SNAKES-0.9.32/snakes/plugins/modules.py
--rw-r--r--   0 franck    (1000) franck    (1000)    11449 2017-05-18 12:26:14.243229 SNAKES-0.9.32/snakes/plugins/ops.py
--rw-r--r--   0 franck    (1000) franck    (1000)    11054 2015-03-14 16:15:28.952069 SNAKES-0.9.32/snakes/plugins/pids.py
--rw-r--r--   0 franck    (1000) franck    (1000)    13387 2017-05-18 12:24:24.007225 SNAKES-0.9.32/snakes/plugins/pos.py
--rw-r--r--   0 franck    (1000) franck    (1000)     9573 2015-03-14 16:15:28.956069 SNAKES-0.9.32/snakes/plugins/query.py
--rw-r--r--   0 franck    (1000) franck    (1000)    25669 2017-05-18 12:25:58.315229 SNAKES-0.9.32/snakes/plugins/status.py
--rw-r--r--   0 franck    (1000) franck    (1000)    38797 2015-03-14 16:15:28.956069 SNAKES-0.9.32/snakes/plugins/synchro.py
--rw-r--r--   0 franck    (1000) franck    (1000)    31015 2015-03-14 16:15:28.956069 SNAKES-0.9.32/snakes/pnml.py
--rw-r--r--   0 franck    (1000) franck    (1000)    52213 2015-03-14 16:15:28.956069 SNAKES-0.9.32/snakes/typing.py
-drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-10-02 11:41:24.816441 SNAKES-0.9.32/snakes/utils/
--rw-r--r--   0 franck    (1000) franck    (1000)      382 2015-03-14 16:15:28.956069 SNAKES-0.9.32/snakes/utils/__init__.py
-drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-10-02 11:41:24.816441 SNAKES-0.9.32/snakes/utils/abcd/
--rw-r--r--   0 franck    (1000) franck    (1000)      630 2015-03-14 16:15:28.956069 SNAKES-0.9.32/snakes/utils/abcd/__init__.py
--rw-r--r--   0 franck    (1000) franck    (1000)    24866 2017-04-19 21:46:39.152750 SNAKES-0.9.32/snakes/utils/abcd/build.py
--rw-r--r--   0 franck    (1000) franck    (1000)     2505 2016-11-15 09:57:29.928644 SNAKES-0.9.32/snakes/utils/abcd/checker.py
--rw-r--r--   0 franck    (1000) franck    (1000)    17492 2015-03-14 16:15:28.956069 SNAKES-0.9.32/snakes/utils/abcd/html.py
--rw-r--r--   0 franck    (1000) franck    (1000)    10458 2016-10-10 16:27:06.566514 SNAKES-0.9.32/snakes/utils/abcd/main.py
-drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-10-02 11:41:24.816441 SNAKES-0.9.32/snakes/utils/abcd/resources/
--rw-r--r--   0 franck    (1000) franck    (1000)      249 2015-03-14 16:15:28.956069 SNAKES-0.9.32/snakes/utils/abcd/resources/about.html
--rw-r--r--   0 franck    (1000) franck    (1000)     1806 2015-03-14 16:15:28.956069 SNAKES-0.9.32/snakes/utils/abcd/resources/alive.txt
-drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-10-02 11:41:24.816441 SNAKES-0.9.32/snakes/utils/abcd/resources/css/
--rw-r--r--   0 franck    (1000) franck    (1000)    14936 2015-03-14 16:15:28.956069 SNAKES-0.9.32/snakes/utils/abcd/resources/css/bootstrap-theme.css
--rw-r--r--   0 franck    (1000) franck    (1000)    38388 2015-03-14 16:15:28.956069 SNAKES-0.9.32/snakes/utils/abcd/resources/css/bootstrap-theme.css.map
--rw-r--r--   0 franck    (1000) franck    (1000)   121220 2015-03-14 16:15:28.960069 SNAKES-0.9.32/snakes/utils/abcd/resources/css/bootstrap.css
--rw-r--r--   0 franck    (1000) franck    (1000)   245960 2015-03-14 16:15:28.960069 SNAKES-0.9.32/snakes/utils/abcd/resources/css/bootstrap.css.map
--rw-r--r--   0 franck    (1000) franck    (1000)    73046 2015-03-14 16:15:28.964069 SNAKES-0.9.32/snakes/utils/abcd/resources/css/docs.css
--rw-r--r--   0 franck    (1000) franck    (1000)   146525 2015-03-14 16:15:28.964069 SNAKES-0.9.32/snakes/utils/abcd/resources/d3.min.js
-drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-10-02 11:41:24.816441 SNAKES-0.9.32/snakes/utils/abcd/resources/fonts/
--rw-r--r--   0 franck    (1000) franck    (1000)    20335 2015-03-14 16:15:28.964069 SNAKES-0.9.32/snakes/utils/abcd/resources/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 franck    (1000) franck    (1000)    62927 2015-03-14 16:15:28.964069 SNAKES-0.9.32/snakes/utils/abcd/resources/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 franck    (1000) franck    (1000)    41280 2015-03-14 16:15:28.964069 SNAKES-0.9.32/snakes/utils/abcd/resources/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 franck    (1000) franck    (1000)    23320 2015-03-14 16:15:28.964069 SNAKES-0.9.32/snakes/utils/abcd/resources/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 franck    (1000) franck    (1000)     3842 2015-03-14 16:15:28.964069 SNAKES-0.9.32/snakes/utils/abcd/resources/index.html
--rw-r--r--   0 franck    (1000) franck    (1000)   247350 2015-03-14 16:15:28.968069 SNAKES-0.9.32/snakes/utils/abcd/resources/jquery.min.js
--rw-r--r--   0 franck    (1000) franck    (1000)     2640 2015-03-14 16:15:28.968069 SNAKES-0.9.32/snakes/utils/abcd/resources/jquery.periodic.js
-drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-10-02 11:41:24.816441 SNAKES-0.9.32/snakes/utils/abcd/resources/js/
--rw-r--r--   0 franck    (1000) franck    (1000)     4602 2015-03-14 16:15:28.968069 SNAKES-0.9.32/snakes/utils/abcd/resources/js/bootstrap.file-input.js
--rw-r--r--   0 franck    (1000) franck    (1000)    29110 2015-03-14 16:15:28.968069 SNAKES-0.9.32/snakes/utils/abcd/resources/js/bootstrap.min.js
--rw-r--r--   0 franck    (1000) franck    (1000)      923 2015-03-14 16:15:28.968069 SNAKES-0.9.32/snakes/utils/abcd/resources/js/petri.js
--rw-r--r--   0 franck    (1000) franck    (1000)     1533 2015-03-14 16:15:28.968069 SNAKES-0.9.32/snakes/utils/abcd/resources/model.css
--rw-r--r--   0 franck    (1000) franck    (1000)      960 2015-03-14 16:15:28.968069 SNAKES-0.9.32/snakes/utils/abcd/resources/model.html
--rw-r--r--   0 franck    (1000) franck    (1000)     1689 2015-03-14 16:15:28.968069 SNAKES-0.9.32/snakes/utils/abcd/resources/model.js
--rw-r--r--   0 franck    (1000) franck    (1000)     1939 2015-03-14 16:15:28.968069 SNAKES-0.9.32/snakes/utils/abcd/resources/simulator.css
--rw-r--r--   0 franck    (1000) franck    (1000)    66924 2015-03-14 16:15:28.968069 SNAKES-0.9.32/snakes/utils/abcd/resources/simulator.js
--rw-r--r--   0 franck    (1000) franck    (1000)     3880 2015-03-14 16:15:28.968069 SNAKES-0.9.32/snakes/utils/abcd/simul.py
--rw-r--r--   0 franck    (1000) franck    (1000)     3101 2015-03-14 16:15:28.968069 SNAKES-0.9.32/snakes/utils/abcd/transform.py
--rw-r--r--   0 franck    (1000) franck    (1000)    25530 2017-05-18 12:20:59.263218 SNAKES-0.9.32/snakes/utils/apidoc.py
-drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-10-02 11:41:24.816441 SNAKES-0.9.32/snakes/utils/ctlstar/
--rw-r--r--   0 franck    (1000) franck    (1000)     1157 2015-03-14 16:15:28.968069 SNAKES-0.9.32/snakes/utils/ctlstar/__init__.py
--rw-r--r--   0 franck    (1000) franck    (1000)     6154 2015-03-14 16:15:28.968069 SNAKES-0.9.32/snakes/utils/ctlstar/build.py
-drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-10-02 11:41:24.816441 SNAKES-0.9.32/snakes/utils/simul/
--rw-r--r--   0 franck    (1000) franck    (1000)     8786 2016-09-16 08:14:17.115513 SNAKES-0.9.32/snakes/utils/simul/__init__.py
--rw-r--r--   0 franck    (1000) franck    (1000)     2548 2015-04-09 12:05:23.690282 SNAKES-0.9.32/snakes/utils/simul/html.py
--rw-r--r--   0 franck    (1000) franck    (1000)     7237 2023-10-02 11:38:31.580669 SNAKES-0.9.32/snakes/utils/simul/httpd.py
--rw-r--r--   0 franck    (1000) franck    (1000)     7139 2023-10-02 11:37:12.456772 SNAKES-0.9.32/snakes/utils/simul/logger.py
-drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-10-02 11:41:24.816441 SNAKES-0.9.32/snakes/utils/simul/resources/
--rw-r--r--   0 franck    (1000) franck    (1000)        0 2015-03-14 16:15:28.968069 SNAKES-0.9.32/snakes/utils/simul/resources/about.css
--rw-r--r--   0 franck    (1000) franck    (1000)      241 2015-03-14 16:15:28.968069 SNAKES-0.9.32/snakes/utils/simul/resources/about.html
--rw-r--r--   0 franck    (1000) franck    (1000)        0 2015-03-14 16:15:28.968069 SNAKES-0.9.32/snakes/utils/simul/resources/about.js
--rw-r--r--   0 franck    (1000) franck    (1000)     1806 2015-03-14 16:15:28.968069 SNAKES-0.9.32/snakes/utils/simul/resources/alive.txt
--rw-r--r--   0 franck    (1000) franck    (1000)     1621 2015-03-14 16:15:28.968069 SNAKES-0.9.32/snakes/utils/simul/resources/index.html
--rw-r--r--   0 franck    (1000) franck    (1000)    96381 2015-03-14 16:15:28.968069 SNAKES-0.9.32/snakes/utils/simul/resources/jquery.min.js
--rw-r--r--   0 franck    (1000) franck    (1000)     2653 2015-03-14 16:15:28.968069 SNAKES-0.9.32/snakes/utils/simul/resources/jquery.periodic.js
--rw-r--r--   0 franck    (1000) franck    (1000)       57 2015-03-14 16:15:28.968069 SNAKES-0.9.32/snakes/utils/simul/resources/model.css
--rw-r--r--   0 franck    (1000) franck    (1000)      195 2015-03-14 16:15:28.968069 SNAKES-0.9.32/snakes/utils/simul/resources/model.html
--rw-r--r--   0 franck    (1000) franck    (1000)        0 2015-03-14 16:15:28.968069 SNAKES-0.9.32/snakes/utils/simul/resources/model.js
--rw-r--r--   0 franck    (1000) franck    (1000)     1939 2015-03-14 16:15:28.968069 SNAKES-0.9.32/snakes/utils/simul/resources/simulator.css
--rw-r--r--   0 franck    (1000) franck    (1000)     4341 2015-03-14 16:15:28.968069 SNAKES-0.9.32/snakes/utils/simul/resources/simulator.js
--rw-r--r--   0 franck    (1000) franck    (1000)       57 2015-03-14 16:15:28.968069 SNAKES-0.9.32/snakes/utils/simul/resources/trace.css
--rw-r--r--   0 franck    (1000) franck    (1000)        0 2015-03-14 16:15:28.968069 SNAKES-0.9.32/snakes/utils/simul/resources/trace.js
--rw-r--r--   0 franck    (1000) franck    (1000)     2044 2015-03-14 16:15:28.972069 SNAKES-0.9.32/test.py
-drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-10-02 11:41:24.820441 SNAKES-0.9.32/utils/
--rw-r--r--   0 franck    (1000) franck    (1000)      226 2015-03-14 16:15:28.972069 SNAKES-0.9.32/utils/abcd-mode.el
--rw-r--r--   0 franck    (1000) franck    (1000)     3112 2016-06-20 09:09:40.347122 SNAKES-0.9.32/utils/abcd-mode.elc
--rw-r--r--   0 franck    (1000) franck    (1000)      777 2016-06-23 13:09:38.208567 SNAKES-0.9.32/version.py
+drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2024-06-03 11:00:13.000000 SNAKES-0.9.33/
+drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2024-06-03 11:00:13.000000 SNAKES-0.9.33/utils/
+-rw-r--r--   0 franck    (1000) franck    (1000)     3112 2016-06-20 09:09:40.000000 SNAKES-0.9.33/utils/abcd-mode.elc
+-rw-r--r--   0 franck    (1000) franck    (1000)      226 2015-03-14 16:15:28.000000 SNAKES-0.9.33/utils/abcd-mode.el
+drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2024-06-03 11:00:13.000000 SNAKES-0.9.33/doc/
+drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2024-06-03 11:00:13.000000 SNAKES-0.9.33/doc/examples/
+drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2024-06-03 11:00:13.000000 SNAKES-0.9.33/doc/examples/abcd/
+-rw-r--r--   0 franck    (1000) franck    (1000)      482 2015-03-14 16:15:28.000000 SNAKES-0.9.33/doc/examples/abcd/railroad.py
+-rw-r--r--   0 franck    (1000) franck    (1000)      274 2015-03-14 16:15:28.000000 SNAKES-0.9.33/doc/examples/abcd/README
+-rw-r--r--   0 franck    (1000) franck    (1000)      469 2015-03-14 16:15:28.000000 SNAKES-0.9.33/doc/examples/abcd/prod-cons.abcd
+drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2024-06-03 11:00:13.000000 SNAKES-0.9.33/doc/examples/abcd/ns/
+-rw-r--r--   0 franck    (1000) franck    (1000)     1590 2015-03-14 16:15:28.000000 SNAKES-0.9.33/doc/examples/abcd/ns/ns.abcd
+-rw-r--r--   0 franck    (1000) franck    (1000)      595 2015-03-14 16:15:28.000000 SNAKES-0.9.33/doc/examples/abcd/ns/ns.py
+-rw-r--r--   0 franck    (1000) franck    (1000)    10652 2015-03-14 16:15:28.000000 SNAKES-0.9.33/doc/examples/abcd/ns/dolev_yao.py
+-rw-r--r--   0 franck    (1000) franck    (1000)      439 2015-03-14 16:15:28.000000 SNAKES-0.9.33/doc/examples/abcd/philo.abcd
+-rw-r--r--   0 franck    (1000) franck    (1000)      878 2015-03-14 16:15:28.000000 SNAKES-0.9.33/doc/examples/abcd/railroad.abcd
+-rw-r--r--   0 franck    (1000) franck    (1000)     7639 2015-03-14 16:15:28.000000 SNAKES-0.9.33/doc/COPYING
+-rw-r--r--   0 franck    (1000) franck    (1000)    13756 2015-03-14 16:15:28.000000 SNAKES-0.9.33/doc/abcd.txt
+-rw-r--r--   0 franck    (1000) franck    (1000)    19513 2015-03-14 16:15:28.000000 SNAKES-0.9.33/doc/snakes-pnml.txt
+-rw-r--r--   0 franck    (1000) franck    (1000)    21394 2015-03-14 16:15:28.000000 SNAKES-0.9.33/doc/queries.txt
+-rw-r--r--   0 franck    (1000) franck    (1000)      922 2015-03-14 16:15:28.000000 SNAKES-0.9.33/doc/simple-coloured.pnml
+-rw-r--r--   0 franck    (1000) franck    (1000)    15652 2015-03-14 16:15:28.000000 SNAKES-0.9.33/doc/tutorial.png
+-rw-r--r--   0 franck    (1000) franck    (1000)      805 2015-03-14 16:15:28.000000 SNAKES-0.9.33/doc/simple-pt.pnml
+-rw-r--r--   0 franck    (1000) franck    (1000)    51066 2015-03-14 16:15:28.000000 SNAKES-0.9.33/doc/tutorial.txt
+-rw-r--r--   0 franck    (1000) franck    (1000)     3747 2024-06-03 11:00:13.000000 SNAKES-0.9.33/MANIFEST
+-rw-rw-r--   0 franck    (1000) franck    (1000)     7642 2022-05-13 06:38:09.000000 SNAKES-0.9.33/LICENCE.md
+-rw-r--r--   0 franck    (1000) franck    (1000)     2331 2021-06-09 15:58:26.000000 SNAKES-0.9.33/README.md
+-rw-r--r--   0 franck    (1000) franck    (1000)      423 2015-03-14 16:15:28.000000 SNAKES-0.9.33/BUGS
+-rw-r--r--   0 franck    (1000) franck    (1000)      693 2015-03-14 16:15:28.000000 SNAKES-0.9.33/mklang.py
+-rw-rw-r--   0 franck    (1000) franck    (1000)      987 2024-06-03 11:00:13.000000 SNAKES-0.9.33/PKG-INFO
+drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2024-06-03 11:00:13.000000 SNAKES-0.9.33/bin/
+-rwxr-xr-x   0 franck    (1000) franck    (1000)     4018 2015-03-14 16:15:28.000000 SNAKES-0.9.33/bin/snkc
+-rwxr-xr-x   0 franck    (1000) franck    (1000)       80 2015-03-14 16:15:28.000000 SNAKES-0.9.33/bin/abcd
+-rwxr-xr-x   0 franck    (1000) franck    (1000)     1908 2015-03-14 16:15:28.000000 SNAKES-0.9.33/bin/snkd
+-rw-r--r--   0 franck    (1000) franck    (1000)     3381 2021-06-09 16:04:05.000000 SNAKES-0.9.33/setup.py
+-rw-r--r--   0 franck    (1000) franck    (1000)     1133 2020-10-14 14:14:50.000000 SNAKES-0.9.33/Makefile
+-rw-r--r--   0 franck    (1000) franck    (1000)      777 2016-06-23 13:09:38.000000 SNAKES-0.9.33/version.py
+-rw-r--r--   0 franck    (1000) franck    (1000)       95 2016-06-20 09:18:26.000000 SNAKES-0.9.33/MANIFEST.in
+-rw-r--r--   0 franck    (1000) franck    (1000)       60 2016-09-20 08:55:14.000000 SNAKES-0.9.33/.gitignore
+-rw-r--r--   0 franck    (1000) franck    (1000)        7 2024-06-03 10:56:37.000000 SNAKES-0.9.33/VERSION
+-rw-r--r--   0 franck    (1000) franck    (1000)     2044 2015-03-14 16:15:28.000000 SNAKES-0.9.33/test.py
+drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2024-06-03 11:00:13.000000 SNAKES-0.9.33/snakes/
+drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2024-06-03 11:00:13.000000 SNAKES-0.9.33/snakes/utils/
+drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2024-06-03 11:00:13.000000 SNAKES-0.9.33/snakes/utils/ctlstar/
+-rw-r--r--   0 franck    (1000) franck    (1000)     6154 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/utils/ctlstar/build.py
+-rw-r--r--   0 franck    (1000) franck    (1000)     1157 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/utils/ctlstar/__init__.py
+-rw-r--r--   0 franck    (1000) franck    (1000)      382 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/utils/__init__.py
+drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2024-06-03 11:00:13.000000 SNAKES-0.9.33/snakes/utils/abcd/
+drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2024-06-03 11:00:13.000000 SNAKES-0.9.33/snakes/utils/abcd/resources/
+-rw-r--r--   0 franck    (1000) franck    (1000)     3842 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/utils/abcd/resources/index.html
+-rw-r--r--   0 franck    (1000) franck    (1000)      960 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/utils/abcd/resources/model.html
+drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2024-06-03 11:00:13.000000 SNAKES-0.9.33/snakes/utils/abcd/resources/fonts/
+-rw-r--r--   0 franck    (1000) franck    (1000)    41280 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/utils/abcd/resources/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 franck    (1000) franck    (1000)    23320 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/utils/abcd/resources/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 franck    (1000) franck    (1000)    62927 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/utils/abcd/resources/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 franck    (1000) franck    (1000)    20335 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/utils/abcd/resources/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 franck    (1000) franck    (1000)     1533 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/utils/abcd/resources/model.css
+-rw-r--r--   0 franck    (1000) franck    (1000)    66924 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/utils/abcd/resources/simulator.js
+-rw-r--r--   0 franck    (1000) franck    (1000)     2640 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/utils/abcd/resources/jquery.periodic.js
+-rw-r--r--   0 franck    (1000) franck    (1000)      249 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/utils/abcd/resources/about.html
+-rw-r--r--   0 franck    (1000) franck    (1000)   146525 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/utils/abcd/resources/d3.min.js
+-rw-r--r--   0 franck    (1000) franck    (1000)     1689 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/utils/abcd/resources/model.js
+drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2024-06-03 11:00:13.000000 SNAKES-0.9.33/snakes/utils/abcd/resources/js/
+-rw-r--r--   0 franck    (1000) franck    (1000)    29110 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/utils/abcd/resources/js/bootstrap.min.js
+-rw-r--r--   0 franck    (1000) franck    (1000)      923 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/utils/abcd/resources/js/petri.js
+-rw-r--r--   0 franck    (1000) franck    (1000)     4602 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/utils/abcd/resources/js/bootstrap.file-input.js
+-rw-r--r--   0 franck    (1000) franck    (1000)     1939 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/utils/abcd/resources/simulator.css
+drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2024-06-03 11:00:13.000000 SNAKES-0.9.33/snakes/utils/abcd/resources/css/
+-rw-r--r--   0 franck    (1000) franck    (1000)    73046 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/utils/abcd/resources/css/docs.css
+-rw-r--r--   0 franck    (1000) franck    (1000)   121220 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/utils/abcd/resources/css/bootstrap.css
+-rw-r--r--   0 franck    (1000) franck    (1000)    14936 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/utils/abcd/resources/css/bootstrap-theme.css
+-rw-r--r--   0 franck    (1000) franck    (1000)    38388 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/utils/abcd/resources/css/bootstrap-theme.css.map
+-rw-r--r--   0 franck    (1000) franck    (1000)   245960 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/utils/abcd/resources/css/bootstrap.css.map
+-rw-r--r--   0 franck    (1000) franck    (1000)   247350 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/utils/abcd/resources/jquery.min.js
+-rw-r--r--   0 franck    (1000) franck    (1000)     1806 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/utils/abcd/resources/alive.txt
+-rw-r--r--   0 franck    (1000) franck    (1000)     3880 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/utils/abcd/simul.py
+-rw-r--r--   0 franck    (1000) franck    (1000)    24866 2017-04-19 21:46:39.000000 SNAKES-0.9.33/snakes/utils/abcd/build.py
+-rw-r--r--   0 franck    (1000) franck    (1000)      630 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/utils/abcd/__init__.py
+-rw-r--r--   0 franck    (1000) franck    (1000)     2505 2016-11-15 09:57:29.000000 SNAKES-0.9.33/snakes/utils/abcd/checker.py
+-rw-r--r--   0 franck    (1000) franck    (1000)     3101 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/utils/abcd/transform.py
+-rw-r--r--   0 franck    (1000) franck    (1000)    17492 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/utils/abcd/html.py
+-rw-r--r--   0 franck    (1000) franck    (1000)    10458 2016-10-10 16:27:06.000000 SNAKES-0.9.33/snakes/utils/abcd/main.py
+-rw-r--r--   0 franck    (1000) franck    (1000)    25530 2017-05-18 12:20:59.000000 SNAKES-0.9.33/snakes/utils/apidoc.py
+drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2024-06-03 11:00:13.000000 SNAKES-0.9.33/snakes/utils/simul/
+drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2024-06-03 11:00:13.000000 SNAKES-0.9.33/snakes/utils/simul/resources/
+-rw-r--r--   0 franck    (1000) franck    (1000)        0 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/utils/simul/resources/about.css
+-rw-r--r--   0 franck    (1000) franck    (1000)     1621 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/utils/simul/resources/index.html
+-rw-r--r--   0 franck    (1000) franck    (1000)      195 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/utils/simul/resources/model.html
+-rw-r--r--   0 franck    (1000) franck    (1000)       57 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/utils/simul/resources/model.css
+-rw-r--r--   0 franck    (1000) franck    (1000)     4341 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/utils/simul/resources/simulator.js
+-rw-r--r--   0 franck    (1000) franck    (1000)     2653 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/utils/simul/resources/jquery.periodic.js
+-rw-r--r--   0 franck    (1000) franck    (1000)      241 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/utils/simul/resources/about.html
+-rw-r--r--   0 franck    (1000) franck    (1000)        0 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/utils/simul/resources/about.js
+-rw-r--r--   0 franck    (1000) franck    (1000)        0 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/utils/simul/resources/model.js
+-rw-r--r--   0 franck    (1000) franck    (1000)       57 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/utils/simul/resources/trace.css
+-rw-r--r--   0 franck    (1000) franck    (1000)     1939 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/utils/simul/resources/simulator.css
+-rw-r--r--   0 franck    (1000) franck    (1000)    96381 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/utils/simul/resources/jquery.min.js
+-rw-r--r--   0 franck    (1000) franck    (1000)     1806 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/utils/simul/resources/alive.txt
+-rw-r--r--   0 franck    (1000) franck    (1000)        0 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/utils/simul/resources/trace.js
+-rw-r--r--   0 franck    (1000) franck    (1000)     7237 2023-10-02 11:38:31.000000 SNAKES-0.9.33/snakes/utils/simul/httpd.py
+-rw-r--r--   0 franck    (1000) franck    (1000)     8786 2016-09-16 08:14:17.000000 SNAKES-0.9.33/snakes/utils/simul/__init__.py
+-rw-r--r--   0 franck    (1000) franck    (1000)     2548 2015-04-09 12:05:23.000000 SNAKES-0.9.33/snakes/utils/simul/html.py
+-rw-r--r--   0 franck    (1000) franck    (1000)     7139 2023-10-02 11:37:12.000000 SNAKES-0.9.33/snakes/utils/simul/logger.py
+-rw-r--r--   0 franck    (1000) franck    (1000)    52213 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/typing.py
+-rw-r--r--   0 franck    (1000) franck    (1000)    32205 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/data.py
+drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2024-06-03 11:00:13.000000 SNAKES-0.9.33/snakes/lang/
+drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2024-06-03 11:00:13.000000 SNAKES-0.9.33/snakes/lang/pylib/
+-rw-r--r--   0 franck    (1000) franck    (1000)    26841 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/lang/pylib/spark.py
+-rw-r--r--   0 franck    (1000) franck    (1000)        0 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/lang/pylib/__init__.py
+-rw-r--r--   0 franck    (1000) franck    (1000)    14022 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/lang/pylib/unparse.py
+-rw-r--r--   0 franck    (1000) franck    (1000)    11630 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/lang/pylib/asdl.py
+-rw-r--r--   0 franck    (1000) franck    (1000)    10324 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/lang/astpypy.py
+drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2024-06-03 11:00:13.000000 SNAKES-0.9.33/snakes/lang/ctlstar/
+-rw-r--r--   0 franck    (1000) franck    (1000)    27179 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/lang/ctlstar/parser.py
+-rw-r--r--   0 franck    (1000) franck    (1000)        0 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/lang/ctlstar/__init__.py
+-rw-r--r--   0 franck    (1000) franck    (1000)   286604 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/lang/ctlstar/pgen.py
+-rw-r--r--   0 franck    (1000) franck    (1000)    29069 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/lang/ctlstar/asdl.py
+-rw-r--r--   0 franck    (1000) franck    (1000)    10235 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/lang/astjy25.py
+-rw-r--r--   0 franck    (1000) franck    (1000)    11933 2023-10-02 11:39:38.000000 SNAKES-0.9.33/snakes/lang/astpy25.py
+-rw-r--r--   0 franck    (1000) franck    (1000)     6396 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/lang/__init__.py
+-rw-r--r--   0 franck    (1000) franck    (1000)    49093 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/lang/pgen.py
+-rw-r--r--   0 franck    (1000) franck    (1000)    14221 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/lang/unparse.py
+drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2024-06-03 11:00:13.000000 SNAKES-0.9.33/snakes/lang/abcd/
+-rw-r--r--   0 franck    (1000) franck    (1000)    37555 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/lang/abcd/parser.py
+-rw-r--r--   0 franck    (1000) franck    (1000)        0 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/lang/abcd/__init__.py
+-rw-r--r--   0 franck    (1000) franck    (1000)   290093 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/lang/abcd/pgen.py
+-rw-r--r--   0 franck    (1000) franck    (1000)    31781 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/lang/abcd/asdl.py
+-rw-r--r--   0 franck    (1000) franck    (1000)     9839 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/lang/asdl.py
+drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2024-06-03 11:00:13.000000 SNAKES-0.9.33/snakes/lang/python/
+-rw-r--r--   0 franck    (1000) franck    (1000)    97603 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/lang/python/parser.py
+-rw-r--r--   0 franck    (1000) franck    (1000)        0 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/lang/python/__init__.py
+-rw-r--r--   0 franck    (1000) franck    (1000)   210533 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/lang/python/pgen.py
+-rw-r--r--   0 franck    (1000) franck    (1000)    22425 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/lang/python/asdl.py
+drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2024-06-03 11:00:13.000000 SNAKES-0.9.33/snakes/plugins/
+-rw-r--r--   0 franck    (1000) franck    (1000)    25669 2017-05-18 12:25:58.000000 SNAKES-0.9.33/snakes/plugins/status.py
+-rw-r--r--   0 franck    (1000) franck    (1000)     5850 2017-09-12 12:54:19.000000 SNAKES-0.9.33/snakes/plugins/bound.py
+-rw-r--r--   0 franck    (1000) franck    (1000)    38797 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/plugins/synchro.py
+-rw-r--r--   0 franck    (1000) franck    (1000)    11054 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/plugins/pids.py
+-rw-r--r--   0 franck    (1000) franck    (1000)     9577 2024-05-03 08:14:37.000000 SNAKES-0.9.33/snakes/plugins/query.py
+-rw-r--r--   0 franck    (1000) franck    (1000)     7759 2024-05-03 08:14:59.000000 SNAKES-0.9.33/snakes/plugins/__init__.py
+-rw-r--r--   0 franck    (1000) franck    (1000)    17105 2023-03-16 10:10:42.000000 SNAKES-0.9.33/snakes/plugins/gv.py
+-rw-r--r--   0 franck    (1000) franck    (1000)    11004 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/plugins/labels.py
+-rw-r--r--   0 franck    (1000) franck    (1000)     4689 2017-11-05 15:30:00.000000 SNAKES-0.9.33/snakes/plugins/modules.py
+-rw-r--r--   0 franck    (1000) franck    (1000)     1022 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/plugins/hello.py
+-rw-r--r--   0 franck    (1000) franck    (1000)    13387 2017-05-18 12:24:24.000000 SNAKES-0.9.33/snakes/plugins/pos.py
+-rw-r--r--   0 franck    (1000) franck    (1000)    15116 2023-04-26 13:16:22.000000 SNAKES-0.9.33/snakes/plugins/clusters.py
+-rw-r--r--   0 franck    (1000) franck    (1000)     3461 2016-10-10 16:15:27.000000 SNAKES-0.9.33/snakes/plugins/let.py
+-rw-r--r--   0 franck    (1000) franck    (1000)    11449 2017-05-18 12:26:14.000000 SNAKES-0.9.33/snakes/plugins/ops.py
+-rw-r--r--   0 franck    (1000) franck    (1000)   158725 2024-05-03 08:16:06.000000 SNAKES-0.9.33/snakes/nets.py
+-rw-r--r--   0 franck    (1000) franck    (1000)    11922 2015-03-14 16:15:28.000000 SNAKES-0.9.33/snakes/hashables.py
+-rw-r--r--   0 franck    (1000) franck    (1000)    31010 2024-05-03 08:03:58.000000 SNAKES-0.9.33/snakes/pnml.py
+-rw-rw-r--   0 franck    (1000) franck    (1000)     1603 2024-06-03 10:56:37.000000 SNAKES-0.9.33/snakes/__init__.py
+-rw-r--r--   0 franck    (1000) franck    (1000)      688 2024-05-03 08:13:53.000000 SNAKES-0.9.33/snakes/compat.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `SNAKES-0.9.32/LICENCE.md` & `SNAKES-0.9.33/LICENCE.md`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/MANIFEST` & `SNAKES-0.9.33/MANIFEST`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/Makefile` & `SNAKES-0.9.33/Makefile`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/PKG-INFO` & `SNAKES-0.9.33/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: SNAKES
-Version: 0.9.32
+Version: 0.9.33
 Summary: SNAKES is the Net Algebra Kit for Editors and Simulators
 Home-page: http://snakes.ibisc.univ-evry.fr/
 Author: Franck Pommereau
 Author-email: franck.pommereau@univ-evry.fr
 License: UNKNOWN
 Description: SNAKES is a general purpose Petri net Python
         library allowing to define and execute most classes of Petri
```

### Comparing `SNAKES-0.9.32/README.md` & `SNAKES-0.9.33/README.md`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/bin/snkc` & `SNAKES-0.9.33/bin/snkc`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/bin/snkd` & `SNAKES-0.9.33/bin/snkd`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/doc/COPYING` & `SNAKES-0.9.33/doc/COPYING`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/doc/abcd.txt` & `SNAKES-0.9.33/doc/abcd.txt`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/doc/examples/abcd/ns/dolev_yao.py` & `SNAKES-0.9.33/doc/examples/abcd/ns/dolev_yao.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/doc/examples/abcd/ns/ns.abcd` & `SNAKES-0.9.33/doc/examples/abcd/ns/ns.abcd`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/doc/examples/abcd/ns/ns.py` & `SNAKES-0.9.33/doc/examples/abcd/ns/ns.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/doc/examples/abcd/railroad.abcd` & `SNAKES-0.9.33/doc/examples/abcd/railroad.abcd`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/doc/queries.txt` & `SNAKES-0.9.33/doc/queries.txt`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/doc/simple-coloured.pnml` & `SNAKES-0.9.33/doc/simple-coloured.pnml`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/doc/simple-pt.pnml` & `SNAKES-0.9.33/doc/simple-pt.pnml`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/doc/snakes-pnml.txt` & `SNAKES-0.9.33/doc/snakes-pnml.txt`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/doc/tutorial.png` & `SNAKES-0.9.33/doc/tutorial.png`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/doc/tutorial.txt` & `SNAKES-0.9.33/doc/tutorial.txt`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/mklang.py` & `SNAKES-0.9.33/mklang.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/setup.py` & `SNAKES-0.9.33/setup.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/__init__.py` & `SNAKES-0.9.33/snakes/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 @copyright: (C) 2005-2013 Franck Pommereau
 @license: GNU Lesser General Public Licence (aka. GNU LGPL), see the
     file `doc/COPYING` in the distribution or visit the [GNU web
     site](http://www.gnu.org/licenses/licenses.html#LGPL)
 @contact: franck.pommereau@ibisc.univ-evry.fr
 """
 
-version = "0.9.32"
+version = "0.9.33"
 defaultencoding = "utf-8"
 
 """## Module `snakes`
 
 This module only provides the exceptions used throughout SNAKES.
 """
```

### Comparing `SNAKES-0.9.32/snakes/compat.py` & `SNAKES-0.9.33/snakes/compat.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,7 +36,14 @@
 
 try :
     unicode
 except NameError :
     unicode = str
 
 PY3 = sys.version > "3"
+
+try:
+    from imp import new_module
+except (NameError, ImportError):
+    import types
+    def new_module(name):
+        return types.ModuleType(name)
```

### Comparing `SNAKES-0.9.32/snakes/data.py` & `SNAKES-0.9.33/snakes/data.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/hashables.py` & `SNAKES-0.9.33/snakes/hashables.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/lang/__init__.py` & `SNAKES-0.9.33/snakes/lang/__init__.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/lang/abcd/asdl.py` & `SNAKES-0.9.33/snakes/lang/abcd/asdl.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/lang/abcd/parser.py` & `SNAKES-0.9.33/snakes/lang/abcd/parser.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/lang/abcd/pgen.py` & `SNAKES-0.9.33/snakes/lang/abcd/pgen.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/lang/asdl.py` & `SNAKES-0.9.33/snakes/lang/asdl.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/lang/astjy25.py` & `SNAKES-0.9.33/snakes/lang/astjy25.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/lang/astpy25.py` & `SNAKES-0.9.33/snakes/lang/astpy25.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/lang/astpypy.py` & `SNAKES-0.9.33/snakes/lang/astpypy.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/lang/ctlstar/asdl.py` & `SNAKES-0.9.33/snakes/lang/ctlstar/asdl.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/lang/ctlstar/parser.py` & `SNAKES-0.9.33/snakes/lang/ctlstar/parser.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/lang/ctlstar/pgen.py` & `SNAKES-0.9.33/snakes/lang/ctlstar/pgen.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/lang/pgen.py` & `SNAKES-0.9.33/snakes/lang/pgen.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/lang/pylib/asdl.py` & `SNAKES-0.9.33/snakes/lang/pylib/asdl.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/lang/pylib/spark.py` & `SNAKES-0.9.33/snakes/lang/pylib/spark.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/lang/pylib/unparse.py` & `SNAKES-0.9.33/snakes/lang/pylib/unparse.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/lang/python/asdl.py` & `SNAKES-0.9.33/snakes/lang/python/asdl.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/lang/python/parser.py` & `SNAKES-0.9.33/snakes/lang/python/parser.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/lang/python/pgen.py` & `SNAKES-0.9.33/snakes/lang/python/pgen.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/lang/unparse.py` & `SNAKES-0.9.33/snakes/lang/unparse.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/nets.py` & `SNAKES-0.9.33/snakes/nets.py`

 * *Files 0% similar despite different names*

```diff
@@ -658,15 +658,15 @@
         @type binding: `Substitution`
         """
         pass
 
 class Variable (ArcAnnotation) :
     "A variable which may be bound to a token."
     input_allowed = True
-    syntax = re.compile("^[a-zA-Z]\w*$")
+    syntax = re.compile(r"^[a-zA-Z]\w*$")
     def __init__ (self, name) :
         """Variable names must start with a letter and may continue with
         any alphanumeric character.
 
         >>> Variable('x')
         Variable('x')
         >>> try : Variable('_test')
```

### Comparing `SNAKES-0.9.32/snakes/plugins/__init__.py` & `SNAKES-0.9.33/snakes/plugins/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,16 +45,17 @@
 >>> n = PetriNet('a net')
 >>> n.hello()  # works thanks to plugin `hello`
 Hello from a net
 >>> n.bbox()   # works thanks to plugin `pos`
 ((0, 0), (0, 0))
 """
 
-import imp, sys, inspect
+import sys, inspect
 from functools import wraps
+from snakes.compat import new_module
 
 # apidoc skip
 def update (module, objects) :
     """Update a module content
     """
     for obj in objects :
         if isinstance(obj, tuple) :
@@ -199,15 +200,15 @@
     @param module: the extended module
     @type module: `module`
     @param objects: the sub-objects
     @type objects: each is a class object
     @return: the new module
     @rtype: `module`
     """
-    result = imp.new_module(name)
+    result = new_module(name)
     result.__dict__.update(module.__dict__)
     update(result, objects)
     result.__plugins__ = (module.__dict__.get("__plugins__",
                                               (module.__name__,))
                           + (name,))
     for obj in objects :
         if inspect.isclass(obj) :
```

### Comparing `SNAKES-0.9.32/snakes/plugins/bound.py` & `SNAKES-0.9.33/snakes/plugins/bound.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/plugins/clusters.py` & `SNAKES-0.9.33/snakes/plugins/clusters.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/plugins/gv.py` & `SNAKES-0.9.33/snakes/plugins/gv.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/plugins/hello.py` & `SNAKES-0.9.33/snakes/plugins/hello.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/plugins/labels.py` & `SNAKES-0.9.33/snakes/plugins/labels.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/plugins/let.py` & `SNAKES-0.9.33/snakes/plugins/let.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/plugins/modules.py` & `SNAKES-0.9.33/snakes/plugins/modules.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/plugins/ops.py` & `SNAKES-0.9.33/snakes/plugins/ops.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/plugins/pids.py` & `SNAKES-0.9.33/snakes/plugins/pids.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/plugins/pos.py` & `SNAKES-0.9.33/snakes/plugins/pos.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/plugins/query.py` & `SNAKES-0.9.33/snakes/plugins/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 @todo: revise (actually make) documentation
 """
 
+from snakes.compat import new_module
 from snakes.plugins import plugin
 from snakes.pnml import Tree, loads, dumps
-import imp, sys, socket, traceback, operator
+import sys, socket, traceback, operator
 
 class QueryError (Exception) :
     pass
 
 class Query (object) :
     def __init__ (self, name, *larg, **karg) :
         self._name = name
@@ -112,15 +113,15 @@
                 for child in tree.get_children("argument"))
         karg = dict((child["name"], child.child().to_obj())
                     for child in tree.get_children("keyword"))
         return cls(tree["name"], *larg, **karg)
     def run (self, envt) :
         """
         >>> import imp
-        >>> env = imp.new_module('environment')
+        >>> env = new_module('environment')
         >>> Query('set', 'x', 'hello').run(env)
         >>> env.x
         'hello'
         >>> Query('set', 'x', Query('call', 'x.upper')).run(env)
         >>> env.x
         'HELLO'
         >>> Query('test', 1, 2, 3).run(env)
@@ -152,48 +153,48 @@
         obj = self._envt
         for n in path :
             obj = getattr(obj, n)
         return obj
     def _run_set (self, name, value) :
         """
         >>> import imp
-        >>> env = imp.new_module('environment')
+        >>> env = new_module('environment')
         >>> Query('set', 'x', 1).run(env)
         >>> env.x
         1
         """
         path = name.split(".")
         setattr(self._get_object(path[:-1]), path[-1], value)
     def _run_get (self, name) :
         """
         >>> import imp
-        >>> env = imp.new_module('environment')
+        >>> env = new_module('environment')
         >>> env.x = 2
         >>> Query('get', 'x').run(env)
         2
         """
         path = name.split(".")
         return self._get_object(path)
     def _run_del (self, name) :
         """
         >>> import imp
-        >>> env = imp.new_module('environment')
+        >>> env = new_module('environment')
         >>> env.x = 2
         >>> Query('del', 'x').run(env)
         >>> env.x
         Traceback (most recent call last):
          ...
         AttributeError: 'module' object has no attribute 'x'
         """
         path = name.split(".")
         delattr(self._get_object(path[:-1]), path[-1])
     def _run_call (self, fun, *larg, **karg) :
         """
         >>> import imp
-        >>> env = imp.new_module('environment')
+        >>> env = new_module('environment')
         >>> env.x = 'hello'
         >>> Query('call', 'x.center', 7).run(env)
         ' hello '
         >>> env.__dict__.update(__builtins__)
         >>> Query('call', Query('call', 'getattr',
         ...                     Query('call', 'x.center', 7),
         ...                     'upper')).run(env)
@@ -207,15 +208,15 @@
 def extend (module) :
     class UDPServer (object) :
         def __init__ (self, port, size=2**20, verbose=0) :
             self._size = size
             self._verbose = verbose
             self._sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
             self._sock.bind(("", port))
-            self._env = imp.new_module("snk")
+            self._env = new_module("snk")
             self._env.__dict__.update(__builtins__)
             self._env.__dict__.update(operator.__dict__)
             self._env.__dict__.update(module.__dict__)
         def recvfrom (self) :
             return self._sock.recvfrom(self._size)
         def sendto (self, data, address) :
             self._sock.sendto(data.strip() + "\n", address)
@@ -255,15 +256,15 @@
     class TCPServer (UDPServer) :
         def __init__ (self, port, size=2**20, verbose=0) :
             self._size = size
             self._verbose = verbose
             self._sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
             self._sock.bind(("", port))
             self._sock.listen(1)
-            self._env = imp.new_module("snk")
+            self._env = new_module("snk")
             self._env.__dict__.update(__builtins__)
             self._env.__dict__.update(operator.__dict__)
             self._env.__dict__.update(module.__dict__)
             self._connection = {}
         def recvfrom (self) :
             connection, address = self._sock.accept()
             self._connection[address] = connection
```

### Comparing `SNAKES-0.9.32/snakes/plugins/status.py` & `SNAKES-0.9.33/snakes/plugins/status.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/plugins/synchro.py` & `SNAKES-0.9.33/snakes/plugins/synchro.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/pnml.py` & `SNAKES-0.9.33/snakes/pnml.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 @warning: this module will be replaced in a future version of SNAKES,
     so its documentation will be kept minimal.
 """
 
 import xml.dom.minidom
 import pickle
-import sys, inspect, os, os.path, imp, pkgutil
+import sys, inspect, os, os.path, pkgutil
 import snakes, snakes.plugins
 from snakes import SnakesError
 from snakes.compat import *
 if PY3 :
     import ast
 
 try :
```

### Comparing `SNAKES-0.9.32/snakes/typing.py` & `SNAKES-0.9.33/snakes/typing.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/utils/abcd/__init__.py` & `SNAKES-0.9.33/snakes/utils/abcd/__init__.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/utils/abcd/build.py` & `SNAKES-0.9.33/snakes/utils/abcd/build.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/utils/abcd/checker.py` & `SNAKES-0.9.33/snakes/utils/abcd/checker.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/utils/abcd/html.py` & `SNAKES-0.9.33/snakes/utils/abcd/html.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/utils/abcd/main.py` & `SNAKES-0.9.33/snakes/utils/abcd/main.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/utils/abcd/resources/alive.txt` & `SNAKES-0.9.33/snakes/utils/abcd/resources/alive.txt`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/utils/abcd/resources/css/bootstrap-theme.css` & `SNAKES-0.9.33/snakes/utils/abcd/resources/css/bootstrap-theme.css`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/utils/abcd/resources/css/bootstrap-theme.css.map` & `SNAKES-0.9.33/snakes/utils/abcd/resources/css/bootstrap-theme.css.map`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/utils/abcd/resources/css/bootstrap.css` & `SNAKES-0.9.33/snakes/utils/abcd/resources/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/utils/abcd/resources/css/bootstrap.css.map` & `SNAKES-0.9.33/snakes/utils/abcd/resources/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/utils/abcd/resources/css/docs.css` & `SNAKES-0.9.33/snakes/utils/abcd/resources/css/docs.css`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/utils/abcd/resources/d3.min.js` & `SNAKES-0.9.33/snakes/utils/abcd/resources/d3.min.js`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/utils/abcd/resources/fonts/glyphicons-halflings-regular.eot` & `SNAKES-0.9.33/snakes/utils/abcd/resources/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/utils/abcd/resources/fonts/glyphicons-halflings-regular.svg` & `SNAKES-0.9.33/snakes/utils/abcd/resources/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/utils/abcd/resources/fonts/glyphicons-halflings-regular.ttf` & `SNAKES-0.9.33/snakes/utils/abcd/resources/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/utils/abcd/resources/fonts/glyphicons-halflings-regular.woff` & `SNAKES-0.9.33/snakes/utils/abcd/resources/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/utils/abcd/resources/index.html` & `SNAKES-0.9.33/snakes/utils/abcd/resources/index.html`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/utils/abcd/resources/jquery.min.js` & `SNAKES-0.9.33/snakes/utils/abcd/resources/jquery.min.js`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/utils/abcd/resources/jquery.periodic.js` & `SNAKES-0.9.33/snakes/utils/abcd/resources/jquery.periodic.js`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/utils/abcd/resources/js/bootstrap.file-input.js` & `SNAKES-0.9.33/snakes/utils/abcd/resources/js/bootstrap.file-input.js`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/utils/abcd/resources/js/bootstrap.min.js` & `SNAKES-0.9.33/snakes/utils/abcd/resources/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/utils/abcd/resources/js/petri.js` & `SNAKES-0.9.33/snakes/utils/abcd/resources/js/petri.js`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/utils/abcd/resources/model.css` & `SNAKES-0.9.33/snakes/utils/abcd/resources/model.css`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/utils/abcd/resources/model.html` & `SNAKES-0.9.33/snakes/utils/abcd/resources/model.html`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/utils/abcd/resources/model.js` & `SNAKES-0.9.33/snakes/utils/abcd/resources/model.js`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/utils/abcd/resources/simulator.css` & `SNAKES-0.9.33/snakes/utils/abcd/resources/simulator.css`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/utils/abcd/resources/simulator.js` & `SNAKES-0.9.33/snakes/utils/abcd/resources/simulator.js`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/utils/abcd/simul.py` & `SNAKES-0.9.33/snakes/utils/abcd/simul.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/utils/abcd/transform.py` & `SNAKES-0.9.33/snakes/utils/abcd/transform.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/utils/apidoc.py` & `SNAKES-0.9.33/snakes/utils/apidoc.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/utils/ctlstar/__init__.py` & `SNAKES-0.9.33/snakes/utils/ctlstar/__init__.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/utils/ctlstar/build.py` & `SNAKES-0.9.33/snakes/utils/ctlstar/build.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/utils/simul/__init__.py` & `SNAKES-0.9.33/snakes/utils/simul/__init__.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/utils/simul/html.py` & `SNAKES-0.9.33/snakes/utils/simul/html.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/utils/simul/httpd.py` & `SNAKES-0.9.33/snakes/utils/simul/httpd.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/utils/simul/logger.py` & `SNAKES-0.9.33/snakes/utils/simul/logger.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/utils/simul/resources/alive.txt` & `SNAKES-0.9.33/snakes/utils/simul/resources/alive.txt`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/utils/simul/resources/index.html` & `SNAKES-0.9.33/snakes/utils/simul/resources/index.html`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/utils/simul/resources/jquery.min.js` & `SNAKES-0.9.33/snakes/utils/simul/resources/jquery.min.js`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/utils/simul/resources/jquery.periodic.js` & `SNAKES-0.9.33/snakes/utils/simul/resources/jquery.periodic.js`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/utils/simul/resources/simulator.css` & `SNAKES-0.9.33/snakes/utils/simul/resources/simulator.css`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/snakes/utils/simul/resources/simulator.js` & `SNAKES-0.9.33/snakes/utils/simul/resources/simulator.js`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/test.py` & `SNAKES-0.9.33/test.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/utils/abcd-mode.elc` & `SNAKES-0.9.33/utils/abcd-mode.elc`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.32/version.py` & `SNAKES-0.9.33/version.py`

 * *Files identical despite different names*

