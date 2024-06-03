# Comparing `tmp/dao_analyzer-1.3.3.dev6.tar.gz` & `tmp/dao_analyzer-1.3.3.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dao_analyzer-1.3.3.dev6.tar", last modified: Mon May 27 09:59:52 2024, max compression
+gzip compressed data, was "dao_analyzer-1.3.3.dev7.tar", last modified: Mon Jun  3 15:35:47 2024, max compression
```

## Comparing `dao_analyzer-1.3.3.dev6.tar` & `dao_analyzer-1.3.3.dev7.tar`

### file list

```diff
@@ -1,412 +1,412 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.641815 dao_analyzer-1.3.3.dev6/
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/.envrc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.581815 dao_analyzer-1.3.3.dev6/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.581815 dao_analyzer-1.3.3.dev6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     5782 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/.hintrc
--rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/ABOUT.md
--rw-r--r--   0 runner    (1001) docker     (127)     7608 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12201 2024-05-27 09:59:52.641815 dao_analyzer-1.3.3.dev6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9815 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.569815 dao_analyzer-1.3.3.dev6/dao_analyzer/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.585815 dao_analyzer-1.3.3.dev6/dao_analyzer/web/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-27 09:59:52.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.585815 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.585815 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.585815 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/business/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/business/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16209 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/business/app_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.585815 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/business/metric_adapter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/business/metric_adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/business/metric_adapter/asset_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/business/metric_adapter/asset_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/business/metric_adapter/basic_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/business/metric_adapter/cast_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/business/metric_adapter/installed_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/business/metric_adapter/vote_outcome.py
--rw-r--r--   0 runner    (1001) docker     (127)   399465 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/class_diagram.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.585815 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/data_access/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/data_access/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.585815 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/data_access/daos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/data_access/daos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.589815 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6301 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/metric_dao_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/srcs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.589815 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_active_organization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_active_token_holders.py
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_active_voters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_approval_vote_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_assets_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_assets_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_cast_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_casted_votes_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_casted_votes_voters_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_installed_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_new_additions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_organization_activity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_total_token_holders.py
--rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_vote_outcome.py
--rw-r--r--   0 runner    (1001) docker     (127)     5890 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/data_access/daos/platform_dao.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.589815 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/presentation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/presentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.589815 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/resources/strings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.593814 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.593814 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.593814 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/api/graphql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/api/graphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/api/graphql/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/api/graphql/query_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.593814 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/business/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/business/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/business/i_metric_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/business/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.593814 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/business/transfers/
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/business/transfers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/business/transfers/hierarchical_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/business/transfers/n_stacked_serie.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.593814 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/business/transfers/organization/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/business/transfers/organization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/business/transfers/organization/organization.py
--rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/business/transfers/organization/organization_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5678 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/business/transfers/organization/organization_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/business/transfers/organization/participation_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/business/transfers/organization/platform.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/business/transfers/serie.py
--rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/business/transfers/stacked_serie.py
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/business/transfers/tabular_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.593814 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/data_access/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/data_access/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.597814 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/data_access/daos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/data_access/daos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.597814 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/data_access/daos/metric/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/data_access/daos/metric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/data_access/daos/metric/metric_dao.py
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/data_access/daos/metric/srcs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.597814 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/data_access/daos/metric/strategy/
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/data_access/daos/metric/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/data_access/daos/metric/strategy/imetric_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/data_access/daos/metric/strategy/st_assets_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     4554 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/data_access/daos/metric/strategy/st_assets_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/data_access/daos/platform_dao.py
--rw-r--r--   0 runner    (1001) docker     (127)     4369 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/data_access/pandas_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.597814 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/data_access/requesters/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/data_access/requesters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/data_access/requesters/cache_requester.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/data_access/requesters/irequester.py
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/data_access/requesters/join_cache_requester.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.597814 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/presentation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/presentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.597814 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/presentation/about_view/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/presentation/about_view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/presentation/about_view/about_view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.597814 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/presentation/charts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/presentation/charts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/presentation/charts/chart_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/presentation/charts/chart_sum_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/presentation/charts/dt_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.601815 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/presentation/charts/layout/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/presentation/charts/layout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/presentation/charts/layout/chart_pane_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3711 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/presentation/charts/layout/chart_pane_layout.py
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/presentation/charts/layout/data_table_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/presentation/charts/layout/data_table_layout.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.601815 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/presentation/charts/layout/figure/
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/presentation/charts/layout/figure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/presentation/charts/layout/figure/bar_figure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/presentation/charts/layout/figure/calplot.py
--rw-r--r--   0 runner    (1001) docker     (127)     4723 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/presentation/charts/layout/figure/double_scatter_figure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/presentation/charts/layout/figure/figure.py
--rw-r--r--   0 runner    (1001) docker     (127)     4532 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/presentation/charts/layout/figure/figure_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/presentation/charts/layout/figure/multi_bar_figure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/presentation/charts/layout/figure/treemap_figure.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/presentation/charts/layout/ilayout.py
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/presentation/charts/layout/layout_configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.601815 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/presentation/dashboard_view/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/presentation/dashboard_view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/presentation/dashboard_view/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     9375 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/presentation/dashboard_view/dashboard_view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.601815 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/presentation/main_view/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/presentation/main_view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/presentation/main_view/main_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     6670 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/presentation/main_view/main_view_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.601815 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/resources/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/resources/strings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.605815 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.605815 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/business/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/business/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16026 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/business/app_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.605815 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/business/metric_adapter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/business/metric_adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/business/metric_adapter/asset_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/business/metric_adapter/asset_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/business/metric_adapter/basic_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/business/metric_adapter/proposal_outcome.py
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/business/metric_adapter/proposal_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/business/metric_adapter/votes_type.py
--rw-r--r--   0 runner    (1001) docker     (127)   418772 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/class_diagram.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.605815 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/data_access/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/data_access/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.605815 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.605815 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/metric_dao_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/srcs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.609815 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_active_members.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_active_organization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_active_voters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_approval_proposal_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_assets_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_assets_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_new_additions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_organization_activity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_proposal_outcome.py
--rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_proposal_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_total_members.py
--rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_voters_percentage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_votes_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_votes_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_votes_voters_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)     5274 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/platform_dao.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.609815 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/presentation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/presentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.609815 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/resources/strings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.609815 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.613814 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/business/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/business/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17742 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/business/app_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.613814 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/business/metric_adapter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/business/metric_adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/business/metric_adapter/asset_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/business/metric_adapter/asset_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/business/metric_adapter/majority_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/business/metric_adapter/metric_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/business/metric_adapter/proposal_boost_outcome.py
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/business/metric_adapter/success_ratio_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/business/metric_adapter/vote_type.py
--rw-r--r--   0 runner    (1001) docker     (127)   461806 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/class_diagram.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.613814 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/data_access/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/data_access/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.613814 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/data_access/daos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/data_access/daos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.613814 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6965 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/metric_dao_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/srcs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.617814 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_active_organization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_active_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_approval_proposal_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_assets_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_assets_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_different_voters_stakers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_organization_activity.py
--rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_proposal_majority.py
--rw-r--r--   0 runner    (1001) docker     (127)     9374 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_proposal_outcome.py
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_time_serie.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_total_reputation_holders.py
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_total_votes_stakes_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_voters_percentage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_votes_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_votes_voters_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/data_access/daos/platform_dao.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.617814 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/presentation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/presentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.617814 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/resources/strings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.625815 dao_analyzer-1.3.3.dev6/dao_analyzer/web/assets/
--rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/assets/ABOUT.md
--rw-r--r--   0 runner    (1001) docker     (127)    65944 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/assets/aragon.png
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/assets/callbacks.js
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/assets/cc-by.png
--rw-r--r--   0 runner    (1001) docker     (127)    18045 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/assets/dao-analyzer_header.svg
--rw-r--r--   0 runner    (1001) docker     (127)    36174 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/assets/dao-analyzer_logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)    54135 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/assets/daohaus.png
--rw-r--r--   0 runner    (1001) docker     (127)    16481 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/assets/daostack.png
--rw-r--r--   0 runner    (1001) docker     (127)   101409 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/assets/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)    58578 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/assets/github_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     4434 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/assets/ico-github.svg
--rw-r--r--   0 runner    (1001) docker     (127)    17972 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/assets/img_header.jpg
--rw-r--r--   0 runner    (1001) docker     (127)   129808 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/assets/kaggle_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/assets/logo-GPL.png
--rw-r--r--   0 runner    (1001) docker     (127)    10979 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/assets/logo-erc.png
--rw-r--r--   0 runner    (1001) docker     (127)     5475 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/assets/logo-grasia.png
--rw-r--r--   0 runner    (1001) docker     (127)    12180 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/assets/logo-ministerio.png
--rw-r--r--   0 runner    (1001) docker     (127)     7539 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/assets/logo-ucm.png
--rw-r--r--   0 runner    (1001) docker     (127)     5910 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/assets/logo_dao_analyzer.png
--rw-r--r--   0 runner    (1001) docker     (127)     5333 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/assets/logo_dao_analyzer.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/assets/logo_dao_analyzer_orig.svg
--rw-r--r--   0 runner    (1001) docker     (127)    10237 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/assets/stylesheet.css
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer/web/matomo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.641815 dao_analyzer-1.3.3.dev6/dao_analyzer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12201 2024-05-27 09:59:52.000000 dao_analyzer-1.3.3.dev6/dao_analyzer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18845 2024-05-27 09:59:52.000000 dao_analyzer-1.3.3.dev6/dao_analyzer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 09:59:52.000000 dao_analyzer-1.3.3.dev6/dao_analyzer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-27 09:59:52.000000 dao_analyzer-1.3.3.dev6/dao_analyzer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-27 09:59:52.000000 dao_analyzer-1.3.3.dev6/dao_analyzer.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-27 09:59:52.000000 dao_analyzer-1.3.3.dev6/dao_analyzer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-27 09:59:52.000000 dao_analyzer-1.3.3.dev6/dao_analyzer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.629814 dao_analyzer-1.3.3.dev6/dao_analyzer_components/
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer_components/.babelrc
--rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer_components/.eslintrc
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer_components/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer_components/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer_components/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer_components/_validate_init.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.629814 dao_analyzer-1.3.3.dev6/dao_analyzer_components/dao_analyzer_components/
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer_components/dao_analyzer_components/DAOInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer_components/dao_analyzer_components/DataPoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer_components/dao_analyzer_components/ParticipationStat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer_components/dao_analyzer_components/PlatformInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer_components/dao_analyzer_components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer_components/dao_analyzer_components/_imports_.py
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer_components/dao_analyzer_components/dao_analyzer_components.css
--rw-r--r--   0 runner    (1001) docker     (127)    13751 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer_components/dao_analyzer_components/dao_analyzer_components.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    18894 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer_components/dao_analyzer_components/dao_analyzer_components.min.js.map
--rw-r--r--   0 runner    (1001) docker     (127)     5984 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer_components/dao_analyzer_components/metadata.json
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer_components/dao_analyzer_components/package-info.json
--rw-r--r--   0 runner    (1001) docker     (127)   371186 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer_components/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer_components/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.629814 dao_analyzer-1.3.3.dev6/dao_analyzer_components/public/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer_components/public/index.html
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer_components/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer_components/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.573814 dao_analyzer-1.3.3.dev6/dao_analyzer_components/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.629814 dao_analyzer-1.3.3.dev6/dao_analyzer_components/src/demo/
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer_components/src/demo/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.629814 dao_analyzer-1.3.3.dev6/dao_analyzer_components/src/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.629814 dao_analyzer-1.3.3.dev6/dao_analyzer_components/src/lib/components/
--rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer_components/src/lib/components/DAOInfo.jsx
--rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer_components/src/lib/components/DataPoint.jsx
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer_components/src/lib/components/ParticipationStat.jsx
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer_components/src/lib/components/PlatformInfo.jsx
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer_components/src/lib/index.js
--rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer_components/webpack.config.js
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/dao_analyzer_components/webpack.demo.config.js
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/gunicorn_config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      197 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/init.sh
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.633814 dao_analyzer-1.3.3.dev6/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.633814 dao_analyzer-1.3.3.dev6/scripts/archive/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/scripts/archive/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)   339476 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/scripts/archive/names.ipynb
--rwxr-xr-x   0 runner    (1001) docker     (127)     1010 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/scripts/archive/uploadToKaggle.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     1790 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/scripts/checkContinue.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     4349 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/scripts/datawarehouseDiff.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      251 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/scripts/deploy.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      111 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/scripts/printArrow.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1148 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/scripts/updateAragonNames.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2900 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/scripts/uploadDataWarehouse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-05-27 09:59:52.645815 dao_analyzer-1.3.3.dev6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.633814 dao_analyzer-1.3.3.dev6/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.633814 dao_analyzer-1.3.3.dev6/test/mocks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/test/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/test/mocks/api_requester_mock.py
--rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/test/mocks/unix_date_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.633814 dao_analyzer-1.3.3.dev6/test/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/test/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.633814 dao_analyzer-1.3.3.dev6/test/unit/apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/test/unit/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.633814 dao_analyzer-1.3.3.dev6/test/unit/apps/aragon/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/test/unit/apps/aragon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.633814 dao_analyzer-1.3.3.dev6/test/unit/apps/aragon/data_access/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/test/unit/apps/aragon/data_access/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.633814 dao_analyzer-1.3.3.dev6/test/unit/apps/aragon/data_access/daos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/test/unit/apps/aragon/data_access/daos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.633814 dao_analyzer-1.3.3.dev6/test/unit/apps/aragon/data_access/daos/metric/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/test/unit/apps/aragon/data_access/daos/metric/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.633814 dao_analyzer-1.3.3.dev6/test/unit/apps/aragon/data_access/daos/metric/strategy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/test/unit/apps/aragon/data_access/daos/metric/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/test/unit/apps/aragon/data_access/daos/metric/strategy/test_aragon_st_new_additions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_active_organization_aragon.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_active_token_holders.py
--rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_cast_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_installed_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_vote_outcome.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.637814 dao_analyzer-1.3.3.dev6/test/unit/apps/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/test/unit/apps/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.637814 dao_analyzer-1.3.3.dev6/test/unit/apps/common/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/test/unit/apps/common/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.637814 dao_analyzer-1.3.3.dev6/test/unit/apps/common/api/graphql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/test/unit/apps/common/api/graphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/test/unit/apps/common/api/graphql/test_query_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.637814 dao_analyzer-1.3.3.dev6/test/unit/apps/common/business/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/test/unit/apps/common/business/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.637814 dao_analyzer-1.3.3.dev6/test/unit/apps/common/business/transfers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/test/unit/apps/common/business/transfers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/test/unit/apps/common/business/transfers/test_organization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.637814 dao_analyzer-1.3.3.dev6/test/unit/apps/common/data_access/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/test/unit/apps/common/data_access/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.637814 dao_analyzer-1.3.3.dev6/test/unit/apps/common/data_access/daos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/test/unit/apps/common/data_access/daos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.637814 dao_analyzer-1.3.3.dev6/test/unit/apps/daohaus/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/test/unit/apps/daohaus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.637814 dao_analyzer-1.3.3.dev6/test/unit/apps/daohaus/data_access/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/test/unit/apps/daohaus/data_access/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.637814 dao_analyzer-1.3.3.dev6/test/unit/apps/daohaus/data_access/daos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/test/unit/apps/daohaus/data_access/daos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.637814 dao_analyzer-1.3.3.dev6/test/unit/apps/daohaus/data_access/daos/metric/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/test/unit/apps/daohaus/data_access/daos/metric/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.637814 dao_analyzer-1.3.3.dev6/test/unit/apps/daohaus/data_access/daos/metric/strategy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/test/unit/apps/daohaus/data_access/daos/metric/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_active_members.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_active_organization_daohaus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_active_voters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_dproposal_outcome.py
--rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_new_additions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_proposal_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_total_members.py
--rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_votes_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.637814 dao_analyzer-1.3.3.dev6/test/unit/apps/daostack/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/test/unit/apps/daostack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.637814 dao_analyzer-1.3.3.dev6/test/unit/apps/daostack/data_access/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/test/unit/apps/daostack/data_access/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.637814 dao_analyzer-1.3.3.dev6/test/unit/apps/daostack/data_access/daos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/test/unit/apps/daostack/data_access/daos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.637814 dao_analyzer-1.3.3.dev6/test/unit/apps/daostack/data_access/daos/metric/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/test/unit/apps/daostack/data_access/daos/metric/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.641815 dao_analyzer-1.3.3.dev6/test/unit/apps/daostack/data_access/daos/metric/strategy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/test/unit/apps/daostack/data_access/daos/metric/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_active_organization_daostack.py
--rw-r--r--   0 runner    (1001) docker     (127)     3935 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_active_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_diff_voters_stakers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_proposal_majority.py
--rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_proposal_outcome.py
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_time_serie.py
--rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_voters_percentage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.641815 dao_analyzer-1.3.3.dev6/test/unit/apps/daostack/data_access/requesters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/test/unit/apps/daostack/data_access/requesters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:59:52.641815 dao_analyzer-1.3.3.dev6/test/unit/components/
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-27 09:59:42.000000 dao_analyzer-1.3.3.dev6/test/unit/components/test_dao_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.841345 dao_analyzer-1.3.3.dev7/
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/.envrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.781345 dao_analyzer-1.3.3.dev7/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.781345 dao_analyzer-1.3.3.dev7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     5782 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/.hintrc
+-rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/ABOUT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7713 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12201 2024-06-03 15:35:47.841345 dao_analyzer-1.3.3.dev7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9815 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.769345 dao_analyzer-1.3.3.dev7/dao_analyzer/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.785345 dao_analyzer-1.3.3.dev7/dao_analyzer/web/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-06-03 15:35:47.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.785345 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.785345 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.785345 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/business/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/business/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16209 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/business/app_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.789345 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/business/metric_adapter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/business/metric_adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/business/metric_adapter/asset_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/business/metric_adapter/asset_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/business/metric_adapter/basic_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/business/metric_adapter/cast_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/business/metric_adapter/installed_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/business/metric_adapter/vote_outcome.py
+-rw-r--r--   0 runner    (1001) docker     (127)   399465 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/class_diagram.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.789345 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/data_access/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/data_access/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.789345 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/data_access/daos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/data_access/daos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.789345 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6301 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/metric_dao_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/srcs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.793345 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_active_organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_active_token_holders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_active_voters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_approval_vote_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_assets_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_assets_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_cast_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_casted_votes_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_casted_votes_voters_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_installed_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_new_additions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_organization_activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_total_token_holders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_vote_outcome.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5890 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/data_access/daos/platform_dao.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.793345 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/presentation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/presentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.793345 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/resources/strings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.793345 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.793345 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.793345 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/api/graphql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/api/graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/api/graphql/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/api/graphql/query_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.793345 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/business/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/business/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/business/i_metric_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/business/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.793345 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/business/transfers/
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/business/transfers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/business/transfers/hierarchical_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/business/transfers/n_stacked_serie.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.797345 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/business/transfers/organization/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/business/transfers/organization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/business/transfers/organization/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/business/transfers/organization/organization_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5678 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/business/transfers/organization/organization_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/business/transfers/organization/participation_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/business/transfers/organization/platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/business/transfers/serie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/business/transfers/stacked_serie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/business/transfers/tabular_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.797345 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/data_access/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/data_access/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.797345 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/data_access/daos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/data_access/daos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.797345 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/data_access/daos/metric/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/data_access/daos/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/data_access/daos/metric/metric_dao.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/data_access/daos/metric/srcs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.797345 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/data_access/daos/metric/strategy/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/data_access/daos/metric/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/data_access/daos/metric/strategy/imetric_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/data_access/daos/metric/strategy/st_assets_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4554 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/data_access/daos/metric/strategy/st_assets_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/data_access/daos/platform_dao.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4369 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/data_access/pandas_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.797345 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/data_access/requesters/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/data_access/requesters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/data_access/requesters/cache_requester.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/data_access/requesters/irequester.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/data_access/requesters/join_cache_requester.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.797345 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/presentation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/presentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.797345 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/presentation/about_view/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/presentation/about_view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/presentation/about_view/about_view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.801345 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/presentation/charts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/presentation/charts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/presentation/charts/chart_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/presentation/charts/chart_sum_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/presentation/charts/dt_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.801345 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/chart_pane_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3711 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/chart_pane_layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/data_table_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/data_table_layout.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.801345 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/figure/
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/figure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/figure/bar_figure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/figure/calplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4723 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/figure/double_scatter_figure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/figure/figure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4532 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/figure/figure_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/figure/multi_bar_figure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/figure/treemap_figure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/ilayout.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/layout_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.801345 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/presentation/dashboard_view/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/presentation/dashboard_view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/presentation/dashboard_view/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9420 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/presentation/dashboard_view/dashboard_view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.805345 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/presentation/main_view/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/presentation/main_view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/presentation/main_view/main_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6670 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/presentation/main_view/main_view_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.805345 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/resources/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/resources/strings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.805345 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.805345 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/business/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/business/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16026 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/business/app_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.805345 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/business/metric_adapter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/business/metric_adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/business/metric_adapter/asset_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/business/metric_adapter/asset_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/business/metric_adapter/basic_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/business/metric_adapter/proposal_outcome.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/business/metric_adapter/proposal_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/business/metric_adapter/votes_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)   418772 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/class_diagram.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.805345 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/data_access/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/data_access/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.805345 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.809345 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/metric_dao_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/srcs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.809345 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_active_members.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_active_organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_active_voters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_approval_proposal_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_assets_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_assets_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_new_additions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_organization_activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_proposal_outcome.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_proposal_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_total_members.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_voters_percentage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_votes_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_votes_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_votes_voters_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5274 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/platform_dao.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.809345 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/presentation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/presentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.809345 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/resources/strings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.813345 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.813345 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/business/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/business/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17742 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/business/app_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.813345 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/business/metric_adapter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/business/metric_adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/business/metric_adapter/asset_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/business/metric_adapter/asset_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/business/metric_adapter/majority_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/business/metric_adapter/metric_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/business/metric_adapter/proposal_boost_outcome.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/business/metric_adapter/success_ratio_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/business/metric_adapter/vote_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)   461806 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/class_diagram.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.813345 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/data_access/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/data_access/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.813345 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/data_access/daos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/data_access/daos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.813345 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6965 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/metric_dao_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/srcs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.817345 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_active_organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_active_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_approval_proposal_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_assets_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_assets_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_different_voters_stakers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_organization_activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_proposal_majority.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9374 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_proposal_outcome.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_time_serie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_total_reputation_holders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_total_votes_stakes_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_voters_percentage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_votes_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_votes_voters_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/data_access/daos/platform_dao.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.817345 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/presentation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/presentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.817345 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/resources/strings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.825345 dao_analyzer-1.3.3.dev7/dao_analyzer/web/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/assets/ABOUT.md
+-rw-r--r--   0 runner    (1001) docker     (127)    65944 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/assets/aragon.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/assets/callbacks.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/assets/cc-by.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18045 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/assets/dao-analyzer_header.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    36174 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/assets/dao-analyzer_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    54135 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/assets/daohaus.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16481 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/assets/daostack.png
+-rw-r--r--   0 runner    (1001) docker     (127)   101409 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/assets/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    58578 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/assets/github_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4434 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/assets/ico-github.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    17972 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/assets/img_header.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)   129808 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/assets/kaggle_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/assets/logo-GPL.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10979 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/assets/logo-erc.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5475 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/assets/logo-grasia.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12180 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/assets/logo-ministerio.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7539 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/assets/logo-ucm.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5910 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/assets/logo_dao_analyzer.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5333 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/assets/logo_dao_analyzer.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/assets/logo_dao_analyzer_orig.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    10310 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/assets/stylesheet.css
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer/web/matomo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.841345 dao_analyzer-1.3.3.dev7/dao_analyzer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12201 2024-06-03 15:35:47.000000 dao_analyzer-1.3.3.dev7/dao_analyzer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18845 2024-06-03 15:35:47.000000 dao_analyzer-1.3.3.dev7/dao_analyzer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 15:35:47.000000 dao_analyzer-1.3.3.dev7/dao_analyzer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-06-03 15:35:47.000000 dao_analyzer-1.3.3.dev7/dao_analyzer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-06-03 15:35:47.000000 dao_analyzer-1.3.3.dev7/dao_analyzer.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-06-03 15:35:47.000000 dao_analyzer-1.3.3.dev7/dao_analyzer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-06-03 15:35:47.000000 dao_analyzer-1.3.3.dev7/dao_analyzer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.825345 dao_analyzer-1.3.3.dev7/dao_analyzer_components/
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer_components/.babelrc
+-rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer_components/.eslintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer_components/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer_components/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer_components/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer_components/_validate_init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.829345 dao_analyzer-1.3.3.dev7/dao_analyzer_components/dao_analyzer_components/
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-06-03 15:35:41.000000 dao_analyzer-1.3.3.dev7/dao_analyzer_components/dao_analyzer_components/DAOInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-06-03 15:35:41.000000 dao_analyzer-1.3.3.dev7/dao_analyzer_components/dao_analyzer_components/DataPoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-06-03 15:35:41.000000 dao_analyzer-1.3.3.dev7/dao_analyzer_components/dao_analyzer_components/ParticipationStat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-06-03 15:35:41.000000 dao_analyzer-1.3.3.dev7/dao_analyzer_components/dao_analyzer_components/PlatformInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-06-03 15:35:41.000000 dao_analyzer-1.3.3.dev7/dao_analyzer_components/dao_analyzer_components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-06-03 15:35:41.000000 dao_analyzer-1.3.3.dev7/dao_analyzer_components/dao_analyzer_components/_imports_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-06-03 15:35:41.000000 dao_analyzer-1.3.3.dev7/dao_analyzer_components/dao_analyzer_components/dao_analyzer_components.css
+-rw-r--r--   0 runner    (1001) docker     (127)    13751 2024-06-03 15:35:41.000000 dao_analyzer-1.3.3.dev7/dao_analyzer_components/dao_analyzer_components/dao_analyzer_components.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    18894 2024-06-03 15:35:41.000000 dao_analyzer-1.3.3.dev7/dao_analyzer_components/dao_analyzer_components/dao_analyzer_components.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     5984 2024-06-03 15:35:41.000000 dao_analyzer-1.3.3.dev7/dao_analyzer_components/dao_analyzer_components/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-06-03 15:35:41.000000 dao_analyzer-1.3.3.dev7/dao_analyzer_components/dao_analyzer_components/package-info.json
+-rw-r--r--   0 runner    (1001) docker     (127)   371186 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer_components/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer_components/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.829345 dao_analyzer-1.3.3.dev7/dao_analyzer_components/public/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer_components/public/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer_components/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer_components/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.773345 dao_analyzer-1.3.3.dev7/dao_analyzer_components/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.829345 dao_analyzer-1.3.3.dev7/dao_analyzer_components/src/demo/
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer_components/src/demo/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.829345 dao_analyzer-1.3.3.dev7/dao_analyzer_components/src/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.829345 dao_analyzer-1.3.3.dev7/dao_analyzer_components/src/lib/components/
+-rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer_components/src/lib/components/DAOInfo.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer_components/src/lib/components/DataPoint.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer_components/src/lib/components/ParticipationStat.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer_components/src/lib/components/PlatformInfo.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer_components/src/lib/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer_components/webpack.config.js
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/dao_analyzer_components/webpack.demo.config.js
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/gunicorn_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      197 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/init.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.829345 dao_analyzer-1.3.3.dev7/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.833345 dao_analyzer-1.3.3.dev7/scripts/archive/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/scripts/archive/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   339476 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/scripts/archive/names.ipynb
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1010 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/scripts/archive/uploadToKaggle.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1790 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/scripts/checkContinue.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4349 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/scripts/datawarehouseDiff.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      251 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/scripts/deploy.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      111 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/scripts/printArrow.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1148 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/scripts/updateAragonNames.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2900 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/scripts/uploadDataWarehouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-06-03 15:35:47.841345 dao_analyzer-1.3.3.dev7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.833345 dao_analyzer-1.3.3.dev7/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.833345 dao_analyzer-1.3.3.dev7/test/mocks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/test/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/test/mocks/api_requester_mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/test/mocks/unix_date_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.833345 dao_analyzer-1.3.3.dev7/test/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/test/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.833345 dao_analyzer-1.3.3.dev7/test/unit/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/test/unit/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.833345 dao_analyzer-1.3.3.dev7/test/unit/apps/aragon/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/test/unit/apps/aragon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.833345 dao_analyzer-1.3.3.dev7/test/unit/apps/aragon/data_access/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/test/unit/apps/aragon/data_access/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.833345 dao_analyzer-1.3.3.dev7/test/unit/apps/aragon/data_access/daos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/test/unit/apps/aragon/data_access/daos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.833345 dao_analyzer-1.3.3.dev7/test/unit/apps/aragon/data_access/daos/metric/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/test/unit/apps/aragon/data_access/daos/metric/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.833345 dao_analyzer-1.3.3.dev7/test/unit/apps/aragon/data_access/daos/metric/strategy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/test/unit/apps/aragon/data_access/daos/metric/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/test/unit/apps/aragon/data_access/daos/metric/strategy/test_aragon_st_new_additions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_active_organization_aragon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_active_token_holders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_cast_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_installed_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_vote_outcome.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.833345 dao_analyzer-1.3.3.dev7/test/unit/apps/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/test/unit/apps/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.833345 dao_analyzer-1.3.3.dev7/test/unit/apps/common/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/test/unit/apps/common/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.833345 dao_analyzer-1.3.3.dev7/test/unit/apps/common/api/graphql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/test/unit/apps/common/api/graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/test/unit/apps/common/api/graphql/test_query_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.833345 dao_analyzer-1.3.3.dev7/test/unit/apps/common/business/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/test/unit/apps/common/business/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.837345 dao_analyzer-1.3.3.dev7/test/unit/apps/common/business/transfers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/test/unit/apps/common/business/transfers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/test/unit/apps/common/business/transfers/test_organization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.837345 dao_analyzer-1.3.3.dev7/test/unit/apps/common/data_access/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/test/unit/apps/common/data_access/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.837345 dao_analyzer-1.3.3.dev7/test/unit/apps/common/data_access/daos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/test/unit/apps/common/data_access/daos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.837345 dao_analyzer-1.3.3.dev7/test/unit/apps/daohaus/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/test/unit/apps/daohaus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.837345 dao_analyzer-1.3.3.dev7/test/unit/apps/daohaus/data_access/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/test/unit/apps/daohaus/data_access/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.837345 dao_analyzer-1.3.3.dev7/test/unit/apps/daohaus/data_access/daos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/test/unit/apps/daohaus/data_access/daos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.837345 dao_analyzer-1.3.3.dev7/test/unit/apps/daohaus/data_access/daos/metric/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/test/unit/apps/daohaus/data_access/daos/metric/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.837345 dao_analyzer-1.3.3.dev7/test/unit/apps/daohaus/data_access/daos/metric/strategy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/test/unit/apps/daohaus/data_access/daos/metric/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_active_members.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_active_organization_daohaus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_active_voters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_dproposal_outcome.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_new_additions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_proposal_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_total_members.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_votes_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.837345 dao_analyzer-1.3.3.dev7/test/unit/apps/daostack/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/test/unit/apps/daostack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.837345 dao_analyzer-1.3.3.dev7/test/unit/apps/daostack/data_access/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/test/unit/apps/daostack/data_access/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.837345 dao_analyzer-1.3.3.dev7/test/unit/apps/daostack/data_access/daos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/test/unit/apps/daostack/data_access/daos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.837345 dao_analyzer-1.3.3.dev7/test/unit/apps/daostack/data_access/daos/metric/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/test/unit/apps/daostack/data_access/daos/metric/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.841345 dao_analyzer-1.3.3.dev7/test/unit/apps/daostack/data_access/daos/metric/strategy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/test/unit/apps/daostack/data_access/daos/metric/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_active_organization_daostack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3935 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_active_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_diff_voters_stakers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_proposal_majority.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_proposal_outcome.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_time_serie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_voters_percentage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.841345 dao_analyzer-1.3.3.dev7/test/unit/apps/daostack/data_access/requesters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/test/unit/apps/daostack/data_access/requesters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:35:47.841345 dao_analyzer-1.3.3.dev7/test/unit/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-06-03 15:35:40.000000 dao_analyzer-1.3.3.dev7/test/unit/components/test_dao_info.py
```

### Comparing `dao_analyzer-1.3.3.dev6/.github/dependabot.yml` & `dao_analyzer-1.3.3.dev7/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/.github/workflows/ci.yml` & `dao_analyzer-1.3.3.dev7/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/.gitignore` & `dao_analyzer-1.3.3.dev7/.gitignore`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/ABOUT.md` & `dao_analyzer-1.3.3.dev7/ABOUT.md`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/CHANGELOG.md` & `dao_analyzer-1.3.3.dev7/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
+# 1.3.3 - 2024-06-03
+- Updated dao-scripts to 1.4.6
+- Changed some network names
+- Updated dependencies
+
 # 1.3.1 - 2024-05-27
 - Updated dao-scripts to 1.3.1
 
 # 1.3.0 - 2024-05-27
 - Updated dao-scripts to 1.3.0, now The Graph API key is needed to download data
 - Updated dependencies
 - Added Python 3.12 support
