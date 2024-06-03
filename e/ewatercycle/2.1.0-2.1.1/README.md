# Comparing `tmp/ewatercycle-2.1.0.tar.gz` & `tmp/ewatercycle-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ewatercycle-2.1.0.tar", last modified: Mon Mar 25 12:47:59 2024, max compression
+gzip compressed data, was "ewatercycle-2.1.1.tar", last modified: Mon Jun  3 08:03:54 2024, max compression
```

## Comparing `ewatercycle-2.1.0.tar` & `ewatercycle-2.1.1.tar`

### file list

```diff
@@ -1,64 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:47:59.622382 ewatercycle-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-25 12:47:53.000000 ewatercycle-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-25 12:47:53.000000 ewatercycle-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7964 2024-03-25 12:47:59.622382 ewatercycle-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5428 2024-03-25 12:47:53.000000 ewatercycle-2.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-03-25 12:47:53.000000 ewatercycle-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-03-25 12:47:59.622382 ewatercycle-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 12:47:53.000000 ewatercycle-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:47:59.610382 ewatercycle-2.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:47:59.614382 ewatercycle-2.1.0/src/ewatercycle/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-25 12:47:53.000000 ewatercycle-2.1.0/src/ewatercycle/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:47:59.618382 ewatercycle-2.1.0/src/ewatercycle/_forcings/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 12:47:53.000000 ewatercycle-2.1.0/src/ewatercycle/_forcings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-03-25 12:47:53.000000 ewatercycle-2.1.0/src/ewatercycle/_forcings/makkink.py
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-03-25 12:47:53.000000 ewatercycle-2.1.0/src/ewatercycle/_repr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:47:59.618382 ewatercycle-2.1.0/src/ewatercycle/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-03-25 12:47:53.000000 ewatercycle-2.1.0/src/ewatercycle/analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:47:59.618382 ewatercycle-2.1.0/src/ewatercycle/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 12:47:53.000000 ewatercycle-2.1.0/src/ewatercycle/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21922 2024-03-25 12:47:53.000000 ewatercycle-2.1.0/src/ewatercycle/base/forcing.py
--rw-r--r--   0 runner    (1001) docker     (127)    14236 2024-03-25 12:47:53.000000 ewatercycle-2.1.0/src/ewatercycle/base/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9459 2024-03-25 12:47:53.000000 ewatercycle-2.1.0/src/ewatercycle/base/parameter_set.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:47:59.618382 ewatercycle-2.1.0/src/ewatercycle/config/
--rw-r--r--   0 runner    (1001) docker     (127)    11137 2024-03-25 12:47:53.000000 ewatercycle-2.1.0/src/ewatercycle/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14373 2024-03-25 12:47:53.000000 ewatercycle-2.1.0/src/ewatercycle/container.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:47:59.618382 ewatercycle-2.1.0/src/ewatercycle/esmvaltool/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-25 12:47:53.000000 ewatercycle-2.1.0/src/ewatercycle/esmvaltool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14468 2024-03-25 12:47:53.000000 ewatercycle-2.1.0/src/ewatercycle/esmvaltool/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-03-25 12:47:53.000000 ewatercycle-2.1.0/src/ewatercycle/esmvaltool/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:47:59.618382 ewatercycle-2.1.0/src/ewatercycle/esmvaltool/diagnostic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 12:47:53.000000 ewatercycle-2.1.0/src/ewatercycle/esmvaltool/diagnostic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-03-25 12:47:53.000000 ewatercycle-2.1.0/src/ewatercycle/esmvaltool/diagnostic/copier.py
--rw-r--r--   0 runner    (1001) docker     (127)     6049 2024-03-25 12:47:53.000000 ewatercycle-2.1.0/src/ewatercycle/esmvaltool/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     4452 2024-03-25 12:47:53.000000 ewatercycle-2.1.0/src/ewatercycle/esmvaltool/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-03-25 12:47:53.000000 ewatercycle-2.1.0/src/ewatercycle/forcing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-03-25 12:47:53.000000 ewatercycle-2.1.0/src/ewatercycle/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:47:59.618382 ewatercycle-2.1.0/src/ewatercycle/observation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 12:47:53.000000 ewatercycle-2.1.0/src/ewatercycle/observation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10641 2024-03-25 12:47:53.000000 ewatercycle-2.1.0/src/ewatercycle/observation/grdc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-03-25 12:47:53.000000 ewatercycle-2.1.0/src/ewatercycle/observation/usgs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-03-25 12:47:53.000000 ewatercycle-2.1.0/src/ewatercycle/parameter_sets.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 12:47:53.000000 ewatercycle-2.1.0/src/ewatercycle/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-03-25 12:47:53.000000 ewatercycle-2.1.0/src/ewatercycle/shared.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:47:59.618382 ewatercycle-2.1.0/src/ewatercycle/testing/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-25 12:47:53.000000 ewatercycle-2.1.0/src/ewatercycle/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:47:59.614382 ewatercycle-2.1.0/src/ewatercycle/testing/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:47:59.622382 ewatercycle-2.1.0/src/ewatercycle/testing/data/Rhine/
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-03-25 12:47:53.000000 ewatercycle-2.1.0/src/ewatercycle/testing/data/Rhine/Rhine.dbf
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-25 12:47:53.000000 ewatercycle-2.1.0/src/ewatercycle/testing/data/Rhine/Rhine.prj
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-25 12:47:53.000000 ewatercycle-2.1.0/src/ewatercycle/testing/data/Rhine/Rhine.qpj
--rw-r--r--   0 runner    (1001) docker     (127)    93372 2024-03-25 12:47:53.000000 ewatercycle-2.1.0/src/ewatercycle/testing/data/Rhine/Rhine.shp
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-25 12:47:53.000000 ewatercycle-2.1.0/src/ewatercycle/testing/data/Rhine/Rhine.shx
--rw-r--r--   0 runner    (1001) docker     (127)     6242 2024-03-25 12:47:53.000000 ewatercycle-2.1.0/src/ewatercycle/testing/fake_models.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-03-25 12:47:53.000000 ewatercycle-2.1.0/src/ewatercycle/testing/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-03-25 12:47:53.000000 ewatercycle-2.1.0/src/ewatercycle/testing/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    10978 2024-03-25 12:47:53.000000 ewatercycle-2.1.0/src/ewatercycle/util.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-25 12:47:53.000000 ewatercycle-2.1.0/src/ewatercycle/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:47:59.622382 ewatercycle-2.1.0/src/ewatercycle.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7964 2024-03-25 12:47:59.000000 ewatercycle-2.1.0/src/ewatercycle.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-03-25 12:47:59.000000 ewatercycle-2.1.0/src/ewatercycle.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 12:47:59.000000 ewatercycle-2.1.0/src/ewatercycle.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 12:47:59.000000 ewatercycle-2.1.0/src/ewatercycle.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-03-25 12:47:59.000000 ewatercycle-2.1.0/src/ewatercycle.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-25 12:47:59.000000 ewatercycle-2.1.0/src/ewatercycle.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:03:54.735207 ewatercycle-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-06-03 08:03:50.000000 ewatercycle-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-06-03 08:03:50.000000 ewatercycle-2.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8037 2024-06-03 08:03:54.735207 ewatercycle-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5435 2024-06-03 08:03:50.000000 ewatercycle-2.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-06-03 08:03:50.000000 ewatercycle-2.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-06-03 08:03:54.735207 ewatercycle-2.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 08:03:50.000000 ewatercycle-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:03:54.723207 ewatercycle-2.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:03:54.727207 ewatercycle-2.1.1/src/ewatercycle/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-06-03 08:03:50.000000 ewatercycle-2.1.1/src/ewatercycle/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:03:54.727207 ewatercycle-2.1.1/src/ewatercycle/_forcings/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 08:03:50.000000 ewatercycle-2.1.1/src/ewatercycle/_forcings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11634 2024-06-03 08:03:50.000000 ewatercycle-2.1.1/src/ewatercycle/_forcings/caravan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-06-03 08:03:50.000000 ewatercycle-2.1.1/src/ewatercycle/_forcings/makkink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-06-03 08:03:50.000000 ewatercycle-2.1.1/src/ewatercycle/_repr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:03:54.727207 ewatercycle-2.1.1/src/ewatercycle/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-06-03 08:03:50.000000 ewatercycle-2.1.1/src/ewatercycle/analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:03:54.727207 ewatercycle-2.1.1/src/ewatercycle/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 08:03:50.000000 ewatercycle-2.1.1/src/ewatercycle/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21937 2024-06-03 08:03:50.000000 ewatercycle-2.1.1/src/ewatercycle/base/forcing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14539 2024-06-03 08:03:50.000000 ewatercycle-2.1.1/src/ewatercycle/base/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9459 2024-06-03 08:03:50.000000 ewatercycle-2.1.1/src/ewatercycle/base/parameter_set.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:03:54.727207 ewatercycle-2.1.1/src/ewatercycle/config/
+-rw-r--r--   0 runner    (1001) docker     (127)    11137 2024-06-03 08:03:50.000000 ewatercycle-2.1.1/src/ewatercycle/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14373 2024-06-03 08:03:50.000000 ewatercycle-2.1.1/src/ewatercycle/container.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:03:54.727207 ewatercycle-2.1.1/src/ewatercycle/esmvaltool/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-06-03 08:03:50.000000 ewatercycle-2.1.1/src/ewatercycle/esmvaltool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14468 2024-06-03 08:03:50.000000 ewatercycle-2.1.1/src/ewatercycle/esmvaltool/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-06-03 08:03:50.000000 ewatercycle-2.1.1/src/ewatercycle/esmvaltool/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:03:54.731207 ewatercycle-2.1.1/src/ewatercycle/esmvaltool/diagnostic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 08:03:50.000000 ewatercycle-2.1.1/src/ewatercycle/esmvaltool/diagnostic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-06-03 08:03:50.000000 ewatercycle-2.1.1/src/ewatercycle/esmvaltool/diagnostic/copier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6049 2024-06-03 08:03:50.000000 ewatercycle-2.1.1/src/ewatercycle/esmvaltool/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4452 2024-06-03 08:03:50.000000 ewatercycle-2.1.1/src/ewatercycle/esmvaltool/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-06-03 08:03:50.000000 ewatercycle-2.1.1/src/ewatercycle/forcing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-06-03 08:03:50.000000 ewatercycle-2.1.1/src/ewatercycle/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:03:54.731207 ewatercycle-2.1.1/src/ewatercycle/observation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 08:03:50.000000 ewatercycle-2.1.1/src/ewatercycle/observation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10641 2024-06-03 08:03:50.000000 ewatercycle-2.1.1/src/ewatercycle/observation/grdc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-06-03 08:03:50.000000 ewatercycle-2.1.1/src/ewatercycle/observation/usgs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-06-03 08:03:50.000000 ewatercycle-2.1.1/src/ewatercycle/parameter_sets.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 08:03:50.000000 ewatercycle-2.1.1/src/ewatercycle/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-06-03 08:03:50.000000 ewatercycle-2.1.1/src/ewatercycle/shared.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:03:54.731207 ewatercycle-2.1.1/src/ewatercycle/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-06-03 08:03:50.000000 ewatercycle-2.1.1/src/ewatercycle/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:03:54.723207 ewatercycle-2.1.1/src/ewatercycle/testing/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:03:54.731207 ewatercycle-2.1.1/src/ewatercycle/testing/data/Rhine/
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-06-03 08:03:50.000000 ewatercycle-2.1.1/src/ewatercycle/testing/data/Rhine/Rhine.dbf
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-06-03 08:03:50.000000 ewatercycle-2.1.1/src/ewatercycle/testing/data/Rhine/Rhine.prj
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-06-03 08:03:50.000000 ewatercycle-2.1.1/src/ewatercycle/testing/data/Rhine/Rhine.qpj
+-rw-r--r--   0 runner    (1001) docker     (127)    93372 2024-06-03 08:03:50.000000 ewatercycle-2.1.1/src/ewatercycle/testing/data/Rhine/Rhine.shp
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-06-03 08:03:50.000000 ewatercycle-2.1.1/src/ewatercycle/testing/data/Rhine/Rhine.shx
+-rw-r--r--   0 runner    (1001) docker     (127)     6296 2024-06-03 08:03:50.000000 ewatercycle-2.1.1/src/ewatercycle/testing/fake_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-06-03 08:03:50.000000 ewatercycle-2.1.1/src/ewatercycle/testing/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-06-03 08:03:50.000000 ewatercycle-2.1.1/src/ewatercycle/testing/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11350 2024-06-03 08:03:50.000000 ewatercycle-2.1.1/src/ewatercycle/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-06-03 08:03:50.000000 ewatercycle-2.1.1/src/ewatercycle/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:03:54.731207 ewatercycle-2.1.1/src/ewatercycle.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8037 2024-06-03 08:03:54.000000 ewatercycle-2.1.1/src/ewatercycle.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-06-03 08:03:54.000000 ewatercycle-2.1.1/src/ewatercycle.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 08:03:54.000000 ewatercycle-2.1.1/src/ewatercycle.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 08:03:54.000000 ewatercycle-2.1.1/src/ewatercycle.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-06-03 08:03:54.000000 ewatercycle-2.1.1/src/ewatercycle.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-06-03 08:03:54.000000 ewatercycle-2.1.1/src/ewatercycle.egg-info/top_level.txt
```

### Comparing `ewatercycle-2.1.0/LICENSE` & `ewatercycle-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ewatercycle-2.1.0/PKG-INFO` & `ewatercycle-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewatercycle
-Version: 2.1.0
+Version: 2.1.1
 Summary: A Python package for running and validating a hydrology model
 Home-page: https://www.ewatercycle.org/
 Author: Stefan Verhoeven
 Author-email: s.verhoeven@esciencecenter.nl
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/eWaterCycle/ewatercycle/issues
 Project-URL: Documentation, https://ewatercycle.readthedocs.io/
