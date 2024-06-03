# Comparing `tmp/vectice-24.2.7.0.tar.gz` & `tmp/vectice-24.2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vectice-24.2.7.0.tar", last modified: Mon May 27 12:27:12 2024, max compression
+gzip compressed data, was "vectice-24.2.8.0.tar", last modified: Mon Jun  3 07:55:51 2024, max compression
```

## Comparing `vectice-24.2.7.0.tar` & `vectice-24.2.8.0.tar`

### file list

```diff
@@ -1,169 +1,171 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:27:12.893410 vectice-24.2.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-27 12:27:07.000000 vectice-24.2.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-05-27 12:27:12.893410 vectice-24.2.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-27 12:27:07.000000 vectice-24.2.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-27 12:27:07.000000 vectice-24.2.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-27 12:27:12.893410 vectice-24.2.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-05-27 12:27:07.000000 vectice-24.2.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:27:12.853410 vectice-24.2.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:27:12.857410 vectice-24.2.7.0/src/vectice/
--rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:27:12.861410 vectice-24.2.7.0/src/vectice/api/
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8075 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)    23447 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/gql_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/gql_attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)     6506 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/gql_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/gql_entity_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/gql_feature_flag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/gql_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     7279 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/gql_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/gql_organization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/gql_property.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/gql_user_workspace_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/http_error.py
--rw-r--r--   0 runner    (1001) docker     (127)    13467 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/http_error_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)    12109 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/iteration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:27:12.869410 vectice-24.2.7.0/src/vectice/api/json/
--rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json/artifact_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json/attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json/code.py
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json/code_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json/dataset_register.py
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json/dataset_representation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json/dataset_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json/dataset_version_representation.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json/entity_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json/files_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json/iteration.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json/json_to_class.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json/json_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json/last_assets.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json/model_register.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json/model_representation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json/model_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json/model_version_representation.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json/organization_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json/page.py
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json/paged_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json/phase.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json/property.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json/public_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json/requirement.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json/section.py
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json/user_and_workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json/workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     4894 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/phase.py
--rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     8364 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/rest_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:27:12.869410 vectice-24.2.7.0/src/vectice/autolog/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/autolog/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:27:12.873410 vectice-24.2.7.0/src/vectice/autolog/asset_services/
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/autolog/asset_services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/autolog/asset_services/catboost_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/autolog/asset_services/keras_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/autolog/asset_services/lightgbm_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/autolog/asset_services/metric_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/autolog/asset_services/pandas_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/autolog/asset_services/pyspark_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/autolog/asset_services/pytorch_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/autolog/asset_services/sklearn_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/autolog/asset_services/statsmodel_wrapper_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/autolog/asset_services/vectice_asset_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     9912 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/autolog/autolog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/autolog/autolog_asset_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    33379 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/autolog/autolog_class.py
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/autolog/model_library.py
--rw-r--r--   0 runner    (1001) docker     (127)    22308 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:27:12.873410 vectice-24.2.7.0/src/vectice/models/
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/additional_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/attachment_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/code_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    11659 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    19022 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/iteration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    11174 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/model_exp_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/model_mlflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     6486 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/phase.py
--rw-r--r--   0 runner    (1001) docker     (127)     6055 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/project.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/property.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:27:12.877410 vectice-24.2.7.0/src/vectice/models/representation/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/representation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/representation/dataset_representation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7126 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/representation/dataset_version_representation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/representation/model_representation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7494 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/representation/model_version_representation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:27:12.877410 vectice-24.2.7.0/src/vectice/models/resource/
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4951 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/resource/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8522 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/resource/bigquery_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    11795 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/resource/databricks_table_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/resource/description.py
--rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/resource/file_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     7293 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/resource/gcs_resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:27:12.881410 vectice-24.2.7.0/src/vectice/models/resource/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/resource/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/resource/metadata/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/resource/metadata/column_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/resource/metadata/dataframe_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/resource/metadata/db_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/resource/metadata/df_wrapper_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/resource/metadata/df_wrapper_pandas_default.py
--rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/resource/metadata/df_wrapper_pyspark_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/resource/metadata/df_wrapper_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    11952 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/resource/metadata/df_wrapper_spark_df.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/resource/metadata/extra_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/resource/metadata/files_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/resource/metadata/pyspark_pandas_dataframe_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/resource/metadata/pyspark_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/resource/metadata/source.py
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/resource/no_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     8986 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/resource/s3_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     7915 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/resource/snowflake_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/table.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:27:12.881410 vectice-24.2.7.0/src/vectice/models/test_library/
--rw-r--r--   0 runner    (1001) docker     (127)    11948 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/test_library/binary_classification_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:27:12.881410 vectice-24.2.7.0/src/vectice/services/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7367 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/services/iteration_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     7354 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/services/phase_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:27:12.881410 vectice-24.2.7.0/src/vectice/types/
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/types/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:27:12.885410 vectice-24.2.7.0/src/vectice/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/utils/api_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11664 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/utils/code_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    15222 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/utils/common_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/utils/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/utils/dataframe_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9540 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/utils/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/utils/instance_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/utils/last_assets.py
--rw-r--r--   0 runner    (1001) docker     (127)     5342 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/utils/logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/utils/vectice_ids_regex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:27:12.885410 vectice-24.2.7.0/src/vectice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-05-27 12:27:12.000000 vectice-24.2.7.0/src/vectice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5878 2024-05-27 12:27:12.000000 vectice-24.2.7.0/src/vectice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 12:27:12.000000 vectice-24.2.7.0/src/vectice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-27 12:27:12.000000 vectice-24.2.7.0/src/vectice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-27 12:27:12.000000 vectice-24.2.7.0/src/vectice.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:55:51.953487 vectice-24.2.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-06-03 07:55:41.000000 vectice-24.2.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-06-03 07:55:51.953487 vectice-24.2.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-06-03 07:55:41.000000 vectice-24.2.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-06-03 07:55:41.000000 vectice-24.2.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-06-03 07:55:51.953487 vectice-24.2.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-06-03 07:55:41.000000 vectice-24.2.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:55:51.917487 vectice-24.2.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:55:51.921487 vectice-24.2.8.0/src/vectice/
+-rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:55:51.925487 vectice-24.2.8.0/src/vectice/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/api/_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/api/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8075 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/api/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24535 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/api/columns_description.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/api/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/api/gql_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/api/gql_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6506 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/api/gql_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/api/gql_entity_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/api/gql_feature_flag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/api/gql_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7279 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/api/gql_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/api/gql_organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/api/gql_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/api/gql_user_workspace_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/api/http_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13467 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/api/http_error_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12109 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/api/iteration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:55:51.933487 vectice-24.2.8.0/src/vectice/api/json/
+-rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/api/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/api/json/artifact_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/api/json/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/api/json/code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/api/json/code_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/api/json/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/api/json/dataset_register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/api/json/dataset_representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/api/json/dataset_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/api/json/dataset_version_representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/api/json/entity_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/api/json/files_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/api/json/iteration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/api/json/json_to_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/api/json/json_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/api/json/last_assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/api/json/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/api/json/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/api/json/model_register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/api/json/model_representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/api/json/model_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/api/json/model_version_representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/api/json/organization_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/api/json/page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/api/json/paged_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/api/json/phase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/api/json/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/api/json/property.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/api/json/public_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/api/json/requirement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/api/json/section.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/api/json/user_and_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/api/json/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/api/json_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4894 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/api/phase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/api/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8364 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/api/rest_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/api/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/api/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:55:51.933487 vectice-24.2.8.0/src/vectice/autolog/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/autolog/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:55:51.933487 vectice-24.2.8.0/src/vectice/autolog/asset_services/
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/autolog/asset_services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/autolog/asset_services/catboost_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/autolog/asset_services/keras_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/autolog/asset_services/lightgbm_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/autolog/asset_services/metric_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/autolog/asset_services/pandas_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/autolog/asset_services/pyspark_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/autolog/asset_services/pytorch_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/autolog/asset_services/sklearn_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/autolog/asset_services/statsmodel_wrapper_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/autolog/asset_services/vectice_asset_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9925 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/autolog/autolog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/autolog/autolog_asset_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37125 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/autolog/autolog_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/autolog/model_library.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22308 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:55:51.937487 vectice-24.2.8.0/src/vectice/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/models/additional_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/models/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/models/attachment_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/models/code_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11659 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/models/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/models/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19029 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/models/iteration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/models/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11174 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/models/model_exp_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/models/model_mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6486 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/models/phase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6055 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/models/property.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:55:51.941487 vectice-24.2.8.0/src/vectice/models/representation/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/models/representation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/models/representation/dataset_representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7326 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/models/representation/dataset_version_representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/models/representation/model_representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7494 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/models/representation/model_version_representation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:55:51.941487 vectice-24.2.8.0/src/vectice/models/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/models/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/models/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8561 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/models/resource/bigquery_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11835 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/models/resource/databricks_table_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/models/resource/description.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6206 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/models/resource/file_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7333 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/models/resource/gcs_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:55:51.945487 vectice-24.2.8.0/src/vectice/models/resource/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/models/resource/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/models/resource/metadata/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/models/resource/metadata/column_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/models/resource/metadata/dataframe_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/models/resource/metadata/db_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/models/resource/metadata/df_wrapper_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/models/resource/metadata/df_wrapper_pandas_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/models/resource/metadata/df_wrapper_pyspark_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/models/resource/metadata/df_wrapper_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11952 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/models/resource/metadata/df_wrapper_spark_df.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/models/resource/metadata/extra_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/models/resource/metadata/files_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/models/resource/metadata/pyspark_pandas_dataframe_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/models/resource/metadata/pyspark_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/models/resource/metadata/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/models/resource/no_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9025 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/models/resource/s3_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7954 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/models/resource/snowflake_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/models/table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:55:51.945487 vectice-24.2.8.0/src/vectice/models/test_library/
+-rw-r--r--   0 runner    (1001) docker     (127)    11948 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/models/test_library/binary_classification_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/models/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/models/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:55:51.945487 vectice-24.2.8.0/src/vectice/services/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7367 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/services/iteration_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7354 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/services/phase_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:55:51.945487 vectice-24.2.8.0/src/vectice/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/types/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:55:51.945487 vectice-24.2.8.0/src/vectice/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/utils/api_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11664 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/utils/code_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15222 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/utils/common_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/utils/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/utils/dataframe_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9540 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/utils/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/utils/instance_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/utils/last_assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5342 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/utils/logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/utils/sklearn_pipe_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-06-03 07:55:41.000000 vectice-24.2.8.0/src/vectice/utils/vectice_ids_regex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:55:51.949487 vectice-24.2.8.0/src/vectice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-06-03 07:55:51.000000 vectice-24.2.8.0/src/vectice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-06-03 07:55:51.000000 vectice-24.2.8.0/src/vectice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 07:55:51.000000 vectice-24.2.8.0/src/vectice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-06-03 07:55:51.000000 vectice-24.2.8.0/src/vectice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-06-03 07:55:51.000000 vectice-24.2.8.0/src/vectice.egg-info/top_level.txt
```

### Comparing `vectice-24.2.7.0/LICENSE` & `vectice-24.2.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/PKG-INFO` & `vectice-24.2.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectice
-Version: 24.2.7.0
+Version: 24.2.8.0
 Summary: Vectice Python library
 Home-page: https://www.vectice.com
 Author: Vectice Inc.
 Author-email: sdk@vectice.com
 License: Apache License 2.0
 Keywords: Vectice,Client,API,Adapter
 Platform: Linux
