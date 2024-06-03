# Comparing `tmp/dvcx-0.85.1.tar.gz` & `tmp/dvcx-0.86.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvcx-0.85.1.tar", last modified: Thu May 30 03:40:38 2024, max compression
+gzip compressed data, was "dvcx-0.86.0.tar", last modified: Mon Jun  3 09:33:59 2024, max compression
```

## Comparing `dvcx-0.85.1.tar` & `dvcx-0.86.0.tar`

### file list

```diff
@@ -1,253 +1,253 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:38.359616 dvcx-0.85.1/
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-30 03:40:30.000000 dvcx-0.85.1/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-30 03:40:30.000000 dvcx-0.85.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:38.311616 dvcx-0.85.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:38.311616 dvcx-0.85.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-30 03:40:30.000000 dvcx-0.85.1/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-30 03:40:30.000000 dvcx-0.85.1/.github/ISSUE_TEMPLATE/empty_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-30 03:40:30.000000 dvcx-0.85.1/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-30 03:40:30.000000 dvcx-0.85.1/.github/codecov.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-30 03:40:30.000000 dvcx-0.85.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:38.311616 dvcx-0.85.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-30 03:40:30.000000 dvcx-0.85.1/.github/workflows/benchmarks.yml
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-30 03:40:30.000000 dvcx-0.85.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-05-30 03:40:30.000000 dvcx-0.85.1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-30 03:40:30.000000 dvcx-0.85.1/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-05-30 03:40:30.000000 dvcx-0.85.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-30 03:40:30.000000 dvcx-0.85.1/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:38.311616 dvcx-0.85.1/.reuse/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-30 03:40:30.000000 dvcx-0.85.1/.reuse/dep5
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-30 03:40:30.000000 dvcx-0.85.1/.safety-policy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-05-30 03:40:30.000000 dvcx-0.85.1/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-30 03:40:30.000000 dvcx-0.85.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-30 03:40:30.000000 dvcx-0.85.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:38.311616 dvcx-0.85.1/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-05-30 03:40:30.000000 dvcx-0.85.1/LICENSES/Apache-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-30 03:40:30.000000 dvcx-0.85.1/LICENSES/BSD-3-Clause.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9411 2024-05-30 03:40:30.000000 dvcx-0.85.1/LICENSES/Python-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6669 2024-05-30 03:40:38.355616 dvcx-0.85.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-05-30 03:40:30.000000 dvcx-0.85.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:38.311616 dvcx-0.85.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     6987 2024-05-30 03:40:30.000000 dvcx-0.85.1/docs/cv_intro.md
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-30 03:40:30.000000 dvcx-0.85.1/docs/udfs.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:38.315616 dvcx-0.85.1/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/blip2_image_desc_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/clip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/common_sql_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/dir_expansion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/hf_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/iptc_exif_xmp_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/llava2_image_desc_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/llm-claude-aggregate-query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/llm-claude-simple-query.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/llm-claude.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:38.315616 dvcx-0.85.1/examples/neurips/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/neurips/README
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/neurips/distance_to_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/neurips/llm_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/neurips/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/neurips/single_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/neurips/text_loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/openai_image_desc_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/openimage-detect.py
--rw-r--r--   0 runner    (1001) docker     (127)     6942 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/pose_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/torch-loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:38.319616 dvcx-0.85.1/examples/udfs/
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/udfs/batching.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/udfs/image_transformation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/udfs/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/udfs/simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/udfs/stateful.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/udfs/stateful_similarity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/unstructured-text.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/wds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/wds_filtered.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/wds_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:38.319616 dvcx-0.85.1/examples/zalando/
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/zalando/zalando_clip.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/zalando/zalando_dir_as_class.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/zalando/zalando_splits_and_classes_ds.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/zalando/zalando_splits_and_classes_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-30 03:40:30.000000 dvcx-0.85.1/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-05-30 03:40:30.000000 dvcx-0.85.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 03:40:38.359616 dvcx-0.85.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:38.303616 dvcx-0.85.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:38.323616 dvcx-0.85.1/src/dvcx/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-30 03:40:38.000000 dvcx-0.85.1/src/dvcx/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     7641 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/asyn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:38.323616 dvcx-0.85.1/src/dvcx/catalog/
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    73445 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/catalog/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/catalog/datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/catalog/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    31848 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/cli_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:38.323616 dvcx-0.85.1/src/dvcx/client/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/client/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/client/fileslice.py
--rw-r--r--   0 runner    (1001) docker     (127)    12012 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/client/fsspec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/client/gcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/client/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/client/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:38.327616 dvcx-0.85.1/src/dvcx/data_storage/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/data_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/data_storage/db_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/data_storage/id_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    46118 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/data_storage/metastore.py
--rw-r--r--   0 runner    (1001) docker     (127)    10884 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/data_storage/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/data_storage/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)    24815 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/data_storage/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)    31653 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/data_storage/warehouse.py
--rw-r--r--   0 runner    (1001) docker     (127)    16157 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:38.331616 dvcx-0.85.1/src/dvcx/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/lib/cached_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/lib/claude.py
--rw-r--r--   0 runner    (1001) docker     (127)    16438 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/lib/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    10195 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/lib/feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/lib/feature_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    10249 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/lib/feature_udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/lib/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/lib/gpt4_vision.py
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/lib/hf_image_to_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/lib/hf_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/lib/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/lib/image_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/lib/iptc_exif_xmp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/lib/pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/lib/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/lib/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     7782 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/lib/udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/lib/unstructured.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/lib/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/lib/vfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     8406 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/lib/webdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/lib/webdataset_laion.py
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/lib/webdataset_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     8123 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/listing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/node.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/nodes_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/nodes_thread_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     4550 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:38.331616 dvcx-0.85.1/src/dvcx/query/
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/query/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/query/builtins.py
--rw-r--r--   0 runner    (1001) docker     (127)    61615 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/query/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    13098 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/query/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/query/params.py
--rw-r--r--   0 runner    (1001) docker     (127)     7507 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/query/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/query/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/query/udf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:38.335616 dvcx-0.85.1/src/dvcx/remote/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7418 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/remote/studio.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:38.335616 dvcx-0.85.1/src/dvcx/sql/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/sql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:38.335616 dvcx-0.85.1/src/dvcx/sql/default/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/sql/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/sql/default/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:38.335616 dvcx-0.85.1/src/dvcx/sql/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/sql/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/sql/functions/array.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/sql/functions/conditional.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/sql/functions/path.py
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/sql/functions/random.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/sql/functions/string.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/sql/selectable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:38.335616 dvcx-0.85.1/src/dvcx/sql/sqlite/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/sql/sqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10930 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/sql/sqlite/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/sql/sqlite/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/sql/sqlite/vector.py
--rw-r--r--   0 runner    (1001) docker     (127)    10234 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/sql/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/sql/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    10242 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:38.351616 dvcx-0.85.1/src/dvcx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6669 2024-05-30 03:40:38.000000 dvcx-0.85.1/src/dvcx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5970 2024-05-30 03:40:38.000000 dvcx-0.85.1/src/dvcx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 03:40:38.000000 dvcx-0.85.1/src/dvcx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-30 03:40:38.000000 dvcx-0.85.1/src/dvcx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-30 03:40:38.000000 dvcx-0.85.1/src/dvcx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-30 03:40:38.000000 dvcx-0.85.1/src/dvcx.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:38.339616 dvcx-0.85.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:38.339616 dvcx-0.85.1/tests/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/benchmarks/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/benchmarks/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/benchmarks/test_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    16373 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4947 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:38.339616 dvcx-0.85.1/tests/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/func/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35240 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/func/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/func/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)   112436 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/func/test_dataset_query.py
--rw-r--r--   0 runner    (1001) docker     (127)    29281 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/func/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    10558 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/func/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (127)    10291 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/func/test_pull.py
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/func/test_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     9017 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/func/test_query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:38.343616 dvcx-0.85.1/tests/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/scripts/name_len_normal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/scripts/name_len_slow.py
--rw-r--r--   0 runner    (1001) docker     (127)     6472 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/test_cli_e2e.py
--rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/test_query_e2e.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:38.347616 dvcx-0.85.1/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:38.347616 dvcx-0.85.1/tests/unit/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/lib/test_cached_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    15029 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/lib/test_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)    10158 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/lib/test_feature_udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/lib/test_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/lib/test_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/lib/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/lib/test_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/lib/test_webdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/lib/test_webdataset_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:38.351616 dvcx-0.85.1/tests/unit/sql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/sql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:38.351616 dvcx-0.85.1/tests/unit/sql/sqlite/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/sql/sqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/sql/sqlite/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/sql/test_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/sql/test_conditional.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/sql/test_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/sql/test_random.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/sql/test_selectable.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/sql/test_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/test_asyn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/test_catalog_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/test_cli_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/test_client_s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/test_data_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/test_database_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/test_dataset_row.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/test_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/test_fileslice.py
--rw-r--r--   0 runner    (1001) docker     (127)     5902 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/test_id_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/test_listing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/test_metastore.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/test_query_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/test_serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     6790 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/test_udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/test_warehouse.py
--rw-r--r--   0 runner    (1001) docker     (127)     7657 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:33:59.432520 dvcx-0.86.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-06-03 09:33:53.000000 dvcx-0.86.0/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-06-03 09:33:53.000000 dvcx-0.86.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:33:59.384519 dvcx-0.86.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:33:59.384519 dvcx-0.86.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-06-03 09:33:53.000000 dvcx-0.86.0/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-06-03 09:33:53.000000 dvcx-0.86.0/.github/ISSUE_TEMPLATE/empty_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-06-03 09:33:53.000000 dvcx-0.86.0/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-06-03 09:33:53.000000 dvcx-0.86.0/.github/codecov.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-06-03 09:33:53.000000 dvcx-0.86.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:33:59.384519 dvcx-0.86.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-06-03 09:33:53.000000 dvcx-0.86.0/.github/workflows/benchmarks.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-06-03 09:33:53.000000 dvcx-0.86.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-06-03 09:33:53.000000 dvcx-0.86.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-06-03 09:33:53.000000 dvcx-0.86.0/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-06-03 09:33:53.000000 dvcx-0.86.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-06-03 09:33:53.000000 dvcx-0.86.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:33:59.384519 dvcx-0.86.0/.reuse/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-06-03 09:33:53.000000 dvcx-0.86.0/.reuse/dep5
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-06-03 09:33:53.000000 dvcx-0.86.0/.safety-policy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-06-03 09:33:53.000000 dvcx-0.86.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-06-03 09:33:53.000000 dvcx-0.86.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-06-03 09:33:53.000000 dvcx-0.86.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:33:59.384519 dvcx-0.86.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-06-03 09:33:53.000000 dvcx-0.86.0/LICENSES/Apache-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-06-03 09:33:53.000000 dvcx-0.86.0/LICENSES/BSD-3-Clause.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9411 2024-06-03 09:33:53.000000 dvcx-0.86.0/LICENSES/Python-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6669 2024-06-03 09:33:59.432520 dvcx-0.86.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-06-03 09:33:53.000000 dvcx-0.86.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:33:59.384519 dvcx-0.86.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6987 2024-06-03 09:33:53.000000 dvcx-0.86.0/docs/cv_intro.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-06-03 09:33:53.000000 dvcx-0.86.0/docs/udfs.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:33:59.388519 dvcx-0.86.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-06-03 09:33:53.000000 dvcx-0.86.0/examples/blip2_image_desc_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-06-03 09:33:53.000000 dvcx-0.86.0/examples/clip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-06-03 09:33:53.000000 dvcx-0.86.0/examples/common_sql_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-06-03 09:33:53.000000 dvcx-0.86.0/examples/dir_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-06-03 09:33:53.000000 dvcx-0.86.0/examples/hf_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-06-03 09:33:53.000000 dvcx-0.86.0/examples/iptc_exif_xmp_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-06-03 09:33:53.000000 dvcx-0.86.0/examples/llava2_image_desc_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-06-03 09:33:53.000000 dvcx-0.86.0/examples/llm-claude-aggregate-query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-06-03 09:33:53.000000 dvcx-0.86.0/examples/llm-claude-simple-query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-06-03 09:33:53.000000 dvcx-0.86.0/examples/llm-claude.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-06-03 09:33:53.000000 dvcx-0.86.0/examples/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:33:59.388519 dvcx-0.86.0/examples/neurips/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-06-03 09:33:53.000000 dvcx-0.86.0/examples/neurips/README
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-06-03 09:33:53.000000 dvcx-0.86.0/examples/neurips/distance_to_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-06-03 09:33:53.000000 dvcx-0.86.0/examples/neurips/llm_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-06-03 09:33:53.000000 dvcx-0.86.0/examples/neurips/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-06-03 09:33:53.000000 dvcx-0.86.0/examples/neurips/single_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-06-03 09:33:53.000000 dvcx-0.86.0/examples/neurips/text_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-06-03 09:33:53.000000 dvcx-0.86.0/examples/openai_image_desc_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-06-03 09:33:53.000000 dvcx-0.86.0/examples/openimage-detect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6942 2024-06-03 09:33:53.000000 dvcx-0.86.0/examples/pose_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-06-03 09:33:53.000000 dvcx-0.86.0/examples/torch-loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:33:59.392519 dvcx-0.86.0/examples/udfs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-06-03 09:33:53.000000 dvcx-0.86.0/examples/udfs/batching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-06-03 09:33:53.000000 dvcx-0.86.0/examples/udfs/image_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-06-03 09:33:53.000000 dvcx-0.86.0/examples/udfs/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-06-03 09:33:53.000000 dvcx-0.86.0/examples/udfs/simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-06-03 09:33:53.000000 dvcx-0.86.0/examples/udfs/stateful.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-06-03 09:33:53.000000 dvcx-0.86.0/examples/udfs/stateful_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-06-03 09:33:53.000000 dvcx-0.86.0/examples/unstructured-text.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-06-03 09:33:53.000000 dvcx-0.86.0/examples/wds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-06-03 09:33:53.000000 dvcx-0.86.0/examples/wds_filtered.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-06-03 09:33:53.000000 dvcx-0.86.0/examples/wds_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:33:59.392519 dvcx-0.86.0/examples/zalando/
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-06-03 09:33:53.000000 dvcx-0.86.0/examples/zalando/zalando_clip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-06-03 09:33:53.000000 dvcx-0.86.0/examples/zalando/zalando_dir_as_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-06-03 09:33:53.000000 dvcx-0.86.0/examples/zalando/zalando_splits_and_classes_ds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-06-03 09:33:53.000000 dvcx-0.86.0/examples/zalando/zalando_splits_and_classes_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-06-03 09:33:53.000000 dvcx-0.86.0/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-06-03 09:33:53.000000 dvcx-0.86.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 09:33:59.432520 dvcx-0.86.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:33:59.376519 dvcx-0.86.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:33:59.396519 dvcx-0.86.0/src/dvcx/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-06-03 09:33:59.000000 dvcx-0.86.0/src/dvcx/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7641 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/asyn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:33:59.396519 dvcx-0.86.0/src/dvcx/catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73580 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/catalog/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/catalog/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/catalog/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31848 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/cli_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:33:59.400519 dvcx-0.86.0/src/dvcx/client/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/client/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/client/fileslice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12012 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/client/fsspec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/client/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5171 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/client/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/client/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:33:59.400519 dvcx-0.86.0/src/dvcx/data_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/data_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/data_storage/db_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/data_storage/id_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46118 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/data_storage/metastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10853 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/data_storage/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/data_storage/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24530 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/data_storage/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32022 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/data_storage/warehouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16157 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:33:59.404519 dvcx-0.86.0/src/dvcx/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/lib/cached_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/lib/claude.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16438 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/lib/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10195 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/lib/feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/lib/feature_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10249 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/lib/feature_udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/lib/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/lib/gpt4_vision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/lib/hf_image_to_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/lib/hf_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/lib/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/lib/image_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/lib/iptc_exif_xmp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/lib/pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/lib/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/lib/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7782 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/lib/udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/lib/unstructured.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/lib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/lib/vfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8406 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/lib/webdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/lib/webdataset_laion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/lib/webdataset_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8123 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/listing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/nodes_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/nodes_thread_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4550 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:33:59.408519 dvcx-0.86.0/src/dvcx/query/
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/query/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/query/builtins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61221 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/query/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13098 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/query/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/query/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7507 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/query/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/query/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/query/udf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:33:59.408519 dvcx-0.86.0/src/dvcx/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7418 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/remote/studio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:33:59.408519 dvcx-0.86.0/src/dvcx/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/sql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:33:59.408519 dvcx-0.86.0/src/dvcx/sql/default/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/sql/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/sql/default/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:33:59.408519 dvcx-0.86.0/src/dvcx/sql/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/sql/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/sql/functions/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/sql/functions/conditional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/sql/functions/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/sql/functions/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/sql/functions/string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/sql/selectable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:33:59.412519 dvcx-0.86.0/src/dvcx/sql/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/sql/sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10930 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/sql/sqlite/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/sql/sqlite/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/sql/sqlite/vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10234 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/sql/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/sql/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10242 2024-06-03 09:33:53.000000 dvcx-0.86.0/src/dvcx/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:33:59.424519 dvcx-0.86.0/src/dvcx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6669 2024-06-03 09:33:59.000000 dvcx-0.86.0/src/dvcx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5970 2024-06-03 09:33:59.000000 dvcx-0.86.0/src/dvcx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 09:33:59.000000 dvcx-0.86.0/src/dvcx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-06-03 09:33:59.000000 dvcx-0.86.0/src/dvcx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-06-03 09:33:59.000000 dvcx-0.86.0/src/dvcx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-06-03 09:33:59.000000 dvcx-0.86.0/src/dvcx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:33:59.412519 dvcx-0.86.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-06-03 09:33:53.000000 dvcx-0.86.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:33:59.412519 dvcx-0.86.0/tests/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:33:53.000000 dvcx-0.86.0/tests/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-06-03 09:33:53.000000 dvcx-0.86.0/tests/benchmarks/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-06-03 09:33:53.000000 dvcx-0.86.0/tests/benchmarks/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-06-03 09:33:53.000000 dvcx-0.86.0/tests/benchmarks/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16373 2024-06-03 09:33:53.000000 dvcx-0.86.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4947 2024-06-03 09:33:53.000000 dvcx-0.86.0/tests/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:33:59.416519 dvcx-0.86.0/tests/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:33:53.000000 dvcx-0.86.0/tests/func/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35240 2024-06-03 09:33:53.000000 dvcx-0.86.0/tests/func/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-06-03 09:33:53.000000 dvcx-0.86.0/tests/func/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)   112236 2024-06-03 09:33:53.000000 dvcx-0.86.0/tests/func/test_dataset_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29281 2024-06-03 09:33:53.000000 dvcx-0.86.0/tests/func/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10558 2024-06-03 09:33:53.000000 dvcx-0.86.0/tests/func/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10291 2024-06-03 09:33:53.000000 dvcx-0.86.0/tests/func/test_pull.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-06-03 09:33:53.000000 dvcx-0.86.0/tests/func/test_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9017 2024-06-03 09:33:53.000000 dvcx-0.86.0/tests/func/test_query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:33:59.416519 dvcx-0.86.0/tests/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-06-03 09:33:53.000000 dvcx-0.86.0/tests/scripts/name_len_normal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-06-03 09:33:53.000000 dvcx-0.86.0/tests/scripts/name_len_slow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6472 2024-06-03 09:33:53.000000 dvcx-0.86.0/tests/test_cli_e2e.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-06-03 09:33:53.000000 dvcx-0.86.0/tests/test_query_e2e.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:33:59.420519 dvcx-0.86.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:33:53.000000 dvcx-0.86.0/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:33:59.420519 dvcx-0.86.0/tests/unit/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:33:53.000000 dvcx-0.86.0/tests/unit/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-06-03 09:33:53.000000 dvcx-0.86.0/tests/unit/lib/test_cached_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15029 2024-06-03 09:33:53.000000 dvcx-0.86.0/tests/unit/lib/test_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10158 2024-06-03 09:33:53.000000 dvcx-0.86.0/tests/unit/lib/test_feature_udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-06-03 09:33:53.000000 dvcx-0.86.0/tests/unit/lib/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-06-03 09:33:53.000000 dvcx-0.86.0/tests/unit/lib/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-06-03 09:33:53.000000 dvcx-0.86.0/tests/unit/lib/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-06-03 09:33:53.000000 dvcx-0.86.0/tests/unit/lib/test_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-06-03 09:33:53.000000 dvcx-0.86.0/tests/unit/lib/test_webdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-06-03 09:33:53.000000 dvcx-0.86.0/tests/unit/lib/test_webdataset_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:33:59.424519 dvcx-0.86.0/tests/unit/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:33:53.000000 dvcx-0.86.0/tests/unit/sql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:33:59.424519 dvcx-0.86.0/tests/unit/sql/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:33:53.000000 dvcx-0.86.0/tests/unit/sql/sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-06-03 09:33:53.000000 dvcx-0.86.0/tests/unit/sql/sqlite/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-06-03 09:33:53.000000 dvcx-0.86.0/tests/unit/sql/test_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-06-03 09:33:53.000000 dvcx-0.86.0/tests/unit/sql/test_conditional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-06-03 09:33:53.000000 dvcx-0.86.0/tests/unit/sql/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-06-03 09:33:53.000000 dvcx-0.86.0/tests/unit/sql/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-06-03 09:33:53.000000 dvcx-0.86.0/tests/unit/sql/test_selectable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-06-03 09:33:53.000000 dvcx-0.86.0/tests/unit/sql/test_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-06-03 09:33:53.000000 dvcx-0.86.0/tests/unit/test_asyn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-06-03 09:33:53.000000 dvcx-0.86.0/tests/unit/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-06-03 09:33:53.000000 dvcx-0.86.0/tests/unit/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-06-03 09:33:53.000000 dvcx-0.86.0/tests/unit/test_catalog_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-06-03 09:33:53.000000 dvcx-0.86.0/tests/unit/test_cli_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-06-03 09:33:53.000000 dvcx-0.86.0/tests/unit/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-06-03 09:33:53.000000 dvcx-0.86.0/tests/unit/test_client_s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-06-03 09:33:53.000000 dvcx-0.86.0/tests/unit/test_data_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-06-03 09:33:53.000000 dvcx-0.86.0/tests/unit/test_database_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-06-03 09:33:53.000000 dvcx-0.86.0/tests/unit/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-06-03 09:33:53.000000 dvcx-0.86.0/tests/unit/test_dataset_row.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-06-03 09:33:53.000000 dvcx-0.86.0/tests/unit/test_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-06-03 09:33:53.000000 dvcx-0.86.0/tests/unit/test_fileslice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5902 2024-06-03 09:33:53.000000 dvcx-0.86.0/tests/unit/test_id_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-06-03 09:33:53.000000 dvcx-0.86.0/tests/unit/test_listing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-06-03 09:33:53.000000 dvcx-0.86.0/tests/unit/test_metastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-06-03 09:33:53.000000 dvcx-0.86.0/tests/unit/test_query_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-06-03 09:33:53.000000 dvcx-0.86.0/tests/unit/test_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-06-03 09:33:53.000000 dvcx-0.86.0/tests/unit/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6790 2024-06-03 09:33:53.000000 dvcx-0.86.0/tests/unit/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-06-03 09:33:53.000000 dvcx-0.86.0/tests/unit/test_udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-06-03 09:33:53.000000 dvcx-0.86.0/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-06-03 09:33:53.000000 dvcx-0.86.0/tests/unit/test_warehouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7657 2024-06-03 09:33:53.000000 dvcx-0.86.0/tests/utils.py
```

### Comparing `dvcx-0.85.1/.cruft.json` & `dvcx-0.86.0/.cruft.json`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/.github/workflows/benchmarks.yml` & `dvcx-0.86.0/.github/workflows/benchmarks.yml`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/.github/workflows/release.yml` & `dvcx-0.86.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/.github/workflows/tests.yml` & `dvcx-0.86.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/.gitignore` & `dvcx-0.86.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/.pre-commit-config.yaml` & `dvcx-0.86.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/CODE_OF_CONDUCT.rst` & `dvcx-0.86.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/CONTRIBUTING.rst` & `dvcx-0.86.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/LICENSE` & `dvcx-0.86.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/LICENSES/Apache-2.0.txt` & `dvcx-0.86.0/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/LICENSES/BSD-3-Clause.txt` & `dvcx-0.86.0/LICENSES/BSD-3-Clause.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/LICENSES/Python-2.0.txt` & `dvcx-0.86.0/LICENSES/Python-2.0.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/PKG-INFO` & `dvcx-0.86.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvcx
-Version: 0.85.1
+Version: 0.86.0
 Summary: DVCx
 Author-email: Dmitry Petrov <support@dvc.org>
 License: Apache-2.0
 Project-URL: Issues, https://github.com/iterative/dvcx/issues
 Project-URL: Source, https://github.com/iterative/dvcx
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dvcx-0.85.1/README.rst` & `dvcx-0.86.0/README.rst`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/docs/cv_intro.md` & `dvcx-0.86.0/docs/cv_intro.md`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/docs/udfs.md` & `dvcx-0.86.0/docs/udfs.md`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/examples/blip2_image_desc_lib.py` & `dvcx-0.86.0/examples/blip2_image_desc_lib.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/examples/clip.py` & `dvcx-0.86.0/examples/clip.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/examples/common_sql_functions.py` & `dvcx-0.86.0/examples/common_sql_functions.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/examples/dir_expansion.py` & `dvcx-0.86.0/examples/dir_expansion.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/examples/hf_pipeline.py` & `dvcx-0.86.0/examples/hf_pipeline.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/examples/llava2_image_desc_lib.py` & `dvcx-0.86.0/examples/llava2_image_desc_lib.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/examples/llm-claude-aggregate-query.py` & `dvcx-0.86.0/examples/llm-claude-aggregate-query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/examples/llm-claude-simple-query.py` & `dvcx-0.86.0/examples/llm-claude-simple-query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/examples/llm-claude.py` & `dvcx-0.86.0/examples/llm-claude.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/examples/loader.py` & `dvcx-0.86.0/examples/loader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/examples/neurips/README` & `dvcx-0.86.0/examples/neurips/README`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/examples/neurips/distance_to_query.py` & `dvcx-0.86.0/examples/neurips/distance_to_query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/examples/neurips/llm_chat.py` & `dvcx-0.86.0/examples/neurips/llm_chat.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/examples/neurips/single_query.py` & `dvcx-0.86.0/examples/neurips/single_query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/examples/neurips/text_loaders.py` & `dvcx-0.86.0/examples/neurips/text_loaders.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/examples/openai_image_desc_lib.py` & `dvcx-0.86.0/examples/openai_image_desc_lib.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/examples/openimage-detect.py` & `dvcx-0.86.0/examples/openimage-detect.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/examples/pose_detection.py` & `dvcx-0.86.0/examples/pose_detection.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/examples/torch-loader.py` & `dvcx-0.86.0/examples/torch-loader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/examples/udfs/batching.py` & `dvcx-0.86.0/examples/udfs/batching.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/examples/udfs/image_transformation.py` & `dvcx-0.86.0/examples/udfs/image_transformation.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/examples/udfs/parallel.py` & `dvcx-0.86.0/examples/udfs/parallel.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/examples/udfs/simple.py` & `dvcx-0.86.0/examples/udfs/simple.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/examples/udfs/stateful.py` & `dvcx-0.86.0/examples/udfs/stateful.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/examples/udfs/stateful_similarity.py` & `dvcx-0.86.0/examples/udfs/stateful_similarity.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/examples/unstructured-text.py` & `dvcx-0.86.0/examples/unstructured-text.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/examples/wds.py` & `dvcx-0.86.0/examples/wds.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/examples/wds_filtered.py` & `dvcx-0.86.0/examples/wds_filtered.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/examples/wds_meta.py` & `dvcx-0.86.0/examples/wds_meta.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/examples/zalando/zalando_clip.py` & `dvcx-0.86.0/examples/zalando/zalando_clip.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/examples/zalando/zalando_dir_as_class.py` & `dvcx-0.86.0/examples/zalando/zalando_dir_as_class.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/noxfile.py` & `dvcx-0.86.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/pyproject.toml` & `dvcx-0.86.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/src/dvcx/asyn.py` & `dvcx-0.86.0/src/dvcx/asyn.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/src/dvcx/cache.py` & `dvcx-0.86.0/src/dvcx/cache.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/src/dvcx/catalog/catalog.py` & `dvcx-0.86.0/src/dvcx/catalog/catalog.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,14 @@
 from attrs import asdict
 from sqlalchemy import Column
 from tqdm import tqdm
 
 from dvcx.cache import DVCXCache
 from dvcx.client import Client
 from dvcx.config import get_remote_config, read_config
