# Comparing `tmp/astro-gdt-fermi-2.0.0.tar.gz` & `tmp/astro_gdt_fermi-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astro-gdt-fermi-2.0.0.tar", last modified: Wed Apr 12 20:35:33 2023, max compression
+gzip compressed data, was "astro_gdt_fermi-2.1.0.tar", last modified: Mon Jun  3 14:19:14 2024, max compression
```

## Comparing `astro-gdt-fermi-2.0.0.tar` & `astro_gdt_fermi-2.1.0.tar`

### file list

```diff
@@ -1,45 +1,64 @@
-drwxr-xr-x   0 wcleveland   (502) staff       (20)        0 2023-04-12 20:35:33.230233 astro-gdt-fermi-2.0.0/
--rw-r--r--   0 wcleveland   (502) staff       (20)       43 2023-04-12 13:20:21.000000 astro-gdt-fermi-2.0.0/MANIFEST.in
--rw-r--r--   0 wcleveland   (502) staff       (20)     1702 2023-04-12 20:35:33.229953 astro-gdt-fermi-2.0.0/PKG-INFO
--rw-r--r--   0 wcleveland   (502) staff       (20)      847 2023-04-12 15:02:14.000000 astro-gdt-fermi-2.0.0/PYPI-README.rst
--rw-r--r--   0 wcleveland   (502) staff       (20)     3367 2023-04-12 15:10:21.000000 astro-gdt-fermi-2.0.0/README.rst
--rw-r--r--   0 wcleveland   (502) staff       (20)    11357 2023-03-28 16:42:58.000000 astro-gdt-fermi-2.0.0/license.txt
--rw-r--r--   0 wcleveland   (502) staff       (20)       38 2023-04-12 20:35:33.230310 astro-gdt-fermi-2.0.0/setup.cfg
--rw-r--r--   0 wcleveland   (502) staff       (20)     3192 2023-04-12 19:31:21.000000 astro-gdt-fermi-2.0.0/setup.py
-drwxr-xr-x   0 wcleveland   (502) staff       (20)        0 2023-04-12 20:35:33.201583 astro-gdt-fermi-2.0.0/src/
-drwxr-xr-x   0 wcleveland   (502) staff       (20)        0 2023-04-12 20:35:33.209504 astro-gdt-fermi-2.0.0/src/astro_gdt_fermi.egg-info/
--rw-r--r--   0 wcleveland   (502) staff       (20)     1702 2023-04-12 20:35:33.000000 astro-gdt-fermi-2.0.0/src/astro_gdt_fermi.egg-info/PKG-INFO
--rw-r--r--   0 wcleveland   (502) staff       (20)     1121 2023-04-12 20:35:33.000000 astro-gdt-fermi-2.0.0/src/astro_gdt_fermi.egg-info/SOURCES.txt
--rw-r--r--   0 wcleveland   (502) staff       (20)        1 2023-04-12 20:35:33.000000 astro-gdt-fermi-2.0.0/src/astro_gdt_fermi.egg-info/dependency_links.txt
--rw-r--r--   0 wcleveland   (502) staff       (20)      120 2023-04-12 20:35:33.000000 astro-gdt-fermi-2.0.0/src/astro_gdt_fermi.egg-info/requires.txt
--rw-r--r--   0 wcleveland   (502) staff       (20)        4 2023-04-12 20:35:33.000000 astro-gdt-fermi-2.0.0/src/astro_gdt_fermi.egg-info/top_level.txt
-drwxr-xr-x   0 wcleveland   (502) staff       (20)        0 2023-04-12 20:35:33.201795 astro-gdt-fermi-2.0.0/src/gdt/
-drwxr-xr-x   0 wcleveland   (502) staff       (20)        0 2023-04-12 20:35:33.209926 astro-gdt-fermi-2.0.0/src/gdt/data/
--rw-r--r--   0 wcleveland   (502) staff       (20)     1324 2023-04-12 13:20:21.000000 astro-gdt-fermi-2.0.0/src/gdt/data/fermi-gbm.urls
-drwxr-xr-x   0 wcleveland   (502) staff       (20)        0 2023-04-12 20:35:33.201963 astro-gdt-fermi-2.0.0/src/gdt/missions/
-drwxr-xr-x   0 wcleveland   (502) staff       (20)        0 2023-04-12 20:35:33.213989 astro-gdt-fermi-2.0.0/src/gdt/missions/fermi/
--rw-r--r--   0 wcleveland   (502) staff       (20)     1097 2023-04-12 19:42:50.000000 astro-gdt-fermi-2.0.0/src/gdt/missions/fermi/__init__.py
-drwxr-xr-x   0 wcleveland   (502) staff       (20)        0 2023-04-12 20:35:33.214948 astro-gdt-fermi-2.0.0/src/gdt/missions/fermi/data/
--rw-r--r--   0 wcleveland   (502) staff       (20)     1232 2023-03-28 16:42:58.000000 astro-gdt-fermi-2.0.0/src/gdt/missions/fermi/data/McIlwainL_Coeffs.npy
--rw-r--r--   0 wcleveland   (502) staff       (20)     2999 2023-03-28 16:42:58.000000 astro-gdt-fermi-2.0.0/src/gdt/missions/fermi/frame.py
-drwxr-xr-x   0 wcleveland   (502) staff       (20)        0 2023-04-12 20:35:33.229011 astro-gdt-fermi-2.0.0/src/gdt/missions/fermi/gbm/
--rw-r--r--   0 wcleveland   (502) staff       (20)        0 2023-03-23 21:39:17.000000 astro-gdt-fermi-2.0.0/src/gdt/missions/fermi/gbm/__init__.py
--rw-r--r--   0 wcleveland   (502) staff       (20)     2562 2023-03-28 23:06:31.000000 astro-gdt-fermi-2.0.0/src/gdt/missions/fermi/gbm/catalogs.py
--rw-r--r--   0 wcleveland   (502) staff       (20)     8443 2023-03-28 17:13:33.000000 astro-gdt-fermi-2.0.0/src/gdt/missions/fermi/gbm/collection.py
--rw-r--r--   0 wcleveland   (502) staff       (20)     3902 2023-03-28 17:13:33.000000 astro-gdt-fermi-2.0.0/src/gdt/missions/fermi/gbm/detectors.py
--rw-r--r--   0 wcleveland   (502) staff       (20)    20605 2023-03-31 16:57:31.000000 astro-gdt-fermi-2.0.0/src/gdt/missions/fermi/gbm/finders.py
--rw-r--r--   0 wcleveland   (502) staff       (20)    30382 2023-03-28 17:13:33.000000 astro-gdt-fermi-2.0.0/src/gdt/missions/fermi/gbm/headers.py
--rw-r--r--   0 wcleveland   (502) staff       (20)    33460 2023-03-28 17:13:33.000000 astro-gdt-fermi-2.0.0/src/gdt/missions/fermi/gbm/localization.py
--rw-r--r--   0 wcleveland   (502) staff       (20)     8466 2023-03-28 17:13:33.000000 astro-gdt-fermi-2.0.0/src/gdt/missions/fermi/gbm/phaii.py
--rw-r--r--   0 wcleveland   (502) staff       (20)     4062 2023-03-23 21:39:17.000000 astro-gdt-fermi-2.0.0/src/gdt/missions/fermi/gbm/poshist.py
--rw-r--r--   0 wcleveland   (502) staff       (20)    12107 2023-03-28 17:13:33.000000 astro-gdt-fermi-2.0.0/src/gdt/missions/fermi/gbm/response.py
--rw-r--r--   0 wcleveland   (502) staff       (20)     1781 2023-03-28 17:13:33.000000 astro-gdt-fermi-2.0.0/src/gdt/missions/fermi/gbm/saa.py
--rw-r--r--   0 wcleveland   (502) staff       (20)    22808 2023-03-28 23:15:20.000000 astro-gdt-fermi-2.0.0/src/gdt/missions/fermi/gbm/scat.py
--rw-r--r--   0 wcleveland   (502) staff       (20)     3755 2023-03-28 17:13:33.000000 astro-gdt-fermi-2.0.0/src/gdt/missions/fermi/gbm/tcat.py
--rw-r--r--   0 wcleveland   (502) staff       (20)    51161 2023-03-28 17:13:33.000000 astro-gdt-fermi-2.0.0/src/gdt/missions/fermi/gbm/trigdat.py
--rw-r--r--   0 wcleveland   (502) staff       (20)     7675 2023-03-28 17:13:33.000000 astro-gdt-fermi-2.0.0/src/gdt/missions/fermi/gbm/tte.py
-drwxr-xr-x   0 wcleveland   (502) staff       (20)        0 2023-04-12 20:35:33.229645 astro-gdt-fermi-2.0.0/src/gdt/missions/fermi/lat/
--rw-r--r--   0 wcleveland   (502) staff       (20)        0 2023-03-23 21:39:17.000000 astro-gdt-fermi-2.0.0/src/gdt/missions/fermi/lat/__init__.py
--rw-r--r--   0 wcleveland   (502) staff       (20)     3347 2023-03-28 16:42:58.000000 astro-gdt-fermi-2.0.0/src/gdt/missions/fermi/mcilwainl.py
--rw-r--r--   0 wcleveland   (502) staff       (20)    12829 2023-03-28 16:42:58.000000 astro-gdt-fermi-2.0.0/src/gdt/missions/fermi/plot.py
--rw-r--r--   0 wcleveland   (502) staff       (20)     6513 2023-03-28 16:42:58.000000 astro-gdt-fermi-2.0.0/src/gdt/missions/fermi/time.py
+drwxr-xr-x   0 wcleveland   (502) staff       (20)        0 2024-06-03 14:19:14.988303 astro_gdt_fermi-2.1.0/
+-rw-r--r--   0 wcleveland   (502) staff       (20)       43 2023-04-12 13:20:21.000000 astro_gdt_fermi-2.1.0/MANIFEST.in
+-rw-r--r--   0 wcleveland   (502) staff       (20)     1942 2024-06-03 14:19:14.987714 astro_gdt_fermi-2.1.0/PKG-INFO
+-rw-r--r--   0 wcleveland   (502) staff       (20)      847 2023-11-30 19:03:33.000000 astro_gdt_fermi-2.1.0/PYPI-README.rst
+-rw-r--r--   0 wcleveland   (502) staff       (20)     3486 2024-06-03 13:57:55.000000 astro_gdt_fermi-2.1.0/README.rst
+-rw-r--r--   0 wcleveland   (502) staff       (20)    11357 2023-03-28 16:42:58.000000 astro_gdt_fermi-2.1.0/license.txt
+drwxr-xr-x   0 wcleveland   (502) staff       (20)        0 2024-06-03 14:19:14.921784 astro_gdt_fermi-2.1.0/scripts/
+-rwxr-xr-x   0 wcleveland   (502) staff       (20)     2198 2024-06-03 13:57:55.000000 astro_gdt_fermi-2.1.0/scripts/dol4.exe
+-rwxr-xr-x   0 wcleveland   (502) staff       (20)     4681 2024-06-03 13:57:55.000000 astro_gdt_fermi-2.1.0/scripts/dol_source_angles.py
+-rw-r--r--   0 wcleveland   (502) staff       (20)       38 2024-06-03 14:19:14.988449 astro_gdt_fermi-2.1.0/setup.cfg
+-rw-r--r--   0 wcleveland   (502) staff       (20)     3759 2024-06-03 13:57:55.000000 astro_gdt_fermi-2.1.0/setup.py
+drwxr-xr-x   0 wcleveland   (502) staff       (20)        0 2024-06-03 14:19:14.913944 astro_gdt_fermi-2.1.0/src/
+drwxr-xr-x   0 wcleveland   (502) staff       (20)        0 2024-06-03 14:19:14.986528 astro_gdt_fermi-2.1.0/src/astro_gdt_fermi.egg-info/
+-rw-r--r--   0 wcleveland   (502) staff       (20)     1942 2024-06-03 14:19:14.000000 astro_gdt_fermi-2.1.0/src/astro_gdt_fermi.egg-info/PKG-INFO
+-rw-r--r--   0 wcleveland   (502) staff       (20)     2079 2024-06-03 14:19:14.000000 astro_gdt_fermi-2.1.0/src/astro_gdt_fermi.egg-info/SOURCES.txt
+-rw-r--r--   0 wcleveland   (502) staff       (20)        1 2024-06-03 14:19:14.000000 astro_gdt_fermi-2.1.0/src/astro_gdt_fermi.egg-info/dependency_links.txt
+-rw-r--r--   0 wcleveland   (502) staff       (20)      120 2024-06-03 14:19:14.000000 astro_gdt_fermi-2.1.0/src/astro_gdt_fermi.egg-info/requires.txt
+-rw-r--r--   0 wcleveland   (502) staff       (20)        4 2024-06-03 14:19:14.000000 astro_gdt_fermi-2.1.0/src/astro_gdt_fermi.egg-info/top_level.txt
+drwxr-xr-x   0 wcleveland   (502) staff       (20)        0 2024-06-03 14:19:14.914626 astro_gdt_fermi-2.1.0/src/gdt/
+drwxr-xr-x   0 wcleveland   (502) staff       (20)        0 2024-06-03 14:19:14.925611 astro_gdt_fermi-2.1.0/src/gdt/data/
+-rw-r--r--   0 wcleveland   (502) staff       (20)     1324 2023-04-12 13:20:21.000000 astro_gdt_fermi-2.1.0/src/gdt/data/fermi-gbm.urls
+drwxr-xr-x   0 wcleveland   (502) staff       (20)        0 2024-06-03 14:19:14.914903 astro_gdt_fermi-2.1.0/src/gdt/missions/
+drwxr-xr-x   0 wcleveland   (502) staff       (20)        0 2024-06-03 14:19:14.929724 astro_gdt_fermi-2.1.0/src/gdt/missions/fermi/
+-rw-r--r--   0 wcleveland   (502) staff       (20)     1097 2024-06-03 14:00:05.000000 astro_gdt_fermi-2.1.0/src/gdt/missions/fermi/__init__.py
+drwxr-xr-x   0 wcleveland   (502) staff       (20)        0 2024-06-03 14:19:14.930174 astro_gdt_fermi-2.1.0/src/gdt/missions/fermi/data/
+-rw-r--r--   0 wcleveland   (502) staff       (20)     1232 2023-03-28 16:42:58.000000 astro_gdt_fermi-2.1.0/src/gdt/missions/fermi/data/McIlwainL_Coeffs.npy
+-rw-r--r--   0 wcleveland   (502) staff       (20)     2999 2023-03-28 16:42:58.000000 astro_gdt_fermi-2.1.0/src/gdt/missions/fermi/frame.py
+drwxr-xr-x   0 wcleveland   (502) staff       (20)        0 2024-06-03 14:19:14.942258 astro_gdt_fermi-2.1.0/src/gdt/missions/fermi/gbm/
+-rw-r--r--   0 wcleveland   (502) staff       (20)        0 2023-03-23 21:39:17.000000 astro_gdt_fermi-2.1.0/src/gdt/missions/fermi/gbm/__init__.py
+-rw-r--r--   0 wcleveland   (502) staff       (20)     2562 2023-03-28 23:06:31.000000 astro_gdt_fermi-2.1.0/src/gdt/missions/fermi/gbm/catalogs.py
+-rw-r--r--   0 wcleveland   (502) staff       (20)     8443 2023-03-28 17:13:33.000000 astro_gdt_fermi-2.1.0/src/gdt/missions/fermi/gbm/collection.py
+-rw-r--r--   0 wcleveland   (502) staff       (20)     3902 2023-03-28 17:13:33.000000 astro_gdt_fermi-2.1.0/src/gdt/missions/fermi/gbm/detectors.py
+-rw-r--r--   0 wcleveland   (502) staff       (20)    20605 2023-03-31 16:57:31.000000 astro_gdt_fermi-2.1.0/src/gdt/missions/fermi/gbm/finders.py
+-rw-r--r--   0 wcleveland   (502) staff       (20)    30384 2024-06-03 13:21:37.000000 astro_gdt_fermi-2.1.0/src/gdt/missions/fermi/gbm/headers.py
+drwxr-xr-x   0 wcleveland   (502) staff       (20)        0 2024-06-03 14:19:14.943198 astro_gdt_fermi-2.1.0/src/gdt/missions/fermi/gbm/localization/
+-rw-r--r--   0 wcleveland   (502) staff       (20)    35741 2024-06-03 13:57:55.000000 astro_gdt_fermi-2.1.0/src/gdt/missions/fermi/gbm/localization/__init__.py
+drwxr-xr-x   0 wcleveland   (502) staff       (20)        0 2024-06-03 14:19:14.945704 astro_gdt_fermi-2.1.0/src/gdt/missions/fermi/gbm/localization/dol/
+-rwxr-xr-x   0 wcleveland   (502) staff       (20)     1537 2024-06-03 13:57:55.000000 astro_gdt_fermi-2.1.0/src/gdt/missions/fermi/gbm/localization/dol/__init__.py
+drwxr-xr-x   0 wcleveland   (502) staff       (20)        0 2024-06-03 14:19:14.984452 astro_gdt_fermi-2.1.0/src/gdt/missions/fermi/gbm/localization/dol/data/
+-rw-r--r--   0 wcleveland   (502) staff       (20)   287104 2024-06-03 13:57:55.000000 astro_gdt_fermi-2.1.0/src/gdt/missions/fermi/gbm/localization/dol/data/alocdat_comp.npy
+-rw-r--r--   0 wcleveland   (502) staff       (20)  2305801 2024-06-03 13:57:55.000000 astro_gdt_fermi-2.1.0/src/gdt/missions/fermi/gbm/localization/dol/data/band_1deg_50_300_hard.npy
+-rw-r--r--   0 wcleveland   (502) staff       (20)  2305801 2024-06-03 13:57:55.000000 astro_gdt_fermi-2.1.0/src/gdt/missions/fermi/gbm/localization/dol/data/band_1deg_50_300_norm.npy
+-rw-r--r--   0 wcleveland   (502) staff       (20)  2305801 2024-06-03 13:57:55.000000 astro_gdt_fermi-2.1.0/src/gdt/missions/fermi/gbm/localization/dol/data/band_1deg_50_300_soft.npy
+-rw-r--r--   0 wcleveland   (502) staff       (20)  2305801 2024-06-03 13:57:55.000000 astro_gdt_fermi-2.1.0/src/gdt/missions/fermi/gbm/localization/dol/data/band_1deg_5_50_soft.npy
+-rw-r--r--   0 wcleveland   (502) staff       (20)  2305759 2024-06-03 13:57:55.000000 astro_gdt_fermi-2.1.0/src/gdt/missions/fermi/gbm/localization/dol/data/comp_1deg_50_300_hard.npy
+-rw-r--r--   0 wcleveland   (502) staff       (20)  2305759 2024-06-03 13:57:55.000000 astro_gdt_fermi-2.1.0/src/gdt/missions/fermi/gbm/localization/dol/data/comp_1deg_50_300_norm.npy
+-rw-r--r--   0 wcleveland   (502) staff       (20)  2305759 2024-06-03 13:57:55.000000 astro_gdt_fermi-2.1.0/src/gdt/missions/fermi/gbm/localization/dol/data/comp_1deg_50_300_soft.npy
+-rw-r--r--   0 wcleveland   (502) staff       (20)     2960 2024-06-03 13:57:55.000000 astro_gdt_fermi-2.1.0/src/gdt/missions/fermi/gbm/localization/dol/data/earth_points.npy
+-rwxr-xr-x   0 wcleveland   (502) staff       (20)    30658 2024-06-03 13:57:55.000000 astro_gdt_fermi-2.1.0/src/gdt/missions/fermi/gbm/localization/dol/legacy_dol.py
+-rwxr-xr-x   0 wcleveland   (502) staff       (20)    65342 2024-06-03 13:57:55.000000 astro_gdt_fermi-2.1.0/src/gdt/missions/fermi/gbm/localization/dol/legacy_functions.py
+-rwxr-xr-x   0 wcleveland   (502) staff       (20)     4229 2024-06-03 13:57:55.000000 astro_gdt_fermi-2.1.0/src/gdt/missions/fermi/gbm/localization/dol/legacy_spectral_models.py
+-rw-r--r--   0 wcleveland   (502) staff       (20)     8466 2023-03-28 17:13:33.000000 astro_gdt_fermi-2.1.0/src/gdt/missions/fermi/gbm/phaii.py
+-rw-r--r--   0 wcleveland   (502) staff       (20)     4062 2023-03-23 21:39:17.000000 astro_gdt_fermi-2.1.0/src/gdt/missions/fermi/gbm/poshist.py
+-rw-r--r--   0 wcleveland   (502) staff       (20)    12107 2023-03-28 17:13:33.000000 astro_gdt_fermi-2.1.0/src/gdt/missions/fermi/gbm/response.py
+-rw-r--r--   0 wcleveland   (502) staff       (20)     1781 2023-03-28 17:13:33.000000 astro_gdt_fermi-2.1.0/src/gdt/missions/fermi/gbm/saa.py
+-rw-r--r--   0 wcleveland   (502) staff       (20)    22808 2023-03-28 23:15:20.000000 astro_gdt_fermi-2.1.0/src/gdt/missions/fermi/gbm/scat.py
+-rw-r--r--   0 wcleveland   (502) staff       (20)     3755 2023-03-28 17:13:33.000000 astro_gdt_fermi-2.1.0/src/gdt/missions/fermi/gbm/tcat.py
+-rw-r--r--   0 wcleveland   (502) staff       (20)    51835 2024-06-03 13:21:37.000000 astro_gdt_fermi-2.1.0/src/gdt/missions/fermi/gbm/trigdat.py
+-rw-r--r--   0 wcleveland   (502) staff       (20)     8308 2023-12-03 22:26:54.000000 astro_gdt_fermi-2.1.0/src/gdt/missions/fermi/gbm/tte.py
+drwxr-xr-x   0 wcleveland   (502) staff       (20)        0 2024-06-03 14:19:14.985664 astro_gdt_fermi-2.1.0/src/gdt/missions/fermi/lat/
+-rw-r--r--   0 wcleveland   (502) staff       (20)        0 2023-03-23 21:39:17.000000 astro_gdt_fermi-2.1.0/src/gdt/missions/fermi/lat/__init__.py
+-rw-r--r--   0 wcleveland   (502) staff       (20)     3347 2023-03-28 16:42:58.000000 astro_gdt_fermi-2.1.0/src/gdt/missions/fermi/mcilwainl.py
+-rw-r--r--   0 wcleveland   (502) staff       (20)    12939 2023-11-30 19:03:33.000000 astro_gdt_fermi-2.1.0/src/gdt/missions/fermi/plot.py
+-rw-r--r--   0 wcleveland   (502) staff       (20)     6497 2024-06-03 13:57:55.000000 astro_gdt_fermi-2.1.0/src/gdt/missions/fermi/time.py
```

### Comparing `astro-gdt-fermi-2.0.0/PKG-INFO` & `astro_gdt_fermi-2.1.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro-gdt-fermi
-Version: 2.0.0
+Version: 2.1.0
 Summary: Gamma-ray Data Tools: Fermi Mission
 Home-page: https://github.com/USRA-STI/gdt-fermi
 Author: Cleveland, Goldstein, Kocevski
 Project-URL: Documentation, https://astro-gdt-fermi.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/USRA-STI/gdt-fermi
 Project-URL: Tracker, https://github.com/USRA-STI/gdt-fermi/issues
 Keywords: astronomy,gammaray,gamma-ray,usra
