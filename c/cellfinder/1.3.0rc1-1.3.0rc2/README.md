# Comparing `tmp/cellfinder-1.3.0rc1.tar.gz` & `tmp/cellfinder-1.3.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellfinder-1.3.0rc1.tar", last modified: Fri May 31 13:59:40 2024, max compression
+gzip compressed data, was "cellfinder-1.3.0rc2.tar", last modified: Mon Jun  3 14:31:00 2024, max compression
```

## Comparing `cellfinder-1.3.0rc1.tar` & `cellfinder-1.3.0rc2.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:40.967397 cellfinder-1.3.0rc1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:40.951397 cellfinder-1.3.0rc1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:40.955397 cellfinder-1.3.0rc1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     5102 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/.github/workflows/test_include_guard.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:40.955397 cellfinder-1.3.0rc1/.napari/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/.napari/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6508 2024-05-31 13:59:40.967397 cellfinder-1.3.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:40.955397 cellfinder-1.3.0rc1/cellfinder/
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/cli_migration_warning.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:40.955397 cellfinder-1.3.0rc1/cellfinder/core/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:40.955397 cellfinder-1.3.0rc1/cellfinder/core/classify/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/classify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6321 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/classify/augment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/classify/classify.py
--rw-r--r--   0 runner    (1001) docker     (127)    17125 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/classify/cube_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    10034 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/classify/resnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/classify/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:40.959397 cellfinder-1.3.0rc1/cellfinder/core/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/config/cellfinder.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:40.959397 cellfinder-1.3.0rc1/cellfinder/core/detect/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/detect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9592 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/detect/detect.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:40.959397 cellfinder-1.3.0rc1/cellfinder/core/detect/filters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/detect/filters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:40.959397 cellfinder-1.3.0rc1/cellfinder/core/detect/filters/plane/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/detect/filters/plane/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/detect/filters/plane/classical_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/detect/filters/plane/plane_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/detect/filters/plane/tile_walker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/detect/filters/setup_filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:40.959397 cellfinder-1.3.0rc1/cellfinder/core/detect/filters/volume/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/detect/filters/volume/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13894 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/detect/filters/volume/ball_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    11307 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/detect/filters/volume/structure_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     7660 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/detect/filters/volume/structure_splitting.py
--rw-r--r--   0 runner    (1001) docker     (127)     7035 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/detect/filters/volume/volume_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:40.959397 cellfinder-1.3.0rc1/cellfinder/core/download/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/download/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/download/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/download/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:40.959397 cellfinder-1.3.0rc1/cellfinder/core/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/tools/array_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/tools/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/tools/image_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/tools/prep.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/tools/source_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/tools/system.py
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/tools/tiff.py
--rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/tools/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:40.963397 cellfinder-1.3.0rc1/cellfinder/core/train/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/train/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13260 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/train/train_yml.py
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:40.963397 cellfinder-1.3.0rc1/cellfinder/napari/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/napari/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21447 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/napari/curation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:40.963397 cellfinder-1.3.0rc1/cellfinder/napari/detect/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/napari/detect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13658 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/napari/detect/detect.py
--rw-r--r--   0 runner    (1001) docker     (127)     5377 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/napari/detect/detect_containers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/napari/detect/thread_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/napari/input_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/napari/napari.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/napari/sample_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:40.963397 cellfinder-1.3.0rc1/cellfinder/napari/train/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/napari/train/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5941 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/napari/train/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/napari/train/train_containers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/napari/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:40.963397 cellfinder-1.3.0rc1/cellfinder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6508 2024-05-31 13:59:40.000000 cellfinder-1.3.0rc1/cellfinder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-31 13:59:40.000000 cellfinder-1.3.0rc1/cellfinder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 13:59:40.000000 cellfinder-1.3.0rc1/cellfinder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-31 13:59:40.000000 cellfinder-1.3.0rc1/cellfinder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-31 13:59:40.000000 cellfinder-1.3.0rc1/cellfinder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-31 13:59:40.000000 cellfinder-1.3.0rc1/cellfinder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 13:59:40.967397 cellfinder-1.3.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:31:00.162577 cellfinder-1.3.0rc2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:31:00.142577 cellfinder-1.3.0rc2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:31:00.146577 cellfinder-1.3.0rc2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     5102 2024-06-03 14:30:47.000000 cellfinder-1.3.0rc2/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-06-03 14:30:47.000000 cellfinder-1.3.0rc2/.github/workflows/test_include_guard.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-06-03 14:30:47.000000 cellfinder-1.3.0rc2/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:31:00.146577 cellfinder-1.3.0rc2/.napari/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-06-03 14:30:47.000000 cellfinder-1.3.0rc2/.napari/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-06-03 14:30:47.000000 cellfinder-1.3.0rc2/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-06-03 14:30:47.000000 cellfinder-1.3.0rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-06-03 14:30:47.000000 cellfinder-1.3.0rc2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6508 2024-06-03 14:31:00.162577 cellfinder-1.3.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-06-03 14:30:47.000000 cellfinder-1.3.0rc2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:31:00.146577 cellfinder-1.3.0rc2/cellfinder/
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-06-03 14:30:47.000000 cellfinder-1.3.0rc2/cellfinder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-06-03 14:30:47.000000 cellfinder-1.3.0rc2/cellfinder/cli_migration_warning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:31:00.150577 cellfinder-1.3.0rc2/cellfinder/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-06-03 14:30:47.000000 cellfinder-1.3.0rc2/cellfinder/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:31:00.150577 cellfinder-1.3.0rc2/cellfinder/core/classify/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:30:47.000000 cellfinder-1.3.0rc2/cellfinder/core/classify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6321 2024-06-03 14:30:47.000000 cellfinder-1.3.0rc2/cellfinder/core/classify/augment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-06-03 14:30:47.000000 cellfinder-1.3.0rc2/cellfinder/core/classify/classify.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17125 2024-06-03 14:30:47.000000 cellfinder-1.3.0rc2/cellfinder/core/classify/cube_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10034 2024-06-03 14:30:47.000000 cellfinder-1.3.0rc2/cellfinder/core/classify/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-06-03 14:30:47.000000 cellfinder-1.3.0rc2/cellfinder/core/classify/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:31:00.150577 cellfinder-1.3.0rc2/cellfinder/core/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:30:47.000000 cellfinder-1.3.0rc2/cellfinder/core/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-06-03 14:30:47.000000 cellfinder-1.3.0rc2/cellfinder/core/config/cellfinder.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:31:00.150577 cellfinder-1.3.0rc2/cellfinder/core/detect/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:30:47.000000 cellfinder-1.3.0rc2/cellfinder/core/detect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9592 2024-06-03 14:30:47.000000 cellfinder-1.3.0rc2/cellfinder/core/detect/detect.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:31:00.150577 cellfinder-1.3.0rc2/cellfinder/core/detect/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:30:47.000000 cellfinder-1.3.0rc2/cellfinder/core/detect/filters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:31:00.154577 cellfinder-1.3.0rc2/cellfinder/core/detect/filters/plane/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-06-03 14:30:47.000000 cellfinder-1.3.0rc2/cellfinder/core/detect/filters/plane/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-06-03 14:30:47.000000 cellfinder-1.3.0rc2/cellfinder/core/detect/filters/plane/classical_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-06-03 14:30:47.000000 cellfinder-1.3.0rc2/cellfinder/core/detect/filters/plane/plane_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-06-03 14:30:47.000000 cellfinder-1.3.0rc2/cellfinder/core/detect/filters/plane/tile_walker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-06-03 14:30:47.000000 cellfinder-1.3.0rc2/cellfinder/core/detect/filters/setup_filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:31:00.154577 cellfinder-1.3.0rc2/cellfinder/core/detect/filters/volume/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:30:47.000000 cellfinder-1.3.0rc2/cellfinder/core/detect/filters/volume/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13894 2024-06-03 14:30:47.000000 cellfinder-1.3.0rc2/cellfinder/core/detect/filters/volume/ball_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11307 2024-06-03 14:30:47.000000 cellfinder-1.3.0rc2/cellfinder/core/detect/filters/volume/structure_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7660 2024-06-03 14:30:47.000000 cellfinder-1.3.0rc2/cellfinder/core/detect/filters/volume/structure_splitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7035 2024-06-03 14:30:47.000000 cellfinder-1.3.0rc2/cellfinder/core/detect/filters/volume/volume_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:31:00.154577 cellfinder-1.3.0rc2/cellfinder/core/download/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:30:47.000000 cellfinder-1.3.0rc2/cellfinder/core/download/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-06-03 14:30:47.000000 cellfinder-1.3.0rc2/cellfinder/core/download/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-06-03 14:30:47.000000 cellfinder-1.3.0rc2/cellfinder/core/download/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-06-03 14:30:47.000000 cellfinder-1.3.0rc2/cellfinder/core/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:31:00.154577 cellfinder-1.3.0rc2/cellfinder/core/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:30:47.000000 cellfinder-1.3.0rc2/cellfinder/core/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-06-03 14:30:47.000000 cellfinder-1.3.0rc2/cellfinder/core/tools/array_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-06-03 14:30:47.000000 cellfinder-1.3.0rc2/cellfinder/core/tools/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-06-03 14:30:47.000000 cellfinder-1.3.0rc2/cellfinder/core/tools/image_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-06-03 14:30:47.000000 cellfinder-1.3.0rc2/cellfinder/core/tools/prep.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-06-03 14:30:47.000000 cellfinder-1.3.0rc2/cellfinder/core/tools/source_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-06-03 14:30:47.000000 cellfinder-1.3.0rc2/cellfinder/core/tools/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-06-03 14:30:47.000000 cellfinder-1.3.0rc2/cellfinder/core/tools/tiff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-06-03 14:30:47.000000 cellfinder-1.3.0rc2/cellfinder/core/tools/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:31:00.154577 cellfinder-1.3.0rc2/cellfinder/core/train/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:30:47.000000 cellfinder-1.3.0rc2/cellfinder/core/train/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13260 2024-06-03 14:30:47.000000 cellfinder-1.3.0rc2/cellfinder/core/train/train_yml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-06-03 14:30:47.000000 cellfinder-1.3.0rc2/cellfinder/core/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:31:00.158577 cellfinder-1.3.0rc2/cellfinder/napari/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:30:47.000000 cellfinder-1.3.0rc2/cellfinder/napari/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21447 2024-06-03 14:30:47.000000 cellfinder-1.3.0rc2/cellfinder/napari/curation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:31:00.158577 cellfinder-1.3.0rc2/cellfinder/napari/detect/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-06-03 14:30:47.000000 cellfinder-1.3.0rc2/cellfinder/napari/detect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13809 2024-06-03 14:30:47.000000 cellfinder-1.3.0rc2/cellfinder/napari/detect/detect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5467 2024-06-03 14:30:47.000000 cellfinder-1.3.0rc2/cellfinder/napari/detect/detect_containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-06-03 14:30:47.000000 cellfinder-1.3.0rc2/cellfinder/napari/detect/thread_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-06-03 14:30:47.000000 cellfinder-1.3.0rc2/cellfinder/napari/input_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-06-03 14:30:47.000000 cellfinder-1.3.0rc2/cellfinder/napari/napari.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-06-03 14:30:47.000000 cellfinder-1.3.0rc2/cellfinder/napari/sample_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:31:00.158577 cellfinder-1.3.0rc2/cellfinder/napari/train/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-06-03 14:30:47.000000 cellfinder-1.3.0rc2/cellfinder/napari/train/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5941 2024-06-03 14:30:47.000000 cellfinder-1.3.0rc2/cellfinder/napari/train/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-06-03 14:30:47.000000 cellfinder-1.3.0rc2/cellfinder/napari/train/train_containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-06-03 14:30:47.000000 cellfinder-1.3.0rc2/cellfinder/napari/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:31:00.158577 cellfinder-1.3.0rc2/cellfinder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6508 2024-06-03 14:30:59.000000 cellfinder-1.3.0rc2/cellfinder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-06-03 14:31:00.000000 cellfinder-1.3.0rc2/cellfinder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 14:30:59.000000 cellfinder-1.3.0rc2/cellfinder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-06-03 14:30:59.000000 cellfinder-1.3.0rc2/cellfinder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-06-03 14:30:59.000000 cellfinder-1.3.0rc2/cellfinder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-06-03 14:30:59.000000 cellfinder-1.3.0rc2/cellfinder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-06-03 14:30:47.000000 cellfinder-1.3.0rc2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 14:31:00.162577 cellfinder-1.3.0rc2/setup.cfg
```

### Comparing `cellfinder-1.3.0rc1/.github/workflows/test_and_deploy.yml` & `cellfinder-1.3.0rc2/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc1/.github/workflows/test_include_guard.yaml` & `cellfinder-1.3.0rc2/.github/workflows/test_include_guard.yaml`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc1/.gitignore` & `cellfinder-1.3.0rc2/.gitignore`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc1/CITATION.cff` & `cellfinder-1.3.0rc2/CITATION.cff`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc1/LICENSE` & `cellfinder-1.3.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc1/PKG-INFO` & `cellfinder-1.3.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellfinder
-Version: 1.3.0rc1
+Version: 1.3.0rc2
 Summary: Automated 3D cell detection in large microscopy images
 Author-email: "Adam Tyson, Christian Niedworok, Charly Rousseau" <code@adamltyson.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://brainglobe.info/documentation/cellfinder/index.html
 Project-URL: Source Code, https://github.com/brainglobe/cellfinder
 Project-URL: Bug Tracker, https://github.com/brainglobe/cellfinder/issues
 Project-URL: Documentation, https://brainglobe.info/documentation/cellfinder/index.html
```