```

### Comparing `dao_analyzer-1.3.3.dev6/CITATION.cff` & `dao_analyzer-1.3.3.dev7/CITATION.cff`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/Dockerfile` & `dao_analyzer-1.3.3.dev7/Dockerfile`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/LICENSE` & `dao_analyzer-1.3.3.dev7/LICENSE`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/PKG-INFO` & `dao_analyzer-1.3.3.dev7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dao-analyzer
-Version: 1.3.3.dev6
+Version: 1.3.3.dev7
 Summary: "A tool to monitor DAO activity"
 Home-page: https://dao-analyzer.science
 Author: David Davó
 Author-email: ddavo@ucm.es
 Project-URL: Source, https://github.com/Grasia/dao-analyzer
 Project-URL: Bug Tracker, https://github.com/Grasia/dao-analyzer/issues
 Project-URL: Changelog, https://github.com/Grasia/dao-analyzer/blob/master/CHANGELOG.md
@@ -22,15 +22,15 @@
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Sociology
 Classifier: Typing :: Typed
 Classifier: Topic :: Utilities
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: dao-scripts==1.3.1
+Requires-Dist: dao-scripts==1.4.6
 Requires-Dist: dash>=2.17.0
 Requires-Dist: dash-bootstrap-components>=1.1.0
 Requires-Dist: Werkzeug<2.1.0
 Requires-Dist: flask>=2.0.2
 Requires-Dist: gql>=3.0.0a1
 Requires-Dist: millify>=0.1.1
 Requires-Dist: numpy>=1.17.3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dao-analyzer Version: 1.3.3.dev6 Summary: "A tool
+Metadata-Version: 2.1 Name: dao-analyzer Version: 1.3.3.dev7 Summary: "A tool
 to monitor DAO activity" Home-page: https://dao-analyzer.science Author: David
 DavÃ³ Author-email: ddavo@ucm.es Project-URL: Source, https://github.com/
 Grasia/dao-analyzer Project-URL: Bug Tracker, https://github.com/Grasia/dao-
 analyzer/issues Project-URL: Changelog, https://github.com/Grasia/dao-analyzer/
 blob/master/CHANGELOG.md Classifier: Development Status :: 5 - Production/
 Stable Classifier: Environment :: Console Classifier: Environment :: Web
 Environment Classifier: Framework :: Dash Classifier: Intended Audience ::
@@ -10,15 +10,15 @@
 License v3 (GPLv3) Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Classifier: Topic :: Scientific/
 Engineering :: Visualization Classifier: Topic :: Sociology Classifier: Typing
 :: Typed Classifier: Topic :: Utilities Requires-Python: >=3.9 Description-
 Content-Type: text/markdown License-File: LICENSE Requires-Dist: dao-
-scripts==1.3.1 Requires-Dist: dash>=2.17.0 Requires-Dist: dash-bootstrap-
+scripts==1.4.6 Requires-Dist: dash>=2.17.0 Requires-Dist: dash-bootstrap-
 components>=1.1.0 Requires-Dist: Werkzeug<2.1.0 Requires-Dist: flask>=2.0.2
 Requires-Dist: gql>=3.0.0a1 Requires-Dist: millify>=0.1.1 Requires-Dist:
 numpy>=1.17.3 Requires-Dist: pandas>=1.3.4 Requires-Dist: portalocker>=2.3.2
 Requires-Dist: pyarrow>=6.0.0 Requires-Dist: requests>=2.26.0 Requires-Dist:
 requests-cache>=0.8.1 Requires-Dist: requests-toolbelt>=0.9.1 Requires-Dist:
 tenacity>=8.0.0 Requires-Dist: tqdm>=4.62.3 Requires-Dist: plotly-
 calplot==0.1.13 Provides-Extra: docker Requires-Dist: gunicorn>=20.1.0; extra
```

