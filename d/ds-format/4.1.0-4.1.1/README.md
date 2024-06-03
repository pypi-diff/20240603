# Comparing `tmp/ds-format-4.1.0.tar.gz` & `tmp/ds-format-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ds-format-4.1.0.tar", last modified: Fri Feb 16 20:14:34 2024, max compression
+gzip compressed data, was "ds-format-4.1.1.tar", last modified: Mon Jun  3 15:32:31 2024, max compression
```

## Comparing `ds-format-4.1.0.tar` & `ds-format-4.1.1.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-02-16 20:14:34.158317 ds-format-4.1.0/
--rw-r--r--   0 peter     (1000) peter     (1000)     1072 2024-02-16 19:39:20.000000 ds-format-4.1.0/LICENSE.md
--rw-r--r--   0 peter     (1000) peter     (1000)      703 2024-02-16 20:14:34.158317 ds-format-4.1.0/PKG-INFO
--rw-r--r--   0 peter     (1000) peter     (1000)      563 2024-02-16 19:39:20.000000 ds-format-4.1.0/README.md
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-02-16 20:14:34.154317 ds-format-4.1.0/ds_format/
--rw-r--r--   0 peter     (1000) peter     (1000)      681 2024-02-16 19:39:20.000000 ds-format-4.1.0/ds_format/__init__.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-02-16 20:14:34.154317 ds-format-4.1.0/ds_format/bin/
--rw-r--r--   0 peter     (1000) peter     (1000)        0 2024-02-16 19:39:20.000000 ds-format-4.1.0/ds_format/bin/__init__.py
--rwxr-xr-x   0 peter     (1000) peter     (1000)      310 2024-02-16 19:39:20.000000 ds-format-4.1.0/ds_format/bin/ds.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-02-16 20:14:34.154317 ds-format-4.1.0/ds_format/cmd/
--rw-r--r--   0 peter     (1000) peter     (1000)      578 2024-02-16 19:39:20.000000 ds-format-4.1.0/ds_format/cmd/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1645 2024-02-16 19:39:20.000000 ds-format-4.1.0/ds_format/cmd/attrs.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2624 2024-02-16 19:39:20.000000 ds-format-4.1.0/ds_format/cmd/cat.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1212 2024-02-16 19:39:20.000000 ds-format-4.1.0/ds_format/cmd/dims.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2565 2024-02-16 19:39:20.000000 ds-format-4.1.0/ds_format/cmd/ls.py
--rw-r--r--   0 peter     (1000) peter     (1000)     5083 2024-02-16 19:39:20.000000 ds-format-4.1.0/ds_format/cmd/main.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2965 2024-02-16 19:39:20.000000 ds-format-4.1.0/ds_format/cmd/merge.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1335 2024-02-16 19:39:20.000000 ds-format-4.1.0/ds_format/cmd/meta.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2971 2024-02-16 19:39:20.000000 ds-format-4.1.0/ds_format/cmd/rename.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1266 2024-02-16 19:39:20.000000 ds-format-4.1.0/ds_format/cmd/rename_dim.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2244 2024-02-16 19:39:20.000000 ds-format-4.1.0/ds_format/cmd/rm.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2594 2024-02-16 19:39:20.000000 ds-format-4.1.0/ds_format/cmd/select.py
--rw-r--r--   0 peter     (1000) peter     (1000)     5279 2024-02-16 19:39:20.000000 ds-format-4.1.0/ds_format/cmd/set_.py
--rw-r--r--   0 peter     (1000) peter     (1000)      850 2024-02-16 19:39:20.000000 ds-format-4.1.0/ds_format/cmd/size.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1984 2024-02-16 19:39:20.000000 ds-format-4.1.0/ds_format/cmd/stats.py
--rw-r--r--   0 peter     (1000) peter     (1000)      859 2024-02-16 19:39:20.000000 ds-format-4.1.0/ds_format/cmd/type_.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-02-16 20:14:34.158317 ds-format-4.1.0/ds_format/drivers/
--rw-r--r--   0 peter     (1000) peter     (1000)      179 2024-02-16 19:39:20.000000 ds-format-4.1.0/ds_format/drivers/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2049 2024-02-16 19:39:20.000000 ds-format-4.1.0/ds_format/drivers/csv.py
--rw-r--r--   0 peter     (1000) peter     (1000)     5574 2024-02-16 19:39:20.000000 ds-format-4.1.0/ds_format/drivers/ds.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2780 2024-02-16 19:39:20.000000 ds-format-4.1.0/ds_format/drivers/hdf.py
--rw-r--r--   0 peter     (1000) peter     (1000)      602 2024-02-16 19:39:20.000000 ds-format-4.1.0/ds_format/drivers/json.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2472 2024-02-16 19:39:20.000000 ds-format-4.1.0/ds_format/drivers/netcdf.py
--rw-r--r--   0 peter     (1000) peter     (1000)     4874 2024-02-16 19:39:20.000000 ds-format-4.1.0/ds_format/help.py
--rw-r--r--   0 peter     (1000) peter     (1000)     8593 2024-02-16 19:39:20.000000 ds-format-4.1.0/ds_format/io.py
--rw-r--r--   0 peter     (1000) peter     (1000)     5333 2024-02-16 19:39:20.000000 ds-format-4.1.0/ds_format/misc.py
--rw-r--r--   0 peter     (1000) peter     (1000)    39401 2024-02-16 19:39:20.000000 ds-format-4.1.0/ds_format/op.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1122 2024-02-16 19:39:20.000000 ds-format-4.1.0/ds_format/validate.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-02-16 20:14:34.154317 ds-format-4.1.0/ds_format.egg-info/
--rw-r--r--   0 peter     (1000) peter     (1000)      703 2024-02-16 20:14:34.000000 ds-format-4.1.0/ds_format.egg-info/PKG-INFO
--rw-r--r--   0 peter     (1000) peter     (1000)     1225 2024-02-16 20:14:34.000000 ds-format-4.1.0/ds_format.egg-info/SOURCES.txt
--rw-r--r--   0 peter     (1000) peter     (1000)        1 2024-02-16 20:14:34.000000 ds-format-4.1.0/ds_format.egg-info/dependency_links.txt
--rw-r--r--   0 peter     (1000) peter     (1000)       45 2024-02-16 20:14:34.000000 ds-format-4.1.0/ds_format.egg-info/entry_points.txt
--rw-r--r--   0 peter     (1000) peter     (1000)      158 2024-02-16 20:14:34.000000 ds-format-4.1.0/ds_format.egg-info/requires.txt
--rw-r--r--   0 peter     (1000) peter     (1000)       10 2024-02-16 20:14:34.000000 ds-format-4.1.0/ds_format.egg-info/top_level.txt
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-02-16 20:14:34.158317 ds-format-4.1.0/man/
--rw-r--r--   0 peter     (1000) peter     (1000)     1189 2024-02-16 19:39:20.000000 ds-format-4.1.0/man/ds-attrs.1
--rw-r--r--   0 peter     (1000) peter     (1000)     1446 2024-02-16 19:39:20.000000 ds-format-4.1.0/man/ds-cat.1
--rw-r--r--   0 peter     (1000) peter     (1000)      812 2024-02-16 19:39:20.000000 ds-format-4.1.0/man/ds-dims.1
--rw-r--r--   0 peter     (1000) peter     (1000)      299 2024-02-16 19:39:20.000000 ds-format-4.1.0/man/ds-get.1
--rw-r--r--   0 peter     (1000) peter     (1000)     1602 2024-02-16 19:39:20.000000 ds-format-4.1.0/man/ds-ls.1
--rw-r--r--   0 peter     (1000) peter     (1000)     2716 2024-02-16 19:39:20.000000 ds-format-4.1.0/man/ds-merge.1
--rw-r--r--   0 peter     (1000) peter     (1000)      880 2024-02-16 19:39:20.000000 ds-format-4.1.0/man/ds-meta.1
--rw-r--r--   0 peter     (1000) peter     (1000)     1860 2024-02-16 19:39:20.000000 ds-format-4.1.0/man/ds-rename.1
--rw-r--r--   0 peter     (1000) peter     (1000)     1023 2024-02-16 19:39:20.000000 ds-format-4.1.0/man/ds-rename_attr.1
--rw-r--r--   0 peter     (1000) peter     (1000)      915 2024-02-16 19:39:20.000000 ds-format-4.1.0/man/ds-rename_dim.1
--rw-r--r--   0 peter     (1000) peter     (1000)     1391 2024-02-16 19:39:20.000000 ds-format-4.1.0/man/ds-rm.1
--rw-r--r--   0 peter     (1000) peter     (1000)      896 2024-02-16 19:39:20.000000 ds-format-4.1.0/man/ds-rm_attr.1
--rw-r--r--   0 peter     (1000) peter     (1000)     2146 2024-02-16 19:39:20.000000 ds-format-4.1.0/man/ds-select.1
--rw-r--r--   0 peter     (1000) peter     (1000)     3780 2024-02-16 19:39:20.000000 ds-format-4.1.0/man/ds-set.1
--rw-r--r--   0 peter     (1000) peter     (1000)      688 2024-02-16 19:39:20.000000 ds-format-4.1.0/man/ds-set_attrs.1
--rw-r--r--   0 peter     (1000) peter     (1000)      750 2024-02-16 19:39:20.000000 ds-format-4.1.0/man/ds-set_dims.1
--rw-r--r--   0 peter     (1000) peter     (1000)      545 2024-02-16 19:39:20.000000 ds-format-4.1.0/man/ds-size.1
--rw-r--r--   0 peter     (1000) peter     (1000)     1281 2024-02-16 19:39:20.000000 ds-format-4.1.0/man/ds-stats.1
--rw-r--r--   0 peter     (1000) peter     (1000)      551 2024-02-16 19:39:20.000000 ds-format-4.1.0/man/ds-type.1
--rw-r--r--   0 peter     (1000) peter     (1000)     1195 2024-02-16 19:39:20.000000 ds-format-4.1.0/man/ds-write.1
--rw-r--r--   0 peter     (1000) peter     (1000)     3416 2024-02-16 19:39:20.000000 ds-format-4.1.0/man/ds.1
--rw-r--r--   0 peter     (1000) peter     (1000)       38 2024-02-16 20:14:34.158317 ds-format-4.1.0/setup.cfg
--rwxr-xr-x   0 peter     (1000) peter     (1000)     1173 2024-02-16 19:39:20.000000 ds-format-4.1.0/setup.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-06-03 15:32:31.094056 ds-format-4.1.1/
+-rw-r--r--   0 peter     (1000) peter     (1000)     1072 2024-06-03 15:31:16.000000 ds-format-4.1.1/LICENSE.md
+-rw-r--r--   0 peter     (1000) peter     (1000)      703 2024-06-03 15:32:31.090056 ds-format-4.1.1/PKG-INFO
+-rw-r--r--   0 peter     (1000) peter     (1000)      563 2024-06-03 15:31:16.000000 ds-format-4.1.1/README.md
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-06-03 15:32:31.086056 ds-format-4.1.1/ds_format/
+-rw-r--r--   0 peter     (1000) peter     (1000)      681 2024-06-03 15:31:16.000000 ds-format-4.1.1/ds_format/__init__.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-06-03 15:32:31.086056 ds-format-4.1.1/ds_format/bin/
+-rw-r--r--   0 peter     (1000) peter     (1000)        0 2024-06-03 15:31:16.000000 ds-format-4.1.1/ds_format/bin/__init__.py
+-rwxr-xr-x   0 peter     (1000) peter     (1000)      310 2024-06-03 15:31:16.000000 ds-format-4.1.1/ds_format/bin/ds.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-06-03 15:32:31.090056 ds-format-4.1.1/ds_format/cmd/
+-rw-r--r--   0 peter     (1000) peter     (1000)      578 2024-06-03 15:31:16.000000 ds-format-4.1.1/ds_format/cmd/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1645 2024-06-03 15:31:16.000000 ds-format-4.1.1/ds_format/cmd/attrs.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2624 2024-06-03 15:31:16.000000 ds-format-4.1.1/ds_format/cmd/cat.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1212 2024-06-03 15:31:16.000000 ds-format-4.1.1/ds_format/cmd/dims.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2565 2024-06-03 15:31:16.000000 ds-format-4.1.1/ds_format/cmd/ls.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     5083 2024-06-03 15:31:16.000000 ds-format-4.1.1/ds_format/cmd/main.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2965 2024-06-03 15:31:16.000000 ds-format-4.1.1/ds_format/cmd/merge.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1335 2024-06-03 15:31:16.000000 ds-format-4.1.1/ds_format/cmd/meta.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2971 2024-06-03 15:31:16.000000 ds-format-4.1.1/ds_format/cmd/rename.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1266 2024-06-03 15:31:16.000000 ds-format-4.1.1/ds_format/cmd/rename_dim.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2244 2024-06-03 15:31:16.000000 ds-format-4.1.1/ds_format/cmd/rm.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2594 2024-06-03 15:31:16.000000 ds-format-4.1.1/ds_format/cmd/select.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     5279 2024-06-03 15:31:16.000000 ds-format-4.1.1/ds_format/cmd/set_.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      850 2024-06-03 15:31:16.000000 ds-format-4.1.1/ds_format/cmd/size.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1984 2024-06-03 15:31:16.000000 ds-format-4.1.1/ds_format/cmd/stats.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      859 2024-06-03 15:31:16.000000 ds-format-4.1.1/ds_format/cmd/type_.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-06-03 15:32:31.090056 ds-format-4.1.1/ds_format/drivers/
+-rw-r--r--   0 peter     (1000) peter     (1000)      179 2024-06-03 15:31:16.000000 ds-format-4.1.1/ds_format/drivers/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2049 2024-06-03 15:31:16.000000 ds-format-4.1.1/ds_format/drivers/csv.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     5574 2024-06-03 15:31:16.000000 ds-format-4.1.1/ds_format/drivers/ds.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2780 2024-06-03 15:31:16.000000 ds-format-4.1.1/ds_format/drivers/hdf.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      602 2024-06-03 15:31:16.000000 ds-format-4.1.1/ds_format/drivers/json.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2472 2024-06-03 15:31:16.000000 ds-format-4.1.1/ds_format/drivers/netcdf.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     4874 2024-06-03 15:31:16.000000 ds-format-4.1.1/ds_format/help.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     8593 2024-06-03 15:31:16.000000 ds-format-4.1.1/ds_format/io.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     5333 2024-06-03 15:31:16.000000 ds-format-4.1.1/ds_format/misc.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    39430 2024-06-03 15:31:16.000000 ds-format-4.1.1/ds_format/op.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1122 2024-06-03 15:31:16.000000 ds-format-4.1.1/ds_format/validate.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-06-03 15:32:31.086056 ds-format-4.1.1/ds_format.egg-info/
+-rw-r--r--   0 peter     (1000) peter     (1000)      703 2024-06-03 15:32:31.000000 ds-format-4.1.1/ds_format.egg-info/PKG-INFO
+-rw-r--r--   0 peter     (1000) peter     (1000)     1225 2024-06-03 15:32:31.000000 ds-format-4.1.1/ds_format.egg-info/SOURCES.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)        1 2024-06-03 15:32:31.000000 ds-format-4.1.1/ds_format.egg-info/dependency_links.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)       45 2024-06-03 15:32:31.000000 ds-format-4.1.1/ds_format.egg-info/entry_points.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)      158 2024-06-03 15:32:31.000000 ds-format-4.1.1/ds_format.egg-info/requires.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)       10 2024-06-03 15:32:31.000000 ds-format-4.1.1/ds_format.egg-info/top_level.txt
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-06-03 15:32:31.090056 ds-format-4.1.1/man/
+-rw-r--r--   0 peter     (1000) peter     (1000)     1185 2024-06-03 15:31:16.000000 ds-format-4.1.1/man/ds-attrs.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     1442 2024-06-03 15:31:16.000000 ds-format-4.1.1/man/ds-cat.1
+-rw-r--r--   0 peter     (1000) peter     (1000)      808 2024-06-03 15:31:16.000000 ds-format-4.1.1/man/ds-dims.1
+-rw-r--r--   0 peter     (1000) peter     (1000)      299 2024-06-03 15:31:16.000000 ds-format-4.1.1/man/ds-get.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     1598 2024-06-03 15:31:16.000000 ds-format-4.1.1/man/ds-ls.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     2712 2024-06-03 15:31:16.000000 ds-format-4.1.1/man/ds-merge.1
+-rw-r--r--   0 peter     (1000) peter     (1000)      876 2024-06-03 15:31:16.000000 ds-format-4.1.1/man/ds-meta.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     1856 2024-06-03 15:31:16.000000 ds-format-4.1.1/man/ds-rename.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     1023 2024-06-03 15:31:16.000000 ds-format-4.1.1/man/ds-rename_attr.1
+-rw-r--r--   0 peter     (1000) peter     (1000)      911 2024-06-03 15:31:16.000000 ds-format-4.1.1/man/ds-rename_dim.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     1387 2024-06-03 15:31:16.000000 ds-format-4.1.1/man/ds-rm.1
+-rw-r--r--   0 peter     (1000) peter     (1000)      896 2024-06-03 15:31:16.000000 ds-format-4.1.1/man/ds-rm_attr.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     2142 2024-06-03 15:31:16.000000 ds-format-4.1.1/man/ds-select.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     3776 2024-06-03 15:31:16.000000 ds-format-4.1.1/man/ds-set.1
+-rw-r--r--   0 peter     (1000) peter     (1000)      688 2024-06-03 15:31:16.000000 ds-format-4.1.1/man/ds-set_attrs.1
+-rw-r--r--   0 peter     (1000) peter     (1000)      750 2024-06-03 15:31:16.000000 ds-format-4.1.1/man/ds-set_dims.1
+-rw-r--r--   0 peter     (1000) peter     (1000)      541 2024-06-03 15:31:16.000000 ds-format-4.1.1/man/ds-size.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     1277 2024-06-03 15:31:16.000000 ds-format-4.1.1/man/ds-stats.1
+-rw-r--r--   0 peter     (1000) peter     (1000)      547 2024-06-03 15:31:16.000000 ds-format-4.1.1/man/ds-type.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     1195 2024-06-03 15:31:16.000000 ds-format-4.1.1/man/ds-write.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     3412 2024-06-03 15:31:16.000000 ds-format-4.1.1/man/ds.1
+-rw-r--r--   0 peter     (1000) peter     (1000)       38 2024-06-03 15:32:31.094056 ds-format-4.1.1/setup.cfg
+-rwxr-xr-x   0 peter     (1000) peter     (1000)     1173 2024-06-03 15:31:16.000000 ds-format-4.1.1/setup.py
```

### Comparing `ds-format-4.1.0/LICENSE.md` & `ds-format-4.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ds-format-4.1.0/PKG-INFO` & `ds-format-4.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ds-format
-Version: 4.1.0
+Version: 4.1.1
 Summary: ds-format is an open source program, a Python package and a storage format which provides an interface for reading and writing NetCDF files, as well as its own data file format.
 Home-page: https://ds-format.peterkuma.net
 Author: Peter Kuma
 Author-email: peter@peterkuma.net
 License: MIT
 Keywords: dataset,netcdf,hdf,json,numpy
 Platform: any
