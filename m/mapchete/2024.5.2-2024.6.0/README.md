# Comparing `tmp/mapchete-2024.5.2.tar.gz` & `tmp/mapchete-2024.6.0.tar.gz`

## Comparing `mapchete-2024.5.2.tar` & `mapchete-2024.6.0.tar`

### file list

```diff
@@ -1,110 +1,110 @@
--rw-r--r--   0        0        0     3828 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/__init__.py
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/enums.py
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/errors.py
--rw-r--r--   0        0        0    17605 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/index.py
--rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/log.py
--rw-r--r--   0        0        0    33227 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/path.py
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/pretty.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/protocols.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/registered.py
--rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/settings.py
--rw-r--r--   0        0        0    18489 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/stac.py
--rw-r--r--   0        0        0     6115 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/testing.py
--rw-r--r--   0        0        0    17586 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/tile.py
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/timer.py
--rw-r--r--   0        0        0    12812 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/types.py
--rw-r--r--   0        0        0     5314 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/validate.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/cli/__init__.py
--rwxr-xr-x   0        0        0      307 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/cli/main.py
--rw-r--r--   0        0        0     5566 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/cli/mpath.py
--rw-r--r--   0        0        0    11251 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/cli/options.py
--rw-r--r--   0        0        0     2404 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/cli/progress_bar.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/cli/default/__init__.py
--rw-r--r--   0        0        0     3748 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/cli/default/convert.py
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/cli/default/cp.py
--rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/cli/default/create.py
--rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/cli/default/execute.py
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/cli/default/formats.py
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/cli/default/index.py
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/cli/default/processes.py
--rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/cli/default/rm.py
--rwxr-xr-x   0        0        0     5055 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/cli/default/serve.py
--rw-r--r--   0        0        0     4279 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/cli/default/stac.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/commands/__init__.py
--rw-r--r--   0        0        0     9459 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/commands/convert.py
--rw-r--r--   0        0        0     6601 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/commands/cp.py
--rw-r--r--   0        0        0     8384 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/commands/execute.py
--rw-r--r--   0        0        0     3450 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/commands/index.py
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/commands/observer.py
--rw-r--r--   0        0        0     6797 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/commands/parser.py
--rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/commands/rm.py
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/config/__init__.py
--rw-r--r--   0        0        0    33609 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/config/base.py
--rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/config/models.py
--rw-r--r--   0        0        0    15283 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/config/parse.py
--rw-r--r--   0        0        0     6287 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/config/process_func.py
--rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/executor/__init__.py
--rw-r--r--   0        0        0     6109 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/executor/base.py
--rw-r--r--   0        0        0     6037 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/executor/concurrent_futures.py
--rw-r--r--   0        0        0    10449 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/executor/dask.py
--rw-r--r--   0        0        0     8238 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/executor/future.py
--rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/executor/sequential.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/executor/types.py
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/formats/__init__.py
--rw-r--r--   0        0        0    20399 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/formats/base.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/formats/drivers.py
--rw-r--r--   0        0        0     3926 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/formats/loaders.py
--rw-r--r--   0        0        0     4855 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/formats/protocols.py
--rw-r--r--   0        0        0    12932 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/formats/tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/formats/default/__init__.py
--rw-r--r--   0        0        0     6523 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/formats/default/_fiona_base.py
--rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/formats/default/flatgeobuf.py
--rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/formats/default/geojson.py
--rw-r--r--   0        0        0    22157 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/formats/default/gtiff.py
--rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/formats/default/mapchete_input.py
--rw-r--r--   0        0        0     6958 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/formats/default/png.py
--rw-r--r--   0        0        0     6381 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/formats/default/png_hillshade.py
--rw-r--r--   0        0        0    11624 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/formats/default/raster_file.py
--rw-r--r--   0        0        0    16845 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/formats/default/tile_directory.py
--rw-r--r--   0        0        0     9690 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/formats/default/vector_file.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/io/__init__.py
--rw-r--r--   0        0        0    12038 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/io/_geometry_operations.py
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/io/_json.py
--rw-r--r--   0        0        0     7559 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/io/_misc.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/io/_path.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/io/profiles.py
--rw-r--r--   0        0        0    20397 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/io/vector.py
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/io/raster/__init__.py
--rw-r--r--   0        0        0    11704 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/io/raster/array.py
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/io/raster/convert.py
--rw-r--r--   0        0        0     7961 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/io/raster/mosaic.py
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/io/raster/open.py
--rw-r--r--   0        0        0    17643 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/io/raster/read.py
--rw-r--r--   0        0        0     7409 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/io/raster/referenced_raster.py
--rw-r--r--   0        0        0     6188 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/io/raster/write.py
--rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/processes/__init__.py
--rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/processes/clip.py
--rw-r--r--   0        0        0     5793 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/processes/contours.py
--rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/processes/convert.py
--rw-r--r--   0        0        0     6764 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/processes/hillshade.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/processes/examples/__init__.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/processes/examples/example_process.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/processing/__init__.py
--rw-r--r--   0        0        0    30124 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/processing/base.py
--rw-r--r--   0        0        0     7107 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/processing/execute.py
--rw-r--r--   0        0        0     5111 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/processing/mp.py
--rw-r--r--   0        0        0    23083 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/processing/tasks.py
--rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/processing/types.py
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/processing/profilers/__init__.py
--rw-r--r--   0        0        0     4289 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/processing/profilers/memory.py
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/processing/profilers/requests.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/processing/profilers/time.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/static/__init__.py
--rw-r--r--   0        0        0     8416 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/static/index.html
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/static/mapchete_template.mapchete
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 mapchete-2024.5.2/mapchete/static/process_template.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 mapchete-2024.5.2/.gitignore
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 mapchete-2024.5.2/LICENSE
--rw-r--r--   0        0        0     6140 2020-02-02 00:00:00.000000 mapchete-2024.5.2/README.rst
--rw-r--r--   0        0        0     3612 2020-02-02 00:00:00.000000 mapchete-2024.5.2/pyproject.toml
--rw-r--r--   0        0        0     9259 2020-02-02 00:00:00.000000 mapchete-2024.5.2/PKG-INFO
+-rw-r--r--   0        0        0     3828 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/__init__.py
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/enums.py
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/errors.py
+-rw-r--r--   0        0        0    17605 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/index.py
+-rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/log.py
+-rw-r--r--   0        0        0    34492 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/path.py
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/pretty.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/protocols.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/registered.py
+-rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/settings.py
+-rw-r--r--   0        0        0    18489 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/stac.py
+-rw-r--r--   0        0        0     6115 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/testing.py
+-rw-r--r--   0        0        0    17586 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/tile.py
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/timer.py
+-rw-r--r--   0        0        0    12812 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/types.py
+-rw-r--r--   0        0        0     5314 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/validate.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/cli/__init__.py
+-rwxr-xr-x   0        0        0      307 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/cli/main.py
+-rw-r--r--   0        0        0     5566 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/cli/mpath.py
+-rw-r--r--   0        0        0    11251 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/cli/options.py
+-rw-r--r--   0        0        0     2404 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/cli/progress_bar.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/cli/default/__init__.py
+-rw-r--r--   0        0        0     3748 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/cli/default/convert.py
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/cli/default/cp.py
+-rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/cli/default/create.py
+-rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/cli/default/execute.py
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/cli/default/formats.py
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/cli/default/index.py
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/cli/default/processes.py
+-rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/cli/default/rm.py
+-rwxr-xr-x   0        0        0     5055 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/cli/default/serve.py
+-rw-r--r--   0        0        0     4279 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/cli/default/stac.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/commands/__init__.py
+-rw-r--r--   0        0        0     9459 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/commands/convert.py
+-rw-r--r--   0        0        0     6601 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/commands/cp.py
+-rw-r--r--   0        0        0     8384 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/commands/execute.py
+-rw-r--r--   0        0        0     3450 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/commands/index.py
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/commands/observer.py
+-rw-r--r--   0        0        0     6797 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/commands/parser.py
+-rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/commands/rm.py
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/config/__init__.py
+-rw-r--r--   0        0        0    33609 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/config/base.py
+-rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/config/models.py
+-rw-r--r--   0        0        0    15283 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/config/parse.py
+-rw-r--r--   0        0        0     6287 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/config/process_func.py
+-rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/executor/__init__.py
+-rw-r--r--   0        0        0     6109 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/executor/base.py
+-rw-r--r--   0        0        0     6037 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/executor/concurrent_futures.py
+-rw-r--r--   0        0        0    10449 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/executor/dask.py
+-rw-r--r--   0        0        0     8238 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/executor/future.py
+-rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/executor/sequential.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/executor/types.py
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/formats/__init__.py
+-rw-r--r--   0        0        0    20399 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/formats/base.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/formats/drivers.py
+-rw-r--r--   0        0        0     3926 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/formats/loaders.py
+-rw-r--r--   0        0        0     4855 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/formats/protocols.py
+-rw-r--r--   0        0        0    12932 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/formats/tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/formats/default/__init__.py
+-rw-r--r--   0        0        0     6523 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/formats/default/_fiona_base.py
+-rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/formats/default/flatgeobuf.py
+-rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/formats/default/geojson.py
+-rw-r--r--   0        0        0    22157 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/formats/default/gtiff.py
+-rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/formats/default/mapchete_input.py
+-rw-r--r--   0        0        0     6958 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/formats/default/png.py
+-rw-r--r--   0        0        0     6381 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/formats/default/png_hillshade.py
+-rw-r--r--   0        0        0    11624 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/formats/default/raster_file.py
+-rw-r--r--   0        0        0    16845 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/formats/default/tile_directory.py
+-rw-r--r--   0        0        0     9690 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/formats/default/vector_file.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/io/__init__.py
+-rw-r--r--   0        0        0    12038 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/io/_geometry_operations.py
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/io/_json.py
+-rw-r--r--   0        0        0     7559 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/io/_misc.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/io/_path.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/io/profiles.py
+-rw-r--r--   0        0        0    20397 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/io/vector.py
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/io/raster/__init__.py
+-rw-r--r--   0        0        0    11704 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/io/raster/array.py
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/io/raster/convert.py
+-rw-r--r--   0        0        0     7961 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/io/raster/mosaic.py
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/io/raster/open.py
+-rw-r--r--   0        0        0    17643 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/io/raster/read.py
+-rw-r--r--   0        0        0     7409 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/io/raster/referenced_raster.py
+-rw-r--r--   0        0        0     6188 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/io/raster/write.py
+-rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/processes/__init__.py
+-rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/processes/clip.py
+-rw-r--r--   0        0        0     5793 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/processes/contours.py
+-rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/processes/convert.py
+-rw-r--r--   0        0        0     6764 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/processes/hillshade.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/processes/examples/__init__.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/processes/examples/example_process.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/processing/__init__.py
+-rw-r--r--   0        0        0    30124 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/processing/base.py
+-rw-r--r--   0        0        0     7107 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/processing/execute.py
+-rw-r--r--   0        0        0     5111 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/processing/mp.py
+-rw-r--r--   0        0        0    23083 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/processing/tasks.py
+-rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/processing/types.py
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/processing/profilers/__init__.py
+-rw-r--r--   0        0        0     4289 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/processing/profilers/memory.py
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/processing/profilers/requests.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/processing/profilers/time.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/static/__init__.py
+-rw-r--r--   0        0        0     8416 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/static/index.html
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/static/mapchete_template.mapchete
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 mapchete-2024.6.0/mapchete/static/process_template.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 mapchete-2024.6.0/.gitignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 mapchete-2024.6.0/LICENSE
+-rw-r--r--   0        0        0     6140 2020-02-02 00:00:00.000000 mapchete-2024.6.0/README.rst
+-rw-r--r--   0        0        0     3612 2020-02-02 00:00:00.000000 mapchete-2024.6.0/pyproject.toml
+-rw-r--r--   0        0        0     9259 2020-02-02 00:00:00.000000 mapchete-2024.6.0/PKG-INFO
```