### Comparing `cellfinder-1.3.0rc1/README.md` & `cellfinder-1.3.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc1/cellfinder/__init__.py` & `cellfinder-1.3.0rc2/cellfinder/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -22,11 +22,12 @@
         f"For more information on brainglobe, please see "
         f"https://github.com/brainglobe/brainglobe-meta#readme."
     ) from e
 
 
 # Set the Keras backend to torch
 os.environ["KERAS_BACKEND"] = "torch"
+os.environ["PYTORCH_ENABLE_MPS_FALLBACK"] = "1"
 
 __license__ = "BSD-3-Clause"
 
 DEFAULT_CELLFINDER_DIRECTORY = Path.home() / ".brainglobe" / "cellfinder"
```

### Comparing `cellfinder-1.3.0rc1/cellfinder/cli_migration_warning.py` & `cellfinder-1.3.0rc2/cellfinder/cli_migration_warning.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc1/cellfinder/core/classify/augment.py` & `cellfinder-1.3.0rc2/cellfinder/core/classify/augment.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc1/cellfinder/core/classify/classify.py` & `cellfinder-1.3.0rc2/cellfinder/core/classify/classify.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+from datetime import datetime
 from typing import Any, Callable, Dict, List, Optional, Tuple
 
 import keras
 import numpy as np
 from brainglobe_utils.cells.cells import Cell
 from brainglobe_utils.general.system import get_num_processes
 