@@ -13,14 +13,22 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 License-File: license.txt
+Requires-Dist: astro-gdt>=2.0.0
+Requires-Dist: pyproj>=1.9.6
+Requires-Dist: numpy>=1.17.3
+Requires-Dist: scipy>=1.1.0
+Requires-Dist: matplotlib>=3.7.1
+Requires-Dist: astropy>=3.1
+Requires-Dist: healpy>=1.12.4
+Requires-Dist: cartopy>=0.21.1
 
 =========
 GDT-Fermi
 =========
 
 The GDT-Fermi is an extension to Gamma-ray Data Tools that adds functions specific to the Fermi mission (GBM and LAT).
 
@@ -30,15 +38,15 @@
 If you don't plan to contribute code to the project, the recommended install method is installing from PyPI using:
 
 .. code-block:: sh
 
    pip install astro-gdt-fermi
    gdt-data init
 
-The ``gdt data init`` is required to initialize the library after installation of astro-gdt. You do not need to
+The ``gdt-data init`` is required to initialize the library after installation of astro-gdt. You do not need to
 perform the initialization again if astro-gdt was already installed and initialized.  There is no harm in running
 it again "just in case".
 
 Contributing Code or Documentation
 ----------------------------------
 
 If you plan to help with the development or documentation of astro-gdt, then please visit our github site at
