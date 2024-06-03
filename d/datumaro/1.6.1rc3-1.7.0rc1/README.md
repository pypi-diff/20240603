# Comparing `tmp/datumaro-1.6.1rc3.tar.gz` & `tmp/datumaro-1.7.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datumaro-1.6.1rc3.tar", last modified: Fri Apr 19 02:44:12 2024, max compression
+gzip compressed data, was "datumaro-1.7.0rc1.tar", last modified: Mon Jun  3 01:44:20 2024, max compression
```

## Comparing `datumaro-1.6.1rc3.tar` & `datumaro-1.7.0rc1.tar`

### file list

```diff
@@ -1,396 +1,403 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.525696 datumaro-1.6.1rc3/
--rw-r--r--   0 runner    (1001) docker     (127)   393113 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/3rd-party.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     7790 2024-04-19 02:44:12.525696 datumaro-1.6.1rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/requirements-core.txt
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/requirements-default.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.465696 datumaro-1.6.1rc3/rust/
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/rust/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.465696 datumaro-1.6.1rc3/rust/src/
--rw-r--r--   0 runner    (1001) docker     (127)     6711 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/rust/src/coco_page_mapper.rs
--rw-r--r--   0 runner    (1001) docker     (127)     6592 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/rust/src/datum_page_mapper.rs
--rw-r--r--   0 runner    (1001) docker     (127)     6110 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/rust/src/json_section_page_mapper.rs
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/rust/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/rust/src/page_mapper.rs
--rw-r--r--   0 runner    (1001) docker     (127)     8637 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/rust/src/page_maps.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/rust/src/utils.rs
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 02:44:12.525696 datumaro-1.6.1rc3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.457696 datumaro-1.6.1rc3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.469696 datumaro-1.6.1rc3/src/datumaro/
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.469696 datumaro-1.6.1rc3/src/datumaro/capi/
--rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/capi/pybind.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.469696 datumaro-1.6.1rc3/src/datumaro/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.473696 datumaro-1.6.1rc3/src/datumaro/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8966 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/commands/compare.py
--rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/commands/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/commands/detect_format.py
--rw-r--r--   0 runner    (1001) docker     (127)    10170 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/commands/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     9176 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/commands/explain.py
--rw-r--r--   0 runner    (1001) docker     (127)     6841 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/commands/explore.py
--rw-r--r--   0 runner    (1001) docker     (127)     9046 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/commands/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/commands/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/commands/info.py
--rw-r--r--   0 runner    (1001) docker     (127)    10289 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/commands/merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     5990 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/commands/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/commands/prune.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.473696 datumaro-1.6.1rc3/src/datumaro/cli/commands/require_project/
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/commands/require_project/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.473696 datumaro-1.6.1rc3/src/datumaro/cli/commands/require_project/modification/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/commands/require_project/modification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/commands/require_project/modification/add.py
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/commands/require_project/modification/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     5924 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/commands/require_project/modification/export.py
--rw-r--r--   0 runner    (1001) docker     (127)     5912 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/commands/require_project/modification/import_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/commands/require_project/modification/remove.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.473696 datumaro-1.6.1rc3/src/datumaro/cli/commands/require_project/versioning/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/commands/require_project/versioning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/commands/require_project/versioning/checkout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/commands/require_project/versioning/commit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/commands/require_project/versioning/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/commands/require_project/versioning/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/commands/require_project/versioning/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/commands/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     8383 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/commands/transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/commands/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.477696 datumaro-1.6.1rc3/src/datumaro/cli/contexts/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9089 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/contexts/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.477696 datumaro-1.6.1rc3/src/datumaro/cli/contexts/project/
--rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/contexts/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/contexts/source.py
--rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/contexts/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.477696 datumaro-1.6.1rc3/src/datumaro/cli/util/
--rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13053 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/util/compare.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/util/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5640 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/cli/util/project.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.481696 datumaro-1.6.1rc3/src/datumaro/components/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.481696 datumaro-1.6.1rc3/src/datumaro/components/abstracts/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/abstracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/abstracts/merger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/abstracts/model_interpreter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.481696 datumaro-1.6.1rc3/src/datumaro/components/algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/algorithms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.485696 datumaro-1.6.1rc3/src/datumaro/components/algorithms/hash_key_inference/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/algorithms/hash_key_inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/algorithms/hash_key_inference/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5629 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/algorithms/hash_key_inference/explorer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5511 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/algorithms/hash_key_inference/hashkey_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    13546 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/algorithms/hash_key_inference/prune.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.485696 datumaro-1.6.1rc3/src/datumaro/components/algorithms/noisy_label_detection/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/algorithms/noisy_label_detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8957 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4706 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/algorithms/rise.py
--rw-r--r--   0 runner    (1001) docker     (127)    36472 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/annotation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.485696 datumaro-1.6.1rc3/src/datumaro/components/annotations/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/annotations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11469 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/annotations/matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/annotations/merger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/cli_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    25400 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/comparator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/config_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.485696 datumaro-1.6.1rc3/src/datumaro/components/contexts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/contexts/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/crypter.py
--rw-r--r--   0 runner    (1001) docker     (127)    34148 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     7574 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/dataset_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6585 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/dataset_item_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    26104 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/dataset_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     9843 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)    18441 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    14785 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)    19973 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/extractor_tfds.py
--rw-r--r--   0 runner    (1001) docker     (127)    14541 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    19999 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/format_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.485696 datumaro-1.6.1rc3/src/datumaro/components/hl_ops/
--rw-r--r--   0 runner    (1001) docker     (127)    15576 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/hl_ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8271 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6878 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/launcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/lazy_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    41468 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/media.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.485696 datumaro-1.6.1rc3/src/datumaro/components/merge/
--rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/merge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/merge/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    12380 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/merge/exact_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/merge/extractor_merger.py
--rw-r--r--   0 runner    (1001) docker     (127)    24403 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/merge/intersect_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/merge/union_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)    14387 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/progress_reporting.py
--rw-r--r--   0 runner    (1001) docker     (127)    89550 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     9666 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/shift_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6542 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/validator.py
--rw-r--r--   0 runner    (1001) docker     (127)    23697 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/components/visualizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/ops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.489696 datumaro-1.6.1rc3/src/datumaro/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.489696 datumaro-1.6.1rc3/src/datumaro/plugins/accuracy_checker_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/accuracy_checker_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.489696 datumaro-1.6.1rc3/src/datumaro/plugins/accuracy_checker_plugin/details/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/accuracy_checker_plugin/details/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4508 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/accuracy_checker_plugin/details/ac.py
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/accuracy_checker_plugin/details/representation.py
--rw-r--r--   0 runner    (1001) docker     (127)    15491 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/anchor_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    37755 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/configurable_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.497696 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/ade20k2017.py
--rw-r--r--   0 runner    (1001) docker     (127)     8831 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/ade20k2020.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.497696 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/arrow/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/arrow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5553 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/arrow/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9866 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/arrow/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/arrow/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/arrow/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.497696 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/arrow/mapper/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/arrow/mapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/arrow/mapper/dataset_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     7260 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/arrow/mapper/media.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.497696 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/ava/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/ava/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8897 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/ava/ava.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/ava/ava_label_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/brats.py
--rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/brats_numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)    17865 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/camvid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.497696 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/celeba/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/celeba/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/celeba/align_celeba.py
--rw-r--r--   0 runner    (1001) docker     (127)    10889 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/celeba/celeba.py
--rw-r--r--   0 runner    (1001) docker     (127)    12623 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/cifar.py
--rw-r--r--   0 runner    (1001) docker     (127)    21780 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/cityscapes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.497696 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/coco/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/coco/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24813 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/coco/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    33535 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/coco/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/coco/extractor_merger.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/coco/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     6915 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/coco/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/coco/page_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/common_semantic_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/common_super_resolution.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.501696 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/cvat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/cvat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16158 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/cvat/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    21501 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/cvat/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/cvat/format.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.501696 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/datumaro/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/datumaro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18239 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/datumaro/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    19062 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/datumaro/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/datumaro/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/datumaro/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/datumaro/page_mapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.501696 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/datumaro_binary/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/datumaro_binary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7383 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/datumaro_binary/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11209 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/datumaro_binary/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/datumaro_binary/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/datumaro_binary/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.501696 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/datumaro_binary/mapper/
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11158 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     6297 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.505696 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/icdar/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/icdar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12539 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/icdar/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6522 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/icdar/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/icdar/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/image_dir.py
--rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/image_zip.py
--rw-r--r--   0 runner    (1001) docker     (127)     8073 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/imagenet.py
--rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/imagenet_txt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.505696 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/kaggle/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/kaggle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17530 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/kaggle/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6523 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/kinetics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.505696 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/kitti/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/kitti/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6210 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/kitti/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11401 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/kitti/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/kitti/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/kitti/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.505696 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/kitti_raw/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/kitti_raw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11539 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/kitti_raw/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    17906 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/kitti_raw/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/kitti_raw/format.py
--rw-r--r--   0 runner    (1001) docker     (127)    20219 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/labelme.py
--rw-r--r--   0 runner    (1001) docker     (127)    15274 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/lfw.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.505696 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mapillary_vistas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mapillary_vistas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11577 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mapillary_vistas/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    12609 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mapillary_vistas/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     4404 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mapillary_vistas/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6603 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/market1501.py
--rw-r--r--   0 runner    (1001) docker     (127)     5244 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mars.py
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mmdet.py
--rw-r--r--   0 runner    (1001) docker     (127)     9373 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mnist.py
--rw-r--r--   0 runner    (1001) docker     (127)     7597 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mnist_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)    11120 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mot.py
--rw-r--r--   0 runner    (1001) docker     (127)     6763 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mots.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.505696 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mpii/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mpii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mpii/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     5541 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mpii/mpii_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     5304 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mpii/mpii_mat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.509696 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mvtec/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mvtec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mvtec/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mvtec/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mvtec/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mvtec/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/nyu_depth_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    38893 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/open_images.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.509696 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/roboflow/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/roboflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10251 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/roboflow/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/roboflow/base_tfrecord.py
--rw-r--r--   0 runner    (1001) docker     (127)     6742 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/roboflow/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.509696 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/segment_anything/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/segment_anything/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6087 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/segment_anything/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6062 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/segment_anything/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/segment_anything/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.509696 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/sly_pointcloud/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/sly_pointcloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7215 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/sly_pointcloud/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    16317 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/sly_pointcloud/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/sly_pointcloud/format.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.509696 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/synthia/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/synthia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6671 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/synthia/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/synthia/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/synthia/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8306 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/tabular.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.509696 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/tf_detection_api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/tf_detection_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9237 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/tf_detection_api/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8855 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/tf_detection_api/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/tf_detection_api/format.py
--rw-r--r--   0 runner    (1001) docker     (127)    15800 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/vgg_face2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6585 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/video.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.513696 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/voc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/voc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16675 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/voc/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    31405 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/voc/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10734 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/voc/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/voc/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/vott_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     4242 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/vott_json.py
--rw-r--r--   0 runner    (1001) docker     (127)    10445 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/widerface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.513696 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/yolo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/yolo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14467 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/yolo/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    12211 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/yolo/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/yolo/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     7143 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/yolo/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/explorer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/framework_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.513696 datumaro-1.6.1rc3/src/datumaro/plugins/inference_server_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/inference_server_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4101 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/inference_server_plugin/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/inference_server_plugin/ovms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.513696 datumaro-1.6.1rc3/src/datumaro/plugins/inference_server_plugin/samples/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/inference_server_plugin/samples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/inference_server_plugin/samples/face_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     5356 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/inference_server_plugin/triton.py
--rw-r--r--   0 runner    (1001) docker     (127)     6370 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/missing_annotation_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)    16787 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/ndr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.513696 datumaro-1.6.1rc3/src/datumaro/plugins/openvino_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/openvino_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9864 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/openvino_plugin/launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.517696 datumaro-1.6.1rc3/src/datumaro/plugins/openvino_plugin/samples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/openvino_plugin/samples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/openvino_plugin/samples/clip_text_ViT-B_32_interp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/openvino_plugin/samples/clip_visual_ViT-B_32_interp.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/openvino_plugin/samples/coco.class
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/openvino_plugin/samples/googlenet-v4-tf_interp.py
--rw-r--r--   0 runner    (1001) docker     (127)    10475 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/openvino_plugin/samples/imagenet.class
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_atss_interp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_ssd_interp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_yolox_interp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/openvino_plugin/samples/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/openvino_plugin/shift_launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.517696 datumaro-1.6.1rc3/src/datumaro/plugins/sam_transforms/
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/sam_transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7810 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/sam_transforms/automatic_mask_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)     5760 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/sam_transforms/bbox_to_inst_mask.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.517696 datumaro-1.6.1rc3/src/datumaro/plugins/sam_transforms/interpreters/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/sam_transforms/interpreters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8109 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/sam_transforms/interpreters/sam_decoder_for_amg.py
--rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/sam_transforms/interpreters/sam_decoder_for_bbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/sam_transforms/interpreters/sam_encoder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.517696 datumaro-1.6.1rc3/src/datumaro/plugins/sampler/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/sampler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.517696 datumaro-1.6.1rc3/src/datumaro/plugins/sampler/algorithm/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/sampler/algorithm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/sampler/algorithm/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (127)     7285 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/sampler/algorithm/entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)     7814 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/sampler/random_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8901 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/sampler/relevancy_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)    51901 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/specs.json
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/specs.py
--rw-r--r--   0 runner    (1001) docker     (127)    32124 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.521696 datumaro-1.6.1rc3/src/datumaro/plugins/synthetic_data/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/synthetic_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11335 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/synthetic_data/background_colors.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11713 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/synthetic_data/image_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/synthetic_data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.521696 datumaro-1.6.1rc3/src/datumaro/plugins/tiling/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/tiling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9398 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/tiling/merge_tile.py
--rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/tiling/tile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/tiling/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    50015 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)    45116 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/plugins/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/project.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.525696 datumaro-1.6.1rc3/src/datumaro/util/
--rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8553 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/util/annotation_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/util/attrs_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/util/definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/util/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13348 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/util/image.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/util/image_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/util/import_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/util/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14465 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/util/mask_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/util/meta_file_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/util/multi_procs_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     8833 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/util/os_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/util/pickle_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/util/samples.py
--rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/util/scope.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/util/telemetry_stub.py
--rw-r--r--   0 runner    (1001) docker     (127)     6079 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/util/telemetry_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/util/tf_util.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-19 02:44:06.000000 datumaro-1.6.1rc3/src/datumaro/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:44:12.525696 datumaro-1.6.1rc3/src/datumaro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7790 2024-04-19 02:44:12.000000 datumaro-1.6.1rc3/src/datumaro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15527 2024-04-19 02:44:12.000000 datumaro-1.6.1rc3/src/datumaro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 02:44:12.000000 datumaro-1.6.1rc3/src/datumaro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-19 02:44:12.000000 datumaro-1.6.1rc3/src/datumaro.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 02:44:12.000000 datumaro-1.6.1rc3/src/datumaro.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-19 02:44:12.000000 datumaro-1.6.1rc3/src/datumaro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-19 02:44:12.000000 datumaro-1.6.1rc3/src/datumaro.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:20.098753 datumaro-1.7.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)   393113 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/3rd-party.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     7718 2024-06-03 01:44:20.098753 datumaro-1.7.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/requirements-core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/requirements-default.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:20.042753 datumaro-1.7.0rc1/rust/
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/rust/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:20.042753 datumaro-1.7.0rc1/rust/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     6711 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/rust/src/coco_page_mapper.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     6592 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/rust/src/datum_page_mapper.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     6110 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/rust/src/json_section_page_mapper.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/rust/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/rust/src/page_mapper.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     8637 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/rust/src/page_maps.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/rust/src/utils.rs
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 01:44:20.098753 datumaro-1.7.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:20.034752 datumaro-1.7.0rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:20.042753 datumaro-1.7.0rc1/src/datumaro/
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:20.046753 datumaro-1.7.0rc1/src/datumaro/capi/
+-rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/capi/pybind.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:20.046753 datumaro-1.7.0rc1/src/datumaro/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/cli/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:20.046753 datumaro-1.7.0rc1/src/datumaro/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8966 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/cli/commands/compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/cli/commands/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/cli/commands/detect_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/cli/commands/download.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:20.050752 datumaro-1.7.0rc1/src/datumaro/cli/commands/downloaders/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/cli/commands/downloaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/cli/commands/downloaders/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4477 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/cli/commands/downloaders/kaggle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37518 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/cli/commands/downloaders/kaggle_formats.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7497 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/cli/commands/downloaders/tfds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9176 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/cli/commands/explain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6841 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/cli/commands/explore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9046 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/cli/commands/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/cli/commands/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/cli/commands/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10289 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/cli/commands/merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5990 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/cli/commands/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/cli/commands/prune.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:20.050752 datumaro-1.7.0rc1/src/datumaro/cli/commands/require_project/
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/cli/commands/require_project/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:20.050752 datumaro-1.7.0rc1/src/datumaro/cli/commands/require_project/modification/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/cli/commands/require_project/modification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/cli/commands/require_project/modification/add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/cli/commands/require_project/modification/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5924 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/cli/commands/require_project/modification/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5912 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/cli/commands/require_project/modification/import_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/cli/commands/require_project/modification/remove.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:20.050752 datumaro-1.7.0rc1/src/datumaro/cli/commands/require_project/versioning/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/cli/commands/require_project/versioning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/cli/commands/require_project/versioning/checkout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/cli/commands/require_project/versioning/commit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/cli/commands/require_project/versioning/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/cli/commands/require_project/versioning/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/cli/commands/require_project/versioning/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/cli/commands/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8383 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/cli/commands/transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/cli/commands/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:20.050752 datumaro-1.7.0rc1/src/datumaro/cli/contexts/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/cli/contexts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9089 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/cli/contexts/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:20.050752 datumaro-1.7.0rc1/src/datumaro/cli/contexts/project/
+-rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/cli/contexts/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/cli/contexts/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/cli/contexts/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:20.050752 datumaro-1.7.0rc1/src/datumaro/cli/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/cli/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13053 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/cli/util/compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/cli/util/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5640 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/cli/util/project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:20.058753 datumaro-1.7.0rc1/src/datumaro/components/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:20.058753 datumaro-1.7.0rc1/src/datumaro/components/abstracts/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/components/abstracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/components/abstracts/merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/components/abstracts/model_interpreter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:20.058753 datumaro-1.7.0rc1/src/datumaro/components/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/components/algorithms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:20.058753 datumaro-1.7.0rc1/src/datumaro/components/algorithms/hash_key_inference/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/components/algorithms/hash_key_inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/components/algorithms/hash_key_inference/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5629 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/components/algorithms/hash_key_inference/explorer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/components/algorithms/hash_key_inference/hashkey_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13605 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/components/algorithms/hash_key_inference/prune.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:20.058753 datumaro-1.7.0rc1/src/datumaro/components/algorithms/noisy_label_detection/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/components/algorithms/noisy_label_detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8957 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4706 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/components/algorithms/rise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44839 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/components/annotation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:20.058753 datumaro-1.7.0rc1/src/datumaro/components/annotations/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/components/annotations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11772 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/components/annotations/matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5599 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/components/annotations/merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/components/cli_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25400 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/components/comparator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/components/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/components/config_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:20.058753 datumaro-1.7.0rc1/src/datumaro/components/contexts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/components/contexts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/components/contexts/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/components/crypter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34649 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/components/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8191 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/components/dataset_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6806 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/components/dataset_item_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27680 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/components/dataset_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9843 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/components/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18494 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/components/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15262 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/components/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20345 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/components/extractor_tfds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14541 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/components/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19999 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/components/format_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/components/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:20.058753 datumaro-1.7.0rc1/src/datumaro/components/hl_ops/
+-rw-r--r--   0 runner    (1001) docker     (127)    15576 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/components/hl_ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8271 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/components/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6878 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/components/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/components/lazy_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45044 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/components/media.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:20.062753 datumaro-1.7.0rc1/src/datumaro/components/merge/
+-rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/components/merge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/components/merge/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12380 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/components/merge/exact_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/components/merge/extractor_merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24656 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/components/merge/intersect_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/components/merge/union_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14387 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/components/operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/components/progress_reporting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89717 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/components/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/components/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9666 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/components/shift_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6542 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/components/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/components/validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23697 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/components/visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:20.062753 datumaro-1.7.0rc1/src/datumaro/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:20.062753 datumaro-1.7.0rc1/src/datumaro/plugins/accuracy_checker_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/accuracy_checker_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:20.062753 datumaro-1.7.0rc1/src/datumaro/plugins/accuracy_checker_plugin/details/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/accuracy_checker_plugin/details/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4508 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/accuracy_checker_plugin/details/ac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/accuracy_checker_plugin/details/representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15491 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/anchor_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37755 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/configurable_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:20.070753 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/ade20k2017.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8995 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/ade20k2020.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:20.070753 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/arrow/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/arrow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5858 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/arrow/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9866 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/arrow/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/arrow/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/arrow/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:20.070753 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/arrow/mapper/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/arrow/mapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/arrow/mapper/dataset_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7260 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/arrow/mapper/media.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:20.070753 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/ava/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/ava/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8954 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/ava/ava.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/ava/ava_label_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/brats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/brats_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18019 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/camvid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:20.070753 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/celeba/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/celeba/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7948 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/celeba/align_celeba.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11075 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/celeba/celeba.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12680 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/cifar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21856 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/cityscapes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:20.074753 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/coco/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/coco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24993 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/coco/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33535 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/coco/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/coco/extractor_merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/coco/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7068 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/coco/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/coco/page_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6871 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/common_semantic_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/common_super_resolution.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:20.074753 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/cvat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/cvat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16259 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/cvat/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21501 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/cvat/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/cvat/format.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:20.074753 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/datumaro/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/datumaro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20272 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/datumaro/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20224 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/datumaro/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/datumaro/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/datumaro/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/datumaro/page_mapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:20.074753 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7710 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11209 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:20.078753 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11158 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7622 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8894 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/dota.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:20.078753 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/icdar/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/icdar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12866 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/icdar/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6522 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/icdar/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/icdar/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/image_dir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/image_zip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8370 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/imagenet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8578 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/imagenet_txt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:20.078753 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/kaggle/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/kaggle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18921 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/kaggle/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6574 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/kinetics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:20.078753 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/kitti/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/kitti/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6478 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/kitti/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11401 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/kitti/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/kitti/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/kitti/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:20.078753 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/kitti_raw/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/kitti_raw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11638 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/kitti_raw/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17906 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/kitti_raw/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/kitti_raw/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20302 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/labelme.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15349 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/lfw.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:20.078753 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/mapillary_vistas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/mapillary_vistas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10901 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/mapillary_vistas/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12609 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/mapillary_vistas/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4404 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/mapillary_vistas/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6603 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/market1501.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/mars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/mmdet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9432 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/mnist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7656 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/mnist_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11177 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/mot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6878 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/mots.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:20.082753 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/mpii/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/mpii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/mpii/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5624 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/mpii/mpii_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/mpii/mpii_mat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:20.082753 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/mvtec/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/mvtec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/mvtec/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/mvtec/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/mvtec/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/mvtec/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/nyu_depth_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39077 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/open_images.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:20.082753 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/roboflow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/roboflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10405 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/roboflow/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/roboflow/base_tfrecord.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7363 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/roboflow/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:20.082753 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/segment_anything/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/segment_anything/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6192 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/segment_anything/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6062 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/segment_anything/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/segment_anything/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:20.082753 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/sly_pointcloud/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/sly_pointcloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7316 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/sly_pointcloud/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16317 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/sly_pointcloud/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/sly_pointcloud/format.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:20.082753 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/synthia/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/synthia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6756 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/synthia/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/synthia/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/synthia/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9739 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/tabular.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:20.086753 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/tf_detection_api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/tf_detection_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9320 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/tf_detection_api/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8855 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/tf_detection_api/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/tf_detection_api/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15986 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/vgg_face2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6617 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/video.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:20.086753 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/voc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/voc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16912 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/voc/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31405 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/voc/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10734 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/voc/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/voc/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/vott_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/vott_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10587 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/widerface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:20.086753 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/yolo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/yolo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14647 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/yolo/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12211 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/yolo/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/yolo/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7143 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/yolo/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/explorer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/framework_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:20.086753 datumaro-1.7.0rc1/src/datumaro/plugins/inference_server_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/inference_server_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4101 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/inference_server_plugin/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/inference_server_plugin/ovms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:20.086753 datumaro-1.7.0rc1/src/datumaro/plugins/inference_server_plugin/samples/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/inference_server_plugin/samples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/inference_server_plugin/samples/face_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5356 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/inference_server_plugin/triton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6370 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/missing_annotation_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16787 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/ndr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:20.086753 datumaro-1.7.0rc1/src/datumaro/plugins/openvino_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/openvino_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9864 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/openvino_plugin/launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:20.090753 datumaro-1.7.0rc1/src/datumaro/plugins/openvino_plugin/samples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/openvino_plugin/samples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/openvino_plugin/samples/clip_text_ViT-B_32_interp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/openvino_plugin/samples/clip_visual_ViT-B_32_interp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/openvino_plugin/samples/coco.class
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/openvino_plugin/samples/googlenet-v4-tf_interp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10475 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/openvino_plugin/samples/imagenet.class
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_atss_interp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_ssd_interp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_yolox_interp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/openvino_plugin/samples/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/openvino_plugin/shift_launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:20.090753 datumaro-1.7.0rc1/src/datumaro/plugins/sam_transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/sam_transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7810 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/sam_transforms/automatic_mask_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5760 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/sam_transforms/bbox_to_inst_mask.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:20.090753 datumaro-1.7.0rc1/src/datumaro/plugins/sam_transforms/interpreters/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/sam_transforms/interpreters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8109 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/sam_transforms/interpreters/sam_decoder_for_amg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/sam_transforms/interpreters/sam_decoder_for_bbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/sam_transforms/interpreters/sam_encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:20.090753 datumaro-1.7.0rc1/src/datumaro/plugins/sampler/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/sampler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:20.090753 datumaro-1.7.0rc1/src/datumaro/plugins/sampler/algorithm/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/sampler/algorithm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/sampler/algorithm/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7285 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/sampler/algorithm/entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7814 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/sampler/random_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8901 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/sampler/relevancy_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52532 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/specs.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/specs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32124 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:20.090753 datumaro-1.7.0rc1/src/datumaro/plugins/synthetic_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/synthetic_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11335 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/synthetic_data/background_colors.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11713 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/synthetic_data/image_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/synthetic_data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:20.094753 datumaro-1.7.0rc1/src/datumaro/plugins/tiling/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/tiling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9398 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/tiling/merge_tile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/tiling/tile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/tiling/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53369 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45116 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/plugins/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:20.094753 datumaro-1.7.0rc1/src/datumaro/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8553 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/util/annotation_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/util/attrs_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/util/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/util/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13444 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/util/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/util/image_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/util/import_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/util/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14465 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/util/mask_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/util/meta_file_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/util/multi_procs_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8833 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/util/os_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/util/pickle_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/util/samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/util/scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/util/telemetry_stub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6079 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/util/telemetry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/util/tf_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-06-03 01:44:15.000000 datumaro-1.7.0rc1/src/datumaro/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:44:20.094753 datumaro-1.7.0rc1/src/datumaro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7718 2024-06-03 01:44:20.000000 datumaro-1.7.0rc1/src/datumaro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15823 2024-06-03 01:44:20.000000 datumaro-1.7.0rc1/src/datumaro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 01:44:20.000000 datumaro-1.7.0rc1/src/datumaro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-06-03 01:44:20.000000 datumaro-1.7.0rc1/src/datumaro.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 01:44:19.000000 datumaro-1.7.0rc1/src/datumaro.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-06-03 01:44:20.000000 datumaro-1.7.0rc1/src/datumaro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-06-03 01:44:20.000000 datumaro-1.7.0rc1/src/datumaro.egg-info/top_level.txt
```

### Comparing `datumaro-1.6.1rc3/3rd-party.txt` & `datumaro-1.7.0rc1/3rd-party.txt`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/LICENSE` & `datumaro-1.7.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/PKG-INFO` & `datumaro-1.7.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datumaro
-Version: 1.6.1rc3
+Version: 1.7.0rc1
 Summary: Dataset Management Framework (Datumaro)
 Home-page: https://github.com/openvinotoolkit/datumaro
 Author: Intel
 Author-email: emily.chun@intel.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,27 +17,27 @@
 Requires-Dist: h5py>=2.10.0
 Requires-Dist: imagesize>=1.4.1
 Requires-Dist: lxml<6,>=5.2.0
 Requires-Dist: matplotlib>=3.3.1
 Requires-Dist: networkx>=2.6
 Requires-Dist: nibabel>=3.2.1
 Requires-Dist: numpy<2,>=1.23.4
-Requires-Dist: orjson==3.10.0
-Requires-Dist: Pillow>=10.2.0
+Requires-Dist: orjson==3.10.3
+Requires-Dist: Pillow>=10.3.0
 Requires-Dist: ruamel.yaml>=0.17.0
 Requires-Dist: shapely>=1.7
 Requires-Dist: typing_extensions>=3.7.4.3
 Requires-Dist: tqdm
 Requires-Dist: pycocotools>=2.0.4; platform_system != "Windows" or python_version >= "3.9"
 Requires-Dist: pycocotools-windows; platform_system == "Windows" and python_version < "3.9"
 Requires-Dist: PyYAML==6.0.1
 Requires-Dist: tensorboardX!=2.3,>=1.8
 Requires-Dist: scipy
 Requires-Dist: requests
-Requires-Dist: pandas~=1.4.0
+Requires-Dist: pandas>=1.4.0
 Requires-Dist: openvino>=2023.2.0
 Requires-Dist: tokenizers
 Requires-Dist: cryptography>=38.03
 Requires-Dist: pyemd
 Requires-Dist: pyarrow
 Requires-Dist: protobuf
 Requires-Dist: tabulate
@@ -46,16 +46,14 @@
 Requires-Dist: scikit-learn
 Requires-Dist: json-stream
 Requires-Dist: opencv-python
 Provides-Extra: tf
 Requires-Dist: tensorflow; extra == "tf"
 Provides-Extra: tfds
 Requires-Dist: tensorflow-datasets<4.9.3; extra == "tfds"
-Provides-Extra: tf-gpu
-Requires-Dist: tensorflow-gpu; extra == "tf-gpu"
 Provides-Extra: torch
 Requires-Dist: torch; extra == "torch"
 Requires-Dist: torchvision; extra == "torch"
 Provides-Extra: default
 Requires-Dist: dvc==3.49.0; extra == "default"
 Requires-Dist: fsspec<=2022.11.0; python_version < "3.8" and extra == "default"
 Requires-Dist: GitPython!=3.1.25,>=3.1.18; extra == "default"
```

