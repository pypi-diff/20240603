# Comparing `tmp/jord-0.6.1.tar.gz` & `tmp/jord-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jord-0.6.1.tar", last modified: Fri May  3 12:20:07 2024, max compression
+gzip compressed data, was "jord-0.6.2.tar", last modified: Mon Jun  3 12:14:21 2024, max compression
```

## Comparing `jord-0.6.1.tar` & `jord-0.6.2.tar`

### file list

```diff
@@ -1,163 +1,163 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:20:07.911470 jord-0.6.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:20:07.883470 jord-0.6.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-05-03 12:20:03.000000 jord-0.6.1/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-03 12:20:03.000000 jord-0.6.1/.github/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-03 12:20:03.000000 jord-0.6.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 12:20:03.000000 jord-0.6.1/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:20:07.903470 jord-0.6.1/Jord.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7059 2024-05-03 12:20:07.000000 jord-0.6.1/Jord.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-05-03 12:20:07.000000 jord-0.6.1/Jord.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 12:20:07.000000 jord-0.6.1/Jord.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-03 12:20:07.000000 jord-0.6.1/Jord.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-03 12:20:07.000000 jord-0.6.1/Jord.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-03 12:20:03.000000 jord-0.6.1/KEYWORDS.md
--rw-r--r--   0 runner    (1001) docker     (127)    10646 2024-05-03 12:20:03.000000 jord-0.6.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-03 12:20:03.000000 jord-0.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7059 2024-05-03 12:20:07.911470 jord-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-03 12:20:03.000000 jord-0.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-03 12:20:03.000000 jord-0.6.1/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:20:07.883470 jord-0.6.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-03 12:20:03.000000 jord-0.6.1/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:20:07.883470 jord-0.6.1/jord/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-03 12:20:04.000000 jord-0.6.1/jord/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     1484 2024-05-03 12:20:04.000000 jord-0.6.1/jord/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:20:07.883470 jord-0.6.1/jord/fiona_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 12:20:04.000000 jord-0.6.1/jord/fiona_utilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      749 2024-05-03 12:20:04.000000 jord-0.6.1/jord/fiona_utilities/deserialise.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:20:07.887470 jord-0.6.1/jord/gdal_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-03 12:20:04.000000 jord-0.6.1/jord/gdal_utilities/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      672 2024-05-03 12:20:04.000000 jord-0.6.1/jord/gdal_utilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1087 2024-05-03 12:20:04.000000 jord-0.6.1/jord/gdal_utilities/cloning.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1077 2024-05-03 12:20:04.000000 jord-0.6.1/jord/gdal_utilities/context.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2228 2024-05-03 12:20:04.000000 jord-0.6.1/jord/gdal_utilities/conversion.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      491 2024-05-03 12:20:04.000000 jord-0.6.1/jord/gdal_utilities/drivers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      404 2024-05-03 12:20:04.000000 jord-0.6.1/jord/gdal_utilities/enums.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      768 2024-05-03 12:20:04.000000 jord-0.6.1/jord/gdal_utilities/error_handling.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1231 2024-05-03 12:20:04.000000 jord-0.6.1/jord/gdal_utilities/importing.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2750 2024-05-03 12:20:04.000000 jord-0.6.1/jord/gdal_utilities/persistence.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      351 2024-05-03 12:20:04.000000 jord-0.6.1/jord/gdal_utilities/spatial_reference.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:20:07.887470 jord-0.6.1/jord/geojson_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-03 12:20:04.000000 jord-0.6.1/jord/geojson_utilities/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      448 2024-05-03 12:20:04.000000 jord-0.6.1/jord/geojson_utilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      704 2024-05-03 12:20:04.000000 jord-0.6.1/jord/geojson_utilities/geometry_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:20:07.887470 jord-0.6.1/jord/geometric_analysis/
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-03 12:20:04.000000 jord-0.6.1/jord/geometric_analysis/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      351 2024-05-03 12:20:04.000000 jord-0.6.1/jord/geometric_analysis/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5638 2024-05-03 12:20:04.000000 jord-0.6.1/jord/geometric_analysis/center_line.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      394 2024-05-03 12:20:04.000000 jord-0.6.1/jord/geometric_analysis/degrees_of_freedom.py
--rw-r--r--   0 runner    (1001) docker     (127)    10232 2024-05-03 12:20:04.000000 jord-0.6.1/jord/geometric_analysis/intersections.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      125 2024-05-03 12:20:04.000000 jord-0.6.1/jord/geometric_analysis/tracing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:20:07.887470 jord-0.6.1/jord/geopandas_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-03 12:20:04.000000 jord-0.6.1/jord/geopandas_utilities/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)       82 2024-05-03 12:20:04.000000 jord-0.6.1/jord/geopandas_utilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      756 2024-05-03 12:20:04.000000 jord-0.6.1/jord/geopandas_utilities/geometry_filtering.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      108 2024-05-03 12:20:04.000000 jord-0.6.1/jord/geopandas_utilities/importing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:20:07.887470 jord-0.6.1/jord/geopandas_utilities/serialisation/
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-03 12:20:04.000000 jord-0.6.1/jord/geopandas_utilities/serialisation/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      303 2024-05-03 12:20:04.000000 jord-0.6.1/jord/geopandas_utilities/serialisation/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      673 2024-05-03 12:20:04.000000 jord-0.6.1/jord/geopandas_utilities/serialisation/well_known_binary.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1401 2024-05-03 12:20:04.000000 jord-0.6.1/jord/geopandas_utilities/serialisation/well_known_text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:20:07.891470 jord-0.6.1/jord/networkx_utilities/
--rwxr-xr-x   0 runner    (1001) docker     (127)       51 2024-05-03 12:20:04.000000 jord-0.6.1/jord/networkx_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-03 12:20:04.000000 jord-0.6.1/jord/networkx_utilities/construction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:20:07.891470 jord-0.6.1/jord/pillow_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-03 12:20:04.000000 jord-0.6.1/jord/pillow_utilities/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      455 2024-05-03 12:20:04.000000 jord-0.6.1/jord/pillow_utilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      280 2024-05-03 12:20:04.000000 jord-0.6.1/jord/pillow_utilities/exif.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      476 2024-05-03 12:20:04.000000 jord-0.6.1/jord/pillow_utilities/tiff.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:20:07.891470 jord-0.6.1/jord/qgis_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      937 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3521 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/categorisation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:20:07.891470 jord-0.6.1/jord/qgis_utilities/configuration/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/configuration/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      300 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/configuration/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1057 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/configuration/plugin_settings.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3263 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/configuration/project_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:20:07.895470 jord-0.6.1/jord/qgis_utilities/conversion/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/conversion/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      261 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/conversion/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      179 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/conversion/parsing.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14840 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/data_provider.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1296 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/geo_interface_serialisation.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      915 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/geometry_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:20:07.895470 jord-0.6.1/jord/qgis_utilities/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/helpers/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      502 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/helpers/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2484 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/helpers/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/helpers/copying.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1088 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/helpers/drawing.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6589 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/helpers/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/helpers/garbage_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/helpers/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     8570 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/helpers/logging.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1780 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/helpers/models.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3566 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/helpers/progress_bar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/helpers/randomize.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1208 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/helpers/sessions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2077 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/helpers/signals.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1223 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/helpers/timestamp.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      460 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/importing.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16113 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/layer_creation.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2128 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/layer_serialisation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:20:07.895470 jord-0.6.1/jord/qgis_utilities/numpy_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/numpy_utilities/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      297 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/numpy_utilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2676 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/numpy_utilities/conversion.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4075 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/numpy_utilities/data_type.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2925 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/numpy_utilities/numpy_image_widget.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      474 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/numpy_utilities/rasters.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      392 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/plugin_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/styles.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1978 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/styling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:20:07.899470 jord-0.6.1/jord/qlive_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qlive_utilities/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      367 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qlive_utilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1862 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qlive_utilities/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:20:07.899470 jord-0.6.1/jord/qlive_utilities/clients/
--rwxr-xr-x   0 runner    (1001) docker     (127)       69 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qlive_utilities/clients/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      447 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qlive_utilities/clients/arguments.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2865 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qlive_utilities/clients/auto.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      142 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qlive_utilities/clients/batching.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      366 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qlive_utilities/clients/interfaced.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qlive_utilities/pandas_procedures.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    20181 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qlive_utilities/procedures.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2566 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qlive_utilities/serialisation.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      624 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qlive_utilities/uri_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:20:07.899470 jord-0.6.1/jord/qt_utilities/
--rwxr-xr-x   0 runner    (1001) docker     (127)      240 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qt_utilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    23855 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qt_utilities/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:20:07.899470 jord-0.6.1/jord/rasterio_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-03 12:20:04.000000 jord-0.6.1/jord/rasterio_utilities/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      351 2024-05-03 12:20:04.000000 jord-0.6.1/jord/rasterio_utilities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:20:07.903470 jord-0.6.1/jord/shapely_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-03 12:20:04.000000 jord-0.6.1/jord/shapely_utilities/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      558 2024-05-03 12:20:04.000000 jord-0.6.1/jord/shapely_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-03 12:20:04.000000 jord-0.6.1/jord/shapely_utilities/base.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8327 2024-05-03 12:20:04.000000 jord-0.6.1/jord/shapely_utilities/clamp.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1907 2024-05-03 12:20:04.000000 jord-0.6.1/jord/shapely_utilities/geometry_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-05-03 12:20:04.000000 jord-0.6.1/jord/shapely_utilities/grouping.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    27441 2024-05-03 12:20:04.000000 jord-0.6.1/jord/shapely_utilities/lines.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      918 2024-05-03 12:20:04.000000 jord-0.6.1/jord/shapely_utilities/mirroring.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10107 2024-05-03 12:20:04.000000 jord-0.6.1/jord/shapely_utilities/morphology.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4177 2024-05-03 12:20:04.000000 jord-0.6.1/jord/shapely_utilities/points.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12570 2024-05-03 12:20:04.000000 jord-0.6.1/jord/shapely_utilities/polygons.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5885 2024-05-03 12:20:04.000000 jord-0.6.1/jord/shapely_utilities/projection.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2796 2024-05-03 12:20:04.000000 jord-0.6.1/jord/shapely_utilities/rings.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      585 2024-05-03 12:20:04.000000 jord-0.6.1/jord/shapely_utilities/selection.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2902 2024-05-03 12:20:04.000000 jord-0.6.1/jord/shapely_utilities/transformation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:20:07.903470 jord-0.6.1/jord/spatialite_utilities/
--rwxr-xr-x   0 runner    (1001) docker     (127)       46 2024-05-03 12:20:04.000000 jord-0.6.1/jord/spatialite_utilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      241 2024-05-03 12:20:04.000000 jord-0.6.1/jord/spatialite_utilities/loading.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:20:07.903470 jord-0.6.1/jord/torch_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 12:20:04.000000 jord-0.6.1/jord/torch_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-03 12:20:04.000000 jord-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-03 12:20:04.000000 jord-0.6.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-03 12:20:07.911470 jord-0.6.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     9495 2024-05-03 12:20:04.000000 jord-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:20:07.903470 jord-0.6.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:20:07.903470 jord-0.6.1/tests/qgis/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-03 12:20:04.000000 jord-0.6.1/tests/qgis/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     1997 2024-05-03 12:20:04.000000 jord-0.6.1/tests/test_import.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      471 2024-05-03 12:20:04.000000 jord-0.6.1/tests/test_sanity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:14:21.548720 jord-0.6.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:14:21.516720 jord-0.6.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-06-03 12:14:13.000000 jord-0.6.2/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-06-03 12:14:13.000000 jord-0.6.2/.github/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-06-03 12:14:13.000000 jord-0.6.2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:14:13.000000 jord-0.6.2/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:14:21.540720 jord-0.6.2/Jord.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7059 2024-06-03 12:14:21.000000 jord-0.6.2/Jord.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-06-03 12:14:21.000000 jord-0.6.2/Jord.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 12:14:21.000000 jord-0.6.2/Jord.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-06-03 12:14:21.000000 jord-0.6.2/Jord.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-06-03 12:14:21.000000 jord-0.6.2/Jord.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-06-03 12:14:13.000000 jord-0.6.2/KEYWORDS.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10646 2024-06-03 12:14:13.000000 jord-0.6.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-06-03 12:14:13.000000 jord-0.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7059 2024-06-03 12:14:21.548720 jord-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-06-03 12:14:13.000000 jord-0.6.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-06-03 12:14:13.000000 jord-0.6.2/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:14:21.516720 jord-0.6.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-06-03 12:14:13.000000 jord-0.6.2/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:14:21.516720 jord-0.6.2/jord/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-06-03 12:14:13.000000 jord-0.6.2/jord/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1484 2024-06-03 12:14:13.000000 jord-0.6.2/jord/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:14:21.520720 jord-0.6.2/jord/fiona_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:14:13.000000 jord-0.6.2/jord/fiona_utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      749 2024-06-03 12:14:13.000000 jord-0.6.2/jord/fiona_utilities/deserialise.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:14:21.520720 jord-0.6.2/jord/gdal_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-06-03 12:14:13.000000 jord-0.6.2/jord/gdal_utilities/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      672 2024-06-03 12:14:13.000000 jord-0.6.2/jord/gdal_utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1087 2024-06-03 12:14:13.000000 jord-0.6.2/jord/gdal_utilities/cloning.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1077 2024-06-03 12:14:13.000000 jord-0.6.2/jord/gdal_utilities/context.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2228 2024-06-03 12:14:13.000000 jord-0.6.2/jord/gdal_utilities/conversion.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      491 2024-06-03 12:14:13.000000 jord-0.6.2/jord/gdal_utilities/drivers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      404 2024-06-03 12:14:13.000000 jord-0.6.2/jord/gdal_utilities/enums.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      768 2024-06-03 12:14:13.000000 jord-0.6.2/jord/gdal_utilities/error_handling.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1231 2024-06-03 12:14:13.000000 jord-0.6.2/jord/gdal_utilities/importing.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2750 2024-06-03 12:14:13.000000 jord-0.6.2/jord/gdal_utilities/persistence.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      351 2024-06-03 12:14:13.000000 jord-0.6.2/jord/gdal_utilities/spatial_reference.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:14:21.520720 jord-0.6.2/jord/geojson_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-06-03 12:14:13.000000 jord-0.6.2/jord/geojson_utilities/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      448 2024-06-03 12:14:13.000000 jord-0.6.2/jord/geojson_utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      704 2024-06-03 12:14:13.000000 jord-0.6.2/jord/geojson_utilities/geometry_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:14:21.520720 jord-0.6.2/jord/geometric_analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-06-03 12:14:13.000000 jord-0.6.2/jord/geometric_analysis/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      351 2024-06-03 12:14:13.000000 jord-0.6.2/jord/geometric_analysis/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5638 2024-06-03 12:14:13.000000 jord-0.6.2/jord/geometric_analysis/center_line.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      394 2024-06-03 12:14:13.000000 jord-0.6.2/jord/geometric_analysis/degrees_of_freedom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10232 2024-06-03 12:14:13.000000 jord-0.6.2/jord/geometric_analysis/intersections.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      125 2024-06-03 12:14:13.000000 jord-0.6.2/jord/geometric_analysis/tracing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:14:21.524720 jord-0.6.2/jord/geopandas_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-06-03 12:14:13.000000 jord-0.6.2/jord/geopandas_utilities/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)       82 2024-06-03 12:14:13.000000 jord-0.6.2/jord/geopandas_utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      756 2024-06-03 12:14:13.000000 jord-0.6.2/jord/geopandas_utilities/geometry_filtering.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      108 2024-06-03 12:14:13.000000 jord-0.6.2/jord/geopandas_utilities/importing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:14:21.524720 jord-0.6.2/jord/geopandas_utilities/serialisation/
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-06-03 12:14:13.000000 jord-0.6.2/jord/geopandas_utilities/serialisation/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      303 2024-06-03 12:14:13.000000 jord-0.6.2/jord/geopandas_utilities/serialisation/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      673 2024-06-03 12:14:13.000000 jord-0.6.2/jord/geopandas_utilities/serialisation/well_known_binary.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1401 2024-06-03 12:14:13.000000 jord-0.6.2/jord/geopandas_utilities/serialisation/well_known_text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:14:21.524720 jord-0.6.2/jord/networkx_utilities/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       51 2024-06-03 12:14:13.000000 jord-0.6.2/jord/networkx_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-06-03 12:14:13.000000 jord-0.6.2/jord/networkx_utilities/construction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:14:21.524720 jord-0.6.2/jord/pillow_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-06-03 12:14:13.000000 jord-0.6.2/jord/pillow_utilities/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      455 2024-06-03 12:14:13.000000 jord-0.6.2/jord/pillow_utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      280 2024-06-03 12:14:13.000000 jord-0.6.2/jord/pillow_utilities/exif.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      476 2024-06-03 12:14:13.000000 jord-0.6.2/jord/pillow_utilities/tiff.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:14:21.528720 jord-0.6.2/jord/qgis_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-06-03 12:14:13.000000 jord-0.6.2/jord/qgis_utilities/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      937 2024-06-03 12:14:13.000000 jord-0.6.2/jord/qgis_utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3521 2024-06-03 12:14:13.000000 jord-0.6.2/jord/qgis_utilities/categorisation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:14:21.528720 jord-0.6.2/jord/qgis_utilities/configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-06-03 12:14:13.000000 jord-0.6.2/jord/qgis_utilities/configuration/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      300 2024-06-03 12:14:13.000000 jord-0.6.2/jord/qgis_utilities/configuration/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1057 2024-06-03 12:14:13.000000 jord-0.6.2/jord/qgis_utilities/configuration/plugin_settings.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3263 2024-06-03 12:14:13.000000 jord-0.6.2/jord/qgis_utilities/configuration/project_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:14:21.528720 jord-0.6.2/jord/qgis_utilities/conversion/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-06-03 12:14:13.000000 jord-0.6.2/jord/qgis_utilities/conversion/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      261 2024-06-03 12:14:13.000000 jord-0.6.2/jord/qgis_utilities/conversion/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      179 2024-06-03 12:14:13.000000 jord-0.6.2/jord/qgis_utilities/conversion/parsing.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14840 2024-06-03 12:14:13.000000 jord-0.6.2/jord/qgis_utilities/data_provider.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1296 2024-06-03 12:14:13.000000 jord-0.6.2/jord/qgis_utilities/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-06-03 12:14:13.000000 jord-0.6.2/jord/qgis_utilities/geo_interface_serialisation.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      915 2024-06-03 12:14:13.000000 jord-0.6.2/jord/qgis_utilities/geometry_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:14:21.532720 jord-0.6.2/jord/qgis_utilities/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-06-03 12:14:13.000000 jord-0.6.2/jord/qgis_utilities/helpers/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      502 2024-06-03 12:14:13.000000 jord-0.6.2/jord/qgis_utilities/helpers/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2484 2024-06-03 12:14:13.000000 jord-0.6.2/jord/qgis_utilities/helpers/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-06-03 12:14:13.000000 jord-0.6.2/jord/qgis_utilities/helpers/copying.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1088 2024-06-03 12:14:13.000000 jord-0.6.2/jord/qgis_utilities/helpers/drawing.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6589 2024-06-03 12:14:13.000000 jord-0.6.2/jord/qgis_utilities/helpers/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-06-03 12:14:13.000000 jord-0.6.2/jord/qgis_utilities/helpers/garbage_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-06-03 12:14:13.000000 jord-0.6.2/jord/qgis_utilities/helpers/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8570 2024-06-03 12:14:13.000000 jord-0.6.2/jord/qgis_utilities/helpers/logging.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1780 2024-06-03 12:14:13.000000 jord-0.6.2/jord/qgis_utilities/helpers/models.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3566 2024-06-03 12:14:13.000000 jord-0.6.2/jord/qgis_utilities/helpers/progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-06-03 12:14:13.000000 jord-0.6.2/jord/qgis_utilities/helpers/randomize.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1208 2024-06-03 12:14:13.000000 jord-0.6.2/jord/qgis_utilities/helpers/sessions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2077 2024-06-03 12:14:13.000000 jord-0.6.2/jord/qgis_utilities/helpers/signals.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1223 2024-06-03 12:14:13.000000 jord-0.6.2/jord/qgis_utilities/helpers/timestamp.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      460 2024-06-03 12:14:13.000000 jord-0.6.2/jord/qgis_utilities/importing.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16113 2024-06-03 12:14:13.000000 jord-0.6.2/jord/qgis_utilities/layer_creation.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2128 2024-06-03 12:14:13.000000 jord-0.6.2/jord/qgis_utilities/layer_serialisation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:14:21.532720 jord-0.6.2/jord/qgis_utilities/numpy_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 12:14:13.000000 jord-0.6.2/jord/qgis_utilities/numpy_utilities/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      297 2024-06-03 12:14:13.000000 jord-0.6.2/jord/qgis_utilities/numpy_utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2676 2024-06-03 12:14:13.000000 jord-0.6.2/jord/qgis_utilities/numpy_utilities/conversion.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4075 2024-06-03 12:14:13.000000 jord-0.6.2/jord/qgis_utilities/numpy_utilities/data_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2925 2024-06-03 12:14:13.000000 jord-0.6.2/jord/qgis_utilities/numpy_utilities/numpy_image_widget.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      474 2024-06-03 12:14:13.000000 jord-0.6.2/jord/qgis_utilities/numpy_utilities/rasters.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      392 2024-06-03 12:14:13.000000 jord-0.6.2/jord/qgis_utilities/plugin_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-06-03 12:14:13.000000 jord-0.6.2/jord/qgis_utilities/styles.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1978 2024-06-03 12:14:13.000000 jord-0.6.2/jord/qgis_utilities/styling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:14:21.536720 jord-0.6.2/jord/qlive_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-06-03 12:14:13.000000 jord-0.6.2/jord/qlive_utilities/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      367 2024-06-03 12:14:13.000000 jord-0.6.2/jord/qlive_utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1862 2024-06-03 12:14:13.000000 jord-0.6.2/jord/qlive_utilities/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:14:21.536720 jord-0.6.2/jord/qlive_utilities/clients/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       69 2024-06-03 12:14:13.000000 jord-0.6.2/jord/qlive_utilities/clients/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      447 2024-06-03 12:14:13.000000 jord-0.6.2/jord/qlive_utilities/clients/arguments.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2865 2024-06-03 12:14:13.000000 jord-0.6.2/jord/qlive_utilities/clients/auto.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      142 2024-06-03 12:14:13.000000 jord-0.6.2/jord/qlive_utilities/clients/batching.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      366 2024-06-03 12:14:13.000000 jord-0.6.2/jord/qlive_utilities/clients/interfaced.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:14:13.000000 jord-0.6.2/jord/qlive_utilities/pandas_procedures.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20181 2024-06-03 12:14:13.000000 jord-0.6.2/jord/qlive_utilities/procedures.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2566 2024-06-03 12:14:13.000000 jord-0.6.2/jord/qlive_utilities/serialisation.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      624 2024-06-03 12:14:13.000000 jord-0.6.2/jord/qlive_utilities/uri_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:14:21.536720 jord-0.6.2/jord/qt_utilities/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      240 2024-06-03 12:14:13.000000 jord-0.6.2/jord/qt_utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23809 2024-06-03 12:14:13.000000 jord-0.6.2/jord/qt_utilities/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:14:21.536720 jord-0.6.2/jord/rasterio_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-06-03 12:14:13.000000 jord-0.6.2/jord/rasterio_utilities/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      351 2024-06-03 12:14:13.000000 jord-0.6.2/jord/rasterio_utilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:14:21.540720 jord-0.6.2/jord/shapely_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-06-03 12:14:13.000000 jord-0.6.2/jord/shapely_utilities/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      558 2024-06-03 12:14:13.000000 jord-0.6.2/jord/shapely_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-06-03 12:14:13.000000 jord-0.6.2/jord/shapely_utilities/base.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8327 2024-06-03 12:14:13.000000 jord-0.6.2/jord/shapely_utilities/clamp.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1907 2024-06-03 12:14:13.000000 jord-0.6.2/jord/shapely_utilities/geometry_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-06-03 12:14:13.000000 jord-0.6.2/jord/shapely_utilities/grouping.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27441 2024-06-03 12:14:13.000000 jord-0.6.2/jord/shapely_utilities/lines.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      918 2024-06-03 12:14:13.000000 jord-0.6.2/jord/shapely_utilities/mirroring.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10107 2024-06-03 12:14:13.000000 jord-0.6.2/jord/shapely_utilities/morphology.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4177 2024-06-03 12:14:13.000000 jord-0.6.2/jord/shapely_utilities/points.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12570 2024-06-03 12:14:13.000000 jord-0.6.2/jord/shapely_utilities/polygons.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5885 2024-06-03 12:14:13.000000 jord-0.6.2/jord/shapely_utilities/projection.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2796 2024-06-03 12:14:13.000000 jord-0.6.2/jord/shapely_utilities/rings.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      585 2024-06-03 12:14:13.000000 jord-0.6.2/jord/shapely_utilities/selection.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2902 2024-06-03 12:14:13.000000 jord-0.6.2/jord/shapely_utilities/transformation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:14:21.540720 jord-0.6.2/jord/spatialite_utilities/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       46 2024-06-03 12:14:13.000000 jord-0.6.2/jord/spatialite_utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      241 2024-06-03 12:14:13.000000 jord-0.6.2/jord/spatialite_utilities/loading.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:14:21.540720 jord-0.6.2/jord/torch_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:14:13.000000 jord-0.6.2/jord/torch_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-06-03 12:14:13.000000 jord-0.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-06-03 12:14:13.000000 jord-0.6.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-06-03 12:14:21.548720 jord-0.6.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9495 2024-06-03 12:14:13.000000 jord-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:14:21.540720 jord-0.6.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:14:21.540720 jord-0.6.2/tests/qgis/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-06-03 12:14:13.000000 jord-0.6.2/tests/qgis/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1997 2024-06-03 12:14:13.000000 jord-0.6.2/tests/test_import.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      471 2024-06-03 12:14:13.000000 jord-0.6.2/tests/test_sanity.py
```

### Comparing `jord-0.6.1/.github/CODE_OF_CONDUCT.md` & `jord-0.6.2/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `jord-0.6.1/.github/CONTRIBUTING.md` & `jord-0.6.2/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `jord-0.6.1/Jord.egg-info/PKG-INFO` & `jord-0.6.2/Jord.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jord
-Version: 0.6.1
+Version: 0.6.2
 Home-page: https://github.com/aivclab/jord
 Download-URL: https://github.com/aivclab/jord/releases
 Author: Christian Heider Lindbjerg
 Author-email: chen@mapspeople.dk
 Maintainer: Christian Heider Lindbjerg
 Maintainer-email: chen@mapspeople.dk
 License: Apache License, Version 2.0