```

### Comparing `ds-format-4.1.0/README.md` & `ds-format-4.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ds-format-4.1.0/ds_format/__init__.py` & `ds-format-4.1.1/ds_format/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '4.1.0'
+__version__ = '4.1.1'
 
 import os
 mode = os.environ.get('DS_MODE', 'soft')
 output = 'pst'
 
 from .misc import \
 	escape, \
```

### Comparing `ds-format-4.1.0/ds_format/cmd/__init__.py` & `ds-format-4.1.1/ds_format/cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `ds-format-4.1.0/ds_format/cmd/attrs.py` & `ds-format-4.1.1/ds_format/cmd/attrs.py`

 * *Files identical despite different names*

### Comparing `ds-format-4.1.0/ds_format/cmd/cat.py` & `ds-format-4.1.1/ds_format/cmd/cat.py`

 * *Files identical despite different names*

### Comparing `ds-format-4.1.0/ds_format/cmd/dims.py` & `ds-format-4.1.1/ds_format/cmd/dims.py`

 * *Files identical despite different names*

### Comparing `ds-format-4.1.0/ds_format/cmd/ls.py` & `ds-format-4.1.1/ds_format/cmd/ls.py`

 * *Files identical despite different names*

### Comparing `ds-format-4.1.0/ds_format/cmd/main.py` & `ds-format-4.1.1/ds_format/cmd/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 		JSON: `.json`
 		NetCDF4: "`.nc`, `.nc4`, `.netcdf`"
 	}}
 	environment: {{
 		DS_MODE: "Error handling mode. If \\"strict\\", handle missing variables, dimensions and attributes as errors. If \\"moderate\\", report a warning. If \\"soft\\", ignore missing items."
 	}}
 	author: "Written by Peter Kuma."