### Comparing `dao_analyzer-1.3.3.dev6/README.md` & `dao_analyzer-1.3.3.dev7/README.md`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/app.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/app.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/business/app_service.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/business/app_service.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/business/metric_adapter/asset_tokens.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/business/metric_adapter/asset_tokens.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/business/metric_adapter/asset_values.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/business/metric_adapter/asset_values.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/business/metric_adapter/basic_adapter.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/business/metric_adapter/basic_adapter.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/business/metric_adapter/cast_type.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/business/metric_adapter/cast_type.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/business/metric_adapter/installed_apps.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/business/metric_adapter/installed_apps.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/business/metric_adapter/vote_outcome.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/business/metric_adapter/vote_outcome.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/class_diagram.png` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/class_diagram.png`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/metric_dao_factory.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/metric_dao_factory.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/srcs.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/srcs.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_active_organization.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_active_organization.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_active_token_holders.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_active_token_holders.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_active_voters.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_active_voters.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_approval_vote_rate.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_approval_vote_rate.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_cast_type.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_cast_type.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_casted_votes_rate.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_casted_votes_rate.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_casted_votes_voters_rate.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_casted_votes_voters_rate.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_installed_apps.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_installed_apps.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_new_additions.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_new_additions.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_organization_activity.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_organization_activity.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_total_token_holders.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_total_token_holders.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_vote_outcome.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_vote_outcome.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/data_access/daos/platform_dao.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/data_access/daos/platform_dao.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/aragon/resources/strings.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/aragon/resources/strings.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/api/graphql/query.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/api/graphql/query.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/api/graphql/query_builder.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/api/graphql/query_builder.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/business/i_metric_adapter.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/business/i_metric_adapter.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/business/singleton.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/business/singleton.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/business/transfers/hierarchical_data.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/business/transfers/hierarchical_data.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/business/transfers/n_stacked_serie.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/business/transfers/n_stacked_serie.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/business/transfers/organization/organization.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/business/transfers/organization/organization.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/business/transfers/organization/organization_filter.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/business/transfers/organization/organization_filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 import abc
 from typing import List, Callable, Iterable, Dict, Union
 from datetime import datetime, timedelta
 
 from dao_analyzer.web.apps.common.business.transfers.organization.organization import Organization
 