```

### Comparing `astro-gdt-fermi-2.0.0/PYPI-README.rst` & `astro_gdt_fermi-2.1.0/PYPI-README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 If you don't plan to contribute code to the project, the recommended install method is installing from PyPI using:
 
 .. code-block:: sh
 
    pip install astro-gdt-fermi
    gdt-data init
 
-The ``gdt data init`` is required to initialize the library after installation of astro-gdt. You do not need to
+The ``gdt-data init`` is required to initialize the library after installation of astro-gdt. You do not need to
 perform the initialization again if astro-gdt was already installed and initialized.  There is no harm in running
 it again "just in case".
 
 Contributing Code or Documentation
 ----------------------------------
 
 If you plan to help with the development or documentation of astro-gdt, then please visit our github site at
```

### Comparing `astro-gdt-fermi-2.0.0/README.rst` & `astro_gdt_fermi-2.1.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 =========
 GDT-Fermi
 =========
 
 The GDT-Fermi is an extension to Gamma-ray Data Tools that adds functions specific to the Fermi mission (GBM and LAT).
 
+The full documentation can be found `here <https://astro-gdt.readthedocs.io/projects/astro-gdt-fermi/en/latest/>`_.
+
 Normal Installation
 -------------------
 
 If you don't plan to contribute code to the project, the recommended install method is installing from PyPI using:
 
 .. code-block:: sh
 
    pip install astro-gdt-fermi
    gdt-data init
 
-The ``gdt data init`` is required to initialize the library after installation of astro-gdt. You do not need to
+The ``gdt-data init`` is required to initialize the library after installation of astro-gdt. You do not need to
 perform the initialization again if astro-gdt was already installed and initialized.  There is no harm in running
 it again "just in case".
 
 
 Setting up a development environment
 ------------------------------------
 
@@ -86,16 +88,16 @@
 
 You can learn more about Namespace packages by reading `PEP-420 <https://peps.python.org/pep-0420/>`_.
 
 Helping with Documentation
 --------------------------
 
 You can contribute additions and changes to the documentation. In order to use sphinx to compile the documentation
-source files, we recommend that you install the packages contained within ``requirments.txt``.
+source files, we recommend that you install the packages contained within ``requirements.txt``.
 
 To compile the documentation, use the following commands:
 
 .. code-block:: sh
 
-   cd gdt-core/docs
+   cd gdt-fermi/docs
    make html
```

### Comparing `astro-gdt-fermi-2.0.0/license.txt` & `astro_gdt_fermi-2.1.0/license.txt`

 * *Files identical despite different names*

### Comparing `astro-gdt-fermi-2.0.0/setup.py` & `astro_gdt_fermi-2.1.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -54,16 +54,31 @@
             "Topic :: Software Development :: Libraries",
         ],
         license_files=['license.txt'],
         keywords=['astronomy', 'gammaray', 'gamma-ray', 'usra'],
         package_dir={"": "src"},
         package_data={
             'gdt.missions.fermi': ['data/McIlwainL_Coeffs.npy'],
-            'gdt.data': ['fermi-gbm.urls']
+            'gdt.data': ['fermi-gbm.urls'],
+            'gdt.missions.fermi.gbm.localization.dol.data': [
+                'alocdat_comp.npy',
+                'band_1deg_5_50_soft.npy',
+                'band_1deg_50_300_hard.npy',
+                'band_1deg_50_300_norm.npy',
+                'band_1deg_50_300_soft.npy',
+                'comp_1deg_50_300_hard.npy',
+                'comp_1deg_50_300_norm.npy',
+                'comp_1deg_50_300_soft.npy',
+                'earth_points.npy',
+            ],
         },