@@ -38,14 +38,15 @@
 Requires-Dist: pandas
 Requires-Dist: pydantic>=2
 Requires-Dist: pyoos
 Requires-Dist: python-dateutil
 Requires-Dist: ruamel.yaml
 Requires-Dist: scipy
 Requires-Dist: xarray
+Requires-Dist: dask
 Provides-Extra: dev
 Requires-Dist: black[jupyter]; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Requires-Dist: bump2version; extra == "dev"
 Requires-Dist: deepdiff; extra == "dev"
 Requires-Dist: ipython; extra == "dev"
 Requires-Dist: isort; extra == "dev"
@@ -61,14 +62,15 @@
 Requires-Dist: sphinx; extra == "dev"
 Requires-Dist: sphinx-copybutton; extra == "dev"
 Requires-Dist: sphinx-rtd-theme; extra == "dev"
 Requires-Dist: sphinx-autoapi; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: types-python-dateutil; extra == "dev"
 Requires-Dist: types-PyYAML; extra == "dev"
+Requires-Dist: types-requests; extra == "dev"
 
 # ewatercycle
 
 ![image](https://github.com/eWaterCycle/ewatercycle/raw/main/docs/examples/logo.png)
 
 A Python package for running hydrological models.
 
@@ -191,11 +193,11 @@
 ## Contributing
 
 If you want to contribute to the development of ewatercycle package,
 have a look at the [contribution guidelines](CONTRIBUTING.md).
 
 ## License
 
-Copyright (c) 2018, Netherlands eScience Center & Delft University of
+Copyright (c) 2018 - 2024, Netherlands eScience Center & Delft University of
 Technology
 
 Apache Software License 2.0
```

### Comparing `ewatercycle-2.1.0/README.md` & `ewatercycle-2.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -123,11 +123,11 @@
 ## Contributing
 
 If you want to contribute to the development of ewatercycle package,
 have a look at the [contribution guidelines](CONTRIBUTING.md).
 
 ## License
 
-Copyright (c) 2018, Netherlands eScience Center & Delft University of
+Copyright (c) 2018 - 2024, Netherlands eScience Center & Delft University of
 Technology
 
 Apache Software License 2.0
```

### Comparing `ewatercycle-2.1.0/setup.cfg` & `ewatercycle-2.1.1/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ewatercycle
-version = 2.1.0
+version = 2.1.1
 description = A Python package for running and validating a hydrology model
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://www.ewatercycle.org/
 author = Stefan Verhoeven
 author_email = s.verhoeven@esciencecenter.nl
 license = Apache-2.0
@@ -48,14 +48,15 @@
 	pandas
 	pydantic>=2
 	pyoos
 	python-dateutil
 	ruamel.yaml
 	scipy
 	xarray
+	dask
 python_requires = >=3.10
 package_dir = 
 	= src
 zip_safe = False
 
 [options.packages.find]
 where = src
@@ -80,14 +81,15 @@
 	sphinx
 	sphinx-copybutton
 	sphinx-rtd-theme
 	sphinx-autoapi
 	twine
 	types-python-dateutil
 	types-PyYAML
+	types-requests
 
 [options.package_data]
 ewatercycle = 
 	py.typed
 	testing/data/Rhine/Rhine.*
 
 [coverage:run]
```

### Comparing `ewatercycle-2.1.0/src/ewatercycle/_forcings/makkink.py` & `ewatercycle-2.1.1/src/ewatercycle/_forcings/makkink.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,22 @@
 )
 from ewatercycle.esmvaltool.schema import Dataset
 from ewatercycle.util import merge_esvmaltool_datasets
 
 
 def derive_e_pot(recipe_output: dict) -> tuple[str, ...]:
     """Derive the Makkink PET from the ESMValTool recipe output."""