-from dao_analyzer.web.apps.common.resources.strings import TEXT
+from dao_analyzer.web.apps.common.resources.strings import TEXT, NETWORKS
 
 class Filter(metaclass=abc.ABCMeta):
 
     def pred(self, org: Organization) -> bool:
         raise NotImplementedError
 
 class OrganizationFilter(Filter, metaclass=abc.ABCMeta):
@@ -122,15 +122,15 @@
     def __init__(self, a: Union[NetworkFilters, List[str]], network_value: str = ALL_NETWORKS_VALUE):
         self._options = ALL_NETWORKS_DICT()
         self._value = network_value or ALL_NETWORKS_VALUE
 
         if isinstance(a, NetworkFilters):
             self._options = a.get_options()
         else:
-            self._options = { n:n.capitalize() for n in a }
+            self._options = { n:NETWORKS.get(n, n.capitalize()) for n in a }
 
         if len(self._options) > 1:
             self._options = ALL_NETWORKS_DICT() | dict(sorted(self._options.items(), key=self.sorted_key))
         else:
             # We show the network name, but with the ALL_NETWORKS_VALUE key
             name = next(iter(self._options.values()))
             self._options = { ALL_NETWORKS_VALUE:name }
```

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/business/transfers/organization/organization_list.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/business/transfers/organization/organization_list.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/business/transfers/organization/participation_stats.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/business/transfers/organization/participation_stats.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/business/transfers/organization/platform.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/business/transfers/organization/platform.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/business/transfers/serie.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/business/transfers/serie.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/business/transfers/stacked_serie.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/business/transfers/stacked_serie.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/business/transfers/tabular_data.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/business/transfers/tabular_data.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/data_access/daos/metric/metric_dao.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/data_access/daos/metric/metric_dao.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/data_access/daos/metric/strategy/imetric_strategy.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/data_access/daos/metric/strategy/imetric_strategy.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/data_access/daos/metric/strategy/st_assets_tokens.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/data_access/daos/metric/strategy/st_assets_tokens.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/data_access/daos/metric/strategy/st_assets_values.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/data_access/daos/metric/strategy/st_assets_values.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/data_access/daos/platform_dao.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/data_access/daos/platform_dao.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/data_access/pandas_utils.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/data_access/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/data_access/requesters/cache_requester.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/data_access/requesters/cache_requester.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/data_access/requesters/irequester.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/data_access/requesters/irequester.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/data_access/requesters/join_cache_requester.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/data_access/requesters/join_cache_requester.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/presentation/about_view/about_view.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/presentation/about_view/about_view.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/presentation/charts/chart_controller.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/presentation/charts/chart_controller.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/presentation/charts/chart_sum_controller.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/presentation/charts/chart_sum_controller.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/presentation/charts/dt_controller.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/presentation/charts/dt_controller.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/presentation/charts/layout/chart_pane_configuration.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/chart_pane_configuration.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/presentation/charts/layout/chart_pane_layout.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/chart_pane_layout.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/presentation/charts/layout/data_table_layout.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/data_table_layout.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/presentation/charts/layout/figure/bar_figure.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/figure/bar_figure.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/presentation/charts/layout/figure/calplot.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/figure/calplot.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/presentation/charts/layout/figure/double_scatter_figure.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/figure/double_scatter_figure.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/presentation/charts/layout/figure/figure.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/figure/figure.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/presentation/charts/layout/figure/figure_configuration.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/figure/figure_configuration.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/presentation/charts/layout/figure/multi_bar_figure.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/figure/multi_bar_figure.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/presentation/charts/layout/figure/treemap_figure.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/figure/treemap_figure.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/presentation/charts/layout/layout_configuration.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/layout_configuration.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/presentation/dashboard_view/controller.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/presentation/dashboard_view/controller.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/presentation/dashboard_view/dashboard_view.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/presentation/dashboard_view/dashboard_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from dao_analyzer.web.apps.common.business.transfers.organization import Organization, OrganizationList
 from dao_analyzer.web.apps.common.business.transfers.organization.organization_filter import NetworkRadioButton, OrganizationFilterGroup
 from dao_analyzer.web.apps.common.business.transfers.organization.participation_stats import ParticipationStat
 from dao_analyzer.web.apps.common.business.transfers.organization.platform import Platform
 
 from dao_analyzer.web.apps.common.resources import colors as COLOR
-from dao_analyzer.web.apps.common.resources.strings import TEXT
+from dao_analyzer.web.apps.common.resources.strings import TEXT, NETWORKS
 from dao_analyzer.web.apps.common.presentation.main_view.main_view import REL_PATH
 
 __ECOSYSTEM_SELECTED: Dict[str, List[str]] = {
     'default': ['', '', ''],
     'daohaus': ['daohaus-selected', '', ''],
     'aragon': ['', 'aragon-selected', ''],
     'daostack': ['', '', 'daostack-selected'],
@@ -116,15 +116,15 @@
                 html.Div(html.Span(TEXT['network_selector_title'])),
                 dcc.RadioItems(
                     options = networkRadio.get_options(),
                     value = networkRadio.get_value(),
                     className = 'checklist-filter',
                     id='org-network-radio'),
             ], className='header-selector-wrapper'),
-        className='col-3 d-flex justify-content-center'),
+        className='col-4 d-flex justify-content-center'),
         # 3. DAO selector (and filtering)
         html.Div(
             html.Div(children=[
                 html.Div(TEXT['dao_selector_title']),
                 html.Div([
                     dcc.Checklist(
                         options = filterGroup.get_options(),
@@ -170,23 +170,23 @@
 
 def _get_platform_info(p: Platform) -> dac.PlatformInfo:
     if p is None:
         return html.Div(TEXT['no_data_selected'], className='dao-info-name')
 
     return dac.PlatformInfo(
         name=p.name,
-        networks=p.networks,
+        networks=[ NETWORKS[n] for n in p.networks ],
         creation_date=_aux_crdatetime(p.creation_date),
         participation_stats=_gen_participation_stats(p.participation_stats)
     )
 
 def _get_dao_info(org: Organization) -> dac.DAOInfo:
     return dac.DAOInfo(
         name=org.get_name(), 
-        network=org.get_network(),
+        network=NETWORKS[org.get_network()],
         address=org.get_id(),
         creation_date=_aux_crdatetime(org.get_creation_date()),
         first_activity=_aux_crdatetime(org.get_first_activity()),
         participation_stats=_gen_participation_stats(org.get_participation_stats()),
     )
 
 def _gen_sum_hdr(org: Organization = None):
```

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/presentation/main_view/main_view.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/presentation/main_view/main_view.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/presentation/main_view/main_view_controller.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/presentation/main_view/main_view_controller.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/resources/colors.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/resources/colors.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/common/resources/strings.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/common/resources/strings.py`

 * *Files 17% similar despite different names*

```diff
@@ -76,7 +76,17 @@
     # 'unknown_dao_name': '———', # Em dash
     'unknown_dao_name': 'no name given',
     'url_about': 'about',
     'url_aragon': 'aragon',
     'url_daostack': 'daostack',
     'url_daohaus': 'daohaus',
 }