@@ -27,96 +27,96 @@
 Requires-Dist: draugr>=1.0.9
 Requires-Dist: numpy>=1.20.0
 Requires-Dist: pyzmq>=1.1.1
 Requires-Dist: sorcery>=0.2.0
 Requires-Dist: sympy>=1.1.1
 Requires-Dist: tqdm>=1.1.1
 Requires-Dist: warg>=1.1.6
-Provides-Extra: q
-Requires-Dist: PySide2; extra == "q"
+Provides-Extra: network
+Requires-Dist: networkx; extra == "network"
+Provides-Extra: shapely
+Requires-Dist: pyproj; extra == "shapely"
+Requires-Dist: shapely; extra == "shapely"
+Provides-Extra: pil
+Requires-Dist: Pillow; extra == "pil"
+Provides-Extra: setup
+Provides-Extra: tests
+Requires-Dist: pytest>=4.4.1; extra == "tests"
+Requires-Dist: mock; extra == "tests"
 Provides-Extra: qgis
 Requires-Dist: PySide2; extra == "qgis"
-Provides-Extra: samples
+Provides-Extra: legacy
+Requires-Dist: importlib-metadata; extra == "legacy"
+Requires-Dist: importlib-resources; extra == "legacy"
+Provides-Extra: gdal
 Provides-Extra: geopandas
 Requires-Dist: geopandas; extra == "geopandas"