-    ds_tas = xr.open_dataset(Path(recipe_output["directory"]) / recipe_output["tas"])
-    ds_rsds = xr.open_dataset(Path(recipe_output["directory"]) / recipe_output["rsds"])
+    ds_tas = xr.open_dataset(
+        Path(recipe_output["directory"]) / recipe_output["tas"],
+        chunks="auto",
+    )
+    ds_rsds = xr.open_dataset(
+        Path(recipe_output["directory"]) / recipe_output["rsds"],
+        chunks="auto",
+    )
     # We need to make sure the coordinates line up. Floating point errors from
     #  ESMValTool mess with this:
     ds = merge_esvmaltool_datasets([ds_tas, ds_rsds])
 
     da_et = et_makkink(ds["tas"], ds["rsds"])
     et_fname = "Derived_Makkink_evspsblpot.nc"
     da_et.to_netcdf(Path(recipe_output["directory"]) / et_fname)
```

### Comparing `ewatercycle-2.1.0/src/ewatercycle/_repr.py` & `ewatercycle-2.1.1/src/ewatercycle/_repr.py`

 * *Files identical despite different names*

### Comparing `ewatercycle-2.1.0/src/ewatercycle/analysis/__init__.py` & `ewatercycle-2.1.1/src/ewatercycle/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `ewatercycle-2.1.0/src/ewatercycle/base/forcing.py` & `ewatercycle-2.1.1/src/ewatercycle/base/forcing.py`

 * *Files 1% similar despite different names*