+
+NETWORKS: dict[str, str] = {
+    '__all_networks': TEXT['radio_button_all_networks'],
+    'arbitrum': 'Arbitrum One',
+    'arbitrum-one': 'Arbitrum One',
+    'xdai': 'Gnosis (xdai)',
+    'mainnet': 'Ethereum Mainnet',
+    'matic': 'Matic (polygon)',
+    'polygon': 'Polygon (matic)',
+}
```

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/business/app_service.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/business/app_service.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/business/metric_adapter/asset_tokens.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/business/metric_adapter/asset_tokens.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/business/metric_adapter/asset_values.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/business/metric_adapter/asset_values.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/business/metric_adapter/basic_adapter.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/business/metric_adapter/basic_adapter.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/business/metric_adapter/proposal_outcome.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/business/metric_adapter/proposal_outcome.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/business/metric_adapter/proposal_type.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/business/metric_adapter/proposal_type.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/business/metric_adapter/votes_type.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/business/metric_adapter/votes_type.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/class_diagram.png` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/class_diagram.png`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/metric_dao_factory.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/metric_dao_factory.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/srcs.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/srcs.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_active_members.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_active_members.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_active_organization.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_active_organization.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_active_voters.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_active_voters.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_approval_proposal_rate.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_approval_proposal_rate.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_new_additions.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_new_additions.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_organization_activity.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_organization_activity.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_proposal_outcome.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_proposal_outcome.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_proposal_type.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_proposal_type.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_total_members.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_total_members.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_voters_percentage.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_voters_percentage.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_votes_rate.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_votes_rate.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_votes_type.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_votes_type.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_votes_voters_rate.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_votes_voters_rate.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/platform_dao.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/platform_dao.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daohaus/resources/strings.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daohaus/resources/strings.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/business/app_service.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/business/app_service.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/business/metric_adapter/asset_tokens.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/business/metric_adapter/asset_tokens.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/business/metric_adapter/asset_values.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/business/metric_adapter/asset_values.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/business/metric_adapter/majority_type.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/business/metric_adapter/majority_type.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/business/metric_adapter/metric_adapter.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/business/metric_adapter/metric_adapter.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/business/metric_adapter/proposal_boost_outcome.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/business/metric_adapter/proposal_boost_outcome.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/business/metric_adapter/success_ratio_type.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/business/metric_adapter/success_ratio_type.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/business/metric_adapter/vote_type.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/business/metric_adapter/vote_type.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/class_diagram.png` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/class_diagram.png`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/metric_dao_factory.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/metric_dao_factory.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/srcs.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/srcs.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_active_organization.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_active_organization.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_active_users.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_active_users.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_approval_proposal_rate.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_approval_proposal_rate.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_different_voters_stakers.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_different_voters_stakers.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_organization_activity.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_organization_activity.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_proposal_majority.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_proposal_majority.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_proposal_outcome.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_proposal_outcome.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_time_serie.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_time_serie.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_total_reputation_holders.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_total_reputation_holders.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_total_votes_stakes_option.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_total_votes_stakes_option.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_voters_percentage.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_voters_percentage.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_votes_rate.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_votes_rate.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_votes_voters_rate.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_votes_voters_rate.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/data_access/daos/platform_dao.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/data_access/daos/platform_dao.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/apps/daostack/resources/strings.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/apps/daostack/resources/strings.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/assets/ABOUT.md` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/assets/ABOUT.md`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/assets/aragon.png` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/assets/aragon.png`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/assets/callbacks.js` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/assets/callbacks.js`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/assets/cc-by.png` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/assets/cc-by.png`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/assets/dao-analyzer_header.svg` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/assets/dao-analyzer_header.svg`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/assets/dao-analyzer_logo.svg` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/assets/dao-analyzer_logo.svg`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/assets/daohaus.png` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/assets/daohaus.png`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/assets/daostack.png` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/assets/daostack.png`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/assets/favicon.ico` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/assets/github_logo.png` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/assets/github_logo.png`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/assets/ico-github.svg` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/assets/ico-github.svg`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/assets/img_header.jpg` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/assets/img_header.jpg`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/assets/kaggle_logo.png` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/assets/kaggle_logo.png`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/assets/logo-GPL.png` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/assets/logo-GPL.png`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/assets/logo-erc.png` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/assets/logo-erc.png`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/assets/logo-grasia.png` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/assets/logo-grasia.png`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/assets/logo-ministerio.png` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/assets/logo-ministerio.png`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/assets/logo-ucm.png` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/assets/logo-ucm.png`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/assets/logo_dao_analyzer.png` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/assets/logo_dao_analyzer.png`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/assets/logo_dao_analyzer.svg` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/assets/logo_dao_analyzer.svg`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/assets/logo_dao_analyzer_orig.svg` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/assets/logo_dao_analyzer_orig.svg`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/assets/stylesheet.css` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/assets/stylesheet.css`

 * *Files 1% similar despite different names*