-	copyright: "Copyright (c) 2019-2023 Peter Kuma. This software is distributed under an MIT license."
+	copyright: "Copyright (c) 2019-2024 Peter Kuma. This software is distributed under an MIT license."
 	'''
 	a = pst.decode([os.fsencode(y) for y in sys.argv[1:]], as_unicode=True)
 	args = []
 	opts = {}
 	if type(a) is list:
 		if len(a) > 0 and type(a[-1]) is dict:
 			opts = a[-1]
```

### Comparing `ds-format-4.1.0/ds_format/cmd/merge.py` & `ds-format-4.1.1/ds_format/cmd/merge.py`

 * *Files identical despite different names*

### Comparing `ds-format-4.1.0/ds_format/cmd/meta.py` & `ds-format-4.1.1/ds_format/cmd/meta.py`

 * *Files identical despite different names*

### Comparing `ds-format-4.1.0/ds_format/cmd/rename.py` & `ds-format-4.1.1/ds_format/cmd/rename.py`

 * *Files identical despite different names*

### Comparing `ds-format-4.1.0/ds_format/cmd/rename_dim.py` & `ds-format-4.1.1/ds_format/cmd/rename_dim.py`

 * *Files identical despite different names*

### Comparing `ds-format-4.1.0/ds_format/cmd/rm.py` & `ds-format-4.1.1/ds_format/cmd/rm.py`

 * *Files identical despite different names*

### Comparing `ds-format-4.1.0/ds_format/cmd/select.py` & `ds-format-4.1.1/ds_format/cmd/select.py`

 * *Files identical despite different names*

### Comparing `ds-format-4.1.0/ds_format/cmd/set_.py` & `ds-format-4.1.1/ds_format/cmd/set_.py`

 * *Files identical despite different names*

### Comparing `ds-format-4.1.0/ds_format/cmd/size.py` & `ds-format-4.1.1/ds_format/cmd/size.py`

 * *Files identical despite different names*

### Comparing `ds-format-4.1.0/ds_format/cmd/stats.py` & `ds-format-4.1.1/ds_format/cmd/stats.py`

 * *Files identical despite different names*

### Comparing `ds-format-4.1.0/ds_format/cmd/type_.py` & `ds-format-4.1.1/ds_format/cmd/type_.py`

 * *Files identical despite different names*

### Comparing `ds-format-4.1.0/ds_format/drivers/csv.py` & `ds-format-4.1.1/ds_format/drivers/csv.py`

 * *Files identical despite different names*

### Comparing `ds-format-4.1.0/ds_format/drivers/ds.py` & `ds-format-4.1.1/ds_format/drivers/ds.py`

 * *Files identical despite different names*

### Comparing `ds-format-4.1.0/ds_format/drivers/hdf.py` & `ds-format-4.1.1/ds_format/drivers/hdf.py`

 * *Files identical despite different names*

### Comparing `ds-format-4.1.0/ds_format/drivers/json.py` & `ds-format-4.1.1/ds_format/drivers/json.py`

 * *Files identical despite different names*

### Comparing `ds-format-4.1.0/ds_format/drivers/netcdf.py` & `ds-format-4.1.1/ds_format/drivers/netcdf.py`

 * *Files identical despite different names*

### Comparing `ds-format-4.1.0/ds_format/help.py` & `ds-format-4.1.1/ds_format/help.py`

 * *Files identical despite different names*

### Comparing `ds-format-4.1.0/ds_format/io.py` & `ds-format-4.1.1/ds_format/io.py`

 * *Files identical despite different names*

### Comparing `ds-format-4.1.0/ds_format/misc.py` & `ds-format-4.1.1/ds_format/misc.py`

 * *Files identical despite different names*

### Comparing `ds-format-4.1.0/ds_format/op.py` & `ds-format-4.1.1/ds_format/op.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import types
 import fnmatch
 import numpy as np
 import copy as copy_
 import datetime as dt
-from warnings import warn, catch_warnings
+import warnings
+from warnings import warn
 from collections.abc import Mapping, Iterable
 import ds_format as ds
 from ds_format.misc import check
 from . import misc
 
 #
 # Private variables.
@@ -172,15 +173,16 @@
 		ds.var(d2, var, data)
 	meta = ds.meta(d)
 	ds.meta(d2, None, copy_.deepcopy(meta))
 	return d2
 
 def normalize_var(data):
 	if isinstance(data, (list, tuple)):
-		with catch_warnings(action='ignore'):
+		with warnings.catch_warnings():
+			warnings.simplefilter('ignore')
 			data = np.ma.asarray(data)
 		data = np.ma.masked_equal(data, None)
 		mask = data.mask.copy()
 		if np.ma.is_masked(data):
 			data[mask] = 0
 			tmp = data.flatten().tolist()
 			data = np.ma.array(tmp, mask=mask)
```

### Comparing `ds-format-4.1.0/ds_format/validate.py` & `ds-format-4.1.1/ds_format/validate.py`

 * *Files identical despite different names*

### Comparing `ds-format-4.1.0/ds_format.egg-info/PKG-INFO` & `ds-format-4.1.1/ds_format.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ds-format
-Version: 4.1.0
+Version: 4.1.1
 Summary: ds-format is an open source program, a Python package and a storage format which provides an interface for reading and writing NetCDF files, as well as its own data file format.
 Home-page: https://ds-format.peterkuma.net
 Author: Peter Kuma
 Author-email: peter@peterkuma.net
 License: MIT
 Keywords: dataset,netcdf,hdf,json,numpy
 Platform: any
```

### Comparing `ds-format-4.1.0/ds_format.egg-info/SOURCES.txt` & `ds-format-4.1.1/ds_format.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ds-format-4.1.0/man/ds-attrs.1` & `ds-format-4.1.1/man/ds-attrs.1`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" generated with Ronn-NG/v0.9.1
 .\" http://github.com/apjanke/ronn-ng/tree/0.9.1
-.TH "DS\-ATTRS" "1" "February 2024" ""
+.TH "DS\-ATTRS" "1" "June 2024" ""
 .SH "NAME"
 \fBds\-attrs\fR \- Print attributes in a dataset\.
 .SH "SYNOPSIS"
 \fBds attrs\fR [\fIvar\fR] [\fIattr\fR] \fIinput\fR [\fIoptions\fR]
 .SH "DESCRIPTION"
 The output is formatted as PST \fIhttps://github\.com/peterkuma/pst\fR\.
 .SH "ARGUMENTS"
```

### Comparing `ds-format-4.1.0/man/ds-cat.1` & `ds-format-4.1.1/man/ds-cat.1`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" generated with Ronn-NG/v0.9.1
 .\" http://github.com/apjanke/ronn-ng/tree/0.9.1
-.TH "DS\-CAT" "1" "February 2024" ""
+.TH "DS\-CAT" "1" "June 2024" ""
 .SH "NAME"
 \fBds\-cat\fR \- Print variable data\.
 .SH "SYNOPSIS"
 \fBds cat\fR \fIvar\fR \fIinput\fR [\fIoptions\fR]
 .br
 \fBds cat\fR \fIvar\fR\|\.\|\.\|\. \fIinput\fR [\fIoptions\fR]
 .br
```

### Comparing `ds-format-4.1.0/man/ds-dims.1` & `ds-format-4.1.1/man/ds-dims.1`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" generated with Ronn-NG/v0.9.1
 .\" http://github.com/apjanke/ronn-ng/tree/0.9.1
-.TH "DS\-DIMS" "1" "February 2024" ""
+.TH "DS\-DIMS" "1" "June 2024" ""
 .SH "NAME"
 \fBds\-dims\fR \- Print dimensions of a dataset or a variable\.
 .SH "SYNOPSIS"
 \fBds dims\fR [\fIvar\fR] \fIinput\fR [\fIoptions\fR]
 .SH "ARGUMENTS"
 .TP
 \fIvar\fR
```

### Comparing `ds-format-4.1.0/man/ds-ls.1` & `ds-format-4.1.1/man/ds-ls.1`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" generated with Ronn-NG/v0.9.1
 .\" http://github.com/apjanke/ronn-ng/tree/0.9.1
-.TH "DS\-LS" "1" "February 2024" ""
+.TH "DS\-LS" "1" "June 2024" ""
 .SH "NAME"
 \fBds\-ls\fR \- List variables\.
 .SH "SYNOPSIS"
 \fBds\fR [\fIvar\fR]\|\.\|\.\|\. \fIinput\fR [\fIoptions\fR]
 .br
 \fBds ls\fR [\fIvar\fR]\|\.\|\.\|\. \fIinput\fR [\fIoptions\fR]
 .br
```

### Comparing `ds-format-4.1.0/man/ds-merge.1` & `ds-format-4.1.1/man/ds-merge.1`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" generated with Ronn-NG/v0.9.1
 .\" http://github.com/apjanke/ronn-ng/tree/0.9.1
-.TH "DS\-MERGE" "1" "February 2024" ""
+.TH "DS\-MERGE" "1" "June 2024" ""
 .SH "NAME"
 \fBds\-merge\fR \- Merge datasets along a dimension\.
 .SH "SYNOPSIS"
 \fBds merge\fR \fIdim\fR \fIinput\fR\|\.\|\.\|\. \fIoutput\fR [\fIoptions\fR]
 .SH "DESCRIPTION"
 Merge datasets along a dimension \fIdim\fR\. If the dimension is not defined in the dataset, merge along a new dimension \fIdim\fR\. If \fInew\fR is \fBnone\fR and \fIdim\fR is not new, variables without the dimension \fIdim\fR are set with the first occurrence of the variable\. If \fInew\fR is not \fBnone\fR and \fIdim\fR is not new, variables without the dimension \fIdim\fR are merged along a new dimension \fInew\fR\. If \fIvariables\fR is not \fBnone\fR, only those variables are merged along a new dimension, and other variables are set to the first occurrence of the variable\. Variables which are merged along a new dimension and are not present in all datasets have their subsets corresponding to the datasets where they are missing filled with missing values\. Dataset and variable metadata are merged sequentially from all datasets, with metadata from later datasets overriding metadata from the former ones\.
 .SH "ARGUMENTS"
```

### Comparing `ds-format-4.1.0/man/ds-meta.1` & `ds-format-4.1.1/man/ds-meta.1`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" generated with Ronn-NG/v0.9.1
 .\" http://github.com/apjanke/ronn-ng/tree/0.9.1
-.TH "DS\-META" "1" "February 2024" ""
+.TH "DS\-META" "1" "June 2024" ""
 .SH "NAME"
 \fBds\-meta\fR \- Print dataset metadata\.
 .SH "SYNOPSIS"
 \fBds meta\fR [\fIvar\fR] \fIinput\fR [\fIoptions\fR]
 .SH "DESCRIPTION"
 The output is formatted as PST \fIhttps://github\.com/peterkuma/pst\fR\.
 .SH "ARGUMENTS"
```

### Comparing `ds-format-4.1.0/man/ds-rename.1` & `ds-format-4.1.1/man/ds-rename.1`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" generated with Ronn-NG/v0.9.1
 .\" http://github.com/apjanke/ronn-ng/tree/0.9.1
-.TH "DS\-RENAME" "1" "February 2024" ""
+.TH "DS\-RENAME" "1" "June 2024" ""
 .SH "NAME"
 \fBds\-rename\fR \- Rename variables and attributes\.
 .SH "SYNOPSIS"
 \fBds rename\fR \fIvars\fR \fIinput\fR \fIoutput\fR [\fIoptions\fR]
 .br
 \fBds rename\fR \fIvar\fR \fIattrs\fR \fIinput\fR \fIoutput\fR [\fIoptions\fR]
 .br
```

### Comparing `ds-format-4.1.0/man/ds-rename_attr.1` & `ds-format-4.1.1/man/ds-rename_attr.1`

 * *Files identical despite different names*

### Comparing `ds-format-4.1.0/man/ds-rename_dim.1` & `ds-format-4.1.1/man/ds-rename_dim.1`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" generated with Ronn-NG/v0.9.1
 .\" http://github.com/apjanke/ronn-ng/tree/0.9.1
-.TH "DS\-RENAME_DIM" "1" "February 2024" ""
+.TH "DS\-RENAME_DIM" "1" "June 2024" ""
 .SH "NAME"
 \fBds\-rename_dim\fR \- Rename a dimension\.
 .SH "SYNOPSIS"
 \fBds rename_dim\fR \fIdims\fR \fIinput\fR \fIoutput\fR [\fIoptions\fR]
 .br
 .SH "ARGUMENTS"
 .TP
```

### Comparing `ds-format-4.1.0/man/ds-rm.1` & `ds-format-4.1.1/man/ds-rm.1`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" generated with Ronn-NG/v0.9.1
 .\" http://github.com/apjanke/ronn-ng/tree/0.9.1
-.TH "DS\-RM" "1" "February 2024" ""
+.TH "DS\-RM" "1" "June 2024" ""
 .SH "NAME"
 \fBds\-rm\fR \- Remove variables or attributes\.
 .SH "SYNOPSIS"
 \fBds rm\fR \fIvar\fR \fIinput\fR \fIoutput\fR [\fIoptions\fR]
 .br
 \fBds rm\fR \fIvar\fR \fIattr\fR \fIinput\fR \fIoutput\fR [\fIoptions\fR]
 .br
```

### Comparing `ds-format-4.1.0/man/ds-rm_attr.1` & `ds-format-4.1.1/man/ds-rm_attr.1`

 * *Files identical despite different names*

### Comparing `ds-format-4.1.0/man/ds-select.1` & `ds-format-4.1.1/man/ds-select.1`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" generated with Ronn-NG/v0.9.1
 .\" http://github.com/apjanke/ronn-ng/tree/0.9.1
-.TH "DS\-SELECT" "1" "February 2024" ""
+.TH "DS\-SELECT" "1" "June 2024" ""
 .SH "NAME"
 \fBds\-select\fR \- Select and subset variables\.
 .SH "SYNOPSIS"
 \fBds select\fR [\fIvar\fR\|\.\|\.\|\.] [\fIsel\fR] \fIinput\fR \fIoutput\fR [\fIoptions\fR]
 .SH "DESCRIPTION"
 select can also be used to convert between different file formats (\fBds select\fR \fIinput\fR \fIoutput\fR)\.
 .SH "ARGUMENTS"
```

### Comparing `ds-format-4.1.0/man/ds-set.1` & `ds-format-4.1.1/man/ds-set.1`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" generated with Ronn-NG/v0.9.1
 .\" http://github.com/apjanke/ronn-ng/tree/0.9.1
-.TH "DS\-SET" "1" "February 2024" ""
+.TH "DS\-SET" "1" "June 2024" ""
 .SH "NAME"
 \fBds\-set\fR \- Set variable data, dimensions and attributes in an existing or new dataset\.
 .SH "SYNOPSIS"
 \fBds set\fR \fIds_attrs\fR \fIinput\fR \fIoutput\fR [\fIoptions\fR]
 .br
 \fBds set\fR \fIvar\fR [\fItype\fR [\fIdims\fR [\fIdata\fR]]] [\fIattrs\fR]\|\.\|\.\|\. \fIinput\fR \fIoutput\fR [\fIoptions\fR]
 .br
```

### Comparing `ds-format-4.1.0/man/ds-set_attrs.1` & `ds-format-4.1.1/man/ds-set_attrs.1`

 * *Files identical despite different names*

### Comparing `ds-format-4.1.0/man/ds-set_dims.1` & `ds-format-4.1.1/man/ds-set_dims.1`

 * *Files identical despite different names*

### Comparing `ds-format-4.1.0/man/ds-size.1` & `ds-format-4.1.1/man/ds-size.1`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" generated with Ronn-NG/v0.9.1
 .\" http://github.com/apjanke/ronn-ng/tree/0.9.1
-.TH "DS\-SIZE" "1" "February 2024" ""
+.TH "DS\-SIZE" "1" "June 2024" ""
 .SH "NAME"
 \fBds\-size\fR \- Print a variable size\.
 .SH "SYNOPSIS"
 \fBds size\fR \fIvar\fR \fIinput\fR [\fIoptions\fR]
 .SH "ARGUMENTS"
 .TP
 \fIvar\fR
```

### Comparing `ds-format-4.1.0/man/ds-stats.1` & `ds-format-4.1.1/man/ds-stats.1`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" generated with Ronn-NG/v0.9.1
 .\" http://github.com/apjanke/ronn-ng/tree/0.9.1
-.TH "DS\-STATS" "1" "February 2024" ""
+.TH "DS\-STATS" "1" "June 2024" ""
 .SH "NAME"
 \fBds\-stats\fR \- Print variable statistics\.
 .SH "SYNOPSIS"
 \fBds stats\fR \fIvar\fR \fIinput\fR [\fIoptions\fR]
 .SH "DESCRIPTION"
 NaNs are ignored in all statistics except for \fBcount\fR\. The output is formatted as PST \fIhttps://github\.com/peterkuma/pst\fR\.
 .SH "ARGUMENTS"
```

### Comparing `ds-format-4.1.0/man/ds-type.1` & `ds-format-4.1.1/man/ds-type.1`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" generated with Ronn-NG/v0.9.1
 .\" http://github.com/apjanke/ronn-ng/tree/0.9.1
-.TH "DS\-TYPE" "1" "February 2024" ""
+.TH "DS\-TYPE" "1" "June 2024" ""
 .SH "NAME"
 \fBds\-type\fR \- Print a variable type\.
 .SH "SYNOPSIS"
 \fBds type\fR \fIvar\fR \fIinput\fR [\fIoptions\fR]
 .SH "ARGUMENTS"
 .TP
 \fIvar\fR
```

### Comparing `ds-format-4.1.0/man/ds-write.1` & `ds-format-4.1.1/man/ds-write.1`

 * *Files identical despite different names*

### Comparing `ds-format-4.1.0/man/ds.1` & `ds-format-4.1.1/man/ds.1`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" generated with Ronn-NG/v0.9.1
 .\" http://github.com/apjanke/ronn-ng/tree/0.9.1
-.TH "DS" "1" "February 2024" ""
+.TH "DS" "1" "June 2024" ""
 .SH "NAME"
 \fBds\fR \- Tool for reading, writing and modifying dataset files\.
 .SH "SYNOPSIS"
 \fBds\fR [\fIcmd\fR [\fIargs\fR]] [\fIoptions\fR]
 .br
 \fBds \-\-help\fR [\fIcmd\fR]
 .br
@@ -122,8 +122,8 @@
 .SH "ENVIRONMENT"
 .TP
 DS_MODE
 Error handling mode\. If "strict", handle missing variables, dimensions and attributes as errors\. If "moderate", report a warning\. If "soft", ignore missing items\.
 .SH "AUTHOR"
 Written by Peter Kuma\.
 .SH "COPYRIGHT"
-Copyright (c) 2019\-2023 Peter Kuma\. This software is distributed under an MIT license\.
+Copyright (c) 2019\-2024 Peter Kuma\. This software is distributed under an MIT license\.
```

### Comparing `ds-format-4.1.0/setup.py` & `ds-format-4.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 from glob import glob
 
 setup(
 	name='ds-format',
-	version='4.1.0',
+	version='4.1.1',
 	entry_points={
 		'console_scripts': ['ds = ds_format.bin.ds:main'],
 	},
 	packages=find_packages(),
 	description='ds-format is an open source program, a Python package and a storage format which provides an interface for reading and writing NetCDF files, as well as its own data file format.',
 	author='Peter Kuma',
 	author_email='peter@peterkuma.net',
```