### Comparing `mapchete-2024.5.2/mapchete/__init__.py` & `mapchete-2024.6.0/mapchete/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     "MapcheteNodataTile",
     "MFuture",
     "RasterInput",
     "RasterInputGroup",
     "VectorInput",
     "VectorInputGroup",
 ]
-__version__ = "2024.5.2"
+__version__ = "2024.6.0"
 
 logger = logging.getLogger(__name__)
 logger.addHandler(logging.NullHandler())
 
 
 def open(
     some_input: Union[MPathLike, dict, MapcheteConfig],
```

### Comparing `mapchete-2024.5.2/mapchete/enums.py` & `mapchete-2024.6.0/mapchete/enums.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/errors.py` & `mapchete-2024.6.0/mapchete/errors.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/index.py` & `mapchete-2024.6.0/mapchete/index.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/log.py` & `mapchete-2024.6.0/mapchete/log.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/path.py` & `mapchete-2024.6.0/mapchete/path.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 """Functions handling paths and file systems."""
+
 from __future__ import annotations
 
 import json
 import logging
 import os
 import warnings
 from collections import defaultdict
 from datetime import datetime
 from functools import cached_property
-from typing import IO, Generator, List, Optional, Set, TextIO, Union
+from io import TextIOWrapper
+from typing import IO, Generator, List, Optional, Set, TextIO, Tuple, Union
 
 import fiona
 import fsspec
 import oyaml as yaml
 import rasterio
 from fiona.session import Session as FioSession
-from fsspec import AbstractFileSystem
+from fsspec.spec import AbstractBufferedFile, AbstractFileSystem
 from rasterio.session import Session as RioSession
 from retry import retry
 
 from mapchete.executor import Executor
 from mapchete.settings import GDALHTTPOptions, IORetrySettings, mapchete_options
 from mapchete.tile import BufferedTile
 from mapchete.types import MPathLike
@@ -32,18 +34,21 @@
 
 
 class MPath(os.PathLike):
     """
     Partially replicates pathlib.Path but with remote file support.
     """
 
+    _storage_options: dict
+    _gdal_options: dict
+
     def __init__(
         self,
         path: Union[str, os.PathLike, MPath],
-        fs: AbstractFileSystem = None,
+        fs: Optional[AbstractFileSystem] = None,
         storage_options: Union[dict, None] = None,
         _info: Union[dict, None] = None,
         **kwargs,
     ):
         self._kwargs = {}
         if isinstance(path, MPath):
             path_str = str(path)
@@ -69,14 +74,15 @@
         if storage_options:
             self._kwargs.update(storage_options=storage_options)
         self._fs = fs
         self._storage_options = dict(
             DEFAULT_STORAGE_OPTIONS, **self._kwargs.get("storage_options") or {}
         )
         self._info = _info
+        self._gdal_options = dict()
 
     @staticmethod
     def from_dict(dictionary: dict) -> MPath:
         path_str = dictionary.get("path")
         if not path_str:
             raise ValueError(
                 f"dictionary representation requires at least a 'path' item: {dictionary}"
@@ -162,22 +168,21 @@
                 **{
                     k: v
                     for k, v in self._storage_options.items()
                     if k not in UNALLOWED_S3_KWARGS
                 },
             )
         elif self._path_str.startswith(("http://", "https://")):
-            if self._storage_options.get("username") or self._storage_options.get(
-                "password"
-            ):  # pragma: no cover
+            username = self._storage_options.get("username")
+            if username:
                 from aiohttp import BasicAuth
 
                 auth = BasicAuth(
-                    self._storage_options.get("username"),
-                    self._storage_options.get("password"),
+                    login=username,
+                    password=self._storage_options.get("password", ""),
                 )
             else:
                 auth = None
             return fsspec.filesystem(
                 "https",
                 auth=auth,
                 **{
@@ -187,15 +192,15 @@
                 },
             )
         else:
             return fsspec.filesystem("file", **self._storage_options)
 
     def fs_session(self):
         if hasattr(self.fs, "session"):
-            return self.fs.session
+            return getattr(self.fs, "session")
         else:
             return None
 
     @cached_property
     def protocols(self) -> Set[str]:
         """Return set of filesystem protocols."""
         if isinstance(self.fs.protocol, str):
@@ -297,26 +302,32 @@
         start = start or base_dir
         if self.is_remote() or self.is_absolute():
             return self
         else:
             return self.new(os.path.relpath(self._path_str, start=start))
 
     def relative_to(self, other: MPathLike) -> str:
-        return str(self.without_protocol().relative_path(other.without_protocol()))
+        return str(
+            self.without_protocol().relative_path(
+                MPath.from_inp(other).without_protocol()
+            )
+        )
 
-    def open(self, mode: str = "r") -> Union[IO, TextIO]:
+    def open(
+        self, mode: str = "r"
+    ) -> Union[IO, TextIO, TextIOWrapper, AbstractBufferedFile]:
         """Open file."""
         return self.fs.open(self._path_str, mode)
 
     @retry(logger=logger, **dict(IORetrySettings()))
     def read_text(self) -> str:
         """Open and return file content as text."""
         try:
             with self.open() as src:
-                return src.read()
+                return str(src.read())
         except FileNotFoundError:
             raise FileNotFoundError(f"{str(self)} not found")
         except Exception as e:  # pragma: no cover
             if self.exists():
                 logger.exception(e)
                 raise e
             else:
@@ -387,36 +398,37 @@
     def walk(
         self,
         maxdepth: Optional[int] = None,
         topdown: bool = True,
         absolute_paths: bool = True,
         **kwargs,
     ) -> Generator[
-        List[Union[MPath, dict], List[Union[MPath, dict]], List[Union[MPath, dict]]],
+        Tuple[Union[MPath, dict], List[Union[MPath, dict]], List[Union[MPath, dict]]],
         None,
         None,
     ]:
         for root, subpaths, files in self.fs.walk(
             str(self), maxdepth=maxdepth, topdown=topdown, **kwargs
         ):
-            yield (
-                self._create_full_path(root, absolute_path=absolute_paths),
-                [
-                    self._create_full_path(
-                        MPath(root) / subpath, absolute_path=absolute_paths
-                    )
-                    for subpath in subpaths
-                ],
-                [
-                    self._create_full_path(
-                        MPath(root) / file, absolute_path=absolute_paths
-                    )
-                    for file in files
-                ],
-            )
+            if isinstance(root, str):
+                yield (
+                    self._create_full_path(root, absolute_path=absolute_paths),
+                    [
+                        self._create_full_path(
+                            MPath(root) / subpath, absolute_path=absolute_paths
+                        )
+                        for subpath in subpaths
+                    ],
+                    [
+                        self._create_full_path(
+                            MPath(root) / file, absolute_path=absolute_paths
+                        )
+                        for file in files
+                    ],
+                )
 
     def rm(self, recursive: bool = False, ignore_errors: bool = False) -> None:
         if (
             not recursive and not ignore_errors and self.is_directory()
         ):  # pragma: no cover
             warnings.warn(f"{self} is a directory, use 'recursive' flag to delete")
         try:
@@ -428,31 +440,32 @@
                 raise
 
     def size(self) -> int:
         return self.info().get("size", self.info().get("Size"))
 
     def last_modified(self) -> datetime:
         # for S3 objects
-        if "LastModified" in self.info():
-            return self.info().get("LastModified")
+        last_modified = self.info().get("LastModified")
+        mtime = self.info().get("mtime")
+        if last_modified:
+            return last_modified
         # for local files
-        elif "mtime" in self.info():
-            mtime = self.info().get("mtime")
+        elif mtime:
             return datetime.fromtimestamp(mtime)
         else:  # pragma: no cover
             raise ValueError("Object timestamp could not be determined.")
 
     def is_directory(self) -> bool:
         # for S3 objects use the possible cached info directory
         if "StorageClass" in self.info():  # pragma: no cover
             return self.info().get("StorageClass") == "DIRECTORY"
         else:
             return self.fs.isdir(self._path_str)
 
-    def joinpath(self, *other: List[MPathLike]) -> MPath:
+    def joinpath(self, *other: Union[MPathLike, List[MPathLike]]) -> MPath:
         """Join path with other."""
         return self.new(os.path.join(self._path_str, *list(map(str, other))))
 
     def as_gdal_str(self) -> str:
         """Return path as GDAL VSI string."""
         if self._path_str.startswith(("http://", "https://")):
             return "/vsicurl/" + self._path_str
@@ -498,35 +511,35 @@
                 gdal_opts.update(GDAL_DISABLE_READDIR_ON_OPEN="EMPTY_DIR")
 
             # limit requests only to allowed extensions
             else:
                 default_remote_extensions = gdal_opts.get(
                     "CPL_VSIL_CURL_ALLOWED_EXTENSIONS", ""
                 ).split(", ")
-                if allowed_remote_extensions:
-                    extensions = allowed_remote_extensions.split(",") + (
-                        default_remote_extensions
-                    )
                 extensions = default_remote_extensions + [self.suffix]
+                if allowed_remote_extensions:
+                    extensions += allowed_remote_extensions
                 # make sure current path extension is added to allowed_remote_extensions
                 gdal_opts.update(
                     CPL_VSIL_CURL_ALLOWED_EXTENSIONS=", ".join(
                         set([ext for ext in extensions if ext != ""])
                     )
                 )
 
             # secure HTTP credentials
-            if self.fs.kwargs.get("auth"):
-                gdal_opts.update(
-                    GDAL_HTTP_USERPWD=f"{self.fs.kwargs['auth'].login}:{self.fs.kwargs['auth'].password}"
-                )
+            auth = getattr(self.fs, "kwargs", {}).get("auth")
+            if auth:
+                gdal_opts.update(GDAL_HTTP_USERPWD=f"{auth.login}:{auth.password}")
 
             # if a custom S3 endpoint is used, we need to deactivate these AWS options
             if self._endpoint_url:
-                gdal_opts.update(AWS_VIRTUAL_HOSTING=False, AWS_HTTPS=False)
+                gdal_opts.update(
+                    AWS_VIRTUAL_HOSTING=False,
+                    AWS_HTTPS=self._gdal_options.get("aws_https", False),
+                )
 
             # merge everything with user options
             gdal_opts.update(user_opts)
 
         # reading only locally, go with user options
         else:
             gdal_opts = user_opts
@@ -534,29 +547,33 @@
         logger.debug("using GDAL options: %s", gdal_opts)
         return gdal_opts
 
     @cached_property
     def _endpoint_url(self) -> Union[str, None]:
         # GDAL parses the paths in a weird way, so we have to be careful with a custom
         # endpoint
-        if hasattr(self.fs, "endpoint_url") and isinstance(self.fs.endpoint_url, str):
-            return self.fs.endpoint_url.lstrip("http://").lstrip("https://")
+        endpoint_url = getattr(self.fs, "endpoint_url", None)
+        if endpoint_url:
+            self._gdal_options.update(aws_https=endpoint_url.startswith("https://"))
+            return endpoint_url.replace("http://", "").replace("https://", "")
         else:
             return None
 
-    def rio_session(self) -> "rasterio.session.Session":
+    def rio_session(self) -> RioSession:
         if self.fs_session():
             # rasterio accepts a Session object but only a boto3.session.Session
             # object and not a aiobotocore.session.AioSession which we get from fsspec
             return RioSession.from_path(
                 self._path_str,
-                aws_access_key_id=self.fs.key,
-                aws_secret_access_key=self.fs.secret,
+                aws_access_key_id=getattr(self.fs, "key"),
+                aws_secret_access_key=getattr(self.fs, "secret"),
                 endpoint_url=self._endpoint_url,
-                requester_pays=self.fs.storage_options.get("requester_pays", False),
+                requester_pays=getattr(self.fs, "storage_options", {}).get(
+                    "requester_pays", False
+                ),
             )
         else:
             return RioSession.from_path(self._path_str)
 
     def rio_env_config(
         self,
         opts: Union[dict, None] = None,
@@ -579,24 +596,26 @@
         """Return preconfigured rasterio.Env context manager for path."""
         return rasterio.Env(
             **self.rio_env_config(
                 opts=opts, allowed_remote_extensions=allowed_remote_extensions
             )
         )
 
-    def fio_session(self) -> "fiona.session.Session":
+    def fio_session(self) -> FioSession:
         if self.fs_session():
             # fiona accepts a Session object but only a boto3.session.Session
             # object and not a aiobotocore.session.AioSession which we get from fsspec
             return FioSession.from_path(
                 self._path_str,
-                aws_access_key_id=self.fs.key,
-                aws_secret_access_key=self.fs.secret,
+                aws_access_key_id=getattr(self.fs, "key"),
+                aws_secret_access_key=getattr(self.fs, "secret"),
                 endpoint_url=self._endpoint_url,
-                requester_pays=self.fs.storage_options.get("requester_pays", False),
+                requester_pays=getattr(self.fs, "storage_options", {}).get(
+                    "requester_pays", False
+                ),
             )
         else:
             return FioSession.from_path(self._path_str)
 
     def fio_env_config(
         self,
         opts: Union[dict, None] = None,
@@ -625,15 +644,15 @@
 
     def __truediv__(self, other: MPathLike) -> MPath:
         """Short for self.joinpath()."""
         return self.joinpath(other)
 
     def __add__(self, other: MPathLike) -> "MPath":
         """Short for self.joinpath()."""
-        return self.new(str(self) + other)
+        return self.new(str(self) + str(other))
 
     def __eq__(self, other: MPathLike):
         if isinstance(other, str):
             return str(self) == other
         else:
             return hash(self) == hash(MPath(other))
 
@@ -685,15 +704,15 @@
     -------
     exists : bool
     """
     return MPath.from_inp(path, fs=fs, **kwargs).exists()
 
 
 def absolute_path(
-    path: Union[MPathLike, None] = None,
+    path: MPathLike,
     base_dir: Union[MPathLike, None] = None,
     **kwargs,
 ) -> MPath:
     """
     Return absolute path if path is local.
 
     Parameters
@@ -705,15 +724,15 @@
     -------
     absolute path
     """
     return MPath.from_inp(path, **kwargs).absolute_path(base_dir=base_dir)
 
 
 def relative_path(
-    path: Union[MPathLike, None] = None,
+    path: MPathLike,
     base_dir: Union[MPathLike, None] = None,
     **kwargs,
 ) -> MPath:
     """
     Return relative path if path is local.
 
     Parameters
@@ -738,19 +757,23 @@
     ----------
     path : path
     """
     MPath.from_inp(path, fs=fs, **kwargs).makedirs()
 
 
 def tiles_exist(
-    config=None,
-    output_tiles=None,
-    output_tiles_batches=None,
-    process_tiles=None,
-    process_tiles_batches=None,
+    config,
+    output_tiles: Optional[Generator[BufferedTile, None, None]] = None,
+    output_tiles_batches: Optional[
+        Generator[Generator[BufferedTile, None, None], None, None]
+    ] = None,
+    process_tiles: Optional[Generator[BufferedTile, None, None]] = None,
+    process_tiles_batches: Optional[
+        Generator[Generator[BufferedTile, None, None], None, None]
+    ] = None,
     **kwargs,
 ):
     """
     Yield tiles and whether their output already exists or not.
 
     Either "output_tiles" or "process_tiles" have to be provided.
 
@@ -794,18 +817,23 @@
                 tile,
                 config.output_reader.tiles_exist(
                     **{"process_tile" if process_tiles else "output_tile": tile}
                 ),
             )
 
         def _tiles():
-            if process_tiles or output_tiles:  # pragma: no cover
-                yield from process_tiles or output_tiles
-            else:
-                for batch in process_tiles_batches or output_tiles_batches:
+            if process_tiles:  # pragma: no cover
+                yield from process_tiles
+            elif output_tiles:  # pragma: no cover
+                yield from output_tiles
+            elif process_tiles_batches:
+                for batch in process_tiles_batches:
+                    yield from batch
+            elif output_tiles_batches:  # pragma: no cover
+                for batch in output_tiles_batches:
                     yield from batch
 
         for tile in _tiles():
             yield _exists(tile=tile)
 
     # for tile directory outputs:
     elif process_tiles:
@@ -815,47 +843,60 @@
         )
         process_tiles_batches = _batch_tiles_by_attribute(process_tiles, sort_attribute)
     elif output_tiles:
         sort_attribute = batch_sort_property(config.output_reader.tile_path_schema)
         logger.debug("sort output tiles by %s, this could take a while", sort_attribute)
         output_tiles_batches = _batch_tiles_by_attribute(output_tiles, sort_attribute)
 
+    if process_tiles_batches:
+        yield from _process_tiles_batches_exist(
+            process_tiles_batches,
+            config,
+            _is_https_without_ls(config.output_reader.path),
+        )
+    elif output_tiles_batches:
+        yield from _output_tiles_batches_exist(
+            output_tiles_batches,
+            config,
+            _is_https_without_ls(config.output_reader.path),
+        )
+
+
+def _is_https_without_ls(path: MPath, default_file: str = "metadata.json") -> bool:
     # Some HTTP endpoints won't allow ls() on them, so we will have to
     # request tile by tile in order to determine whether they exist or not.
     # This flag will trigger this further down.
     is_https_without_ls = False
-    if "https" in config.output_reader.path.protocols:
+    if "https" in path.protocols:
         try:
-            config.output_reader.path.ls()
+            path.ls()
         except FileNotFoundError:  # pragma: no cover
-            metadata_json = config.output_reader.path / "metadata.json"
+            metadata_json = path / default_file
             if not metadata_json.exists():
                 raise FileNotFoundError(
-                    f"TileDirectory does not seem to exist or metadata.json is not available: {config.output_reader.path}"
+                    f"TileDirectory does not seem to exist or {default_file} is not available: {path}"
                 )
             is_https_without_ls = True
+    return is_https_without_ls
 
-    if process_tiles_batches:
-        yield from _process_tiles_batches_exist(
-            process_tiles_batches, config, is_https_without_ls
-        )
-    elif output_tiles_batches:
-        yield from _output_tiles_batches_exist(
-            output_tiles_batches, config, is_https_without_ls
-        )
 
-
-def _batch_tiles_by_attribute(tiles: List[BufferedTile], attribute: str = "row"):
+def _batch_tiles_by_attribute(
+    tiles: Generator[BufferedTile, None, None], attribute: str = "row"
+) -> Generator[Generator[BufferedTile, None, None], None, None]:
     ordered = defaultdict(set)
     for tile in tiles:
         ordered[getattr(tile, attribute)].add(tile)
     return ((t for t in ordered[key]) for key in sorted(list(ordered.keys())))
 
 
-def _output_tiles_batches_exist(output_tiles_batches, config, is_https_without_ls):
+def _output_tiles_batches_exist(
+    output_tiles_batches: Generator[Generator[BufferedTile, None, None], None, None],
+    config,
+    is_https_without_ls,
+):
     with Executor(concurrency=mapchete_options.tiles_exist_concurrency) as executor:
         for batch in executor.as_completed(
             _output_tiles_batch_exists,
             (list(b) for b in output_tiles_batches),
             fargs=(config, is_https_without_ls),
         ):
             yield from batch.result()
@@ -926,17 +967,17 @@
             for tile in tiles
         ]
     else:  # pragma: no cover
         return []
 
 
 def _existing_output_tiles(
-    output_rows=None,
-    output_paths=None,
-    config=None,
+    output_rows: List[BufferedTile],
+    output_paths: dict,
+    config,
     zoom=None,
     is_https_without_ls=False,
 ):
     existing_tiles = set()
     for row in output_rows:
         logger.debug("check existing tiles in row %s", row)
         rowpath = config.output_reader.path.joinpath(zoom, row)