```diff
@@ -161,15 +161,15 @@
     padding-top: var(--body-header-internal-padding);
     padding-bottom: var(--body-header-internal-padding);
 }
 
 #org-network-radio {
     display: grid;
     grid-auto-flow: column;
-    column-gap: 2em;
+    column-gap: 1em;
     grid-template-rows: repeat(3, 1fr);
 }
 
 #org-network-radio label:first-child {
     grid-column-start: 1;
     grid-column-end: 3;
 }
@@ -422,14 +422,18 @@
     display: none;
 }
 
 .is-all-orgs .only-on-all-orgs {
     display: block;
 }
 
+input[type="radio"], input[type="checkbox"] {
+    margin-right: .7em;
+}
+
 /*********************/
 /*********************/
 
 /*********************/
 /*      FOOT         */
 
 footer {
```

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/logs.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/logs.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer/web/matomo.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer/web/matomo.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer.egg-info/PKG-INFO` & `dao_analyzer-1.3.3.dev7/dao_analyzer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dao-analyzer
-Version: 1.3.3.dev6
+Version: 1.3.3.dev7
 Summary: "A tool to monitor DAO activity"
 Home-page: https://dao-analyzer.science
 Author: David Davó
 Author-email: ddavo@ucm.es
 Project-URL: Source, https://github.com/Grasia/dao-analyzer
 Project-URL: Bug Tracker, https://github.com/Grasia/dao-analyzer/issues
 Project-URL: Changelog, https://github.com/Grasia/dao-analyzer/blob/master/CHANGELOG.md