-Provides-Extra: extra
 Provides-Extra: docs
 Requires-Dist: sphinxcontrib-programoutput; extra == "docs"
 Requires-Dist: sphinx>=4.0.1; extra == "docs"
 Requires-Dist: furo; extra == "docs"
+Provides-Extra: q
+Requires-Dist: PySide2; extra == "q"
+Provides-Extra: extra
+Provides-Extra: samples
 Provides-Extra: fiona
 Requires-Dist: fiona>=1.1.1; extra == "fiona"
-Provides-Extra: gdal
-Provides-Extra: tests
-Requires-Dist: pytest>=4.4.1; extra == "tests"
-Requires-Dist: mock; extra == "tests"
-Provides-Extra: shapely
-Requires-Dist: shapely; extra == "shapely"
-Requires-Dist: pyproj; extra == "shapely"
-Provides-Extra: network
-Requires-Dist: networkx; extra == "network"
 Provides-Extra: dev
-Requires-Dist: numpy>=1.20.0; extra == "dev"
-Requires-Dist: warg>=1.1.6; extra == "dev"
-Requires-Dist: draugr>=1.0.9; extra == "dev"
+Requires-Dist: pytest>=4.4.1; extra == "dev"
+Requires-Dist: pytest-cov>=2.11.1; extra == "dev"
 Requires-Dist: coveralls>=1.6.0; extra == "dev"