@@ -26,15 +26,15 @@
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.7.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: types-python-dateutil
 Requires-Dist: python-dotenv>=0.11.0
-Requires-Dist: requests<=2.30.0
+Requires-Dist: requests<=2.31.0
 Requires-Dist: rich
 Requires-Dist: urllib3
 Requires-Dist: gql[requests]
 Requires-Dist: GitPython
 Requires-Dist: packaging
 Requires-Dist: Pillow
 Requires-Dist: pandas
```

### Comparing `vectice-24.2.7.0/pyproject.toml` & `vectice-24.2.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/setup.py` & `vectice-24.2.8.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     license="Apache License 2.0",
     keywords=["Vectice", "Client", "API", "Adapter"],
     platforms=["Linux", "MacOS X", "Windows"],
     python_requires=version_requires,
     install_requires=[
         "types-python-dateutil",
         "python-dotenv>=0.11.0",
-        "requests<=2.30.0",
+        "requests<=2.31.0",
         "rich",
         "urllib3",
         "gql[requests]",
         "GitPython",
         "packaging",
         "Pillow",
         "pandas",
```

### Comparing `vectice-24.2.7.0/src/vectice/__init__.py` & `vectice-24.2.8.0/src/vectice/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/api/_auth.py` & `vectice-24.2.8.0/src/vectice/api/_auth.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/api/attachment.py` & `vectice-24.2.8.0/src/vectice/api/attachment.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/api/client.py` & `vectice-24.2.8.0/src/vectice/api/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 from __future__ import annotations
 
+import csv
+import functools
 import logging
+import os
 import re
 from datetime import datetime
 from typing import TYPE_CHECKING, Any, BinaryIO
 
 from gql import Client as GQLClient
 from gql.transport.requests import RequestsHTTPTransport
 
 from vectice.__version__ import __version__
 from vectice.api._auth import Auth
 from vectice.api.attachment import AttachmentApi
+from vectice.api.columns_description import ColumnsDescriptionApi
 from vectice.api.compatibility import CompatibilityApi
 from vectice.api.gql_attachment import GqlAttachmentApi
 from vectice.api.gql_dataset import GqlDatasetApi
 from vectice.api.gql_entity_file import GqlEntityFileApi
 from vectice.api.gql_feature_flag import GqlFeatureFlagApi
 from vectice.api.gql_metric import GqlMetricApi
 from vectice.api.gql_model import GqlModelApi
@@ -43,14 +47,15 @@
 from vectice.api.json.model_representation import ModelRepresentationOutput
 from vectice.api.json.model_version_representation import ModelVersionRepresentationOutput, ModelVersionUpdateInput
 from vectice.api.json.organization_config import OrgConfigOutput
 from vectice.api.phase import PhaseApi
 from vectice.api.project import ProjectApi
 from vectice.api.version import VersionApi
 from vectice.api.workspace import WorkspaceApi
+from vectice.models.attachment_container import FILE_PATH_DOES_NOT_EXIST_ERROR_MESSAGE
 from vectice.models.dataset import Dataset
 from vectice.models.iteration import Iteration
 from vectice.models.model import Model
 from vectice.models.phase import Phase
 from vectice.models.representation.dataset_version_representation import DatasetVersionRepresentation
 from vectice.models.representation.model_version_representation import ModelVersionRepresentation
 from vectice.models.resource.metadata.base import DatasetSourceType, MetadataSettings
@@ -410,14 +415,21 @@
 
     def get_dataset_version(self, id: str) -> DatasetVersionRepresentationOutput:
         return GqlDatasetApi(self._gql_client, self.auth).get_dataset_version(id)
 
     def update_dataset_version(self, id: str, columns_description: list[dict[str, str]]):
         return GqlDatasetApi(self._gql_client, self.auth).update_dataset_version(id, columns_description)
 
+    def update_columns_description_via_csv(self, id: str, file_path: str):
+        if not os.path.exists(file_path):
+            raise ValueError(FILE_PATH_DOES_NOT_EXIST_ERROR_MESSAGE % file_path)
+        curr_file = ("file", (file_path, open(file_path, "rb")))
+        ColumnsDescriptionApi(self.auth).post_columns_description(id, curr_file)
+        curr_file[1][1].close()
+
     def get_model(self, id: str) -> ModelRepresentationOutput:
         return GqlModelApi(self._gql_client, self.auth).get_model(id)
 
     def get_model_version_list(self, id: str, size: int) -> PagedResponse[ModelVersionRepresentationOutput]:
         return GqlModelApi(self._gql_client, self.auth).get_model_version_list(id, size)
 
     def get_model_version(self, id: str) -> ModelVersionRepresentationOutput:
@@ -472,15 +484,27 @@
                 else:
                     for file in metadata_dict["files"]:
                         file["columns"] = self._combine_source_column_description(file, columns)
 
                 metadata_asdict.append(metadata_dict)
         return metadata_asdict, is_updating_columns
 
-    def _combine_source_column_description(self, source: dict, columns_description: dict[str, str]):
+    def _combine_source_column_description(self, source: dict, columns_description: dict[str, str] | str):
+        def _transform_path_to_dictionary(path: str):
+            def _reduce_csv(acc: dict[str, str], curr: list[str]):
+                if len(curr) > 1:
+                    return {**acc, curr[0]: curr[1]}
+                return acc
+
+            with open(path, mode="r", newline="") as csv_file:
+                return functools.reduce(_reduce_csv, csv.reader(csv_file), {})
+
+        if isinstance(columns_description, str):
+            columns_description = _transform_path_to_dictionary(columns_description)
+
         def _map_columns(col: dict):
             col_name = col["name"]
             if col_name in columns_description:
                 column_desc = columns_description[col_name]
                 return {**col, "description": column_desc}
             return col
```

### Comparing `vectice-24.2.7.0/src/vectice/api/gql_api.py` & `vectice-24.2.8.0/src/vectice/api/gql_api.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/api/gql_attachment.py` & `vectice-24.2.8.0/src/vectice/api/gql_attachment.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/api/gql_dataset.py` & `vectice-24.2.8.0/src/vectice/api/gql_dataset.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/api/gql_entity_file.py` & `vectice-24.2.8.0/src/vectice/api/gql_entity_file.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/api/gql_feature_flag.py` & `vectice-24.2.8.0/src/vectice/api/gql_feature_flag.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/api/gql_metric.py` & `vectice-24.2.8.0/src/vectice/api/gql_metric.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/api/gql_model.py` & `vectice-24.2.8.0/src/vectice/api/gql_model.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/api/gql_organization.py` & `vectice-24.2.8.0/src/vectice/api/gql_organization.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/api/gql_property.py` & `vectice-24.2.8.0/src/vectice/api/gql_property.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/api/gql_user_workspace_api.py` & `vectice-24.2.8.0/src/vectice/api/gql_user_workspace_api.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/api/http_error.py` & `vectice-24.2.8.0/src/vectice/api/http_error.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/api/http_error_handlers.py` & `vectice-24.2.8.0/src/vectice/api/http_error_handlers.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/api/iteration.py` & `vectice-24.2.8.0/src/vectice/api/iteration.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/api/json/__init__.py` & `vectice-24.2.8.0/src/vectice/api/json/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/api/json/artifact_version.py` & `vectice-24.2.8.0/src/vectice/api/json/artifact_version.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/api/json/code.py` & `vectice-24.2.8.0/src/vectice/api/json/code.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/api/json/code_version.py` & `vectice-24.2.8.0/src/vectice/api/json/code_version.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/api/json/dataset_register.py` & `vectice-24.2.8.0/src/vectice/api/json/dataset_register.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/api/json/dataset_representation.py` & `vectice-24.2.8.0/src/vectice/api/json/dataset_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/api/json/dataset_version.py` & `vectice-24.2.8.0/src/vectice/api/json/dataset_version.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/api/json/dataset_version_representation.py` & `vectice-24.2.8.0/src/vectice/api/json/dataset_version_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/api/json/files_metadata.py` & `vectice-24.2.8.0/src/vectice/api/json/files_metadata.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/api/json/iteration.py` & `vectice-24.2.8.0/src/vectice/api/json/iteration.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/api/json/json_to_class.py` & `vectice-24.2.8.0/src/vectice/api/json/json_to_class.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/api/json/last_assets.py` & `vectice-24.2.8.0/src/vectice/api/json/last_assets.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/api/json/metric.py` & `vectice-24.2.8.0/src/vectice/api/json/metric.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/api/json/model.py` & `vectice-24.2.8.0/src/vectice/api/json/model.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/api/json/model_register.py` & `vectice-24.2.8.0/src/vectice/api/json/model_register.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/api/json/model_representation.py` & `vectice-24.2.8.0/src/vectice/api/json/model_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/api/json/model_version.py` & `vectice-24.2.8.0/src/vectice/api/json/model_version.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/api/json/model_version_representation.py` & `vectice-24.2.8.0/src/vectice/api/json/model_version_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/api/json/paged_response.py` & `vectice-24.2.8.0/src/vectice/api/json/paged_response.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/api/json/phase.py` & `vectice-24.2.8.0/src/vectice/api/json/phase.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/api/json/project.py` & `vectice-24.2.8.0/src/vectice/api/json/project.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/api/json/property.py` & `vectice-24.2.8.0/src/vectice/api/json/property.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/api/json/public_config.py` & `vectice-24.2.8.0/src/vectice/api/json/public_config.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/api/json/requirement.py` & `vectice-24.2.8.0/src/vectice/api/json/requirement.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/api/json/user_and_workspace.py` & `vectice-24.2.8.0/src/vectice/api/json/user_and_workspace.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/api/json/workspace.py` & `vectice-24.2.8.0/src/vectice/api/json/workspace.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/api/phase.py` & `vectice-24.2.8.0/src/vectice/api/phase.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/api/project.py` & `vectice-24.2.8.0/src/vectice/api/project.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/api/rest_api.py` & `vectice-24.2.8.0/src/vectice/api/rest_api.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/api/version.py` & `vectice-24.2.8.0/src/vectice/api/version.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/api/workspace.py` & `vectice-24.2.8.0/src/vectice/api/workspace.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/autolog/asset_services/__init__.py` & `vectice-24.2.8.0/src/vectice/autolog/asset_services/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/autolog/asset_services/catboost_service.py` & `vectice-24.2.8.0/src/vectice/autolog/asset_services/catboost_service.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/autolog/asset_services/keras_service.py` & `vectice-24.2.8.0/src/vectice/autolog/asset_services/keras_service.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/autolog/asset_services/lightgbm_service.py` & `vectice-24.2.8.0/src/vectice/autolog/asset_services/lightgbm_service.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/autolog/asset_services/metric_service.py` & `vectice-24.2.8.0/src/vectice/autolog/asset_services/metric_service.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/autolog/asset_services/pytorch_service.py` & `vectice-24.2.8.0/src/vectice/autolog/asset_services/pytorch_service.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/autolog/asset_services/sklearn_service.py` & `vectice-24.2.8.0/src/vectice/autolog/asset_services/sklearn_service.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,23 +14,28 @@
         super().__init__(cell_data=data)
 
     def get_asset(self):
         # xgboost relies on BaseEstimator
         # lightgbm has Booster and sklearn API which uses BaseEstimator
         try:
             from sklearn.base import is_classifier, is_regressor
+            from sklearn.pipeline import Pipeline
 
-            if is_regressor(self._asset) or is_classifier(self._asset):
+            if is_regressor(self._asset) or is_classifier(self._asset) or isinstance(self._asset, Pipeline):
+                library = ModelLibrary.SKLEARN
+
+                if isinstance(self._asset, Pipeline):
+                    library = ModelLibrary.SKLEARN_PIPELINE
                 try:
                     # TODO fix regex picking up classes
                     # Ignore Initialized variables e.g LogisticRegression Class
                     self._asset.get_params()  # pyright: ignore[reportGeneralTypeIssues]
                     return {
                         "variable": self._key,
                         "model": self._asset,
-                        "library": ModelLibrary.SKLEARN,
+                        "library": library,
                         "metrics": self._get_model_metrics(self._cell_data),
                     }
                 except Exception:
                     pass
         except ImportError:
             pass
```

### Comparing `vectice-24.2.7.0/src/vectice/autolog/asset_services/statsmodel_wrapper_service.py` & `vectice-24.2.8.0/src/vectice/autolog/asset_services/statsmodel_wrapper_service.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/autolog/asset_services/vectice_asset_service.py` & `vectice-24.2.8.0/src/vectice/autolog/asset_services/vectice_asset_service.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/autolog/autolog.py` & `vectice-24.2.8.0/src/vectice/autolog/autolog.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     ```
 
 2.** Supported libraries and environment:**
     Vectice automatically identifies and log assets encapsulated within a specified list of supported libraries and environement mentioned below
 
 NOTE: **Supported libraries and environment**
     - Dataframe: Pandas, Spark.
-    - Model: Scikit, Xgboost, Lightgbm, Catboost, Keras, Pytorch.
+    - Model: Scikit, Xgboost, Lightgbm, Catboost, Keras, Pytorch, Statsmodels.
     - Graphs: Matplotlib, Seaborn, Plotly.
     - Environments: Colab, Jupyter, Vertex, SageMaker, Databricks, Pycharm and VScode notebook.
 
 3.** General behavior:**
     Vectice autolog provides three methods: autolog.config, autolog.notebook, and autolog.cell. These methods are designed to log every asset to Vectice existing as a variable in the notebook's memory. It is important to review the specific behaviors outlined in the documentation for each of these three methods.
 
 NOTE: **IMPORTANT INFORMATION**
```

### Comparing `vectice-24.2.7.0/src/vectice/autolog/autolog_asset_factory.py` & `vectice-24.2.8.0/src/vectice/autolog/autolog_asset_factory.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/autolog/autolog_class.py` & `vectice-24.2.8.0/src/vectice/autolog/autolog_class.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,23 +28,24 @@
     from catboost.core import CatBoost
     from keras import Model as KerasModel  # type: ignore[reportMissingImports]
     from keras.layers import InputLayer  # type: ignore[reportMissingImports]
     from lightgbm.basic import Booster
     from pandas import DataFrame
     from pyspark.sql import DataFrame as SparkDF
     from sklearn.base import BaseEstimator
+    from sklearn.pipeline import Pipeline
     from statsmodels.base.wrapper import ResultsWrapper
     from torch.nn import Module as TorchModel
 
     # Vectice Object types
     from vectice.autolog.asset_services import TVecticeObjects
     from vectice.models import Phase
     from vectice.models.resource.metadata.db_metadata import TableType
 
-    ModelTypes = TypeVar("ModelTypes", BaseEstimator, Booster, CatBoost, KerasModel, TorchModel)
+    ModelTypes = TypeVar("ModelTypes", BaseEstimator, Booster, CatBoost, KerasModel, TorchModel, Pipeline)
     TModel = TypedDict(
         "TModel",
         {
             "variable": str,
             "model": ModelTypes,
             "library": ModelLibrary,
             "metrics": dict,
@@ -283,15 +284,14 @@
                     "Autolog is unable to parse the code. Make sure all non-Python syntax, such as bash commands, are properly indented and preceded by '%' or '!'. If the error persist, please contact your sales representative."
                 ) from err
 
             visitor = VariableVisitor()
             visitor.visit(tree)
             # Keep set of all vectice call vars
             all_vectice_calls = all_vectice_calls.union(visitor.vectice_call_vars)
-
             # Update all_vars with variable names and values in the order they appear
             for var in visitor.variables:
                 if var in local_vars and var not in all_vars:
                     all_vars[var] = local_vars[var]
                 # check if the var exists in a previous cell for autolog.notebook before the vectice object uses the var
                 if self._is_notebook:
                     all_vectice_calls = {vect_var for vect_var in all_vectice_calls if vect_var not in all_cell_vars}
@@ -394,14 +394,54 @@
     def _get_model_library(self, model: ModelTypes):
         if "xgboost" in str(model.__class__):
             return "xgboost"
         if "lightgbm" in str(model.__class__):
             return "lightgbm"
         return "sklearn"
 
+    def _get_pipeline_steps(self, pipeline: Pipeline) -> dict:
+        sklearn_pipeline = {}
+        try:
+            for step in pipeline.steps:
+                step_name, step_obj = step
+                if hasattr(step_obj, "named_transformers_"):
+                    for k, v in step_obj.named_transformers_.items():
+                        sklearn_pipeline[f"pipeline_{step_name}_{k}_steps"] = list(v.named_steps.keys())
+            return sklearn_pipeline
+        except Exception:
+            return sklearn_pipeline
+
+    def _get_pipeline_info(self, pipeline: Pipeline) -> tuple[str, dict[str, Any]] | tuple[None, None]:
+        # if pipeline with classifier
+        try:
+            from sklearn.base import is_classifier, is_regressor
+
+            model = pipeline.steps[-1][-1]
+            model_name = pipeline.steps[-1][0]
+            if is_regressor(model) or is_classifier(model):
+                model_params = {
+                    f"{model_name}_{key}": value
+                    for key, value in model.get_params().items()
+                    if value is not None and bool(str(value))
+                }
+                model_params.update(self._get_pipeline_steps(pipeline))
+                return "sklearn-pipeline", model_params
+        except Exception:
+            pass
+
+        try:
+            pipeline_params = {
+                str(key): value
+                for key, value in pipeline.get_params().items()
+                if value is not None and bool(str(value))
+            }
+            return "sklearn-pipeline", pipeline_params
+        except Exception:
+            return None, None
+
     def _get_sklearn_or_xgboost_or_lgbm_info(
         self, model: BaseEstimator
     ) -> tuple[str, dict[str, Any]] | tuple[None, None]:
         try:
             library = self._get_model_library(model)
             params = {
                 str(key): value for key, value in model.get_params().items() if value is not None and bool(str(value))
@@ -563,14 +603,16 @@
 
     def _get_model_params(self, asset: TModel) -> tuple[str, dict[str, Any]] | tuple[None, None]:
         library = asset["library"]
         model = asset["model"]
 
         if library is ModelLibrary.SKLEARN:
             return self._get_sklearn_or_xgboost_or_lgbm_info(model)  # pyright: ignore[reportArgumentType]
+        if library is ModelLibrary.SKLEARN_PIPELINE:
+            return self._get_pipeline_info(model)  # pyright: ignore[reportArgumentType]
         if library is ModelLibrary.LIGHTGBM:
             return self._get_lightgbm_info(model)  # pyright: ignore[reportArgumentType]
         if library is ModelLibrary.CATBOOST:
             return self._get_catboost_info(model)  # pyright: ignore[reportArgumentType]
         if library is ModelLibrary.KERAS:
             return self._get_keras_info(model)  # pyright: ignore[reportArgumentType]
         if library is ModelLibrary.STATSMODEL:
@@ -625,42 +667,85 @@
 
         model_object = model["model"]
 
         library, params = self._get_model_params(model)
         if model["library"] is ModelLibrary.STATSMODEL:
             algorithm = str(model_object.model.__class__).split(".")[-1]  # type: ignore[reportAttributeAccessIssue]
             model_summary = model_object.summary().as_text()  # type: ignore[reportAttributeAccessIssue]
+        elif model["library"] is ModelLibrary.SKLEARN_PIPELINE:
+            model_summary = None
+            try:
+                algorithm = str(model_object.steps[-1][-1].__class__).split(".")[-1]  # type: ignore[reportAttributeAccessIssue]
+            except Exception:
+                algorithm = str(model_object.__class__).split(".")[-1]
         else:
             algorithm = str(model_object.__class__).split(".")[-1]
             model_summary = None
 
         algorithm = algorithm.replace("'>", "")
         model_name = f"{self._iteration.phase.id}-{model['variable']}"
         # safety check, if no metrics and single model, get metrics
         model_metrics = model["metrics"] if model["metrics"] else self._get_single_model_metrics()
+        temp_files = []
+        if library == "sklearn-pipeline":
+            temp_dir, temp_json_file_path, temp_html_file_path = self._get_sklearn_pipeline(model_object, model_name)
+            if temp_json_file_path:
+                temp_files.append(temp_json_file_path)
+            if temp_html_file_path:
+                temp_files.append(temp_html_file_path)
+
         self._iteration_service.log_model(
             Model(
                 library=library,
                 technique=algorithm,
                 metrics=model_metrics,
                 properties=params,
                 name=model_name,
                 predictor=model_object,
-                attachments=temp_file_path,
+                attachments=temp_file_path or temp_files,
             )
         )
         _logger.info(f"Model {model_name!r} logged in iteration {self._iteration.name!r}.")
 
         if model_summary:
             # log statsmodel summary
             self._iteration_service.log_comment(model_summary)
 
         if temp_dir is not None:
             temp_dir.cleanup()
 
+    def _get_sklearn_pipeline(
+        self, pipeline: ModelTypes, model_name: str
+    ) -> tuple[TemporaryDirectory[str], str, str] | tuple[None, None, None]:
+        temp_dir = None
+        try:
+            from sklearn.utils import estimator_html_repr
+
+            from vectice.utils.sklearn_pipe_utils import pipeline_to_json
+
+            temp_dir = tempfile.TemporaryDirectory()
+            json_file_name = f"{model_name!s}_pipeline.json"
+            html_file_name = f"{model_name!s}_pipeline.html"
+            temp_json_file_path = rf"{temp_dir.name}\{json_file_name}"
+            temp_html_file_path = rf"{temp_dir.name}\{html_file_name}"
+
+            pipeline_json = pipeline_to_json(pipeline)
+            pipeline_html = estimator_html_repr(pipeline)
+            if pipeline_json:
+                with open(temp_json_file_path, "w") as json_file:
+                    json_file.write(pipeline_json)
+
+            if pipeline_html:
+                with open(temp_html_file_path, "w", encoding="utf-8") as html_file:
+                    html_file.write(pipeline_html)
+
+            return temp_dir, temp_json_file_path, temp_html_file_path
+        except Exception:
+            return None, None, None
+
     def _log_vectice_asset(self, asset: TVecticeObjects) -> None:
         asset_to_log = asset["vectice_object"]
         asset_name = asset["variable"]
         if isinstance(asset_to_log, Dataset):
             dataset_name = asset_to_log.name if asset_to_log.name else asset_name
             self._iteration_service.log_dataset(asset_to_log)
             _logger.info(f"Dataset {dataset_name!r} logged in iteration {self._iteration.name!r}.")
```

### Comparing `vectice-24.2.7.0/src/vectice/connection.py` & `vectice-24.2.8.0/src/vectice/connection.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/models/__init__.py` & `vectice-24.2.8.0/src/vectice/models/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/models/additional_info.py` & `vectice-24.2.8.0/src/vectice/models/additional_info.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/models/attachment_container.py` & `vectice-24.2.8.0/src/vectice/models/attachment_container.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/models/code_version.py` & `vectice-24.2.8.0/src/vectice/models/code_version.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/models/dataset.py` & `vectice-24.2.8.0/src/vectice/models/dataset.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/models/iteration.py` & `vectice-24.2.8.0/src/vectice/models/iteration.py`

 * *Files 0% similar despite different names*

```diff
@@ -405,15 +405,15 @@
             self._log_model(asset, section)
 
         elif isinstance(asset, Dataset):
             self._log_dataset(asset, section)
         elif isinstance(asset, ValidationModel):
             self._log_validation_model(asset, section)
         else:
-            raise TypeError(f"Expected Image, Comment, Dataset or a Model, got {type(asset)}")
+            raise TypeError(f"Expected Image, Comment, Table, Dataset or a Model, got {type(asset)}")
 
     def _log_image_or_file(self, asset: str | IOBase | Image, section: str | None = None):
         filename = self._service.log_image_or_file(asset, section)
         comment_or_image_logging(self, _logger, section, filename)
 
     def _log_comment(self, asset: int | float | str, section: str | None = None):
         self._service.log_comment(asset, section)
```

### Comparing `vectice-24.2.7.0/src/vectice/models/metric.py` & `vectice-24.2.8.0/src/vectice/models/metric.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/models/model.py` & `vectice-24.2.8.0/src/vectice/models/model.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/models/model_exp_tracker.py` & `vectice-24.2.8.0/src/vectice/models/model_exp_tracker.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/models/model_mlflow.py` & `vectice-24.2.8.0/src/vectice/models/model_mlflow.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/models/phase.py` & `vectice-24.2.8.0/src/vectice/models/phase.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/models/project.py` & `vectice-24.2.8.0/src/vectice/models/project.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/models/property.py` & `vectice-24.2.8.0/src/vectice/models/property.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/models/representation/dataset_representation.py` & `vectice-24.2.8.0/src/vectice/models/representation/dataset_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/models/representation/dataset_version_representation.py` & `vectice-24.2.8.0/src/vectice/models/representation/dataset_version_representation.py`

 * *Files 3% similar despite different names*

```diff
@@ -107,22 +107,22 @@
             }
         return flattened_resource
 
     def update(
         self,
         properties: dict[str, str | int] | list[Property] | Property | None = None,
         attachments: str | list[str] | None = None,
-        columns_description: dict[str, str] | None = None,
+        columns_description: dict[str, str] | str | None = None,
     ) -> None:
         """Update the Dataset Version from the API.
 
         Parameters:
             properties: The new properties of the dataset.
             attachments: The new attachments of the dataset.
-            columns_description: A dictionary to map the column's name to a specific description. Should follow the format { "column_name": "Description", ... }
+            columns_description: A dictionary or path to a csv file to map the column's name to a specific description. Should follow the format { "column_name": "Description", ... }
 
         Returns:
             None
         """
         if properties is not None:
             self._upsert_properties(properties)
 
@@ -139,13 +139,17 @@
         _logger.info(f"Dataset version {self.id!r} properties successfully updated.")
 
     def _update_attachments(self, attachments: TAttachment):
         container = AttachmentContainer(self._output, self._client)
         container.upsert_attachments(format_attachments(attachments))
         _logger.info(f"Dataset version {self.id!r} attachments successfully updated.")
 
-    def _update_dataset_version(self, columns_description: dict[str, str]):
-        items = columns_description.items()
-        list_columns_description = list(map(lambda x: {"name": x[0], "description": x[1]}, items))
-        self._client.update_dataset_version(self.id, list_columns_description)
+    def _update_dataset_version(self, columns_description: dict[str, str] | str):
+        if isinstance(columns_description, str):
+            self._client.update_columns_description_via_csv(self.id, columns_description)
+        else:
+            items = columns_description.items()
+            list_columns_description = list(map(lambda x: {"name": x[0], "description": x[1]}, items))
+            self._client.update_dataset_version(self.id, list_columns_description)
+
         self._client.warn_if_dataset_version_columns_are_missing_description(self.id)
         _logger.info(f"Dataset version {self.id!r} columns descriptions successfully updated.")
```

### Comparing `vectice-24.2.7.0/src/vectice/models/representation/model_representation.py` & `vectice-24.2.8.0/src/vectice/models/representation/model_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/models/representation/model_version_representation.py` & `vectice-24.2.8.0/src/vectice/models/representation/model_version_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/models/resource/__init__.py` & `vectice-24.2.8.0/src/vectice/models/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/models/resource/base.py` & `vectice-24.2.8.0/src/vectice/models/resource/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 
     @abstractmethod
     def __init__(
         self,
         paths: list[str] | str,
         dataframes: TDataFrameType | list[TDataFrameType] | None = None,
         capture_schema_only: bool = False,
-        columns_description: dict[str, str] | None = None,
+        columns_description: dict[str, str] | str | None = None,
     ):
         """Initialize a resource."""
         self._metadata: Metadata | None = None
         self._data: dict | None = None
         if paths:
             self._paths = paths if isinstance(paths, list) else [paths]
         else:
```

### Comparing `vectice-24.2.7.0/src/vectice/models/resource/bigquery_resource.py` & `vectice-24.2.8.0/src/vectice/models/resource/bigquery_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,24 +42,24 @@
 
     def __init__(
         self,
         paths: str | list[str],
         dataframes: TDataFrameType | list[TDataFrameType] | None = None,
         bq_client: BQClient | None = None,
         capture_schema_only: bool = False,
-        columns_description: dict[str, str] | None = None,
+        columns_description: dict[str, str] | str | None = None,
     ):
         """Initialize a BigQuery resource.
 
         Parameters:
             paths: The paths to retrieve the datasets or the tables.
             dataframes (Optional): The dataframes allowing vectice to optionally compute more metadata about this resource such as columns stats. (Support Pandas, Spark)
             bq_client (Optional): The `google.cloud.bigquery.Client` to optionally retrieve file size, creation date and updated date (used for auto-versioning).
             capture_schema_only (Optional): A boolean parameter indicating whether to capture only the schema or both the schema and column statistics of the dataframes.
-            columns_description (Optional): A dictionary to map the column's name to a specific description. Should follow the format { "column_name": "Description", ... }
+            columns_description (Optional): A dictionary or path to a csv file to map the column's name to a specific description. Dictionary should follow the format { "column_name": "Description", ... }
 
         """
         super().__init__(
             paths=paths,
             dataframes=dataframes,
             capture_schema_only=capture_schema_only,
             columns_description=columns_description,
```

### Comparing `vectice-24.2.7.0/src/vectice/models/resource/databricks_table_resource.py` & `vectice-24.2.8.0/src/vectice/models/resource/databricks_table_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,24 +51,25 @@
 
     def __init__(
         self,
         paths: str | list[str],
         dataframes: TDataFrameType | list[TDataFrameType] | None = None,
         spark_client: SparkSession | None = None,
         capture_schema_only: bool = False,
-        columns_description: dict[str, str] | None = None,
+        columns_description: dict[str, str] | str | None = None,
     ):
         """Initialize a DatabricksTableResource resource.
 
         Parameters:
             paths: The paths to retrieve the tables. Should be either the table name or the location of the table.
             dataframes (Optional): The dataframes allowing vectice to optionally compute more metadata about this resource such as columns stats. (Support Pandas, Spark)
             spark_client (Optional): The spark session allowing vectice to capture the table metadata.
             capture_schema_only (Optional): A boolean parameter indicating whether to capture only the schema or both the schema and column statistics of the dataframes.
-            columns_description (Optional): A dictionary to map the column's name to a specific description. Should follow the format { "column_name": "Description", ... }
+            columns_description (Optional): A dictionary or path to a csv file to map the column's name to a specific description. Dictionary should follow the format { "column_name": "Description", ... }
+
         """
         if spark_imported is False:
             raise ImportError("Pyspark is not installed.")
         super().__init__(
             paths=paths,
             dataframes=dataframes,
             capture_schema_only=capture_schema_only,
```

### Comparing `vectice-24.2.7.0/src/vectice/models/resource/description.py` & `vectice-24.2.8.0/src/vectice/models/resource/description.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/models/resource/file_resource.py` & `vectice-24.2.8.0/src/vectice/models/resource/file_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,23 +35,23 @@
     _origin = DatasetSourceOrigin.LOCAL.value
 
     def __init__(
         self,
         paths: str | list[str],
         dataframes: TDataFrameType | list[TDataFrameType] | None = None,
         capture_schema_only: bool = False,
-        columns_description: dict[str, str] | None = None,
+        columns_description: dict[str, str] | str | None = None,
     ):
         """Initialize a file resource.
 
         Parameters:
             paths: The paths of the files to wrap.
             dataframes (Optional): The dataframes allowing vectice to optionally compute more metadata about this resource such as columns stats. (Support Pandas, Spark)
             capture_schema_only (Optional): A boolean parameter indicating whether to capture only the schema or both the schema and column statistics of the dataframes.
-            columns_description (Optional): A dictionary to map the column's name to a specific description. Should follow the format { "column_name": "Description", ... }
+            columns_description (Optional): A dictionary or path to a csv file to map the column's name to a specific description. Dictionary should follow the format { "column_name": "Description", ... }
 
         Examples:
             The following example shows how to wrap a CSV file
             called `iris.csv` in the current directory:
 
             ```python
             from vectice import FileResource
```

### Comparing `vectice-24.2.7.0/src/vectice/models/resource/gcs_resource.py` & `vectice-24.2.8.0/src/vectice/models/resource/gcs_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,24 +44,25 @@
 
     def __init__(
         self,
         uris: str | list[str],
         dataframes: TDataFrameType | list[TDataFrameType] | None = None,
         gcs_client: Client | None = None,
         capture_schema_only: bool = False,
-        columns_description: dict[str, str] | None = None,
+        columns_description: dict[str, str] | str | None = None,
     ):
         """Initialize a GCS resource.
 
         Parameters:
             uris: The uris of the referenced resources. Should follow the pattern 'gs://<bucket_name>/<file_path_inside_bucket>'
             dataframes (Optional): The dataframes allowing vectice to optionally compute more metadata about this resource such as columns stats. (Support Pandas, Spark)
             gcs_client (Optional): The `google.cloud.storage.Client` to optionally retrieve file size, creation date and updated date (used for auto-versioning) up to 5000 files.
             capture_schema_only (Optional): A boolean parameter indicating whether to capture only the schema or both the schema and column statistics of the dataframes.
-            columns_description (Optional): A dictionary to map the column's name to a specific description. Should follow the format { "column_name": "Description", ... }
+            columns_description (Optional): A dictionary or path to a csv file to map the column's name to a specific description. Dictionary should follow the format { "column_name": "Description", ... }
+
         """
         super().__init__(
             paths=uris,
             dataframes=dataframes,
             capture_schema_only=capture_schema_only,
             columns_description=columns_description,
         )
```

### Comparing `vectice-24.2.7.0/src/vectice/models/resource/metadata/__init__.py` & `vectice-24.2.8.0/src/vectice/models/resource/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/models/resource/metadata/base.py` & `vectice-24.2.8.0/src/vectice/models/resource/metadata/base.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/models/resource/metadata/column_metadata.py` & `vectice-24.2.8.0/src/vectice/models/resource/metadata/column_metadata.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/models/resource/metadata/dataframe_config.py` & `vectice-24.2.8.0/src/vectice/models/resource/metadata/dataframe_config.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/models/resource/metadata/db_metadata.py` & `vectice-24.2.8.0/src/vectice/models/resource/metadata/db_metadata.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/models/resource/metadata/df_wrapper_pandas.py` & `vectice-24.2.8.0/src/vectice/models/resource/metadata/df_wrapper_pandas.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/models/resource/metadata/df_wrapper_pandas_default.py` & `vectice-24.2.8.0/src/vectice/models/resource/metadata/df_wrapper_pandas_default.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/models/resource/metadata/df_wrapper_pyspark_pandas.py` & `vectice-24.2.8.0/src/vectice/models/resource/metadata/df_wrapper_pyspark_pandas.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/models/resource/metadata/df_wrapper_resource.py` & `vectice-24.2.8.0/src/vectice/models/resource/metadata/df_wrapper_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/models/resource/metadata/df_wrapper_spark_df.py` & `vectice-24.2.8.0/src/vectice/models/resource/metadata/df_wrapper_spark_df.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/models/resource/metadata/files_metadata.py` & `vectice-24.2.8.0/src/vectice/models/resource/metadata/files_metadata.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/models/resource/metadata/pyspark_pandas_dataframe_typing.py` & `vectice-24.2.8.0/src/vectice/models/resource/metadata/pyspark_pandas_dataframe_typing.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/models/resource/metadata/source.py` & `vectice-24.2.8.0/src/vectice/models/resource/metadata/source.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/models/resource/no_resource.py` & `vectice-24.2.8.0/src/vectice/models/resource/no_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/models/resource/s3_resource.py` & `vectice-24.2.8.0/src/vectice/models/resource/s3_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,24 +47,24 @@
 
     def __init__(
         self,
         uris: str | list[str],
         dataframes: TDataFrameType | list[TDataFrameType] | None = None,
         s3_client: Client | None = None,
         capture_schema_only: bool = False,
-        columns_description: dict[str, str] | None = None,
+        columns_description: dict[str, str] | str | None = None,
     ):
         """Initialize an S3 resource.
 
         Parameters:
             uris: The uris of the resources to get. Should follow the pattern 's3://<bucket_name>/<file_path_inside_bucket>'
             dataframes (Optional): The dataframes allowing vectice to optionally compute more metadata about this resource such as columns stats. (Support Pandas, Spark)
             s3_client (Optional): The Amazon s3 client to optionally retrieve file size, creation date and updated date (used for auto-versioning) up to 5000 files.
             capture_schema_only (Optional): A boolean parameter indicating whether to capture only the schema or both the schema and column statistics of the dataframes.
-            columns_description (Optional): A dictionary to map the column's name to a specific description. Should follow the format { "column_name": "Description", ... }
+            columns_description (Optional): A dictionary or path to a csv file to map the column's name to a specific description. Dictionary should follow the format { "column_name": "Description", ... }
 
         """
         super().__init__(
             paths=uris,
             dataframes=dataframes,
             capture_schema_only=capture_schema_only,
             columns_description=columns_description,
```

### Comparing `vectice-24.2.7.0/src/vectice/models/resource/snowflake_resource.py` & `vectice-24.2.8.0/src/vectice/models/resource/snowflake_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,25 +64,25 @@
     def __init__(
         self,
         paths: str | list[str],
         dataframes: TDataFrameType | list[TDataFrameType] | None = None,
         snowflake_client: Session | None = None,
         capture_schema_only: bool = False,
         force_dataframe: bool = False,
-        columns_description: dict[str, str] | None = None,
+        columns_description: dict[str, str] | str | None = None,
     ):
         """Initialize a Snowflake resource.
 
         Parameters:
             paths: The pahts of the resources to get.
             dataframes (Optional): The dataframes allowing vectice to optionally compute more metadata about this resource such as columns stats. (Support Pandas, Spark)
             snowflake_client (Optional): The Snowflake client to retrieve table metadatas.
             capture_schema_only (Optional): A boolean parameter indicating whether to capture only the schema or both the schema and column statistics of the dataframes.
             force_dataframe (Optional): A boolean parameter indicating whether the dataframe should be inferred from the table itself.
-            columns_description (Optional): A dictionary to map the column's name to a specific description. Should follow the format { "column_name": "Description", ... }
+            columns_description (Optional): A dictionary or path to a csv file to map the column's name to a specific description. Dictionary should follow the format { "column_name": "Description", ... }
 
         """
         super().__init__(
             paths=paths,
             dataframes=dataframes,
             capture_schema_only=capture_schema_only,
             columns_description=columns_description,
```

### Comparing `vectice-24.2.7.0/src/vectice/models/table.py` & `vectice-24.2.8.0/src/vectice/models/table.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/models/test_library/binary_classification_test.py` & `vectice-24.2.8.0/src/vectice/models/test_library/binary_classification_test.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/models/validation.py` & `vectice-24.2.8.0/src/vectice/models/validation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/models/workspace.py` & `vectice-24.2.8.0/src/vectice/models/workspace.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/services/iteration_service.py` & `vectice-24.2.8.0/src/vectice/services/iteration_service.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/services/phase_service.py` & `vectice-24.2.8.0/src/vectice/services/phase_service.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/types/version.py` & `vectice-24.2.8.0/src/vectice/types/version.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/utils/code_parser.py` & `vectice-24.2.8.0/src/vectice/utils/code_parser.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/utils/common_utils.py` & `vectice-24.2.8.0/src/vectice/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/utils/configuration.py` & `vectice-24.2.8.0/src/vectice/utils/configuration.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/utils/dataframe_utils.py` & `vectice-24.2.8.0/src/vectice/utils/dataframe_utils.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/utils/deprecation.py` & `vectice-24.2.8.0/src/vectice/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/utils/instance_helper.py` & `vectice-24.2.8.0/src/vectice/utils/instance_helper.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/utils/last_assets.py` & `vectice-24.2.8.0/src/vectice/utils/last_assets.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice/utils/logging_utils.py` & `vectice-24.2.8.0/src/vectice/utils/logging_utils.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.7.0/src/vectice.egg-info/PKG-INFO` & `vectice-24.2.8.0/src/vectice.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectice
-Version: 24.2.7.0
+Version: 24.2.8.0
 Summary: Vectice Python library
 Home-page: https://www.vectice.com
 Author: Vectice Inc.
 Author-email: sdk@vectice.com
 License: Apache License 2.0
 Keywords: Vectice,Client,API,Adapter
 Platform: Linux
@@ -26,15 +26,15 @@
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.7.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: types-python-dateutil
 Requires-Dist: python-dotenv>=0.11.0
-Requires-Dist: requests<=2.30.0
+Requires-Dist: requests<=2.31.0
 Requires-Dist: rich
 Requires-Dist: urllib3
 Requires-Dist: gql[requests]
 Requires-Dist: GitPython
 Requires-Dist: packaging
 Requires-Dist: Pillow
 Requires-Dist: pandas
```

### Comparing `vectice-24.2.7.0/src/vectice.egg-info/SOURCES.txt` & `vectice-24.2.8.0/src/vectice.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 src/vectice.egg-info/requires.txt
 src/vectice.egg-info/top_level.txt
 src/vectice/api/__init__.py
 src/vectice/api/_auth.py
 src/vectice/api/_utils.py
 src/vectice/api/attachment.py
 src/vectice/api/client.py
+src/vectice/api/columns_description.py
 src/vectice/api/compatibility.py
 src/vectice/api/gql_api.py
 src/vectice/api/gql_attachment.py
 src/vectice/api/gql_dataset.py
 src/vectice/api/gql_entity_file.py
 src/vectice/api/gql_feature_flag.py
 src/vectice/api/gql_metric.py
@@ -145,8 +146,9 @@
 src/vectice/utils/common_utils.py
 src/vectice/utils/configuration.py
 src/vectice/utils/dataframe_utils.py
 src/vectice/utils/deprecation.py
 src/vectice/utils/instance_helper.py
 src/vectice/utils/last_assets.py
 src/vectice/utils/logging_utils.py
+src/vectice/utils/sklearn_pipe_utils.py
 src/vectice/utils/vectice_ids_regex.py
```

### Comparing `vectice-24.2.7.0/src/vectice.egg-info/requires.txt` & `vectice-24.2.8.0/src/vectice.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 types-python-dateutil
 python-dotenv>=0.11.0
-requests<=2.30.0
+requests<=2.31.0
 rich
 urllib3
 gql[requests]
 GitPython
 packaging
 Pillow
 pandas
```