```diff
@@ -263,15 +263,15 @@
             msg = (
                 "Not all files are netCDF files. Only netCDF files can be opened as "
                 "an xarray Dataset."
             )
             raise ValueError(msg)
         fpaths = [self.directory / filename for _, filename in self.filenames.items()]
 
-        datasets = [xr.open_dataset(fpath) for fpath in fpaths]
+        datasets = [xr.open_dataset(fpath, chunks="auto") for fpath in fpaths]
         return merge_esvmaltool_datasets(datasets)
 
     def variables(self) -> tuple[str, ...]:
         """Return the names of the variables. Shorthand for self.filenames.keys()"""
         return tuple([key for key in self.filenames])
 
     def __eq__(self, other):
```

### Comparing `ewatercycle-2.1.0/src/ewatercycle/base/model.py` & `ewatercycle-2.1.1/src/ewatercycle/base/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -323,14 +323,23 @@
 
     @property
     def output_var_names(self) -> Iterable[str]:
         """List of a model's output variables."""
         return self._bmi.get_output_var_names()
 
     @property
+    def input_var_names(self) -> Iterable[str]:
+        """List of a model's input variables."""
+        return self._bmi.get_input_var_names()
+
+    def var_units(self, name: str) -> str:
+        """Return the given variable's units."""
+        return self._bmi.get_var_units(name)
+
+    @property
     def start_time_as_isostr(self) -> str:
         """Start time of the model.
 
         In UTC and ISO format string e.g. 'YYYY-MM-DDTHH:MM:SSZ'.
         """
         return self.start_time_as_datetime.strftime(ISO_TIMEFMT)
 