@@ -959,16 +1000,15 @@
                 pass
 
     return existing_tiles
 
 
 def fs_from_path(path: MPathLike, **kwargs) -> fsspec.AbstractFileSystem:
     """Guess fsspec FileSystem from path and initialize using the desired options."""
-    path = path if isinstance(path, MPath) else MPath(path, **kwargs)
-    return path.fs
+    return path.fs if isinstance(path, MPath) else MPath(path, **kwargs).fs
 
 
 def batch_sort_property(tile_path_schema: str) -> str:
     """
     Determine by which property according to the schema batches should be sorted.
 
     In order to reduce S3 requests this function determines the root directory name in a
```

### Comparing `mapchete-2024.5.2/mapchete/pretty.py` & `mapchete-2024.6.0/mapchete/pretty.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/protocols.py` & `mapchete-2024.6.0/mapchete/protocols.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/registered.py` & `mapchete-2024.6.0/mapchete/registered.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/settings.py` & `mapchete-2024.6.0/mapchete/settings.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/stac.py` & `mapchete-2024.6.0/mapchete/stac.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/testing.py` & `mapchete-2024.6.0/mapchete/testing.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/tile.py` & `mapchete-2024.6.0/mapchete/tile.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/timer.py` & `mapchete-2024.6.0/mapchete/timer.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/types.py` & `mapchete-2024.6.0/mapchete/types.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/validate.py` & `mapchete-2024.6.0/mapchete/validate.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/cli/mpath.py` & `mapchete-2024.6.0/mapchete/cli/mpath.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/cli/options.py` & `mapchete-2024.6.0/mapchete/cli/options.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/cli/progress_bar.py` & `mapchete-2024.6.0/mapchete/cli/progress_bar.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/cli/default/convert.py` & `mapchete-2024.6.0/mapchete/cli/default/convert.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/cli/default/cp.py` & `mapchete-2024.6.0/mapchete/cli/default/cp.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/cli/default/create.py` & `mapchete-2024.6.0/mapchete/cli/default/create.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/cli/default/execute.py` & `mapchete-2024.6.0/mapchete/cli/default/execute.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/cli/default/formats.py` & `mapchete-2024.6.0/mapchete/cli/default/formats.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/cli/default/index.py` & `mapchete-2024.6.0/mapchete/cli/default/index.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/cli/default/processes.py` & `mapchete-2024.6.0/mapchete/cli/default/processes.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/cli/default/rm.py` & `mapchete-2024.6.0/mapchete/cli/default/rm.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/cli/default/serve.py` & `mapchete-2024.6.0/mapchete/cli/default/serve.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/cli/default/stac.py` & `mapchete-2024.6.0/mapchete/cli/default/stac.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/commands/convert.py` & `mapchete-2024.6.0/mapchete/commands/convert.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/commands/cp.py` & `mapchete-2024.6.0/mapchete/commands/cp.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/commands/execute.py` & `mapchete-2024.6.0/mapchete/commands/execute.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/commands/index.py` & `mapchete-2024.6.0/mapchete/commands/index.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/commands/parser.py` & `mapchete-2024.6.0/mapchete/commands/parser.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/commands/rm.py` & `mapchete-2024.6.0/mapchete/commands/rm.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/config/base.py` & `mapchete-2024.6.0/mapchete/config/base.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/config/models.py` & `mapchete-2024.6.0/mapchete/config/models.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/config/parse.py` & `mapchete-2024.6.0/mapchete/config/parse.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/config/process_func.py` & `mapchete-2024.6.0/mapchete/config/process_func.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/executor/__init__.py` & `mapchete-2024.6.0/mapchete/executor/__init__.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/executor/base.py` & `mapchete-2024.6.0/mapchete/executor/base.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/executor/concurrent_futures.py` & `mapchete-2024.6.0/mapchete/executor/concurrent_futures.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/executor/dask.py` & `mapchete-2024.6.0/mapchete/executor/dask.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/executor/future.py` & `mapchete-2024.6.0/mapchete/executor/future.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/executor/sequential.py` & `mapchete-2024.6.0/mapchete/executor/sequential.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/formats/__init__.py` & `mapchete-2024.6.0/mapchete/formats/__init__.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/formats/base.py` & `mapchete-2024.6.0/mapchete/formats/base.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/formats/loaders.py` & `mapchete-2024.6.0/mapchete/formats/loaders.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/formats/protocols.py` & `mapchete-2024.6.0/mapchete/formats/protocols.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/formats/tools.py` & `mapchete-2024.6.0/mapchete/formats/tools.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/formats/default/_fiona_base.py` & `mapchete-2024.6.0/mapchete/formats/default/_fiona_base.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/formats/default/flatgeobuf.py` & `mapchete-2024.6.0/mapchete/formats/default/flatgeobuf.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/formats/default/geojson.py` & `mapchete-2024.6.0/mapchete/formats/default/geojson.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/formats/default/gtiff.py` & `mapchete-2024.6.0/mapchete/formats/default/gtiff.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/formats/default/mapchete_input.py` & `mapchete-2024.6.0/mapchete/formats/default/mapchete_input.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/formats/default/png.py` & `mapchete-2024.6.0/mapchete/formats/default/png.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/formats/default/png_hillshade.py` & `mapchete-2024.6.0/mapchete/formats/default/png_hillshade.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/formats/default/raster_file.py` & `mapchete-2024.6.0/mapchete/formats/default/raster_file.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/formats/default/tile_directory.py` & `mapchete-2024.6.0/mapchete/formats/default/tile_directory.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/formats/default/vector_file.py` & `mapchete-2024.6.0/mapchete/formats/default/vector_file.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/io/__init__.py` & `mapchete-2024.6.0/mapchete/io/__init__.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/io/_geometry_operations.py` & `mapchete-2024.6.0/mapchete/io/_geometry_operations.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/io/_misc.py` & `mapchete-2024.6.0/mapchete/io/_misc.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/io/profiles.py` & `mapchete-2024.6.0/mapchete/io/profiles.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/io/vector.py` & `mapchete-2024.6.0/mapchete/io/vector.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/io/raster/__init__.py` & `mapchete-2024.6.0/mapchete/io/raster/__init__.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/io/raster/array.py` & `mapchete-2024.6.0/mapchete/io/raster/array.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/io/raster/convert.py` & `mapchete-2024.6.0/mapchete/io/raster/convert.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/io/raster/mosaic.py` & `mapchete-2024.6.0/mapchete/io/raster/mosaic.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/io/raster/open.py` & `mapchete-2024.6.0/mapchete/io/raster/open.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/io/raster/read.py` & `mapchete-2024.6.0/mapchete/io/raster/read.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/io/raster/referenced_raster.py` & `mapchete-2024.6.0/mapchete/io/raster/referenced_raster.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/io/raster/write.py` & `mapchete-2024.6.0/mapchete/io/raster/write.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/processes/__init__.py` & `mapchete-2024.6.0/mapchete/processes/__init__.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/processes/clip.py` & `mapchete-2024.6.0/mapchete/processes/clip.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/processes/contours.py` & `mapchete-2024.6.0/mapchete/processes/contours.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/processes/convert.py` & `mapchete-2024.6.0/mapchete/processes/convert.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/processes/hillshade.py` & `mapchete-2024.6.0/mapchete/processes/hillshade.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/processes/examples/example_process.py` & `mapchete-2024.6.0/mapchete/processes/examples/example_process.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/processing/base.py` & `mapchete-2024.6.0/mapchete/processing/base.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/processing/execute.py` & `mapchete-2024.6.0/mapchete/processing/execute.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/processing/mp.py` & `mapchete-2024.6.0/mapchete/processing/mp.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/processing/tasks.py` & `mapchete-2024.6.0/mapchete/processing/tasks.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/processing/types.py` & `mapchete-2024.6.0/mapchete/processing/types.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/processing/profilers/__init__.py` & `mapchete-2024.6.0/mapchete/processing/profilers/__init__.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/processing/profilers/memory.py` & `mapchete-2024.6.0/mapchete/processing/profilers/memory.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/processing/profilers/requests.py` & `mapchete-2024.6.0/mapchete/processing/profilers/requests.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/processing/profilers/time.py` & `mapchete-2024.6.0/mapchete/processing/profilers/time.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/static/index.html` & `mapchete-2024.6.0/mapchete/static/index.html`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/mapchete/static/process_template.py` & `mapchete-2024.6.0/mapchete/static/process_template.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/LICENSE` & `mapchete-2024.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/README.rst` & `mapchete-2024.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/pyproject.toml` & `mapchete-2024.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.2/PKG-INFO` & `mapchete-2024.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mapchete
-Version: 2024.5.2
+Version: 2024.6.0
 Summary: Tile-based geodata processing using rasterio & Fiona
 Project-URL: Homepage, https://github.com/ungarj/mapchete
 Author-email: Joachim Ungar <joachim.ungar@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