-from dvcx.data_storage.schema import DATASET_CORE_COLUMN_NAMES
 from dvcx.dataset import (
     DATASET_PREFIX,
     QUERY_DATASET_PREFIX,
     DatasetDependency,
     DatasetRecord,
     DatasetRow,
     DatasetStats,
@@ -985,14 +984,15 @@
     def create_dataset(
         self,
         name: str,
         version: Optional[int] = None,
         query_script: str = "",
         create_rows: Optional[bool] = True,
         custom_columns: Sequence[Column] = (),
+        columns: Sequence[Column] = (),
         validate_version: Optional[bool] = True,
         listing: Optional[bool] = False,
     ) -> "DatasetRecord":
         """
         Creates new dataset of a specific version.
         If dataset is not yet created, it will create it with version 1
         If version is None, then next unused version is created.
@@ -1003,19 +1003,21 @@
                 "Cannot create dataset that starts with source prefix, e.g s3://"
             )
         default_version = 1
         try:
             dataset = self.get_dataset(name)
             default_version = dataset.next_version
         except DatasetNotFoundError:
+            if not columns:
+                columns = [
+                    *self.warehouse.schema.dataset_row_cls.dataset_default_columns(),
+                    *custom_columns,
+                ]
             schema = {
-                c.name: c.type.to_dict()
-                for c in self.warehouse.schema.dataset_row_cls.dataset_default_columns()
-                + list(custom_columns)
-                if isinstance(c.type, SQLType)
+                c.name: c.type.to_dict() for c in columns if isinstance(c.type, SQLType)
             }
             dataset = self.metastore.create_dataset(
                 name,
                 query_script=query_script,
                 schema=schema,
                 ignore_if_exists=True,
             )
@@ -1034,37 +1036,42 @@
 
         return self.create_new_dataset_version(
             dataset,
             version,
             query_script=query_script,
             create_rows_table=create_rows,
             custom_columns=custom_columns,
+            columns=columns,
         )
 
     def create_new_dataset_version(
         self,
         dataset: DatasetRecord,
         version: int,
         sources="",
         query_script="",
         error_message="",
         error_stack="",
         script_output="",
         create_rows_table=True,
         custom_columns: Sequence[Column] = (),
+        columns: Sequence[Column] = (),
     ) -> DatasetRecord:
         """
         Creates dataset version if it doesn't exist.
         If create_rows is False, dataset rows table will not be created
         """
+        if not columns:
+            columns = [
+                *self.warehouse.schema.dataset_row_cls.dataset_default_columns(),
+                *custom_columns,
+            ]
+
         schema = {
-            c.name: c.type.to_dict()
-            for c in self.warehouse.schema.dataset_row_cls.dataset_default_columns()
-            + list(custom_columns)
-            if isinstance(c.type, SQLType)
+            c.name: c.type.to_dict() for c in columns if isinstance(c.type, SQLType)
         }
 
         dataset = self.metastore.create_dataset_version(
             dataset,
             version,
             status=DatasetStatus.PENDING,
             sources=sources,
@@ -1074,17 +1081,15 @@
             script_output=script_output,
             schema=schema,
             ignore_if_exists=True,
         )
 
         if create_rows_table:
             table_name = self.warehouse.dataset_table_name(dataset.name, version)
-            self.warehouse.create_dataset_rows_table(
-                table_name, custom_columns=custom_columns
-            )
+            self.warehouse.create_dataset_rows_table(table_name, columns=columns)
 
             self.update_dataset_version_with_warehouse_info(dataset, version)
 
         return dataset
 
     def update_dataset_version_with_warehouse_info(
         self, dataset: DatasetRecord, version: int, rows_dropped=False, **kwargs
@@ -1522,23 +1527,20 @@
             dst_dr = self.warehouse.dataset_rows(dst)
 
             merge_result_columns = list(
                 {
                     c.name: c for c in list(src_dr.table.c) + list(dst_dr.table.c)
                 }.values()
             )
-            custom_columns = [
-                c
-                for c in merge_result_columns
-                if c.name not in DATASET_CORE_COLUMN_NAMES
-            ]
 
             dst_version = dst_version or dst.next_version
             dst = self.create_new_dataset_version(
-                dst, dst_version, custom_columns=custom_columns
+                dst,
+                dst_version,
+                columns=merge_result_columns,
             )
             self.warehouse.merge_dataset_rows(
                 src,
                 dst,
                 src_version,
                 dst_version,
             )
@@ -1670,30 +1672,30 @@
             desc=f"Saving dataset {dataset_uri} locally: ",
             unit=" rows",
             unit_scale=True,
             unit_divisor=1000,
             total=dataset_stats.num_objects,  # type: ignore [union-attr]
         )
 
-        schema = DatasetRecord.parse_schema(
-            remote_dataset_version.schema,
+        schema = DatasetRecord.parse_schema(remote_dataset_version.schema)
+
+        # override schema information for the default columns
+        default_columns = (
+            self.warehouse.schema.dataset_row_cls.dataset_default_columns()
         )
-        custom_columns = [
-            sa.Column(c_name, c_type)
-            for c_name, c_type in schema.items()
-            if c_name not in DATASET_CORE_COLUMN_NAMES
-        ]
+        columns = {name: sa.Column(name, typ) for name, typ in schema.items()}
+        columns.update({c.name: c for c in default_columns if c.name in schema})
 
         # creating new dataset (version) locally
         dataset = self.create_dataset(
             remote_dataset_name,
             version,
             query_script=remote_dataset_version.query_script,
             create_rows=True,
-            custom_columns=custom_columns,
+            columns=list(columns.values()),
             validate_version=False,
         )
 
         # asking remote to export dataset rows table to s3 and to return signed
         # urls of exported parts, which are in parquet format
         export_response = studio_client.export_dataset_table(
             remote_dataset_name, version
```

### Comparing `dvcx-0.85.1/src/dvcx/catalog/datasource.py` & `dvcx-0.86.0/src/dvcx/catalog/datasource.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/src/dvcx/catalog/loader.py` & `dvcx-0.86.0/src/dvcx/catalog/loader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/src/dvcx/cli.py` & `dvcx-0.86.0/src/dvcx/cli.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/src/dvcx/cli_utils.py` & `dvcx-0.86.0/src/dvcx/cli_utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/src/dvcx/client/azure.py` & `dvcx-0.86.0/src/dvcx/client/azure.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/src/dvcx/client/fileslice.py` & `dvcx-0.86.0/src/dvcx/client/fileslice.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/src/dvcx/client/fsspec.py` & `dvcx-0.86.0/src/dvcx/client/fsspec.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/src/dvcx/client/gcs.py` & `dvcx-0.86.0/src/dvcx/client/gcs.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/src/dvcx/client/local.py` & `dvcx-0.86.0/src/dvcx/client/local.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,17 +62,23 @@
         Resolving path, that can be absolute or relative, to file URI which
         starts with file:/// prefix
         In unix like systems we support home shortcut as well.
         Examples:
             ./animals -> file:///home/user/working_dir/animals
             ~/animals -> file:///home/user/animals
             /home/user/animals -> file:///home/user/animals
+            /home/user/animals/ -> file:///home/user/animals/
             C:\\windows\animals -> file:///C:/windows/animals
         """
-        return Path(path).expanduser().absolute().resolve().as_uri()
+        uri = Path(path).expanduser().absolute().resolve().as_uri()
+        if path[-1] == os.sep:
+            # we should keep os separator from the end of the path
+            uri += "/"  # in uri (file:///...) all separators are / regardless of os
+
+        return uri
 
     @classmethod
     def split_url(cls, url: str) -> tuple[str, str]:
         """
         Splits url into two components:
             1. root of the FS which will later on become the name of the storage
             2. path which will later on become partial path
```

### Comparing `dvcx-0.85.1/src/dvcx/client/s3.py` & `dvcx-0.86.0/src/dvcx/client/s3.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/src/dvcx/config.py` & `dvcx-0.86.0/src/dvcx/config.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/src/dvcx/data_storage/db_engine.py` & `dvcx-0.86.0/src/dvcx/data_storage/db_engine.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/src/dvcx/data_storage/id_generator.py` & `dvcx-0.86.0/src/dvcx/data_storage/id_generator.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/src/dvcx/data_storage/metastore.py` & `dvcx-0.86.0/src/dvcx/data_storage/metastore.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/src/dvcx/data_storage/schema.py` & `dvcx-0.86.0/src/dvcx/data_storage/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -266,28 +266,25 @@
             unique=column.unique,
         )
 
     @classmethod
     def new_table(
         cls,
         name: str,
-        custom_columns: Sequence["sa.Column"] = (),
+        columns: Sequence["sa.Column"] = (),
         metadata: Optional["sa.MetaData"] = None,
     ):
         # copy columns, since re-using the same objects from another table
         # may raise an error
-        custom_columns = [cls.copy_signal_column(c) for c in custom_columns]
+        columns = [cls.copy_signal_column(c) for c in columns if c.name != "id"]
+        columns = [sa.Column("id", Int, primary_key=True), *columns]
+
         if metadata is None:
             metadata = sa.MetaData()
-        return sa.Table(
-            name,
-            metadata,
-            *cls.dataset_default_columns(),
-            *custom_columns,
-        )
+        return sa.Table(name, metadata, *columns)
 
     def get_table(self) -> "sa.Table":
         table = self.metadata.tables.get(self.name)
         if table is None:
             table = sa.Table(
                 self.name,
                 self.metadata,
```

### Comparing `dvcx-0.85.1/src/dvcx/data_storage/serializer.py` & `dvcx-0.86.0/src/dvcx/data_storage/serializer.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/src/dvcx/data_storage/sqlite.py` & `dvcx-0.86.0/src/dvcx/data_storage/sqlite.py`

 * *Files 0% similar despite different names*

```diff
@@ -561,19 +561,21 @@
 
     def is_ready(self, timeout: Optional[int] = None) -> bool:
         return True
 
     def create_dataset_rows_table(
         self,
         name: str,
-        custom_columns: Sequence["sqlalchemy.Column"] = (),
+        columns: Sequence["sqlalchemy.Column"] = (),
         if_not_exists: bool = True,
     ) -> Table:
         table = self.schema.dataset_row_cls.new_table(
-            name, custom_columns=custom_columns, metadata=self.db.metadata
+            name,
+            columns=columns,
+            metadata=self.db.metadata,
         )
         self.db.create_table(table, if_not_exists=if_not_exists)
         return table
 
     def dataset_rows_select(
         self, select_query: sqlalchemy.sql.selectable.Select, **kwargs
     ):
@@ -605,26 +607,17 @@
             # source table doesn't exist, nothing to do
             return
 
         src_dr = self.dataset_rows(src, src_version).table
 
         if not self.db.has_table(self.dataset_table_name(dst.name, dst_version)):
             # destination table doesn't exist, create it
-            custom_columns = [
-                c
-                for c in src_dr.c
-                if c.name
-                not in [
-                    c.name
-                    for c in self.schema.dataset_row_cls.dataset_default_columns()
-                ]
-            ]
             self.create_dataset_rows_table(
                 self.dataset_table_name(dst.name, dst_version),
-                custom_columns=custom_columns,
+                columns=src_dr.c,
             )
             dst_empty = True
 
         dst_dr = self.dataset_rows(dst, dst_version).table
         merge_fields = [c.name for c in src_dr.c if c.name != "id"]
         select_src = select(*(getattr(src_dr.c, f) for f in merge_fields))
```

### Comparing `dvcx-0.85.1/src/dvcx/data_storage/warehouse.py` & `dvcx-0.86.0/src/dvcx/data_storage/warehouse.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from dvcx.dataset import DatasetRecord, DatasetRow
 from dvcx.node import DirTypeGroup, Entry, Node, NodeWithPath, get_path
 from dvcx.sql.types import Int, SQLType
 from dvcx.storage import StorageURI
 from dvcx.utils import GLOB_CHARS, sql_escape_like
 
 if TYPE_CHECKING:
+    from sqlalchemy.sql._typing import _ColumnsClauseArgument
     from sqlalchemy.sql.elements import ColumnElement
     from sqlalchemy.types import TypeEngine
 
     from dvcx.data_storage import AbstractIDGenerator, schema
     from dvcx.data_storage.db_engine import DatabaseEngine
 
 try:
@@ -236,15 +237,15 @@
     # Datasets
     #
 
     @abstractmethod
     def create_dataset_rows_table(
         self,
         name: str,
-        custom_columns: Sequence["sa.Column"] = (),
+        columns: Sequence["sa.Column"] = (),
         if_not_exists: bool = True,
     ) -> Table:
         """Creates a dataset rows table for the given dataset name and columns"""
 
     def drop_dataset_rows_table(
         self,
         dataset: DatasetRecord,
@@ -301,14 +302,18 @@
         columns = list(DATASET_CORE_COLUMN_NAMES) if not custom_columns else None
         dr = self.dataset_rows(dataset, version)
 
         if not columns:
             # fetching all columns if specific columns are not defined
             columns = [c.name for c in dr.c]
 
+        if set(DATASET_CORE_COLUMN_NAMES) - set(columns):
+            # TODO: silencing preview for save, remove later
+            return
+
         select_columns = [dr.c[c] for c in columns]
         column_index_mapping = {c: i for i, c in enumerate(columns)}
 
         query = dr.select(*select_columns)
         if source:
             query = query.where(dr.c.source == source)
         if offset:
@@ -395,17 +400,20 @@
         Returns tuple with dataset stats: total number of rows and total dataset size.
         """
         if not (self.db.has_table(self.dataset_table_name(dataset.name, version))):
             return None, None
 
         dr = self.dataset_rows(dataset, version)
         table = dr.get_table()
-        query = select(sa.func.count(table.c.id), sa.func.sum(table.c.size))
-        (res,) = self.db.execute(query)
-        return res[0], res[1]
+        expressions: tuple[_ColumnsClauseArgument[Any], ...] = (sa.func.count(),)
+        if "size" in table.columns:
+            expressions = (*expressions, sa.func.sum(table.c.size))
+        query = select(*expressions)
+        ((nrows, *rest),) = self.db.execute(query)
+        return nrows, rest[0] if rest else None
 
     def prepare_entries(
         self, uri: str, entries: Iterable[Entry]
     ) -> list[dict[str, Any]]:
         """
         Prepares bucket listing entry (row) for inserting into database
         """
```

### Comparing `dvcx-0.85.1/src/dvcx/dataset.py` & `dvcx-0.86.0/src/dvcx/dataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/src/dvcx/error.py` & `dvcx-0.86.0/src/dvcx/error.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/src/dvcx/lib/cached_stream.py` & `dvcx-0.86.0/src/dvcx/lib/cached_stream.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/src/dvcx/lib/claude.py` & `dvcx-0.86.0/src/dvcx/lib/claude.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/src/dvcx/lib/dataset.py` & `dvcx-0.86.0/src/dvcx/lib/dataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/src/dvcx/lib/feature.py` & `dvcx-0.86.0/src/dvcx/lib/feature.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/src/dvcx/lib/feature_types.py` & `dvcx-0.86.0/src/dvcx/lib/feature_types.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/src/dvcx/lib/feature_udf.py` & `dvcx-0.86.0/src/dvcx/lib/feature_udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/src/dvcx/lib/file.py` & `dvcx-0.86.0/src/dvcx/lib/file.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/src/dvcx/lib/gpt4_vision.py` & `dvcx-0.86.0/src/dvcx/lib/gpt4_vision.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/src/dvcx/lib/hf_image_to_text.py` & `dvcx-0.86.0/src/dvcx/lib/hf_image_to_text.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/src/dvcx/lib/hf_pipeline.py` & `dvcx-0.86.0/src/dvcx/lib/hf_pipeline.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/src/dvcx/lib/image.py` & `dvcx-0.86.0/src/dvcx/lib/image.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/src/dvcx/lib/image_transform.py` & `dvcx-0.86.0/src/dvcx/lib/image_transform.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/src/dvcx/lib/iptc_exif_xmp.py` & `dvcx-0.86.0/src/dvcx/lib/iptc_exif_xmp.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/src/dvcx/lib/pytorch.py` & `dvcx-0.86.0/src/dvcx/lib/pytorch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/src/dvcx/lib/reader.py` & `dvcx-0.86.0/src/dvcx/lib/reader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/src/dvcx/lib/text.py` & `dvcx-0.86.0/src/dvcx/lib/text.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/src/dvcx/lib/udf.py` & `dvcx-0.86.0/src/dvcx/lib/udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/src/dvcx/lib/unstructured.py` & `dvcx-0.86.0/src/dvcx/lib/unstructured.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/src/dvcx/lib/utils.py` & `dvcx-0.86.0/src/dvcx/lib/utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/src/dvcx/lib/webdataset.py` & `dvcx-0.86.0/src/dvcx/lib/webdataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/src/dvcx/lib/webdataset_laion.py` & `dvcx-0.86.0/src/dvcx/lib/webdataset_laion.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/src/dvcx/lib/webdataset_meta.py` & `dvcx-0.86.0/src/dvcx/lib/webdataset_meta.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/src/dvcx/listing.py` & `dvcx-0.86.0/src/dvcx/listing.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/src/dvcx/node.py` & `dvcx-0.86.0/src/dvcx/node.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/src/dvcx/nodes_fetcher.py` & `dvcx-0.86.0/src/dvcx/nodes_fetcher.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/src/dvcx/nodes_thread_pool.py` & `dvcx-0.86.0/src/dvcx/nodes_thread_pool.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/src/dvcx/progress.py` & `dvcx-0.86.0/src/dvcx/progress.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/src/dvcx/query/batch.py` & `dvcx-0.86.0/src/dvcx/query/batch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/src/dvcx/query/builtins.py` & `dvcx-0.86.0/src/dvcx/query/builtins.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/src/dvcx/query/dataset.py` & `dvcx-0.86.0/src/dvcx/query/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 )
 
 import attrs
 import sqlalchemy
 from attrs import frozen
 from dill import dumps
 from fsspec.callbacks import DEFAULT_CALLBACK, Callback, TqdmCallback