### Comparing `datumaro-1.6.1rc3/README.md` & `datumaro-1.7.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/pyproject.toml` & `datumaro-1.7.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/requirements-core.txt` & `datumaro-1.7.0rc1/requirements-core.txt`

 * *Files 11% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 h5py>=2.10.0
 imagesize>=1.4.1
 lxml<6,>=5.2.0
 matplotlib>=3.3.1
 networkx>=2.6
 nibabel>=3.2.1
 numpy<2,>=1.23.4
-orjson==3.10.0
-Pillow>=10.2.0
+orjson==3.10.3
+Pillow>=10.3.0
 ruamel.yaml>=0.17.0
 shapely>=1.7
 typing_extensions>=3.7.4.3
 tqdm
 
 pycocotools>=2.0.4; platform_system != "Windows" or python_version >= '3.9'
 
@@ -27,15 +27,15 @@
 # NDR
 scipy
 
 # Image generator
 requests
 
 # Sampler
-pandas~=1.4.0
+pandas>=1.4.0
 
 # OpenVINO
 openvino>=2023.2.0
 tokenizers
 
 # Encryption
 cryptography>= 38.03
```

### Comparing `datumaro-1.6.1rc3/rust/src/coco_page_mapper.rs` & `datumaro-1.7.0rc1/rust/src/coco_page_mapper.rs`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/rust/src/datum_page_mapper.rs` & `datumaro-1.7.0rc1/rust/src/datum_page_mapper.rs`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/rust/src/json_section_page_mapper.rs` & `datumaro-1.7.0rc1/rust/src/json_section_page_mapper.rs`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/rust/src/lib.rs` & `datumaro-1.7.0rc1/rust/src/lib.rs`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/rust/src/page_mapper.rs` & `datumaro-1.7.0rc1/rust/src/page_mapper.rs`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/rust/src/page_maps.rs` & `datumaro-1.7.0rc1/rust/src/page_maps.rs`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/rust/src/utils.rs` & `datumaro-1.7.0rc1/rust/src/utils.rs`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/setup.py` & `datumaro-1.7.0rc1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,14 @@
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.9",
     install_requires=CORE_REQUIREMENTS,
     extras_require={
         "tf": ["tensorflow"],
         "tfds": ["tensorflow-datasets<4.9.3"],
-        "tf-gpu": ["tensorflow-gpu"],
         "torch": ["torch", "torchvision"],
         "default": DEFAULT_REQUIREMENTS,
     },
     ext_modules=ext_modules,
     entry_points={
         "console_scripts": [
             "datum=datumaro.cli.__main__:main",
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/__init__.py` & `datumaro-1.7.0rc1/src/datumaro/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     PointsCategories,
     Polygon,
     PolyLine,
     RgbColor,
     RleMask,
 )
 from .components.cli_plugin import CliPlugin
-from .components.dataset import Dataset, DatasetPatch, DatasetSubset, eager_mode
+from .components.dataset import Dataset, DatasetPatch, DatasetSubset, StreamDataset, eager_mode
 from .components.dataset_base import (
     DEFAULT_SUBSET_NAME,
     CategoriesInfo,
     DatasetBase,
     DatasetItem,
     IDataset,
     SubsetBase,
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/capi/pybind.cpp` & `datumaro-1.7.0rc1/src/datumaro/capi/pybind.cpp`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/cli/__main__.py` & `datumaro-1.7.0rc1/src/datumaro/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/cli/commands/__init__.py` & `datumaro-1.7.0rc1/src/datumaro/cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/cli/commands/compare.py` & `datumaro-1.7.0rc1/src/datumaro/cli/commands/compare.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/cli/commands/convert.py` & `datumaro-1.7.0rc1/src/datumaro/cli/commands/convert.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/cli/commands/detect_format.py` & `datumaro-1.7.0rc1/src/datumaro/cli/commands/detect_format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/cli/commands/explain.py` & `datumaro-1.7.0rc1/src/datumaro/cli/commands/explain.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/cli/commands/explore.py` & `datumaro-1.7.0rc1/src/datumaro/cli/commands/explore.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/cli/commands/filter.py` & `datumaro-1.7.0rc1/src/datumaro/cli/commands/filter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/cli/commands/generate.py` & `datumaro-1.7.0rc1/src/datumaro/cli/commands/generate.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/cli/commands/info.py` & `datumaro-1.7.0rc1/src/datumaro/cli/commands/info.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/cli/commands/merge.py` & `datumaro-1.7.0rc1/src/datumaro/cli/commands/merge.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/cli/commands/patch.py` & `datumaro-1.7.0rc1/src/datumaro/cli/commands/patch.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/cli/commands/prune.py` & `datumaro-1.7.0rc1/src/datumaro/cli/commands/prune.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/cli/commands/require_project/__init__.py` & `datumaro-1.7.0rc1/src/datumaro/cli/commands/require_project/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/cli/commands/require_project/modification/add.py` & `datumaro-1.7.0rc1/src/datumaro/cli/commands/require_project/modification/add.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/cli/commands/require_project/modification/create.py` & `datumaro-1.7.0rc1/src/datumaro/cli/commands/require_project/modification/create.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/cli/commands/require_project/modification/export.py` & `datumaro-1.7.0rc1/src/datumaro/cli/commands/require_project/modification/export.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/cli/commands/require_project/modification/import_.py` & `datumaro-1.7.0rc1/src/datumaro/cli/commands/require_project/modification/import_.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/cli/commands/require_project/modification/remove.py` & `datumaro-1.7.0rc1/src/datumaro/cli/commands/require_project/modification/remove.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/cli/commands/require_project/versioning/checkout.py` & `datumaro-1.7.0rc1/src/datumaro/cli/commands/require_project/versioning/checkout.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/cli/commands/require_project/versioning/commit.py` & `datumaro-1.7.0rc1/src/datumaro/cli/commands/require_project/versioning/commit.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/cli/commands/require_project/versioning/info.py` & `datumaro-1.7.0rc1/src/datumaro/cli/commands/require_project/versioning/info.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/cli/commands/require_project/versioning/log.py` & `datumaro-1.7.0rc1/src/datumaro/cli/commands/require_project/versioning/log.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/cli/commands/require_project/versioning/status.py` & `datumaro-1.7.0rc1/src/datumaro/cli/commands/require_project/versioning/status.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/cli/commands/stats.py` & `datumaro-1.7.0rc1/src/datumaro/cli/commands/stats.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/cli/commands/transform.py` & `datumaro-1.7.0rc1/src/datumaro/cli/commands/transform.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/cli/commands/validate.py` & `datumaro-1.7.0rc1/src/datumaro/cli/commands/validate.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/cli/contexts/model.py` & `datumaro-1.7.0rc1/src/datumaro/cli/contexts/model.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/cli/contexts/project/__init__.py` & `datumaro-1.7.0rc1/src/datumaro/cli/contexts/project/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/cli/contexts/source.py` & `datumaro-1.7.0rc1/src/datumaro/cli/contexts/source.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/cli/contexts/util.py` & `datumaro-1.7.0rc1/src/datumaro/cli/contexts/util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/cli/util/__init__.py` & `datumaro-1.7.0rc1/src/datumaro/cli/util/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/cli/util/compare.py` & `datumaro-1.7.0rc1/src/datumaro/cli/util/compare.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/cli/util/project.py` & `datumaro-1.7.0rc1/src/datumaro/cli/util/project.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/components/abstracts/merger.py` & `datumaro-1.7.0rc1/src/datumaro/components/abstracts/merger.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/components/abstracts/model_interpreter.py` & `datumaro-1.7.0rc1/src/datumaro/components/abstracts/model_interpreter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/components/algorithms/hash_key_inference/base.py` & `datumaro-1.7.0rc1/src/datumaro/components/algorithms/hash_key_inference/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/components/algorithms/hash_key_inference/explorer.py` & `datumaro-1.7.0rc1/src/datumaro/components/algorithms/hash_key_inference/explorer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/components/algorithms/hash_key_inference/hashkey_util.py` & `datumaro-1.7.0rc1/src/datumaro/components/algorithms/hash_key_inference/hashkey_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,15 +156,15 @@
     "kitti": kitti_templates,
     "kinetics": kinetics_templates,
     "mnist": mnist_templates,
 }
 
 
 def select_uninferenced_dataset(dataset):
-    uninferenced_dataset = Dataset(media_type=MediaElement)
+    uninferenced_dataset = Dataset(media_type=MediaElement, ann_types=set())
     for item in dataset:
         if not any(isinstance(annotation, HashKey) for annotation in item.annotations):
             uninferenced_dataset.put(item)
     return uninferenced_dataset
 
 
 def calculate_hamming(B1, B2):
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/components/algorithms/hash_key_inference/prune.py` & `datumaro-1.7.0rc1/src/datumaro/components/algorithms/hash_key_inference/prune.py`

 * *Files 0% similar despite different names*

```diff
@@ -339,15 +339,17 @@
             num_centers=self._num_centers,
             labels=self._labels,
             database_keys=self._database_keys,
             item_list=self._item_list,
             source=self._dataset,
         )
 
-        result_dataset = Dataset(media_type=self._dataset.media_type())
+        result_dataset = Dataset(
+            media_type=self._dataset.media_type(), ann_types=self._dataset.ann_types()
+        )
         result_dataset._source_path = self._dataset._source_path
         result_dataset.define_categories(self._dataset.categories())
         for item in selected_items:
             result_dataset.put(item)
 
         if dist_tuples:
             for center, id_, subset_, d in dist_tuples:
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py` & `datumaro-1.7.0rc1/src/datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/components/algorithms/rise.py` & `datumaro-1.7.0rc1/src/datumaro/components/algorithms/rise.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/components/annotation.py` & `datumaro-1.7.0rc1/src/datumaro/components/annotation.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Copyright (C) 2021-2024 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
+import math
 from enum import IntEnum
 from functools import partial
 from itertools import zip_longest
 from typing import (
     Any,
     Callable,
     Dict,
@@ -44,14 +45,15 @@
     cuboid_3d = 8
     super_resolution_annotation = 9
     depth_annotation = 10
     ellipse = 11
     hash_key = 12
     feature_vector = 13
     tabular = 14
+    rotated_bbox = 15
 
 
 COORDINATE_ROUNDING_DIGITS = 2
 CHECK_POLYGON_EQ_EPSILONE = 1e-7
 NO_GROUP = 0
 NO_OBJECT_ID = -1
 
@@ -339,25 +341,27 @@
             other_color = other.colormap.get(label_id)
             if not np.array_equal(my_color, other_color):
                 return False
         return True
 
 
 BinaryMaskImage = np.ndarray  # 2d array of type bool
+BinaryMaskImageCallable = Callable[[], BinaryMaskImage]
 IndexMaskImage = np.ndarray  # 2d array of type int
+IndexMaskImageCallable = Callable[[], IndexMaskImage]
 
 
 @attrs(slots=True, eq=False, order=False)
 class Mask(Annotation):
     """
     Represents a 2d single-instance binary segmentation mask.
     """
 
     _type = AnnotationType.mask
-    _image = field()
+    _image: Union[BinaryMaskImage, BinaryMaskImageCallable] = field()
     label: Optional[int] = field(
         converter=attr.converters.optional(int), default=None, kw_only=True
     )
     z_order: int = field(default=0, validator=default_if_none(int), kw_only=True)
 
     def __attrs_post_init__(self):
         if isinstance(self._image, np.ndarray):
@@ -495,14 +499,53 @@
 
     def __eq__(self, other):
         if not isinstance(other, __class__):
             return super().__eq__(other)
         return self.rle == other.rle
 
 
+@attrs(slots=True, eq=False, order=False)
+class ExtractedMask(Mask):
+    """Mask annotation (binary mask) extracted from an index mask (integer 2D Numpy array).
+
+    This class can extract a binary mask with given index mask and index value.
+    The advantage of this class is that we can create multiple binary mask but they share a single index mask source.
+
+    Attributes:
+        index_mask: Integer 2D Numpy array. Its pixel can indicate a label id (class) or an instance id.
+        index: Integer value to extract a binary mask from the given index mask.
+
+    Examples:
+        This example demonstrates how to create an `ExtractedMask` from a synthetic index mask,
+        which denotes a semantic segmentation mask with binary values such as 0 for background
+        and 1 for foreground.
+
+        >>> import numpy as np
+        >>> from datumaro.components.annotation import ExtractedMask
+        >>>
+        >>> index_mask = np.random.randint(low=0, high=2, size=(10, 10), dtype=np.uint8)
+        >>> mask1 = ExtractedMask(index_mask=index_mask, index=0, label=0)  # 0 for background
+        >>> mask2 = ExtractedMask(index_mask=index_mask, index=1, label=1)  # 1 for foreground
+        >>> np.unique(mask1.image).tolist()  # `image` property create a binary mask
+        np.array([0, 1])
+        >>> mask1.index_mask == mask2.index_mask  # They share the same source
+        True
+    """
+
+    index_mask: Union[IndexMaskImage, IndexMaskImageCallable] = field()
+    index: int = field()
+
+    _image: None = field(init=False, default=None)
+
+    @property
+    def image(self) -> BinaryMaskImage:
+        index_mask = self.index_mask() if callable(self.index_mask) else self.index_mask
+        return index_mask == self.index
+
+
 CompiledMaskImage = np.ndarray  # 2d of integers (of different precision)
 
 
 class CompiledMask:
     """
     Represents class- and instance- segmentation masks with
     all the instances (opposed to single-instance masks).
@@ -636,19 +679,16 @@
 
     def lazy_extract(self, instance_id: int) -> Callable[[], IndexMaskImage]:
         return partial(self.extract, instance_id)
 
 
 @attrs(slots=True, order=False)
 class _Shape(Annotation):
-    # Flattened list of point coordinates
     points: List[float] = field(
-        converter=lambda x: np.around(
-            np.array(x, dtype=np.float32), COORDINATE_ROUNDING_DIGITS
-        ).tolist()
+        converter=lambda x: np.array(x, dtype=np.float32).round(COORDINATE_ROUNDING_DIGITS).tolist()
     )
 
     label: Optional[int] = field(
         converter=attr.converters.optional(int), default=None, kw_only=True
     )
 
     z_order: int = field(default=0, validator=default_if_none(int), kw_only=True)
@@ -765,19 +805,20 @@
     def __attrs_post_init__(self):
         # keep the message on a single line to produce informative output
         assert len(self.points) % 2 == 0 and 3 <= len(self.points) // 2, (
             "Wrong polygon points: %s" % self.points
         )
 
     def get_area(self):
-        import pycocotools.mask as mask_utils
+        # import pycocotools.mask as mask_utils
 
-        x, y, w, h = self.get_bbox()
-        rle = mask_utils.frPyObjects([self.points], y + h, x + w)
-        area = mask_utils.area(rle)[0]
+        # x, y, w, h = self.get_bbox()
+        # rle = mask_utils.frPyObjects([self.points], y + h, x + w)
+        # area = mask_utils.area(rle)[0]
+        area = self._get_shoelace_area()
         return area
 
     def as_polygon(self) -> List[float]:
         return self.points
 
     def __eq__(self, other):
         if not isinstance(other, __class__):
@@ -795,14 +836,29 @@
         other_polygon = sg.Polygon(other_points)
         # if polygon is not valid, compare points
         if not (self_polygon.is_valid and other_polygon.is_valid):
             return self_points == other_points
         inter_area = self_polygon.intersection(other_polygon).area
         return abs(self_polygon.area - inter_area) < CHECK_POLYGON_EQ_EPSILONE
 
+    def _get_shoelace_area(self):
+        points = self.get_points()
+        n = len(points)
+        # Not a polygon
+        if n < 3:
+            return 0
+
+        area = 0.0
+        for i in range(n):
+            x1, y1 = points[i]
+            x2, y2 = points[(i + 1) % n]  # Next vertex, wrapping around using modulo
+            area += x1 * y2 - y1 * x2
+
+        return abs(area) / 2.0
+
 
 @attrs(slots=True, init=False, order=False)
 class Bbox(_Shape):
     _type = AnnotationType.bbox
 
     def __init__(self, x, y, w, h, *args, **kwargs):
         kwargs.pop("points", None)  # comes from wrap()
@@ -841,14 +897,109 @@
 
     def wrap(item, **kwargs):
         d = {"x": item.x, "y": item.y, "w": item.w, "h": item.h}
         d.update(kwargs)
         return attr.evolve(item, **d)
 
 
+@attrs(slots=True, init=False, order=False)
+class RotatedBbox(_Shape):
+    _type = AnnotationType.rotated_bbox
+
+    def __init__(self, cx, cy, w, h, r, *args, **kwargs):
+        kwargs.pop("points", None)  # comes from wrap()
+        self.__attrs_init__([cx, cy, w, h, r], *args, **kwargs)
+
+    @classmethod
+    def from_rectangle(cls, points: List[Tuple[float, float]], *args, **kwargs):
+        assert len(points) == 4, "polygon for a rotated bbox should have only 4 coordinates."
+
+        # Calculate rotation angle
+        rot = math.atan2(points[1][1] - points[0][1], points[1][0] - points[0][0])
+
+        # Calculate the center of the bounding box
+        cx = (points[0][0] + points[2][0]) / 2
+        cy = (points[0][1] + points[2][1]) / 2
+
+        # Calculate the width and height
+        width = math.sqrt((points[1][0] - points[0][0]) ** 2 + (points[1][1] - points[0][1]) ** 2)
+        height = math.sqrt((points[2][0] - points[1][0]) ** 2 + (points[2][1] - points[1][1]) ** 2)
+
+        return cls(cx=cx, cy=cy, w=width, h=height, r=math.degrees(rot), *args, **kwargs)
+
+    @property
+    def cx(self):
+        return self.points[0]
+
+    @property
+    def cy(self):
+        return self.points[1]
+
+    @property
+    def w(self):
+        return self.points[2]
+
+    @property
+    def h(self):
+        return self.points[3]
+
+    @property
+    def r(self):
+        return self.points[4]
+
+    def get_area(self):
+        return self.w * self.h
+
+    def get_bbox(self):
+        polygon = self.as_polygon()
+        xs = [pt[0] for pt in polygon]
+        ys = [pt[1] for pt in polygon]
+
+        return [min(xs), min(ys), max(xs) - min(xs), max(ys) - min(ys)]
+
+    def get_rotated_bbox(self):
+        return [self.cx, self.cy, self.w, self.h, self.r]
+
+    def as_polygon(self) -> List[Tuple[float, float]]:
+        """Convert [center_x, center_y, width, height, rotation] to 4 coordinates for a rotated bounding box."""
+
+        def _rotate_point(x, y, angle):
+            """Rotate a point around another point."""
+            angle_rad = math.radians(angle)
+            cos_theta = math.cos(angle_rad)
+            sin_theta = math.sin(angle_rad)
+            nx = cos_theta * x - sin_theta * y
+            ny = sin_theta * x + cos_theta * y
+            return nx, ny
+
+        # Calculate corner points of the rectangle
+        corners = [
+            (-self.w / 2, -self.h / 2),
+            (self.w / 2, -self.h / 2),
+            (self.w / 2, self.h / 2),
+            (-self.w / 2, self.h / 2),
+        ]
+
+        # Rotate each corner point
+        rotated_corners = [_rotate_point(p[0], p[1], self.r) for p in corners]
+
+        # Translate the rotated points to the original position
+        return [(p[0] + self.cx, p[1] + self.cy) for p in rotated_corners]
+
+    def iou(self, other: _Shape) -> Union[float, Literal[-1]]:
+        from datumaro.util.annotation_util import bbox_iou
+
+        return bbox_iou(self.get_bbox(), other.get_bbox())
+
+    def wrap(item, **kwargs):
+        d = {"x": item.x, "y": item.y, "w": item.w, "h": item.h, "r": item.r}
+        d.update(kwargs)
+        return attr.evolve(item, **d)
+
+
 @attrs(slots=True, order=False)
 class PointsCategories(Categories):
     """
     Describes (key-)point metainfo such as point names and joints.
     """
 
     @attrs(slots=True, order=False)
@@ -1226,7 +1377,73 @@
 class Tabular(Annotation):
     """
     Represents values of target columns in a tabular dataset.
     """
 
     _type = AnnotationType.tabular
     values: Dict[str, TableDtype] = field(converter=dict)
+
+
+class Annotations(List[Annotation]):
+    """List of `Annotation` equipped with additional utility functions."""
+
+    def get_semantic_seg_mask(
+        self, ignore_index: int = 0, dtype: np.dtype = np.uint8
+    ) -> np.ndarray:
+        """Extract semantic segmentation mask from a collection of Datumaro `Mask`s.
+
+        Args:
+            ignore_index: Scalar value to fill in the zeros in each binary mask
+                before merging into a semantic segmentation mask. This value is usually used
+                to represent a pixel denoting a not-interested region. Defaults to 0.
+            dtype: Data type for the resulting mask. Defaults to np.uint8.
+
+        Returns:
+            Semantic segmentation mask generated by merging Datumaro `Mask`s.
+
+        Raises:
+            ValueError: If there are no mask annotations or if there is an inconsistency in mask sizes.
+        """
+
+        masks = [ann for ann in self if isinstance(ann, Mask)]
+        # Mask with a lower z_order value will come first
+        masks.sort(key=lambda mask: mask.z_order)
+
+        if not masks:
+            msg = "There is no mask annotations."
+            raise ValueError(msg)
+
+        # Dispatching for better performance
+        # If all masks are `ExtractedMask`, share a same source `index_mask`, and
+        # there is no label remapping.
+        if (
+            all(isinstance(mask, ExtractedMask) for mask in masks)
+            # and set(id(mask.index_mask) for mask in masks) == 1
+            and all(mask.index_mask == next(iter(masks)).index_mask for mask in masks)
+            and all(mask.index == mask.label for mask in masks)
+        ):
+            index_mask = next(iter(masks)).index_mask
+            semantic_seg_mask: np.ndarray = index_mask() if callable(index_mask) else index_mask
+            if semantic_seg_mask.dtype != dtype:
+                semantic_seg_mask = semantic_seg_mask.astype(dtype)
+
+            labels = np.unique(np.array([mask.label for mask in masks]))
+            ignore_index_mask = np.isin(semantic_seg_mask, labels, invert=True)
+
+            return np.where(ignore_index_mask, ignore_index, semantic_seg_mask)
+
+        class_masks = [mask.as_class_mask(ignore_index=ignore_index, dtype=dtype) for mask in masks]
+
+        max_h = max([mask.shape[0] for mask in class_masks])
+        max_w = max([mask.shape[1] for mask in class_masks])
+
+        semantic_seg_mask = np.full(shape=(max_h, max_w), fill_value=ignore_index, dtype=dtype)
+
+        for class_mask in class_masks:
+            if class_mask.shape != semantic_seg_mask.shape:
+                msg = f"There is inconsistency in mask size: {class_mask.shape}!={semantic_seg_mask.shape}."
+                raise ValueError(msg, class_mask.shape, semantic_seg_mask.shape)
+
+            ignore_index_mask = class_mask == ignore_index
+            semantic_seg_mask = np.where(ignore_index_mask, semantic_seg_mask, class_mask)
+
+        return semantic_seg_mask
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/components/annotations/matcher.py` & `datumaro-1.7.0rc1/src/datumaro/components/annotations/matcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import List, Optional, Union
 
 import numpy as np
 from attr import attrib, attrs
 
 from datumaro.components.abstracts import IMergerContext
 from datumaro.components.abstracts.merger import IMatcherContext
-from datumaro.components.annotation import Annotation
+from datumaro.components.annotation import Annotation, Points
 from datumaro.util.annotation_util import (
     OKS,
     approximate_line,
     bbox_iou,
     max_bbox,
     mean_bbox,
     segment_iou,
@@ -363,7 +363,18 @@
         raise NotImplementedError()
 
 
 @attrs
 class TabularMatcher(AnnotationMatcher):
     def match_annotations(self, sources):
         raise NotImplementedError()
+
+
+@attrs
+class RotatedBboxMatcher(ShapeMatcher):
+    sigma: Optional[list] = attrib(default=None)
+
+    def distance(self, a, b):
+        a = Points([p for pt in a.as_polygon() for p in pt])
+        b = Points([p for pt in b.as_polygon() for p in pt])
+
+        return OKS(a, b, sigma=self.sigma)
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/components/annotations/merger.py` & `datumaro-1.7.0rc1/src/datumaro/components/annotations/merger.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,22 +17,24 @@
     HashKeyMatcher,
     ImageAnnotationMatcher,
     LabelMatcher,
     LineMatcher,
     MaskMatcher,
     PointsMatcher,
     PolygonMatcher,
+    RotatedBboxMatcher,
     ShapeMatcher,
     TabularMatcher,
 )
 
 __all__ = [
     "AnnotationMerger",
     "LabelMerger",
     "BboxMerger",
+    "RotatedBboxMerger",
     "PolygonMerger",
     "MaskMerger",
     "PointsMerger",
     "LineMerger",
     "CaptionsMerger",
     "Cuboid3dMerger",
     "ImageAnnotationMerger",
@@ -199,7 +201,12 @@
 class FeatureVectorMerger(AnnotationMerger, FeatureVectorMatcher):
     pass
 
 
 @attrs
 class TabularMerger(AnnotationMerger, TabularMatcher):
     pass
+
+
+@attrs
+class RotatedBboxMerger(_ShapeMerger, RotatedBboxMatcher):
+    pass
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/components/cli_plugin.py` & `datumaro-1.7.0rc1/src/datumaro/components/cli_plugin.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/components/comparator.py` & `datumaro-1.7.0rc1/src/datumaro/components/comparator.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/components/config.py` & `datumaro-1.7.0rc1/src/datumaro/components/config.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/components/config_model.py` & `datumaro-1.7.0rc1/src/datumaro/components/config_model.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/components/contexts/importer.py` & `datumaro-1.7.0rc1/src/datumaro/components/contexts/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/components/crypter.py` & `datumaro-1.7.0rc1/src/datumaro/components/crypter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/components/dataset.py` & `datumaro-1.7.0rc1/src/datumaro/components/dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2020-2023 Intel Corporation
+# Copyright (C) 2020-2024 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
 import inspect
 import logging as log
@@ -15,14 +15,15 @@
     Any,
     Callable,
     Dict,
     Iterable,
     Iterator,
     List,
     Optional,
+    Set,
     Tuple,
     Type,
     Union,
     overload,
 )
 
 from datumaro.components.annotation import Annotation, AnnotationType, LabelCategories
@@ -36,14 +37,15 @@
     IDataset,
 )
 from datumaro.components.dataset_item_storage import DatasetItemStorageDatasetView
 from datumaro.components.dataset_storage import DatasetPatch, DatasetStorage, StreamDatasetStorage
 from datumaro.components.environment import DEFAULT_ENVIRONMENT, Environment
 from datumaro.components.errors import (
     DatasetImportError,
+    DatumaroError,
     MultipleFormatsMatchError,
     NoMatchingFormatsError,
     StreamedItemError,
     UnknownFormatError,
 )
 from datumaro.components.exporter import ExportContext, Exporter, ExportErrorPolicy, _ExportFail
 from datumaro.components.filter import (
@@ -107,30 +109,27 @@
 
     def categories(self):
         return self.parent.categories()
 
     def media_type(self):
         return self.parent.media_type()
 
+    def ann_types(self):
+        return self.parent.ann_types()
+
     def get_annotated_items(self):
         return sum(bool(s.annotations) for s in self.parent._data.get_subset(self.name))
 
     def get_annotations(self):
         annotations_by_type = {t.name: {"count": 0} for t in AnnotationType}
         for item in self.parent._data.get_subset(self.name):
             for ann in item.annotations:
                 annotations_by_type[ann.type.name]["count"] += 1
         return sum(t["count"] for t in annotations_by_type.values())
 
-    def get_annotated_type(self):
-        annotation_types = []
-        for item in self.parent._data.get_subset(self.name):
-            annotation_types.extend([str(anno.type).split(".")[-1] for anno in item.annotations])
-        return list(set(annotation_types))
-
     def as_dataset(self) -> Dataset:
         dataset = Dataset.from_extractors(self, env=self.parent.env)
         dataset._format = self.parent._format
         dataset._source_path = self.parent._source_path
         return dataset
 
 
@@ -156,14 +155,15 @@
         cls,
         iterable: Iterable[DatasetItem],
         infos: Optional[DatasetInfo] = None,
         categories: Union[CategoriesInfo, List[str], None] = None,
         *,
         env: Optional[Environment] = None,
         media_type: Type[MediaElement] = Image,
+        ann_types: Optional[Set[AnnotationType]] = [],
     ) -> Dataset:
         """
         Creates a new dataset from an iterable object producing dataset items -
         a generator, a list etc. It is a convenient way to create and fill
         a custom dataset.
 
         Parameters:
@@ -195,14 +195,15 @@
             categories = {}
 
         class _extractor(DatasetBase):
             def __init__(self):
                 super().__init__(
                     length=len(iterable) if hasattr(iterable, "__len__") else None,
                     media_type=media_type,
+                    ann_types=ann_types,
                 )
 
             def __iter__(self):
                 return iter(iterable)
 
             def infos(self):
                 return infos
@@ -250,24 +251,29 @@
     def __init__(
         self,
         source: Optional[IDataset] = None,
         *,
         infos: Optional[DatasetInfo] = None,
         categories: Optional[CategoriesInfo] = None,
         media_type: Optional[Type[MediaElement]] = None,
+        ann_types: Optional[Set[AnnotationType]] = None,
         env: Optional[Environment] = None,
     ) -> None:
         super().__init__()
 
         assert env is None or isinstance(env, Environment), env
         self._env = env
 
         self.eager = None
         self._data = DatasetStorage(
-            source, infos=infos, categories=categories, media_type=media_type
+            source=source,
+            infos=infos,
+            categories=categories,
+            media_type=media_type,
+            ann_types=ann_types,
         )
         if self.is_eager:
             self.init_cache()
 
         self._format = DEFAULT_FORMAT
         self._source_path = None
         self._options = {}
@@ -275,14 +281,15 @@
     def __repr__(self) -> str:
         separator = "\t"
         return (
             f"Dataset\n"
             f"\tsize={len(self._data)}\n"
             f"\tsource_path={self._source_path}\n"
             f"\tmedia_type={self.media_type()}\n"
+            f"\tann_types={self.ann_types()}\n"
             f"\tannotated_items_count={self.get_annotated_items()}\n"
             f"\tannotations_count={self.get_annotations()}\n"
             f"subsets\n"
             f"\t{separator.join(self.get_subset_info())}"
             f"infos\n"
             f"\t{separator.join(self.get_infos())}"
             f"categories\n"
@@ -315,14 +322,17 @@
 
     def categories(self) -> CategoriesInfo:
         return self._data.categories()
 
     def media_type(self) -> Type[MediaElement]:
         return self._data.media_type()
 
+    def ann_types(self) -> Set[AnnotationType]:
+        return self._data.ann_types()
+
     def get(self, id: str, subset: Optional[str] = None) -> Optional[DatasetItem]:
         return self._data.get(id, subset)
 
     def get_annotated_items(self):
         return self._data.get_annotated_items()
 
     def get_annotations(self):
@@ -339,16 +349,15 @@
             for label in self._data.categories().get(AnnotationType.label, LabelCategories())
         ]
 
     def get_subset_info(self) -> str:
         return (
             f"{subset_name}: # of items={len(self.get_subset(subset_name))}, "
             f"# of annotated items={self.get_subset(subset_name).get_annotated_items()}, "
-            f"# of annotations={self.get_subset(subset_name).get_annotations()}, "
-            f"annotation types={self.get_subset(subset_name).get_annotated_type()}\n"
+            f"# of annotations={self.get_subset(subset_name).get_annotations()}\n"
             for subset_name in sorted(self.subsets().keys())
         )
 
     def get_infos(self) -> Tuple[str]:
         if self.infos() is not None:
             return (f"{k}: {v}\n" for k, v in self.infos().items())
         else:
@@ -865,26 +874,29 @@
                             DeprecationWarning,
                         )
                     extractor_kwargs.pop("ctx")
 
                     extractors.append(
                         env.make_extractor(src_conf.format, src_conf.url, **extractor_kwargs)
                     )