+Requires-Dist: sphinxcontrib-programoutput; extra == "dev"
 Requires-Dist: sorcery>=0.2.0; extra == "dev"
-Requires-Dist: pytest>=4.3.0; extra == "dev"
-Requires-Dist: pytest-cov>=2.11.1; extra == "dev"
-Requires-Dist: twine>=1.13.0; extra == "dev"
-Requires-Dist: wheel>=0.33.0; extra == "dev"
-Requires-Dist: apppath>=1.0.2; extra == "dev"
-Requires-Dist: pip>=22.1.2; extra == "dev"
-Requires-Dist: sphinx>=4.0.1; extra == "dev"
-Requires-Dist: tqdm>=1.1.1; extra == "dev"
-Requires-Dist: sympy>=1.1.1; extra == "dev"
-Requires-Dist: pytest>=4.4.1; extra == "dev"
 Requires-Dist: black[jupyter]>=21.5b0; extra == "dev"
+Requires-Dist: warg>=1.1.6; extra == "dev"
+Requires-Dist: apppath>=1.0.2; extra == "dev"
+Requires-Dist: pytest>=4.3.0; extra == "dev"
 Requires-Dist: furo; extra == "dev"
-Requires-Dist: pyzmq>=1.1.1; extra == "dev"
+Requires-Dist: numpy>=1.20.0; extra == "dev"
+Requires-Dist: sympy>=1.1.1; extra == "dev"
+Requires-Dist: draugr>=1.0.9; extra == "dev"
 Requires-Dist: mock; extra == "dev"
