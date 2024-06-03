# Comparing `tmp/ul-db-utils-3.3.6.tar.gz` & `tmp/ul-db-utils-3.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ul-db-utils-3.3.6.tar", last modified: Mon May  6 13:29:38 2024, max compression
+gzip compressed data, was "ul-db-utils-3.3.7.tar", last modified: Mon Jun  3 09:07:33 2024, max compression
```

## Comparing `ul-db-utils-3.3.6.tar` & `ul-db-utils-3.3.7.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 13:29:38.344478 ul-db-utils-3.3.6/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-06 13:29:35.000000 ul-db-utils-3.3.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)     7093 2024-05-06 13:29:38.344478 ul-db-utils-3.3.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6419 2023-04-21 10:03:22.000000 ul-db-utils-3.3.6/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-06 13:29:38.344478 ul-db-utils-3.3.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2074 2024-05-06 13:29:35.000000 ul-db-utils-3.3.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 13:29:38.280477 ul-db-utils-3.3.6/ul_db_utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-06 13:29:35.000000 ul-db-utils-3.3.6/ul_db_utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 13:29:38.296477 ul-db-utils-3.3.6/ul_db_utils/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-06 13:29:35.000000 ul-db-utils-3.3.6/ul_db_utils/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1351 2024-04-24 06:53:46.000000 ul-db-utils-3.3.6/ul_db_utils/commands/cmd_action.py
--rw-rw-rw-   0 root         (0) root         (0)     2464 2023-09-21 10:06:49.000000 ul-db-utils-3.3.6/ul_db_utils/commands/cmd_docs.py
--rw-rw-rw-   0 root         (0) root         (0)     1401 2023-09-21 10:06:49.000000 ul-db-utils-3.3.6/ul_db_utils/commands/cmd_dump.py
--rw-rw-rw-   0 root         (0) root         (0)     3894 2023-09-21 10:06:49.000000 ul-db-utils-3.3.6/ul_db_utils/commands/cmd_restore.py
--rw-rw-rw-   0 root         (0) root         (0)     1236 2023-11-27 13:40:30.000000 ul-db-utils-3.3.6/ul_db_utils/commands/cmd_waiting.py
--rw-rw-rw-   0 root         (0) root         (0)      794 2023-09-21 10:06:49.000000 ul-db-utils-3.3.6/ul_db_utils/commands/doc_request_sql.sql
--rw-rw-rw-   0 root         (0) root         (0)     1128 2024-04-24 06:53:46.000000 ul-db-utils-3.3.6/ul_db_utils/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 13:29:38.308477 ul-db-utils-3.3.6/ul_db_utils/errors/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-06 13:29:35.000000 ul-db-utils-3.3.6/ul_db_utils/errors/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      278 2023-09-21 10:06:49.000000 ul-db-utils-3.3.6/ul_db_utils/errors/compare_null_error.py
--rw-rw-rw-   0 root         (0) root         (0)       35 2023-09-21 10:06:49.000000 ul-db-utils-3.3.6/ul_db_utils/errors/db_error.py
--rw-rw-rw-   0 root         (0) root         (0)      167 2023-09-21 10:06:49.000000 ul-db-utils-3.3.6/ul_db_utils/errors/db_filter_error.py
--rw-rw-rw-   0 root         (0) root         (0)      161 2023-09-21 10:06:49.000000 ul-db-utils-3.3.6/ul_db_utils/errors/db_sort_error.py
--rw-rw-rw-   0 root         (0) root         (0)      155 2023-09-21 10:06:49.000000 ul-db-utils-3.3.6/ul_db_utils/errors/deletion_not_allowed.py
--rw-rw-rw-   0 root         (0) root         (0)      161 2023-09-21 10:06:49.000000 ul-db-utils-3.3.6/ul_db_utils/errors/multiple_objects_returned.py
--rw-rw-rw-   0 root         (0) root         (0)      318 2023-09-21 10:06:49.000000 ul-db-utils-3.3.6/ul_db_utils/errors/unknow_field_error.py
--rw-rw-rw-   0 root         (0) root         (0)      166 2023-09-21 10:06:49.000000 ul-db-utils-3.3.6/ul_db_utils/errors/update_column_not_allowed_error.py
--rw-rw-rw-   0 root         (0) root         (0)      153 2023-09-21 10:06:49.000000 ul-db-utils-3.3.6/ul_db_utils/errors/update_not_allowed.py
--rw-rw-rw-   0 root         (0) root         (0)      830 2023-09-21 10:06:49.000000 ul-db-utils-3.3.6/ul_db_utils/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 13:29:38.312477 ul-db-utils-3.3.6/ul_db_utils/model/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-06 13:29:35.000000 ul-db-utils-3.3.6/ul_db_utils/model/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      695 2024-04-24 06:53:46.000000 ul-db-utils-3.3.6/ul_db_utils/model/api_user.py
--rw-rw-rw-   0 root         (0) root         (0)     5739 2024-04-24 06:53:46.000000 ul-db-utils-3.3.6/ul_db_utils/model/base_api_user_log_model.py
--rw-rw-rw-   0 root         (0) root         (0)      510 2024-04-24 06:53:46.000000 ul-db-utils-3.3.6/ul_db_utils/model/base_document.py
--rw-rw-rw-   0 root         (0) root         (0)     3191 2024-04-24 06:53:46.000000 ul-db-utils-3.3.6/ul_db_utils/model/base_immutable_model.py
--rw-rw-rw-   0 root         (0) root         (0)     5826 2024-04-24 06:53:46.000000 ul-db-utils-3.3.6/ul_db_utils/model/base_mater_pg_view.py
--rw-rw-rw-   0 root         (0) root         (0)     4355 2024-04-24 06:53:46.000000 ul-db-utils-3.3.6/ul_db_utils/model/base_model.py
--rw-rw-rw-   0 root         (0) root         (0)     3899 2024-04-24 06:53:46.000000 ul-db-utils-3.3.6/ul_db_utils/model/base_undeletable_model.py
--rw-rw-rw-   0 root         (0) root         (0)     4931 2024-04-24 06:53:46.000000 ul-db-utils-3.3.6/ul_db_utils/model/base_undeletable_user_log_model.py
--rw-rw-rw-   0 root         (0) root         (0)     5457 2024-04-24 06:53:46.000000 ul-db-utils-3.3.6/ul_db_utils/model/base_user_log_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 13:29:38.312477 ul-db-utils-3.3.6/ul_db_utils/model/media_storage/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-06 13:29:35.000000 ul-db-utils-3.3.6/ul_db_utils/model/media_storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1297 2024-04-24 06:53:46.000000 ul-db-utils-3.3.6/ul_db_utils/model/media_storage/media_file.py
--rw-rw-rw-   0 root         (0) root         (0)     1295 2024-04-24 06:53:46.000000 ul-db-utils-3.3.6/ul_db_utils/model/media_storage/media_file_download_link.py
--rw-rw-rw-   0 root         (0) root         (0)      695 2024-04-24 06:53:46.000000 ul-db-utils-3.3.6/ul_db_utils/model/media_storage/media_file_type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 13:29:38.312477 ul-db-utils-3.3.6/ul_db_utils/model/methods/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-06 13:29:35.000000 ul-db-utils-3.3.6/ul_db_utils/model/methods/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      722 2024-04-24 06:53:46.000000 ul-db-utils-3.3.6/ul_db_utils/model/methods/make_immutable_column.py
--rw-rw-rw-   0 root         (0) root         (0)     1057 2024-04-24 06:53:46.000000 ul-db-utils-3.3.6/ul_db_utils/model/referense_link.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 13:29:38.312477 ul-db-utils-3.3.6/ul_db_utils/modules/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-06 13:29:35.000000 ul-db-utils-3.3.6/ul_db_utils/modules/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11888 2023-09-21 10:06:49.000000 ul-db-utils-3.3.6/ul_db_utils/modules/audit.sql
--rw-rw-rw-   0 root         (0) root         (0)     1699 2024-04-24 06:53:46.000000 ul-db-utils-3.3.6/ul_db_utils/modules/audit_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     2123 2024-05-06 13:29:35.000000 ul-db-utils-3.3.6/ul_db_utils/modules/custom_query.py
--rw-rw-rw-   0 root         (0) root         (0)     5798 2024-05-06 13:29:35.000000 ul-db-utils-3.3.6/ul_db_utils/modules/db.py
--rw-rw-rw-   0 root         (0) root         (0)      585 2024-05-06 13:29:35.000000 ul-db-utils-3.3.6/ul_db_utils/modules/db_context.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 13:29:38.312477 ul-db-utils-3.3.6/ul_db_utils/modules/mongo_db_modules/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-06 13:29:35.000000 ul-db-utils-3.3.6/ul_db_utils/modules/mongo_db_modules/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4369 2024-05-06 13:29:35.000000 ul-db-utils-3.3.6/ul_db_utils/modules/mongo_db_modules/db.py
--rw-rw-rw-   0 root         (0) root         (0)      591 2023-11-27 13:40:30.000000 ul-db-utils-3.3.6/ul_db_utils/modules/mongo_db_modules/db_context.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 13:29:38.316478 ul-db-utils-3.3.6/ul_db_utils/modules/postgres_modules/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-06 13:29:35.000000 ul-db-utils-3.3.6/ul_db_utils/modules/postgres_modules/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2123 2024-04-24 06:53:46.000000 ul-db-utils-3.3.6/ul_db_utils/modules/postgres_modules/custom_query.py
--rw-rw-rw-   0 root         (0) root         (0)     6105 2024-05-06 13:29:35.000000 ul-db-utils-3.3.6/ul_db_utils/modules/postgres_modules/db.py
--rw-rw-rw-   0 root         (0) root         (0)      585 2024-04-24 06:53:46.000000 ul-db-utils-3.3.6/ul_db_utils/modules/postgres_modules/db_context.py
--rw-rw-rw-   0 root         (0) root         (0)      504 2024-04-24 06:53:46.000000 ul-db-utils-3.3.6/ul_db_utils/modules/postgres_modules/transaction_commit.py
--rw-rw-rw-   0 root         (0) root         (0)      504 2024-05-06 13:29:35.000000 ul-db-utils-3.3.6/ul_db_utils/modules/transaction_commit.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-06 13:29:35.000000 ul-db-utils-3.3.6/ul_db_utils/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 13:29:38.316478 ul-db-utils-3.3.6/ul_db_utils/repository/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-06 13:29:35.000000 ul-db-utils-3.3.6/ul_db_utils/repository/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1072 2024-05-06 13:29:35.000000 ul-db-utils-3.3.6/ul_db_utils/repository/abstract_repository.py
--rw-rw-rw-   0 root         (0) root         (0)     1797 2024-05-06 13:29:35.000000 ul-db-utils-3.3.6/ul_db_utils/repository/mongoengine_repository.py
--rw-rw-rw-   0 root         (0) root         (0)     1887 2024-05-06 13:29:35.000000 ul-db-utils-3.3.6/ul_db_utils/repository/sqlalchemy_repository.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 13:29:38.316478 ul-db-utils-3.3.6/ul_db_utils/search/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-06 13:29:35.000000 ul-db-utils-3.3.6/ul_db_utils/search/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13824 2023-09-21 10:06:49.000000 ul-db-utils-3.3.6/ul_db_utils/search/db_search.py
--rw-rw-rw-   0 root         (0) root         (0)     1153 2024-04-24 06:53:46.000000 ul-db-utils-3.3.6/ul_db_utils/search/doc_db_search.py
--rw-rw-rw-   0 root         (0) root         (0)     9316 2023-09-21 10:06:49.000000 ul-db-utils-3.3.6/ul_db_utils/search/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 13:29:38.324478 ul-db-utils-3.3.6/ul_db_utils/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-06 13:29:35.000000 ul-db-utils-3.3.6/ul_db_utils/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      140 2024-04-24 06:53:46.000000 ul-db-utils-3.3.6/ul_db_utils/utils/camel_to_snake.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 13:29:38.340478 ul-db-utils-3.3.6/ul_db_utils/utils/ensure/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-06 13:29:35.000000 ul-db-utils-3.3.6/ul_db_utils/utils/ensure/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      119 2023-09-21 10:06:49.000000 ul-db-utils-3.3.6/ul_db_utils/utils/ensure/ensure_bool.py
--rw-rw-rw-   0 root         (0) root         (0)      356 2023-09-21 10:06:49.000000 ul-db-utils-3.3.6/ul_db_utils/utils/ensure/ensure_choices.py
--rw-rw-rw-   0 root         (0) root         (0)      307 2023-09-21 10:06:49.000000 ul-db-utils-3.3.6/ul_db_utils/utils/ensure/ensure_dict_keys.py
--rw-rw-rw-   0 root         (0) root         (0)      383 2023-09-21 10:06:49.000000 ul-db-utils-3.3.6/ul_db_utils/utils/ensure/ensure_dict_keys_choice.py
--rw-rw-rw-   0 root         (0) root         (0)      579 2023-09-21 10:06:49.000000 ul-db-utils-3.3.6/ul_db_utils/utils/ensure/ensure_dict_keys_strict.py
--rw-rw-rw-   0 root         (0) root         (0)      293 2023-09-21 10:06:49.000000 ul-db-utils-3.3.6/ul_db_utils/utils/ensure/ensure_dict_str_keys.py
--rw-rw-rw-   0 root         (0) root         (0)      341 2023-09-21 10:06:49.000000 ul-db-utils-3.3.6/ul_db_utils/utils/ensure/ensure_dict_upper_keys.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2023-09-21 10:06:49.000000 ul-db-utils-3.3.6/ul_db_utils/utils/ensure/ensure_float.py
--rw-rw-rw-   0 root         (0) root         (0)      115 2023-09-21 10:06:49.000000 ul-db-utils-3.3.6/ul_db_utils/utils/ensure/ensure_int.py
--rw-rw-rw-   0 root         (0) root         (0)      307 2023-09-21 10:06:49.000000 ul-db-utils-3.3.6/ul_db_utils/utils/ensure/ensure_int_positive.py
--rw-rw-rw-   0 root         (0) root         (0)      119 2023-09-21 10:06:49.000000 ul-db-utils-3.3.6/ul_db_utils/utils/ensure/ensure_len.py
--rw-rw-rw-   0 root         (0) root         (0)      331 2023-09-21 10:06:49.000000 ul-db-utils-3.3.6/ul_db_utils/utils/ensure/ensure_list.py
--rw-rw-rw-   0 root         (0) root         (0)      305 2023-09-21 10:06:49.000000 ul-db-utils-3.3.6/ul_db_utils/utils/ensure/ensure_list_of.py
--rw-rw-rw-   0 root         (0) root         (0)      170 2023-09-21 10:06:49.000000 ul-db-utils-3.3.6/ul_db_utils/utils/ensure/ensure_positive_int_non_zero.py
--rw-rw-rw-   0 root         (0) root         (0)      173 2023-09-21 10:06:49.000000 ul-db-utils-3.3.6/ul_db_utils/utils/ensure/ensure_set.py
--rw-rw-rw-   0 root         (0) root         (0)      115 2023-09-21 10:06:49.000000 ul-db-utils-3.3.6/ul_db_utils/utils/ensure/ensure_str.py
--rw-rw-rw-   0 root         (0) root         (0)      220 2023-09-21 10:06:49.000000 ul-db-utils-3.3.6/ul_db_utils/utils/ensure/ensure_type.py
--rw-rw-rw-   0 root         (0) root         (0)      283 2023-09-21 10:06:49.000000 ul-db-utils-3.3.6/ul_db_utils/utils/ensure/ensure_url_with_scheme_and_netloc.py
--rw-rw-rw-   0 root         (0) root         (0)      511 2024-04-24 06:53:46.000000 ul-db-utils-3.3.6/ul_db_utils/utils/ensure_db_object_exists.py
--rw-rw-rw-   0 root         (0) root         (0)     4450 2024-04-24 06:53:46.000000 ul-db-utils-3.3.6/ul_db_utils/utils/filter_conversion_doc_db.py
--rw-rw-rw-   0 root         (0) root         (0)     1209 2024-04-24 06:53:46.000000 ul-db-utils-3.3.6/ul_db_utils/utils/get_model_template.py
--rw-rw-rw-   0 root         (0) root         (0)     2170 2024-04-24 06:53:46.000000 ul-db-utils-3.3.6/ul_db_utils/utils/query_soft_delete.py
--rw-rw-rw-   0 root         (0) root         (0)      161 2023-09-21 10:06:49.000000 ul-db-utils-3.3.6/ul_db_utils/utils/remove_duplicated_spaces_of_string.py
--rw-rw-rw-   0 root         (0) root         (0)      113 2024-04-24 06:53:46.000000 ul-db-utils-3.3.6/ul_db_utils/utils/types.py
--rw-rw-rw-   0 root         (0) root         (0)      703 2023-11-27 13:40:30.000000 ul-db-utils-3.3.6/ul_db_utils/utils/waiting_for_mongo.py
--rw-rw-rw-   0 root         (0) root         (0)     1032 2023-09-21 10:06:49.000000 ul-db-utils-3.3.6/ul_db_utils/utils/waiting_for_postgres.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 13:29:38.280477 ul-db-utils-3.3.6/ul_db_utils.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7093 2024-05-06 13:29:38.000000 ul-db-utils-3.3.6/ul_db_utils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3890 2024-05-06 13:29:38.000000 ul-db-utils-3.3.6/ul_db_utils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-06 13:29:38.000000 ul-db-utils-3.3.6/ul_db_utils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2024-05-06 13:29:38.000000 ul-db-utils-3.3.6/ul_db_utils.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      504 2024-05-06 13:29:38.000000 ul-db-utils-3.3.6/ul_db_utils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-05-06 13:29:38.000000 ul-db-utils-3.3.6/ul_db_utils.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 09:07:33.831559 ul-db-utils-3.3.7/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-03 09:07:32.000000 ul-db-utils-3.3.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     7093 2024-06-03 09:07:33.831559 ul-db-utils-3.3.7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6419 2023-04-21 10:27:38.000000 ul-db-utils-3.3.7/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-06-03 09:07:33.831559 ul-db-utils-3.3.7/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2103 2024-06-03 09:07:32.000000 ul-db-utils-3.3.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 09:07:33.703555 ul-db-utils-3.3.7/ul_db_utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-03 09:07:32.000000 ul-db-utils-3.3.7/ul_db_utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 09:07:33.771557 ul-db-utils-3.3.7/ul_db_utils/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-03 09:07:32.000000 ul-db-utils-3.3.7/ul_db_utils/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1351 2023-12-20 09:16:29.000000 ul-db-utils-3.3.7/ul_db_utils/commands/cmd_action.py
+-rw-rw-rw-   0 root         (0) root         (0)     2464 2023-09-20 12:05:30.000000 ul-db-utils-3.3.7/ul_db_utils/commands/cmd_docs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1401 2023-08-15 07:54:33.000000 ul-db-utils-3.3.7/ul_db_utils/commands/cmd_dump.py
+-rw-rw-rw-   0 root         (0) root         (0)     3894 2023-08-15 07:54:33.000000 ul-db-utils-3.3.7/ul_db_utils/commands/cmd_restore.py
+-rw-rw-rw-   0 root         (0) root         (0)     1236 2023-11-29 15:18:45.000000 ul-db-utils-3.3.7/ul_db_utils/commands/cmd_waiting.py
+-rw-rw-rw-   0 root         (0) root         (0)      794 2023-08-15 07:54:33.000000 ul-db-utils-3.3.7/ul_db_utils/commands/doc_request_sql.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1128 2024-06-03 09:07:32.000000 ul-db-utils-3.3.7/ul_db_utils/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 09:07:33.795558 ul-db-utils-3.3.7/ul_db_utils/errors/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-03 09:07:32.000000 ul-db-utils-3.3.7/ul_db_utils/errors/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      278 2023-08-15 07:54:33.000000 ul-db-utils-3.3.7/ul_db_utils/errors/compare_null_error.py
+-rw-rw-rw-   0 root         (0) root         (0)       35 2023-08-15 07:54:33.000000 ul-db-utils-3.3.7/ul_db_utils/errors/db_error.py
+-rw-rw-rw-   0 root         (0) root         (0)      167 2023-08-15 07:54:33.000000 ul-db-utils-3.3.7/ul_db_utils/errors/db_filter_error.py
+-rw-rw-rw-   0 root         (0) root         (0)      161 2023-08-15 07:54:33.000000 ul-db-utils-3.3.7/ul_db_utils/errors/db_sort_error.py
+-rw-rw-rw-   0 root         (0) root         (0)      155 2023-08-15 07:54:33.000000 ul-db-utils-3.3.7/ul_db_utils/errors/deletion_not_allowed.py
+-rw-rw-rw-   0 root         (0) root         (0)      161 2023-08-15 07:54:33.000000 ul-db-utils-3.3.7/ul_db_utils/errors/multiple_objects_returned.py
+-rw-rw-rw-   0 root         (0) root         (0)      318 2023-08-15 07:54:33.000000 ul-db-utils-3.3.7/ul_db_utils/errors/unknow_field_error.py
+-rw-rw-rw-   0 root         (0) root         (0)      166 2023-08-15 07:54:33.000000 ul-db-utils-3.3.7/ul_db_utils/errors/update_column_not_allowed_error.py
+-rw-rw-rw-   0 root         (0) root         (0)      153 2023-08-15 07:54:33.000000 ul-db-utils-3.3.7/ul_db_utils/errors/update_not_allowed.py
+-rw-rw-rw-   0 root         (0) root         (0)      830 2023-08-15 07:54:33.000000 ul-db-utils-3.3.7/ul_db_utils/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 09:07:33.795558 ul-db-utils-3.3.7/ul_db_utils/model/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-03 09:07:32.000000 ul-db-utils-3.3.7/ul_db_utils/model/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      695 2024-04-22 07:48:28.000000 ul-db-utils-3.3.7/ul_db_utils/model/api_user.py
+-rw-rw-rw-   0 root         (0) root         (0)     5739 2024-04-22 07:48:28.000000 ul-db-utils-3.3.7/ul_db_utils/model/base_api_user_log_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      510 2023-12-20 09:16:29.000000 ul-db-utils-3.3.7/ul_db_utils/model/base_document.py
+-rw-rw-rw-   0 root         (0) root         (0)     3191 2024-04-22 07:48:28.000000 ul-db-utils-3.3.7/ul_db_utils/model/base_immutable_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     5826 2024-04-22 07:48:28.000000 ul-db-utils-3.3.7/ul_db_utils/model/base_mater_pg_view.py
+-rw-rw-rw-   0 root         (0) root         (0)     4355 2024-04-22 07:48:28.000000 ul-db-utils-3.3.7/ul_db_utils/model/base_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     3899 2024-04-22 07:48:28.000000 ul-db-utils-3.3.7/ul_db_utils/model/base_undeletable_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     4931 2024-04-22 07:48:28.000000 ul-db-utils-3.3.7/ul_db_utils/model/base_undeletable_user_log_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     5457 2024-04-22 07:48:28.000000 ul-db-utils-3.3.7/ul_db_utils/model/base_user_log_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 09:07:33.795558 ul-db-utils-3.3.7/ul_db_utils/model/media_storage/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-03 09:07:32.000000 ul-db-utils-3.3.7/ul_db_utils/model/media_storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1297 2024-04-22 07:48:28.000000 ul-db-utils-3.3.7/ul_db_utils/model/media_storage/media_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     1295 2024-04-22 07:48:28.000000 ul-db-utils-3.3.7/ul_db_utils/model/media_storage/media_file_download_link.py
+-rw-rw-rw-   0 root         (0) root         (0)      695 2024-04-22 07:48:28.000000 ul-db-utils-3.3.7/ul_db_utils/model/media_storage/media_file_type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 09:07:33.795558 ul-db-utils-3.3.7/ul_db_utils/model/methods/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-03 09:07:32.000000 ul-db-utils-3.3.7/ul_db_utils/model/methods/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      722 2024-04-22 07:48:28.000000 ul-db-utils-3.3.7/ul_db_utils/model/methods/make_immutable_column.py
+-rw-rw-rw-   0 root         (0) root         (0)     1057 2024-04-22 07:48:28.000000 ul-db-utils-3.3.7/ul_db_utils/model/referense_link.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 09:07:33.799558 ul-db-utils-3.3.7/ul_db_utils/modules/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-03 09:07:32.000000 ul-db-utils-3.3.7/ul_db_utils/modules/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11888 2023-08-15 07:54:33.000000 ul-db-utils-3.3.7/ul_db_utils/modules/audit.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1699 2024-04-22 07:48:28.000000 ul-db-utils-3.3.7/ul_db_utils/modules/audit_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     2123 2024-06-03 09:07:32.000000 ul-db-utils-3.3.7/ul_db_utils/modules/custom_query.py
+-rw-rw-rw-   0 root         (0) root         (0)     5798 2024-06-03 09:07:32.000000 ul-db-utils-3.3.7/ul_db_utils/modules/db.py
+-rw-rw-rw-   0 root         (0) root         (0)      585 2024-06-03 09:07:32.000000 ul-db-utils-3.3.7/ul_db_utils/modules/db_context.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 09:07:33.799558 ul-db-utils-3.3.7/ul_db_utils/modules/mongo_db_modules/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-03 09:07:32.000000 ul-db-utils-3.3.7/ul_db_utils/modules/mongo_db_modules/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4369 2024-06-03 09:07:32.000000 ul-db-utils-3.3.7/ul_db_utils/modules/mongo_db_modules/db.py
+-rw-rw-rw-   0 root         (0) root         (0)      591 2023-11-29 15:18:45.000000 ul-db-utils-3.3.7/ul_db_utils/modules/mongo_db_modules/db_context.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 09:07:33.799558 ul-db-utils-3.3.7/ul_db_utils/modules/postgres_modules/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-03 09:07:32.000000 ul-db-utils-3.3.7/ul_db_utils/modules/postgres_modules/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2123 2024-04-22 07:48:28.000000 ul-db-utils-3.3.7/ul_db_utils/modules/postgres_modules/custom_query.py
+-rw-rw-rw-   0 root         (0) root         (0)     6105 2024-06-03 09:07:32.000000 ul-db-utils-3.3.7/ul_db_utils/modules/postgres_modules/db.py
+-rw-rw-rw-   0 root         (0) root         (0)      585 2024-04-22 07:48:28.000000 ul-db-utils-3.3.7/ul_db_utils/modules/postgres_modules/db_context.py
+-rw-rw-rw-   0 root         (0) root         (0)      504 2024-04-22 07:48:28.000000 ul-db-utils-3.3.7/ul_db_utils/modules/postgres_modules/transaction_commit.py
+-rw-rw-rw-   0 root         (0) root         (0)      504 2024-06-03 09:07:32.000000 ul-db-utils-3.3.7/ul_db_utils/modules/transaction_commit.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-03 09:07:32.000000 ul-db-utils-3.3.7/ul_db_utils/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 09:07:33.799558 ul-db-utils-3.3.7/ul_db_utils/repository/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-03 09:07:32.000000 ul-db-utils-3.3.7/ul_db_utils/repository/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2024-06-03 09:07:32.000000 ul-db-utils-3.3.7/ul_db_utils/repository/abstract_repository.py
+-rw-rw-rw-   0 root         (0) root         (0)     1797 2024-06-03 09:07:32.000000 ul-db-utils-3.3.7/ul_db_utils/repository/mongoengine_repository.py
+-rw-rw-rw-   0 root         (0) root         (0)     1887 2024-06-03 09:07:32.000000 ul-db-utils-3.3.7/ul_db_utils/repository/sqlalchemy_repository.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 09:07:33.803558 ul-db-utils-3.3.7/ul_db_utils/search/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-03 09:07:32.000000 ul-db-utils-3.3.7/ul_db_utils/search/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13824 2023-09-20 12:05:30.000000 ul-db-utils-3.3.7/ul_db_utils/search/db_search.py
+-rw-rw-rw-   0 root         (0) root         (0)     1153 2024-04-22 07:48:28.000000 ul-db-utils-3.3.7/ul_db_utils/search/doc_db_search.py
+-rw-rw-rw-   0 root         (0) root         (0)     9316 2023-09-20 12:05:30.000000 ul-db-utils-3.3.7/ul_db_utils/search/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 09:07:33.811558 ul-db-utils-3.3.7/ul_db_utils/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-03 09:07:32.000000 ul-db-utils-3.3.7/ul_db_utils/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      140 2023-12-20 09:16:29.000000 ul-db-utils-3.3.7/ul_db_utils/utils/camel_to_snake.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 09:07:33.831559 ul-db-utils-3.3.7/ul_db_utils/utils/ensure/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-03 09:07:32.000000 ul-db-utils-3.3.7/ul_db_utils/utils/ensure/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      119 2023-08-15 07:54:33.000000 ul-db-utils-3.3.7/ul_db_utils/utils/ensure/ensure_bool.py
+-rw-rw-rw-   0 root         (0) root         (0)      356 2023-08-15 07:54:33.000000 ul-db-utils-3.3.7/ul_db_utils/utils/ensure/ensure_choices.py
+-rw-rw-rw-   0 root         (0) root         (0)      307 2023-08-15 07:54:33.000000 ul-db-utils-3.3.7/ul_db_utils/utils/ensure/ensure_dict_keys.py
+-rw-rw-rw-   0 root         (0) root         (0)      383 2023-08-15 07:54:33.000000 ul-db-utils-3.3.7/ul_db_utils/utils/ensure/ensure_dict_keys_choice.py
+-rw-rw-rw-   0 root         (0) root         (0)      579 2023-08-15 07:54:33.000000 ul-db-utils-3.3.7/ul_db_utils/utils/ensure/ensure_dict_keys_strict.py
+-rw-rw-rw-   0 root         (0) root         (0)      293 2023-08-15 07:54:33.000000 ul-db-utils-3.3.7/ul_db_utils/utils/ensure/ensure_dict_str_keys.py
+-rw-rw-rw-   0 root         (0) root         (0)      341 2023-08-15 07:54:33.000000 ul-db-utils-3.3.7/ul_db_utils/utils/ensure/ensure_dict_upper_keys.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2023-08-15 07:54:33.000000 ul-db-utils-3.3.7/ul_db_utils/utils/ensure/ensure_float.py
+-rw-rw-rw-   0 root         (0) root         (0)      115 2023-08-15 07:54:33.000000 ul-db-utils-3.3.7/ul_db_utils/utils/ensure/ensure_int.py
+-rw-rw-rw-   0 root         (0) root         (0)      307 2023-08-15 07:54:33.000000 ul-db-utils-3.3.7/ul_db_utils/utils/ensure/ensure_int_positive.py
+-rw-rw-rw-   0 root         (0) root         (0)      119 2023-08-15 07:54:33.000000 ul-db-utils-3.3.7/ul_db_utils/utils/ensure/ensure_len.py
+-rw-rw-rw-   0 root         (0) root         (0)      331 2023-08-15 07:54:33.000000 ul-db-utils-3.3.7/ul_db_utils/utils/ensure/ensure_list.py
+-rw-rw-rw-   0 root         (0) root         (0)      305 2023-08-15 07:54:33.000000 ul-db-utils-3.3.7/ul_db_utils/utils/ensure/ensure_list_of.py
+-rw-rw-rw-   0 root         (0) root         (0)      170 2023-08-15 07:54:33.000000 ul-db-utils-3.3.7/ul_db_utils/utils/ensure/ensure_positive_int_non_zero.py
+-rw-rw-rw-   0 root         (0) root         (0)      173 2023-08-15 07:54:33.000000 ul-db-utils-3.3.7/ul_db_utils/utils/ensure/ensure_set.py
+-rw-rw-rw-   0 root         (0) root         (0)      115 2023-08-15 07:54:33.000000 ul-db-utils-3.3.7/ul_db_utils/utils/ensure/ensure_str.py
+-rw-rw-rw-   0 root         (0) root         (0)      220 2023-08-15 07:54:33.000000 ul-db-utils-3.3.7/ul_db_utils/utils/ensure/ensure_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      283 2023-08-15 07:54:33.000000 ul-db-utils-3.3.7/ul_db_utils/utils/ensure/ensure_url_with_scheme_and_netloc.py
+-rw-rw-rw-   0 root         (0) root         (0)      511 2024-04-22 07:48:28.000000 ul-db-utils-3.3.7/ul_db_utils/utils/ensure_db_object_exists.py
+-rw-rw-rw-   0 root         (0) root         (0)     4450 2023-12-20 09:16:29.000000 ul-db-utils-3.3.7/ul_db_utils/utils/filter_conversion_doc_db.py
+-rw-rw-rw-   0 root         (0) root         (0)     1209 2024-04-22 07:48:28.000000 ul-db-utils-3.3.7/ul_db_utils/utils/get_model_template.py
+-rw-rw-rw-   0 root         (0) root         (0)     2170 2024-04-22 07:48:28.000000 ul-db-utils-3.3.7/ul_db_utils/utils/query_soft_delete.py
+-rw-rw-rw-   0 root         (0) root         (0)      161 2023-08-15 07:54:33.000000 ul-db-utils-3.3.7/ul_db_utils/utils/remove_duplicated_spaces_of_string.py
+-rw-rw-rw-   0 root         (0) root         (0)      113 2023-12-20 09:16:29.000000 ul-db-utils-3.3.7/ul_db_utils/utils/types.py
+-rw-rw-rw-   0 root         (0) root         (0)      703 2023-11-29 15:18:45.000000 ul-db-utils-3.3.7/ul_db_utils/utils/waiting_for_mongo.py
+-rw-rw-rw-   0 root         (0) root         (0)     1032 2023-08-15 07:54:33.000000 ul-db-utils-3.3.7/ul_db_utils/utils/waiting_for_postgres.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 09:07:33.707555 ul-db-utils-3.3.7/ul_db_utils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7093 2024-06-03 09:07:33.000000 ul-db-utils-3.3.7/ul_db_utils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3890 2024-06-03 09:07:33.000000 ul-db-utils-3.3.7/ul_db_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-06-03 09:07:33.000000 ul-db-utils-3.3.7/ul_db_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2024-06-03 09:07:33.000000 ul-db-utils-3.3.7/ul_db_utils.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      522 2024-06-03 09:07:33.000000 ul-db-utils-3.3.7/ul_db_utils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-06-03 09:07:33.000000 ul-db-utils-3.3.7/ul_db_utils.egg-info/top_level.txt
```

### Comparing `ul-db-utils-3.3.6/PKG-INFO` & `ul-db-utils-3.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ul-db-utils
-Version: 3.3.6
+Version: 3.3.7
 Summary: Python ul db utils
 Home-page: https://gitlab.neroelectronics.by/unic-lab/libraries/common-python-utils/db-utils.git
 Author: Unic-lab
 Author-email: 
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ul-db-utils-3.3.6/README.md` & `ul-db-utils-3.3.7/README.md`

 * *Files identical despite different names*

### Comparing `ul-db-utils-3.3.6/setup.py` & `ul-db-utils-3.3.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     name='ul-db-utils',
-    version='3.3.6',
+    version='3.3.7',
     description='Python ul db utils',
     author='Unic-lab',
     author_email='',
     url='https://gitlab.neroelectronics.by/unic-lab/libraries/common-python-utils/db-utils.git',
     packages=find_packages(include=['ul_db_utils*']),
     platforms='any',
     package_data={
@@ -39,14 +39,15 @@
     },
     include_package_data=True,
     install_requires=[
         "flask==2.1.3",  # FOR COMPATIBILITY
         "py-dateutil==2.2",
 
         "psycopg2-binary==2.9.5",
+        "psycogreen==1.0.2",
         "flask-sqlalchemy==2.5.1",
         "flask-migrate==3.1.0",
         "sqlalchemy[mypy]==1.4.41",
         "sqlalchemy-stubs==0.4",
         "sqlalchemy-utils==0.38.3",
         "sqlalchemy-serializer==1.4.1",
         "alembic==1.8.1",
```

### Comparing `ul-db-utils-3.3.6/ul_db_utils/commands/cmd_action.py` & `ul-db-utils-3.3.7/ul_db_utils/commands/cmd_action.py`

 * *Files identical despite different names*

### Comparing `ul-db-utils-3.3.6/ul_db_utils/commands/cmd_docs.py` & `ul-db-utils-3.3.7/ul_db_utils/commands/cmd_docs.py`

 * *Files identical despite different names*

### Comparing `ul-db-utils-3.3.6/ul_db_utils/commands/cmd_dump.py` & `ul-db-utils-3.3.7/ul_db_utils/commands/cmd_dump.py`

 * *Files identical despite different names*

### Comparing `ul-db-utils-3.3.6/ul_db_utils/commands/cmd_restore.py` & `ul-db-utils-3.3.7/ul_db_utils/commands/cmd_restore.py`

 * *Files identical despite different names*

### Comparing `ul-db-utils-3.3.6/ul_db_utils/commands/cmd_waiting.py` & `ul-db-utils-3.3.7/ul_db_utils/commands/cmd_waiting.py`

 * *Files identical despite different names*

### Comparing `ul-db-utils-3.3.6/ul_db_utils/commands/doc_request_sql.sql` & `ul-db-utils-3.3.7/ul_db_utils/commands/doc_request_sql.sql`

 * *Files identical despite different names*

### Comparing `ul-db-utils-3.3.6/ul_db_utils/conf.py` & `ul-db-utils-3.3.7/ul_db_utils/conf.py`

 * *Files identical despite different names*

### Comparing `ul-db-utils-3.3.6/ul_db_utils/main.py` & `ul-db-utils-3.3.7/ul_db_utils/main.py`

 * *Files identical despite different names*

### Comparing `ul-db-utils-3.3.6/ul_db_utils/model/api_user.py` & `ul-db-utils-3.3.7/ul_db_utils/model/api_user.py`

 * *Files identical despite different names*

### Comparing `ul-db-utils-3.3.6/ul_db_utils/model/base_api_user_log_model.py` & `ul-db-utils-3.3.7/ul_db_utils/model/base_api_user_log_model.py`

 * *Files identical despite different names*

### Comparing `ul-db-utils-3.3.6/ul_db_utils/model/base_immutable_model.py` & `ul-db-utils-3.3.7/ul_db_utils/model/base_immutable_model.py`

 * *Files identical despite different names*

### Comparing `ul-db-utils-3.3.6/ul_db_utils/model/base_mater_pg_view.py` & `ul-db-utils-3.3.7/ul_db_utils/model/base_mater_pg_view.py`

 * *Files identical despite different names*

### Comparing `ul-db-utils-3.3.6/ul_db_utils/model/base_model.py` & `ul-db-utils-3.3.7/ul_db_utils/model/base_model.py`

 * *Files identical despite different names*

### Comparing `ul-db-utils-3.3.6/ul_db_utils/model/base_undeletable_model.py` & `ul-db-utils-3.3.7/ul_db_utils/model/base_undeletable_model.py`

 * *Files identical despite different names*

### Comparing `ul-db-utils-3.3.6/ul_db_utils/model/base_undeletable_user_log_model.py` & `ul-db-utils-3.3.7/ul_db_utils/model/base_undeletable_user_log_model.py`

 * *Files identical despite different names*

### Comparing `ul-db-utils-3.3.6/ul_db_utils/model/base_user_log_model.py` & `ul-db-utils-3.3.7/ul_db_utils/model/base_user_log_model.py`

 * *Files identical despite different names*

### Comparing `ul-db-utils-3.3.6/ul_db_utils/model/media_storage/media_file.py` & `ul-db-utils-3.3.7/ul_db_utils/model/media_storage/media_file.py`

 * *Files identical despite different names*

### Comparing `ul-db-utils-3.3.6/ul_db_utils/model/media_storage/media_file_download_link.py` & `ul-db-utils-3.3.7/ul_db_utils/model/media_storage/media_file_download_link.py`

 * *Files identical despite different names*

### Comparing `ul-db-utils-3.3.6/ul_db_utils/model/media_storage/media_file_type.py` & `ul-db-utils-3.3.7/ul_db_utils/model/media_storage/media_file_type.py`

 * *Files identical despite different names*

### Comparing `ul-db-utils-3.3.6/ul_db_utils/model/methods/make_immutable_column.py` & `ul-db-utils-3.3.7/ul_db_utils/model/methods/make_immutable_column.py`

 * *Files identical despite different names*

### Comparing `ul-db-utils-3.3.6/ul_db_utils/model/referense_link.py` & `ul-db-utils-3.3.7/ul_db_utils/model/referense_link.py`

 * *Files identical despite different names*

### Comparing `ul-db-utils-3.3.6/ul_db_utils/modules/audit.sql` & `ul-db-utils-3.3.7/ul_db_utils/modules/audit.sql`

 * *Files identical despite different names*

### Comparing `ul-db-utils-3.3.6/ul_db_utils/modules/audit_manager.py` & `ul-db-utils-3.3.7/ul_db_utils/modules/audit_manager.py`

 * *Files identical despite different names*

### Comparing `ul-db-utils-3.3.6/ul_db_utils/modules/custom_query.py` & `ul-db-utils-3.3.7/ul_db_utils/modules/custom_query.py`

 * *Files identical despite different names*

### Comparing `ul-db-utils-3.3.6/ul_db_utils/modules/db.py` & `ul-db-utils-3.3.7/ul_db_utils/modules/db.py`

 * *Files identical despite different names*

### Comparing `ul-db-utils-3.3.6/ul_db_utils/modules/db_context.py` & `ul-db-utils-3.3.7/ul_db_utils/modules/db_context.py`

 * *Files identical despite different names*

### Comparing `ul-db-utils-3.3.6/ul_db_utils/modules/mongo_db_modules/db.py` & `ul-db-utils-3.3.7/ul_db_utils/modules/mongo_db_modules/db.py`

 * *Files identical despite different names*

### Comparing `ul-db-utils-3.3.6/ul_db_utils/modules/mongo_db_modules/db_context.py` & `ul-db-utils-3.3.7/ul_db_utils/modules/mongo_db_modules/db_context.py`

 * *Files identical despite different names*

### Comparing `ul-db-utils-3.3.6/ul_db_utils/modules/postgres_modules/custom_query.py` & `ul-db-utils-3.3.7/ul_db_utils/modules/postgres_modules/custom_query.py`

 * *Files identical despite different names*

### Comparing `ul-db-utils-3.3.6/ul_db_utils/modules/postgres_modules/db.py` & `ul-db-utils-3.3.7/ul_db_utils/modules/postgres_modules/db.py`

 * *Files identical despite different names*

### Comparing `ul-db-utils-3.3.6/ul_db_utils/modules/postgres_modules/db_context.py` & `ul-db-utils-3.3.7/ul_db_utils/modules/postgres_modules/db_context.py`

 * *Files identical despite different names*

### Comparing `ul-db-utils-3.3.6/ul_db_utils/repository/abstract_repository.py` & `ul-db-utils-3.3.7/ul_db_utils/repository/abstract_repository.py`

 * *Files identical despite different names*

### Comparing `ul-db-utils-3.3.6/ul_db_utils/repository/mongoengine_repository.py` & `ul-db-utils-3.3.7/ul_db_utils/repository/mongoengine_repository.py`

 * *Files identical despite different names*

### Comparing `ul-db-utils-3.3.6/ul_db_utils/repository/sqlalchemy_repository.py` & `ul-db-utils-3.3.7/ul_db_utils/repository/sqlalchemy_repository.py`

 * *Files identical despite different names*

### Comparing `ul-db-utils-3.3.6/ul_db_utils/search/db_search.py` & `ul-db-utils-3.3.7/ul_db_utils/search/db_search.py`

 * *Files identical despite different names*

### Comparing `ul-db-utils-3.3.6/ul_db_utils/search/doc_db_search.py` & `ul-db-utils-3.3.7/ul_db_utils/search/doc_db_search.py`

 * *Files identical despite different names*

### Comparing `ul-db-utils-3.3.6/ul_db_utils/search/helpers.py` & `ul-db-utils-3.3.7/ul_db_utils/search/helpers.py`

 * *Files identical despite different names*

### Comparing `ul-db-utils-3.3.6/ul_db_utils/utils/ensure/ensure_dict_keys_strict.py` & `ul-db-utils-3.3.7/ul_db_utils/utils/ensure/ensure_dict_keys_strict.py`

 * *Files identical despite different names*

### Comparing `ul-db-utils-3.3.6/ul_db_utils/utils/filter_conversion_doc_db.py` & `ul-db-utils-3.3.7/ul_db_utils/utils/filter_conversion_doc_db.py`

 * *Files identical despite different names*

### Comparing `ul-db-utils-3.3.6/ul_db_utils/utils/get_model_template.py` & `ul-db-utils-3.3.7/ul_db_utils/utils/get_model_template.py`

 * *Files identical despite different names*

### Comparing `ul-db-utils-3.3.6/ul_db_utils/utils/query_soft_delete.py` & `ul-db-utils-3.3.7/ul_db_utils/utils/query_soft_delete.py`

 * *Files identical despite different names*

### Comparing `ul-db-utils-3.3.6/ul_db_utils/utils/waiting_for_mongo.py` & `ul-db-utils-3.3.7/ul_db_utils/utils/waiting_for_mongo.py`

 * *Files identical despite different names*

### Comparing `ul-db-utils-3.3.6/ul_db_utils/utils/waiting_for_postgres.py` & `ul-db-utils-3.3.7/ul_db_utils/utils/waiting_for_postgres.py`

 * *Files identical despite different names*

### Comparing `ul-db-utils-3.3.6/ul_db_utils.egg-info/PKG-INFO` & `ul-db-utils-3.3.7/ul_db_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ul-db-utils
-Version: 3.3.6
+Version: 3.3.7
 Summary: Python ul db utils
 Home-page: https://gitlab.neroelectronics.by/unic-lab/libraries/common-python-utils/db-utils.git
 Author: Unic-lab
 Author-email: 
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ul-db-utils-3.3.6/ul_db_utils.egg-info/SOURCES.txt` & `ul-db-utils-3.3.7/ul_db_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