+        scripts=[
+            'scripts/dol4.exe',
+            'scripts/dol_source_angles.py'
+        ],
         include_package_data=True,
         python_requires='>=3.8',
         install_requires=[
             'astro-gdt>=2.0.0',
             'pyproj>=1.9.6',
             'numpy>=1.17.3',
             'scipy>=1.1.0',
```

### Comparing `astro-gdt-fermi-2.0.0/src/astro_gdt_fermi.egg-info/PKG-INFO` & `astro_gdt_fermi-2.1.0/src/astro_gdt_fermi.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro-gdt-fermi
-Version: 2.0.0
+Version: 2.1.0
 Summary: Gamma-ray Data Tools: Fermi Mission
 Home-page: https://github.com/USRA-STI/gdt-fermi
 Author: Cleveland, Goldstein, Kocevski
 Project-URL: Documentation, https://astro-gdt-fermi.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/USRA-STI/gdt-fermi
 Project-URL: Tracker, https://github.com/USRA-STI/gdt-fermi/issues
 Keywords: astronomy,gammaray,gamma-ray,usra
@@ -13,14 +13,22 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 License-File: license.txt
+Requires-Dist: astro-gdt>=2.0.0
+Requires-Dist: pyproj>=1.9.6
+Requires-Dist: numpy>=1.17.3
+Requires-Dist: scipy>=1.1.0
+Requires-Dist: matplotlib>=3.7.1
+Requires-Dist: astropy>=3.1
+Requires-Dist: healpy>=1.12.4
+Requires-Dist: cartopy>=0.21.1
 
 =========
 GDT-Fermi
 =========
 
 The GDT-Fermi is an extension to Gamma-ray Data Tools that adds functions specific to the Fermi mission (GBM and LAT).
 
@@ -30,15 +38,15 @@
 If you don't plan to contribute code to the project, the recommended install method is installing from PyPI using:
 
 .. code-block:: sh
 
    pip install astro-gdt-fermi
    gdt-data init
 
-The ``gdt data init`` is required to initialize the library after installation of astro-gdt. You do not need to
+The ``gdt-data init`` is required to initialize the library after installation of astro-gdt. You do not need to
 perform the initialization again if astro-gdt was already installed and initialized.  There is no harm in running
 it again "just in case".
 
 Contributing Code or Documentation
 ----------------------------------
 
 If you plan to help with the development or documentation of astro-gdt, then please visit our github site at
```

### Comparing `astro-gdt-fermi-2.0.0/src/gdt/data/fermi-gbm.urls` & `astro_gdt_fermi-2.1.0/src/gdt/data/fermi-gbm.urls`

 * *Files identical despite different names*

### Comparing `astro-gdt-fermi-2.0.0/src/gdt/missions/fermi/__init__.py` & `astro_gdt_fermi-2.1.0/src/gdt/missions/fermi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License
 # is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
 # implied. See the License for the specific language governing permissions and limitations under the
 # License.
 #
-__version__ = '2.0.0'
+__version__ = '2.1.0'
```

### Comparing `astro-gdt-fermi-2.0.0/src/gdt/missions/fermi/data/McIlwainL_Coeffs.npy` & `astro_gdt_fermi-2.1.0/src/gdt/missions/fermi/data/McIlwainL_Coeffs.npy`

 * *Files identical despite different names*

### Comparing `astro-gdt-fermi-2.0.0/src/gdt/missions/fermi/frame.py` & `astro_gdt_fermi-2.1.0/src/gdt/missions/fermi/frame.py`

 * *Files identical despite different names*

### Comparing `astro-gdt-fermi-2.0.0/src/gdt/missions/fermi/gbm/catalogs.py` & `astro_gdt_fermi-2.1.0/src/gdt/missions/fermi/gbm/catalogs.py`

 * *Files identical despite different names*

### Comparing `astro-gdt-fermi-2.0.0/src/gdt/missions/fermi/gbm/collection.py` & `astro_gdt_fermi-2.1.0/src/gdt/missions/fermi/gbm/collection.py`

 * *Files identical despite different names*

### Comparing `astro-gdt-fermi-2.0.0/src/gdt/missions/fermi/gbm/detectors.py` & `astro_gdt_fermi-2.1.0/src/gdt/missions/fermi/gbm/detectors.py`

 * *Files identical despite different names*

### Comparing `astro-gdt-fermi-2.0.0/src/gdt/missions/fermi/gbm/finders.py` & `astro_gdt_fermi-2.1.0/src/gdt/missions/fermi/gbm/finders.py`

 * *Files identical despite different names*

### Comparing `astro-gdt-fermi-2.0.0/src/gdt/missions/fermi/gbm/headers.py` & `astro_gdt_fermi-2.1.0/src/gdt/missions/fermi/gbm/headers.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,17 +92,17 @@
 
 #----------------
 class GbmHeader(Header):
 
     def __setitem__(self, key, val):
         if not isinstance(key, tuple):
             if key.upper() == 'TSTART':
-                self['DATE-OBS'] = Time(val, format='fermi').iso
+                self['DATE-OBS'] = Time(val, format='fermi').isot
             elif key.upper() == 'TSTOP':
-                self['DATE-END'] = Time(val, format='fermi').iso
+                self['DATE-END'] = Time(val, format='fermi').isot
             else:
                 pass
 
             if 'INFILE' in key.upper():
                 super(Header, self).__setitem__(key, val)
                 return
```

### Comparing `astro-gdt-fermi-2.0.0/src/gdt/missions/fermi/gbm/localization.py` & `astro_gdt_fermi-2.1.0/src/gdt/missions/fermi/gbm/localization/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,32 +26,36 @@
 # implied. See the License for the specific language governing permissions and limitations under the
 # License.
 #
 import warnings
 import astropy.io.fits as fits
 import numpy as np
 from scipy.stats import chi2
+import scipy.interpolate
 import healpy as hp
-from astropy.coordinates import get_sun, SkyCoord
+from astropy.coordinates import get_sun, SkyCoord, angular_separation
 from astropy.coordinates.representation import CartesianRepresentation
 from astropy.units import Quantity
 
-from gdt.core.coords import SpacecraftFrame, Quaternion
+from gdt.core.coords import Quaternion
 from gdt.core.file import FitsFileContextManager
 from gdt.core.healpix import HealPixLocalization
-from ..time import Time
-from .detectors import GbmDetectors
-from .headers import HealpixHeaders
+from gdt.missions.fermi.frame import *
+from gdt.missions.fermi.time import Time
+from gdt.missions.fermi.gbm.detectors import GbmDetectors
+from gdt.missions.fermi.gbm.headers import HealpixHeaders
 
 __all__ = ['GbmHealPix', 'Chi2Grid', 'ga_model', 'gbuts_o3_model', 'hitl_model',
            'robo_ba_model', 'untargeted_search_model']
 
+
 class GbmHealPix(HealPixLocalization, FitsFileContextManager):
     """Class for GBM HEALPix localization files.
     """
+
     def __init__(self):
         HealPixLocalization.__init__(self)
         FitsFileContextManager.__init__(self)
         self._frame = None
         self._geo_loc = None
         self._geo_rad = None
         self._quat = None
@@ -59,18 +63,18 @@
         self._sun_loc = None
 
     @property
     def frame(self):
         """(:class:`~gdt.core.coords.SpacecraftFrame`): The spacecraft frame at
         the time of the localization"""
         return self._frame
-    
+
     @property
     def geo_location(self):
-        """(astropy.coordinates.SkyCoord): The geocenter location at 
+        """(astropy.coordinates.SkyCoord): The geocenter location at
         :attr:`trigtime`"""
         return self._geo_loc
 
     @property
     def geo_probability(self):
         """(float): The amount of localization probability on the Earth"""
         if self.geo_location is None:
@@ -78,232 +82,252 @@
         prob_mask, geo_mask = self._earth_mask()
         return self.prob[prob_mask][geo_mask].sum()
 
     @property
     def geo_radius(self):
         """(astropy.units.Quantity): The apparent angular radius of the Earth at
         :attr:`trigtime`.
-        
+
         Note:
             If a :attr:`scpos` isn't set, then an average 67.5 deg is returned
         """
         # if the radius isn't known, use the average 67.5 deg radius
         if self._geo_rad is not None:
             return self._geo_rad
         else:
             return Quantity(67.5, unit='deg')
 
     @property
     def quaternion(self):
-        """(:class:`~gdt.core.coords.Quaternion`): The spacecraft attitude 
+        """(:class:`~gdt.core.coords.Quaternion`): The spacecraft attitude
         quaternion"""
         return self._quat
 
     @property
     def scpos(self):
-        """(np.array): The spacecraft position in Earth inertial coordinates"""
+        """(astropy.coordinates.CartesianRepresentation):
+           The spacecraft position in Earth inertial coordinates"""
         return self._scpos
 
     @property
     def sun_location(self):
-        """(astropy.coordinates.SkyCoord): The Sun location at 
+        """(astropy.coordinates.SkyCoord): The Sun location at
         :attr:`trigtime`"""
         return self._sun_loc
 
     @classmethod
-    def from_chi2grid(cls, chi2grid, nside=128, headers=None, filename=None):
+    def from_chi2grid(cls, chi2grid, nside=128, headers=None, filename=None, exact_nearest=False, grid_nearest=False):
         """Create a GbmHealPix object from a :class:`Chi2Grid` object.
-        
+
         Args:
-            chi2grid (:class:`Chi2Grid`): The chi2grid object containing the 
+            chi2grid (:class:`Chi2Grid`): The chi2grid object containing the
                                          chi-squared/log-likelihood info.
             nside (int, optional): The nside resolution to use. Default is 128.
             headers (:class:`~gdt.core.headers.FileHeaders`, optional):
                 The file headers
             filename (str, optional): The filename
-                    
-        Returns:        
+            exact_nearest (bool): Use exact nearest pixel interpolation when True.
+                                  This method is slow O(minute) due to
+                                  angular difference calculation.
+            grid_nearest (bool): Use approximate nearest pixel interpolation when True.
+                                 This method is fast O(second) by using 2D grid.
+
+        Returns:
             (:class:`GbmHealPix`)
         """
         if not isinstance(chi2grid, Chi2Grid):
             raise TypeError('chi2grid must be a Chi2Grid object')
-        
-        # fill up a low-resolution healpix map with significance
+
+        # convert chisq map to probability map assuming Wilk's theorem applies
+        loglike = -chi2grid.chisq / 2.0
+        probs = np.exp(loglike - np.max(loglike))
+
+        # fill a low-resolution healpix map with probability values
         lores_nside = 64
         lores_npix = hp.nside2npix(lores_nside)
-        lores_array = np.zeros((lores_npix))
+        lores_array = np.zeros(lores_npix)
         theta = cls._dec_to_theta(chi2grid.dec)
         phi = cls._ra_to_phi(chi2grid.ra)
-        idx = hp.ang2pix(lores_nside, theta, phi)
-        lores_array[idx] = chi2grid.significance
+        if exact_nearest:
+            # exact nearest pixel method using angular difference (slow)
+            lores_pix = np.arange(lores_npix)
+            proj_theta, proj_phi = hp.pix2ang(lores_nside, lores_pix)
+            idx = [angular_separation(proj_phi[i], 0.5 * np.pi - proj_theta[i],
+                                      phi, 0.5 * np.pi - theta).argmin() for i in lores_pix]
+            lores_array = probs[idx]
+        elif grid_nearest:
+            # approximate nearest pixel method using 2D grid (fast)
+            lores_pix = np.arange(lores_npix)
+            proj_theta, proj_phi = hp.pix2ang(lores_nside, lores_pix)
+            lores_array = scipy.interpolate.griddata((phi, theta), probs, (proj_phi, proj_theta), method='nearest')
+        else:
+            # basic healpix conversion (can result in missing pixels)
+            idx = hp.ang2pix(lores_nside, theta, phi)
+            lores_array[idx] = probs
 
         # upscale to high-resolution
         hires_nside = nside
         hires_npix = hp.nside2npix(hires_nside)
         theta, phi = hp.pix2ang(hires_nside, np.arange(hires_npix))
-
-        # convert chisq map to probability map
-        loglike = -chi2grid.chisq / 2.0
-        probs = np.exp(loglike - np.max(loglike))
-        lores_array = np.zeros(lores_npix)
-        lores_array[idx] = probs
         prob_array = hp.get_interp_val(lores_array, theta, phi)
 
-        obj = cls.from_data(prob_array, trigtime=chi2grid.trigtime, 
-                            headers=headers, filename=filename, 
-                            scpos=chi2grid.scpos, quaternion=chi2grid.quaternion)
+        quat = Quaternion(chi2grid.quaternion)
+        scpos = CartesianRepresentation(chi2grid.scpos, unit='m')
+
+        obj = cls.from_data(prob_array, trigtime=chi2grid.trigtime,
+                            headers=headers, filename=filename,
+                            scpos=scpos, quaternion=quat)
         return obj
 
     @classmethod
     def from_data(cls, prob_arr, trigtime=None, headers=None, filename=None,
                   quaternion=None, scpos=None):
         """Create a GbmHealPix object from a healpix array.
 
         Args:
-            prob_arr (np.array): 
+            prob_arr (np.array):
                 The HEALPix array containing the probability/pixel
-            trigtime (float, optional): 
+            trigtime (float, optional):
                 The time corresponding to the localization
             headers (:class:`~gdt.core.headers.FileHeaders`, optional):
                 The file headers
             filename (str, optional): The filename
-            quaternion (np.array, optional): 
-                The associated spacecraft quaternion used to determine the 
+            quaternion (:class:`~gdt.core.coords.Quaternion`, optional):
+                The associated spacecraft quaternion used to determine the
                 detector pointings in equatorial coordinates
-            scpos (np.array, optional): 
-                The associated spacecraft position in Earth inertial coordinates 
-                used to determine the geocenter location in equatorial 
+            scpos (np.array, optional):
+                The associated spacecraft position in Earth inertial coordinates
+                used to determine the geocenter location in equatorial
                 coordinates
-            
-        Returns:        
+
+        Returns:
             (:class:`GbmHealPix`)
         """
         obj = super().from_data(prob_arr, trigtime=trigtime, filename=filename)
 
         if headers is not None:
             if not isinstance(headers, HealpixHeaders):
                 raise TypeError('headers must be a HealpixHeaders object')
+        else:
+            headers = cls._none_default_headers()
         obj._headers = headers
-        
+
         if quaternion is not None:
-            try:
-                iter(quaternion)
-                quaternion = np.asarray(quaternion)
-            except:
-                raise TypeError('quaternion must be an array')
-            if quaternion.size != 4:
-                raise ValueError('quaternion must be a 4-element array')
-            
+            if not isinstance(quaternion, Quaternion):
+                raise TypeError('quaternion must be a Quaternion object')
+
         if scpos is not None:
-            try:
-                iter(scpos)
-                scpos = np.asarray(scpos)
-            except:
-                raise TypeError('scpos must be an array')
-            if scpos.size != 3:
-                raise ValueError('scpos must be a 3-element array')
-        
+            if not isinstance(scpos, CartesianRepresentation):
+                raise TypeError('scpos must be a CartesianRepresentation object')
+
         # if we have a trigtime, calculate sun position
         if trigtime is not None:
             obj._sun_loc = get_sun(Time(trigtime, format='fermi'))
-        elif obj._headers is not None:
-            obj._sun_loc = SkyCoord(obj._headers[1]['SUN_RA'], 
+        elif obj._headers[1]['SUN_RA'] is not None:
+            obj._sun_loc = SkyCoord(obj._headers[1]['SUN_RA'],
                                     obj._headers[1]['SUN_DEC'], unit='deg',
                                     frame='gcrs')
-        
+        else:
+            obj._sun_loc = None
+
         if (trigtime is not None) and (scpos is not None) and \
-           (quaternion is not None):
+                (quaternion is not None):
             obj._scpos = scpos
-            obj._quat = Quaternion(quaternion)
-            
-            obj._frame = SpacecraftFrame(obstime=Time(trigtime, format='fermi'),
-                                         quaternion=obj._quat,
-                             obsgeoloc=CartesianRepresentation(scpos, unit='m'),
-                             detectors=GbmDetectors)
-            
+            obj._quat = quaternion
+
+            obj._frame = FermiFrame(obstime=Time(trigtime, format='fermi'),
+                                    quaternion=obj._quat, obsgeoloc=scpos,
+                                    detectors=GbmDetectors)
+
             obj._geo_loc = obj._frame.geocenter
             obj._geo_rad = obj._frame.earth_angular_radius
             for det in obj._frame.detectors:
                 pointing = (det.azimuth, det.elevation)
                 det_coord = SkyCoord(*pointing, frame=obj._frame).gcrs[0]
                 setattr(obj, det.name.lower() + '_pointing', det_coord)
-        else:
-            if obj._headers is not None:
-                
-                obj._geo_loc = SkyCoord(obj._headers[1]['GEO_RA'], 
-                                        obj._headers[1]['GEO_DEC'], unit='deg',
-                                        frame='gcrs')
-                
-                for det in GbmDetectors:
-                    ra_key = det.name.upper() + '_RA'
-                    dec_key = det.name.upper() + '_DEC'
-                    det_coord = SkyCoord(obj._headers[1][ra_key], 
-                                         obj._headers[1][dec_key], unit='deg', 
-                                         frame='gcrs')
-                    setattr(obj, det.name.lower() + '_pointing', det_coord)
-                                
+        elif obj._headers[1]['GEO_RA'] is not None:
+
+            obj._geo_loc = SkyCoord(obj._headers[1]['GEO_RA'],
+                                    obj._headers[1]['GEO_DEC'], unit='deg',
+                                    frame='gcrs')
+            obj._geo_rad = Quantity(obj._headers[1]['GEO_RAD'], unit='deg')
+
+            for det in GbmDetectors:
+                ra_key = det.name.upper() + '_RA'
+                dec_key = det.name.upper() + '_DEC'
+                det_coord = SkyCoord(obj._headers[1][ra_key],
+                                     obj._headers[1][dec_key], unit='deg',
+                                     frame='gcrs')
+                setattr(obj, det.name.lower() + '_pointing', det_coord)
+
+        obj._headers = obj._build_headers(obj.trigtime, obj.nside)
 
         return obj
 
     @classmethod
     def multiply(cls, healpix1, healpix2, primary=0, output_nside=128):
         """Multiply two GbmHealPix maps and return a new map.
-        
+
         Note:
-            Either ``healpix1`` *or* ``healpix2`` can be a non-GbmHealPix 
-            object, however at least one of them must be a GbmHealPix object 
-            **and** the ``primary`` argument must be set to the appropriate 
+            Either ``healpix1`` *or* ``healpix2`` can be a non-GbmHealPix
+            object, however at least one of them must be a GbmHealPix object
+            **and** the ``primary`` argument must be set to the appropriate
             GbmHealPix object otherwise a TypeError will be raised.
 
         Args:
-            healpix1 (:class:`~.gdt.core.healpix.HealPix` or :class:`GbmHealPix`): 
+            healpix1 (:class:`~.gdt.core.healpix.HealPix` or :class:`GbmHealPix`):
                 One of the HEALPix maps to multiply
-            healpix2 (:class:`~.gdt.core.healpix.HealPix` or :class:`GbmHealPix`): 
+            healpix2 (:class:`~.gdt.core.healpix.HealPix` or :class:`GbmHealPix`):
                 The other HEALPix map to multiply
-            primary (int, optional): If 0, use the first map header information, 
-                                     or if 1, use the second map header 
+            primary (int, optional): If 0, use the first map header information,
+                                     or if 1, use the second map header
                                      information. Default is 1.
-            output_nside (int, optional): The nside of the multiplied map. 
+            output_nside (int, optional): The nside of the multiplied map.
                                           Default is 128.
         Returns
             :class:`GbmHealPix`: The multiplied map
         """
 
         if primary == 0:
             if not isinstance(healpix1, cls):
-                 raise TypeError('Primary HealPix (healpix1) is not of class {}. '
-                'Perhaps try setting healpix2 as the primary'.format(cls.__name__))
+                raise TypeError('Primary HealPix (healpix1) is not of class {}. '
+                                'Perhaps try setting healpix2 as the primary'.format(cls.__name__))
         else:
             if not isinstance(healpix2, cls):
                 raise TypeError('Primary HealPix (healpix2) is not of class {}. '
-                'Perhaps try setting healpix1 as the primary'.format(cls.__name__))
+                                'Perhaps try setting healpix1 as the primary'.format(cls.__name__))
 
         if primary == 0:
             headers = healpix1.headers
+            quat = healpix1.quaternion
+            scpos = healpix1.scpos
         else:
             headers = healpix2.headers
+            quat = healpix2.quaternion
+            scpos = healpix2.scpos
 
-        obj = super().multiply(healpix1, healpix2, primary=primary, 
-                               output_nside=output_nside)   
+        obj = super().multiply(healpix1, healpix2, primary=primary,
+                               output_nside=output_nside, quaternion=quat,
+                               scpos=scpos)
 
-        return obj 
+        return obj
 
     def observable_fraction(self, healpix):
-        """The observable fraction of a healpix probability region on the sky. 
+        """The observable fraction of a healpix probability region on the sky.
         Non-observable regions are ones that are behind the Earth.
-        
+
         Args:
-            healpix (:class:`HealPix`): The healpix region for which to 
+            healpix (:class:`HealPix`): The healpix region for which to
                                         calculate the observable fraction.
-        Returns:        
+        Returns:
             (float)
         """
         if self.geo_location is None:
             raise RuntimeError('Location of geocenter is not known')
-        
+
         # speed things up a bit by only considering pixels with non-zero prob
         prob_mask = (healpix.prob > 0.0)
         # get ra, dec coords for pixels and calculate angle from geocenter
         theta, phi = hp.pix2ang(healpix.nside, np.arange(healpix.npix))
         ra = self._phi_to_ra(phi)[prob_mask]
         dec = self._theta_to_dec(theta)[prob_mask]
         pts = SkyCoord(ra, dec, frame='icrs', unit='deg')
@@ -316,112 +340,114 @@
         temp = temp[prob_mask]
         frac = temp[geo_mask].sum() / healpix.prob.sum()
         return frac
 
     @classmethod
     def open(cls, file_path, **kwargs):
         """Open a GBM HEALPix FITS file and return the GbmHealPix object
-        
+
         Args:
             file_path (str): The file path of the FITS file
-        
-        Returns:        
+
+        Returns:
             (:class:`GbmHealPix`)
         """
         # ignore comment length warnings
-        warnings.filterwarnings("ignore", category=UserWarning)
-        
-        obj = super().open(file_path, **kwargs)
+        with warnings.catch_warnings():
+            warnings.filterwarnings("ignore", category=UserWarning)
+            obj = super().open(file_path, **kwargs)
 
         # get the headers
         hdrs = [hdu.header for hdu in obj.hdulist]
 
         # some older files do not have these keywords
         if 'GEO_RAD' not in hdrs[1]:
             hdrs[1]['GEO_RAD'] = 67.5
         if 'COMMENT' not in hdrs[1]:
             hdrs[1]['COMMENT'] = ''
             hdrs[1]['COMMENT'] = ''
         headers = HealpixHeaders.from_headers(hdrs)
-   
+
         trigtime = headers['PRIMARY']['TRIGTIME']
-            
+
         # quaternion and scpos are stored as comments
         try:
             headers[1]['COMMENT'][0] = obj.hdulist[1].header['COMMENT'][0]
             headers[1]['COMMENT'][1] = obj.hdulist[1].header['COMMENT'][1]
         except:
             headers[1]['COMMENT'][0] = ''
             headers[1]['COMMENT'][1] = ''
-        
+
         try:
             scpos_comment = headers[1]['COMMENT'][0]
             scpos = scpos_comment.split('[')[1].split(']')[0]
             scpos = np.array([float(el) for el in scpos.split()])
+            scpos = CartesianRepresentation(scpos, unit='m')
         except:
             scpos = None
         try:
             quat_comment = headers[1]['COMMENT'][1]
             quat = quat_comment.split('[')[1].split(']')[0]
             quat = np.array([float(el) for el in quat.split()])
+            quat = Quaternion(quat)
         except:
             quat = None
-        
+
         # get the probability and significance arrays
         prob = obj.column(1, 'PROBABILITY').flatten()
         sig = obj.column(1, 'SIGNIFICANCE').flatten()
         if headers[1]['ORDERING'] == 'NESTED':
             npix = prob.size
             idx = hp.ring2nest(hp.npix2nside(npix), np.arange(npix))
             prob = prob[idx]
             sig = sig[idx]
-        
+
         obj.close()
-        
+
         obj = cls.from_data(prob, trigtime=trigtime, quaternion=quat,
                             scpos=scpos, filename=obj.filename,
                             headers=headers)
         obj._sig = sig
-        
+
         return obj
-        
+
     def region_probability(self, healpix, prior=0.5):
         r"""The probability that the localization is associated with
-        the localization region from another map.  This is calculated 
-        against the null hypothesis that the two maps represent 
+        the localization region from another map.  This is calculated
+        against the null hypothesis that the two maps represent
         unassociated sources:
-        
-        :math:`P(A | \mathcal{I}) = 
+
+        :math:`P(A | \mathcal{I}) =
         \frac{P(\mathcal{I} | A) \ P(A)}
         {P(\mathcal{I} | A) \ P(A) + P(\mathcal{I} | \neg A) \ P(\neg A)}`
-        
+
         where
-        
-        * :math:`P(\mathcal{I} | A)` is the integral over the overlap of the two 
+
+        * :math:`P(\mathcal{I} | A)` is the integral over the overlap of the two
           maps once the Earth occultation has been removed for *this* map.
         * :math:`P(\mathcal{I} | \neg A)` is the integral over the overlap of
-          *this* map with a uniform distribution on the sky (i.e. the probability 
+          *this* map with a uniform distribution on the sky (i.e. the probability
           the localization is associated with a random point on the sky)
-        * :math:`P(A)` is the prior probability that *this* localization is 
+        * :math:`P(A)` is the prior probability that *this* localization is
           associated with the *other* HEALPix map.
 
-        Note: 
+        Note:
             The localization region of *this* map overlapping the Earth will be
             removed and the remaining unocculted region is used for the
             calculation.  The *other* map is assumed to have no exclusionary
             region.
-        
+
         Args:
-            healpix (:class:`~gdt.core.healpix.HealPixLocalization`): 
+            healpix (:class:`~gdt.core.healpix.HealPixLocalization`):
                 The healpix map for which to calculate the spatial association.
             prior (float, optional): The prior probability that the localization
-                                     is associated with the source. Default is 
+                                     is associated with the source. Default is
                                      0.5.
-        
-        Returns:  
+
+        Returns:
             (float)
         """
         if (prior < 0.0) or (prior > 1.0):
             raise ValueError('Prior probability must be within 0-1, inclusive')
 
         # convert uniform prob/sr to prob/pixel
         u = 1.0 / (4.0 * np.pi)
@@ -434,15 +460,15 @@
             geo_mask = np.zeros_like(self.prob, dtype=bool)
         probmap1 = np.copy(self.prob)
         temp = probmap1[prob_mask]
         temp[geo_mask] = 0.0
         probmap1[prob_mask] = temp
         probmap1 = self._assert_prob(probmap1)
 
-        # ensure maps are the same resolution and convert uniform prob/sr to 
+        # ensure maps are the same resolution and convert uniform prob/sr to
         # prob/pixel
         probmap2 = np.copy(healpix.prob)
         if self.nside > healpix.nside:
             probmap2 = hp.ud_grade(probmap2, nside_out=self.nside)
             probmap2 = self._assert_prob(probmap2)
             u *= hp.nside2resol(self.nside) ** 2
         elif self.nside < healpix.nside:
@@ -456,27 +482,27 @@
         alt_hyp = np.sum(probmap1 * probmap2)
         # null hypothesis: one of the maps is from an unassociated source
         # (uniform spatial probability)
         null_hyp = np.sum(probmap1 * u)
 
         # since we have an exhaustive and complete list of possibilities, we can
         # easily calculate the probability
-        prob = (alt_hyp * prior) / ((alt_hyp*prior) + (null_hyp*(1.0-prior)))
+        prob = (alt_hyp * prior) / ((alt_hyp * prior) + (null_hyp * (1.0 - prior)))
         return prob
 
     def remove_earth(self):
         """Return a new GbmHealPix with the probability on the Earth masked out.
         The remaining probability on the sky is renormalized.
 
         Note:
-            The :attr:`geo_location` attribute must be available to use this 
+            The :attr:`geo_location` attribute must be available to use this
             function.
 
-        
-        Returns: 
+
+        Returns:
             (:class:`GbmHealPix`)
         """
         if self.geo_location is None:
             raise RuntimeError('Location of geocenter is not known')
 
         # get the non-zero probability and earth masks
         prob_mask, geo_mask = self._earth_mask()
@@ -484,165 +510,206 @@
         # zero out the probabilities behind the earth
         new_prob = np.copy(self.prob)
         temp = new_prob[prob_mask]
         temp[geo_mask] = 0.0
         new_prob[prob_mask] = temp
         # renormalize
         new_prob = self._assert_prob(new_prob)
-        obj = type(self).from_data(new_prob, trigtime=self.trigtime, 
+        obj = type(self).from_data(new_prob, trigtime=self.trigtime,
                                    headers=self.headers, scpos=self.scpos,
-                                   filename=self.filename, 
+                                   filename=self.filename,
                                    quaternion=self.quaternion)
         return obj
 
     def source_probability(self, ra, dec, prior=0.5):
         r"""The probability that the GbmHealPix localization is associated with
         a known point location.  This is calculated against the null hypothesis
-        that the localization originates from an unassociated random source 
-        that has equal probability of origination anywhere in the sky: 
-        
-        :math:`P(A | \mathcal{I}) = 
+        that the localization originates from an unassociated random source
+        that has equal probability of origination anywhere in the sky:
+
+        :math:`P(A | \mathcal{I}) =
         \frac{P(\mathcal{I} | A) \ P(A)}
         {P(\mathcal{I} | A) \ P(A) + P(\mathcal{I} | \neg A) \ P(\neg A)}`
-        
+
         where
-        
+
         * :math:`P(\mathcal{I} | A)` is the probability of the localization at
           the point source once the Earth occultation has been removed
-        * :math:`P(\mathcal{I} | \neg A)` is the probability per pixel assuming 
-          a uniform distribution on the sky (i.e. the probability the 
+        * :math:`P(\mathcal{I} | \neg A)` is the probability per pixel assuming
+          a uniform distribution on the sky (i.e. the probability the
           localization is associated with a random point on the sky)
-        * :math:`P(A)` is the prior probability that the localization is 
+        * :math:`P(A)` is the prior probability that the localization is
           associated with the point source
-        
-        Note: 
+
+        Note:
             If the point source is behind the Earth, then it is assumed that
-            GBM could not observe it, therefore the probability will be zero. 
-        
+            GBM could not observe it, therefore the probability will be zero.
+
         Args:
             ra (float): The RA of the known source location
             dec (float): The Dec of the known source location
             prior (float, optional): The prior probability that the localization
-                                     is associated with the source. Default is 
+                                     is associated with the source. Default is
                                      0.5.
-        
-        Returns:        
+
+        Returns:
             (float)
         """
         if (prior < 0.0) or (prior > 1.0):
             raise ValueError('Prior probability must be within 0-1, inclusive')
-        
+
         # convert uniform prob/sr to prob/pixel
         u = 1.0 / (4.0 * np.pi)
         u *= hp.nside2resol(self.nside) ** 2
 
         # the pixel probability of the skymap at the location of the point source
         try:
             p = self.remove_earth().probability(ra, dec, per_pixel=True)
         except:
             p = self.probability(ra, dec, per_pixel=True)
-        
+
         # if we know the location of the earth and it's behind the earth,
         # then we obviously couldn't have seen it
         if self.geo_location is not None:
             pt = SkyCoord(ra, dec, frame='icrs', unit='deg')
             ang = self.geo_location.separation(pt)
             if ang < self.geo_radius:
                 p = 0.0
 
         # null hypothesis is that they are not associated, therefore the sky map
         # is result of some source that has uniform probability on the sky
-        prob = (p*prior) / ((p*prior) + (u*(1.0-prior)))
+        prob = (p * prior) / ((p * prior) + (u * (1.0 - prior)))
         return prob
 
     def _build_hdulist(self):
 
         # create FITS and primary header
         hdulist = fits.HDUList()
         primary_hdu = fits.PrimaryHDU(header=self.headers['PRIMARY'])
         for key, val in self.headers['PRIMARY'].items():
             primary_hdu.header[key] = val
         hdulist.append(primary_hdu)
-        
+
         # the healpix extension
         prob_arr = hp.reorder(self.prob, r2n=True).reshape(-1, 1024)
-        prob_col = fits.Column(name='PROBABILITY', format='1024E', 
+        prob_col = fits.Column(name='PROBABILITY', format='1024E',
                                array=prob_arr)
         sig_arr = hp.reorder(self.sig, r2n=True).reshape(-1, 1024)
-        sig_col = fits.Column(name='SIGNIFICANCE', format='1024E', 
+        sig_col = fits.Column(name='SIGNIFICANCE', format='1024E',
                               array=sig_arr)
         hpx_hdu = fits.BinTableHDU.from_columns([prob_col, sig_col],
                                                 header=self.headers['HEALPIX'])
         cflag = 0
         for key, val in self.headers['HEALPIX'].items():
             if key == 'COMMENT':
                 hpx_hdu.header['COMMENT'][cflag] = val
                 cflag += 1
                 continue
             hpx_hdu.header[key] = val
         hdulist.append(hpx_hdu)
-        hpx_hdu.header.comments['TTYPE1'] = 'Differential probability per pixel' 
-        hpx_hdu.header.comments['TTYPE2'] = 'Integrated probability' 
-        
+        hpx_hdu.header.comments['TTYPE1'] = 'Differential probability per pixel'
+        hpx_hdu.header.comments['TTYPE2'] = 'Integrated probability'
+
         return hdulist
 
     def _build_headers(self, trigtime, nside):
-        
+
         headers = self.headers.copy()
         headers['PRIMARY']['TRIGTIME'] = trigtime
         headers['HEALPIX']['NSIDE'] = nside
         headers['HEALPIX']['LASTPIX'] = hp.nside2npix(nside)
         headers['HEALPIX']['OBJECT'] = 'FULLSKY'
-        
+
         if self.trigtime is not None:
             headers['HEALPIX']['SUN_RA'] = self.sun_location.ra.value
             headers['HEALPIX']['SUN_DEC'] = self.sun_location.dec.value
 
         if self.scpos is not None:
             headers['HEALPIX']['COMMENT'][0] = 'SCPOS: ' + \
-                                               np.array2string(self.scpos)
-            headers['HEALPIX']['GEO_RA'] = self.geo_location.ra.value          
-            headers['HEALPIX']['GEO_DEC'] = self.geo_location.dec.value          
-            headers['HEALPIX']['GEO_RAD'] = self.geo_radius.value         
+                                               np.array2string(self.scpos.xyz.value)
+            headers['HEALPIX']['GEO_RA'] = self.geo_location.ra.value
+            headers['HEALPIX']['GEO_DEC'] = self.geo_location.dec.value
+            headers['HEALPIX']['GEO_RAD'] = self.geo_radius.value
 
         if self.quaternion is not None:
-            headers['HEALPIX']['COMMENT'][1] = 'QUAT: ' + \
-                                               np.array2string(self.quaternion)       
+            quat = np.append(self.quaternion.xyz, self.quaternion.w)
+            headers['HEALPIX']['COMMENT'][1] = 'QUAT: ' + np.array2string(quat)
             for det in GbmDetectors:
-                pointing = getattr(self, det.name.lower()+'_pointing')
-                headers['HEALPIX'][det.name.upper()+'_RA'] = pointing.ra.value
-                headers['HEALPIX'][det.name.upper()+'_DEC'] = pointing.dec.value
-                        
+                pointing = getattr(self, det.name.lower() + '_pointing')
+                headers['HEALPIX'][det.name.upper() + '_RA'] = pointing.ra.value
+                headers['HEALPIX'][det.name.upper() + '_DEC'] = pointing.dec.value
+
         return headers
-        
+
     def _earth_mask(self):
         # speed things up a bit by only considering pixels with non-zero prob
         mask = (self.prob > 0.0)
         # get ra, dec coords for pixels and calculate angle from geocenter
         theta, phi = hp.pix2ang(self.nside, np.arange(self.npix))
-        pts = SkyCoord(self._phi_to_ra(phi)[mask], 
-                       self._theta_to_dec(theta)[mask], frame='icrs', 
+        pts = SkyCoord(self._phi_to_ra(phi)[mask],
+                       self._theta_to_dec(theta)[mask], frame='icrs',
                        unit='deg')
         ang = self.geo_location.separation(pts)
 
         # the mask of the non-zero probability pixels that are behind the earth
         geo_mask = (ang <= self.geo_radius)
 
         return mask, geo_mask
 
+    @staticmethod
+    def _none_default_headers():
+        hdr = HealpixHeaders()
+        hdr[0]['TRIGTIME'] = None
+        hdr[1]['SUN_RA'] = None
+        hdr[1]['SUN_DEC'] = None
+        hdr[1]['GEO_RA'] = None
+        hdr[1]['GEO_DEC'] = None
+        hdr[1]['GEO_RAD'] = None
+        hdr[1]['N0_RA'] = None
+        hdr[1]['N0_DEC'] = None
+        hdr[1]['N1_RA'] = None
+        hdr[1]['N1_DEC'] = None
+        hdr[1]['N2_RA'] = None
+        hdr[1]['N2_DEC'] = None
+        hdr[1]['N3_RA'] = None
+        hdr[1]['N3_DEC'] = None
+        hdr[1]['N4_RA'] = None
+        hdr[1]['N4_DEC'] = None
+        hdr[1]['N5_RA'] = None
+        hdr[1]['N5_DEC'] = None
+        hdr[1]['N6_RA'] = None
+        hdr[1]['N6_DEC'] = None
+        hdr[1]['N7_RA'] = None
+        hdr[1]['N7_DEC'] = None
+        hdr[1]['N8_RA'] = None
+        hdr[1]['N8_DEC'] = None
+        hdr[1]['N9_RA'] = None
+        hdr[1]['N9_DEC'] = None
+        hdr[1]['NA_RA'] = None
+        hdr[1]['NA_DEC'] = None
+        hdr[1]['NB_RA'] = None
+        hdr[1]['NB_DEC'] = None
+        hdr[1]['B0_RA'] = None
+        hdr[1]['B0_DEC'] = None
+        hdr[1]['B1_RA'] = None
+        hdr[1]['B1_DEC'] = None
+
+        return hdr
+
     def __repr__(self):
         s = '<{0}: {1}\n'.format(self.__class__.__name__, self.filename)
         s += ' NSIDE={0}; trigtime={1};\n'.format(self.nside, self.trigtime)
         s += ' centroid={}>'.format(self.centroid)
         return s
 
 
 class Chi2Grid():
     """Class for the GBM legacy internal Chi2Grid localization files/objects.
     """
+
     def __init__(self):
         self._az = np.array([])
         self._zen = np.array([])
         self._ra = np.array([])
         self._dec = np.array([])
         self._chisq = np.array([])
         self._quaternion = None
@@ -669,14 +736,15 @@
         """(int): Number of sky points in the Chi2Grid"""
         return self._az.size
 
     @property
     def quaternion(self):
         """(np.array): The spacecraft attitude quaternion"""
         return self._quaternion
+
     @quaternion.setter
     def quaternion(self, val):
         if len(val) != 4:
             raise ValueError('quaternion must be a 4-element array')
         self._quaternion = np.asarray(val)
 
     @property
@@ -684,14 +752,15 @@
         """(np.array): The RA grid points"""
         return self._ra
 
     @property
     def scpos(self):
         """(np.array): The spacecraft position in Earth inertial coordinates"""
         return self._scpos
+
     @scpos.setter
     def scpos(self, val):
         if len(val) != 3:
             raise ValueError('scpos must be a 3-element array')
         self._scpos = np.asarray(val)
 
     @property
@@ -700,14 +769,15 @@
         min_chisq = np.min(self.chisq)
         return 1.0 - chi2.cdf(self.chisq - min_chisq, 2)
 
     @property
     def trigtime(self):
         """(float): The trigger time"""
         return self._trigtime
+
     @trigtime.setter
     def trigtime(self, val):
         try:
             val = float(val)
         except:
             raise ValueError('trigtime must be a float')
         self._trigtime = val
@@ -716,19 +786,19 @@
     def zenith(self):
         """(np.array): The spacecraft zenith grid points"""
         return self._zen
 
     @classmethod
     def open(cls, filename):
         """Read a chi2grid file and create a Chi2Grid object
-        
+
         Args:
             filename (str): The filename of the chi2grid file
-        
-        Returns:        
+
+        Returns:
            :class:`Chi2Grid`: The Chi2Grid object
         """
         with open(filename, 'r') as f:
             txt = list(f)
 
         obj = cls()
 
@@ -748,84 +818,84 @@
             obj._dec[i] = float(line[5].strip())
 
         return obj
 
     @classmethod
     def from_data(cls, az, zen, ra, dec, chisq):
         """Create a Chi2Grid object from arrays
-        
+
         Args:
             az (np.array): The azimuth grid points
             zen (np.array): The zenith grid points
             ra (np.array): The RA grid points
             dec (np.array): The Dec grid points
             chisq (np.array): The chi-squared values at each grid point
-        
-        Returns:        
+
+        Returns:
             :class:`Chi2Grid`: The Chi2Grid object
         """
         az = np.asarray(az, dtype=float).flatten()
         zen = np.asarray(zen, dtype=float).flatten()
         ra = np.asarray(ra, dtype=float).flatten()
         dec = np.asarray(dec, dtype=float).flatten()
         chisq = np.asarray(chisq, dtype=float).flatten()
-        
+
         numpts = az.size
         if (zen.size != numpts) or (ra.size != numpts) or (dec.size != numpts) \
-           or (chisq.size != numpts):
+                or (chisq.size != numpts):
             raise ValueError('All inputs must have same size')
-        
+
         obj = cls()
         obj._az = az
         obj._zen = zen
         obj._ra = ra
         obj._dec = dec
         obj._chisq = chisq
         return obj
 
 
 # Systematic Model definitions using healpy.smoothing
 # --------------------------------------------------------
 def ga_model():
     """The localization systematic model for the Ground-Automated localization:
     A mixture of a 3.72 deg Gaussian (80.4% weight) and a 13.7 deg Gaussian.
-    
+
     References:
-        `Connaughton, V. et al. 2015, ApJ, 216, 32 
+        `Connaughton, V. et al. 2015, ApJ, 216, 32
         <https://iopscience.iop.org/article/10.1088/0067-0049/216/2/32>`_
     """
     sigma1 = np.deg2rad(3.72)
     sigma2 = np.deg2rad(13.7)
     frac1 = 0.804
     return ([sigma1, sigma2], [frac1])
 
 
 def gbuts_o3_model():
     """The localization systematic model for the targeted search during O3:
     a 2.7 deg Gaussian.
-    
+
     References:
-        `Goldstein, A. et al. 2019, arXiv: 1903.12597 
+        `Goldstein, A. et al. 2019, arXiv: 1903.12597
         <https://arxiv.org/abs/1903.12597>`_
     """
     sigma = np.deg2rad(2.7)
     return ([sigma], [1.0])
 
 
 def hitl_model(az):
     """The localization systematic model for the human-in-the loop localization:
     A mixture of a 4.17 deg Gaussian (91.8% weight) and a 15.3 deg Gaussian
-    for a centroid between azimuth 292.5 - 67.5 or azimuth 112.5 - 247.5, 
-    otherwise a mixture of a 2.31 deg Gaussian (88.4% weight) and a 
+    for a centroid between azimuth 292.5 - 67.5 or azimuth 112.5 - 247.5,
+    otherwise a mixture of a 2.31 deg Gaussian (88.4% weight) and a
     13.2 deg Gaussian.
-    
+
     References:
-        `Connaughton, V. et al. 2015, ApJ, 216, 32 
+        `Connaughton, V. et al. 2015, ApJ, 216, 32
         <https://iopscience.iop.org/article/10.1088/0067-0049/216/2/32>`_
-    
+
     Args:
         az (float): The localization centroid in spacecraft azimuth
     """
     if (az > 292.5) or (az <= 67.5) or ((az > 112.5) and (az < 247.5)):
         sigma1 = np.deg2rad(4.17)
         sigma2 = np.deg2rad(15.3)
         frac1 = 0.918
@@ -835,21 +905,21 @@
         frac1 = 0.884
     return ([sigma1, sigma2], [frac1])
 
 
 def robo_ba_model(grb_type):
     """The localization systematic model for the RoboBA localization:
     A mixture of a 1.86 deg Gaussian (57.9% weight) and a 4.14 deg Gaussian
-    for a "long" GRB, and a mixture of a 2.55 deg Gaussian (39.0% weight) and a 
+    for a "long" GRB, and a mixture of a 2.55 deg Gaussian (39.0% weight) and a
     4.43 deg Gaussian for a "short" GRB.
-    
+
     References:
-        `Goldstein, A. et al. 2020, ApJ, 895, 40 
+        `Goldstein, A. et al. 2020, ApJ, 895, 40
         <https://iopscience.iop.org/article/10.3847/1538-4357/ab8bdb>`_
-    
+
     Args:
         grb_type (str): The type of GRB, either 'long' or 'short'
     """
     if grb_type == 'long':
         sigma1 = np.deg2rad(1.86)
         sigma2 = np.deg2rad(4.14)
         frac1 = 0.579
```

### Comparing `astro-gdt-fermi-2.0.0/src/gdt/missions/fermi/gbm/phaii.py` & `astro_gdt_fermi-2.1.0/src/gdt/missions/fermi/gbm/phaii.py`

 * *Files identical despite different names*

### Comparing `astro-gdt-fermi-2.0.0/src/gdt/missions/fermi/gbm/poshist.py` & `astro_gdt_fermi-2.1.0/src/gdt/missions/fermi/gbm/poshist.py`

 * *Files identical despite different names*

### Comparing `astro-gdt-fermi-2.0.0/src/gdt/missions/fermi/gbm/response.py` & `astro_gdt_fermi-2.1.0/src/gdt/missions/fermi/gbm/response.py`

 * *Files identical despite different names*

### Comparing `astro-gdt-fermi-2.0.0/src/gdt/missions/fermi/gbm/saa.py` & `astro_gdt_fermi-2.1.0/src/gdt/missions/fermi/gbm/saa.py`

 * *Files identical despite different names*

### Comparing `astro-gdt-fermi-2.0.0/src/gdt/missions/fermi/gbm/scat.py` & `astro_gdt_fermi-2.1.0/src/gdt/missions/fermi/gbm/scat.py`

 * *Files identical despite different names*

### Comparing `astro-gdt-fermi-2.0.0/src/gdt/missions/fermi/gbm/tcat.py` & `astro_gdt_fermi-2.1.0/src/gdt/missions/fermi/gbm/tcat.py`

 * *Files identical despite different names*

### Comparing `astro-gdt-fermi-2.0.0/src/gdt/missions/fermi/gbm/trigdat.py` & `astro_gdt_fermi-2.1.0/src/gdt/missions/fermi/gbm/trigdat.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,18 +148,24 @@
 
         # get the headers
         hdrs = [hdu.header for hdu in obj.hdulist]
         obj._headers = TrigdatHeaders.from_headers(hdrs)
         obj._trigtime = obj._headers[0]['TRIGTIME']
         
         # store trigrate, maxrates, backrates, and fsw location
-        obj._trigrates = MaxRates.from_recarray(obj.hdulist['TRIGRATE'].data[0])
+        trigrate_data =  obj.hdulist['TRIGRATE'].data
+        if trigrate_data.size > 0:
+            obj._trigrates = MaxRates.from_recarray(trigrate_data[0])
         obj._maxrates = [MaxRates.from_recarray(maxrate) for maxrate in
                          obj.hdulist['MAXRATES'].data]
-        obj._backrates = BackRates.from_recarray(obj.hdulist['BCKRATES'].data[0])
+        
+        try:
+            obj._backrates = BackRates.from_recarray(obj.hdulist['BCKRATES'].data[0])
+        except:
+            warnings.warn('No BCKRATES data in this file.', RuntimeWarning)      
         obj._fsw_locations = [FswLocation.from_recarray(ob_calc) \
                               for ob_calc in obj.hdulist['OB_CALC'].data]
         
         # store the data            
         obj._data = obj.hdulist['EVNTRATE'].data
         obj._data.sort(order='TIME')
         # incorrectly shaped in the file, so we have to fix that here
@@ -681,28 +687,40 @@
         Args: 
             idx1 (np.array): Indices of the "bracketing" timescale
             idx2 (np.array): Indices of the "inserted" timescale 
         
         Returns:
             np.array: Indices of idx2 spliced into idx1
 		"""
+        # if there is no idx1, then we only have to return idx2 and v.v.
+        if idx1.size == 0:
+            return idx2
+        if idx2.size == 0:
+            return idx1
+
         # bin edges for both selections
         start_times1 = self._data['TIME'][idx1]
         end_times1 = self._data['ENDTIME'][idx1]
         start_times2 = self._data['TIME'][idx2]
         end_times2 = self._data['ENDTIME'][idx2]
 
         # find where bracketing timescale ends and inserted timescale begins
-        start_idx = (np.where(end_times1 >= start_times2[0]))[0][0]
-        idx = np.concatenate((idx1[0:start_idx], idx2))
-
-        # find wehere inserted timescale ends and bracketing timescale begins again
-        end_idx = (np.where(start_times1 >= end_times2[-1]))[0][0]
-        idx = np.concatenate((idx, idx1[end_idx:]))
+        mask = end_times1 >= start_times2[0]
+        if mask.sum():
+            start_idx = (np.where(mask))[0][0]
+            idx = np.concatenate((idx1[0:start_idx], idx2))
+        else:
+            idx = np.concatenate((idx1, idx2))
 
+        # find where inserted timescale ends and bracketing timescale begins again
+        mask = start_times1 >= end_times2[-1]
+        if mask.sum():
+            end_idx = (np.where(mask))[0][0]
+            idx = np.concatenate((idx, idx1[end_idx:]))
+                
         return idx
 
     def _gti_from_times(self, tstarts, tstops):
         """Estimate the GTI from the bin start and stop times.
         This may return multiple GTIs if several background packets are missing
 		
 		Args:
@@ -1242,16 +1260,22 @@
         obj._class2 = (classifications[rec_array['EVTCLASS'][1]],
                         rec_array['RELIABLT'][1])
         obj._intensity = rec_array['INTNSITY']
         obj._hardness = rec_array['HDRATIO']
         obj._fluence = rec_array['FLUENCE']
         obj._sigma = rec_array['SIGMA']
         obj._rates = rec_array['LOCRATES']
-        obj._timescale = rec_array['TRIG_TS']
-        obj._azzen = (rec_array['TR_SCAZ'], rec_array['TR_SCZEN'])
+        try:
+            obj._timescale = rec_array['TRIG_TS']
+        except KeyError:
+            pass
+        try:
+            obj._azzen = (rec_array['TR_SCAZ'], rec_array['TR_SCZEN'])
+        except KeyError:
+            pass
         return obj
     
     def to_recarray(self):
         """Convert contents of the object to a numpy record array
         
         Returns:
             (np.recarray)
```

### Comparing `astro-gdt-fermi-2.0.0/src/gdt/missions/fermi/gbm/tte.py` & `astro_gdt_fermi-2.1.0/src/gdt/missions/fermi/gbm/tte.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,21 +47,37 @@
     def detector(self):
         """(str): The detector name"""
         try:
             return GbmDetectors.from_full_name(self.headers[0]['DETNAM']).name
         except:
             return self.headers[0]['DETNAM']
 
-    # mark TODO: copy over relevant header keywords
     def to_phaii(self, bin_method, *args, time_range=None, energy_range=None,
                  channel_range=None, **kwargs):
         if self.trigtime is not None:
             headers = PhaiiTriggerHeaders()
         else:
             headers = PhaiiHeaders()
+        
+        # do not copy the value of these keys
+        exceptions = ['CREATOR', 'DATATYPE', 'EXTNAME', 'FILENAME', 'FILETYPE',
+                      'HDUCLAS1']
+        # copy over the key values for each header
+        for i in range(self.headers.num_headers):
+            for key, val in self.headers[i].items():
+                if key in exceptions:
+                    continue
+                try:
+                    headers[i][key] = val        
+                except:
+                    # header key is present in TTE but not in PHAII
+                    pass
+        headers['PRIMARY']['FILETYPE'] = 'PHAII'
+        headers['PRIMARY']['DATATYPE'] = 'PHAII'
+        
         return super().to_phaii(bin_method, *args, time_range=time_range, 
                                 energy_range=energy_range, 
                                 channel_range=channel_range, 
                                 phaii_class=GbmPhaii, headers=headers, **kwargs)
     @classmethod
     def open(cls, file_path, **kwargs):
         """Open a TTE FITS file and return the TTE object
```

### Comparing `astro-gdt-fermi-2.0.0/src/gdt/missions/fermi/mcilwainl.py` & `astro_gdt_fermi-2.1.0/src/gdt/missions/fermi/mcilwainl.py`

 * *Files identical despite different names*

### Comparing `astro-gdt-fermi-2.0.0/src/gdt/missions/fermi/plot.py` & `astro_gdt_fermi-2.1.0/src/gdt/missions/fermi/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -340,10 +340,12 @@
     
     def standard_title(self):
         """Add a standard plot title containing orbital position and McIlwain L
         """
         if self.spacecraft is not None:
             coord = self.spacecraft.coordinates
             title = 'Latitude, East Longitude: ({0}, {1})\n'.format(*coord)
-            mcl = calc_mcilwain_l(float(coord[0][:-1]), float(coord[1][:-1]))
+            lat = float(coord[0][:-1]) * (-1 if "S" in coord[0] else 1)
+            lon = float(coord[1][:-1]) * (-1 if "W" in coord[1] else 1)
+            mcl = calc_mcilwain_l(lat, lon)
             title += 'McIlwain L: {:.2f}'.format(mcl)
             self._m.set_title(title)
```

### Comparing `astro-gdt-fermi-2.0.0/src/gdt/missions/fermi/time.py` & `astro_gdt_fermi-2.1.0/src/gdt/missions/fermi/time.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,69 +33,70 @@
 import erfa
 import numpy as np
 from astropy.time import TimeFromEpoch, TimeUnique, ScaleValueError, Time
 from astropy.time.utils import day_frac
 
 __all__ = ['FermiSecTime', 'GbmBurstNumber', 'Time']
 
+
 class FermiSecTime(TimeFromEpoch):
     """Represents the number of seconds elapsed since Jan 1, 2001, 00:00:00 UTC,
     including leap seconds
     """
     name = 'fermi'
     """(str): Name of the mission"""
-    
-    unit = 1.0 / 86400 
+
+    unit = 1.0 / 86400
     """(float): unit in days"""
-    
+
     epoch_val = '2001-01-01 00:01:04.184'
     """(str): The epoch in Terrestrial Time"""
-    
+
     epoch_val2 = None
-    
+
     epoch_scale = 'tt'
     """(str): The scale of :attr:`epoch_val`"""
-    
+
     epoch_format = 'iso'
     """(str): Format of :attr:`epoch_val`"""
 
 
 class GbmBurstNumber(TimeUnique):
     """Represent date as Fermi GBM burst number"""
-    
+
     name = 'gbm_bn'
     """(str): The name of the time format"""
-    
-    bn_pattern = re.compile(r'^(?P<year>\d\d)(?P<month>\d\d)(?P<day>\d\d)(?P<frac>\d\d\d)$', re.I | re.S)
 
-    second_corrections = [
+    _bn_pattern = re.compile(r'^(?P<year>\d\d)(?P<month>\d\d)(?P<day>\d\d)(?P<frac>\d\d\d)$', re.I | re.S)
+
+    _second_corrections = [
         # 2008-01-01 00:00:00.000 UTC < x < 2009-01-01 00:00:00.000 UTC adjust seconds by 1
         (datetime.datetime(2008, 1, 1), datetime.datetime(2009, 1, 1), 1),
         # 2009-01-01 00:00:00.000 UTC < met <= 2009-01-13 00:00:00.000 UTC adjust seconds by 2
         (datetime.datetime(2009, 1, 1), datetime.datetime(2009, 1, 13), 2)
     ]
 
     def _check_val_type(self, val1, val2):
-        if not all(self.bn_pattern.match(val) is not None for val in val1.flat):
+        if not all(self._bn_pattern.match(val) is not None for val in val1.flat):
             raise TypeError('Input values for {} class must be '
                             'burst numbers'.format(self.name))
         if val2 is not None:
             raise ValueError(
                 f'{self.name} objects do not accept a val2 but you provided {val2}')
         return val1, None
 
     def set_jds(self, val1, val2):
-        """Convert burst numbers contained in val1 to jd1, jd2"""
+        """Convert burst number contained in val1 to jd1, jd2"""
         # Iterate through the datetime objects, getting year, month, etc.
         iterator = np.nditer([val1, None, None, None, None, None, None],
                              flags=['refs_ok', 'zerosize_ok'],
                              op_dtypes=[None] + 5 * [np.intc] + [np.double])
 
         for val, iy, im, iday, ihr, imin, dsec in iterator:
-            m = self.bn_pattern.match(str(val))
+            m = self._bn_pattern.match(str(val))
             if not m:
                 raise ValueError('burst number was not the correct format.')
 
             bn = m.groupdict()
             iy[...] = int(bn['year']) + 2000
             im[...] = int(bn['month'])
             iday[...] = int(bn['day'])
@@ -108,15 +109,15 @@
             dsec[...] = secs_of_day % 60
 
         jd1, jd2 = erfa.dtf2d(self.scale.upper().encode('ascii'),
                               *iterator.operands[1:])
         self.jd1, self.jd2 = day_frac(jd1, jd2)
 
     def to_value(self, parent=None, out_subfmt=None):
-        """Convert to burst number"""
+        """Convert to string representation of GBM burst number"""
         if out_subfmt is not None:
             # Out_subfmt not allowed for this format, so raise the standard
             # exception by trying to validate the value.
             self._select_subfmts(out_subfmt)
 
         # GBM Burst Numbers are in the UTC scale, so make sure that we use UTC
         if self.scale != 'utc':
@@ -146,17 +147,17 @@
                              op_dtypes=7 * [None] + [object])
 
         for iy, im, iday, ihr, imin, isec, ifracsec, out in iterator:
             day_secs = ihr * 3600 + imin * 60 + isec
 
             # Adjust results to match the burst numbers issued early in the mission
             dt = datetime.datetime(iy, im, iday, ihr, imin, isec)
-            for beg_dt, end_dt, adj_secs in self.second_corrections:
+            for beg_dt, end_dt, adj_secs in self._second_corrections:
                 if beg_dt < dt <= end_dt:
                     # print(f'{beg_dt} < {dt} <= {end_dt}')
                     day_secs += adj_secs
             frac = min(int(round(day_secs / 86400 * 1000)), 999)
             out[...] = f'{iy - 2000:02d}{im:02d}{iday:02d}{frac:03d}'
 
-        return self.mask_if_needed(iterator.operands[-1])
+        return iterator.operands[-1]
 
     value = property(to_value)
```