@@ -22,15 +22,15 @@
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Sociology
 Classifier: Typing :: Typed
 Classifier: Topic :: Utilities
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: dao-scripts==1.3.1
+Requires-Dist: dao-scripts==1.4.6
 Requires-Dist: dash>=2.17.0
 Requires-Dist: dash-bootstrap-components>=1.1.0
 Requires-Dist: Werkzeug<2.1.0
 Requires-Dist: flask>=2.0.2
 Requires-Dist: gql>=3.0.0a1
 Requires-Dist: millify>=0.1.1
 Requires-Dist: numpy>=1.17.3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dao-analyzer Version: 1.3.3.dev6 Summary: "A tool
+Metadata-Version: 2.1 Name: dao-analyzer Version: 1.3.3.dev7 Summary: "A tool
 to monitor DAO activity" Home-page: https://dao-analyzer.science Author: David
 DavÃ³ Author-email: ddavo@ucm.es Project-URL: Source, https://github.com/
 Grasia/dao-analyzer Project-URL: Bug Tracker, https://github.com/Grasia/dao-
 analyzer/issues Project-URL: Changelog, https://github.com/Grasia/dao-analyzer/
 blob/master/CHANGELOG.md Classifier: Development Status :: 5 - Production/
 Stable Classifier: Environment :: Console Classifier: Environment :: Web
 Environment Classifier: Framework :: Dash Classifier: Intended Audience ::
@@ -10,15 +10,15 @@
 License v3 (GPLv3) Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Classifier: Topic :: Scientific/
 Engineering :: Visualization Classifier: Topic :: Sociology Classifier: Typing
 :: Typed Classifier: Topic :: Utilities Requires-Python: >=3.9 Description-
 Content-Type: text/markdown License-File: LICENSE Requires-Dist: dao-
-scripts==1.3.1 Requires-Dist: dash>=2.17.0 Requires-Dist: dash-bootstrap-
+scripts==1.4.6 Requires-Dist: dash>=2.17.0 Requires-Dist: dash-bootstrap-
 components>=1.1.0 Requires-Dist: Werkzeug<2.1.0 Requires-Dist: flask>=2.0.2
 Requires-Dist: gql>=3.0.0a1 Requires-Dist: millify>=0.1.1 Requires-Dist:
 numpy>=1.17.3 Requires-Dist: pandas>=1.3.4 Requires-Dist: portalocker>=2.3.2
 Requires-Dist: pyarrow>=6.0.0 Requires-Dist: requests>=2.26.0 Requires-Dist:
 requests-cache>=0.8.1 Requires-Dist: requests-toolbelt>=0.9.1 Requires-Dist:
 tenacity>=8.0.0 Requires-Dist: tqdm>=4.62.3 Requires-Dist: plotly-
 calplot==0.1.13 Provides-Extra: docker Requires-Dist: gunicorn>=20.1.0; extra