@@ -433,15 +442,15 @@
     # Make pydantic accept ContainerImage type.
     model_config = ConfigDict(arbitrary_types_allowed=True)
 
     @property
     def version(self) -> str:
         return self.bmi_image.version
 
-    def _make_bmi_instance(self) -> bmipy.Bmi:
+    def _make_bmi_instance(self) -> OptionalDestBmi:
         if self.parameter_set:
             self._additional_input_dirs.append(str(self.parameter_set.directory))
         if self.forcing:
             self._additional_input_dirs.append(str(self.forcing.directory))
 
         return start_container(
             image=self.bmi_image,
```

### Comparing `ewatercycle-2.1.0/src/ewatercycle/base/parameter_set.py` & `ewatercycle-2.1.1/src/ewatercycle/base/parameter_set.py`

 * *Files identical despite different names*

### Comparing `ewatercycle-2.1.0/src/ewatercycle/config/__init__.py` & `ewatercycle-2.1.1/src/ewatercycle/config/__init__.py`

 * *Files identical despite different names*

### Comparing `ewatercycle-2.1.0/src/ewatercycle/container.py` & `ewatercycle-2.1.1/src/ewatercycle/container.py`

 * *Files identical despite different names*

### Comparing `ewatercycle-2.1.0/src/ewatercycle/esmvaltool/builder.py` & `ewatercycle-2.1.1/src/ewatercycle/esmvaltool/builder.py`

 * *Files identical despite different names*

### Comparing `ewatercycle-2.1.0/src/ewatercycle/esmvaltool/datasets.py` & `ewatercycle-2.1.1/src/ewatercycle/esmvaltool/datasets.py`

 * *Files identical despite different names*

### Comparing `ewatercycle-2.1.0/src/ewatercycle/esmvaltool/diagnostic/copier.py` & `ewatercycle-2.1.1/src/ewatercycle/esmvaltool/diagnostic/copier.py`

 * *Files identical despite different names*

### Comparing `ewatercycle-2.1.0/src/ewatercycle/esmvaltool/run.py` & `ewatercycle-2.1.1/src/ewatercycle/esmvaltool/run.py`

 * *Files identical despite different names*

### Comparing `ewatercycle-2.1.0/src/ewatercycle/esmvaltool/schema.py` & `ewatercycle-2.1.1/src/ewatercycle/esmvaltool/schema.py`

 * *Files identical despite different names*

### Comparing `ewatercycle-2.1.0/src/ewatercycle/forcing.py` & `ewatercycle-2.1.1/src/ewatercycle/forcing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Forcing module of eWaterCycle. Contains the forcing sources."""
 from importlib.metadata import entry_points
 from typing import Any, Type
 
 from ewatercycle import shared
+from ewatercycle._forcings.caravan import CaravanForcing
 from ewatercycle._forcings.makkink import (
     DistributedMakkinkForcing,
     LumpedMakkinkForcing,
 )
 from ewatercycle.base.forcing import (
     DefaultForcing,
     DistributedUserForcing,
@@ -61,14 +62,15 @@
 _forcings: dict[str, Any] = {
     "GenericDistributedForcing": GenericDistributedForcing,
     "GenericLumpedForcing": GenericLumpedForcing,
     "DistributedUserForcing": DistributedUserForcing,
     "LumpedUserForcing": LumpedUserForcing,
     "DistributedMakkinkForcing": DistributedMakkinkForcing,
     "LumpedMakkinkForcing": LumpedMakkinkForcing,
+    "CaravanForcing": CaravanForcing,
 }
 _forcings.update(
     {
         entry_point.name: entry_point
         for entry_point in entry_points(group="ewatercycle.forcings")  # /NOSONAR
     }
 )
```

### Comparing `ewatercycle-2.1.0/src/ewatercycle/observation/grdc.py` & `ewatercycle-2.1.1/src/ewatercycle/observation/grdc.py`

 * *Files identical despite different names*

### Comparing `ewatercycle-2.1.0/src/ewatercycle/observation/usgs.py` & `ewatercycle-2.1.1/src/ewatercycle/observation/usgs.py`

 * *Files identical despite different names*

### Comparing `ewatercycle-2.1.0/src/ewatercycle/parameter_sets.py` & `ewatercycle-2.1.1/src/ewatercycle/parameter_sets.py`

 * *Files identical despite different names*

### Comparing `ewatercycle-2.1.0/src/ewatercycle/shared.py` & `ewatercycle-2.1.1/src/ewatercycle/shared.py`

 * *Files identical despite different names*

### Comparing `ewatercycle-2.1.0/src/ewatercycle/testing/data/Rhine/Rhine.dbf` & `ewatercycle-2.1.1/src/ewatercycle/testing/data/Rhine/Rhine.dbf`

 * *Files identical despite different names*

### Comparing `ewatercycle-2.1.0/src/ewatercycle/testing/data/Rhine/Rhine.shp` & `ewatercycle-2.1.1/src/ewatercycle/testing/data/Rhine/Rhine.shp`

 * *Files identical despite different names*

### Comparing `ewatercycle-2.1.0/src/ewatercycle/testing/fake_models.py` & `ewatercycle-2.1.1/src/ewatercycle/testing/fake_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,14 +216,17 @@
             ],
             dtype=self.dtype,
         )
 
     def get_output_var_names(self) -> tuple[str]:
         return ("plate_surface__temperature",)
 
+    def get_input_var_names(self):
+        return ()
+
     def get_var_type(self, name):
         return str(self.dtype)
 
     def get_var_grid(self, name):
         return 0
 
     def get_var_units(self, name):
```

### Comparing `ewatercycle-2.1.0/src/ewatercycle/testing/fixtures.py` & `ewatercycle-2.1.1/src/ewatercycle/testing/fixtures.py`

 * *Files identical despite different names*

### Comparing `ewatercycle-2.1.0/src/ewatercycle/testing/helpers.py` & `ewatercycle-2.1.1/src/ewatercycle/testing/helpers.py`

 * *Files identical despite different names*

### Comparing `ewatercycle-2.1.0/src/ewatercycle/util.py` & `ewatercycle-2.1.1/src/ewatercycle/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -148,15 +148,15 @@
     ('waldo-on-a-page' precision)[1], while solving the floating point inprecision
     issue.
 
     References:
         [1] Randall Monroe, 2019. xkcd: Coordinate Precision. https://xkcd.com/2170/
     """
     TOLERANCE = 1e-7
-    datasets = copy(datasets)
+    datasets = [ds.copy(deep=True) for ds in datasets]
 
     # First check that the coordinates all line up before merging.
     for coord in ["lat", "lon"]:
         coords = [ds[coord].to_numpy() for ds in datasets]
         if len(set([c.size for c in coords])) > 1:
             msg = f"The coordinate '{coord}' is not of the same size in every dataset."
             raise ValueError(msg)
@@ -191,17 +191,26 @@
             ) + np.timedelta64(12, "h")
             datasets[i] = datasets[i].drop_vars("time_bnds")
 
         # A "height" coordinate can be present, which will result in conflicts.
         #   Instead, we move it to the variable's attributes.
         if "height" in datasets[i].variables:
             data_vars = list(datasets[i].data_vars)