-Requires-Dist: sphinxcontrib-programoutput; extra == "dev"
+Requires-Dist: sphinx>=4.0.1; extra == "dev"
+Requires-Dist: pip>=22.1.2; extra == "dev"
+Requires-Dist: twine>=1.13.0; extra == "dev"
 Requires-Dist: pre-commit>=2.17.0; extra == "dev"
-Provides-Extra: pil
-Requires-Dist: Pillow; extra == "pil"
-Provides-Extra: legacy
-Requires-Dist: importlib-resources; extra == "legacy"
-Requires-Dist: importlib-metadata; extra == "legacy"
-Provides-Extra: setup
+Requires-Dist: pyzmq>=1.1.1; extra == "dev"
+Requires-Dist: tqdm>=1.1.1; extra == "dev"
+Requires-Dist: wheel>=0.33.0; extra == "dev"
 Provides-Extra: all
-Requires-Dist: fiona>=1.1.1; extra == "all"
-Requires-Dist: numpy>=1.20.0; extra == "all"
-Requires-Dist: geopandas; extra == "all"
-Requires-Dist: warg>=1.1.6; extra == "all"
-Requires-Dist: draugr>=1.0.9; extra == "all"
-Requires-Dist: sorcery>=0.2.0; extra == "all"
+Requires-Dist: pytest>=4.4.1; extra == "all"
+Requires-Dist: pytest-cov>=2.11.1; extra == "all"
 Requires-Dist: coveralls>=1.6.0; extra == "all"
+Requires-Dist: sphinxcontrib-programoutput; extra == "all"
+Requires-Dist: sorcery>=0.2.0; extra == "all"
+Requires-Dist: black[jupyter]>=21.5b0; extra == "all"
+Requires-Dist: warg>=1.1.6; extra == "all"
+Requires-Dist: apppath>=1.0.2; extra == "all"
 Requires-Dist: pytest>=4.3.0; extra == "all"
+Requires-Dist: importlib-metadata; extra == "all"
+Requires-Dist: geopandas; extra == "all"
+Requires-Dist: furo; extra == "all"
+Requires-Dist: numpy>=1.20.0; extra == "all"
+Requires-Dist: pyproj; extra == "all"
+Requires-Dist: sympy>=1.1.1; extra == "all"
+Requires-Dist: draugr>=1.0.9; extra == "all"
+Requires-Dist: PySide2; extra == "all"
+Requires-Dist: mock; extra == "all"
+Requires-Dist: sphinx>=4.0.1; extra == "all"
+Requires-Dist: importlib-resources; extra == "all"
 Requires-Dist: Pillow; extra == "all"
-Requires-Dist: pytest-cov>=2.11.1; extra == "all"
-Requires-Dist: twine>=1.13.0; extra == "all"
-Requires-Dist: wheel>=0.33.0; extra == "all"
-Requires-Dist: apppath>=1.0.2; extra == "all"
+Requires-Dist: fiona>=1.1.1; extra == "all"
 Requires-Dist: pip>=22.1.2; extra == "all"
-Requires-Dist: sphinx>=4.0.1; extra == "all"
-Requires-Dist: tqdm>=1.1.1; extra == "all"
-Requires-Dist: importlib-metadata; extra == "all"
+Requires-Dist: twine>=1.13.0; extra == "all"
+Requires-Dist: pre-commit>=2.17.0; extra == "all"
 Requires-Dist: networkx; extra == "all"
-Requires-Dist: sympy>=1.1.1; extra == "all"
-Requires-Dist: pytest>=4.4.1; extra == "all"
-Requires-Dist: black[jupyter]>=21.5b0; extra == "all"
-Requires-Dist: furo; extra == "all"
 Requires-Dist: pyzmq>=1.1.1; extra == "all"
-Requires-Dist: importlib-resources; extra == "all"
-Requires-Dist: mock; extra == "all"
-Requires-Dist: PySide2; extra == "all"
-Requires-Dist: pyproj; extra == "all"
-Requires-Dist: sphinxcontrib-programoutput; extra == "all"
+Requires-Dist: tqdm>=1.1.1; extra == "all"
+Requires-Dist: wheel>=0.33.0; extra == "all"
 Requires-Dist: shapely; extra == "all"
-Requires-Dist: pre-commit>=2.17.0; extra == "all"
 
 <!--![header](.github/images/header.png)-->
 
 <p align="center">
   <img src=".github/images/header.svg" alt='header' />
 </p>
```

### Comparing `jord-0.6.1/Jord.egg-info/SOURCES.txt` & `jord-0.6.2/Jord.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jord-0.6.1/Jord.egg-info/requires.txt` & `jord-0.6.2/Jord.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -4,67 +4,67 @@
 pyzmq>=1.1.1
 sorcery>=0.2.0
 sympy>=1.1.1
 tqdm>=1.1.1
 warg>=1.1.6
 
 [all]
-fiona>=1.1.1
-numpy>=1.20.0
-geopandas
-warg>=1.1.6
-draugr>=1.0.9
-sorcery>=0.2.0
+pytest>=4.4.1
+pytest-cov>=2.11.1
 coveralls>=1.6.0
+sphinxcontrib-programoutput
+sorcery>=0.2.0
+black[jupyter]>=21.5b0
+warg>=1.1.6
+apppath>=1.0.2
 pytest>=4.3.0
+importlib-metadata
+geopandas
+furo
+numpy>=1.20.0
+pyproj
+sympy>=1.1.1
+draugr>=1.0.9
+PySide2
+mock
+sphinx>=4.0.1
+importlib-resources
 Pillow
-pytest-cov>=2.11.1
-twine>=1.13.0
-wheel>=0.33.0
-apppath>=1.0.2
+fiona>=1.1.1
 pip>=22.1.2
-sphinx>=4.0.1
-tqdm>=1.1.1
-importlib-metadata
+twine>=1.13.0
+pre-commit>=2.17.0
 networkx
-sympy>=1.1.1
-pytest>=4.4.1
-black[jupyter]>=21.5b0
-furo
 pyzmq>=1.1.1
-importlib-resources
-mock
-PySide2
-pyproj
-sphinxcontrib-programoutput
+tqdm>=1.1.1
+wheel>=0.33.0
 shapely
-pre-commit>=2.17.0
 
 [dev]
-numpy>=1.20.0
-warg>=1.1.6
-draugr>=1.0.9
+pytest>=4.4.1
+pytest-cov>=2.11.1
 coveralls>=1.6.0
+sphinxcontrib-programoutput
 sorcery>=0.2.0
-pytest>=4.3.0
-pytest-cov>=2.11.1
-twine>=1.13.0
-wheel>=0.33.0
-apppath>=1.0.2
-pip>=22.1.2
-sphinx>=4.0.1
-tqdm>=1.1.1
-sympy>=1.1.1
-pytest>=4.4.1
 black[jupyter]>=21.5b0
+warg>=1.1.6
+apppath>=1.0.2
+pytest>=4.3.0
 furo
-pyzmq>=1.1.1
+numpy>=1.20.0
+sympy>=1.1.1
+draugr>=1.0.9
 mock
-sphinxcontrib-programoutput
+sphinx>=4.0.1
+pip>=22.1.2
+twine>=1.13.0
 pre-commit>=2.17.0
+pyzmq>=1.1.1
+tqdm>=1.1.1
+wheel>=0.33.0
 
 [docs]
 sphinxcontrib-programoutput
 sphinx>=4.0.1
 furo
 
 [extra]