+from sqlalchemy import Column
 from sqlalchemy.sql import func as f
 from sqlalchemy.sql.elements import ColumnClause, ColumnElement
 from sqlalchemy.sql.expression import label
 from sqlalchemy.sql.schema import TableClause
 from sqlalchemy.sql.selectable import Select
 
 from dvcx.asyn import ASYNC_WORKERS, AsyncMapper, OrderedMapper
@@ -259,22 +260,22 @@
         temp_tables.extend(self.dq.temp_table_names)
 
         # creating temp table that will hold subtract results
         temp_table_name = self.catalog.warehouse.TMP_TABLE_NAME_PREFIX + _random_string(
             6
         )
         temp_tables.append(temp_table_name)
-        custom_columns: list[sqlalchemy.Column] = [
-            sqlalchemy.Column(col.name, col.type)
-            for col in source_query.columns
-            if col.name not in DATASET_CORE_COLUMN_NAMES
+
+        columns = [
+            c if isinstance(c, Column) else Column(c.name, c.type)
+            for c in source_query.columns
         ]
         temp_table = self.catalog.warehouse.create_dataset_rows_table(
             temp_table_name,
-            custom_columns=custom_columns,
+            columns=columns,
             if_not_exists=False,
         )
 
         diff_q = self.query(source_query, target_query)
 
         insert_q = temp_table.insert().from_select(
             source_query.selected_columns, diff_q
@@ -431,15 +432,15 @@
     parallel: Optional[int] = None
     workers: Union[bool, int] = False
     min_task_size: Optional[int] = None
     is_generator = False
     cache: bool = False
 
     @abstractmethod
-    def create_udf_table(self) -> "Table":
+    def create_udf_table(self, query: Select) -> "Table":
         """Method that creates a table where temp udf results will be saved"""
 
     def process_input_query(self, query: Select) -> tuple[Select, list["Table"]]:
         """Apply any necessary processing to the input query"""
         return query, []
 
     @abstractmethod
@@ -612,15 +613,15 @@
                 min_task_size=self.min_task_size,
             )
         return self.__class__(self.udf, self.catalog)
 
     def apply(
         self, query_generator: QueryGenerator, temp_tables: list[str]
     ) -> "StepResult":
-        query = query_generator.select()
+        _query = query = query_generator.select()
 
         # Apply partitioning if needed.
         if self.partition_by is not None:
             partition_tbl = self.create_partitions_table(query)
             temp_tables.append(partition_tbl.name)
 
             subq = query.subquery()
@@ -629,27 +630,27 @@
                 .outerjoin(partition_tbl, partition_tbl.c.id == subq.c.id)
                 .add_columns(*partition_columns())
             )
 
         query, tables = self.process_input_query(query)
         for t in tables:
             temp_tables.append(t.name)