-
             dataset = (
                 cls(source=extractor_merger(extractors), env=env)
                 if extractor_merger is not None
                 else cls.from_extractors(*extractors, env=env, merge_policy=merge_policy)
             )
             if eager:
                 dataset.init_cache()
         except _ImportFail as e:
             cause = e.__cause__ if getattr(e, "__cause__", None) is not None else e
             cause.__traceback__ = e.__traceback__
             raise DatasetImportError(f"Failed to import dataset '{format}' at '{path}'.") from cause
+        except DatumaroError as e:
+            cause = e.__cause__ if getattr(e, "__cause__", None) is not None else e
+            cause.__traceback__ = e.__traceback__
+            raise DatasetImportError(f"Failed to import dataset '{format}' at '{path}'.") from cause
         except Exception as e:
             raise DatasetImportError(f"Failed to import dataset '{format}' at '{path}'.") from e
 
         dataset._source_path = path
         dataset._format = format
 
         dataset = load_hash_key(path, dataset)
@@ -943,21 +955,26 @@
     def __init__(
         self,
         source: Optional[IDataset] = None,
         *,
         infos: Optional[DatasetInfo] = None,
         categories: Optional[CategoriesInfo] = None,
         media_type: Optional[Type[MediaElement]] = None,
+        ann_types: Optional[Set[AnnotationType]] = None,
         env: Optional[Environment] = None,
     ) -> None:
         assert env is None or isinstance(env, Environment), env
         self._env = env
 
         self._data = StreamDatasetStorage(
-            source, infos=infos, categories=categories, media_type=media_type
+            source,
+            infos=infos,
+            categories=categories,
+            media_type=media_type,
+            ann_types=ann_types,
         )
 
         self._format = DEFAULT_FORMAT
         self._source_path = None
         self._options = {}
 
     @property
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/components/dataset_base.py` & `datumaro-1.7.0rc1/src/datumaro/components/dataset_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from __future__ import annotations
 
 from typing import Any, Dict, Iterator, List, Optional, Sequence, Type, TypeVar, Union, cast
 
 import attr
 from attr import attrs, field
 
-from datumaro.components.annotation import Annotation, AnnotationType, Categories
+from datumaro.components.annotation import Annotation, Annotations, AnnotationType, Categories
 from datumaro.components.cli_plugin import CliPlugin
 from datumaro.components.contexts.importer import ImportContext, NullImportContext
 from datumaro.components.media import Image, MediaElement
 from datumaro.util.attrs_util import default_if_none, not_empty
 from datumaro.util.definitions import DEFAULT_SUBSET_NAME
 
 T = TypeVar("T", bound=MediaElement)
@@ -25,15 +25,15 @@
 
     subset: str = field(converter=lambda v: v or DEFAULT_SUBSET_NAME, default=None)
 
     media: Optional[MediaElement] = field(
         default=None, validator=attr.validators.optional(attr.validators.instance_of(MediaElement))
     )
 
-    annotations: List[Annotation] = field(factory=list, validator=default_if_none(list))
+    annotations: Annotations = field(factory=Annotations, validator=default_if_none(Annotations))
 
     attributes: Dict[str, Any] = field(factory=dict, validator=default_if_none(dict))
 
     def wrap(item, **kwargs):
         return attr.evolve(item, **kwargs)
 
     def media_as(self, t: Type[T]) -> T:
@@ -104,27 +104,34 @@
 
         All the items are supposed to have the same media type.
         Supposed to be constant and known immediately after the
         object construction (i.e. doesn't require dataset iteration).
         """
         raise NotImplementedError()
 
+    def ann_types(self) -> List[AnnotationType]:
+        """
+        Returns available task type from dataset annotation types.
+        """
+        raise NotImplementedError()
+
     @property
     def is_stream(self) -> bool:
         """Boolean indicating whether the dataset is a stream
 
         If the dataset is a stream, the dataset item is generated on demand from its iterator.
         """
         return False
 
 
 class _DatasetBase(IDataset):
     def __init__(self, *, length: Optional[int] = None, subsets: Optional[Sequence[str]] = None):
         self._length = length
         self._subsets = subsets
+        self._ann_types = set()
 
     def _init_cache(self):
         subsets = set()
         length = -1
         for length, item in enumerate(self):
             subsets.add(item.subset)
         length += 1
@@ -172,14 +179,17 @@
 
             def categories(_):
                 return self.categories()
 
             def media_type(_):
                 return self.media_type()
 
+            def ann_types(_):
+                return self.ann_types()
+
         return _DatasetFilter()
 
     def infos(self) -> DatasetInfo:
         return {}
 
     def categories(self) -> CategoriesInfo:
         return {}
@@ -201,41 +211,53 @@
 
     def __init__(
         self,
         *,
         length: Optional[int] = None,
         subsets: Optional[Sequence[str]] = None,
         media_type: Type[MediaElement] = Image,
+        ann_types: Optional[List[AnnotationType]] = None,
         ctx: Optional[ImportContext] = None,
     ):
         super().__init__(length=length, subsets=subsets)
 
         self._ctx: ImportContext = ctx or NullImportContext()
         self._media_type = media_type
+        self._ann_types = ann_types if ann_types else set()
 
     def media_type(self):
         return self._media_type
 
+    def ann_types(self):
+        return self._ann_types
+
 
 class SubsetBase(DatasetBase):
     """
     A base class for simple, single-subset extractors.
     Should be used by default for user-defined extractors.
     """
 
     def __init__(
         self,
         *,
         length: Optional[int] = None,
         subset: Optional[str] = None,
         media_type: Type[MediaElement] = Image,
+        ann_types: List[AnnotationType] = None,
         ctx: Optional[ImportContext] = None,
     ):
         self._subset = subset or DEFAULT_SUBSET_NAME
-        super().__init__(length=length, subsets=[self._subset], media_type=media_type, ctx=ctx)
+        super().__init__(
+            length=length,
+            subsets=[self._subset],
+            media_type=media_type,
+            ann_types=ann_types,
+            ctx=ctx,
+        )
 
         self._infos = {}
         self._categories = {}
         self._items = []
 
     def infos(self):
         return self._infos
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/components/dataset_item_storage.py` & `datumaro-1.7.0rc1/src/datumaro/components/dataset_item_storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright (C) 2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 from copy import copy
 from enum import Enum, auto
-from typing import Any, Iterator, Optional, Tuple, Type, Union
+from typing import Any, Iterator, Optional, Set, Tuple, Type, Union
 
 from datumaro.components.annotation import AnnotationType
 from datumaro.components.dataset_base import CategoriesInfo, DatasetInfo, DatasetItem, IDataset
 from datumaro.components.media import MediaElement
 from datumaro.util.definitions import DEFAULT_SUBSET_NAME
 
 __all__ = ["ItemStatus", "DatasetItemStorage", "DatasetItemStorageDatasetView"]
@@ -165,25 +165,30 @@
 
         def categories(self):
             return self.parent.categories()
 
         def media_type(self):
             return self.parent.media_type()
 
+        def ann_types(self):
+            return self.parent.ann_types()
+
     def __init__(
         self,
         parent: DatasetItemStorage,
         infos: DatasetInfo,
         categories: CategoriesInfo,
         media_type: Optional[Type[MediaElement]],
+        ann_types: Optional[Set[AnnotationType]],
     ):
         self._parent = parent
         self._infos = infos
         self._categories = categories
         self._media_type = media_type
+        self._ann_types = ann_types
 
     def __iter__(self):
         yield from self._parent
 
     def __len__(self):
         return len(self._parent)
 
@@ -203,7 +208,10 @@
         return {k: self.get_subset(k) for k in self._parent.subsets()}
 
     def get(self, id, subset=None):
         return self._parent.get(id, subset=subset)
 
     def media_type(self):
         return self._media_type
+
+    def ann_types(self):
+        return self._ann_types
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/components/dataset_storage.py` & `datumaro-1.7.0rc1/src/datumaro/components/dataset_storage.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright (C) 2020-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import logging as log
-from typing import Dict, Iterable, Iterator, List, Optional, Tuple, Type, Union
+from typing import Dict, Iterable, Iterator, List, Optional, Set, Tuple, Type, Union
 
 from datumaro.components.annotation import AnnotationType, LabelCategories
 from datumaro.components.dataset_base import (
     DEFAULT_SUBSET_NAME,
     CategoriesInfo,
     DatasetBase,
     DatasetInfo,
@@ -41,14 +41,15 @@
         # a patch and autofill patch info in Exporter
         def __init__(self, patch: "DatasetPatch", parent: IDataset):
             super().__init__(
                 patch.data,
                 infos=parent.infos(),
                 categories=parent.categories(),
                 media_type=parent.media_type(),
+                ann_types=parent.ann_types(),
             )
             self.patch = patch
 
         def subsets(self):
             return {s: self.get_subset(s) for s in self.patch.updated_subsets}
 
     def __init__(
@@ -111,22 +112,26 @@
 
     def categories(self) -> CategoriesInfo:
         return self.transforms[-1].categories()
 
     def media_type(self) -> Type[MediaElement]:
         return self.transforms[-1].media_type()
 
+    def ann_types(self) -> Set[AnnotationType]:
+        return self.transforms[-1].ann_types()
+
 
 class DatasetStorage(IDataset):
     def __init__(
         self,
         source: Union[IDataset, DatasetItemStorage],
         infos: Optional[DatasetInfo] = None,
         categories: Optional[CategoriesInfo] = None,
         media_type: Optional[Type[MediaElement]] = None,
+        ann_types: Optional[Set[AnnotationType]] = None,
     ):
         if source is None and categories is None:
             categories = {}
         elif isinstance(source, IDataset) and categories is not None:
             raise ValueError("Can't use both source and categories")
         self._categories = categories
 
@@ -139,16 +144,26 @@
         if media_type:
             pass
         elif isinstance(source, IDataset) and source.media_type():
             media_type = source.media_type()
         else:
             raise ValueError("Media type must be provided for a dataset")
         assert issubclass(media_type, MediaElement)
+
         self._media_type = media_type
 
+        if ann_types:
+            pass
+        elif isinstance(source, IDataset) and source.ann_types():
+            ann_types = source.ann_types()
+        else:
+            ann_types = set()
+
+        self._ann_types = ann_types
+
         # Possible combinations:
         # 1. source + storage
         #      - Storage contains a patch to the Source data.
         # 2. no source + storage
         #      - a dataset created from scratch
         #      - a dataset from a source or transform, which was cached
         if isinstance(source, DatasetItemStorage):
@@ -220,19 +235,29 @@
                     self._updated_items[item_id] = ItemStatus.modified
             elif new_status == ItemStatus.added:
                 if current_status != ItemStatus.added:
                     self._updated_items[item_id] = ItemStatus.modified
             else:
                 assert False, "Unknown status %s" % new_status
 
+        def _add_ann_types(item: DatasetItem):
+            for ann in item.annotations:
+                if ann.type == AnnotationType.hash_key:
+                    continue
+                self._ann_types.add(ann.type)
+
         media_type = self._media_type
         patch = self._storage  # must be empty after transforming
         cache = DatasetItemStorage()
         source = self._source or DatasetItemStorageDatasetView(
-            self._storage, infos=self._infos, categories=self._categories, media_type=media_type
+            self._storage,
+            infos=self._infos,
+            categories=self._categories,
+            media_type=media_type,
+            ann_types=self._ann_types,
         )
         transform = None
 
         if self._transforms:
             transform = _StackedTransform(source, self._transforms)
             if transform.is_local:
                 # An optimized way to find modified items:
@@ -295,29 +320,32 @@
                             _update_status(item_id, ItemStatus.modified)
 
             if not item:
                 continue
 
             cache.put(item)
             yield item
+            _add_ann_types(item)
 
         if i == -1:
             cache = patch
             for item in patch:
                 if not self._flush_changes:
                     _update_status((item.id, item.subset), ItemStatus.added)
                 yield item
+                _add_ann_types(item)
         else:
             for item in patch:
                 if item in cache:  # already processed
                     continue
                 if not self._flush_changes:
                     _update_status((item.id, item.subset), ItemStatus.added)
                 cache.put(item)
                 yield item
+                _add_ann_types(item)
 
         if not self._flush_changes and transform and not transform.is_local:
             # Mark removed items that were not produced by transforms
             for old_id in old_ids:
                 if old_id not in self._updated_items:
                     self._updated_items[old_id] = ItemStatus.removed
 
@@ -358,14 +386,15 @@
         elif self._source is not None:
             self.init_cache()
         return DatasetItemStorageDatasetView(
             self._storage,
             infos=self._infos,
             categories=self._categories,
             media_type=self._media_type,
+            ann_types=self._ann_types,
         )
 
     def __len__(self) -> int:
         if self._length is None:
             self.init_cache()
         return self._length
 
@@ -400,30 +429,38 @@
         if self._categories or self._source is not None:
             raise CategoriesRedefinedError()
         self._categories = categories
 
     def media_type(self) -> Type[MediaElement]:
         return self._media_type
 
+    def ann_types(self) -> Set[AnnotationType]:
+        return self._ann_types
+
     def put(self, item: DatasetItem) -> None:
         if item.media and not isinstance(item.media, self._media_type):
             raise MediaTypeError(
                 "Mismatching item media type '%s', "
                 "the dataset contains '%s' items." % (type(item.media), self._media_type)
             )
 
+        ann_types = set([ann.type for ann in item.annotations])
+        # hash_key can be included any task
+        ann_types.discard(AnnotationType.hash_key)
+
         is_new = self._storage.put(item)
 
         if not self.is_cache_initialized() or is_new:
             self._updated_items[(item.id, item.subset)] = ItemStatus.added
         else:
             self._updated_items[(item.id, item.subset)] = ItemStatus.modified
 
         if is_new and not self.is_cache_initialized():
             self._length = None
+            self._ann_types = set()
         if self._length is not None:
             self._length += is_new
 
     def get(self, id: str, subset: Optional[str] = None) -> Optional[DatasetItem]:
         id = str(id)
         subset = subset or DEFAULT_SUBSET_NAME
 
@@ -445,14 +482,15 @@
 
         self._storage.remove(id, subset)
         is_removed = self._updated_items.get((id, subset)) != ItemStatus.removed
         if is_removed:
             self._updated_items[(id, subset)] = ItemStatus.removed
         if is_removed and not self.is_cache_initialized():
             self._length = None
+            self._ann_types = set()
         if self._length is not None:
             self._length -= is_removed
 
     def get_subset(self, name: str) -> IDataset:
         return self._merged().get_subset(name)
 
     def subsets(self) -> Dict[str, IDataset]:
@@ -484,14 +522,15 @@
 
         if is_method_redefined("infos", Transform, method):
             self._infos = None
 
         if is_method_redefined("categories", Transform, method):
             self._categories = None
         self._length = None
+        self._ann_types = set()
 
     def has_updated_items(self):
         return bool(self._transforms) or bool(self._updated_items)
 
     def get_patch(self) -> DatasetPatch:
         # Patch includes only added or modified items.
         # To find removed items, one needs to consult updated_items list.
@@ -600,32 +639,36 @@
             "Random access to the dataset item is not allowed in streaming. "
             "You can access to the dataset item only by using its iterator."
         )
 
     def media_type(self) -> Type[MediaElement]:
         return self._source.media_type()
 
+    def ann_types(self) -> Set[AnnotationType]:
+        return self._source.ann_types()
+
     @property
     def is_stream(self) -> bool:
         return True
 
 
 class StreamDatasetStorage(DatasetStorage):
     def __init__(
         self,
         source: IDataset,
         infos: Optional[DatasetInfo] = None,
         categories: Optional[CategoriesInfo] = None,
         media_type: Optional[Type[MediaElement]] = None,
+        ann_types: Optional[Set[AnnotationType]] = None,
     ):
         if not source.is_stream:
             raise ValueError("source should be a stream.")
         self._subset_names = list(source.subsets().keys())
         self._transform_ids_for_latest_subset_names = []
-        super().__init__(source, infos, categories, media_type)
+        super().__init__(source, infos, categories, media_type, ann_types)
 
     def is_cache_initialized(self) -> bool:
         log.debug("This function has no effect on streaming.")
         return True
 
     def init_cache(self) -> None:
         log.debug("This function has no effect on streaming.")
@@ -639,15 +682,21 @@
         else:
             transform = self._source
 
         self._flush_changes = True
         return transform
 
     def __iter__(self) -> Iterator[DatasetItem]:
-        yield from self.stacked_transform
+        for item in self.stacked_transform:
+            yield item
+
+            for ann in item.annotations:
+                if ann.type == AnnotationType.hash_key:
+                    continue
+                self._ann_types.add(ann.type)
 
     def __len__(self) -> int:
         if self._length is None:
             self._length = len(self._source)
         return self._length
 
     def put(self, item: DatasetItem) -> None:
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/components/environment.py` & `datumaro-1.7.0rc1/src/datumaro/components/environment.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/components/errors.py` & `datumaro-1.7.0rc1/src/datumaro/components/errors.py`

 * *Files 0% similar despite different names*

```diff
@@ -308,14 +308,18 @@
         return "Failed to detect dataset format automatically: " "no matching formats found"
 
 
 class DatasetError(DatumaroError):
     pass
 
 
+class AnnotationTypeError(DatumaroError):
+    pass
+
+
 class MediaTypeError(DatumaroError):
     pass
 
 
 class MediaShapeError(DatumaroError):
     pass
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/components/exporter.py` & `datumaro-1.7.0rc1/src/datumaro/components/exporter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2019-2023 Intel Corporation
+# Copyright (C) 2019-2024 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import logging as log
 import os
 import os.path as osp
 import shutil
@@ -18,15 +18,15 @@
 from datumaro.components.dataset_base import DatasetItem, IDataset
 from datumaro.components.errors import (
     AnnotationExportError,
     DatasetExportError,
     DatumaroError,
     ItemExportError,
 )
-from datumaro.components.media import Image, PointCloud, VideoFrame
+from datumaro.components.media import Image, PointCloud, Video, VideoFrame
 from datumaro.components.progress_reporting import NullProgressReporter, ProgressReporter
 from datumaro.util.meta_file_util import save_hashkey_file, save_meta_file
 from datumaro.util.os_util import rmtree
 from datumaro.util.scope import on_error_do, scoped
 
 T = TypeVar("T")
 
@@ -335,18 +335,23 @@
 
     def make_pcd_extra_image_filename(self, item, idx, image, *, name=None, subdir=None):
         return self._make_item_filename(
             item, name=name if name else f"{item.id}/extra_image_{idx}", subdir=subdir
         ) + self.find_image_ext(image)
 
     def make_video_filename(self, item, *, name=None):
-        if isinstance(item, DatasetItem) and isinstance(item.media, VideoFrame):
+        STR_WRONG_MEDIA_TYPE = "Video item's media type should be Video or VideoFrame"
+        assert isinstance(item, DatasetItem), STR_WRONG_MEDIA_TYPE
+
+        if isinstance(item.media, VideoFrame):
             video_file_name = osp.basename(item.media.video.path)
+        elif isinstance(item.media, Video):
+            video_file_name = osp.basename(item.media.path)
         else:
-            assert "Video item type should be VideoFrame"
+            assert False, STR_WRONG_MEDIA_TYPE
 
         return video_file_name
 
     def save_image(
         self,
         item: DatasetItem,
         *,
@@ -396,28 +401,33 @@
         item.media.save(path, helper, crypter=NULL_CRYPTER)
 
     def save_video(
         self,
         item: DatasetItem,
         *,
         basedir: Optional[str] = None,
+        subdir: Optional[str] = None,
         fname: Optional[str] = None,
     ):
-        if not item.media or not isinstance(item.media, VideoFrame):
+        if not item.media or not isinstance(item.media, (Video, VideoFrame)):
             log.warning("Item '%s' has no video", item.id)
             return
         basedir = self._video_dir if basedir is None else basedir
+        basedir = osp.join(basedir, subdir) if subdir is not None else basedir
         fname = self.make_video_filename(item) if fname is None else fname
 
         path = osp.join(basedir, fname)
         path = osp.abspath(path)
 
         os.makedirs(osp.dirname(path), exist_ok=True)
 
-        item.media.video.save(path, crypter=NULL_CRYPTER)
+        if isinstance(item.media, VideoFrame):
+            item.media.video.save(path, crypter=NULL_CRYPTER)
+        else:  # Video
+            item.media.save(path, crypter=NULL_CRYPTER)
 
     @property
     def images_dir(self) -> str:
         return self._images_dir
 
     @property
     def pcd_dir(self) -> str:
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/components/extractor_tfds.py` & `datumaro-1.7.0rc1/src/datumaro/components/extractor_tfds.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     Any,
     Callable,
     Dict,
     Iterator,
     Mapping,
     Optional,
     Sequence,
+    Set,
     Tuple,
     Type,
     Union,
 )
 
 import attrs
 import numpy as np
@@ -478,14 +479,17 @@
                 return item
 
         return None
 
     def media_type(self) -> Type[MediaElement]:
         return self._parent._media_type
 
+    def ann_types(self) -> Set[AnnotationType]:
+        return self._parent.ann_types()
+
 
 class _TfdsExtractor(IDataset):
     _categories: CategoriesInfo
     _infos: DatasetInfo
 
     def __init__(self, tfds_ds_name: str) -> None:
         self._adapter = _TFDS_ADAPTERS[tfds_ds_name]
@@ -543,14 +547,22 @@
         if subset not in self._split_extractors:
             return None
         return self._split_extractors[subset].get(id)
 
     def media_type(self) -> Type[MediaElement]:
         return self._media_type
 
+    def ann_types(self) -> Set[AnnotationType]:
+        ann_types = set()
+        for items in self._split_extractors.values():
+            for item in items:
+                for ann in item.annotations:
+                    ann_types.add(ann.type)
+        return ann_types
+
 
 # Some dataset metadata elements are either inconvenient to hardcode, or may change
 # depending on the version of TFDS. We fetch them from the attributes of the `tfds.Builder`
 # object. However, creating the builder may be time-consuming, because if the dataset
 # is not already downloaded, TFDS fetches some data from its Google Cloud bucket.
 # We therefore only fetch this metadata (which we call _remote_ metadata) when
 # we actually need it.
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/components/filter.py` & `datumaro-1.7.0rc1/src/datumaro/components/filter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/components/format_detection.py` & `datumaro-1.7.0rc1/src/datumaro/components/format_detection.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/components/generator.py` & `datumaro-1.7.0rc1/src/datumaro/components/generator.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/components/hl_ops/__init__.py` & `datumaro-1.7.0rc1/src/datumaro/components/hl_ops/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/components/importer.py` & `datumaro-1.7.0rc1/src/datumaro/components/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/components/launcher.py` & `datumaro-1.7.0rc1/src/datumaro/components/launcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/components/lazy_plugin.py` & `datumaro-1.7.0rc1/src/datumaro/components/lazy_plugin.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/components/media.py` & `datumaro-1.7.0rc1/src/datumaro/components/media.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2021-2022 Intel Corporation
+# Copyright (C) 2021-2024 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
 import errno
 import io
@@ -90,15 +90,15 @@
             return TableRow
         raise NotImplementedError
 
 
 class MediaElement(Generic[AnyData]):
     _type = MediaType.MEDIA_ELEMENT
 
-    def __init__(self, crypter: Crypter = NULL_CRYPTER) -> None:
+    def __init__(self, crypter: Crypter = NULL_CRYPTER, *args, **kwargs) -> None:
         self._crypter = crypter
 
     def as_dict(self) -> Dict[str, Any]:
         # NOTE:
         # attributes starting with a single underscore are assumed
         # to be arguments of __init__ method and
         # attributes starting with double underscores are assuemd
@@ -484,14 +484,34 @@
     def video(self) -> Video:
         return self._video
 
     @property
     def path(self) -> str:
         return self._video.path
 
+    def from_self(self, **kwargs):
+        attrs = deepcopy(self.as_dict())
+        if "path" in kwargs:
+            attrs.update({"video": self.video.from_self(**kwargs)})
+            kwargs.pop("path")
+        attrs.update(kwargs)
+        return self.__class__(**attrs)
+
+    def __getstate__(self):
+        # Return only the picklable parts of the state.
+        state = self.__dict__.copy()
+        del state["_data"]
+        return state
+
+    def __setstate__(self, state):
+        # Restore the objects' state.
+        self.__dict__.update(state)
+        # Reinitialize unpichlable attributes
+        self._data = lambda: self._video.get_frame_data(self._index)
+
 
 class _VideoFrameIterator(Iterator[VideoFrame]):
     """
     Provides sequential access to the video frames.
     """
 
     _video: Video
@@ -523,14 +543,19 @@
                 self._current_frame_data = frame.astype(float)
                 yield self._make_frame(index=self._pos)
 
             success, frame = cap.read()
 
         if self._video._frame_count is None:
             self._video._frame_count = self._pos + 1
+            if self._video._end_frame and self._video._end_frame >= self._video._frame_count:
+                raise ValueError(
+                    f"The end_frame value({self._video._end_frame}) of the video "
+                    f"must be less than the frame count({self._video._frame_count})."
+                )
 
     def _make_frame(self, index) -> VideoFrame:
         return VideoFrame(self._video, index=index)
 
     def __next__(self):
         return next(self._iterator)
 
@@ -571,21 +596,30 @@
     _type = MediaType.VIDEO
 
     """
     Provides random access to the video frames.
     """
 
     def __init__(
-        self, path: str, *, step: int = 1, start_frame: int = 0, end_frame: Optional[int] = None
+        self,
+        path: str,
+        step: int = 1,
+        start_frame: int = 0,
+        end_frame: Optional[int] = None,
+        *args,
+        **kwargs,
     ) -> None:
-        super().__init__()
+        super().__init__(*args, **kwargs)
         self._path = path
 
+        assert 0 <= start_frame
         if end_frame:
-            assert start_frame < end_frame
+            assert start_frame <= end_frame
+            # we can't know the video length here,
+            # so we cannot validate if the end_frame is valid.
         assert 0 < step
         self._step = step
         self._start_frame = start_frame
         self._end_frame = end_frame or None
 
         self._reader = None
         self._iterator: Optional[_VideoFrameIterator] = None
@@ -626,24 +660,25 @@
         Iterates over frames lazily, if possible.
         """
 
         if self._frame_count is not None:
             # Decoding is not necessary to get frame pointers
             # However, it can be inacurrate
             end_frame = self._get_end_frame()
-            for index in range(self._start_frame, end_frame, self._step):
+            for index in range(self._start_frame, end_frame + 1, self._step):
                 yield VideoFrame(video=self, index=index)
         else:
             # Need to decode to iterate over frames
             yield from self._get_iterator()
 
     @property
     def length(self) -> Optional[int]:
         """
-        Returns frame count, if video provides such information.
+        Returns frame count of the closed interval [start_frame, end_frame],
+        if video provides such information.
 
         Note that not all videos provide length / duration metainfo, so the
         result may be undefined.
 
         Also note, that information may be inaccurate because of variable
         FPS in video or incorrect metainfo. The count is only guaranteed to
         be valid after video is completely read once.
@@ -651,20 +686,23 @@
         The count is affected by the frame filtering options of the object,
         i.e. start frame, end frame and frame step.
         """
 
         if self._length is None:
             end_frame = self._get_end_frame()
 
-            length = None
             if end_frame is not None:
-                length = (end_frame - self._start_frame) // self._step
-                assert 0 < length
-
-            self._length = length
+                length = (end_frame + 1 - self._start_frame) // self._step
+                if 0 >= length:
+                    raise ValueError(
+                        "There is no valid frame for the closed interval"
+                        f"[start_frame({self._start_frame}),"
+                        f" end_frame({end_frame})] with step({self._step})."
+                    )
+                self._length = length
 
         return self._length
 
     @property
     def frame_size(self) -> Tuple[int, int]:
         """Returns (H, W)"""
 
@@ -682,26 +720,31 @@
         else:
             image = next(self._get_iterator()).data
             frame_size = image.shape[0:2]
 
         return frame_size
 
     def _get_end_frame(self):
+        # Note that end_frame could less than the last frame of the video
         if self._end_frame is not None and self._frame_count is not None:
             end_frame = min(self._end_frame, self._frame_count)
+        elif self._end_frame is not None:
+            end_frame = self._end_frame
+        elif self._frame_count is not None:
+            end_frame = self._frame_count - 1
         else:
-            end_frame = self._end_frame or self._frame_count
+            end_frame = None
 
         return end_frame
 
     def _includes_frame(self, i):
-        end_frame = self._get_end_frame()
         if self._start_frame <= i:
             if (i - self._start_frame) % self._step == 0:
-                if end_frame is None or i < end_frame:
+                end_frame = self._get_end_frame()
+                if end_frame is None or i <= end_frame:
                     return True
 
         return False
 
     def _get_iterator(self):
         if self._iterator is None:
             self._iterator = _VideoFrameIterator(self)
@@ -715,23 +758,57 @@
     def _reset_reader(self):
         if self._reader is not None:
             self._reader.release()
         self._reader = cv2.VideoCapture(self._path)
         assert self._reader.isOpened()
 
     def __eq__(self, other: object) -> bool:
+        def _get_frame(obj: Video, idx: int):
+            try:
+                return obj[idx]
+            except IndexError:
+                return None
+
         if not isinstance(other, __class__):
             return False
+        if self._start_frame != other._start_frame or self._step != other._step:
+            return False
 
-        return (
-            self.path == other.path
-            and self._start_frame == other._start_frame
-            and self._step == other._step
-            and self._end_frame == other._end_frame
-        )
+        # The video path can vary if a dataset is copied.
+        # So, we need to check if the video data is the same instead of checking paths.
+        if self._end_frame is not None and self._end_frame == other._end_frame:
+            for idx in range(self._start_frame, self._end_frame + 1, self._step):
+                if self[idx] != other[idx]:
+                    return False
+            return True
+
+        end_frame = self._end_frame or other._end_frame
+        if end_frame is None:
+            last_frame = None
+            for idx, frame in enumerate(self):
+                if frame != _get_frame(other, frame.index):
+                    return False
+                last_frame = frame
+            # check if the actual last frames are same
+            try:
+                other[last_frame.index + self._step if last_frame else self._start_frame]
+            except IndexError:
+                return True
+            return False
+
+        # _end_frame values, only one of the two is valid
+        for idx in range(self._start_frame, end_frame + 1, self._step):
+            frame = _get_frame(self, idx)
+            if frame is None:
+                return False
+            if frame != _get_frame(other, idx):
+                return False
+        # check if the actual last frames are same
+        idx_next = end_frame + self._step
+        return None is (_get_frame(self, idx_next) or _get_frame(other, idx_next))
 
     def __hash__(self):
         # Required for caching
         return hash((self._path, self._step, self._start_frame, self._end_frame))
 
     def save(
         self,
@@ -1230,14 +1307,17 @@
     def columns(self) -> List[str]:
         """Returns column names"""
         return self.data.columns.to_list()
 
     def dtype(self, column: str) -> Optional[Type[TableDtype]]:
         """Returns native python type for a given column"""
         numpy_type = self.data.dtypes[column]
+        if self.data[column].nunique() / self.shape[0] < 0.1:  # TODO
+            # Convert to CategoricalDtype for efficient storage and categorical analysis
+            return pd.api.types.CategoricalDtype()
         if numpy_type == object:
             return str
         else:
             return type(np.zeros(1, numpy_type).tolist()[0])
 
     def features(self, column: str, unique: Optional[bool] = False) -> List[TableDtype]:
         """Get features for a given column name."""
@@ -1295,14 +1375,18 @@
         self._shape = data.shape
 
     @property
     def data(self) -> Optional[pd.DataFrame]:
         """Table data in pandas DataFrame format"""
         return self.__data
 
+    def select(self, columns: List[str]):
+        self.__data = self.__data[columns]
+        self._shape = self.__data.shape
+
 
 class TableFromDataFrame(FromDataMixin, Table):
     def __init__(
         self,
         data: Union[Callable[[], pd.DataFrame], pd.DataFrame],
         *args,
         **kwargs,
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/components/merge/__init__.py` & `datumaro-1.7.0rc1/src/datumaro/components/merge/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/components/merge/base.py` & `datumaro-1.7.0rc1/src/datumaro/components/merge/base.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # Copyright (C) 2020-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 import logging as log
 import os
 from collections import OrderedDict
-from typing import Dict, Optional, Sequence, Type
+from typing import Dict, Optional, Sequence, Set, Type
 
 from datumaro.components.abstracts.merger import IMergerContext
+from datumaro.components.annotation import AnnotationType
 from datumaro.components.cli_plugin import CliPlugin
 from datumaro.components.dataset_base import CategoriesInfo, DatasetInfo, IDataset
 from datumaro.components.dataset_item_storage import DatasetItemStorageDatasetView
 from datumaro.components.errors import (
     ConflictingCategoriesError,
     DatasetMergeError,
     DatasetQualityError,
@@ -69,20 +70,32 @@
                     # Symmetric comparision is needed in the case of subclasses:
                     # eg. Image and RoIImage
                     raise MediaTypeError("Datasets have different media types")
             return media_type
 
         return None
 
+    @staticmethod
+    def merge_ann_types(sources: Sequence[IDataset]) -> Optional[Set[AnnotationType]]:
+        ann_types = set()
+        for source in sources:
+            ann_types.union(source.ann_types())
+        return ann_types
+
     def __call__(self, *datasets: IDataset) -> DatasetItemStorageDatasetView:
         infos = self.merge_infos(d.infos() for d in datasets)
         categories = self.merge_categories(d.categories() for d in datasets)
         media_type = self.merge_media_types(datasets)
+        ann_types = self.merge_ann_types(datasets)
         return DatasetItemStorageDatasetView(
-            parent=self.merge(datasets), infos=infos, categories=categories, media_type=media_type
+            parent=self.merge(datasets),
+            infos=infos,
+            categories=categories,
+            media_type=media_type,
+            ann_types=ann_types,
         )
 
     def save_merge_report(self, path: str) -> None:
         item_errors = OrderedDict()
         source_errors = OrderedDict()
         all_errors = []
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/components/merge/exact_merge.py` & `datumaro-1.7.0rc1/src/datumaro/components/merge/exact_merge.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/components/merge/extractor_merger.py` & `datumaro-1.7.0rc1/src/datumaro/components/merge/extractor_merger.py`

 * *Files 14% similar despite different names*

```diff
@@ -38,14 +38,20 @@
     ):
         if len(sources) == 0:
             raise _ImportFail("It should not be empty.")
 
         self._infos = check_identicalness([s.infos() for s in sources])
         self._categories = check_identicalness([s.categories() for s in sources])
         self._media_type = check_identicalness([s.media_type() for s in sources])
+
+        ann_types = set()
+        for source in sources:
+            ann_types.union(source.ann_types())
+        self._ann_types = ann_types
+
         self._is_stream = check_identicalness([s.is_stream for s in sources])
 
         self._subsets: Dict[str, List[SubsetBase]] = defaultdict(list)
         for source in sources:
             self._subsets[source.subset] += [source]
 
     def infos(self) -> DatasetInfo:
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/components/merge/intersect_merge.py` & `datumaro-1.7.0rc1/src/datumaro/components/merge/intersect_merge.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     HashKeyMerger,
     ImageAnnotationMerger,
     LabelMerger,
     LineMerger,
     MaskMerger,
     PointsMerger,
     PolygonMerger,
+    RotatedBboxMerger,
     TabularMerger,
 )
 from datumaro.components.dataset_base import DatasetItem, IDataset
 from datumaro.components.dataset_item_storage import (
     DatasetItemStorage,
     DatasetItemStorageDatasetView,
 )
@@ -183,16 +184,21 @@
     def __call__(self, *datasets: IDataset) -> DatasetItemStorageDatasetView:
         # TODO: self.merge() should be the first since this order matters for
         # IntersectMerge.
         merged = self.merge(datasets)
         infos = self.merge_infos(d.infos() for d in datasets)
         categories = self.merge_categories(d.categories() for d in datasets)
         media_type = self.merge_media_types(datasets)
+        ann_types = self.merge_ann_types(datasets)
         return DatasetItemStorageDatasetView(
-            parent=merged, infos=infos, categories=categories, media_type=media_type
+            parent=merged,
+            infos=infos,
+            categories=categories,
+            media_type=media_type,
+            ann_types=ann_types,
         )
 
     def merge_categories(self, sources: Sequence[IDataset]) -> Dict:
         # TODO: This is a temporary workaround to minimize code changes.
         # We have to revisit it to make this class stateless.
         if hasattr(self, "_categories"):
             return self._categories
@@ -443,14 +449,16 @@
                 return _make(EllipseMerger, **kwargs)
             elif t is AnnotationType.hash_key:
                 return _make(HashKeyMerger, **kwargs)
             elif t is AnnotationType.feature_vector:
                 return _make(FeatureVectorMerger, **kwargs)
             elif t is AnnotationType.tabular:
                 return _make(TabularMerger, **kwargs)
+            elif t is AnnotationType.rotated_bbox:
+                return _make(RotatedBboxMerger, **kwargs)
             else:
                 raise NotImplementedError("Type %s is not supported" % t)
 
         instance_map = {}
         for s in sources:
             s_instances = find_instances(s)
             for inst in s_instances:
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/components/merge/union_merge.py` & `datumaro-1.7.0rc1/src/datumaro/components/merge/union_merge.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/components/operations.py` & `datumaro-1.7.0rc1/src/datumaro/components/operations.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/components/progress_reporting.py` & `datumaro-1.7.0rc1/src/datumaro/components/progress_reporting.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/components/project.py` & `datumaro-1.7.0rc1/src/datumaro/components/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,14 +96,16 @@
 class ProjectSourceDataset(IDataset):
     def __init__(self, path: str, tree: Tree, source: str, readonly: bool = False):
         config = tree.sources[source]
 
         rpath = path
         if config.path:
             rpath = osp.join(path, config.path)
+        if "path" in config.options:
+            rpath = osp.join(path, config.options.pop("path"))
 
         dataset = Dataset.import_from(rpath, env=tree.env, format=config.format, **config.options)
 
         # Using rpath won't allow to save directly with .save() when a file
         # path is specified. Dataset doesn't know the root location and if
         # it exists at all, but in a project, we do.
         dataset.bind(path, format=dataset.format, options=dataset.options)
@@ -155,14 +157,17 @@
 
     def get(self, id, subset=None):
         return self._dataset.get(id, subset)
 
     def media_type(self):
         return self._dataset.media_type()
 
+    def ann_types(self):
+        return self._dataset.ann_types()
+
 
 class IgnoreMode(Enum):
     rewrite = auto()
     append = auto()
     remove = auto()
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/components/registry.py` & `datumaro-1.7.0rc1/src/datumaro/components/registry.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/components/shift_analyzer.py` & `datumaro-1.7.0rc1/src/datumaro/components/shift_analyzer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/components/transformer.py` & `datumaro-1.7.0rc1/src/datumaro/components/transformer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/components/validator.py` & `datumaro-1.7.0rc1/src/datumaro/components/validator.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/components/visualizer.py` & `datumaro-1.7.0rc1/src/datumaro/components/visualizer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/accuracy_checker_plugin/details/ac.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/accuracy_checker_plugin/details/ac.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/accuracy_checker_plugin/details/representation.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/accuracy_checker_plugin/details/representation.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/anchor_generator.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/anchor_generator.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/configurable_validator.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/configurable_validator.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/ade20k2017.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/ade20k2017.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import os
 import os.path as osp
 import re
 from typing import List, Optional
 
 import numpy as np
 
-from datumaro.components.annotation import AnnotationType, CompiledMask, LabelCategories, Mask
+from datumaro.components.annotation import AnnotationType, ExtractedMask, LabelCategories
 from datumaro.components.dataset_base import DatasetBase, DatasetItem
 from datumaro.components.errors import InvalidAnnotationError
 from datumaro.components.format_detection import FormatDetectionContext
 from datumaro.components.importer import ImportContext, Importer
 from datumaro.components.media import Image
 from datumaro.util.image import IMAGE_EXTENSIONS, find_images, lazy_image, load_image
 from datumaro.util.meta_file_util import has_meta_file, parse_meta_file
@@ -64,15 +64,14 @@
         return self._categories
 
     def _load_items(self, subset):
         labels = self._categories.setdefault(AnnotationType.label, LabelCategories())
         path = osp.join(self._path, subset)
 
         images = [i for i in find_images(path, recursive=True)]
-
         for image_path in sorted(images):
             item_id = osp.splitext(osp.relpath(image_path, path))[0]
 
             if Ade20k2017Path.MASK_PATTERN.fullmatch(osp.basename(item_id)):
                 continue
 
             item_annotations = []
@@ -91,28 +90,28 @@
             max_part_level = max([p["part_level"] for p in item_info])
             for part_level in range(max_part_level + 1):
                 if not osp.exists(mask_path):
                     log.warning("Can`t find part level %s mask for %s" % (part_level, image_path))
                     continue
 
                 mask = lazy_image(mask_path, loader=self._load_instance_mask)
-                mask = CompiledMask(instance_mask=mask)
 
                 for v in item_info:
                     if v["part_level"] != part_level:
                         continue
 
                     label_id = labels.find(v["label_name"])[0]
                     instance_id = v["id"]
                     attributes = {k: True for k in v["attributes"]}
 
                     item_annotations.append(
-                        Mask(
+                        ExtractedMask(
+                            index_mask=mask,
+                            index=instance_id,
                             label=label_id,
-                            image=mask.lazy_extract(instance_id),
                             id=instance_id,
                             attributes=attributes,
                             z_order=part_level,
                             group=instance_id,
                         )
                     )
 
@@ -122,14 +121,16 @@
                 DatasetItem(
                     item_id,
                     subset=subset,
                     media=Image.from_file(path=image_path),
                     annotations=item_annotations,
                 )
             )
+            for ann in item_annotations:
+                self._ann_types.add(ann.type)
 
     def _load_item_info(self, path):
         attr_path = osp.splitext(path)[0] + "_atr.txt"
         if not osp.isfile(attr_path):
             raise FileNotFoundError(
                 errno.ENOENT, "Can't find annotation file for image %s" % path, attr_path
             )
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/ade20k2020.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/ade20k2020.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,21 +4,22 @@
 
 import errno
 import glob
 import logging as log
 import os
 import os.path as osp
 import re
+from functools import partial
 from typing import List, Optional
 
 import numpy as np
 
 from datumaro.components.annotation import (
     AnnotationType,
-    CompiledMask,
+    ExtractedMask,
     LabelCategories,
     Mask,
     Polygon,
 )
 from datumaro.components.dataset_base import DatasetBase, DatasetItem
 from datumaro.components.format_detection import FormatDetectionContext
 from datumaro.components.importer import ImportContext, Importer
@@ -72,15 +73,14 @@
         return self._categories
 
     def _load_items(self, subset):
         labels = self._categories.setdefault(AnnotationType.label, LabelCategories())
         path = osp.join(self._path, subset)
 
         images = [i for i in find_images(path, recursive=True)]
-
         for image_path in sorted(images):
             item_id = osp.splitext(osp.relpath(image_path, path))[0]
 
             if Ade20k2020Path.MASK_PATTERN.fullmatch(osp.basename(item_id)):
                 continue
 
             item_annotations = []
@@ -94,54 +94,53 @@
             max_part_level = max([p["part_level"] for p in item_info])
             for part_level in range(max_part_level + 1):
                 if not osp.exists(mask_path):
                     log.warning("Can`t find part level %s mask for %s" % (part_level, image_path))
                     continue
 
                 mask = lazy_image(mask_path, loader=self._load_class_mask)
-                mask = CompiledMask(instance_mask=mask)
 
                 classes = {
                     (v["class_idx"], v["label_name"])
                     for v in item_info
                     if v["part_level"] == part_level
                 }
 
                 for class_idx, label_name in classes:
                     label_id = labels.find(label_name)[0]
                     item_annotations.append(
-                        Mask(
+                        ExtractedMask(
+                            index_mask=mask,
+                            index=class_idx,
                             label=label_id,
                             id=class_idx,
-                            image=mask.lazy_extract(class_idx),
                             group=class_idx,
                             z_order=part_level,
                         )
                     )
 
                 mask_path = osp.splitext(image_path)[0] + "_parts_%s.png" % (part_level + 1)
 
             for item in item_info:
                 instance_path = osp.join(osp.dirname(image_path), item["instance_mask"])
                 if not osp.isfile(instance_path):
                     log.warning("Can`t find instance mask: %s" % instance_path)
                     continue
 
                 mask = lazy_image(instance_path, loader=self._load_instance_mask)
-                mask = CompiledMask(instance_mask=mask)
 
                 label_id = labels.find(item["label_name"])[0]
                 instance_id = item["id"]
                 attributes = {k: True for k in item["attributes"]}
                 polygon_points = item["polygon_points"]
 
                 item_annotations.append(
                     Mask(
                         label=label_id,
-                        image=mask.lazy_extract(1),
+                        image=partial(self._get_instance_mask, mask),
                         id=instance_id,
                         attributes=attributes,
                         z_order=item["part_level"],
                         group=instance_id,
                     )
                 )
 
@@ -161,14 +160,16 @@
                 DatasetItem(
                     item_id,
                     subset=subset,
                     media=Image.from_file(path=image_path),
                     annotations=item_annotations,
                 )
             )
+            for ann in item_annotations:
+                self._ann_types.add(ann.type)
 
     def _load_item_info(self, path):
         json_path = osp.splitext(path)[0] + ".json"
         item_info = []
         if not osp.isfile(json_path):
             raise FileNotFoundError(
                 errno.ENOENT, "Can't find annotation file for image %s" % path, json_path
@@ -211,14 +212,18 @@
 
     @staticmethod
     def _load_class_mask(path):
         mask = load_image(path)
         mask = ((mask[:, :, 2] / 10).astype(np.int32) << 8) + mask[:, :, 1].astype(np.int32)
         return mask
 
+    @staticmethod
+    def _get_instance_mask(mask: lazy_image) -> np.ndarray:
+        return mask() == 1
+
 
 class Ade20k2020Importer(Importer):
     _ANNO_EXT = ".json"
 
     @classmethod
     def detect(cls, context: FormatDetectionContext) -> None:
         annot_path = context.require_file(f"*/**/*{cls._ANNO_EXT}")
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/arrow/base.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/arrow/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright (C) 2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import struct
 from dataclasses import dataclass
-from typing import Any, Dict, Iterator, List, Optional, Type
+from typing import Any, Dict, Iterator, List, Optional, Set, Type
 
 import pyarrow as pa
 
 from datumaro.components.annotation import AnnotationType, Categories
 from datumaro.components.dataset_base import (
     CategoriesInfo,
     DatasetBase,
@@ -34,16 +34,19 @@
     def __init__(
         self,
         lookup: Dict[str, DatasetItem],
         infos: Dict[str, Any],
         categories: Dict[AnnotationType, Categories],
         subset: str,
         media_type: Type[MediaElement] = Image,
+        ann_types: Set[AnnotationType] = None,
     ):
-        super().__init__(length=len(lookup), subset=subset, media_type=media_type, ctx=None)
+        super().__init__(
+            length=len(lookup), subset=subset, media_type=media_type, ann_types=ann_types, ctx=None
+        )
 
         self._lookup = lookup
         self._infos = infos
         self._categories = categories
 
     def __iter__(self) -> Iterator[DatasetItem]:
         for item in self._lookup.values():
@@ -124,31 +127,36 @@
         self._lookup: Dict[str, Dict[str, DatasetItem]] = {subset: {} for subset in subsets}
 
         total = len(self)
         cnt = 0
         pbar = self._ctx.progress_reporter
         pbar.start(total=total, desc="Importing")
 
+        ann_types = set()
         for table_path in file_paths:
             with pa.OSFile(table_path, "r") as source:
                 with pa.ipc.open_file(source) as reader:
                     table = reader.read_all()
                     for idx in range(len(table)):
                         item = DatasetItemMapper.backward(idx, table, table_path)
                         self._lookup[item.subset][item.id] = item
+                        for ann in item.annotations:
+                            ann_types.add(ann.type)
                         pbar.report_status(cnt)
                         cnt += 1
+        self._ann_types = ann_types
 
         self._subsets = {
             subset: ArrowSubsetBase(
                 lookup=lookup,
                 infos=self._infos,
                 categories=self._categories,
                 subset=self._subsets,
                 media_type=self._media_type,
+                ann_types=self._ann_types,
             )
             for subset, lookup in self._lookup.items()
         }
 
         pbar.finish()
 
     def get(self, item_id: str, subset: Optional[str] = None) -> Optional[DatasetItem]:
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/arrow/exporter.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/arrow/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/arrow/format.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/arrow/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/arrow/importer.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/arrow/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/arrow/mapper/dataset_item.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/arrow/mapper/dataset_item.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/arrow/mapper/media.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/arrow/mapper/media.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/ava/ava.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/ava/ava.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,14 +148,15 @@
                         y=bbox[1],
                         w=bbox[2] - bbox[0],
                         h=bbox[3] - bbox[1],
                         label=label,
                         attributes={"track_id": entity_id},
                     )
                 )
+                self._ann_types.add(AnnotationType.bbox)
 
         return items.values()
 
 
 class AvaImporter(Importer):
     _ANNO_EXT = "csv"
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/ava/ava_label_pb2.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/ava/ava_label_pb2.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/brats.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/brats.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import glob
 import os.path as osp
 from typing import List, Optional
 
 import nibabel as nib
 import numpy as np
 
-from datumaro.components.annotation import AnnotationType, LabelCategories, Mask
+from datumaro.components.annotation import AnnotationType, ExtractedMask, LabelCategories
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
 from datumaro.components.format_detection import FormatDetectionContext
 from datumaro.components.importer import ImportContext, Importer
 from datumaro.components.media import MultiframeImage
 
 
 class BratsPath:
@@ -74,32 +74,31 @@
             item_id = osp.basename(image_path)[: -len(BratsPath.DATA_EXT)]
 
             if item_id not in items:
                 items[item_id] = DatasetItem(id=item_id)
 
             anno = []
             for i in range(data.shape[2]):
-                classes = np.unique(data[:, :, i])
+                np_mask = data[:, :, i]
+                classes = np.unique(np_mask)
                 for class_id in classes:
                     anno.append(
-                        Mask(
-                            image=self._lazy_extract_mask(data[:, :, i], class_id),
+                        ExtractedMask(
+                            index_mask=np_mask,
+                            index=class_id,
                             label=class_id,
                             attributes={"image_id": i},
                         )
                     )
+                    self._ann_types.add(AnnotationType.mask)
 
             items[item_id].annotations = anno
 
         return items
 
-    @staticmethod
-    def _lazy_extract_mask(mask, c):
-        return lambda: mask == c
-
 
 class BratsImporter(Importer):
     @classmethod
     def detect(cls, context: FormatDetectionContext) -> None:
         with context.require_any():
             with context.alternative():
                 context.require_file(f"*/*{BratsPath.DATA_EXT}")
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/brats_numpy.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/brats_numpy.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import errno
 import os.path as osp
 from typing import List, Optional
 
 import numpy as np
 
-from datumaro.components.annotation import AnnotationType, Cuboid3d, LabelCategories, Mask
+from datumaro.components.annotation import AnnotationType, Cuboid3d, ExtractedMask, LabelCategories
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
 from datumaro.components.format_detection import FormatDetectionContext
 from datumaro.components.importer import ImportContext, Importer
 from datumaro.components.media import MultiframeImage
 from datumaro.util.pickle_util import PickleLoader
 
 
@@ -60,14 +60,15 @@
 
         boxes = None
         boxes_file = osp.join(self._root_dir, BratsNumpyPath.BOXES_FILE)
         if osp.isfile(boxes_file):
             with open(boxes_file, "rb") as f:
                 boxes = PickleLoader.restricted_load(f)
 
+        # TODO(vinnamki): Apply lazy loading for images and masks
         for i, item_id in enumerate(ids):
             image_path = osp.join(self._root_dir, item_id + BratsNumpyPath.DATA_SUFFIX + ".npy")
             media = None
             if osp.isfile(image_path):
                 data = np.load(image_path)[0].transpose()
                 images = [0] * data.shape[2]
                 for j in range(data.shape[2]):
@@ -76,36 +77,36 @@
                 media = MultiframeImage(images, path=image_path)
 
             anno = []
             mask_path = osp.join(self._root_dir, item_id + BratsNumpyPath.LABEL_SUFFIX + ".npy")
             if osp.isfile(mask_path):
                 mask = np.load(mask_path)[0].transpose()
                 for j in range(mask.shape[2]):
-                    classes = np.unique(mask[:, :, j])
+                    np_mask = mask[:, :, j]
+                    classes = np.unique(np_mask)
                     for class_id in classes:
                         anno.append(
-                            Mask(
-                                image=self._lazy_extract_mask(mask[:, :, j], class_id),
+                            ExtractedMask(
+                                index_mask=np_mask,
+                                index=class_id,
                                 label=class_id,
                                 attributes={"image_id": j},
                             )
                         )
+                        self._ann_types.add(AnnotationType.mask)
 
             if boxes is not None:
                 box = boxes[i]
                 anno.append(Cuboid3d(position=list(box[0]), rotation=list(box[1])))
+                self._ann_types.add(AnnotationType.cuboid_3d)
 
             items[item_id] = DatasetItem(id=item_id, media=media, annotations=anno)
 
         return items
 
-    @staticmethod
-    def _lazy_extract_mask(mask, c):
-        return lambda: mask == c
-
 
 class BratsNumpyImporter(Importer):
     @classmethod
     def detect(cls, context: FormatDetectionContext) -> None:
         context.require_file(BratsNumpyPath.IDS_FILE)
 
     @classmethod
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/camvid.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/camvid.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 from typing import List, Optional, Tuple
 
 import numpy as np
 
 from datumaro.components.annotation import (
     AnnotationType,
     CompiledMask,
+    ExtractedMask,
     LabelCategories,
-    Mask,
     MaskCategories,
 )
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
 from datumaro.components.dataset_item_storage import ItemStatus
 from datumaro.components.errors import AnnotationExportError, InvalidAnnotationError, MediaTypeError
 from datumaro.components.exporter import Exporter
 from datumaro.components.format_detection import FormatDetectionContext
@@ -219,35 +219,38 @@
 
                 item_annotations = []
                 if gt is not None:
                     gt_path = osp.join(self._dataset_dir, gt)
                     mask = lazy_mask(
                         gt_path, self._categories[AnnotationType.mask].inverse_colormap
                     )
-                    mask = mask()  # loading mask through cache
+                    np_mask = mask()  # loading mask through cache
 
-                    classes = np.unique(mask)
+                    classes = np.unique(np_mask)
                     for label_id in classes:
                         if labels[label_id] in self._labels:
-                            image = self._lazy_extract_mask(mask, label_id)
-                            item_annotations.append(Mask(image=image, label=label_id))
+                            item_annotations.append(
+                                ExtractedMask(
+                                    index_mask=mask,
+                                    index=label_id,
+                                    label=label_id,
+                                )
+                            )
+
+                            self._ann_types.add(AnnotationType.mask)
 
                 items[item_id] = DatasetItem(
                     id=item_id,
                     subset=self._subset,
                     media=Image.from_file(path=image_path),
                     annotations=item_annotations,
                 )
 
         return items
 
-    @staticmethod
-    def _lazy_extract_mask(mask, c):
-        return lambda: mask == c
-
 
 class CamvidImporter(Importer):
     _ANNO_EXT = ".txt"
 
     @classmethod
     def detect(cls, context: FormatDetectionContext) -> None:
         annot_path = context.require_file(
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/celeba/align_celeba.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/celeba/align_celeba.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,15 @@
                 item_id, item_ann = self.split_annotation(line)
                 label_ids = [int(id) for id in item_ann]
                 anno = []
                 for label in label_ids:
                     while len(label_categories) <= label:
                         label_categories.add("class-%d" % len(label_categories))
                     anno.append(Label(label))
+                    self._ann_types.add(AnnotationType.label)
 
                 image = images.get(item_id)
                 if image:
                     image = Image.from_file(path=image)
 
                 items[item_id] = DatasetItem(id=item_id, media=image, annotations=anno)
 
@@ -117,14 +118,15 @@
                             "for this item are not label in %s "
                             % (landmark_path, line, AlignCelebaPath.LABELS_FILE)
                         )
 
                     anno = items[item_id].annotations
                     label = anno[0].label
                     anno.append(Points(landmarks, label=label))
+                    self._ann_types.add(AnnotationType.points)
 
                 if landmarks_number - 1 != counter:
                     raise InvalidAnnotationError(
                         "File '%s': the number of "
                         "landmarks does not match the specified number "
                         "at the beginning of the file " % landmark_path
                     )
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/celeba/celeba.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/celeba/celeba.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,14 +80,15 @@
                 item_id, item_ann = self.split_annotation(line)
                 label_ids = [int(id) for id in item_ann]
                 anno = []
                 for label in label_ids:
                     while len(label_categories) <= label:
                         label_categories.add("class-%d" % len(label_categories))
                     anno.append(Label(label))
+                    self._ann_types.add(AnnotationType.label)
 
                 image = images.get(item_id)
                 if image:
                     image = Image.from_file(path=image)
 
                 items[item_id] = DatasetItem(id=item_id, media=image, annotations=anno)
 
@@ -118,14 +119,15 @@
                             "for this item are not label in %s "
                             % (landmark_path, line, CelebaPath.LABELS_FILE)
                         )
 
                     anno = items[item_id].annotations
                     label = anno[0].label
                     anno.append(Points(landmarks, label=label))
+                    self._ann_types.add(AnnotationType.points)
 
                 if landmarks_number - 1 != counter:
                     raise InvalidAnnotationError(
                         "File '%s': the number of "
                         "landmarks does not match the specified number "
                         "at the beginning of the file " % landmark_path
                     )
@@ -153,14 +155,15 @@
                             "for this item are not label in %s "
                             % (bbox_path, line, CelebaPath.LABELS_FILE)
                         )
 
                     anno = items[item_id].annotations
                     label = anno[0].label
                     anno.append(Bbox(bbox[0], bbox[1], bbox[2], bbox[3], label=label))
+                    self._ann_types.add(AnnotationType.bbox)
 
                 if bboxes_number - 1 != counter:
                     raise InvalidAnnotationError(
                         "File '%s': the number of bounding "
                         "boxes does not match the specified number "
                         "at the beginning of the file " % bbox_path
                     )
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/cifar.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/cifar.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,14 +138,15 @@
             )
 
         for i, (filename, label) in enumerate(zip(filenames, labels)):
             item_id = osp.splitext(filename)[0]
             annotations = []
             if label is not None:
                 annotations.append(Label(label))
+                self._ann_types.add(AnnotationType.label)
                 if (
                     0 < len(coarse_labels)
                     and coarse_labels[i] is not None
                     and label_cat[label].parent == ""
                 ):
                     label_cat[label].parent = self._coarse_labels[coarse_labels[i]]
 
@@ -163,15 +164,14 @@
 
             if image is not None:
                 image = Image.from_numpy(data=image)
 
             items[item_id] = DatasetItem(
                 id=item_id, subset=self._subset, media=image, annotations=annotations
             )
-
         return items
 
 
 class CifarImporter(Importer):
     @classmethod
     def detect(
         cls,
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/cityscapes.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/cityscapes.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,28 +12,28 @@
 from typing import List, Optional
 
 import numpy as np
 
 from datumaro.components.annotation import (
     AnnotationType,
     CompiledMask,
+    ExtractedMask,
     LabelCategories,
-    Mask,
     MaskCategories,
 )
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
 from datumaro.components.dataset_item_storage import ItemStatus
 from datumaro.components.errors import AnnotationExportError, InvalidAnnotationError, MediaTypeError
 from datumaro.components.exporter import Exporter
 from datumaro.components.format_detection import FormatDetectionContext
 from datumaro.components.importer import ImportContext, Importer
 from datumaro.components.media import Image
 from datumaro.util import find
 from datumaro.util.annotation_util import make_label_id_mapping
-from datumaro.util.image import find_images, load_image, save_image
+from datumaro.util.image import find_images, lazy_image, save_image
 from datumaro.util.mask_tools import generate_colormap, paint_mask
 from datumaro.util.meta_file_util import has_meta_file, is_meta_file, parse_meta_file
 
 TRAIN_CITYSCAPES_LABEL_MAP = OrderedDict(
     [
         ("road", (128, 64, 128)),
         ("sidewalk", (244, 35, 232)),
@@ -276,28 +276,31 @@
             if label_id:
                 label_ids.append(label_id)
 
         for mask_path in masks:
             item_id = self._get_id_from_mask_path(mask_path, mask_suffix)
 
             anns = []
-            instances_mask = load_image(mask_path, dtype=np.int32)
+            index_mask = lazy_image(mask_path, dtype=np.int32)
+            np_index_mask = index_mask()
+
             mask_id = 1
             for label_id in label_ids:
-                if label_id not in instances_mask:
+                if label_id not in np_index_mask:
                     continue
-                binary_mask = self._lazy_extract_mask(instances_mask, label_id)
                 anns.append(
-                    Mask(
+                    ExtractedMask(
+                        index_mask=index_mask,
+                        index=label_id,
                         id=mask_id,
-                        image=binary_mask,
                         label=label_id,
                     )
                 )
                 mask_id += 1
+                self._ann_types.add(AnnotationType.mask)
 
             image = image_path_by_id.pop(item_id, None)
             if image:
                 image = Image.from_file(path=image)
 
             items[item_id] = DatasetItem(
                 id=item_id, subset=self._subset, media=image, annotations=anns
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/coco/base.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/coco/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -297,14 +297,16 @@
             _, item = parsed
 
             for ann_info in ann_infos:
                 self._parse_anns(img_info, ann_info, item)
 
             yield item
             length += 1
+            for ann in item.annotations:
+                self._ann_types.add(ann.type)
 
         self._length = length
 
     def _parse_anns(self, img_info, ann_info, item):
         try:
             if self._task is not CocoTask.panoptic:
                 self._load_annotations(ann_info, img_info, parsed_annotations=item.annotations)
@@ -333,15 +335,14 @@
             img_id, item = parsed
 
             # Store item (DatasetItem) and img_info (Dict) to the integer key dictionary
             items[img_id] = item
             img_infos[img_id] = img_info
 
         ann_lists = self._parse_field(json_data, "annotations", list)
-
         for ann_info in pbar.iter(
             _gen_ann(ann_lists),
             desc=f"Importing '{self._subset}'",
             total=len(ann_lists),
         ):
             try:
                 img_id = self._parse_field(ann_info, "image_id", int)
@@ -349,15 +350,16 @@
                     log.warn(f"Unknown image id '{img_id}'")
                     continue
 
                 # Retrieve item (DatasetItem) and img_info (Dict) from the integer key dictionary
                 item = items[img_id]
                 img_info = img_infos[img_id]
                 self._parse_anns(img_info, ann_info, item)
-
+                for ann in item.annotations:
+                    self._ann_types.add(ann.type)
             except Exception as e:
                 self._ctx.error_policy.report_annotation_error(
                     e, item_id=(ann_info.get("id", None), self._subset)
                 )
 
         return items
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/coco/exporter.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/coco/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/coco/extractor_merger.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/coco/extractor_merger.py`

 * *Files 10% similar despite different names*

```diff
@@ -75,14 +75,19 @@
             raise _ImportFail("It should not be empty.")
 
         self._infos = check_identicalness([s.infos() for s in sources])
         self._media_type = check_identicalness([s.media_type() for s in sources])
         self._is_stream = check_identicalness([s.is_stream for s in sources])
         self._categories = ExactMerge.merge_categories([s.categories() for s in sources])
 
+        ann_types = set()
+        for source in sources:
+            ann_types.union(source.ann_types())
+        self._ann_types = ann_types
+
         grouped_by_subset = defaultdict(list)
 
         for s in sources:
             grouped_by_subset[s.subset] += [s]
 
         self._subsets = {
             subset: [COCOTaskMergedBase(sources, subset)]
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/coco/format.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/coco/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/coco/importer.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/coco/importer.py`

 * *Files 11% similar despite different names*

```diff
@@ -52,26 +52,29 @@
         return parser
 
     @classmethod
     def detect(
         cls,
         context: FormatDetectionContext,
     ) -> FormatDetectionConfidence:
-        # The `coco` format is inherently ambiguous with `coco_instances`,
-        # `coco_stuff`, etc. To remove the ambiguity (and thus make it possible
-        # to use autodetection with the COCO dataset), disable autodetection
-        # for the single-task formats.
-        if len(cls._TASKS) == 1:
+        num_tasks = 0
+        for task in cls._TASKS.keys():
+            try:
+                context.require_files(f"annotations/{task.name}_*{cls._ANNO_EXT}")
+                num_tasks += 1
+            except Exception:
+                pass
+        if num_tasks > 1:
+            log.warning(
+                "Multiple COCO tasks are detected. The detected format will be `coco` instead."
+            )
+            return FormatDetectionConfidence.MEDIUM
+        else:
             context.raise_unsupported()
 
-        with context.require_any():
-            for task in cls._TASKS.keys():
-                with context.alternative():
-                    context.require_file(f"annotations/{task.name}_*{cls._ANNO_EXT}")
-
     def __call__(self, path, stream: bool = False, **extra_params):
         subsets = self.find_sources(path)
 
         if len(subsets) == 0:
             raise DatasetNotFoundError(path, self.NAME)
 
         # TODO: should be removed when proper label merging is implemented
@@ -136,16 +139,14 @@
             subset_paths = [path] if path.endswith(".json") else []
         else:
             subset_paths = glob(osp.join(path, "**", "*_*.json"), recursive=True)
 
         subsets = {}
         for subset_path in subset_paths:
             ann_type = detect_coco_task(osp.basename(subset_path))
-            if ann_type is None and len(cls._TASKS) == 1:
-                ann_type = list(cls._TASKS)[0]
 
             if ann_type not in cls._TASKS:
                 log.warning(
                     "File '%s' was skipped, could't match this file "
                     "with any of these tasks: %s"
                     % (subset_path, ",".join(e.NAME for e in cls._TASKS.values()))
                 )
@@ -171,36 +172,44 @@
         return COCOExtractorMerger
 
 
 class CocoImageInfoImporter(CocoImporter):
     _TASK = CocoTask.image_info
     _TASKS = {_TASK: CocoImporter._TASKS[_TASK]}
 
+    @classmethod
+    def detect(
+        cls,
+        context: FormatDetectionContext,
+    ) -> FormatDetectionConfidence:
+        context.require_file(f"annotations/{cls._TASK.name}_*{cls._ANNO_EXT}")
+        return FormatDetectionConfidence.LOW
+
 
-class CocoCaptionsImporter(CocoImporter):
+class CocoCaptionsImporter(CocoImageInfoImporter):
     _TASK = CocoTask.captions
     _TASKS = {_TASK: CocoImporter._TASKS[_TASK]}
 
 
-class CocoInstancesImporter(CocoImporter):
+class CocoInstancesImporter(CocoImageInfoImporter):
     _TASK = CocoTask.instances
     _TASKS = {_TASK: CocoImporter._TASKS[_TASK]}
 
 
-class CocoPersonKeypointsImporter(CocoImporter):
+class CocoPersonKeypointsImporter(CocoImageInfoImporter):
     _TASK = CocoTask.person_keypoints
     _TASKS = {_TASK: CocoImporter._TASKS[_TASK]}
 
 
-class CocoLabelsImporter(CocoImporter):
+class CocoLabelsImporter(CocoImageInfoImporter):
     _TASK = CocoTask.labels
     _TASKS = {_TASK: CocoImporter._TASKS[_TASK]}
 
 
-class CocoPanopticImporter(CocoImporter):
+class CocoPanopticImporter(CocoImageInfoImporter):
     _TASK = CocoTask.panoptic
     _TASKS = {_TASK: CocoImporter._TASKS[_TASK]}
 
 
-class CocoStuffImporter(CocoImporter):
+class CocoStuffImporter(CocoImageInfoImporter):
     _TASK = CocoTask.stuff
     _TASKS = {_TASK: CocoImporter._TASKS[_TASK]}
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/coco/page_mapper.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/coco/page_mapper.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/common_semantic_segmentation.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/common_semantic_segmentation.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,20 @@
 import errno
 import glob
 import os.path as osp
 from typing import List, Optional
 
 import numpy as np
 
-from datumaro.components.annotation import AnnotationType, LabelCategories, Mask, MaskCategories
+from datumaro.components.annotation import (
+    AnnotationType,
+    ExtractedMask,
+    LabelCategories,
+    MaskCategories,
+)
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
 from datumaro.components.format_detection import FormatDetectionConfidence, FormatDetectionContext
 from datumaro.components.importer import ImportContext, Importer, with_subset_dirs
 from datumaro.components.media import Image
 from datumaro.util.image import find_images
 from datumaro.util.mask_tools import generate_colormap, lazy_mask
 from datumaro.util.meta_file_util import DATASET_META_FILE, is_meta_file, parse_meta_file
@@ -102,22 +107,29 @@
             item_id = osp.splitext(osp.basename(mask_path))[0][len(self._mask_prefix) :]
 
             image = images.get(item_id)
             if image:
                 image = Image.from_file(path=image)
 
             annotations = []
-            mask = lazy_mask(mask_path, self._categories[AnnotationType.mask].inverse_colormap)
-            mask = mask()  # loading mask through cache
+            index_mask = lazy_mask(
+                mask_path, self._categories[AnnotationType.mask].inverse_colormap
+            )
+            np_mask = index_mask()  # loading mask through cache
 
-            classes = np.unique(mask)
+            classes = np.unique(np_mask)
             for label_id in classes:
                 annotations.append(
-                    Mask(image=self._lazy_extract_mask(mask, label_id), label=label_id)
+                    ExtractedMask(
+                        index_mask=index_mask,
+                        index=label_id,
+                        label=label_id,
+                    )
                 )
+                self._ann_types.add(AnnotationType.mask)
 
             items[item_id] = DatasetItem(
                 id=item_id, subset=self._subset, media=image, annotations=annotations
             )
 
         return items
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/common_super_resolution.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/common_super_resolution.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 import errno
 import os.path as osp
 from typing import List, Optional
 
-from datumaro.components.annotation import SuperResolutionAnnotation
+from datumaro.components.annotation import AnnotationType, SuperResolutionAnnotation
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
 from datumaro.components.format_detection import FormatDetectionContext
 from datumaro.components.importer import ImportContext, Importer
 from datumaro.components.media import Image
 from datumaro.util.image import find_images
 
 
@@ -71,14 +71,15 @@
                 upsampled_image = upsampled_images.get(item_id)
                 if upsampled_image:
                     attributes["upsampled"] = Image.from_file(path=upsampled_image)
 
                 items[item_id] = DatasetItem(id=item_id, subset=self._subset, attributes=attributes)
 
             items[item_id].annotations = [SuperResolutionAnnotation(Image.from_file(path=hr_image))]
+            self._ann_types.add(AnnotationType.super_resolution_annotation)
 
         return items
 
 
 class CommonSuperResolutionImporter(Importer):
     _FORMAT_EXT = ".jpg"
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/cvat/base.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/cvat/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,16 +65,16 @@
         self._path = path
 
         if not subset:
             subset = osp.splitext(osp.basename(path))[0]
         super().__init__(subset=subset, ctx=ctx)
 
         items, categories = self._parse(path)
-        self._items = list(self._load_items(items).values())
         self._categories = categories
+        self._items = list(self._load_items(items).values())
 
     def _parse(self, path):
         meta_root, context = _find_meta_root(path)
 
         categories, frame_size, attribute_types = self._parse_meta(meta_root)
 
         items = OrderedDict()
@@ -173,14 +173,15 @@
 
                     if subset is None or subset == self._subset:
                         frame_desc = items.get(shape["frame"], {"annotations": []})
                         frame_desc["annotations"].append(
                             self._parse_shape_ann(shape, categories, image)
                         )
                         items[shape["frame"]] = frame_desc
+
                     shape = None
 
                 elif el.tag == "tag":
                     if subset is None or subset == self._subset:
                         frame_desc = items.get(tag["frame"], {"annotations": []})
                         frame_desc["annotations"].append(self._parse_tag_ann(tag, categories))
                         items[tag["frame"]] = frame_desc
@@ -384,14 +385,17 @@
             parsed[frame_id] = DatasetItem(
                 id=osp.splitext(name)[0],
                 subset=self._subset,
                 media=image,
                 annotations=item_desc.get("annotations"),
                 attributes={"frame": int(frame_id)},
             )
+            for ann in item_desc.get("annotations"):
+                self._ann_types.add(ann.type)
+
         return parsed
 
 
 class CvatImporter(Importer):
     _ANNO_EXT = ".xml"
 
     @classmethod
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/cvat/exporter.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/cvat/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/cvat/format.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/cvat/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/datumaro/base.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/datumaro/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-# Copyright (C) 2023 Intel Corporation
+# Copyright (C) 2024 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import os.path as osp
 import re
-from typing import Dict, List, Optional, Type
+from typing import Dict, List, Optional, Set, Type
 
 from datumaro.components.annotation import (
     NO_OBJECT_ID,
     AnnotationType,
     Bbox,
     Caption,
     Cuboid3d,
@@ -50,14 +50,15 @@
         self._subset = subset
         self._rootpath = rootpath
         self._images_dir = images_dir
         self._pcd_dir = pcd_dir
         self._video_dir = video_dir
         self._videos = {}
         self._ctx = ctx
+        self.ann_types = {}
 
         self._reader = self._init_reader(path)
         self.media_type = self._load_media_type(self._reader)
         self.infos = self._load_infos(self._reader)
         self.categories = self._load_categories(self._reader)
         self.items = self._load_items(self._reader)
 
@@ -66,14 +67,18 @@
 
     @staticmethod
     def _load_media_type(parsed) -> Type[MediaElement]:
         media_type = parsed.get("media_type", MediaType.IMAGE)
         return MediaType(media_type).media
 
     @staticmethod
+    def _load_ann_types(parsed) -> Set[AnnotationType]:
+        return parsed.get("ann_types", set())
+
+    @staticmethod
     def _load_infos(parsed) -> Dict:
         return parsed.get("infos", {})
 
     @staticmethod
     def _load_categories(parsed) -> Dict:
         categories = {}
 
@@ -122,24 +127,46 @@
         def _gen():
             # Reverse the list to pop from the front of it
             item_descs.reverse()
             while item_descs:
                 yield item_descs.pop()
 
         items = []
+        ann_types = set()
+        actual_media_types = set()
         for item_desc in pbar.iter(
             _gen(), desc=f"Importing '{self._subset}'", total=len(item_descs)
         ):
             item = self._parse_item(item_desc)
             if item is not None:
                 items.append(item)
+                for ann in item.annotations:
+                    ann_types.add(ann.type)
+                if item.media:
+                    actual_media_types.add(item.media.type)
+
+        self.ann_types = ann_types
+
+        if len(actual_media_types) == 1:
+            actual_media_type = actual_media_types.pop()
+        elif len(actual_media_types) > 1:
+            actual_media_type = MediaType.MEDIA_ELEMENT
+        else:
+            actual_media_type = None
+
+        if actual_media_type and not issubclass(actual_media_type.media, self.media_type):
+            raise MediaTypeError(
+                f"Unexpected media type of a dataset '{self.media_type}'. "
+                f"Expected media type is '{actual_media_type.media}."
+            )
 
         return items
 
     def _parse_item(self, item_desc: Dict) -> Optional[DatasetItem]:
+        STR_MULTIPLE_MEDIA = "DatasetItem cannot contain multiple media types"
         try:
             item_id = item_desc["id"]
 
             media = None
             image_info = item_desc.get("image")
             if image_info:
                 image_filename = image_info.get("path") or item_id + DatumaroPath.IMAGE_EXT
@@ -147,20 +174,18 @@
                 if not osp.isfile(image_path):
                     # backward compatibility
                     old_image_path = osp.join(self._images_dir, image_filename)
                     if osp.isfile(old_image_path):
                         image_path = old_image_path
 
                 media = Image.from_file(path=image_path, size=image_info.get("size"))
-                if self.media_type == MediaElement:
-                    self.media_type = Image
 
             pcd_info = item_desc.get("point_cloud")
             if media and pcd_info:
-                raise MediaTypeError("Dataset cannot contain multiple media types")
+                raise MediaTypeError(STR_MULTIPLE_MEDIA)
             if pcd_info:
                 pcd_path = pcd_info.get("path")
                 point_cloud = osp.join(self._pcd_dir, self._subset, pcd_path)
 
                 related_images = None
                 ri_info = item_desc.get("related_images")
                 if ri_info:
@@ -169,30 +194,44 @@
                             size=ri.get("size"),
                             path=osp.join(self._images_dir, self._subset, ri.get("path")),
                         )
                         for ri in ri_info
                     ]
 
                 media = PointCloud.from_file(path=point_cloud, extra_images=related_images)
-                if self.media_type == MediaElement:
-                    self.media_type = PointCloud
 
             video_frame_info = item_desc.get("video_frame")
             if media and video_frame_info:
-                raise MediaTypeError("Dataset cannot contain multiple media types")
+                raise MediaTypeError(STR_MULTIPLE_MEDIA)
             if video_frame_info:
-                video_path = osp.join(self._video_dir, video_frame_info.get("video_path"))
+                video_path = osp.join(
+                    self._video_dir, self._subset, video_frame_info.get("video_path")
+                )
                 if video_path not in self._videos:
                     self._videos[video_path] = Video(video_path)
                 video = self._videos[video_path]
 
                 frame_index = video_frame_info.get("frame_index")
 
                 media = VideoFrame(video, frame_index)
 
+            video_info = item_desc.get("video")
+            if media and video_info:
+                raise MediaTypeError(STR_MULTIPLE_MEDIA)
+            if video_info:
+                video_path = osp.join(self._video_dir, self._subset, video_info.get("path"))
+                if video_path not in self._videos:
+                    self._videos[video_path] = Video(video_path)
+                step = video_info.get("step", 1)
+                start_frame = video_info.get("start_frame", 0)
+                end_frame = video_info.get("end_frame", None)
+                media = Video(
+                    path=video_path, step=step, start_frame=start_frame, end_frame=end_frame
+                )
+
             media_desc = item_desc.get("media")
             if not media and media_desc and media_desc.get("path"):
                 media = MediaElement(path=media_desc.get("path"))
 
         except Exception as e:
             self._ctx.error_policy.report_item_error(
                 e, item_id=(item_desc.get("id", None), self._subset)
@@ -369,34 +408,50 @@
         super().__init__(path, subset, rootpath, images_dir, pcd_dir, video_dir, ctx)
         self._length = None
 
     def __len__(self):
         return len(self._reader)
 
     def __iter__(self):
+        ann_types = set()
         pbar = self._ctx.progress_reporter
         for item_desc in pbar.iter(
             self._reader,
             desc=f"Importing '{self._subset}'",
         ):
-            yield self._parse_item(item_desc)
+            item = self._parse_item(item_desc)
+            yield item
+
+            if item is not None:
+                for ann in item.annotations:
+                    ann_types.add(ann.type)
+        self.ann_types = ann_types
 
     def _init_reader(self, path: str) -> DatumPageMapper:
         return DatumPageMapper(path)
 
     @staticmethod
     def _load_media_type(page_mapper: DatumPageMapper) -> Type[MediaElement]:
         media_type = page_mapper.media_type
 
         if media_type is None:
             return MediaType.IMAGE.media
 
         return media_type.media
 
     @staticmethod
+    def _load_ann_types(page_mapper: DatumPageMapper) -> Set[AnnotationType]:
+        ann_types = page_mapper.ann_types
+
+        if ann_types is None:
+            return set()
+
+        return ann_types
+
+    @staticmethod
     def _load_infos(page_mapper: DatumPageMapper) -> Dict:
         return page_mapper.infos
 
     @staticmethod
     def _load_categories(page_mapper: DatumPageMapper) -> Dict:
         return JsonReader._load_categories({"categories": page_mapper.categories})
 
@@ -470,14 +525,17 @@
 
     def categories(self):
         return self._reader.categories
 
     def media_type(self):
         return self._reader.media_type
 
+    def ann_types(self):
+        return self._reader.ann_types
+
     def _load_impl(self, path: str) -> None:
         """Actual implementation of loading Datumaro format."""
         self._reader = (
             JsonReader(
                 path,
                 self._subset,
                 self._rootpath,
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/datumaro/exporter.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/datumaro/exporter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 Intel Corporation
+# Copyright (C) 2024 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 # pylint: disable=no-self-use
 
 import json
 import os
@@ -175,21 +175,39 @@
         ----------
             item: Dataset item to save its media
             context: Context instance to help the media export
             encryption: If false, prevent the media from being encrypted
         """
         if item.media is None:
             yield
+        elif isinstance(item.media, Video):
+            video = item.media_as(Video)
+
+            if context.save_media:
+                fname = context.make_video_filename(item)
+                # To prevent the video from being overwritten
+                # (A video can have same path but different start/end frames)
+                if not osp.exists(fname):
+                    context.save_video(item, fname=fname, subdir=item.subset)
+                item.media = Video(
+                    path=video.path,
+                    step=video._step,
+                    start_frame=video._start_frame,
+                    end_frame=video._end_frame,
+                )
+
+            yield
+            item.media = video
         elif isinstance(item.media, VideoFrame):
             video_frame = item.media_as(VideoFrame)
 
             if context.save_media:
                 fname = context.make_video_filename(item)
                 if not osp.exists(fname):
-                    context.save_video(item, fname=fname)
+                    context.save_video(item, fname=fname, subdir=item.subset)
                 item.media = VideoFrame(Video(fname), video_frame.index)
 
             yield
             item.media = video_frame
         elif isinstance(item.media, Image):
             image = item.media_as(Image)
 
@@ -241,14 +259,23 @@
             # Since VideoFrame is a descendant of Image, this condition should be ahead of Image
             if isinstance(item.media, VideoFrame):
                 video_frame = item.media_as(VideoFrame)
                 item_desc["video_frame"] = {
                     "video_path": getattr(video_frame.video, "path", None),
                     "frame_index": getattr(video_frame, "index", -1),
                 }
+            elif isinstance(item.media, Video):
+                video = item.media_as(Video)
+                item_desc["video"] = {
+                    "path": getattr(video, "path", None),
+                    "step": video._step,
+                    "start_frame": video._start_frame,
+                }
+                if video._end_frame is not None:
+                    item_desc["video"]["end_frame"] = video._end_frame
             elif isinstance(item.media, Image):
                 image = item.media_as(Image)
                 item_desc["image"] = {"path": getattr(image, "path", None)}
                 if item.media.has_size:  # avoid occasional loading
                     item_desc["image"]["size"] = image.size
             elif isinstance(item.media, PointCloud):
                 pcd = item.media_as(PointCloud)
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/datumaro/importer.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/datumaro/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/datumaro/page_mapper.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/datumaro/page_mapper.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Copyright (C) 2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import logging as log
-from typing import Any, Dict, Iterator, Optional
+from typing import Any, Dict, Iterator, Optional, Set
 
+from datumaro.components.annotation import AnnotationType
 from datumaro.components.media import MediaType
 from datumaro.rust_api import DatumPageMapper as DatumPageMapperImpl
 
 __all__ = ["DatumPageMapper"]
 
 
 class DatumPageMapper:
@@ -54,14 +55,22 @@
         """Parse "media_type" section from the given JSON file using the stream json parser"""
         media_type = self._impl.media_type()
         if media_type is not None:
             return MediaType(media_type)
         return None
 
     @property
+    def ann_types(self) -> Optional[Set[AnnotationType]]:
+        """Parse "media_type" section from the given JSON file using the stream json parser"""
+        ann_types = self._impl.ann_types()
+        if ann_types is not None:
+            return ann_types
+        return None
+
+    @property
     def infos(self) -> Dict[str, Any]:
         """Parse "infos" section from the given JSON file using the stream json parser"""
         return self._impl.infos()
 
     @property
     def categories(self) -> Dict[str, Any]:
         """Parse "categories" section from the given JSON file using the stream json parser"""
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/datumaro_binary/base.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-# Copyright (C) 2023 Intel Corporation
+# Copyright (C) 2024 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import os.path as osp
 import struct
 from io import BufferedReader
 from multiprocessing.pool import AsyncResult, Pool
 from typing import Any, Dict, List, Optional
 
 from datumaro.components.crypter import NULL_CRYPTER, Crypter
 from datumaro.components.dataset_base import DatasetItem
 from datumaro.components.errors import DatasetImportError
 from datumaro.components.importer import ImportContext
-from datumaro.components.media import Image, MediaElement, MediaType, PointCloud, VideoFrame
+from datumaro.components.media import Image, MediaElement, MediaType, PointCloud, Video, VideoFrame
 from datumaro.plugins.data_formats.datumaro_binary.format import DatumaroBinaryPath
 from datumaro.plugins.data_formats.datumaro_binary.mapper import DictMapper
 from datumaro.plugins.data_formats.datumaro_binary.mapper.common import IntListMapper
 from datumaro.plugins.data_formats.datumaro_binary.mapper.dataset_item import DatasetItemMapper
 
 from ..datumaro.base import DatumaroBase, JsonReader
 
@@ -104,14 +104,16 @@
 
     def _read_media_type(self):
         media_type = self._read_header()["media_type"]
         if media_type == MediaType.IMAGE:
             self._media_type = Image
         elif media_type == MediaType.POINT_CLOUD:
             self._media_type = PointCloud
+        elif media_type == MediaType.VIDEO:
+            self._media_type = Video
         elif media_type == MediaType.VIDEO_FRAME:
             self._media_type = VideoFrame
         elif media_type == MediaType.MEDIA_ELEMENT:
             self._media_type = MediaElement
         else:
             raise NotImplementedError(f"media_type={media_type} is currently not supported.")
 
@@ -119,26 +121,30 @@
         (n_blob_sizes_bytes,) = struct.unpack("<I", self._fp.read(4))
         blob_sizes_bytes = self._crypter.decrypt(self._fp.read(n_blob_sizes_bytes))
         blob_sizes, _ = IntListMapper.backward(blob_sizes_bytes, 0)
 
         media_path_prefix = {
             MediaType.IMAGE: osp.join(self._images_dir, self._subset),
             MediaType.POINT_CLOUD: osp.join(self._pcd_dir, self._subset),
-            MediaType.VIDEO_FRAME: self._video_dir,
+            MediaType.VIDEO: osp.join(self._video_dir, self._subset),
+            MediaType.VIDEO_FRAME: osp.join(self._video_dir, self._subset),
         }
 
         if self._num_workers > 0:
             self._items = self._read_items_mp(blob_sizes, media_path_prefix)
         else:
             self._items = self._read_items_sp(blob_sizes, media_path_prefix)
 
         for item in self._items:
             if item.media is not None and self._media_encryption:
                 item.media.set_crypter(self._crypter)
 
+            for ann in item.annotations:
+                self._ann_types.add(ann.type)
+
     def _read_items_mp(
         self, blob_sizes: List[int], media_path_prefix: Dict[MediaType, str]
     ) -> List[DatasetItem]:
         async_results: List[AsyncResult] = []
 
         with Pool(processes=self._num_workers) as pool:
             for blob_size in blob_sizes:
@@ -198,12 +204,15 @@
 
     def categories(self):
         return self._categories
 
     def media_type(self):
         return self._media_type
 
+    def ann_types(self):
+        return self._ann_types
+
     def __len__(self) -> int:
         return len(self._items)
 
     def __iter__(self) -> DatasetItem:
         yield from self._items
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/datumaro_binary/exporter.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/datumaro_binary/format.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/datumaro_binary/importer.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 Intel Corporation
+# Copyright (C) 2024 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import os.path as osp
 import struct
 from typing import Dict, Optional, Tuple
 
@@ -17,14 +17,16 @@
     def forward(cls, obj: Optional[MediaElement]) -> bytes:
         if obj is None:
             return struct.pack("<I", MediaType.NONE)
         elif obj._type == MediaType.IMAGE:
             return ImageMapper.forward(obj)
         elif obj._type == MediaType.POINT_CLOUD:
             return PointCloudMapper.forward(obj)
+        elif obj._type == MediaType.VIDEO:
+            return VideoMapper.forward(obj)
         elif obj._type == MediaType.VIDEO_FRAME:
             return VideoFrameMapper.forward(obj)
         elif obj._type == MediaType.MEDIA_ELEMENT:
             return MediaElementMapper.forward(obj)
         else:
             raise DatumaroError(f"{obj._type} is not allowed for MediaMapper.")
 
@@ -39,14 +41,16 @@
 
         if media_type == MediaType.NONE:
             return None, offset + 4
         elif media_type == MediaType.IMAGE:
             return ImageMapper.backward(_bytes, offset, media_path_prefix)
         elif media_type == MediaType.POINT_CLOUD:
             return PointCloudMapper.backward(_bytes, offset, media_path_prefix)
+        elif media_type == MediaType.VIDEO:
+            return VideoMapper.backward(_bytes, offset, media_path_prefix)
         elif media_type == MediaType.VIDEO_FRAME:
             return VideoFrameMapper.backward(_bytes, offset, media_path_prefix)
         elif media_type == MediaType.MEDIA_ELEMENT:
             return MediaElementMapper.backward(_bytes, offset, media_path_prefix)
         else:
             raise DatumaroError(f"{media_type} is not allowed for MediaMapper.")
 
@@ -124,14 +128,47 @@
             Image.from_file(
                 path=media_dict["path"], size=size if size != cls.MAGIC_SIZE_FOR_NONE else None
             ),
             offset,
         )
 
 
+class VideoMapper(MediaElementMapper):
+    MAGIC_END_FRAME_FOR_NONE = 4294967295  # max value of unsigned int32
+    MEDIA_TYPE = MediaType.VIDEO
+
+    @classmethod
+    def forward(cls, obj: Video) -> bytes:
+        end_frame = obj._end_frame if obj._end_frame else cls.MAGIC_END_FRAME_FOR_NONE
+
+        bytes_arr = bytearray()
+        bytes_arr.extend(super().forward(obj))
+        bytes_arr.extend(struct.pack("<III", obj._step, obj._start_frame, end_frame))
+
+        return bytes(bytes_arr)
+
+    @classmethod
+    def backward(
+        cls,
+        _bytes: bytes,
+        offset: int = 0,
+        media_path_prefix: Optional[Dict[MediaType, str]] = None,
+    ) -> Tuple[Video, int]:
+        media_dict, offset = cls.backward_dict(_bytes, offset, media_path_prefix)
+        step, start_frame, end_frame = struct.unpack_from("<III", _bytes, offset)
+        offset += 12
+        video = Video(
+            path=media_dict["path"],
+            step=step,
+            start_frame=start_frame,
+            end_frame=end_frame if end_frame != cls.MAGIC_END_FRAME_FOR_NONE else None,
+        )
+        return (video, offset)
+
+
 class VideoFrameMapper(MediaElementMapper):
     MEDIA_TYPE = MediaType.VIDEO_FRAME
 
     @classmethod
     def forward(cls, obj: VideoFrame) -> bytes:
         bytes_arr = bytearray()
         bytes_arr.extend(super().forward(obj))
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/icdar/base.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/icdar/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import glob
 import logging as log
 import os.path as osp
 from typing import List, Optional
 
 import numpy as np
 
-from datumaro.components.annotation import Bbox, Caption, Mask, MaskCategories, Polygon
+from datumaro.components.annotation import Bbox, Caption, ExtractedMask, MaskCategories, Polygon
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
 from datumaro.components.errors import InvalidAnnotationError
 from datumaro.components.format_detection import FormatDetectionContext
 from datumaro.components.importer import ImportContext, Importer
 from datumaro.components.media import Image
 from datumaro.util.image import IMAGE_EXTENSIONS, find_images
 from datumaro.util.mask_tools import lazy_mask
@@ -89,14 +89,17 @@
                         item_id, subset=self._subset, media=Image.from_file(path=image_path)
                     )
 
                 annotations = items[item_id].annotations
                 for caption in captions:
                     annotations.append(Caption(caption))
 
+                for ann in annotations:
+                    self._ann_types.add(ann.type)
+
         return items
 
     def _load_localization_items(self):
         items = {}
 
         image_dir = osp.join(self._path, IcdarPath.IMAGES_DIR)
         if osp.isdir(image_dir):
@@ -160,14 +163,18 @@
                         if 0 < len(text):
                             attributes["text"] = text
                         elif len(objects) == 5:
                             text = objects[4]
                             attributes["text"] = text
 
                         annotations.append(Bbox(x, y, w, h, attributes=attributes))
+
+            for ann in annotations:
+                self._ann_types.add(ann.type)
+
         return items
 
     def _load_segmentation_items(self):
         items = {}
 
         image_dir = osp.join(self._path, IcdarPath.IMAGES_DIR)
         if osp.isdir(image_dir):
@@ -234,34 +241,39 @@
 
             mask_categories = MaskCategories({i: colors[i] for i in range(len(colors))})
             inverse_cls_colormap = mask_categories.inverse_colormap
 
             gt_path = osp.join(self._path, item_id + "_GT" + IcdarPath.GT_EXT)
             if osp.isfile(gt_path):
                 # load mask through cache
-                mask = lazy_mask(gt_path, inverse_cls_colormap)
-                mask = mask()
+                index_mask = lazy_mask(gt_path, inverse_cls_colormap)
+                np_index_mask = index_mask()
 
-                classes = np.unique(mask)
+                classes = np.unique(np_index_mask)
                 for label_id in classes:
                     if label_id == 0:
                         continue
                     i = int(label_id)
                     annotations.append(
-                        Mask(
+                        ExtractedMask(
+                            index_mask=index_mask,
+                            index=label_id,
                             group=groups[i],
-                            image=self._lazy_extract_mask(mask, label_id),
                             attributes={
                                 "index": i - 1,
                                 "color": " ".join(str(p) for p in colors[i]),
                                 "text": chars[i],
                                 "center": centers[i],
                             },
                         )
                     )
+
+            for ann in annotations:
+                self._ann_types.add(ann.type)
+
         return items
 
     @staticmethod
     def _lazy_extract_mask(mask, c):
         return lambda: mask == c
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/icdar/exporter.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/icdar/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/image_dir.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/image_dir.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,14 +55,15 @@
         assert osp.isdir(url), url
 
         for path in find_images(url, recursive=True):
             item_id = osp.relpath(osp.splitext(path)[0], url)
             self._items.append(
                 DatasetItem(id=item_id, subset=self._subset, media=Image.from_file(path=path))
             )
+        self._ann_types = set()
 
 
 class ImageDirExporter(Exporter):
     DEFAULT_IMAGE_EXT = ".jpg"
 
     def _apply_impl(self):
         os.makedirs(self._save_dir, exist_ok=True)
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/image_zip.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/image_zip.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,16 @@
             for path in zf.filelist:
                 item_id, extension = osp.splitext(path.filename)
                 if extension.lower() not in IMAGE_EXTENSIONS:
                     continue
                 image = Image.from_bytes(data=zf.read(path.filename))
                 self._items.append(DatasetItem(id=item_id, media=image, subset=self._subset))
 
+        self._ann_types = set()
+
 
 class ImageZipImporter(Importer):
     _FORMAT_EXT = ".zip"
 
     @classmethod
     def find_sources(cls, path):
         return cls._find_sources_recursive(path, cls._FORMAT_EXT, "image_zip")
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/imagenet.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/imagenet.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,14 +75,15 @@
                 self._ctx.error_policy.report_item_error(e, item_id=(item_id, self._subset))
             annotations = item.annotations
 
             if label != ImagenetPath.IMAGE_DIR_NO_LABEL:
                 try:
                     label = self._categories[AnnotationType.label].find(label)[0]
                     annotations.append(Label(label=label))
+                    self._ann_types.add(AnnotationType.label)
                 except Exception as e:
                     self._ctx.error_policy.report_annotation_error(
                         e, item_id=(item_id, self._subset)
                     )
 
         return items
 
@@ -128,14 +129,22 @@
 
         return []
 
     @classmethod
     def get_file_extensions(cls) -> List[str]:
         return list(IMAGE_EXTENSIONS)
 
+    @classmethod
+    def build_cmdline_parser(cls, **kwargs):
+        parser = super().build_cmdline_parser(**kwargs)
+        parser.add_argument("--path", required=True)
+        parser.add_argument("--subset")
+
+        return parser
+
 
 @with_subset_dirs
 class ImagenetWithSubsetDirsImporter(ImagenetImporter):
     """TorchVision ImageFolder style importer.
     For example, it imports the following directory structure.
 
     .. code-block::
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/imagenet_txt.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/imagenet_txt.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,22 +123,22 @@
                                 label_categories.add(f"class-{len(label_categories)}")
                         else:
                             raise DatasetImportError(
                                 f"Image '{item_id}': unknown label id '{label}'"
                             )
 
                     anno.append(Label(label))
+                    self._ann_types.add(AnnotationType.label)
 
                 items[item_id] = DatasetItem(
                     id=item_id,
                     subset=self._subset,
                     media=Image.from_file(path=osp.join(self.image_dir, image)),
                     annotations=anno,
                 )
-
         return items
 
 
 class ImagenetTxtImporter(Importer, CliPlugin):
     _ANNO_EXT = ".txt"
 
     @classmethod
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/kaggle/base.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/kaggle/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 # Copyright (C) 2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
+import json
 import os
 import os.path as osp
 import re
 import warnings
 from typing import Dict, Optional, Type, TypeVar, Union
 
 import numpy as np
 import pandas as pd
 from defusedxml import ElementTree
 
 from datumaro.components.annotation import (
     AnnotationType,
     Bbox,
+    ExtractedMask,
     Label,
     LabelCategories,
-    Mask,
     MaskCategories,
 )
 from datumaro.components.dataset import DatasetItem
 from datumaro.components.dataset_base import DEFAULT_SUBSET_NAME, DatasetBase, SubsetBase
 from datumaro.components.errors import InvalidAnnotationError, InvalidFieldError, MissingFieldError
 from datumaro.components.importer import ImportContext
 from datumaro.components.media import Image, ImageFromFile
 from datumaro.plugins.data_formats.coco.base import CocoInstancesBase
 from datumaro.plugins.data_formats.coco.format import CocoTask
 from datumaro.plugins.data_formats.coco.page_mapper import COCOPageMapper
 from datumaro.util import parse_json_file
-from datumaro.util.image import IMAGE_EXTENSIONS, load_image
+from datumaro.util.image import IMAGE_EXTENSIONS, lazy_image
 
 T = TypeVar("T")
 
 
 class KaggleImageCsvBase(DatasetBase):
     def __init__(
         self,
@@ -152,22 +153,23 @@
         for _, row in df.iloc[1:].iterrows():  # Skip header row
             data_info = list(row)
 
             media_name = data_info[indices["media"]]
             item_id = osp.splitext(media_name)[0]
 
             media_path = self._get_media_path(media_name)
-            if not osp.exists(media_path):
+            if not media_path or not osp.exists(media_path):
                 warnings.warn(
                     f"'{media_path}' is not existed in the directory, "
                     f"so we skip to create an dataset item according to {row}."
                 )
                 continue
 
             ann = self._load_annotations(data_info, indices, bbox_flag)
+            self._ann_types.add(ann.type)
             if item_id in items:
                 items[item_id].annotations.append(ann)
             else:
                 items[item_id] = DatasetItem(
                     id=item_id,
                     subset=self._subset,
                     media=Image.from_file(path=media_path),
@@ -177,14 +179,23 @@
 
     def categories(self):
         return self._categories
 
     def __iter__(self):
         yield from self._items
 
+    @classmethod
+    def build_cmdline_parser(cls, **kwargs):
+        parser = super().build_cmdline_parser(**kwargs)
+        parser.add_argument("--path", required=True)
+        parser.add_argument("--ann_file", required=True)
+        parser.add_argument("--columns", required=True, type=json.loads)
+
+        return parser
+
 
 class KaggleImageTxtBase(KaggleImageCsvBase):
     def __init__(
         self,
         path: str,
         ann_file: str,
         columns: Dict[str, int],
@@ -215,22 +226,23 @@
             for line in f:
                 line = re.split(r"\s|,", line)
 
                 media_name = line[columns["media"]]
                 item_id = osp.splitext(media_name)[0]
 
                 media_path = self._get_media_path(media_name)
-                if not osp.exists(media_path):
+                if not media_path or not osp.exists(media_path):
                     warnings.warn(
                         f"'{media_path}' is not existed in the directory, "
                         f"so we skip to create an dataset item according to {line}."
                     )
                     continue
 
                 ann = self._load_annotations(line, columns, bbox_flag)
+                self._ann_types.add(ann.type)
                 if item_id in items:
                     items[item_id].annotations.append(ann)
                 else:
                     items[item_id] = DatasetItem(
                         id=item_id,
                         subset=self._subset,
                         media=Image.from_file(path=media_path),
@@ -287,35 +299,33 @@
             self._label_ids.append(label_id)
 
         categories[AnnotationType.mask] = MaskCategories(colormap)
 
         return categories
 
     def _load_items(self):
-        def _lazy_extract_mask(mask, c):
-            return lambda: mask == c
-
         items = []
         for media_name in sorted(os.listdir(self._path)):
             id = osp.splitext(media_name)[0]
 
             anns = []
             for mask_name in os.listdir(self._mask_path):
                 if id in mask_name:
-                    instances_mask = load_image(
-                        osp.join(self._mask_path, mask_name), dtype=np.int32
+                    index_mask = lazy_image(
+                        path=osp.join(self._mask_path, mask_name), dtype=np.int32
                     )
-                    # label_ids = np.unique(instances_mask)
                     for label_id in self._label_ids:
                         anns.append(
-                            Mask(
-                                image=_lazy_extract_mask(instances_mask, label_id),
+                            ExtractedMask(
+                                index_mask=index_mask,
+                                index=label_id,
                                 label=label_id,
                             )
                         )
+                        self._ann_types.add(AnnotationType.mask)
 
             items.append(
                 DatasetItem(
                     id=id,
                     subset=self._subset,
                     media=Image.from_file(path=osp.join(self._path, media_name)),
                     annotations=anns,
@@ -326,14 +336,23 @@
 
     def categories(self):
         return self._categories
 
     def __iter__(self):
         yield from self._items
 
+    @classmethod
+    def build_cmdline_parser(cls, **kwargs):
+        parser = super().build_cmdline_parser(**kwargs)
+        parser.add_argument("--path", required=True)
+        parser.add_argument("--mask_path", required=True)
+        parser.add_argument("--labelmap_file")
+
+        return parser
+
 
 class KaggleVocBase(SubsetBase):
     ann_extensions = ".xml"
 
     def __init__(
         self,
         path: str,
@@ -355,14 +374,16 @@
 
             img_file = osp.join(path, img_filename)
             ann_file = osp.join(ann_path, item_id + self.ann_extensions)
 
             annotations = (
                 self._parse_annotations(img_file, ann_file) if osp.isfile(ann_file) else []
             )
+            for ann in annotations:
+                self._ann_types.add(ann.type)
 
             media = Image.from_file(path=img_file, size=self._size)
 
             self._items.append(
                 DatasetItem(
                     id=item_id,
                     subset=self._subset,
@@ -419,14 +440,23 @@
             return elem.text
 
         try:
             return cls(elem.text)
         except Exception as e:
             raise InvalidFieldError(xpath) from e
 
+    @classmethod
+    def build_cmdline_parser(cls, **kwargs):
+        parser = super().build_cmdline_parser(**kwargs)
+        parser.add_argument("--path", required=True)
+        parser.add_argument("--ann_path", required=True)
+        parser.add_argument("--subset")
+
+        return parser
+
 
 class KaggleYoloBase(KaggleVocBase, SubsetBase):
     ann_extensions = ".txt"
 
     def __init__(
         self,
         path: str,
@@ -518,7 +548,16 @@
 
             self._load_categories(
                 {"categories": categories_data},
                 keep_original_ids=keep_original_category_ids,
             )
 
             self._length = None
+
+    @classmethod
+    def build_cmdline_parser(cls, **kwargs):
+        parser = super().build_cmdline_parser(**kwargs)
+        parser.add_argument("--path", required=True)
+        parser.add_argument("--ann_file", required=True)
+        parser.add_argument("--subset")
+
+        return parser
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/kinetics.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/kinetics.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,14 +90,16 @@
         label_id, _ = self._categories[AnnotationType.label].find(label)
         if label_id is None:
             label_id = self._categories[AnnotationType.label].add(label)
 
         media_path = self._search_media_by_id(self._media_files(subset), item_id)
         media = Video(media_path) if media_path else None
 
+        self._ann_types.add(AnnotationType.label)
+
         return DatasetItem(
             id=item_id,
             annotations=[
                 Label(
                     label=label_id,
                     attributes={"time_start": int(time_start), "time_end": int(time_end)},
                 )
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/kitti/base.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/kitti/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 
 import glob
 import os.path as osp
 from typing import Optional
 
 import numpy as np
 
-from datumaro.components.annotation import AnnotationType, Bbox, LabelCategories, Mask
+from datumaro.components.annotation import AnnotationType, Bbox, ExtractedMask, LabelCategories
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
 from datumaro.components.importer import ImportContext
 from datumaro.components.media import Image
-from datumaro.util.image import find_images, load_image
+from datumaro.util.image import find_images, lazy_image
 from datumaro.util.meta_file_util import has_meta_file, parse_meta_file
 
 from .format import KittiLabelMap, KittiPath, KittiTask, make_kitti_categories, parse_label_map
 
 
 class _KittiBase(SubsetBase):
     def __init__(
@@ -63,41 +63,43 @@
                 label_map = KittiLabelMap
 
         self._labels = [label for label in label_map]
         return make_kitti_categories(label_map)
 
     def _load_items(self):
         items = {}
-
         image_dir = osp.join(self._path, KittiPath.IMAGES_DIR)
         image_path_by_id = {
             osp.splitext(osp.relpath(p, image_dir))[0]: p
             for p in find_images(image_dir, recursive=True)
         }
 
         segm_dir = osp.join(self._path, KittiPath.INSTANCES_DIR)
         if self._task == KittiTask.segmentation:
             for instances_path in find_images(segm_dir, exts=KittiPath.MASK_EXT, recursive=True):
                 item_id = osp.splitext(osp.relpath(instances_path, segm_dir))[0]
                 anns = []
 
-                instances_mask = load_image(instances_path, dtype=np.int32)
-                segm_ids = np.unique(instances_mask)
+                instances_mask = lazy_image(instances_path, dtype=np.int32)
+                np_instances_mask = instances_mask()
+                segm_ids = np.unique(np_instances_mask)
                 for segm_id in segm_ids:
                     semantic_id = segm_id >> 8
                     ann_id = int(segm_id % 256)
                     isCrowd = ann_id == 0
                     anns.append(
-                        Mask(
-                            image=self._lazy_extract_mask(instances_mask, segm_id),
+                        ExtractedMask(
+                            index_mask=instances_mask,
+                            index=segm_id,
                             label=semantic_id,
                             id=ann_id,
                             attributes={"is_crowd": isCrowd},
                         )
                     )
+                    self._ann_types.add(AnnotationType.mask)
 
                 image = image_path_by_id.pop(item_id, None)
                 if image:
                     image = Image.from_file(path=image)
 
                 items[item_id] = DatasetItem(
                     id=item_id, annotations=anns, media=image, subset=self._subset
@@ -137,24 +139,28 @@
                             w=x2 - x1,
                             h=y2 - y1,
                             id=line_idx,
                             attributes=attributes,
                             label=label_id,
                         )
                     )
+                    self._ann_types.add(AnnotationType.bbox)
 
                 image = image_path_by_id.pop(item_id, None)
                 if image:
                     image = Image.from_file(path=image)
 
                 items[item_id] = DatasetItem(
                     id=item_id, annotations=anns, media=image, subset=self._subset
                 )
 
         for item_id, image_path in image_path_by_id.items():
+            if item_id in items:
+                continue
+
             items[item_id] = DatasetItem(
                 id=item_id, subset=self._subset, media=Image.from_file(path=image_path)
             )
 
         return items
 
     @staticmethod
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/kitti/exporter.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/kitti/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/kitti/format.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/kitti/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/kitti/importer.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/kitti/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/kitti_raw/base.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/kitti_raw/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,16 +35,16 @@
     ):
         assert osp.isfile(path), path
         self._rootdir = osp.dirname(path)
 
         super().__init__(subset=subset, media_type=PointCloud, ctx=ctx)
 
         items, categories = self._parse(path)
-        self._items = list(self._load_items(items).values())
         self._categories = categories
+        self._items = list(self._load_items(items).values())
 
     @classmethod
     def _parse(cls, path):
         tracks = []
         track = None
         shape = None
         attr = None
@@ -254,14 +254,16 @@
                     extra_images=[
                         Image.from_file(path=image) for image in sorted(images.get(name, []))
                     ],
                 ),
                 annotations=item_desc.get("annotations"),
                 attributes={"frame": int(frame_id)},
             )
+            for ann in item_desc.get("annotations"):
+                self._ann_types.add(ann.type)
 
         for frame_id, name in name_mapping.items():
             if frame_id in items:
                 continue
 
             items[frame_id] = DatasetItem(
                 id=name,
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/kitti_raw/exporter.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/kitti_raw/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/kitti_raw/format.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/kitti_raw/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/labelme.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/labelme.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,14 +85,17 @@
                     (int(height_elem), int(width_elem)) if height_elem and width_elem else None
                 )
 
             image = Image.from_file(path=image_path, size=image_size)
 
             annotations = self._parse_annotations(root, path, subset, categories)
 
+            for ann in annotations:
+                self._ann_types.add(ann.type)
+
             items.append(
                 DatasetItem(id=item_id, subset=subset, media=image, annotations=annotations)
             )
             subsets.add(items[-1].subset)
         return items, categories, subsets
 
     @staticmethod
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/lfw.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/lfw.py`

 * *Files 2% similar despite different names*

```diff
@@ -204,14 +204,17 @@
                             subset=self._subset,
                             image=osp.join(self._images_dir, line[0]),
                         )
 
                     annotations = items[item_id].annotations
                     annotations.append(Points([float(p) for p in line[1:]], label=label))
 
+        for ann in annotations:
+            self._ann_types.add(ann.type)
+
         return items
 
     @staticmethod
     def get_image_name(person, image_id):
         image, item_id = "", ""
         try:
             image_id = int(image_id)
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mapillary_vistas/base.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/mapillary_vistas/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,17 +8,16 @@
 import os.path as osp
 from typing import Optional
 
 import numpy as np
 
 from datumaro.components.annotation import (
     AnnotationType,
-    CompiledMask,
+    ExtractedMask,
     LabelCategories,
-    Mask,
     MaskCategories,
     Polygon,
 )
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
 from datumaro.components.errors import DatasetImportError
 from datumaro.components.importer import ImportContext
 from datumaro.components.media import Image
@@ -145,38 +144,37 @@
                 "height": img.get("height"),
                 "width": img.get("width"),
             }
             for img in config["images"]
         }
 
         polygon_dir = osp.join(self._annotations_dir, MapillaryVistasPath.POLYGON_DIR)
-
         for item_ann in config["annotations"]:
             item_id = item_ann["image_id"]
             image = None
             if images_info.get(item_id):
                 image = Image.from_file(
                     path=images_info[item_id]["path"],
                     size=self._get_image_size(images_info[item_id]),
                 )
 
             mask_path = osp.join(
                 self._annotations_dir, MapillaryVistasPath.PANOPTIC_DIR, item_ann["file_name"]
             )
             mask = lazy_image(mask_path, loader=self._load_pan_mask)
-            mask = CompiledMask(instance_mask=mask)
 
             annotations = []
             for segment_info in item_ann["segments_info"]:
                 cat_id = self._get_label_id(segment_info)
                 segment_id = segment_info["id"]
                 attributes = {"is_crowd": bool(segment_info["iscrowd"])}
                 annotations.append(
-                    Mask(
-                        image=mask.lazy_extract(segment_id),
+                    ExtractedMask(
+                        index_mask=mask,
+                        index=segment_id,
                         label=cat_id,
                         id=segment_id,
                         group=segment_id,
                         attributes=attributes,
                     )
                 )
 
@@ -193,14 +191,16 @@
 
                     points = [int(coord) for point in polygon["polygon"] for coord in point]
                     annotations.append(Polygon(label=label_id, points=points))
 
             items[item_id] = DatasetItem(
                 id=item_id, subset=self._subset, annotations=annotations, media=image
             )
+            for ann in annotations:
+                self._ann_types.add(ann.type)
 
         return items.values()
 
     def _load_instances_categories(self):
         config_file = MapillaryVistasPath.CONFIG_FILES[self._format_version]
         label_map = None
 
@@ -212,47 +212,29 @@
             except FileNotFoundError:
                 label_map = parse_config_file(osp.join(osp.dirname(self._path), config_file))
         return make_mapillary_instance_categories(label_map)
 
     def _load_instances_items(self):
         items = {}
 
-        # class_dir = osp.join(self._annotations_dir, MapillaryVistasPath.CLASS_DIR)
-        # for class_path in find_images(class_dir, recursive=True):
-        #     item_id = osp.splitext(osp.relpath(class_path, class_dir))[0]
-        #     if item_id in items:
-        #         continue
-
-        #     from PIL import Image as PILImage
-
-        #     class_mask = np.array(PILImage.open(class_path))
-        #     classes = np.unique(class_mask)
-
-        #     annotations = []
-        #     for label_id in classes:
-        #         annotations.append(
-        #             Mask(label=label_id, image=self._lazy_extract_mask(class_mask, label_id))
-        #         )
-
-        #     items[item_id] = DatasetItem(id=item_id, subset=self._subset, annotations=annotations)
-
         instance_dir = osp.join(self._annotations_dir, MapillaryVistasPath.INSTANCES_DIR)
         polygon_dir = osp.join(self._annotations_dir, MapillaryVistasPath.POLYGON_DIR)
         for image_path in find_images(self._images_dir, recursive=True):
             item_id = osp.splitext(osp.relpath(image_path, self._images_dir))[0]
             image = Image.from_file(path=image_path)
 
             instance_path = osp.join(instance_dir, item_id + MapillaryVistasPath.MASK_EXT)
-            mask = load_image(instance_path, dtype=np.uint32)
+            index_mask = lazy_image(instance_path, dtype=np.uint32)
+            np_index_mask = index_mask()
 
             annotations = []
-            for uval in np.unique(mask):
+            for uval in np.unique(np_index_mask):
                 label_id, instance_id = uval >> 8, uval & 255
                 annotations.append(
-                    Mask(image=self._lazy_extract_mask(mask, uval), label=label_id, id=instance_id)
+                    ExtractedMask(index_mask=index_mask, index=uval, label=label_id, id=instance_id)
                 )
 
             if self._parse_polygon:
                 polygon_path = osp.join(polygon_dir, item_id + ".json")
                 item_info = parse_json_file(polygon_path)
 
                 polygons = item_info["objects"]
@@ -261,32 +243,31 @@
                     label_id = self._categories[AnnotationType.label].find(label)[0]
                     if label_id is None:
                         label_id = self._categories[AnnotationType.label].add(label)
 
                     points = [int(coord) for point in polygon["polygon"] for coord in point]
                     annotations.append(Polygon(label=label_id, points=points))
 
+            for ann in annotations:
+                self._ann_types.add(ann.type)
+
             items[item_id] = DatasetItem(
                 id=item_id, subset=self._subset, media=image, annotations=annotations
             )
 
         return items.values()
 
     @staticmethod
     def _get_image_size(image_info):
         image_size = image_info.get("height"), image_info.get("width")
         if all(image_size):
             return int(image_size[0]), int(image_size[1])
         return None
 
     @staticmethod
-    def _lazy_extract_mask(mask, c):
-        return lambda: mask == c
-
-    @staticmethod
     def _load_pan_mask(path):
         mask = load_image(path)
         mask = bgr2index(mask)
         return mask
 
     def _get_label_id(self, ann):
         cat_id = ann.get("category_id")
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mapillary_vistas/format.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/mapillary_vistas/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mapillary_vistas/importer.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/mapillary_vistas/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/market1501.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/market1501.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mars.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/mars.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,14 +99,15 @@
                             "person_id": pedestrian_id,
                             "camera_id": int(image_name[5]),
                             "track_id": int(image_name[7:11]),
                             "frame_id": int(image_name[12:15]),
                         },
                     )
                 )
+                self._ann_types.add(AnnotationType.label)
 
         return items
 
 
 class MarsImporter(Importer):
     @classmethod
     def detect(cls, context: FormatDetectionContext):
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mmdet.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/mmdet.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mnist.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/mnist.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,14 +101,15 @@
 
         pix_num = 0
         for i, annotation in enumerate(labels):
             annotations = []
             label = annotation
             if label != MnistPath.NONE_LABEL:
                 annotations.append(Label(label))
+                self._ann_types.add(AnnotationType.label)
 
             image = None
             if images is not None:
                 if 0 < len(meta) and 1 < len(meta[i]):
                     h, w = int(meta[i][-2]), int(meta[i][-1])
                     image = images[pix_num : pix_num + h * w].reshape(h, w)
                     pix_num += h * w
@@ -118,14 +119,15 @@
             if image is not None:
                 image = Image.from_numpy(data=image)
 
             if 0 < len(meta) and (len(meta[i]) == 1 or len(meta[i]) == 3):
                 i = meta[i][0]
 
             items[i] = DatasetItem(id=i, subset=self._subset, media=image, annotations=annotations)
+
         return items
 
 
 class MnistImporter(Importer):
     _FORMAT_EXT = ".gz"
 
     @classmethod
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mnist_csv.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/mnist_csv.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,14 +86,15 @@
             item_anno = []
             try:
                 label = int(data[0])
             except ValueError:
                 continue
             if label != MnistCsvPath.NONE_LABEL:
                 item_anno.append(Label(label))
+                self._ann_types.add(AnnotationType.label)
 
             if 0 < len(meta):
                 meta[i] = meta[i].strip().split(",")
 
             # support for single-channel image only
             image = None
             if 1 < len(data):
@@ -107,14 +108,15 @@
             if image is not None:
                 image = Image.from_numpy(data=image)
 
             if 0 < len(meta) and len(meta[i]) in [1, 3]:
                 i = meta[i][0]
 
             items[i] = DatasetItem(id=i, subset=self._subset, media=image, annotations=item_anno)
+
         return items
 
 
 class MnistCsvImporter(Importer):
     DETECT_CONFIDENCE = FormatDetectionConfidence.MEDIUM
     _ANNO_EXT = ".csv"
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mot.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/mot.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,14 +192,15 @@
                     attributes["visibility"] = visibility
                     attributes["occluded"] = visibility <= self._occlusion_threshold
                     attributes["ignored"] = confidence == 0
                 else:
                     attributes["score"] = float(confidence)
 
                 annotations.append(Bbox(x, y, w, h, label=label_id, attributes=attributes))
+                self._ann_types.add(AnnotationType.bbox)
 
                 items[frame_id] = item
         return items
 
     @classmethod
     def _parse_seq_info(cls, path):
         fields = {}
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mots.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/mots.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,21 +9,21 @@
 import os.path as osp
 from enum import Enum
 from glob import iglob
 from typing import List, Optional
 
 import numpy as np
 
-from datumaro.components.annotation import AnnotationType, LabelCategories, Mask
+from datumaro.components.annotation import AnnotationType, ExtractedMask, LabelCategories
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
 from datumaro.components.errors import MediaTypeError
 from datumaro.components.exporter import Exporter
 from datumaro.components.importer import ImportContext, Importer
 from datumaro.components.media import Image
-from datumaro.util.image import find_images, load_image, save_image
+from datumaro.util.image import find_images, lazy_image, save_image
 from datumaro.util.mask_tools import merge_masks
 from datumaro.util.meta_file_util import has_meta_file, parse_meta_file
 
 
 class MotsPath:
     MASKS_DIR = "instances"
     IMAGE_DIR = "images"
@@ -107,34 +107,38 @@
         return items
 
     @staticmethod
     def _lazy_extract_mask(mask, v):
         return lambda: mask == v
 
     def _parse_annotations(self, path):
-        combined_mask = load_image(path, dtype=np.uint16)
+        index_mask = lazy_image(path, dtype=np.uint16)
+        np_index_mask = index_mask()
+
         masks = []
-        for obj_id in np.unique(combined_mask):
+        for obj_id in np.unique(np_index_mask):
             class_id, instance_id = divmod(obj_id, MotsPath.MAX_INSTANCES)
             z_order = 0
             if class_id == 0:
                 continue  # background
             if class_id == 10 and len(self._categories[AnnotationType.label]) < 10:
                 z_order = 1
                 class_id = self._categories[AnnotationType.label].find(MotsLabels.ignored.name)[0]
             else:
                 class_id -= 1
             masks.append(
-                Mask(
-                    self._lazy_extract_mask(combined_mask, obj_id),
+                ExtractedMask(
+                    index_mask=index_mask,
+                    index=obj_id,
                     label=class_id,
                     z_order=z_order,
                     attributes={"track_id": instance_id},
                 )
             )
+            self._ann_types.add(AnnotationType.mask)
         return masks
 
 
 class MotsImporter(Importer):
     @classmethod
     def find_sources(cls, path):
         if not osp.isdir(path):
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mpii/format.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/mpii/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mpii/mpii_json.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/mpii/mpii_json.py`

 * *Files 3% similar despite different names*

```diff
@@ -158,14 +158,17 @@
             items[item_id] = DatasetItem(
                 id=item_id,
                 subset=self._subset,
                 media=Image.from_file(path=osp.join(root_dir, ann.get("img_paths", ""))),
                 annotations=annotations,
             )
 
+            for ann in annotations:
+                self._ann_types.add(ann.type)
+
         return items
 
 
 class MpiiJsonImporter(Importer):
     @classmethod
     def find_sources(cls, path):
         return cls._find_sources_recursive(path, ".json", "mpii_json")
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mpii/mpii_mat.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/mpii/mpii_mat.py`

 * *Files 3% similar despite different names*

```diff
@@ -134,14 +134,17 @@
             items[item_id] = DatasetItem(
                 id=item_id,
                 subset=self._subset,
                 media=Image.from_file(path=osp.join(root_dir, image)),
                 annotations=annotations,
             )
 
+            for ann in annotations:
+                self._ann_types.add(ann.type)
+
         return items
 
 
 class MpiiImporter(Importer):
     _FORMAT_EXT = ".mat"
 
     @classmethod
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mvtec/base.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/mvtec/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -94,14 +94,17 @@
                                 w=bbox[1] - bbox[0],
                                 h=bbox[3] - bbox[2],
                                 label=label_id,
                             )
                         )
                 else:
                     anns.append(Label(label=label_id))
+            for ann in anns:
+                self._ann_types.add(ann.type)
+
         return items
 
 
 class MvtecClassificationBase(_MvtecBase):
     def __init__(self, path, **kwargs):
         kwargs.pop("merge_policy")
         super().__init__(path, task=MvtecTask.classification, **kwargs)
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mvtec/exporter.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/mvtec/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mvtec/format.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/mvtec/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/mvtec/importer.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/mvtec/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/nyu_depth_v2.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/nyu_depth_v2.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import glob
 import os.path as osp
 from typing import List, Optional
 
 import h5py
 import numpy as np
 
-from datumaro.components.annotation import DepthAnnotation
+from datumaro.components.annotation import AnnotationType, DepthAnnotation
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
 from datumaro.components.format_detection import FormatDetectionContext
 from datumaro.components.importer import ImportContext, Importer
 from datumaro.components.media import Image
 
 
 class NyuDepthV2Base(SubsetBase):
@@ -43,14 +43,15 @@
                 depth = f["depth"][:].astype("float16")
 
             items[item_id] = DatasetItem(
                 id=item_id,
                 media=Image.from_numpy(data=image),
                 annotations=[DepthAnnotation(image=Image.from_numpy(data=depth))],
             )
+            self._ann_types.add(AnnotationType.depth_annotation)
 
         return items
 
 
 class NyuDepthV2Importer(Importer):
     _FORMAT_EXT = ".h5"
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/open_images.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/open_images.py`

 * *Files 1% similar despite different names*

```diff
@@ -395,14 +395,15 @@
                             subset=item.subset,
                             label_name=label_name,
                             severity=Severity.error,
                         )
                     item.annotations.append(
                         Label(label=label_index, attributes={"score": confidence})
                     )
+                    self._ann_types.add(AnnotationType.label)
 
     def _load_bboxes(self, items_by_id):
         label_categories = self._categories[AnnotationType.label]
 
         # OID specifies box coordinates in the normalized form, which we have to
         # convert to the unnormalized form to fit the Datumaro data model.
         # However, we need to temporarily preserve the normalized form as well,
@@ -472,14 +473,15 @@
                             y=y_min,
                             w=x_max - x_min,
                             h=y_max - y_min,
                             attributes=attributes,
                             group=group,
                         )
                     )
+                    self._ann_types.add(AnnotationType.bbox)
 
                     normalized_coords[id(item.annotations[-1])] = np.array(
                         [x_min_norm, x_max_norm, y_min_norm, y_max_norm]
                     )
 
         return normalized_coords
 
@@ -579,14 +581,15 @@
                                 ),
                             ),
                             label=label_index,
                             attributes=attributes,
                             group=group,
                         )
                     )
+                    self._ann_types.add(AnnotationType.mask)
 
     @staticmethod
     def _load_and_resize_mask(path, size):
         raw = load_image(path, dtype=np.uint8)
         resized = cv2.resize(raw, (size[1], size[0]), interpolation=cv2.INTER_NEAREST)
         return resized.astype(bool)
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/roboflow/base.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/roboflow/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 from datumaro.components.annotation import (
     Annotation,
     AnnotationType,
     Bbox,
     Label,
     LabelCategories,
-    Polygon,
+    RotatedBbox,
 )
 from datumaro.components.dataset import DatasetItem
 from datumaro.components.dataset_base import SubsetBase
 from datumaro.components.errors import InvalidAnnotationError, UndeclaredLabelError
 from datumaro.components.importer import ImportContext
 from datumaro.components.media import Image, ImageFromFile
 from datumaro.plugins.data_formats.coco.base import _CocoBase
@@ -166,16 +166,16 @@
             x2 = self._parse_field(x2, float, "x2")
             y2 = self._parse_field(y2, float, "y2")
             x3 = self._parse_field(x3, float, "x3")
             y3 = self._parse_field(y3, float, "y3")
             x4 = self._parse_field(x4, float, "x4")
             y4 = self._parse_field(y4, float, "y4")
             annotations.append(
-                Polygon(
-                    points=[x1, y1, x2, y2, x3, y3, x4, y4],
+                RotatedBbox.from_rectangle(
+                    points=[(x1, y1), (x2, y2), (x3, y3), (x4, y4)],
                     label=label_id,
                     id=idx,
                     group=idx,
                 )
             )
 
         return annotations
@@ -232,14 +232,15 @@
                     raise UndeclaredLabelError(ann["label"])
 
                 x = ann["coordinates"]["x"]
                 y = ann["coordinates"]["y"]
                 w = ann["coordinates"]["width"]
                 h = ann["coordinates"]["height"]
                 annotations.append(Bbox(x, y, w, h, label=label_id, id=ann_id, group=ann_id))
+                self._ann_types.add(AnnotationType.bbox)
 
             img_id = osp.splitext(anns["image"])[0]
             items[img_id] = DatasetItem(
                 id=img_id,
                 subset=self._subset,
                 media=Image.from_file(path=osp.join(osp.dirname(self._path), anns["image"])),
                 annotations=annotations,
@@ -298,14 +299,15 @@
                 for key, val in anns.items():
                     if key.strip() not in self._label_mapping:
                         continue
                     if int(val) == 1:
                         annotations.append(
                             Label(label=self._label_mapping[key.strip()], id=idx, group=idx)
                         )
+                        self._ann_types.add(AnnotationType.label)
                         idx += 1
 
                 items.append(
                     DatasetItem(
                         id=img_id,
                         subset=self._subset,
                         media=Image.from_file(
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/roboflow/base_tfrecord.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/roboflow/base_tfrecord.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/roboflow/importer.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/roboflow/importer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Copyright (C) 2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import os
 import os.path as osp
+import warnings
 from collections import defaultdict
 from glob import glob
 from io import TextIOWrapper
 from typing import Any, Dict, List, Type
 
 from defusedxml import ElementTree
 
@@ -191,14 +192,29 @@
 
 class RoboflowYoloObbImporter(RoboflowYoloImporter):
     FORMAT = "roboflow_yolo_obb"
     FORMAT_EXT = ".txt"
     ANN_DIR_NAME = "labelTxt/"
 
     @classmethod
+    def detect(cls, context: FormatDetectionContext) -> FormatDetectionConfidence:
+        warnings.warn(
+            f"FormatDetectionConfidence of '{cls.FORMAT}' is lowered because of 'dota' format support. "
+            f"It will be deprecated in datumaro==1.8.0.",
+            DeprecationWarning,
+        )
+        with context.require_any():
+            with context.alternative():
+                cls._check_ann_file(
+                    context.require_file("**/" + cls.ANN_DIR_NAME + "*" + cls.FORMAT_EXT), context
+                )
+
+        return FormatDetectionConfidence.LOW
+
+    @classmethod
     def _check_ann_file_impl(cls, fp: TextIOWrapper) -> bool:
         for line in fp:
             fields = line.rstrip("\n").split(" ")
             if len(fields) != 10:
                 raise DatasetImportError(
                     f"Roboflow Yolo OBB format txt file should have 10 fields for each line, "
                     f"but the read line has {len(fields)} fields: fields={fields}."
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/segment_anything/base.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/segment_anything/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,11 +159,13 @@
                             )
                         )
             except Exception as e:
                 self._ctx.error_policy.report_annotation_error(e, item_id=(image_id, self._subset))
 
             try:
                 items.append(DatasetItem(**item_kwargs))
+                for ann in item_kwargs["annotations"]:
+                    self._ann_types.add(ann.type)
             except Exception as e:
                 self._ctx.error_policy.report_item_error(e, item_id=(image_id, self._subset))
 
         return items
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/segment_anything/exporter.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/segment_anything/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/segment_anything/importer.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/segment_anything/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/sly_pointcloud/base.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/sly_pointcloud/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,16 +34,16 @@
 
         rootdir = osp.abspath(osp.dirname(path))
         self._rootdir = rootdir
 
         super().__init__(subset=subset, media_type=PointCloud, ctx=ctx)
 
         items, categories = self._parse(rootdir)
-        self._items = list(self._load_items(items).values())
         self._categories = categories
+        self._items = list(self._load_items(items).values())
 
     @classmethod
     def _parse(cls, rootpath):
         mapping = parse_json_file(osp.join(rootpath, PointCloudPath.KEY_ID_FILE))
         meta = parse_json_file(osp.join(rootpath, PointCloudPath.META_FILE))
 
         label_cat = LabelCategories()
@@ -178,14 +178,17 @@
                 id=name,
                 subset=self._subset,
                 media=PointCloud.from_file(path=pcd_path, extra_images=related_images),
                 annotations=frame_desc.get("annotations"),
                 attributes={"frame": int(frame_id), **frame_desc["attributes"]},
             )
 
+            for ann in frame_desc.get("annotations"):
+                self._ann_types.add(ann.type)
+
         return parsed
 
 
 class SuperviselyPointCloudImporter(Importer):
     NAME = "sly_pointcloud"
     _ANNO_EXT = ".json"
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/sly_pointcloud/exporter.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/sly_pointcloud/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/synthia/base.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/synthia/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,20 @@
 import os.path as osp
 from collections import OrderedDict
 from glob import glob
 from typing import Optional
 
 import numpy as np
 
-from datumaro.components.annotation import AnnotationType, LabelCategories, Mask, MaskCategories
+from datumaro.components.annotation import (
+    AnnotationType,
+    ExtractedMask,
+    LabelCategories,
+    MaskCategories,
+)
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
 from datumaro.components.errors import InvalidAnnotationError
 from datumaro.components.importer import ImportContext
 from datumaro.components.media import Image
 from datumaro.util.image import find_images
 from datumaro.util.mask_tools import generate_colormap, load_mask
 from datumaro.util.meta_file_util import has_meta_file, parse_meta_file
@@ -89,14 +94,15 @@
         if not osp.isdir(path):
             raise NotADirectoryError(errno.ENOTDIR, "Can't find dataset directory", path)
 
         super().__init__(subset=subset, ctx=ctx)
 
         self._path_formats = path_formats
         self._label_map = label_map
+        self._ann_types = set()
 
         self._img_dir = None
         self._inst_dir = None
         self._seg_dir = None
         for path_format in vars(path_formats).keys():
             if path_format == "IMAGES_DIR":
                 self._img_dir = osp.join(path, path_formats.IMAGES_DIR)
@@ -136,16 +142,17 @@
                 item_id = osp.splitext(osp.relpath(gt_label, self._inst_dir))[0].replace("\\", "/")
 
                 anno = []
                 labels_mask = np.loadtxt(gt_label)
                 classes = np.unique(labels_mask)
                 for label_id in classes:
                     anno.append(
-                        Mask(image=self._lazy_extract_mask(labels_mask, label_id), label=label_id)
+                        ExtractedMask(index_mask=labels_mask, index=label_id, label=label_id)
                     )
+                    self._ann_types.add(AnnotationType.mask)
 
                 image = images.get(item_id)
                 if image:
                     image = Image.from_file(path=image)
 
                 items[item_id] = DatasetItem(id=item_id, media=image, annotations=anno)
         elif self._seg_dir and osp.isdir(self._seg_dir):
@@ -158,29 +165,26 @@
 
                 color_mask = load_mask(seg_img_path, inverse_cls_colormap, default_id=0)
 
                 anno = []
                 classes = np.unique(color_mask)
                 for label_id in classes:
                     anno.append(
-                        Mask(image=self._lazy_extract_mask(color_mask, label_id), label=label_id)
+                        ExtractedMask(index_mask=color_mask, index=label_id, label=label_id)
                     )
+                    self._ann_types.add(AnnotationType.mask)
 
                 image = images.get(item_id)
                 if image:
                     image = Image.from_file(path=image)
 
                 items[item_id] = DatasetItem(id=item_id, media=image, annotations=anno)
 
         return items
 
-    @staticmethod
-    def _lazy_extract_mask(mask, c):
-        return lambda: mask == c
-
 
 class SynthiaRandBase(_SynthiaBase):
     def __init__(self, path: str, **kwargs):
         super().__init__(
             path=path, path_formats=SynthiaRandPath, label_map=SynthiaRandLabelMap, **kwargs
         )
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/synthia/format.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/synthia/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/synthia/importer.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/synthia/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/tabular.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/tabular.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 # SPDX-License-Identifier: MIT
 
 import errno
 import os
 import os.path as osp
 from typing import Dict, List, Optional, Tuple, Type, Union
 
+import pandas as pd
+
 from datumaro.components.annotation import AnnotationType, Categories, Tabular, TabularCategories
 from datumaro.components.dataset_base import DatasetBase, DatasetItem
 from datumaro.components.errors import MediaTypeError
 from datumaro.components.exporter import Exporter
 from datumaro.components.importer import ImportContext, Importer
 from datumaro.components.media import Table, TableDtype, TableRow
 from datumaro.util.os_util import find_files
@@ -58,75 +60,85 @@
 
         self._infos = {"path": path}
         self._items, self._categories = self._parse(paths, target, dtype)
 
     def _parse(
         self,
         paths: List[str],
-        target: Optional[Union[str, List[str]]] = None,
+        target: Optional[Dict[str, List[str]]] = None,
         dtype: Optional[Dict[str, Type[TableDtype]]] = None,
     ) -> Tuple[List[DatasetItem], Dict[AnnotationType, Categories]]:
         """
         parse tabular files. Each file is regarded as a subset.
 
         Args:
             paths (list(str)) : A list of paths to tabular data files(csv files).
-            target (optional, str or list) : Target column or list of target columns.
-                If this is not specified (None), the last column is regarded as a target column.
+            target (optional, dict(str or list)) : Target column or list of target columns for each input and output.
+                If this is not specified (None), the whole columns are regarded as a target column.
                 In case of a dataset with no targets, give an empty list as a parameter.
             dtype (optional, dict(str,str)) : Dictionay of column name -> type str ('str', 'int', or 'float').
                 This can be used when automatic type inferencing is failed.
 
         Returns:
             list (DatasetItem): dataset items
             dict (AnnotationType, Categories): categories info
         """
         # assert paths
         items: List[DatasetItem] = []
         categories: TabularCategories = TabularCategories()
 
+        if target is not None:
+            if "input" not in target or "output" not in target:
+                raise TypeError('Target should have both "input" and "output"')
+
         for path in paths:
             table = Table.from_csv(path, dtype=dtype)
 
             targets: List[str] = []
+            targets_ann: List[str] = []
             if target is None:
-                targets.append(table.columns[-1])  # last column
-            elif isinstance(target, str):
-                if target in table.columns:  # add valid column name only
-                    targets.append(target)
-            elif isinstance(target, list):  # add valid column names only
-                for t in target:
-                    if t in table.columns:
-                        targets.append(t)
+                targets.extend(table.columns)  # add all columns
+            else:
+                # add valid targeted output column name only
+                if isinstance(target.get("input"), str) and target["input"] in table.columns:
+                    targets.append(target["input"])
+                elif isinstance(target.get("input"), list):
+                    targets.extend(col for col in target["input"] if col in table.columns)
+                if isinstance(target.get("output"), str) and target["output"] in table.columns:
+                    targets_ann.append(target["output"])
+                elif isinstance(target.get("output"), list):
+                    targets_ann.extend(col for col in target["output"] if col in table.columns)
+            targets = targets + targets_ann
 
             # set categories
-            for target in targets:
-                _, category = categories.find(target)
-                target_dtype = table.dtype(target)
-                if target_dtype == str:
-                    labels = set(table.features(target, unique=True))
+            for target_ in targets_ann:
+                _, category = categories.find(target_)
+                target_dtype = table.dtype(target_)
+                if target_dtype in [int, float, pd.api.types.CategoricalDtype()]:
+                    # 'int' can be categorical, but we don't know this unless user gives information.
+                    labels = set(table.features(target_, unique=True))
                     if category is None:
-                        categories.add(target, target_dtype, labels)
+                        categories.add(target_, target_dtype, labels)
                     else:  # update labels if they are different.
                         category.labels.union(labels)
-                elif target_dtype in [int, float]:
-                    # 'int' can be categorical, but we don't know this unless user gives information.
+                elif target_dtype is str:
                     if category is None:
-                        categories.add(target, target_dtype)
+                        categories.add(target_, target_dtype)
                 else:
                     raise TypeError(
-                        f"Unsupported type '{target_dtype}' for target column '{target}'."
+                        f"Unsupported type '{target_dtype}' for target column '{target_}'."
                     )
 
             # load annotations
             subset = osp.splitext(osp.basename(path))[0]
             row: TableRow
+            table.select(targets)
             for row in table:  # type: TableRow
                 id = f"{row.index}@{subset}"
-                ann = [Tabular(values=row.data(targets))] if targets else None
+                ann = [Tabular(values=row.data(targets_ann))] if targets_ann else None
                 item = DatasetItem(
                     id=id,
                     subset=subset,
                     media=row,
                     annotations=ann,
                 )
                 items.append(item)
@@ -136,30 +148,54 @@
     def categories(self):
         return self._categories
 
     def __iter__(self):
         yield from self._items
 
 
+def string_to_dict(input_string):
+    pairs = input_string.split(",")
+    result = {}
+
+    for pair in pairs:
+        split_pair = pair.split(":")
+        # Check if the key is "input" or "output".
+        if len(split_pair) == 2:
+            key, value = split_pair
+            if key == "input" or key == "output":
+                if key in result:
+                    result[key].append(value)
+                else:
+                    result[key] = [value]
+            else:
+                # Ignore other keys
+                pass
+        else:
+            result[key].extend(split_pair)
+
+    return result
+
+
 class TabularDataImporter(Importer):
     """
     Import a tabular dataset.
     Each '.csv' file is regarded as a subset.
     """
 
     NAME = "tabular"
 
     @classmethod
     def build_cmdline_parser(cls, **kwargs):
         parser = super().build_cmdline_parser(**kwargs)
         parser.add_argument(
             "--target",
-            type=lambda x: x.split(","),
-            help="Target column or list of target columns. (ex. 'class', 'class,breed') (default:None) "
-            "If this is not specified (None), the last column is regarded as a target column."
+            type=lambda x: string_to_dict(x),
+            help="Target column or list of target columns for each input and output."
+            "(ex. 'input:date,output:class', 'input:data,output:class,breed') (default:None)"
+            "If this is not specified (None), the whole columns are regarded as a target column."
             "In case of a dataset with no targets, give an empty list as a parameter.",
         )
         parser.add_argument(
             "--dtype",
             type=lambda x: {k: v for k, v in (map.split(":") for map in x.split(","))},
             help="Type information for a column. (ex. 'date:str,x:int') (default:None) "
             "This can be used when automatic type inferencing is failed",
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/tf_detection_api/base.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/tf_detection_api/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,16 +69,16 @@
             "image/object/class/text": tf.io.VarLenFeature(tf.string),
             "image/object/mask": tf.io.VarLenFeature(tf.string),
         }
         if tfrecord_importer_type == TfrecordImporterType.roboflow:
             del self._features["image/source_id"]
 
         items, labels = self._parse_tfrecord_file(path, self._subset, images_dir)
-        self._items = items
         self._categories = self._load_categories(labels)
+        self._items = items
 
     @staticmethod
     def _load_categories(labels):
         label_categories = LabelCategories().from_iterable(
             e[0] for e in sorted(labels.items(), key=lambda item: item[1])
         )
         return {AnnotationType.label: label_categories}
@@ -181,14 +181,17 @@
                 if isinstance(frame_image, np.ndarray):
                     image = Image.from_numpy(data=frame_image, size=image_size)
                 else:
                     image = Image.from_bytes(data=frame_image, size=image_size)
             elif frame_filename:
                 image = Image.from_file(path=osp.join(images_dir, frame_filename), size=image_size)
 
+            for ann in annotations:
+                self._ann_types.add(ann.type)
+
             dataset_items.append(
                 DatasetItem(
                     id=item_id,
                     subset=subset,
                     media=image,
                     annotations=annotations,
                     attributes={"source_id": frame_id},
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/tf_detection_api/exporter.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/tf_detection_api/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/vgg_face2.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/vgg_face2.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,16 +151,18 @@
                         "Item %s: an image can have only one " "set of landmarks" % item_id
                     )
 
                 if len([p for p in row if row[p] == ""]) == 0 and len(row) == 11:
                     annotations.append(
                         Points([float(row[p]) for p in row if p != "NAME_ID"], label=label)
                     )
+                    self._ann_types.add(AnnotationType.points)
                 elif label is not None:
                     annotations.append(Label(label=label))
+                    self._ann_types.add(AnnotationType.label)
 
         bboxes_path = osp.join(
             self._dataset_dir,
             VggFace2Path.ANNOTATION_DIR,
             VggFace2Path.BBOXES_FILE + subset + ".csv",
         )
         if osp.isfile(bboxes_path):
@@ -190,14 +192,15 @@
                             float(row["X"]),
                             float(row["Y"]),
                             float(row["W"]),
                             float(row["H"]),
                             label=label,
                         )
                     )
+                    self._ann_types.add(AnnotationType.bbox)
         return items
 
 
 class VggFace2Importer(Importer):
     _ANNO_EXT = ".csv"
 
     @classmethod
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/video.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/video.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,14 +118,15 @@
         super().__init__(subsets=[self._subset], media_type=VideoFrame, ctx=ctx)
 
         assert osp.isfile(url), url
 
         self._name_pattern = name_pattern
         self._reader = Video(url, step=step, start_frame=start_frame, end_frame=end_frame)
         self._length = self._reader.length  # NOTE: the value is often incorrect
+        self._ann_types = set()
 
     def __iter__(self):
         for frame in self._reader:
             yield DatasetItem(
                 id=self._name_pattern % (frame.index,), subset=self._subset, media=frame
             )
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/voc/base.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/voc/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 from defusedxml import ElementTree
 
 from datumaro.components.annotation import (
     Annotation,
     AnnotationType,
     Bbox,
     CompiledMask,
+    ExtractedMask,
     Label,
-    Mask,
 )
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
 from datumaro.components.errors import (
     DatasetImportError,
     InvalidAnnotationError,
     InvalidFieldError,
     MissingFieldError,
@@ -194,14 +194,18 @@
                 if image is None:
                     image = images.pop(item_id, None)
 
                 if image or size:
                     image = Image.from_file(path=image, size=size)
 
                 yield DatasetItem(id=item_id, subset=self._subset, media=image, annotations=anns)
+
+                for ann in anns:
+                    self._ann_types.add(ann.type)
+
             except ElementTree.ParseError as e:
                 readable_wrapper = InvalidAnnotationError("Failed to parse XML file")
                 readable_wrapper.__cause__ = e
                 self._ctx.error_policy.report_item_error(
                     readable_wrapper, item_id=(item_id, self._subset)
                 )
             except Exception as e:
@@ -355,30 +359,36 @@
 
             for instance_id, label_id in instance_labels.items():
                 if len(label_cat) <= label_id:
                     self._ctx.error_policy.report_annotation_error(
                         UndeclaredLabelError(str(label_id)), item_id=(item_id, self._subset)
                     )
 
-                image = compiled_mask.lazy_extract(instance_id)
-
-                item_annotations.append(Mask(image=image, label=label_id, group=instance_id))
+                item_annotations.append(
+                    ExtractedMask(
+                        index_mask=instances_mask,
+                        index=instance_id,
+                        label=label_id,
+                        group=instance_id,
+                    )
+                )
         elif class_mask is not None:
             log.warning("Item %s: only class segmentations available", item_id)
 
-            class_mask = class_mask()
-            classes = np.unique(class_mask)
+            np_class_mask = class_mask()
+            classes = np.unique(np_class_mask)
             for label_id in classes:
                 if len(label_cat) <= label_id:
                     self._ctx.error_policy.report_annotation_error(
                         UndeclaredLabelError(str(label_id)), item_id=(item_id, self._subset)
                     )
 
-                image = self._lazy_extract_mask(class_mask, label_id)
-                item_annotations.append(Mask(image=image, label=label_id))
+                item_annotations.append(
+                    ExtractedMask(index_mask=class_mask, index=label_id, label=label_id)
+                )
 
         return item_annotations
 
     def _parse_labels(self) -> Dict[str, List[Label]]:
         annotations = {}
         task_dir = osp.dirname(self._path)
         for label_id, label in enumerate(self._categories[AnnotationType.label]):
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/voc/exporter.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/voc/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/voc/format.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/voc/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/voc/importer.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/voc/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/vott_csv.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/vott_csv.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,15 @@
 
                     x_min = float(x_min)
                     y_min = float(y_min)
                     w = float(x_max) - x_min
                     h = float(y_max) - y_min
 
                     annotations.append(Bbox(x_min, y_min, w, h, label=label_idx))
+                    self._ann_types.add(AnnotationType.bbox)
 
         return items
 
 
 class VottCsvImporter(Importer):
     @classmethod
     def find_sources(cls, path):
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/vott_json.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/vott_json.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,14 +87,15 @@
                                 float(bbox["top"]),
                                 float(bbox["width"]),
                                 float(bbox["height"]),
                                 label=label_idx,
                                 attributes={"id": region.get("id")},
                             )
                         )
+                        self._ann_types.add(AnnotationType.bbox)
 
             items[item_id] = DatasetItem(
                 id=item_id,
                 subset=self._subset,
                 attributes={"id": id},
                 media=Image.from_file(
                     path=osp.join(osp.dirname(path), asset.get("asset", {}).get("path"))
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/widerface.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/widerface.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,14 +113,15 @@
                 label_name = item_id.split("/")[0]
                 if "--" in label_name:
                     label_name = label_name.split("--")[1]
                 if label_name != WiderFacePath.IMAGES_DIR_NO_LABEL:
                     label = label_categories.find(label_name)[0]
                     if label is not None:
                         annotations.append(Label(label=label))
+                        self._ann_types.add(AnnotationType.label)
                 item_id = item_id[len(item_id.split("/")[0]) + 1 :]
 
             items[item_id] = DatasetItem(
                 id=item_id,
                 subset=self._subset,
                 media=Image.from_file(path=image_path),
                 annotations=annotations,
@@ -152,24 +153,25 @@
                             if bbox_list[i] != "-":
                                 if bbox_list[i] in ["True", "False"]:
                                     attributes[attr] = str_to_bool(bbox_list[i])
                                 else:
                                     attributes[attr] = bbox_list[i]
                             i += 1
 
-                    annotations.append(
+                    items[item_id].annotations.append(
                         Bbox(
                             float(bbox_list[0]),
                             float(bbox_list[1]),
                             float(bbox_list[2]),
                             float(bbox_list[3]),
                             attributes=attributes,
                             label=label,
                         )
                     )
+                    self._ann_types.add(AnnotationType.bbox)
 
         return items
 
 
 class WiderFaceImporter(Importer):
     _ANNO_EXT = ".txt"
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/yolo/base.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/yolo/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -284,14 +284,17 @@
     def __iter__(self) -> Iterator[DatasetItem]:
         subsets = self._subsets
         pbars = self._ctx.progress_reporter.split(len(subsets))
         for pbar, (subset_name, subset) in zip(pbars, subsets.items()):
             for item in pbar.iter(subset, desc=f"Importing '{subset_name}'"):
                 yield item
 
+                for ann in item.annotations:
+                    self._ann_types.add(ann.type)
+
     def __len__(self):
         return sum(len(s) for s in self._subsets.values())
 
     def get_subset(self, name):
         return self._subsets[name]
 
     @property
@@ -348,14 +351,17 @@
                 img = Image.from_file(path=self._img_files[fname])
                 anns = self._parse_annotations(
                     url,
                     img,
                     label_categories=label_categories,
                 )
                 yield DatasetItem(id=fname, subset=self._subset, media=img, annotations=anns)
+
+                for ann in anns:
+                    self._ann_types.add(ann.type)
             except Exception as e:
                 self._ctx.error_policy.report_item_error(e, item_id=(fname, self._subset))
 
     def __len__(self) -> int:
         return len(self._urls)
 
     def _get_rootpath(self, config_path: str) -> str:
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/yolo/exporter.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/yolo/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/yolo/format.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/yolo/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/data_formats/yolo/importer.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/data_formats/yolo/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/explorer.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/explorer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/framework_converter.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/framework_converter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/inference_server_plugin/base.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/inference_server_plugin/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/inference_server_plugin/ovms.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/inference_server_plugin/ovms.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/inference_server_plugin/samples/face_detection.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/inference_server_plugin/samples/face_detection.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/inference_server_plugin/triton.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/inference_server_plugin/triton.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/missing_annotation_detection.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/missing_annotation_detection.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/ndr.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/ndr.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/openvino_plugin/launcher.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/openvino_plugin/launcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/openvino_plugin/samples/clip_text_ViT-B_32_interp.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/openvino_plugin/samples/clip_text_ViT-B_32_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/openvino_plugin/samples/clip_visual_ViT-B_32_interp.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/openvino_plugin/samples/clip_visual_ViT-B_32_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/openvino_plugin/samples/coco.class` & `datumaro-1.7.0rc1/src/datumaro/plugins/openvino_plugin/samples/coco.class`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/openvino_plugin/samples/googlenet-v4-tf_interp.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/openvino_plugin/samples/googlenet-v4-tf_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/openvino_plugin/samples/imagenet.class` & `datumaro-1.7.0rc1/src/datumaro/plugins/openvino_plugin/samples/imagenet.class`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_atss_interp.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_atss_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_ssd_interp.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_ssd_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_yolox_interp.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_yolox_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/openvino_plugin/samples/utils.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/openvino_plugin/samples/utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/openvino_plugin/shift_launcher.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/openvino_plugin/shift_launcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/sam_transforms/automatic_mask_gen.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/sam_transforms/automatic_mask_gen.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/sam_transforms/bbox_to_inst_mask.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/sam_transforms/bbox_to_inst_mask.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/sam_transforms/interpreters/sam_decoder_for_amg.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/sam_transforms/interpreters/sam_decoder_for_amg.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/sam_transforms/interpreters/sam_decoder_for_bbox.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/sam_transforms/interpreters/sam_decoder_for_bbox.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/sam_transforms/interpreters/sam_encoder.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/sam_transforms/interpreters/sam_encoder.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/sampler/algorithm/algorithm.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/sampler/algorithm/algorithm.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/sampler/algorithm/entropy.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/sampler/algorithm/entropy.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/sampler/random_sampler.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/sampler/random_sampler.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/sampler/relevancy_sampler.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/sampler/relevancy_sampler.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/specs.json` & `datumaro-1.7.0rc1/src/datumaro/plugins/specs.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9856115107913669%*

 * *Differences: {'insert': "[(66, OrderedDict([('import_path', 'datumaro.plugins.data_formats.dota.DotaBase'), "*

 * *           "('plugin_name', 'dota'), ('plugin_type', 'DatasetBase')])), (67, "*

 * *           "OrderedDict([('import_path', 'datumaro.plugins.data_formats.dota.DotaExporter'), "*

 * *           "('plugin_name', 'dota'), ('plugin_type', 'Exporter')])), (68, "*

 * *           "OrderedDict([('import_path', 'datumaro.plugins.data_formats.dota.DotaImporter'), "*

 * *           "('plugin_name', 'dota'), ('plugin_type', 'Importer'), ('me […]*

```diff
@@ -456,14 +456,34 @@
                 ".datum"
             ]
         },
         "plugin_name": "datumaro_binary",
         "plugin_type": "Importer"
     },
     {
+        "import_path": "datumaro.plugins.data_formats.dota.DotaBase",
+        "plugin_name": "dota",
+        "plugin_type": "DatasetBase"
+    },
+    {
+        "import_path": "datumaro.plugins.data_formats.dota.DotaExporter",
+        "plugin_name": "dota",
+        "plugin_type": "Exporter"
+    },
+    {
+        "import_path": "datumaro.plugins.data_formats.dota.DotaImporter",
+        "metadata": {
+            "file_extensions": [
+                ".txt"
+            ]
+        },
+        "plugin_name": "dota",
+        "plugin_type": "Importer"
+    },
+    {
         "import_path": "datumaro.plugins.data_formats.icdar.base.IcdarTextLocalizationBase",
         "plugin_name": "icdar_text_localization",
         "plugin_type": "DatasetBase"
     },
     {
         "import_path": "datumaro.plugins.data_formats.icdar.base.IcdarTextLocalizationImporter",
         "metadata": {
@@ -1926,14 +1946,19 @@
     },
     {
         "import_path": "datumaro.plugins.transforms.Sort",
         "plugin_name": "sort",
         "plugin_type": "Transform"
     },
     {
+        "import_path": "datumaro.plugins.transforms.AstypeAnnotations",
+        "plugin_name": "astype_annotations",
+        "plugin_type": "Transform"
+    },
+    {
         "import_path": "datumaro.plugins.validators.ClassificationValidator",
         "plugin_name": "classification",
         "plugin_type": "Validator"
     },
     {
         "import_path": "datumaro.plugins.validators.DetectionValidator",
         "plugin_name": "detection",
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/specs.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/specs.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/splitter.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/splitter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/synthetic_data/background_colors.txt` & `datumaro-1.7.0rc1/src/datumaro/plugins/synthetic_data/background_colors.txt`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/synthetic_data/image_generator.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/synthetic_data/image_generator.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/synthetic_data/utils.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/synthetic_data/utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/tiling/merge_tile.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/tiling/merge_tile.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/tiling/tile.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/tiling/tile.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/tiling/util.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/tiling/util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/transforms.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/transforms.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2020-2021 Intel Corporation
+# Copyright (C) 2020-2024 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
 import argparse
 import logging as log
@@ -14,14 +14,15 @@
 from enum import Enum, auto
 from itertools import chain
 from typing import Dict, Iterable, List, Optional, Tuple, Union
 
 import cv2
 import numpy as np
 import pycocotools.mask as mask_utils
+from pandas.api.types import CategoricalDtype
 
 import datumaro.util.mask_tools as mask_tools
 from datumaro.components.annotation import (
     AnnotationType,
     Bbox,
     Caption,
     Ellipse,
@@ -33,16 +34,16 @@
     PointsCategories,
     Polygon,
     PolyLine,
     RleMask,
 )
 from datumaro.components.cli_plugin import CliPlugin
 from datumaro.components.dataset_base import DEFAULT_SUBSET_NAME, DatasetInfo, DatasetItem, IDataset
-from datumaro.components.errors import DatumaroError
-from datumaro.components.media import Image
+from datumaro.components.errors import DatumaroError, MediaTypeError
+from datumaro.components.media import Image, TableRow
 from datumaro.components.transformer import ItemTransform, Transform
 from datumaro.util import NOTSET, filter_dict, parse_json_file, parse_str_enum_value, take_by
 from datumaro.util.annotation_util import find_group_leader, find_instances
 
 
 class CropCoveredSegments(ItemTransform, CliPlugin):
     """
@@ -1443,7 +1444,101 @@
                     new_ann = ann.wrap(attributes=deepcopy(ann.attributes))
                     if ann.label in updated_attrs:
                         new_ann.attributes.update(
                             {attr_name: "" for attr_name in updated_attrs[ann.label]}
                         )
                     updated_anns.append(new_ann)
                 yield item.wrap(annotations=updated_anns)
+
+
+class AstypeAnnotations(ItemTransform):
+    """
+    Enables the conversion of annotation types for the categories and individual items within a dataset.|n
+    |n
+    Based on a specified mapping, it transforms the annotation types,|m
+    changing them to 'Label' if they are categorical, and to 'Caption' if they are of type string, float, or integer.|n
+    |n
+    Examples:|n
+        - Convert type of `title` annotation|n
+
+        .. code-block::
+
+        |s|s%(prog)s --mapping 'title:text'
+    """
+
+    @staticmethod
+    def _split_arg(s):
+        columns = s.split(",")
+        results = []
+        for column in columns:
+            parts = column.split(":")
+            if len(parts) != 2:
+                raise argparse.ArgumentTypeError()
+            results.append((parts[0], parts[1]))
+        return results
+
+    @classmethod
+    def build_cmdline_parser(cls, **kwargs):
+        parser = super().build_cmdline_parser(**kwargs)
+        parser.add_argument(
+            "--mapping",
+            action="append",
+            type=cls._split_arg,
+            dest="mapping",
+            help="Annotations type in the form of: '<src>:<dst>' (repeatable)",
+        )
+        return parser
+
+    def __init__(
+        self,
+        extractor: IDataset,
+        mapping: Optional[Union[Dict[str, str], List[Tuple[str, str]]]] = None,
+    ):
+        super().__init__(extractor)
+
+        if extractor.media_type() and not issubclass(extractor.media_type(), TableRow):
+            raise MediaTypeError(
+                "Media type is not table. This transform only support tabular media"
+            )
+
+        # Turn off for default setting
+        assert mapping is None or isinstance(mapping, (dict, list)), "Mapping must be dict, or list"
+        if isinstance(mapping, list):
+            mapping = dict(mapping)
+
+        self._categories = {}
+
+        src_categories = self._extractor.categories()
+        src_tabular_cat = src_categories.get(AnnotationType.tabular)
+        self._tabular_cat_types = {}
+
+        # Make LabelCategories
+        self._id_mapping = {}
+        dst_label_cat = LabelCategories()
+
+        if src_tabular_cat is None:
+            return
+
+        for src_cat in src_tabular_cat:
+            if src_cat.dtype == CategoricalDtype():
+                dst_parent = src_cat.name
+                dst_labels = sorted(src_cat.labels)
+                for dst_label in dst_labels:
+                    dst_index = dst_label_cat.add(dst_label, parent=dst_parent, attributes={})
+                    self._id_mapping[dst_label] = dst_index
+                dst_label_cat.add_label_group(src_cat.name, src_cat.labels, group_type=0)
+            self._tabular_cat_types[src_cat.name] = src_cat.dtype
+        self._categories[AnnotationType.label] = dst_label_cat
+
+    def categories(self):
+        return self._categories
+
+    def transform_item(self, item: DatasetItem):
+        annotations = []
+        for name, value in item.annotations[0].values.items():
+            dtype = self._tabular_cat_types.get(name, None)
+            if dtype == CategoricalDtype():
+                annotations.append(Label(label=self._id_mapping[value]))
+            else:
+                annotations.append(Caption(value))
+
+        return self.wrap_item(item, annotations=annotations)
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/plugins/validators.py` & `datumaro-1.7.0rc1/src/datumaro/plugins/validators.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/util/__init__.py` & `datumaro-1.7.0rc1/src/datumaro/util/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/util/annotation_util.py` & `datumaro-1.7.0rc1/src/datumaro/util/annotation_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/util/attrs_util.py` & `datumaro-1.7.0rc1/src/datumaro/util/attrs_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/util/definitions.py` & `datumaro-1.7.0rc1/src/datumaro/util/definitions.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/util/file_utils.py` & `datumaro-1.7.0rc1/src/datumaro/util/file_utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/util/image.py` & `datumaro-1.7.0rc1/src/datumaro/util/image.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,27 +6,29 @@
 import os
 import os.path as osp
 import shlex
 import weakref
 from contextlib import contextmanager
 from contextvars import ContextVar
 from enum import Enum, auto
+from functools import partial
 from io import BytesIO, IOBase
 from typing import TYPE_CHECKING, Any, Callable, Dict, Iterable, Iterator, Optional, Tuple, Union
 
 import numpy as np
 
 from datumaro.components.crypter import NULL_CRYPTER, Crypter
 from datumaro.components.errors import DatumaroError
 
-try:
-    # Introduced in 1.20
-    from numpy.typing import DTypeLike
-except ImportError:
-    DTypeLike = Any
+if TYPE_CHECKING:
+    try:
+        # Introduced in 1.20
+        from numpy.typing import DTypeLike
+    except ImportError:
+        DTypeLike = Any
 
 
 class ImageBackend(Enum):
     cv2 = auto()
     PIL = auto()
 
 
@@ -41,17 +43,14 @@
 
     IMAGE_BACKEND.set(ImageBackend.PIL)
     _image_loading_errors = (*_image_loading_errors, PIL.UnidentifiedImageError)
 
 from datumaro.util.image_cache import ImageCache
 from datumaro.util.os_util import find_files
 
-if TYPE_CHECKING:
-    from PIL.Image import Image as PILImage
-
 
 class ImageColorChannel(Enum):
     """Image color channel
 
     - UNCHANGED: Use the original image's channel (default)
     - COLOR_BGR: Use BGR 3 channels (it can ignore the alpha channel or convert the gray scale image)
     - COLOR_RGB: Use RGB 3 channels (it can ignore the alpha channel or convert the gray scale image)
@@ -74,28 +73,29 @@
             return img
 
         if self == ImageColorChannel.COLOR_RGB:
             return cv2.cvtColor(img, cv2.COLOR_BGR2RGB)
 
         raise ValueError
 
-    def decode_by_pil(self, image_bytes: bytes) -> PILImage:
+    def decode_by_pil(self, image_bytes: bytes) -> np.ndarray:
         """Convert image color channel for PIL Image."""
         from PIL import Image
 
         img = Image.open(BytesIO(image_bytes))
 
         if self == ImageColorChannel.UNCHANGED:
-            return img
+            return np.asarray(img)
 
         if self == ImageColorChannel.COLOR_BGR:
-            return Image.fromarray(np.flip(np.asarray(img.convert("RGB")), -1))
+            img = np.asarray(img.convert("RGB"))
+            return cv2.cvtColor(img, cv2.COLOR_RGB2BGR)
 
         if self == ImageColorChannel.COLOR_RGB:
-            return img.convert("RGB")
+            return np.asarray(img.convert("RGB"))
 
         raise ValueError
 
 
 IMAGE_COLOR_CHANNEL: ContextVar[ImageColorChannel] = ContextVar(
     "IMAGE_COLOR_CHANNEL", default=ImageColorChannel.UNCHANGED
 )
@@ -284,21 +284,21 @@
 
 
 def decode_image(image_bytes: bytes, dtype: DTypeLike = np.uint8) -> np.ndarray:
     ctx_color_scale = IMAGE_COLOR_CHANNEL.get()
 
     if IMAGE_BACKEND.get() == ImageBackend.cv2:
         image = ctx_color_scale.decode_by_cv2(image_bytes)
-        image = image.astype(dtype)
     elif IMAGE_BACKEND.get() == ImageBackend.PIL:
         image = ctx_color_scale.decode_by_pil(image_bytes)
-        image = np.asarray(image, dtype=dtype)
     else:
         raise NotImplementedError()
 
+    image = image.astype(dtype)
+
     assert len(image.shape) in {2, 3}
     if len(image.shape) == 3:
         assert image.shape[2] in {3, 4}
     return image
 
 
 IMAGE_EXTENSIONS = {
@@ -351,26 +351,27 @@
 class lazy_image:
     def __init__(
         self,
         path: str,
         loader: Callable[[str], np.ndarray] = None,
         cache: Union[bool, ImageCache] = True,
         crypter: Crypter = NULL_CRYPTER,
+        dtype: Optional[DTypeLike] = None,
     ) -> None:
         """
         Cache:
             - False: do not cache
             - True: use the global cache
             - ImageCache instance: an object to be used as cache
         """
 
         self._custom_loader = True
 
         if loader is None:
-            loader = load_image
+            loader = partial(load_image, dtype=dtype) if dtype else load_image
             self._custom_loader = False
 
         self._path = path
         self._loader = loader
 
         assert isinstance(cache, (ImageCache, bool))
         self._cache = cache
```

### Comparing `datumaro-1.6.1rc3/src/datumaro/util/image_cache.py` & `datumaro-1.7.0rc1/src/datumaro/util/image_cache.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/util/log_utils.py` & `datumaro-1.7.0rc1/src/datumaro/util/log_utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/util/mask_tools.py` & `datumaro-1.7.0rc1/src/datumaro/util/mask_tools.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/util/meta_file_util.py` & `datumaro-1.7.0rc1/src/datumaro/util/meta_file_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/util/multi_procs_util.py` & `datumaro-1.7.0rc1/src/datumaro/util/multi_procs_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/util/os_util.py` & `datumaro-1.7.0rc1/src/datumaro/util/os_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/util/pickle_util.py` & `datumaro-1.7.0rc1/src/datumaro/util/pickle_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/util/scope.py` & `datumaro-1.7.0rc1/src/datumaro/util/scope.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/util/telemetry_stub.py` & `datumaro-1.7.0rc1/src/datumaro/util/telemetry_stub.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/util/telemetry_utils.py` & `datumaro-1.7.0rc1/src/datumaro/util/telemetry_utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro/util/tf_util.py` & `datumaro-1.7.0rc1/src/datumaro/util/tf_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.1rc3/src/datumaro.egg-info/PKG-INFO` & `datumaro-1.7.0rc1/src/datumaro.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datumaro
-Version: 1.6.1rc3
+Version: 1.7.0rc1
 Summary: Dataset Management Framework (Datumaro)
 Home-page: https://github.com/openvinotoolkit/datumaro
 Author: Intel
 Author-email: emily.chun@intel.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,27 +17,27 @@
 Requires-Dist: h5py>=2.10.0
 Requires-Dist: imagesize>=1.4.1
 Requires-Dist: lxml<6,>=5.2.0
 Requires-Dist: matplotlib>=3.3.1
 Requires-Dist: networkx>=2.6
 Requires-Dist: nibabel>=3.2.1
 Requires-Dist: numpy<2,>=1.23.4
-Requires-Dist: orjson==3.10.0
-Requires-Dist: Pillow>=10.2.0
+Requires-Dist: orjson==3.10.3
+Requires-Dist: Pillow>=10.3.0
 Requires-Dist: ruamel.yaml>=0.17.0
 Requires-Dist: shapely>=1.7
 Requires-Dist: typing_extensions>=3.7.4.3
 Requires-Dist: tqdm
 Requires-Dist: pycocotools>=2.0.4; platform_system != "Windows" or python_version >= "3.9"
 Requires-Dist: pycocotools-windows; platform_system == "Windows" and python_version < "3.9"
 Requires-Dist: PyYAML==6.0.1
 Requires-Dist: tensorboardX!=2.3,>=1.8
 Requires-Dist: scipy
 Requires-Dist: requests
-Requires-Dist: pandas~=1.4.0
+Requires-Dist: pandas>=1.4.0
 Requires-Dist: openvino>=2023.2.0
 Requires-Dist: tokenizers
 Requires-Dist: cryptography>=38.03
 Requires-Dist: pyemd
 Requires-Dist: pyarrow
 Requires-Dist: protobuf
 Requires-Dist: tabulate
@@ -46,16 +46,14 @@
 Requires-Dist: scikit-learn
 Requires-Dist: json-stream
 Requires-Dist: opencv-python
 Provides-Extra: tf
 Requires-Dist: tensorflow; extra == "tf"
 Provides-Extra: tfds
 Requires-Dist: tensorflow-datasets<4.9.3; extra == "tfds"
-Provides-Extra: tf-gpu
-Requires-Dist: tensorflow-gpu; extra == "tf-gpu"
 Provides-Extra: torch
 Requires-Dist: torch; extra == "torch"
 Requires-Dist: torchvision; extra == "torch"
 Provides-Extra: default
 Requires-Dist: dvc==3.49.0; extra == "default"
 Requires-Dist: fsspec<=2022.11.0; python_version < "3.8" and extra == "default"
 Requires-Dist: GitPython!=3.1.25,>=3.1.18; extra == "default"
```

### Comparing `datumaro-1.6.1rc3/src/datumaro.egg-info/SOURCES.txt` & `datumaro-1.7.0rc1/src/datumaro.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,19 @@
 src/datumaro/cli/commands/info.py
 src/datumaro/cli/commands/merge.py
 src/datumaro/cli/commands/patch.py
 src/datumaro/cli/commands/prune.py
 src/datumaro/cli/commands/stats.py
 src/datumaro/cli/commands/transform.py
 src/datumaro/cli/commands/validate.py
+src/datumaro/cli/commands/downloaders/__init__.py
+src/datumaro/cli/commands/downloaders/downloader.py
+src/datumaro/cli/commands/downloaders/kaggle.py
+src/datumaro/cli/commands/downloaders/kaggle_formats.json
+src/datumaro/cli/commands/downloaders/tfds.py
 src/datumaro/cli/commands/require_project/__init__.py
 src/datumaro/cli/commands/require_project/modification/__init__.py
 src/datumaro/cli/commands/require_project/modification/add.py
 src/datumaro/cli/commands/require_project/modification/create.py
 src/datumaro/cli/commands/require_project/modification/export.py
 src/datumaro/cli/commands/require_project/modification/import_.py
 src/datumaro/cli/commands/require_project/modification/remove.py
@@ -146,14 +151,15 @@
 src/datumaro/plugins/data_formats/brats.py
 src/datumaro/plugins/data_formats/brats_numpy.py
 src/datumaro/plugins/data_formats/camvid.py
 src/datumaro/plugins/data_formats/cifar.py
 src/datumaro/plugins/data_formats/cityscapes.py
 src/datumaro/plugins/data_formats/common_semantic_segmentation.py
 src/datumaro/plugins/data_formats/common_super_resolution.py
+src/datumaro/plugins/data_formats/dota.py
 src/datumaro/plugins/data_formats/image_dir.py
 src/datumaro/plugins/data_formats/image_zip.py
 src/datumaro/plugins/data_formats/imagenet.py
 src/datumaro/plugins/data_formats/imagenet_txt.py
 src/datumaro/plugins/data_formats/kinetics.py
 src/datumaro/plugins/data_formats/labelme.py
 src/datumaro/plugins/data_formats/lfw.py
```

### Comparing `datumaro-1.6.1rc3/src/datumaro.egg-info/requires.txt` & `datumaro-1.7.0rc1/src/datumaro.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 h5py>=2.10.0
 imagesize>=1.4.1
 lxml<6,>=5.2.0
 matplotlib>=3.3.1
 networkx>=2.6
 nibabel>=3.2.1
 numpy<2,>=1.23.4
-orjson==3.10.0
-Pillow>=10.2.0
+orjson==3.10.3
+Pillow>=10.3.0
 ruamel.yaml>=0.17.0
 shapely>=1.7
 typing_extensions>=3.7.4.3
 tqdm
 PyYAML==6.0.1
 tensorboardX!=2.3,>=1.8
 scipy
 requests
-pandas~=1.4.0
+pandas>=1.4.0
 openvino>=2023.2.0
 tokenizers
 cryptography>=38.03
 pyemd
 pyarrow
 protobuf
 tabulate
@@ -45,16 +45,13 @@
 
 [default:python_version < "3.8"]
 fsspec<=2022.11.0
 
 [tf]
 tensorflow
 
-[tf-gpu]
-tensorflow-gpu
-
 [tfds]
 tensorflow-datasets<4.9.3
 
 [torch]
 torch
 torchvision
```