@@ -74,16 +74,16 @@
 
 [gdal]
 
 [geopandas]
 geopandas
 
 [legacy]
-importlib-resources
 importlib-metadata
+importlib-resources
 
 [network]
 networkx
 
 [pil]
 Pillow
 
@@ -94,13 +94,13 @@
 PySide2
 
 [samples]
 
 [setup]
 
 [shapely]
-shapely
 pyproj
+shapely
 
 [tests]
 pytest>=4.4.1
 mock
```

### Comparing `jord-0.6.1/LICENSE.md` & `jord-0.6.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `jord-0.6.1/PKG-INFO` & `jord-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jord
-Version: 0.6.1
+Version: 0.6.2
 Home-page: https://github.com/aivclab/jord
 Download-URL: https://github.com/aivclab/jord/releases
 Author: Christian Heider Lindbjerg
 Author-email: chen@mapspeople.dk
 Maintainer: Christian Heider Lindbjerg
 Maintainer-email: chen@mapspeople.dk
 License: Apache License, Version 2.0
@@ -27,96 +27,96 @@
 Requires-Dist: draugr>=1.0.9
 Requires-Dist: numpy>=1.20.0
 Requires-Dist: pyzmq>=1.1.1
 Requires-Dist: sorcery>=0.2.0
 Requires-Dist: sympy>=1.1.1
 Requires-Dist: tqdm>=1.1.1
 Requires-Dist: warg>=1.1.6
-Provides-Extra: q
-Requires-Dist: PySide2; extra == "q"
+Provides-Extra: network
+Requires-Dist: networkx; extra == "network"
+Provides-Extra: shapely
+Requires-Dist: pyproj; extra == "shapely"
+Requires-Dist: shapely; extra == "shapely"
+Provides-Extra: pil
+Requires-Dist: Pillow; extra == "pil"
+Provides-Extra: setup
+Provides-Extra: tests
+Requires-Dist: pytest>=4.4.1; extra == "tests"
+Requires-Dist: mock; extra == "tests"
 Provides-Extra: qgis
 Requires-Dist: PySide2; extra == "qgis"
-Provides-Extra: samples
+Provides-Extra: legacy
+Requires-Dist: importlib-metadata; extra == "legacy"
+Requires-Dist: importlib-resources; extra == "legacy"
+Provides-Extra: gdal
 Provides-Extra: geopandas
 Requires-Dist: geopandas; extra == "geopandas"
-Provides-Extra: extra
 Provides-Extra: docs
 Requires-Dist: sphinxcontrib-programoutput; extra == "docs"
 Requires-Dist: sphinx>=4.0.1; extra == "docs"
 Requires-Dist: furo; extra == "docs"
+Provides-Extra: q
+Requires-Dist: PySide2; extra == "q"
+Provides-Extra: extra
+Provides-Extra: samples
 Provides-Extra: fiona
 Requires-Dist: fiona>=1.1.1; extra == "fiona"
-Provides-Extra: gdal
-Provides-Extra: tests
-Requires-Dist: pytest>=4.4.1; extra == "tests"
-Requires-Dist: mock; extra == "tests"
-Provides-Extra: shapely
-Requires-Dist: shapely; extra == "shapely"
-Requires-Dist: pyproj; extra == "shapely"
-Provides-Extra: network
-Requires-Dist: networkx; extra == "network"
 Provides-Extra: dev
-Requires-Dist: numpy>=1.20.0; extra == "dev"
-Requires-Dist: warg>=1.1.6; extra == "dev"
-Requires-Dist: draugr>=1.0.9; extra == "dev"
+Requires-Dist: pytest>=4.4.1; extra == "dev"
+Requires-Dist: pytest-cov>=2.11.1; extra == "dev"
 Requires-Dist: coveralls>=1.6.0; extra == "dev"
+Requires-Dist: sphinxcontrib-programoutput; extra == "dev"
 Requires-Dist: sorcery>=0.2.0; extra == "dev"
-Requires-Dist: pytest>=4.3.0; extra == "dev"
-Requires-Dist: pytest-cov>=2.11.1; extra == "dev"
-Requires-Dist: twine>=1.13.0; extra == "dev"
-Requires-Dist: wheel>=0.33.0; extra == "dev"
-Requires-Dist: apppath>=1.0.2; extra == "dev"
-Requires-Dist: pip>=22.1.2; extra == "dev"
-Requires-Dist: sphinx>=4.0.1; extra == "dev"
-Requires-Dist: tqdm>=1.1.1; extra == "dev"
-Requires-Dist: sympy>=1.1.1; extra == "dev"
-Requires-Dist: pytest>=4.4.1; extra == "dev"
 Requires-Dist: black[jupyter]>=21.5b0; extra == "dev"
+Requires-Dist: warg>=1.1.6; extra == "dev"
+Requires-Dist: apppath>=1.0.2; extra == "dev"
+Requires-Dist: pytest>=4.3.0; extra == "dev"
 Requires-Dist: furo; extra == "dev"
-Requires-Dist: pyzmq>=1.1.1; extra == "dev"
+Requires-Dist: numpy>=1.20.0; extra == "dev"
+Requires-Dist: sympy>=1.1.1; extra == "dev"
+Requires-Dist: draugr>=1.0.9; extra == "dev"
 Requires-Dist: mock; extra == "dev"
-Requires-Dist: sphinxcontrib-programoutput; extra == "dev"
+Requires-Dist: sphinx>=4.0.1; extra == "dev"
+Requires-Dist: pip>=22.1.2; extra == "dev"
+Requires-Dist: twine>=1.13.0; extra == "dev"
 Requires-Dist: pre-commit>=2.17.0; extra == "dev"
-Provides-Extra: pil
-Requires-Dist: Pillow; extra == "pil"
-Provides-Extra: legacy
-Requires-Dist: importlib-resources; extra == "legacy"
-Requires-Dist: importlib-metadata; extra == "legacy"
-Provides-Extra: setup
+Requires-Dist: pyzmq>=1.1.1; extra == "dev"
+Requires-Dist: tqdm>=1.1.1; extra == "dev"
+Requires-Dist: wheel>=0.33.0; extra == "dev"
 Provides-Extra: all
-Requires-Dist: fiona>=1.1.1; extra == "all"
-Requires-Dist: numpy>=1.20.0; extra == "all"
-Requires-Dist: geopandas; extra == "all"
-Requires-Dist: warg>=1.1.6; extra == "all"
-Requires-Dist: draugr>=1.0.9; extra == "all"
-Requires-Dist: sorcery>=0.2.0; extra == "all"
+Requires-Dist: pytest>=4.4.1; extra == "all"
+Requires-Dist: pytest-cov>=2.11.1; extra == "all"
 Requires-Dist: coveralls>=1.6.0; extra == "all"
+Requires-Dist: sphinxcontrib-programoutput; extra == "all"
+Requires-Dist: sorcery>=0.2.0; extra == "all"
+Requires-Dist: black[jupyter]>=21.5b0; extra == "all"
+Requires-Dist: warg>=1.1.6; extra == "all"
+Requires-Dist: apppath>=1.0.2; extra == "all"
 Requires-Dist: pytest>=4.3.0; extra == "all"
+Requires-Dist: importlib-metadata; extra == "all"
+Requires-Dist: geopandas; extra == "all"
+Requires-Dist: furo; extra == "all"
+Requires-Dist: numpy>=1.20.0; extra == "all"
+Requires-Dist: pyproj; extra == "all"
+Requires-Dist: sympy>=1.1.1; extra == "all"
+Requires-Dist: draugr>=1.0.9; extra == "all"
+Requires-Dist: PySide2; extra == "all"
+Requires-Dist: mock; extra == "all"
+Requires-Dist: sphinx>=4.0.1; extra == "all"
+Requires-Dist: importlib-resources; extra == "all"
 Requires-Dist: Pillow; extra == "all"
-Requires-Dist: pytest-cov>=2.11.1; extra == "all"
-Requires-Dist: twine>=1.13.0; extra == "all"
-Requires-Dist: wheel>=0.33.0; extra == "all"
-Requires-Dist: apppath>=1.0.2; extra == "all"
+Requires-Dist: fiona>=1.1.1; extra == "all"
 Requires-Dist: pip>=22.1.2; extra == "all"
-Requires-Dist: sphinx>=4.0.1; extra == "all"
-Requires-Dist: tqdm>=1.1.1; extra == "all"
-Requires-Dist: importlib-metadata; extra == "all"
+Requires-Dist: twine>=1.13.0; extra == "all"
+Requires-Dist: pre-commit>=2.17.0; extra == "all"
 Requires-Dist: networkx; extra == "all"
-Requires-Dist: sympy>=1.1.1; extra == "all"
-Requires-Dist: pytest>=4.4.1; extra == "all"
-Requires-Dist: black[jupyter]>=21.5b0; extra == "all"
-Requires-Dist: furo; extra == "all"
 Requires-Dist: pyzmq>=1.1.1; extra == "all"
-Requires-Dist: importlib-resources; extra == "all"
-Requires-Dist: mock; extra == "all"
-Requires-Dist: PySide2; extra == "all"
-Requires-Dist: pyproj; extra == "all"
-Requires-Dist: sphinxcontrib-programoutput; extra == "all"
+Requires-Dist: tqdm>=1.1.1; extra == "all"
+Requires-Dist: wheel>=0.33.0; extra == "all"
 Requires-Dist: shapely; extra == "all"
-Requires-Dist: pre-commit>=2.17.0; extra == "all"
 
 <!--![header](.github/images/header.png)-->
 
 <p align="center">
   <img src=".github/images/header.svg" alt='header' />
 </p>
```