-            if "time_bnds" in data_vars:
-                data_vars.remove("time_bnds")
-            var = data_vars[0]
+            for bnd in ("lat_bnds", "lon_bnds", "time_bnds"):
+                if bnd in data_vars:
+                    data_vars.remove(bnd)
+            if len(data_vars) == 1:
+                var = data_vars[0]
+            else:
+                msg = (
+                    "More than one variable found in dataset. \n"
+                    "This routine can only handle a single data variable per dataset\n"
+                )
+                raise ValueError(msg)
+
             datasets[i][var].attrs.update(
                 {
                     "height": float(datasets[i]["height"]),
                     "height_units": datasets[i]["height"].attrs["units"],
                 }
             )
             datasets[i] = datasets[i].drop_vars(("height",))
```

### Comparing `ewatercycle-2.1.0/src/ewatercycle.egg-info/PKG-INFO` & `ewatercycle-2.1.1/src/ewatercycle.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewatercycle
-Version: 2.1.0
+Version: 2.1.1
 Summary: A Python package for running and validating a hydrology model
 Home-page: https://www.ewatercycle.org/
 Author: Stefan Verhoeven
 Author-email: s.verhoeven@esciencecenter.nl
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/eWaterCycle/ewatercycle/issues
 Project-URL: Documentation, https://ewatercycle.readthedocs.io/