```

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer.egg-info/SOURCES.txt` & `dao_analyzer-1.3.3.dev7/dao_analyzer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer_components/.eslintrc` & `dao_analyzer-1.3.3.dev7/dao_analyzer_components/.eslintrc`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer_components/MANIFEST.in` & `dao_analyzer-1.3.3.dev7/dao_analyzer_components/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer_components/_validate_init.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer_components/_validate_init.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer_components/dao_analyzer_components/DAOInfo.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer_components/dao_analyzer_components/DAOInfo.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer_components/dao_analyzer_components/DataPoint.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer_components/dao_analyzer_components/DataPoint.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer_components/dao_analyzer_components/ParticipationStat.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer_components/dao_analyzer_components/ParticipationStat.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer_components/dao_analyzer_components/PlatformInfo.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer_components/dao_analyzer_components/PlatformInfo.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer_components/dao_analyzer_components/__init__.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer_components/dao_analyzer_components/__init__.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer_components/dao_analyzer_components/dao_analyzer_components.css` & `dao_analyzer-1.3.3.dev7/dao_analyzer_components/dao_analyzer_components/dao_analyzer_components.css`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer_components/dao_analyzer_components/dao_analyzer_components.min.js` & `dao_analyzer-1.3.3.dev7/dao_analyzer_components/dao_analyzer_components/dao_analyzer_components.min.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -42,15 +42,15 @@
             var e = function(t) {
                     return /\/_dash-component-suites\//.test(t.src)
                 }(r()),
                 o = n(t);
             if (!e) return o;
             var i = o.split("/"),
                 a = i.slice(-1)[0].split(".");
-            return a.splice(1, 0, "v0_0_23m1716803437"), i.splice(-1, 1, a.join(".")), i.join("/")
+            return a.splice(1, 0, "v0_0_23m1717428377"), i.splice(-1, 1, a.join(".")), i.join("/")
         }
     }
     var o = {};
     e.r(o), e.d(o, {
         DAOInfo: () => E,
         DataPoint: () => z,
         ParticipationStat: () => b,
```

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer_components/dao_analyzer_components/dao_analyzer_components.min.js.map` & `dao_analyzer-1.3.3.dev7/dao_analyzer_components/dao_analyzer_components/dao_analyzer_components.min.js.map`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.989010989010989%*

 * *Differences: {"'sourcesContent'": "{insert: [(1, 'var getCurrentScript = function() {\\n    var script = "*

 * *                     'document.currentScript;\\n    if (!script) {\\n        /* Shim for IE11 and '*

 * *                     'below */\\n        /* Do not take into account async scripts and inline '*

 * *                     'scripts */\\n\\n        var doc_scripts = '*

 * *                     "document.getElementsByTagName(\\'script\\');\\n        var scripts = "*

 * *                     '[];\\n\\n        for (var i = 0; i < doc_ […]*

```diff
@@ -116,15 +116,15 @@
         "webpack:///./src/lib/components/ParticipationStat.jsx",
         "webpack:///./src/lib/components/DAOInfo.jsx",
         "webpack:///./src/lib/components/PlatformInfo.jsx",
         "webpack:///./src/lib/components/DataPoint.jsx"
     ],
     "sourcesContent": [
         "// The require scope\nvar __webpack_require__ = {};\n\n",
-        "var getCurrentScript = function() {\n    var script = document.currentScript;\n    if (!script) {\n        /* Shim for IE11 and below */\n        /* Do not take into account async scripts and inline scripts */\n\n        var doc_scripts = document.getElementsByTagName('script');\n        var scripts = [];\n\n        for (var i = 0; i < doc_scripts.length; i++) {\n            scripts.push(doc_scripts[i]);\n        }\n\n        scripts = scripts.filter(function(s) { return !s.async && !s.text && !s.textContent; });\n        script = scripts.slice(-1)[0];\n    }\n\n    return script;\n};\n\nvar isLocalScript = function(script) {\n    return /\\/_dash-component-suites\\//.test(script.src);\n};\n\nObject.defineProperty(__webpack_require__, 'p', {\n    get: (function () {\n        var script = getCurrentScript();\n\n        var url = script.src.split('/').slice(0, -1).join('/') + '/';\n\n        return function() {\n            return url;\n        };\n    })()\n});\n\nif (typeof jsonpScriptSrc !== 'undefined') {\n    var __jsonpScriptSrc__ = jsonpScriptSrc;\n    jsonpScriptSrc = function(chunkId) {\n        var script = getCurrentScript();\n        var isLocal = isLocalScript(script);\n\n        var src = __jsonpScriptSrc__(chunkId);\n\n        if(!isLocal) {\n            return src;\n        }\n\n        var srcFragments = src.split('/');\n        var fileFragments = srcFragments.slice(-1)[0].split('.');\n\n        fileFragments.splice(1, 0, \"v0_0_23m1716803437\");\n        srcFragments.splice(-1, 1, fileFragments.join('.'))\n\n        return srcFragments.join('/');\n    };\n}\n",
+        "var getCurrentScript = function() {\n    var script = document.currentScript;\n    if (!script) {\n        /* Shim for IE11 and below */\n        /* Do not take into account async scripts and inline scripts */\n\n        var doc_scripts = document.getElementsByTagName('script');\n        var scripts = [];\n\n        for (var i = 0; i < doc_scripts.length; i++) {\n            scripts.push(doc_scripts[i]);\n        }\n\n        scripts = scripts.filter(function(s) { return !s.async && !s.text && !s.textContent; });\n        script = scripts.slice(-1)[0];\n    }\n\n    return script;\n};\n\nvar isLocalScript = function(script) {\n    return /\\/_dash-component-suites\\//.test(script.src);\n};\n\nObject.defineProperty(__webpack_require__, 'p', {\n    get: (function () {\n        var script = getCurrentScript();\n\n        var url = script.src.split('/').slice(0, -1).join('/') + '/';\n\n        return function() {\n            return url;\n        };\n    })()\n});\n\nif (typeof jsonpScriptSrc !== 'undefined') {\n    var __jsonpScriptSrc__ = jsonpScriptSrc;\n    jsonpScriptSrc = function(chunkId) {\n        var script = getCurrentScript();\n        var isLocal = isLocalScript(script);\n\n        var src = __jsonpScriptSrc__(chunkId);\n\n        if(!isLocal) {\n            return src;\n        }\n\n        var srcFragments = src.split('/');\n        var fileFragments = srcFragments.slice(-1)[0].split('.');\n\n        fileFragments.splice(1, 0, \"v0_0_23m1717428377\");\n        srcFragments.splice(-1, 1, fileFragments.join('.'))\n\n        return srcFragments.join('/');\n    };\n}\n",
         "// getDefaultExport function for compatibility with non-harmony modules\n__webpack_require__.n = (module) => {\n\tvar getter = module && module.__esModule ?\n\t\t() => (module['default']) :\n\t\t() => (module);\n\t__webpack_require__.d(getter, { a: getter });\n\treturn getter;\n};",
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
         "const __WEBPACK_NAMESPACE_OBJECT__ = window[\"React\"];",
         "const __WEBPACK_NAMESPACE_OBJECT__ = window[\"PropTypes\"];",
         "import React, { Component } from 'react';\nimport PropTypes from 'prop-types';\n\n/** \n * This class will be used by DAOInfo and PlatformInfo\n */\nexport default class ParticipationStat extends Component {\n    render () {\n        const { text, value } = this.props;\n        if (value) {\n            return (<div><b>{value}</b> {text}</div>);\n        } else {\n            return (<div>{text}</div>);\n        }\n    }\n}\n\nParticipationStat.propTypes = {\n    /**\n     * The text to show\n     */\n    text: PropTypes.string.isRequired,\n\n    /**\n     * The value to highlight, which will be appended to text\n     */\n    value: PropTypes.string,\n\n    /**\n     * The key used by React for optimization\n     */\n    key: PropTypes.string,\n}\n",
```

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer_components/dao_analyzer_components/metadata.json` & `dao_analyzer-1.3.3.dev7/dao_analyzer_components/dao_analyzer_components/metadata.json`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer_components/dao_analyzer_components/package-info.json` & `dao_analyzer-1.3.3.dev7/dao_analyzer_components/dao_analyzer_components/package-info.json`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer_components/package-lock.json` & `dao_analyzer-1.3.3.dev7/dao_analyzer_components/package-lock.json`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer_components/package.json` & `dao_analyzer-1.3.3.dev7/dao_analyzer_components/package.json`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer_components/setup.py` & `dao_analyzer-1.3.3.dev7/dao_analyzer_components/setup.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer_components/src/lib/components/DAOInfo.jsx` & `dao_analyzer-1.3.3.dev7/dao_analyzer_components/src/lib/components/DAOInfo.jsx`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer_components/src/lib/components/DataPoint.jsx` & `dao_analyzer-1.3.3.dev7/dao_analyzer_components/src/lib/components/DataPoint.jsx`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer_components/src/lib/components/ParticipationStat.jsx` & `dao_analyzer-1.3.3.dev7/dao_analyzer_components/src/lib/components/ParticipationStat.jsx`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer_components/src/lib/components/PlatformInfo.jsx` & `dao_analyzer-1.3.3.dev7/dao_analyzer_components/src/lib/components/PlatformInfo.jsx`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/dao_analyzer_components/webpack.config.js` & `dao_analyzer-1.3.3.dev7/dao_analyzer_components/webpack.config.js`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/scripts/archive/names.ipynb` & `dao_analyzer-1.3.3.dev7/scripts/archive/names.ipynb`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/scripts/archive/uploadToKaggle.sh` & `dao_analyzer-1.3.3.dev7/scripts/archive/uploadToKaggle.sh`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/scripts/checkContinue.sh` & `dao_analyzer-1.3.3.dev7/scripts/checkContinue.sh`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/scripts/datawarehouseDiff.py` & `dao_analyzer-1.3.3.dev7/scripts/datawarehouseDiff.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/scripts/updateAragonNames.py` & `dao_analyzer-1.3.3.dev7/scripts/updateAragonNames.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/scripts/uploadDataWarehouse.py` & `dao_analyzer-1.3.3.dev7/scripts/uploadDataWarehouse.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/setup.cfg` & `dao_analyzer-1.3.3.dev7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 	Topic :: Sociology
 	Typing :: Typed
 	Topic :: Utilities
 
 [options]
 python_requires = >= 3.9
 install_requires = 
-	dao-scripts == 1.3.1
+	dao-scripts == 1.4.6
 	dash >= 2.17.0
 	dash-bootstrap-components >= 1.1.0
 	Werkzeug < 2.1.0 # Waiting for upstream fix on dash part
 	flask >= 2.0.2
 	gql >= 3.0.0a1
 	millify >= 0.1.1
 	numpy >= 1.17.3
```

### Comparing `dao_analyzer-1.3.3.dev6/setup.py` & `dao_analyzer-1.3.3.dev7/setup.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/test/mocks/api_requester_mock.py` & `dao_analyzer-1.3.3.dev7/test/mocks/api_requester_mock.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/test/mocks/unix_date_builder.py` & `dao_analyzer-1.3.3.dev7/test/mocks/unix_date_builder.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/test/unit/apps/aragon/data_access/daos/metric/strategy/test_aragon_st_new_additions.py` & `dao_analyzer-1.3.3.dev7/test/unit/apps/aragon/data_access/daos/metric/strategy/test_aragon_st_new_additions.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_active_organization_aragon.py` & `dao_analyzer-1.3.3.dev7/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_active_organization_aragon.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_active_token_holders.py` & `dao_analyzer-1.3.3.dev7/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_active_token_holders.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_cast_type.py` & `dao_analyzer-1.3.3.dev7/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_cast_type.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_installed_apps.py` & `dao_analyzer-1.3.3.dev7/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_installed_apps.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_vote_outcome.py` & `dao_analyzer-1.3.3.dev7/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_vote_outcome.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/test/unit/apps/common/api/graphql/test_query_builder.py` & `dao_analyzer-1.3.3.dev7/test/unit/apps/common/api/graphql/test_query_builder.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/test/unit/apps/common/business/transfers/test_organization.py` & `dao_analyzer-1.3.3.dev7/test/unit/apps/common/business/transfers/test_organization.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_active_members.py` & `dao_analyzer-1.3.3.dev7/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_active_members.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_active_organization_daohaus.py` & `dao_analyzer-1.3.3.dev7/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_active_organization_daohaus.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_active_voters.py` & `dao_analyzer-1.3.3.dev7/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_active_voters.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_dproposal_outcome.py` & `dao_analyzer-1.3.3.dev7/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_dproposal_outcome.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_new_additions.py` & `dao_analyzer-1.3.3.dev7/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_new_additions.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_proposal_type.py` & `dao_analyzer-1.3.3.dev7/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_proposal_type.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_total_members.py` & `dao_analyzer-1.3.3.dev7/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_total_members.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_votes_type.py` & `dao_analyzer-1.3.3.dev7/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_votes_type.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_active_organization_daostack.py` & `dao_analyzer-1.3.3.dev7/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_active_organization_daostack.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_active_users.py` & `dao_analyzer-1.3.3.dev7/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_active_users.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_diff_voters_stakers.py` & `dao_analyzer-1.3.3.dev7/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_diff_voters_stakers.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_proposal_majority.py` & `dao_analyzer-1.3.3.dev7/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_proposal_majority.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_proposal_outcome.py` & `dao_analyzer-1.3.3.dev7/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_proposal_outcome.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_time_serie.py` & `dao_analyzer-1.3.3.dev7/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_time_serie.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.3.dev6/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_voters_percentage.py` & `dao_analyzer-1.3.3.dev7/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_voters_percentage.py`

 * *Files identical despite different names*