### Comparing `jord-0.6.1/README.md` & `jord-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `jord-0.6.1/SECURITY.md` & `jord-0.6.2/SECURITY.md`

 * *Files identical despite different names*

### Comparing `jord-0.6.1/jord/__init__.py` & `jord-0.6.2/jord/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     from importlib_metadata import PackageNotFoundError
     from importlib_resources import files
 
 from warg import package_is_editable, clean_string, get_version
 
 __project__ = "Jord"
 __author__ = "Christian Heider Lindbjerg"
-__version__ = "0.6.1"
+__version__ = "0.6.2"
 __doc__ = r"""
 .. module:: jord
    :platform: Unix, Windows
    :synopsis: A set of general tools build for geo data.
 
 .. moduleauthor:: Christian Heider Lindbjerg <chen@mapspeople.dk>
```

### Comparing `jord-0.6.1/jord/fiona_utilities/deserialise.py` & `jord-0.6.2/jord/fiona_utilities/deserialise.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.1/jord/gdal_utilities/__init__.py` & `jord-0.6.2/jord/gdal_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.1/jord/gdal_utilities/cloning.py` & `jord-0.6.2/jord/gdal_utilities/cloning.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.1/jord/gdal_utilities/context.py` & `jord-0.6.2/jord/gdal_utilities/context.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.1/jord/gdal_utilities/conversion.py` & `jord-0.6.2/jord/gdal_utilities/conversion.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.1/jord/gdal_utilities/error_handling.py` & `jord-0.6.2/jord/gdal_utilities/error_handling.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.1/jord/gdal_utilities/importing.py` & `jord-0.6.2/jord/gdal_utilities/importing.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.1/jord/gdal_utilities/persistence.py` & `jord-0.6.2/jord/gdal_utilities/persistence.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.1/jord/geojson_utilities/geometry_types.py` & `jord-0.6.2/jord/geojson_utilities/geometry_types.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.1/jord/geometric_analysis/center_line.py` & `jord-0.6.2/jord/geometric_analysis/center_line.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.1/jord/geometric_analysis/intersections.py` & `jord-0.6.2/jord/geometric_analysis/intersections.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.1/jord/geopandas_utilities/geometry_filtering.py` & `jord-0.6.2/jord/geopandas_utilities/geometry_filtering.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.1/jord/geopandas_utilities/serialisation/well_known_binary.py` & `jord-0.6.2/jord/geopandas_utilities/serialisation/well_known_binary.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.1/jord/geopandas_utilities/serialisation/well_known_text.py` & `jord-0.6.2/jord/geopandas_utilities/serialisation/well_known_text.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.1/jord/networkx_utilities/construction.py` & `jord-0.6.2/jord/networkx_utilities/construction.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.1/jord/qgis_utilities/__init__.py` & `jord-0.6.2/jord/qgis_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.1/jord/qgis_utilities/categorisation.py` & `jord-0.6.2/jord/qgis_utilities/categorisation.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.1/jord/qgis_utilities/configuration/plugin_settings.py` & `jord-0.6.2/jord/qgis_utilities/configuration/plugin_settings.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.1/jord/qgis_utilities/configuration/project_settings.py` & `jord-0.6.2/jord/qgis_utilities/configuration/project_settings.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.1/jord/qgis_utilities/data_provider.py` & `jord-0.6.2/jord/qgis_utilities/data_provider.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.1/jord/qgis_utilities/enums.py` & `jord-0.6.2/jord/qgis_utilities/enums.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.1/jord/qgis_utilities/geo_interface_serialisation.py` & `jord-0.6.2/jord/qgis_utilities/geo_interface_serialisation.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.1/jord/qgis_utilities/geometry_types.py` & `jord-0.6.2/jord/qgis_utilities/geometry_types.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.1/jord/qgis_utilities/helpers/actions.py` & `jord-0.6.2/jord/qgis_utilities/helpers/actions.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.1/jord/qgis_utilities/helpers/drawing.py` & `jord-0.6.2/jord/qgis_utilities/helpers/drawing.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.1/jord/qgis_utilities/helpers/environment.py` & `jord-0.6.2/jord/qgis_utilities/helpers/environment.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.1/jord/qgis_utilities/helpers/groups.py` & `jord-0.6.2/jord/qgis_utilities/helpers/groups.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.1/jord/qgis_utilities/helpers/logging.py` & `jord-0.6.2/jord/qgis_utilities/helpers/logging.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.1/jord/qgis_utilities/helpers/models.py` & `jord-0.6.2/jord/qgis_utilities/helpers/models.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.1/jord/qgis_utilities/helpers/progress_bar.py` & `jord-0.6.2/jord/qgis_utilities/helpers/progress_bar.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.1/jord/qgis_utilities/helpers/randomize.py` & `jord-0.6.2/jord/qgis_utilities/helpers/randomize.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.1/jord/qgis_utilities/helpers/sessions.py` & `jord-0.6.2/jord/qgis_utilities/helpers/sessions.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.1/jord/qgis_utilities/helpers/signals.py` & `jord-0.6.2/jord/qgis_utilities/helpers/signals.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.1/jord/qgis_utilities/helpers/timestamp.py` & `jord-0.6.2/jord/qgis_utilities/helpers/timestamp.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.1/jord/qgis_utilities/layer_creation.py` & `jord-0.6.2/jord/qgis_utilities/layer_creation.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.1/jord/qgis_utilities/layer_serialisation.py` & `jord-0.6.2/jord/qgis_utilities/layer_serialisation.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.1/jord/qgis_utilities/numpy_utilities/conversion.py` & `jord-0.6.2/jord/qgis_utilities/numpy_utilities/conversion.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.1/jord/qgis_utilities/numpy_utilities/data_type.py` & `jord-0.6.2/jord/qgis_utilities/numpy_utilities/data_type.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.1/jord/qgis_utilities/numpy_utilities/numpy_image_widget.py` & `jord-0.6.2/jord/qgis_utilities/numpy_utilities/numpy_image_widget.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.1/jord/qgis_utilities/styles.py` & `jord-0.6.2/jord/qgis_utilities/styles.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.1/jord/qgis_utilities/styling.py` & `jord-0.6.2/jord/qgis_utilities/styling.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.1/jord/qlive_utilities/client.py` & `jord-0.6.2/jord/qlive_utilities/client.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.1/jord/qlive_utilities/clients/auto.py` & `jord-0.6.2/jord/qlive_utilities/clients/auto.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.1/jord/qlive_utilities/procedures.py` & `jord-0.6.2/jord/qlive_utilities/procedures.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.1/jord/qlive_utilities/serialisation.py` & `jord-0.6.2/jord/qlive_utilities/serialisation.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.1/jord/qlive_utilities/uri_utilities.py` & `jord-0.6.2/jord/qlive_utilities/uri_utilities.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.1/jord/qt_utilities/enums.py` & `jord-0.6.2/jord/qt_utilities/enums.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 #!/usr/bin/env python3
-from enum import Flag, Enum
+from enum import Enum
 from typing import Any
 
 __all__ = [
     "DockWidgetAreaFlag",
     "KeyEnum",
-    "AlignmentFlag",
-    "AlignmentFlag",
     "INT_TO_CHECK_STATE",
     "CHECK_STATE_TO_INT",
     "check_state_to_bool",
     "str_to_check_state",
     "check_state_to_str",
     "CheckStateEnum",
     "EdgeFlag",
     "DropActionFlag",
     "FocusPolicyFlag",
     "FocusReasonEnum",
     "ColorEnum",
     "WindowModalityEnum",
-    "AlignmentFlag",
+    # "AlignmentFlag",
 ]
 
 try:
 
     from PyQt6.QtCore import Qt
 
-    class AlignmentFlag(Flag):
+    class AlignmentFlag(Enum):
         """
         Alignment
         """
 
         left = Qt.AlignmentFlag.AlignLeft
         right = Qt.AlignmentFlag.AlignRight
         bottom = Qt.AlignmentFlag.AlignBottom
@@ -63,15 +61,15 @@
 
         The window is modal to the application and blocks input to all windows."""
 
         non_modal = Qt.WindowModality.NonModal
         application = Qt.WindowModality.ApplicationModal
         window = Qt.WindowModality.WindowModal
 