-        udf_table = self.create_udf_table()
+        udf_table = self.create_udf_table(_query)
         temp_tables.append(udf_table.name)
         self.populate_udf_table(udf_table, query)
         q, cols = self.create_result_query(udf_table, query)
 
         return step_result(q, cols)
 
 
 @frozen
 class UDFSignal(UDF):
     is_generator = False
 
-    def create_udf_table(self) -> "Table":
+    def create_udf_table(self, query: Select) -> "Table":
         udf_output_columns: list[sqlalchemy.Column[Any]] = [
             sqlalchemy.Column(col_name, col_type)
             for (col_name, col_type) in self.udf.output.items()
         ]
 
         return self.catalog.warehouse.create_udf_table(
             self.udf_table_name(), udf_output_columns
@@ -738,25 +739,32 @@
 
 @frozen
 class RowGenerator(UDF):
     """Extend dataset with new rows."""
 
     is_generator = True
 
-    def create_udf_table(self) -> "Table":
-        table_name = self.udf_table_name()
-        custom_udf_output_columns: list[sqlalchemy.Column] = [
-            sqlalchemy.Column(col_name, col_type)
-            for (col_name, col_type) in self.udf.output.items()
-            if col_name not in DATASET_CORE_COLUMN_NAMES
-        ]
+    def create_udf_table(self, query: Select) -> "Table":
+        warehouse = self.catalog.warehouse
 
-        return self.catalog.warehouse.create_dataset_rows_table(
+        table_name = self.udf_table_name()
+        columns = {
+            c.name: c if isinstance(c, Column) else Column(c.name, c.type)
+            for c in query.columns
+        }
+        columns.update(
+            {
+                name: Column(name, typ)
+                for name, typ in self.udf.output.items()
+                if name not in columns
+            }
+        )
+        return warehouse.create_dataset_rows_table(
             table_name,
-            custom_columns=custom_udf_output_columns,
+            columns=list(columns.values()),
             if_not_exists=False,
         )
 
     def create_result_query(
         self, udf_table, query: Select
     ) -> tuple[QueryGeneratorFunc, list["sqlalchemy.Column"]]:
         if not query._order_by_clauses:
@@ -1641,35 +1649,22 @@
 
         if not name:
             name = self.session.generate_temp_dataset_name()
 
         try:
             query = self.apply_steps()
 
-            missing_default_columns = [
-                c_name
-                for c_name in DATASET_CORE_COLUMN_NAMES
-                if c_name not in [c.name for c in query.columns]
+            columns = [
+                c if isinstance(c, Column) else Column(c.name, c.type)
+                for c in query.columns
             ]
-            if missing_default_columns:
-                raise RuntimeError(
-                    'Missing default columns from final query: '
-                    f'{", ".join(missing_default_columns)}'
-                )
-
-            custom_columns: list[sqlalchemy.Column] = [
-                sqlalchemy.Column(col.name, col.type)
-                for col in query.columns
-                if col.name not in DATASET_CORE_COLUMN_NAMES
-            ]
-
             dataset = self.catalog.create_dataset(
                 name,
                 version=version,
-                custom_columns=custom_columns,
+                columns=columns,
                 **kwargs,
             )
             version = version or dataset.latest_version
 
             dr = self.catalog.warehouse.dataset_rows(dataset)
 
             # Exclude the id column and let the db create it to avoid unique
```

### Comparing `dvcx-0.85.1/src/dvcx/query/dispatch.py` & `dvcx-0.86.0/src/dvcx/query/dispatch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/src/dvcx/query/params.py` & `dvcx-0.86.0/src/dvcx/query/params.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/src/dvcx/query/schema.py` & `dvcx-0.86.0/src/dvcx/query/schema.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/src/dvcx/query/session.py` & `dvcx-0.86.0/src/dvcx/query/session.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/src/dvcx/query/udf.py` & `dvcx-0.86.0/src/dvcx/query/udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/src/dvcx/remote/studio.py` & `dvcx-0.86.0/src/dvcx/remote/studio.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/src/dvcx/sql/default/base.py` & `dvcx-0.86.0/src/dvcx/sql/default/base.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/src/dvcx/sql/functions/array.py` & `dvcx-0.86.0/src/dvcx/sql/functions/array.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/src/dvcx/sql/functions/path.py` & `dvcx-0.86.0/src/dvcx/sql/functions/path.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/src/dvcx/sql/selectable.py` & `dvcx-0.86.0/src/dvcx/sql/selectable.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/src/dvcx/sql/sqlite/base.py` & `dvcx-0.86.0/src/dvcx/sql/sqlite/base.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/src/dvcx/sql/sqlite/types.py` & `dvcx-0.86.0/src/dvcx/sql/sqlite/types.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/src/dvcx/sql/types.py` & `dvcx-0.86.0/src/dvcx/sql/types.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/src/dvcx/sql/utils.py` & `dvcx-0.86.0/src/dvcx/sql/utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/src/dvcx/storage.py` & `dvcx-0.86.0/src/dvcx/storage.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/src/dvcx/utils.py` & `dvcx-0.86.0/src/dvcx/utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/src/dvcx.egg-info/PKG-INFO` & `dvcx-0.86.0/src/dvcx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvcx
-Version: 0.85.1
+Version: 0.86.0
 Summary: DVCx
 Author-email: Dmitry Petrov <support@dvc.org>
 License: Apache-2.0
 Project-URL: Issues, https://github.com/iterative/dvcx/issues
 Project-URL: Source, https://github.com/iterative/dvcx
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dvcx-0.85.1/src/dvcx.egg-info/SOURCES.txt` & `dvcx-0.86.0/src/dvcx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/src/dvcx.egg-info/requires.txt` & `dvcx-0.86.0/src/dvcx.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/tests/benchmarks/conftest.py` & `dvcx-0.86.0/tests/benchmarks/conftest.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/tests/conftest.py` & `dvcx-0.86.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/tests/data.py` & `dvcx-0.86.0/tests/data.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/tests/func/test_catalog.py` & `dvcx-0.86.0/tests/func/test_catalog.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/tests/func/test_client.py` & `dvcx-0.86.0/tests/func/test_client.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/tests/func/test_dataset_query.py` & `dvcx-0.86.0/tests/func/test_dataset_query.py`

 * *Files 0% similar despite different names*

```diff
@@ -3616,18 +3616,14 @@
 
 
 @pytest.mark.parametrize(
     "cloud_type,version_aware",
     [("s3", True)],
     indirect=True,
 )
-def test_missing_default_columns(cloud_test_catalog):
+def test_with_missing_default_columns(cloud_test_catalog):
     catalog = cloud_test_catalog.catalog
     path = f"{cloud_test_catalog.src_uri}/cats"
-    with pytest.raises(RuntimeError) as exc_info:
-        DatasetQuery(path=path, catalog=catalog).select(C.name).save("cats", version=1)
+    DatasetQuery(path=path, catalog=catalog).select(C.name).save("cats", version=1)
 
-    assert str(exc_info.value) == (
-        "Missing default columns from final query: id, vtype, dir_type, "
-        "parent, etag, version, is_latest, last_modified, size, "
-        "owner_name, owner_id, random, location, source"
-    )
+    dataset = catalog.get_dataset("cats")
+    assert dataset.schema == {"name": String}
```

### Comparing `dvcx-0.85.1/tests/func/test_datasets.py` & `dvcx-0.86.0/tests/func/test_datasets.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/tests/func/test_ls.py` & `dvcx-0.86.0/tests/func/test_ls.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/tests/func/test_pull.py` & `dvcx-0.86.0/tests/func/test_pull.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/tests/func/test_pytorch.py` & `dvcx-0.86.0/tests/func/test_pytorch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/tests/func/test_query.py` & `dvcx-0.86.0/tests/func/test_query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/tests/scripts/name_len_normal.py` & `dvcx-0.86.0/tests/scripts/name_len_normal.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/tests/scripts/name_len_slow.py` & `dvcx-0.86.0/tests/scripts/name_len_slow.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/tests/test_cli_e2e.py` & `dvcx-0.86.0/tests/test_cli_e2e.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/tests/test_query_e2e.py` & `dvcx-0.86.0/tests/test_query_e2e.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/tests/unit/lib/test_cached_stream.py` & `dvcx-0.86.0/tests/unit/lib/test_cached_stream.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/tests/unit/lib/test_feature.py` & `dvcx-0.86.0/tests/unit/lib/test_feature.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/tests/unit/lib/test_feature_udf.py` & `dvcx-0.86.0/tests/unit/lib/test_feature_udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/tests/unit/lib/test_file.py` & `dvcx-0.86.0/tests/unit/lib/test_file.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/tests/unit/lib/test_image.py` & `dvcx-0.86.0/tests/unit/lib/test_image.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/tests/unit/lib/test_reader.py` & `dvcx-0.86.0/tests/unit/lib/test_reader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/tests/unit/lib/test_text.py` & `dvcx-0.86.0/tests/unit/lib/test_text.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/tests/unit/lib/test_webdataset.py` & `dvcx-0.86.0/tests/unit/lib/test_webdataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/tests/unit/lib/test_webdataset_meta.py` & `dvcx-0.86.0/tests/unit/lib/test_webdataset_meta.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/tests/unit/sql/test_array.py` & `dvcx-0.86.0/tests/unit/sql/test_array.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/tests/unit/sql/test_conditional.py` & `dvcx-0.86.0/tests/unit/sql/test_conditional.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/tests/unit/sql/test_path.py` & `dvcx-0.86.0/tests/unit/sql/test_path.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/tests/unit/sql/test_selectable.py` & `dvcx-0.86.0/tests/unit/sql/test_selectable.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/tests/unit/sql/test_string.py` & `dvcx-0.86.0/tests/unit/sql/test_string.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/tests/unit/test_asyn.py` & `dvcx-0.86.0/tests/unit/test_asyn.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/tests/unit/test_cache.py` & `dvcx-0.86.0/tests/unit/test_cache.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/tests/unit/test_catalog.py` & `dvcx-0.86.0/tests/unit/test_catalog.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/tests/unit/test_catalog_loader.py` & `dvcx-0.86.0/tests/unit/test_catalog_loader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/tests/unit/test_cli_parsing.py` & `dvcx-0.86.0/tests/unit/test_cli_parsing.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/tests/unit/test_client.py` & `dvcx-0.86.0/tests/unit/test_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+import os
 import sys
 from pathlib import Path
 
 import pytest
 from hypothesis import HealthCheck, assume, given, settings
 from hypothesis import strategies as st
 
+from dvcx.client import Client
 from dvcx.client.local import FileClient
 from tests.utils import uppercase_scheme
 
 non_null_text = st.text(
     alphabet=st.characters(blacklist_categories=["Cc", "Cs"]), min_size=1
 )
 
@@ -61,25 +63,25 @@
     assert client.uri == root_uri
     assert rel_part == (working_dir / Path("animals")).as_uri()[len(root_uri) :]
 
 
 @pytest.mark.parametrize("cloud_type", ["file"], indirect=True)
 def test_parse_file_relative_path_multiple_dirs_back(cloud_test_catalog):
     catalog = cloud_test_catalog.catalog
-    client, rel_part = catalog.parse_url("../../animals")
+    client, rel_part = catalog.parse_url("../../animals".replace("/", os.sep))
     root_uri = FileClient.root_path().as_uri()
     assert client.uri == root_uri
     assert (
         rel_part
         == (Path().absolute().parents[1] / Path("animals")).as_uri()[len(root_uri) :]
     )
 
 
 @pytest.mark.parametrize("cloud_type", ["file"], indirect=True)
-@pytest.mark.parametrize("url", ["./animals", "animals"])
+@pytest.mark.parametrize("url", ["./animals".replace("/", os.sep), "animals"])
 def test_parse_file_relative_path_working_dir(cloud_test_catalog, url):
     catalog = cloud_test_catalog.catalog
     client, rel_part = catalog.parse_url(url)
     root_uri = FileClient.root_path().as_uri()
     assert client.uri == root_uri
     assert rel_part == (Path().absolute() / Path("animals")).as_uri()[len(root_uri) :]
 
@@ -90,7 +92,27 @@
         # home dir shortcut is not available on windows
         pytest.skip()
     catalog = cloud_test_catalog.catalog
     client, rel_part = catalog.parse_url("~/animals")
     root_uri = FileClient.root_path().as_uri()
     assert client.uri == root_uri
     assert rel_part == (Path().home() / Path("animals")).as_uri()[len(root_uri) :]
+
+
+@pytest.mark.parametrize("cloud_type", ["file"], indirect=True)
+def test_parse_file_path_ends_with_slash(cloud_type):
+    client, rel_part = Client.parse_url("./animals/".replace("/", os.sep), None, None)
+    root_uri = FileClient.root_path().as_uri()
+    assert client.uri == root_uri
+    assert (
+        rel_part
+        == ((Path().absolute() / Path("animals")).as_uri())[len(root_uri) :] + "/"
+    )
+
+
+@pytest.mark.parametrize("cloud_type", ["s3", "azure", "gcs"], indirect=True)
+def test_parse_cloud_path_ends_with_slash(cloud_test_catalog):
+    uri = f"{cloud_test_catalog.src_uri}/animals/"
+    catalog = cloud_test_catalog.catalog
+    client, rel_part = catalog.parse_url(uri)
+    assert client.uri == cloud_test_catalog.src_uri
+    assert rel_part == "animals/"
```

### Comparing `dvcx-0.85.1/tests/unit/test_client_s3.py` & `dvcx-0.86.0/tests/unit/test_client_s3.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/tests/unit/test_data_storage.py` & `dvcx-0.86.0/tests/unit/test_data_storage.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/tests/unit/test_database_engine.py` & `dvcx-0.86.0/tests/unit/test_database_engine.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/tests/unit/test_dataset.py` & `dvcx-0.86.0/tests/unit/test_dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 from dvcx.data_storage.schema import DatasetRow
 from dvcx.sql.types import JSON, Array, Binary, Float, Float32, Float64, Int
 
 
 def test_dataset_table_compilation():
     table = DatasetRow.new_table(
         "ds-1",
-        custom_columns=[
+        columns=[
+            *DatasetRow.dataset_default_columns(),
             Column("score", Float, nullable=False),
             Column("meta_info", JSON),
         ],
     )
     result = CreateTable(table, if_not_exists=True).compile(dialect=sqlite_dialect())
 
     assert result.string == (
```

### Comparing `dvcx-0.85.1/tests/unit/test_dataset_row.py` & `dvcx-0.86.0/tests/unit/test_dataset_row.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/tests/unit/test_dispatch.py` & `dvcx-0.86.0/tests/unit/test_dispatch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/tests/unit/test_fileslice.py` & `dvcx-0.86.0/tests/unit/test_fileslice.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/tests/unit/test_id_generator.py` & `dvcx-0.86.0/tests/unit/test_id_generator.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/tests/unit/test_listing.py` & `dvcx-0.86.0/tests/unit/test_listing.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/tests/unit/test_metastore.py` & `dvcx-0.86.0/tests/unit/test_metastore.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/tests/unit/test_query_params.py` & `dvcx-0.86.0/tests/unit/test_query_params.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/tests/unit/test_serializer.py` & `dvcx-0.86.0/tests/unit/test_serializer.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/tests/unit/test_session.py` & `dvcx-0.86.0/tests/unit/test_session.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/tests/unit/test_storage.py` & `dvcx-0.86.0/tests/unit/test_storage.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/tests/unit/test_udf.py` & `dvcx-0.86.0/tests/unit/test_udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/tests/unit/test_utils.py` & `dvcx-0.86.0/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/tests/unit/test_warehouse.py` & `dvcx-0.86.0/tests/unit/test_warehouse.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.1/tests/utils.py` & `dvcx-0.86.0/tests/utils.py`

 * *Files identical despite different names*