@@ -38,14 +38,15 @@
 Requires-Dist: pandas
 Requires-Dist: pydantic>=2
 Requires-Dist: pyoos
 Requires-Dist: python-dateutil
 Requires-Dist: ruamel.yaml
 Requires-Dist: scipy
 Requires-Dist: xarray
+Requires-Dist: dask
 Provides-Extra: dev
 Requires-Dist: black[jupyter]; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Requires-Dist: bump2version; extra == "dev"
 Requires-Dist: deepdiff; extra == "dev"
 Requires-Dist: ipython; extra == "dev"
 Requires-Dist: isort; extra == "dev"
@@ -61,14 +62,15 @@
 Requires-Dist: sphinx; extra == "dev"
 Requires-Dist: sphinx-copybutton; extra == "dev"
 Requires-Dist: sphinx-rtd-theme; extra == "dev"
 Requires-Dist: sphinx-autoapi; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: types-python-dateutil; extra == "dev"
 Requires-Dist: types-PyYAML; extra == "dev"
+Requires-Dist: types-requests; extra == "dev"
 
 # ewatercycle
 
 ![image](https://github.com/eWaterCycle/ewatercycle/raw/main/docs/examples/logo.png)
 
 A Python package for running hydrological models.
 
@@ -191,11 +193,11 @@
 ## Contributing
 
 If you want to contribute to the development of ewatercycle package,
 have a look at the [contribution guidelines](CONTRIBUTING.md).
 
 ## License
 
-Copyright (c) 2018, Netherlands eScience Center & Delft University of
+Copyright (c) 2018 - 2024, Netherlands eScience Center & Delft University of
 Technology
 
 Apache Software License 2.0
```

### Comparing `ewatercycle-2.1.0/src/ewatercycle.egg-info/SOURCES.txt` & `ewatercycle-2.1.1/src/ewatercycle.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 src/ewatercycle.egg-info/PKG-INFO
 src/ewatercycle.egg-info/SOURCES.txt
 src/ewatercycle.egg-info/dependency_links.txt
 src/ewatercycle.egg-info/not-zip-safe
 src/ewatercycle.egg-info/requires.txt
 src/ewatercycle.egg-info/top_level.txt
 src/ewatercycle/_forcings/__init__.py
+src/ewatercycle/_forcings/caravan.py
 src/ewatercycle/_forcings/makkink.py
 src/ewatercycle/analysis/__init__.py
 src/ewatercycle/base/__init__.py
 src/ewatercycle/base/forcing.py
 src/ewatercycle/base/model.py
 src/ewatercycle/base/parameter_set.py
 src/ewatercycle/config/__init__.py
```