-    class DockWidgetAreaFlag(Flag):
+    class DockWidgetAreaFlag(Enum):
         left = (
             Qt.DockWidgetArea.LeftDockWidgetArea
         )  # 0x1	The left dock area of a QMainWindow.
         right = (
             Qt.DockWidgetArea.RightDockWidgetArea
         )  # 0x2	The right dock area of a QMainWindow.
         top = (
@@ -92,15 +90,15 @@
 
 except:
     try:
         from PyQt5.QtCore import Qt
     except:
         from qgis.PyQt.QtCore import Qt
 
-    class AlignmentFlag(Flag):
+    class AlignmentFlag(Enum):
         """
         Alignment
         """
 
         left = Qt.AlignLeft
         right = Qt.AlignRight
         bottom = Qt.AlignBottom
@@ -133,15 +131,15 @@
 
         The window is modal to the application and blocks input to all windows."""
 
         non_modal = Qt.NonModal
         application = Qt.ApplicationModal
         window = Qt.WindowModal
 
-    class DockWidgetAreaFlag(Flag):
+    class DockWidgetAreaFlag(Enum):
         left = Qt.LeftDockWidgetArea  # 0x1	The left dock area of a QMainWindow.
         right = Qt.RightDockWidgetArea  # 0x2	The right dock area of a QMainWindow.
         top = Qt.TopDockWidgetArea  # 0x4	The top dock area of a QMainWindow.
         bottom = Qt.BottomDockWidgetArea  # 0x8	The bottom dock area of a QMainWindow.
         all = (
             Qt.AllDockWidgetAreas
         )  # DockWidgetArea_Mask	All dock widget areas (default).
@@ -169,37 +167,37 @@
     return str(CHECK_STATE_TO_INT[check_state])
 
 
 def check_state_to_bool(check_state: CheckStateEnum) -> bool:
     return CHECK_STATE_TO_INT[check_state] > 0
 
 
-class DropActionFlag(Flag):
+class DropActionFlag(Enum):
     """
       Qt::CopyAction	0x1	Copy the data to the target.
     Qt::MoveAction	0x2	Move the data from the source to the target.
     Qt::LinkAction	0x4	Create a link from the source to the target.
     Qt::ActionMask	0xff
     Qt::IgnoreAction	0x0	Ignore the action (do nothing with the data).
     Qt::TargetMoveAction	0x8002	On Windows, this value is used when the ownership of the D&D data should be taken over by the target application, i.e., the source application should not delete the data. On X11 this value is used to do a move. TargetMoveAction is not used on the Mac.
 
     """
 
 
-class EdgeFlag(Flag):
+class EdgeFlag(Enum):
     """
       Qt::TopEdge	0x00001	The top edge of the rectangle.
     Qt::LeftEdge	0x00002	The left edge of the rectangle.
     Qt::RightEdge	0x00004	The right edge of the rectangle.
     Qt::BottomEdge	0x00008	The bottom edge of the rectangle.
 
     """
 
 
-class FocusPolicyFlag(Flag):
+class FocusPolicyFlag(Enum):
     """
       Qt::TabFocus	0x1	the widget accepts focus by tabbing.
     Qt::ClickFocus	0x2	the widget accepts focus by clicking.
     Qt::StrongFocus	TabFocus | ClickFocus | 0x8	the widget accepts focus by both tabbing and clicking. On macOS this will also be indicate that the widget accepts tab focus when in 'Text/List focus mode'.
     Qt::WheelFocus	StrongFocus | 0x4	like Qt::StrongFocus plus the widget accepts focus by using the mouse wheel.
     Qt::NoFocus	0	the widget does not accept focus.
     """
```

### Comparing `jord-0.6.1/jord/shapely_utilities/__init__.py` & `jord-0.6.2/jord/shapely_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.1/jord/shapely_utilities/base.py` & `jord-0.6.2/jord/shapely_utilities/base.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.1/jord/shapely_utilities/clamp.py` & `jord-0.6.2/jord/shapely_utilities/clamp.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.1/jord/shapely_utilities/geometry_types.py` & `jord-0.6.2/jord/shapely_utilities/geometry_types.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.1/jord/shapely_utilities/grouping.py` & `jord-0.6.2/jord/shapely_utilities/grouping.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.1/jord/shapely_utilities/lines.py` & `jord-0.6.2/jord/shapely_utilities/lines.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.1/jord/shapely_utilities/mirroring.py` & `jord-0.6.2/jord/shapely_utilities/mirroring.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.1/jord/shapely_utilities/morphology.py` & `jord-0.6.2/jord/shapely_utilities/morphology.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.1/jord/shapely_utilities/points.py` & `jord-0.6.2/jord/shapely_utilities/points.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.1/jord/shapely_utilities/polygons.py` & `jord-0.6.2/jord/shapely_utilities/polygons.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.1/jord/shapely_utilities/projection.py` & `jord-0.6.2/jord/shapely_utilities/projection.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.1/jord/shapely_utilities/rings.py` & `jord-0.6.2/jord/shapely_utilities/rings.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.1/jord/shapely_utilities/selection.py` & `jord-0.6.2/jord/shapely_utilities/selection.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.1/jord/shapely_utilities/transformation.py` & `jord-0.6.2/jord/shapely_utilities/transformation.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.1/setup.py` & `jord-0.6.2/setup.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.1/tests/test_import.py` & `jord-0.6.2/tests/test_import.py`

 * *Files identical despite different names*