@@ -46,14 +47,16 @@
         callbacks = [BatchEndCallback(callback)]
     else:
         callbacks = None
 
     # Too many workers doesn't increase speed, and uses huge amounts of RAM
     workers = get_num_processes(min_free_cpu_cores=n_free_cpus)
 
+    start_time = datetime.now()
+
     logger.debug("Initialising cube generator")
     inference_generator = CubeGeneratorFromFile(
         points,
         signal_array,
         background_array,
         voxel_sizes,
         network_voxel_sizes,
@@ -86,14 +89,19 @@
     points_list = []
 
     # only go through the "extractable" points
     for idx, cell in enumerate(inference_generator.ordered_points):
         cell.type = predictions[idx] + 1
         points_list.append(cell)
 
+    time_elapsed = datetime.now() - start_time
+    print(
+        "Classfication complete - all points done in : {}".format(time_elapsed)
+    )
+
     return points_list
 
 
 class BatchEndCallback(keras.callbacks.Callback):
     def __init__(self, callback: Callable[[int], None]):
         self._callback = callback
```

### Comparing `cellfinder-1.3.0rc1/cellfinder/core/classify/cube_generator.py` & `cellfinder-1.3.0rc2/cellfinder/core/classify/cube_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     def __init__(
         self,
         points: List[Cell],
         signal_array: types.array,
         background_array: types.array,
         voxel_sizes: Tuple[int, int, int],
         network_voxel_sizes: Tuple[int, int, int],
-        batch_size: int = 16,
+        batch_size: int = 64,
         cube_width: int = 50,
         cube_height: int = 50,
         cube_depth: int = 20,
         channels: int = 2,  # No other option currently
         classes: int = 2,
         extract: bool = False,
         train: bool = False,
@@ -341,15 +341,15 @@
     """
 
     def __init__(
         self,
         signal_list: List[Union[str, Path]],
         background_list: List[Union[str, Path]],
         labels: Optional[List[int]] = None,  # only if training or validating
-        batch_size: int = 16,
+        batch_size: int = 64,
         shape: Tuple[int, int, int] = (50, 50, 20),
         channels: int = 2,
         classes: int = 2,
         shuffle: bool = False,
         augment: bool = False,
         augment_likelihood: float = 0.1,
         flip_axis: Tuple[int, int, int] = (0, 1, 2),
```

### Comparing `cellfinder-1.3.0rc1/cellfinder/core/classify/resnet.py` & `cellfinder-1.3.0rc2/cellfinder/core/classify/resnet.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc1/cellfinder/core/classify/tools.py` & `cellfinder-1.3.0rc2/cellfinder/core/classify/tools.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc1/cellfinder/core/detect/detect.py` & `cellfinder-1.3.0rc2/cellfinder/core/detect/detect.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc1/cellfinder/core/detect/filters/plane/classical_filter.py` & `cellfinder-1.3.0rc2/cellfinder/core/detect/filters/plane/classical_filter.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc1/cellfinder/core/detect/filters/plane/plane_filter.py` & `cellfinder-1.3.0rc2/cellfinder/core/detect/filters/plane/plane_filter.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc1/cellfinder/core/detect/filters/plane/tile_walker.py` & `cellfinder-1.3.0rc2/cellfinder/core/detect/filters/plane/tile_walker.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc1/cellfinder/core/detect/filters/setup_filters.py` & `cellfinder-1.3.0rc2/cellfinder/core/detect/filters/setup_filters.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc1/cellfinder/core/detect/filters/volume/ball_filter.py` & `cellfinder-1.3.0rc2/cellfinder/core/detect/filters/volume/ball_filter.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc1/cellfinder/core/detect/filters/volume/structure_detection.py` & `cellfinder-1.3.0rc2/cellfinder/core/detect/filters/volume/structure_detection.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc1/cellfinder/core/detect/filters/volume/structure_splitting.py` & `cellfinder-1.3.0rc2/cellfinder/core/detect/filters/volume/structure_splitting.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc1/cellfinder/core/detect/filters/volume/volume_filter.py` & `cellfinder-1.3.0rc2/cellfinder/core/detect/filters/volume/volume_filter.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc1/cellfinder/core/download/cli.py` & `cellfinder-1.3.0rc2/cellfinder/core/download/cli.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc1/cellfinder/core/download/download.py` & `cellfinder-1.3.0rc2/cellfinder/core/download/download.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc1/cellfinder/core/main.py` & `cellfinder-1.3.0rc2/cellfinder/core/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     background_array: np.ndarray,
     voxel_sizes: Tuple[int, int, int],
     start_plane: int = 0,
     end_plane: int = -1,
     trained_model: Optional[os.PathLike] = None,
     model_weights: Optional[os.PathLike] = None,
     model: model_type = "resnet50_tv",
-    batch_size: int = 32,
+    batch_size: int = 64,
     n_free_cpus: int = 2,
     network_voxel_sizes: Tuple[int, int, int] = (5, 1, 1),
     soma_diameter: int = 16,
     ball_xy_size: int = 6,
     ball_z_size: int = 15,
     ball_overlap_fraction: float = 0.6,
     log_sigma_size: float = 0.2,
```

### Comparing `cellfinder-1.3.0rc1/cellfinder/core/tools/array_operations.py` & `cellfinder-1.3.0rc2/cellfinder/core/tools/array_operations.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc1/cellfinder/core/tools/geometry.py` & `cellfinder-1.3.0rc2/cellfinder/core/tools/geometry.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc1/cellfinder/core/tools/image_processing.py` & `cellfinder-1.3.0rc2/cellfinder/core/tools/image_processing.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc1/cellfinder/core/tools/prep.py` & `cellfinder-1.3.0rc2/cellfinder/core/tools/prep.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc1/cellfinder/core/tools/source_files.py` & `cellfinder-1.3.0rc2/cellfinder/core/tools/source_files.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc1/cellfinder/core/tools/system.py` & `cellfinder-1.3.0rc2/cellfinder/core/tools/system.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc1/cellfinder/core/tools/tiff.py` & `cellfinder-1.3.0rc2/cellfinder/core/tools/tiff.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc1/cellfinder/core/tools/tools.py` & `cellfinder-1.3.0rc2/cellfinder/core/tools/tools.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc1/cellfinder/core/train/train_yml.py` & `cellfinder-1.3.0rc2/cellfinder/core/train/train_yml.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc1/cellfinder/napari/curation.py` & `cellfinder-1.3.0rc2/cellfinder/napari/curation.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         self.cube_width = cube_width
         self.cube_height = cube_height
         self.network_voxel_sizes = network_voxel_sizes
         self.n_free_cpus = n_free_cpus
         self.save_empty_cubes = save_empty_cubes
         self.max_ram = max_ram
         self.voxel_sizes = [5, 2, 2]
-        self.batch_size = 32
+        self.batch_size = 64
         self.viewer = viewer
 
         self.signal_layer = None
         self.background_layer = None
         self.training_data_cell_layer = None
         self.training_data_non_cell_layer = None
```

### Comparing `cellfinder-1.3.0rc1/cellfinder/napari/detect/detect.py` & `cellfinder-1.3.0rc2/cellfinder/napari/detect/detect.py`

 * *Files 2% similar despite different names*

```diff
@@ -249,16 +249,17 @@
         ball_overlap_fraction: float,
         log_sigma_size: float,
         n_sds_above_mean_thresh: int,
         soma_spread_factor: float,
         max_cluster_size: int,
         classification_options,
         skip_classification: bool,
-        trained_model: Optional[Path],
         use_pre_trained_weights: bool,
+        trained_model: Optional[Path],
+        batch_size: int,
         misc_options,
         start_plane: int,
         end_plane: int,
         n_free_cpus: int,
         analyse_local: bool,
         debug: bool,
         reset_button,
@@ -294,14 +295,16 @@
         soma_spread_factor : float
             Cell spread factor (for splitting up cell clusters)
         max_cluster_size : int
             Largest putative cell cluster (in cubic um) where splitting
             should be attempted
         use_pre_trained_weights : bool
             Select to use pre-trained model weights
+        batch_size : int
+            How many points to classify at one time
         skip_classification : bool
             If selected, the classification step is skipped and all cells from
             the detection stage are added
         trained_model : Optional[Path]
             Trained model file path (home directory (default) -> pretrained
             weights)
         start_plane : int
@@ -368,15 +371,18 @@
             soma_spread_factor,
             max_cluster_size,
         )
 
         if use_pre_trained_weights:
             trained_model = None
         classification_inputs = ClassificationInputs(
-            skip_classification, use_pre_trained_weights, trained_model
+            skip_classification,
+            use_pre_trained_weights,
+            trained_model,
+            batch_size,
         )
 
         if analyse_local:
             start_plane, end_plane = find_local_planes(
                 options["viewer"], voxel_size_z, signal_image
             )
         elif not end_plane:
```

### Comparing `cellfinder-1.3.0rc1/cellfinder/napari/detect/detect_containers.py` & `cellfinder-1.3.0rc2/cellfinder/napari/detect/detect_containers.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,14 +110,15 @@
 @dataclass
 class ClassificationInputs(InputContainer):
     """Container for classification inputs."""
 
     skip_classification: bool = False
     use_pre_trained_weights: bool = True
     trained_model: Optional[Path] = Path.home()
+    batch_size: int = 64
 
     def as_core_arguments(self) -> dict:
         args = super().as_core_arguments()
         del args["use_pre_trained_weights"]
         return args
 
     @classmethod
@@ -127,14 +128,15 @@
             use_pre_trained_weights=dict(
                 value=cls.defaults()["use_pre_trained_weights"]
             ),
             trained_model=dict(value=cls.defaults()["trained_model"]),
             skip_classification=dict(
                 value=cls.defaults()["skip_classification"]
             ),
+            batch_size=dict(value=cls.defaults()["batch_size"]),
         )
 
 
 @dataclass
 class MiscInputs(InputContainer):
     """Container for miscellaneous inputs."""
```

### Comparing `cellfinder-1.3.0rc1/cellfinder/napari/detect/thread_worker.py` & `cellfinder-1.3.0rc2/cellfinder/napari/detect/thread_worker.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,18 +68,18 @@
         def detect_finished_callback(points: list) -> None:
             self.npoints_detected = len(points)
             self.update_progress_bar.emit("Setting up classification...", 1, 0)
 
         def classify_callback(batch: int) -> None:
             self.update_progress_bar.emit(
                 "Classifying cells",
-                # Default cellfinder-core batch size is 32. This seems to give
+                # Default cellfinder-core batch size is 64. This seems to give
                 # a slight underestimate of the number of batches though, so
                 # allow for batch number to go over this
-                max(self.npoints_detected // 32 + 1, batch + 1),
+                max(self.npoints_detected // 64 + 1, batch + 1),
                 batch + 1,
             )
 
         result = cellfinder_run(
             **self.data_inputs.as_core_arguments(),
             **self.detection_inputs.as_core_arguments(),
             **self.classification_inputs.as_core_arguments(),
```

### Comparing `cellfinder-1.3.0rc1/cellfinder/napari/input_container.py` & `cellfinder-1.3.0rc2/cellfinder/napari/input_container.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc1/cellfinder/napari/napari.yaml` & `cellfinder-1.3.0rc2/cellfinder/napari/napari.yaml`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc1/cellfinder/napari/sample_data.py` & `cellfinder-1.3.0rc2/cellfinder/napari/sample_data.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc1/cellfinder/napari/train/train.py` & `cellfinder-1.3.0rc2/cellfinder/napari/train/train.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc1/cellfinder/napari/train/train_containers.py` & `cellfinder-1.3.0rc2/cellfinder/napari/train/train_containers.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc1/cellfinder/napari/utils.py` & `cellfinder-1.3.0rc2/cellfinder/napari/utils.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc1/cellfinder.egg-info/PKG-INFO` & `cellfinder-1.3.0rc2/cellfinder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellfinder
-Version: 1.3.0rc1
+Version: 1.3.0rc2
 Summary: Automated 3D cell detection in large microscopy images
 Author-email: "Adam Tyson, Christian Niedworok, Charly Rousseau" <code@adamltyson.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://brainglobe.info/documentation/cellfinder/index.html
 Project-URL: Source Code, https://github.com/brainglobe/cellfinder
 Project-URL: Bug Tracker, https://github.com/brainglobe/cellfinder/issues
 Project-URL: Documentation, https://brainglobe.info/documentation/cellfinder/index.html
```

### Comparing `cellfinder-1.3.0rc1/cellfinder.egg-info/SOURCES.txt` & `cellfinder-1.3.0rc2/cellfinder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc1/pyproject.toml` & `cellfinder-1.3.0rc2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -118,24 +118,16 @@
 python =
     3.9: py39
     3.10: py310
     3.11: py311
 
 [testenv]
 commands = python -m pytest -v --color=yes --cov=cellfinder --cov-report=xml
-deps =
-    pytest
-    pytest-cov
-    pytest-mock
-    pytest-timeout
-    # Even though napari is a requirement for cellfinder.napari, we have to
-    # ensure it is installed with the default Qt backend here.
-    napari[all]
-    pytest-qt
 extras =
+    dev
     napari
 setenv =
     KERAS_BACKEND = torch
 passenv =
     NUMBA_DISABLE_JIT
     CI
     GITHUB_ACTIONS
```

