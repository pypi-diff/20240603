# Comparing `tmp/nista_library-4.5.0.tar.gz` & `tmp/nista_library-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nista_library-4.5.0.tar", max compression
+gzip compressed data, was "nista_library-5.0.0.tar", max compression
```

## Comparing `nista_library-4.5.0.tar` & `nista_library-5.0.0.tar`

### file list

```diff
@@ -1,126 +1,128 @@
--rw-r--r--   0        0        0     1117 2024-04-26 18:00:31.351168 nista_library-4.5.0/LICENSE.md
--rw-r--r--   0        0        0     6428 2024-04-26 18:00:31.351168 nista_library-4.5.0/README.md
--rw-r--r--   0        0        0      153 2024-04-26 18:00:31.352168 nista_library-4.5.0/data_point_client/__init__.py
--rw-r--r--   0        0        0       47 2024-04-26 18:00:31.353168 nista_library-4.5.0/data_point_client/api/__init__.py
--rw-r--r--   0        0        0        0 2024-04-26 18:00:31.387169 nista_library-4.5.0/data_point_client/api/data_export/__init__.py
--rw-r--r--   0        0        0     5330 2024-04-26 18:00:31.353168 nista_library-4.5.0/data_point_client/api/data_export/data_export_create_csv_export.py
--rw-r--r--   0        0        0        0 2024-04-26 18:00:31.388169 nista_library-4.5.0/data_point_client/api/data_point/__init__.py
--rw-r--r--   0        0        0     6042 2024-04-26 18:00:31.353168 nista_library-4.5.0/data_point_client/api/data_point/data_point_append_execution_result_data.py
--rw-r--r--   0        0        0     5525 2024-04-26 18:00:31.353168 nista_library-4.5.0/data_point_client/api/data_point/data_point_append_time_series_data.py
--rw-r--r--   0        0        0     5441 2024-04-26 18:00:31.353168 nista_library-4.5.0/data_point_client/api/data_point/data_point_create_data_point.py
--rw-r--r--   0        0        0     4868 2024-04-26 18:00:31.353168 nista_library-4.5.0/data_point_client/api/data_point/data_point_delete_data_point.py
--rw-r--r--   0        0        0     4873 2024-04-26 18:00:31.353168 nista_library-4.5.0/data_point_client/api/data_point/data_point_delete_data_point_cleanup_rule.py
--rw-r--r--   0        0        0     6049 2024-04-26 18:00:31.353168 nista_library-4.5.0/data_point_client/api/data_point/data_point_finish_execution_result_data.py
--rw-r--r--   0        0        0     5768 2024-04-26 18:00:31.353168 nista_library-4.5.0/data_point_client/api/data_point/data_point_get_data.py
--rw-r--r--   0        0        0     5301 2024-04-26 18:00:31.353168 nista_library-4.5.0/data_point_client/api/data_point/data_point_get_data_point.py
--rw-r--r--   0        0        0     5622 2024-04-26 18:00:31.353168 nista_library-4.5.0/data_point_client/api/data_point/data_point_get_data_point_by_version.py
--rw-r--r--   0        0        0    10245 2024-04-26 18:00:31.353168 nista_library-4.5.0/data_point_client/api/data_point/data_point_get_data_points.py
--rw-r--r--   0        0        0     5888 2024-04-26 18:00:31.353168 nista_library-4.5.0/data_point_client/api/data_point/data_point_get_data_quality.py
--rw-r--r--   0        0        0     6027 2024-04-26 18:00:31.353168 nista_library-4.5.0/data_point_client/api/data_point/data_point_get_quality_statistic.py
--rw-r--r--   0        0        0     5546 2024-04-26 18:00:31.353168 nista_library-4.5.0/data_point_client/api/data_point/data_point_update_constant_data.py
--rw-r--r--   0        0        0     5442 2024-04-26 18:00:31.353168 nista_library-4.5.0/data_point_client/api/data_point/data_point_update_data_point.py
--rw-r--r--   0        0        0     5518 2024-04-26 18:00:31.353168 nista_library-4.5.0/data_point_client/api/data_point/data_point_update_data_point_cleanup_rule.py
--rw-r--r--   0        0        0     5262 2024-04-26 18:00:31.354168 nista_library-4.5.0/data_point_client/api/data_point/data_point_update_data_point_unit.py
--rw-r--r--   0        0        0     5518 2024-04-26 18:00:31.354168 nista_library-4.5.0/data_point_client/api/data_point/data_point_update_day_period_data.py
--rw-r--r--   0        0        0     5530 2024-04-26 18:00:31.354168 nista_library-4.5.0/data_point_client/api/data_point/data_point_update_time_series_data.py
--rw-r--r--   0        0        0     5530 2024-04-26 18:00:31.354168 nista_library-4.5.0/data_point_client/api/data_point/data_point_update_week_period_data.py
--rw-r--r--   0        0        0        0 2024-04-26 18:00:31.388169 nista_library-4.5.0/data_point_client/api/data_point_area/__init__.py
--rw-r--r--   0        0        0     5768 2024-04-26 18:00:31.354168 nista_library-4.5.0/data_point_client/api/data_point_area/data_point_area_create_area.py
--rw-r--r--   0        0        0     6225 2024-04-26 18:00:31.354168 nista_library-4.5.0/data_point_client/api/data_point_area/data_point_area_create_area_message.py
--rw-r--r--   0        0        0     5184 2024-04-26 18:00:31.354168 nista_library-4.5.0/data_point_client/api/data_point_area/data_point_area_delete_area.py
--rw-r--r--   0        0        0     5563 2024-04-26 18:00:31.354168 nista_library-4.5.0/data_point_client/api/data_point_area/data_point_area_delete_message.py
--rw-r--r--   0        0        0     5592 2024-04-26 18:00:31.354168 nista_library-4.5.0/data_point_client/api/data_point_area/data_point_area_list_areas.py
--rw-r--r--   0        0        0     5769 2024-04-26 18:00:31.354168 nista_library-4.5.0/data_point_client/api/data_point_area/data_point_area_update_area.py
--rw-r--r--   0        0        0     6226 2024-04-26 18:00:31.354168 nista_library-4.5.0/data_point_client/api/data_point_area/data_point_area_update_message.py
--rw-r--r--   0        0        0        0 2024-04-26 18:00:31.388169 nista_library-4.5.0/data_point_client/api/data_point_manual_input/__init__.py
--rw-r--r--   0        0        0     5621 2024-04-26 18:00:31.354168 nista_library-4.5.0/data_point_client/api/data_point_manual_input/data_point_manual_input_append_manual_inputs.py
--rw-r--r--   0        0        0     5413 2024-04-26 18:00:31.354168 nista_library-4.5.0/data_point_client/api/data_point_manual_input/data_point_manual_input_get_manual_inputs.py
--rw-r--r--   0        0        0     5628 2024-04-26 18:00:31.354168 nista_library-4.5.0/data_point_client/api/data_point_manual_input/data_point_manual_input_update_manual_inputs.py
--rw-r--r--   0        0        0        0 2024-04-26 18:00:31.388169 nista_library-4.5.0/data_point_client/api/data_point_tag/__init__.py
--rw-r--r--   0        0        0     7848 2024-04-26 18:00:31.354168 nista_library-4.5.0/data_point_client/api/data_point_tag/data_point_tag_get_tags.py
--rw-r--r--   0        0        0     4954 2024-04-26 18:00:31.354168 nista_library-4.5.0/data_point_client/api/data_point_tag/data_point_tag_get_tags_2.py
--rw-r--r--   0        0        0     2817 2024-04-26 18:00:31.354168 nista_library-4.5.0/data_point_client/client.py
--rw-r--r--   0        0        0      470 2024-04-26 18:00:31.354168 nista_library-4.5.0/data_point_client/errors.py
--rw-r--r--   0        0        0     6078 2024-04-26 18:00:31.354168 nista_library-4.5.0/data_point_client/models/__init__.py
--rw-r--r--   0        0        0     1379 2024-04-26 18:00:31.355168 nista_library-4.5.0/data_point_client/models/append_execution_result_data_request.py
--rw-r--r--   0        0        0     2319 2024-04-26 18:00:31.355168 nista_library-4.5.0/data_point_client/models/append_manual_input_request.py
--rw-r--r--   0        0        0     2976 2024-04-26 18:00:31.355168 nista_library-4.5.0/data_point_client/models/append_time_series_request.py
--rw-r--r--   0        0        0     4359 2024-04-26 18:00:31.355168 nista_library-4.5.0/data_point_client/models/area_of_interest_response.py
--rw-r--r--   0        0        0     1858 2024-04-26 18:00:31.355168 nista_library-4.5.0/data_point_client/models/calculation_origin.py
--rw-r--r--   0        0        0     9207 2024-04-26 18:00:31.355168 nista_library-4.5.0/data_point_client/models/constant_data_bucket.py
--rw-r--r--   0        0        0     2965 2024-04-26 18:00:31.355168 nista_library-4.5.0/data_point_client/models/constant_data_point_data.py
--rw-r--r--   0        0        0     2597 2024-04-26 18:00:31.355168 nista_library-4.5.0/data_point_client/models/continuous_location_rest.py
--rw-r--r--   0        0        0      923 2024-04-26 18:00:31.355168 nista_library-4.5.0/data_point_client/models/create_area_message_request.py
--rw-r--r--   0        0        0     2319 2024-04-26 18:00:31.355168 nista_library-4.5.0/data_point_client/models/create_area_request.py
--rw-r--r--   0        0        0     7534 2024-04-26 18:00:31.355168 nista_library-4.5.0/data_point_client/models/data_bucket_base.py
--rw-r--r--   0        0        0     2054 2024-04-26 18:00:31.355168 nista_library-4.5.0/data_point_client/models/data_export_request.py
--rw-r--r--   0        0        0     2702 2024-04-26 18:00:31.355168 nista_library-4.5.0/data_point_client/models/data_point_comment_message_response.py
--rw-r--r--   0        0        0     2016 2024-04-26 18:00:31.355168 nista_library-4.5.0/data_point_client/models/data_point_data_base.py
--rw-r--r--   0        0        0     2418 2024-04-26 18:00:31.355168 nista_library-4.5.0/data_point_client/models/data_point_data_response.py
--rw-r--r--   0        0        0     1905 2024-04-26 18:00:31.355168 nista_library-4.5.0/data_point_client/models/data_point_info.py
--rw-r--r--   0        0        0     2814 2024-04-26 18:00:31.355168 nista_library-4.5.0/data_point_client/models/data_point_list_response.py
--rw-r--r--   0        0        0     1809 2024-04-26 18:00:31.355168 nista_library-4.5.0/data_point_client/models/data_point_list_response_common_units.py
--rw-r--r--   0        0        0      779 2024-04-26 18:00:31.356168 nista_library-4.5.0/data_point_client/models/data_point_origin.py
--rw-r--r--   0        0        0     4487 2024-04-26 18:00:31.356168 nista_library-4.5.0/data_point_client/models/data_point_request.py
--rw-r--r--   0        0        0    10485 2024-04-26 18:00:31.356168 nista_library-4.5.0/data_point_client/models/data_point_response_base.py
--rw-r--r--   0        0        0     1845 2024-04-26 18:00:31.356168 nista_library-4.5.0/data_point_client/models/date_range_dto.py
--rw-r--r--   0        0        0     7569 2024-04-26 18:00:31.356168 nista_library-4.5.0/data_point_client/models/day_data_by_hour_transfer.py
--rw-r--r--   0        0        0     9224 2024-04-26 18:00:31.356168 nista_library-4.5.0/data_point_client/models/day_period_data_bucket.py
--rw-r--r--   0        0        0     4321 2024-04-26 18:00:31.356168 nista_library-4.5.0/data_point_client/models/day_period_data_point_data.py
--rw-r--r--   0        0        0      191 2024-04-26 18:00:31.356168 nista_library-4.5.0/data_point_client/models/en_area_type_rest.py
--rw-r--r--   0        0        0      192 2024-04-26 18:00:31.356168 nista_library-4.5.0/data_point_client/models/en_data_bucket_state.py
--rw-r--r--   0        0        0      208 2024-04-26 18:00:31.356168 nista_library-4.5.0/data_point_client/models/en_data_point_existence_dto.py
--rw-r--r--   0        0        0      214 2024-04-26 18:00:31.356168 nista_library-4.5.0/data_point_client/models/en_data_point_state_dto.py
--rw-r--r--   0        0        0      192 2024-04-26 18:00:31.356168 nista_library-4.5.0/data_point_client/models/en_data_point_status.py
--rw-r--r--   0        0        0      250 2024-04-26 18:00:31.356168 nista_library-4.5.0/data_point_client/models/en_data_point_type.py
--rw-r--r--   0        0        0      240 2024-04-26 18:00:31.356168 nista_library-4.5.0/data_point_client/models/en_import_options.py
--rw-r--r--   0        0        0      181 2024-04-26 18:00:31.356168 nista_library-4.5.0/data_point_client/models/en_operator.py
--rw-r--r--   0        0        0     2375 2024-04-26 18:00:31.356168 nista_library-4.5.0/data_point_client/models/file_origin.py
--rw-r--r--   0        0        0     2571 2024-04-26 18:00:31.356168 nista_library-4.5.0/data_point_client/models/finish_execution_result_data_request.py
--rw-r--r--   0        0        0     2579 2024-04-26 18:00:31.356168 nista_library-4.5.0/data_point_client/models/get_constant_response.py
--rw-r--r--   0        0        0     2839 2024-04-26 18:00:31.356168 nista_library-4.5.0/data_point_client/models/get_data_quality_request.py
--rw-r--r--   0        0        0     4179 2024-04-26 18:00:31.356168 nista_library-4.5.0/data_point_client/models/get_data_request.py
--rw-r--r--   0        0        0      779 2024-04-26 18:00:31.356168 nista_library-4.5.0/data_point_client/models/get_data_response.py
--rw-r--r--   0        0        0     3900 2024-04-26 18:00:31.356168 nista_library-4.5.0/data_point_client/models/get_day_period_response.py
--rw-r--r--   0        0        0     1922 2024-04-26 18:00:31.356168 nista_library-4.5.0/data_point_client/models/get_quality_response.py
--rw-r--r--   0        0        0     1415 2024-04-26 18:00:31.356168 nista_library-4.5.0/data_point_client/models/get_quality_statistic_response.py
--rw-r--r--   0        0        0     3053 2024-04-26 18:00:31.357168 nista_library-4.5.0/data_point_client/models/get_series_response.py
--rw-r--r--   0        0        0     3227 2024-04-26 18:00:31.357168 nista_library-4.5.0/data_point_client/models/get_week_period_response.py
--rw-r--r--   0        0        0     1176 2024-04-26 18:00:31.357168 nista_library-4.5.0/data_point_client/models/gnista_unit_response.py
--rw-r--r--   0        0        0     1810 2024-04-26 18:00:31.357168 nista_library-4.5.0/data_point_client/models/live_data_origin.py
--rw-r--r--   0        0        0      765 2024-04-26 18:00:31.357168 nista_library-4.5.0/data_point_client/models/location_rest.py
--rw-r--r--   0        0        0     2307 2024-04-26 18:00:31.357168 nista_library-4.5.0/data_point_client/models/manual_input_request.py
--rw-r--r--   0        0        0     2311 2024-04-26 18:00:31.357168 nista_library-4.5.0/data_point_client/models/manual_input_response.py
--rw-r--r--   0        0        0     2045 2024-04-26 18:00:31.357168 nista_library-4.5.0/data_point_client/models/point_location_rest.py
--rw-r--r--   0        0        0     3377 2024-04-26 18:00:31.357168 nista_library-4.5.0/data_point_client/models/problem_details.py
--rw-r--r--   0        0        0     1215 2024-04-26 18:00:31.357168 nista_library-4.5.0/data_point_client/models/problem_details_extensions.py
--rw-r--r--   0        0        0     1449 2024-04-26 18:00:31.357168 nista_library-4.5.0/data_point_client/models/remote_origin.py
--rw-r--r--   0        0        0     1247 2024-04-26 18:00:31.357168 nista_library-4.5.0/data_point_client/models/rule.py
--rw-r--r--   0        0        0    12102 2024-04-26 18:00:31.357168 nista_library-4.5.0/data_point_client/models/series_data_bucket.py
--rw-r--r--   0        0        0     3346 2024-04-26 18:00:31.357168 nista_library-4.5.0/data_point_client/models/series_data_point_data.py
--rw-r--r--   0        0        0     1446 2024-04-26 18:00:31.357168 nista_library-4.5.0/data_point_client/models/sub_series_request.py
--rw-r--r--   0        0        0     1214 2024-04-26 18:00:31.357168 nista_library-4.5.0/data_point_client/models/sub_series_request_values.py
--rw-r--r--   0        0        0     1631 2024-04-26 18:00:31.357168 nista_library-4.5.0/data_point_client/models/time_series_period.py
--rw-r--r--   0        0        0     1529 2024-04-26 18:00:31.357168 nista_library-4.5.0/data_point_client/models/time_series_quality_response.py
--rw-r--r--   0        0        0     1257 2024-04-26 18:00:31.357168 nista_library-4.5.0/data_point_client/models/time_series_quality_response_curve.py
--rw-r--r--   0        0        0     3686 2024-04-26 18:00:31.357168 nista_library-4.5.0/data_point_client/models/time_series_response.py
--rw-r--r--   0        0        0     1219 2024-04-26 18:00:31.357168 nista_library-4.5.0/data_point_client/models/time_series_response_curve.py
--rw-r--r--   0        0        0      923 2024-04-26 18:00:31.357168 nista_library-4.5.0/data_point_client/models/update_area_message_request.py
--rw-r--r--   0        0        0     2674 2024-04-26 18:00:31.357168 nista_library-4.5.0/data_point_client/models/update_area_request.py
--rw-r--r--   0        0        0     1401 2024-04-26 18:00:31.357168 nista_library-4.5.0/data_point_client/models/update_constant_data_request.py
--rw-r--r--   0        0        0     2725 2024-04-26 18:00:31.358168 nista_library-4.5.0/data_point_client/models/update_day_period_request.py
--rw-r--r--   0        0        0     4428 2024-04-26 18:00:31.358168 nista_library-4.5.0/data_point_client/models/update_time_series_request.py
--rw-r--r--   0        0        0     2052 2024-04-26 18:00:31.358168 nista_library-4.5.0/data_point_client/models/update_week_period_request.py
--rw-r--r--   0        0        0     7478 2024-04-26 18:00:31.358168 nista_library-4.5.0/data_point_client/models/week_data_transfere.py
--rw-r--r--   0        0        0     9236 2024-04-26 18:00:31.358168 nista_library-4.5.0/data_point_client/models/week_period_data_bucket.py
--rw-r--r--   0        0        0     3648 2024-04-26 18:00:31.358168 nista_library-4.5.0/data_point_client/models/week_period_data_point_data.py
--rw-r--r--   0        0        0       25 2024-04-26 18:00:31.358168 nista_library-4.5.0/data_point_client/py.typed
--rw-r--r--   0        0        0      993 2024-04-26 18:00:31.358168 nista_library-4.5.0/data_point_client/types.py
--rw-r--r--   0        0        0     1007 2024-04-26 18:00:31.359168 nista_library-4.5.0/nista_library/__init__.py
--rw-r--r--   0        0        0    11406 2024-04-26 18:00:31.359168 nista_library-4.5.0/nista_library/nista_connetion.py
--rw-r--r--   0        0        0     1049 2024-04-26 18:00:31.359168 nista_library-4.5.0/nista_library/nista_credential_manager.py
--rw-r--r--   0        0        0    25077 2024-04-26 18:00:31.359168 nista_library-4.5.0/nista_library/nista_data_point.py
--rw-r--r--   0        0        0     1970 2024-04-26 18:00:31.359168 nista_library-4.5.0/nista_library/nista_data_points.py
--rw-r--r--   0        0        0      835 2024-04-26 18:00:31.359168 nista_library-4.5.0/nista_library/nista_date_range.py
--rw-r--r--   0        0        0     1383 2024-04-26 18:00:31.360168 nista_library-4.5.0/pyproject.toml
--rw-r--r--   0        0        0     7522 1970-01-01 00:00:00.000000 nista_library-4.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1117 2024-06-03 14:57:25.516287 nista_library-5.0.0/LICENSE.md
+-rw-r--r--   0        0        0     6428 2024-06-03 14:57:25.517287 nista_library-5.0.0/README.md
+-rw-r--r--   0        0        0      153 2024-06-03 14:57:25.519287 nista_library-5.0.0/data_point_client/__init__.py
+-rw-r--r--   0        0        0       47 2024-06-03 14:57:25.519287 nista_library-5.0.0/data_point_client/api/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-03 14:57:25.569288 nista_library-5.0.0/data_point_client/api/data_export/__init__.py
+-rw-r--r--   0        0        0     5330 2024-06-03 14:57:25.519287 nista_library-5.0.0/data_point_client/api/data_export/data_export_create_csv_export.py
+-rw-r--r--   0        0        0        0 2024-06-03 14:57:25.570288 nista_library-5.0.0/data_point_client/api/data_point/__init__.py
+-rw-r--r--   0        0        0     6042 2024-06-03 14:57:25.519287 nista_library-5.0.0/data_point_client/api/data_point/data_point_append_execution_result_data.py
+-rw-r--r--   0        0        0     5525 2024-06-03 14:57:25.520287 nista_library-5.0.0/data_point_client/api/data_point/data_point_append_time_series_data.py
+-rw-r--r--   0        0        0     5441 2024-06-03 14:57:25.520287 nista_library-5.0.0/data_point_client/api/data_point/data_point_create_data_point.py
+-rw-r--r--   0        0        0     4868 2024-06-03 14:57:25.520287 nista_library-5.0.0/data_point_client/api/data_point/data_point_delete_data_point.py
+-rw-r--r--   0        0        0     4873 2024-06-03 14:57:25.520287 nista_library-5.0.0/data_point_client/api/data_point/data_point_delete_data_point_cleanup_rule.py
+-rw-r--r--   0        0        0     6049 2024-06-03 14:57:25.520287 nista_library-5.0.0/data_point_client/api/data_point/data_point_finish_execution_result_data.py
+-rw-r--r--   0        0        0     5768 2024-06-03 14:57:25.520287 nista_library-5.0.0/data_point_client/api/data_point/data_point_get_data.py
+-rw-r--r--   0        0        0     5301 2024-06-03 14:57:25.520287 nista_library-5.0.0/data_point_client/api/data_point/data_point_get_data_point.py
+-rw-r--r--   0        0        0     5622 2024-06-03 14:57:25.520287 nista_library-5.0.0/data_point_client/api/data_point/data_point_get_data_point_by_version.py
+-rw-r--r--   0        0        0    10245 2024-06-03 14:57:25.520287 nista_library-5.0.0/data_point_client/api/data_point/data_point_get_data_points.py
+-rw-r--r--   0        0        0     5888 2024-06-03 14:57:25.520287 nista_library-5.0.0/data_point_client/api/data_point/data_point_get_data_quality.py
+-rw-r--r--   0        0        0     6027 2024-06-03 14:57:25.520287 nista_library-5.0.0/data_point_client/api/data_point/data_point_get_quality_statistic.py
+-rw-r--r--   0        0        0     5546 2024-06-03 14:57:25.521287 nista_library-5.0.0/data_point_client/api/data_point/data_point_update_constant_data.py
+-rw-r--r--   0        0        0     5442 2024-06-03 14:57:25.521287 nista_library-5.0.0/data_point_client/api/data_point/data_point_update_data_point.py
+-rw-r--r--   0        0        0     5518 2024-06-03 14:57:25.521287 nista_library-5.0.0/data_point_client/api/data_point/data_point_update_data_point_cleanup_rule.py
+-rw-r--r--   0        0        0     5262 2024-06-03 14:57:25.521287 nista_library-5.0.0/data_point_client/api/data_point/data_point_update_data_point_unit.py
+-rw-r--r--   0        0        0     5518 2024-06-03 14:57:25.521287 nista_library-5.0.0/data_point_client/api/data_point/data_point_update_day_period_data.py
+-rw-r--r--   0        0        0     5530 2024-06-03 14:57:25.521287 nista_library-5.0.0/data_point_client/api/data_point/data_point_update_time_series_data.py
+-rw-r--r--   0        0        0     5530 2024-06-03 14:57:25.521287 nista_library-5.0.0/data_point_client/api/data_point/data_point_update_week_period_data.py
+-rw-r--r--   0        0        0        0 2024-06-03 14:57:25.570288 nista_library-5.0.0/data_point_client/api/data_point_area/__init__.py
+-rw-r--r--   0        0        0     5768 2024-06-03 14:57:25.521287 nista_library-5.0.0/data_point_client/api/data_point_area/data_point_area_create_area.py
+-rw-r--r--   0        0        0     6225 2024-06-03 14:57:25.521287 nista_library-5.0.0/data_point_client/api/data_point_area/data_point_area_create_area_message.py
+-rw-r--r--   0        0        0     5184 2024-06-03 14:57:25.521287 nista_library-5.0.0/data_point_client/api/data_point_area/data_point_area_delete_area.py
+-rw-r--r--   0        0        0     5563 2024-06-03 14:57:25.521287 nista_library-5.0.0/data_point_client/api/data_point_area/data_point_area_delete_message.py
+-rw-r--r--   0        0        0     5592 2024-06-03 14:57:25.521287 nista_library-5.0.0/data_point_client/api/data_point_area/data_point_area_list_areas.py
+-rw-r--r--   0        0        0     5769 2024-06-03 14:57:25.522287 nista_library-5.0.0/data_point_client/api/data_point_area/data_point_area_update_area.py
+-rw-r--r--   0        0        0     6226 2024-06-03 14:57:25.522287 nista_library-5.0.0/data_point_client/api/data_point_area/data_point_area_update_message.py
+-rw-r--r--   0        0        0        0 2024-06-03 14:57:25.570288 nista_library-5.0.0/data_point_client/api/data_point_manual_input/__init__.py
+-rw-r--r--   0        0        0     5621 2024-06-03 14:57:25.522287 nista_library-5.0.0/data_point_client/api/data_point_manual_input/data_point_manual_input_append_manual_inputs.py
+-rw-r--r--   0        0        0     5413 2024-06-03 14:57:25.522287 nista_library-5.0.0/data_point_client/api/data_point_manual_input/data_point_manual_input_get_manual_inputs.py
+-rw-r--r--   0        0        0     5628 2024-06-03 14:57:25.522287 nista_library-5.0.0/data_point_client/api/data_point_manual_input/data_point_manual_input_update_manual_inputs.py
+-rw-r--r--   0        0        0        0 2024-06-03 14:57:25.570288 nista_library-5.0.0/data_point_client/api/data_point_tag/__init__.py
+-rw-r--r--   0        0        0     7848 2024-06-03 14:57:25.522287 nista_library-5.0.0/data_point_client/api/data_point_tag/data_point_tag_get_tags.py
+-rw-r--r--   0        0        0     4954 2024-06-03 14:57:25.522287 nista_library-5.0.0/data_point_client/api/data_point_tag/data_point_tag_get_tags_2.py
+-rw-r--r--   0        0        0     2817 2024-06-03 14:57:25.522287 nista_library-5.0.0/data_point_client/client.py
+-rw-r--r--   0        0        0      470 2024-06-03 14:57:25.522287 nista_library-5.0.0/data_point_client/errors.py
+-rw-r--r--   0        0        0     6231 2024-06-03 14:57:25.524287 nista_library-5.0.0/data_point_client/models/__init__.py
+-rw-r--r--   0        0        0     1379 2024-06-03 14:57:25.524287 nista_library-5.0.0/data_point_client/models/append_execution_result_data_request.py
+-rw-r--r--   0        0        0     2319 2024-06-03 14:57:25.524287 nista_library-5.0.0/data_point_client/models/append_manual_input_request.py
+-rw-r--r--   0        0        0     2976 2024-06-03 14:57:25.524287 nista_library-5.0.0/data_point_client/models/append_time_series_request.py
+-rw-r--r--   0        0        0     4359 2024-06-03 14:57:25.524287 nista_library-5.0.0/data_point_client/models/area_of_interest_response.py
+-rw-r--r--   0        0        0     1858 2024-06-03 14:57:25.524287 nista_library-5.0.0/data_point_client/models/calculation_origin.py
+-rw-r--r--   0        0        0     9207 2024-06-03 14:57:25.524287 nista_library-5.0.0/data_point_client/models/constant_data_bucket.py
+-rw-r--r--   0        0        0     2965 2024-06-03 14:57:25.524287 nista_library-5.0.0/data_point_client/models/constant_data_point_data.py
+-rw-r--r--   0        0        0     2597 2024-06-03 14:57:25.524287 nista_library-5.0.0/data_point_client/models/continuous_location_rest.py
+-rw-r--r--   0        0        0      923 2024-06-03 14:57:25.524287 nista_library-5.0.0/data_point_client/models/create_area_message_request.py
+-rw-r--r--   0        0        0     2319 2024-06-03 14:57:25.524287 nista_library-5.0.0/data_point_client/models/create_area_request.py
+-rw-r--r--   0        0        0     7534 2024-06-03 14:57:25.524287 nista_library-5.0.0/data_point_client/models/data_bucket_base.py
+-rw-r--r--   0        0        0     2054 2024-06-03 14:57:25.524287 nista_library-5.0.0/data_point_client/models/data_export_request.py
+-rw-r--r--   0        0        0     2702 2024-06-03 14:57:25.524287 nista_library-5.0.0/data_point_client/models/data_point_comment_message_response.py
+-rw-r--r--   0        0        0     2016 2024-06-03 14:57:25.524287 nista_library-5.0.0/data_point_client/models/data_point_data_base.py
+-rw-r--r--   0        0        0     2418 2024-06-03 14:57:25.524287 nista_library-5.0.0/data_point_client/models/data_point_data_response.py
+-rw-r--r--   0        0        0     1905 2024-06-03 14:57:25.524287 nista_library-5.0.0/data_point_client/models/data_point_info.py
+-rw-r--r--   0        0        0     2814 2024-06-03 14:57:25.524287 nista_library-5.0.0/data_point_client/models/data_point_list_response.py
+-rw-r--r--   0        0        0     1809 2024-06-03 14:57:25.524287 nista_library-5.0.0/data_point_client/models/data_point_list_response_common_units.py
+-rw-r--r--   0        0        0      779 2024-06-03 14:57:25.524287 nista_library-5.0.0/data_point_client/models/data_point_origin.py
+-rw-r--r--   0        0        0     4487 2024-06-03 14:57:25.524287 nista_library-5.0.0/data_point_client/models/data_point_request.py
+-rw-r--r--   0        0        0    10485 2024-06-03 14:57:25.524287 nista_library-5.0.0/data_point_client/models/data_point_response_base.py
+-rw-r--r--   0        0        0     1845 2024-06-03 14:57:25.524287 nista_library-5.0.0/data_point_client/models/date_range_dto.py
+-rw-r--r--   0        0        0     2193 2024-06-03 14:57:25.525287 nista_library-5.0.0/data_point_client/models/day_data_base_transfer.py
+-rw-r--r--   0        0        0     7569 2024-06-03 14:57:25.525287 nista_library-5.0.0/data_point_client/models/day_data_by_hour_transfer.py
+-rw-r--r--   0        0        0     2421 2024-06-03 14:57:25.525287 nista_library-5.0.0/data_point_client/models/day_data_transfer.py
+-rw-r--r--   0        0        0     9224 2024-06-03 14:57:25.525287 nista_library-5.0.0/data_point_client/models/day_period_data_bucket.py
+-rw-r--r--   0        0        0     4303 2024-06-03 14:57:25.525287 nista_library-5.0.0/data_point_client/models/day_period_data_point_data.py
+-rw-r--r--   0        0        0      191 2024-06-03 14:57:25.525287 nista_library-5.0.0/data_point_client/models/en_area_type_rest.py
+-rw-r--r--   0        0        0      192 2024-06-03 14:57:25.525287 nista_library-5.0.0/data_point_client/models/en_data_bucket_state.py
+-rw-r--r--   0        0        0      208 2024-06-03 14:57:25.525287 nista_library-5.0.0/data_point_client/models/en_data_point_existence_dto.py
+-rw-r--r--   0        0        0      214 2024-06-03 14:57:25.525287 nista_library-5.0.0/data_point_client/models/en_data_point_state_dto.py
+-rw-r--r--   0        0        0      192 2024-06-03 14:57:25.525287 nista_library-5.0.0/data_point_client/models/en_data_point_status.py
+-rw-r--r--   0        0        0      250 2024-06-03 14:57:25.525287 nista_library-5.0.0/data_point_client/models/en_data_point_type.py
+-rw-r--r--   0        0        0      240 2024-06-03 14:57:25.525287 nista_library-5.0.0/data_point_client/models/en_import_options.py
+-rw-r--r--   0        0        0      181 2024-06-03 14:57:25.525287 nista_library-5.0.0/data_point_client/models/en_operator.py
+-rw-r--r--   0        0        0     2375 2024-06-03 14:57:25.525287 nista_library-5.0.0/data_point_client/models/file_origin.py
+-rw-r--r--   0        0        0     2571 2024-06-03 14:57:25.525287 nista_library-5.0.0/data_point_client/models/finish_execution_result_data_request.py
+-rw-r--r--   0        0        0     2579 2024-06-03 14:57:25.525287 nista_library-5.0.0/data_point_client/models/get_constant_response.py
+-rw-r--r--   0        0        0     2839 2024-06-03 14:57:25.526287 nista_library-5.0.0/data_point_client/models/get_data_quality_request.py
+-rw-r--r--   0        0        0     4179 2024-06-03 14:57:25.526287 nista_library-5.0.0/data_point_client/models/get_data_request.py
+-rw-r--r--   0        0        0      779 2024-06-03 14:57:25.526287 nista_library-5.0.0/data_point_client/models/get_data_response.py
+-rw-r--r--   0        0        0     3882 2024-06-03 14:57:25.526287 nista_library-5.0.0/data_point_client/models/get_day_period_response.py
+-rw-r--r--   0        0        0     1922 2024-06-03 14:57:25.526287 nista_library-5.0.0/data_point_client/models/get_quality_response.py
+-rw-r--r--   0        0        0     1415 2024-06-03 14:57:25.526287 nista_library-5.0.0/data_point_client/models/get_quality_statistic_response.py
+-rw-r--r--   0        0        0     3053 2024-06-03 14:57:25.526287 nista_library-5.0.0/data_point_client/models/get_series_response.py
+-rw-r--r--   0        0        0     3227 2024-06-03 14:57:25.526287 nista_library-5.0.0/data_point_client/models/get_week_period_response.py
+-rw-r--r--   0        0        0     1176 2024-06-03 14:57:25.526287 nista_library-5.0.0/data_point_client/models/gnista_unit_response.py
+-rw-r--r--   0        0        0     1810 2024-06-03 14:57:25.526287 nista_library-5.0.0/data_point_client/models/live_data_origin.py
+-rw-r--r--   0        0        0      765 2024-06-03 14:57:25.526287 nista_library-5.0.0/data_point_client/models/location_rest.py
+-rw-r--r--   0        0        0     2307 2024-06-03 14:57:25.526287 nista_library-5.0.0/data_point_client/models/manual_input_request.py
+-rw-r--r--   0        0        0     2311 2024-06-03 14:57:25.527287 nista_library-5.0.0/data_point_client/models/manual_input_response.py
+-rw-r--r--   0        0        0     2045 2024-06-03 14:57:25.527287 nista_library-5.0.0/data_point_client/models/point_location_rest.py
+-rw-r--r--   0        0        0     3377 2024-06-03 14:57:25.527287 nista_library-5.0.0/data_point_client/models/problem_details.py
+-rw-r--r--   0        0        0     1215 2024-06-03 14:57:25.527287 nista_library-5.0.0/data_point_client/models/problem_details_extensions.py
+-rw-r--r--   0        0        0     1449 2024-06-03 14:57:25.527287 nista_library-5.0.0/data_point_client/models/remote_origin.py
+-rw-r--r--   0        0        0     1247 2024-06-03 14:57:25.527287 nista_library-5.0.0/data_point_client/models/rule.py
+-rw-r--r--   0        0        0    12102 2024-06-03 14:57:25.527287 nista_library-5.0.0/data_point_client/models/series_data_bucket.py
+-rw-r--r--   0        0        0     3346 2024-06-03 14:57:25.527287 nista_library-5.0.0/data_point_client/models/series_data_point_data.py
+-rw-r--r--   0        0        0     1446 2024-06-03 14:57:25.527287 nista_library-5.0.0/data_point_client/models/sub_series_request.py
+-rw-r--r--   0        0        0     1214 2024-06-03 14:57:25.527287 nista_library-5.0.0/data_point_client/models/sub_series_request_values.py
+-rw-r--r--   0        0        0     1631 2024-06-03 14:57:25.527287 nista_library-5.0.0/data_point_client/models/time_series_period.py
+-rw-r--r--   0        0        0     1529 2024-06-03 14:57:25.527287 nista_library-5.0.0/data_point_client/models/time_series_quality_response.py
+-rw-r--r--   0        0        0     1257 2024-06-03 14:57:25.527287 nista_library-5.0.0/data_point_client/models/time_series_quality_response_curve.py
+-rw-r--r--   0        0        0     3686 2024-06-03 14:57:25.528287 nista_library-5.0.0/data_point_client/models/time_series_response.py
+-rw-r--r--   0        0        0     1219 2024-06-03 14:57:25.528287 nista_library-5.0.0/data_point_client/models/time_series_response_curve.py
+-rw-r--r--   0        0        0      923 2024-06-03 14:57:25.528287 nista_library-5.0.0/data_point_client/models/update_area_message_request.py
+-rw-r--r--   0        0        0     2674 2024-06-03 14:57:25.528287 nista_library-5.0.0/data_point_client/models/update_area_request.py
+-rw-r--r--   0        0        0     1401 2024-06-03 14:57:25.528287 nista_library-5.0.0/data_point_client/models/update_constant_data_request.py
+-rw-r--r--   0        0        0     2725 2024-06-03 14:57:25.528287 nista_library-5.0.0/data_point_client/models/update_day_period_request.py
+-rw-r--r--   0        0        0     4428 2024-06-03 14:57:25.528287 nista_library-5.0.0/data_point_client/models/update_time_series_request.py
+-rw-r--r--   0        0        0     2052 2024-06-03 14:57:25.528287 nista_library-5.0.0/data_point_client/models/update_week_period_request.py
+-rw-r--r--   0        0        0     7412 2024-06-03 14:57:25.528287 nista_library-5.0.0/data_point_client/models/week_data_transfere.py
+-rw-r--r--   0        0        0     9236 2024-06-03 14:57:25.528287 nista_library-5.0.0/data_point_client/models/week_period_data_bucket.py
+-rw-r--r--   0        0        0     3648 2024-06-03 14:57:25.528287 nista_library-5.0.0/data_point_client/models/week_period_data_point_data.py
+-rw-r--r--   0        0        0       25 2024-06-03 14:57:25.528287 nista_library-5.0.0/data_point_client/py.typed
+-rw-r--r--   0        0        0      993 2024-06-03 14:57:25.528287 nista_library-5.0.0/data_point_client/types.py
+-rw-r--r--   0        0        0     1007 2024-06-03 14:57:25.530287 nista_library-5.0.0/nista_library/__init__.py
+-rw-r--r--   0        0        0    11406 2024-06-03 14:57:25.530287 nista_library-5.0.0/nista_library/nista_connetion.py
+-rw-r--r--   0        0        0     1049 2024-06-03 14:57:25.530287 nista_library-5.0.0/nista_library/nista_credential_manager.py
+-rw-r--r--   0        0        0    25070 2024-06-03 14:57:25.531287 nista_library-5.0.0/nista_library/nista_data_point.py
+-rw-r--r--   0        0        0     1970 2024-06-03 14:57:25.531287 nista_library-5.0.0/nista_library/nista_data_points.py
+-rw-r--r--   0        0        0      835 2024-06-03 14:57:25.531287 nista_library-5.0.0/nista_library/nista_date_range.py
+-rw-r--r--   0        0        0     1383 2024-06-03 14:57:25.532287 nista_library-5.0.0/pyproject.toml
+-rw-r--r--   0        0        0     7522 1970-01-01 00:00:00.000000 nista_library-5.0.0/PKG-INFO
```

### Comparing `nista_library-4.5.0/LICENSE.md` & `nista_library-5.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/README.md` & `nista_library-5.0.0/README.md`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/api/data_export/data_export_create_csv_export.py` & `nista_library-5.0.0/data_point_client/api/data_export/data_export_create_csv_export.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/api/data_point/data_point_append_execution_result_data.py` & `nista_library-5.0.0/data_point_client/api/data_point/data_point_append_execution_result_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/api/data_point/data_point_append_time_series_data.py` & `nista_library-5.0.0/data_point_client/api/data_point/data_point_append_time_series_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/api/data_point/data_point_create_data_point.py` & `nista_library-5.0.0/data_point_client/api/data_point/data_point_create_data_point.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/api/data_point/data_point_delete_data_point.py` & `nista_library-5.0.0/data_point_client/api/data_point/data_point_delete_data_point.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/api/data_point/data_point_delete_data_point_cleanup_rule.py` & `nista_library-5.0.0/data_point_client/api/data_point/data_point_delete_data_point_cleanup_rule.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/api/data_point/data_point_finish_execution_result_data.py` & `nista_library-5.0.0/data_point_client/api/data_point/data_point_finish_execution_result_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/api/data_point/data_point_get_data.py` & `nista_library-5.0.0/data_point_client/api/data_point/data_point_get_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/api/data_point/data_point_get_data_point.py` & `nista_library-5.0.0/data_point_client/api/data_point/data_point_get_data_point.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/api/data_point/data_point_get_data_point_by_version.py` & `nista_library-5.0.0/data_point_client/api/data_point/data_point_get_data_point_by_version.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/api/data_point/data_point_get_data_points.py` & `nista_library-5.0.0/data_point_client/api/data_point/data_point_get_data_points.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/api/data_point/data_point_get_data_quality.py` & `nista_library-5.0.0/data_point_client/api/data_point/data_point_get_data_quality.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/api/data_point/data_point_get_quality_statistic.py` & `nista_library-5.0.0/data_point_client/api/data_point/data_point_get_quality_statistic.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/api/data_point/data_point_update_constant_data.py` & `nista_library-5.0.0/data_point_client/api/data_point/data_point_update_constant_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/api/data_point/data_point_update_data_point.py` & `nista_library-5.0.0/data_point_client/api/data_point/data_point_update_data_point.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/api/data_point/data_point_update_data_point_cleanup_rule.py` & `nista_library-5.0.0/data_point_client/api/data_point/data_point_update_data_point_cleanup_rule.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/api/data_point/data_point_update_data_point_unit.py` & `nista_library-5.0.0/data_point_client/api/data_point/data_point_update_data_point_unit.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/api/data_point/data_point_update_day_period_data.py` & `nista_library-5.0.0/data_point_client/api/data_point/data_point_update_day_period_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/api/data_point/data_point_update_time_series_data.py` & `nista_library-5.0.0/data_point_client/api/data_point/data_point_update_time_series_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/api/data_point/data_point_update_week_period_data.py` & `nista_library-5.0.0/data_point_client/api/data_point/data_point_update_week_period_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/api/data_point_area/data_point_area_create_area.py` & `nista_library-5.0.0/data_point_client/api/data_point_area/data_point_area_create_area.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/api/data_point_area/data_point_area_create_area_message.py` & `nista_library-5.0.0/data_point_client/api/data_point_area/data_point_area_create_area_message.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/api/data_point_area/data_point_area_delete_area.py` & `nista_library-5.0.0/data_point_client/api/data_point_area/data_point_area_delete_area.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/api/data_point_area/data_point_area_delete_message.py` & `nista_library-5.0.0/data_point_client/api/data_point_area/data_point_area_delete_message.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/api/data_point_area/data_point_area_list_areas.py` & `nista_library-5.0.0/data_point_client/api/data_point_area/data_point_area_list_areas.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/api/data_point_area/data_point_area_update_area.py` & `nista_library-5.0.0/data_point_client/api/data_point_area/data_point_area_update_area.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/api/data_point_area/data_point_area_update_message.py` & `nista_library-5.0.0/data_point_client/api/data_point_area/data_point_area_update_message.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/api/data_point_manual_input/data_point_manual_input_append_manual_inputs.py` & `nista_library-5.0.0/data_point_client/api/data_point_manual_input/data_point_manual_input_append_manual_inputs.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/api/data_point_manual_input/data_point_manual_input_get_manual_inputs.py` & `nista_library-5.0.0/data_point_client/api/data_point_manual_input/data_point_manual_input_get_manual_inputs.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/api/data_point_manual_input/data_point_manual_input_update_manual_inputs.py` & `nista_library-5.0.0/data_point_client/api/data_point_manual_input/data_point_manual_input_update_manual_inputs.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/api/data_point_tag/data_point_tag_get_tags.py` & `nista_library-5.0.0/data_point_client/api/data_point_tag/data_point_tag_get_tags.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/api/data_point_tag/data_point_tag_get_tags_2.py` & `nista_library-5.0.0/data_point_client/api/data_point_tag/data_point_tag_get_tags_2.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/client.py` & `nista_library-5.0.0/data_point_client/client.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/models/__init__.py` & `nista_library-5.0.0/data_point_client/models/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,17 @@
 from .data_point_info import DataPointInfo
 from .data_point_list_response import DataPointListResponse
 from .data_point_list_response_common_units import DataPointListResponseCommonUnits
 from .data_point_origin import DataPointOrigin
 from .data_point_request import DataPointRequest
 from .data_point_response_base import DataPointResponseBase
 from .date_range_dto import DateRangeDTO
+from .day_data_base_transfer import DayDataBaseTransfer
 from .day_data_by_hour_transfer import DayDataByHourTransfer
+from .day_data_transfer import DayDataTransfer
 from .day_period_data_bucket import DayPeriodDataBucket
 from .day_period_data_point_data import DayPeriodDataPointData
 from .en_area_type_rest import EnAreaTypeRest
 from .en_data_bucket_state import EnDataBucketState
 from .en_data_point_existence_dto import EnDataPointExistenceDTO
 from .en_data_point_state_dto import EnDataPointStateDTO
 from .en_data_point_status import EnDataPointStatus
@@ -92,15 +94,17 @@
     "DataPointInfo",
     "DataPointListResponse",
     "DataPointListResponseCommonUnits",
     "DataPointOrigin",
     "DataPointRequest",
     "DataPointResponseBase",
     "DateRangeDTO",
+    "DayDataBaseTransfer",
     "DayDataByHourTransfer",
+    "DayDataTransfer",
     "DayPeriodDataBucket",
     "DayPeriodDataPointData",
     "EnAreaTypeRest",
     "EnDataBucketState",
     "EnDataPointExistenceDTO",
     "EnDataPointStateDTO",
     "EnDataPointStatus",
```

### Comparing `nista_library-4.5.0/data_point_client/models/append_execution_result_data_request.py` & `nista_library-5.0.0/data_point_client/models/append_execution_result_data_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/models/append_manual_input_request.py` & `nista_library-5.0.0/data_point_client/models/append_manual_input_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/models/append_time_series_request.py` & `nista_library-5.0.0/data_point_client/models/append_time_series_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/models/area_of_interest_response.py` & `nista_library-5.0.0/data_point_client/models/area_of_interest_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/models/calculation_origin.py` & `nista_library-5.0.0/data_point_client/models/calculation_origin.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/models/constant_data_bucket.py` & `nista_library-5.0.0/data_point_client/models/constant_data_bucket.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/models/constant_data_point_data.py` & `nista_library-5.0.0/data_point_client/models/constant_data_point_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/models/continuous_location_rest.py` & `nista_library-5.0.0/data_point_client/models/continuous_location_rest.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/models/create_area_message_request.py` & `nista_library-5.0.0/data_point_client/models/create_area_message_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/models/create_area_request.py` & `nista_library-5.0.0/data_point_client/models/create_area_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/models/data_bucket_base.py` & `nista_library-5.0.0/data_point_client/models/data_bucket_base.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/models/data_export_request.py` & `nista_library-5.0.0/data_point_client/models/data_export_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/models/data_point_comment_message_response.py` & `nista_library-5.0.0/data_point_client/models/data_point_comment_message_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/models/data_point_data_base.py` & `nista_library-5.0.0/data_point_client/models/data_point_data_base.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/models/data_point_data_response.py` & `nista_library-5.0.0/data_point_client/models/data_point_data_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/models/data_point_info.py` & `nista_library-5.0.0/data_point_client/models/data_point_info.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/models/data_point_list_response.py` & `nista_library-5.0.0/data_point_client/models/data_point_list_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/models/data_point_list_response_common_units.py` & `nista_library-5.0.0/data_point_client/models/data_point_list_response_common_units.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/models/data_point_origin.py` & `nista_library-5.0.0/data_point_client/models/data_point_origin.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/models/data_point_request.py` & `nista_library-5.0.0/data_point_client/models/data_point_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/models/data_point_response_base.py` & `nista_library-5.0.0/data_point_client/models/data_point_response_base.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/models/date_range_dto.py` & `nista_library-5.0.0/data_point_client/models/date_range_dto.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/models/day_data_by_hour_transfer.py` & `nista_library-5.0.0/data_point_client/models/day_data_by_hour_transfer.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/models/day_period_data_bucket.py` & `nista_library-5.0.0/data_point_client/models/day_period_data_bucket.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/models/day_period_data_point_data.py` & `nista_library-5.0.0/data_point_client/models/day_period_data_point_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,39 +3,39 @@
 
 import attr
 from dateutil.parser import isoparse
 
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
-    from ..models.day_data_by_hour_transfer import DayDataByHourTransfer
+    from ..models.day_data_base_transfer import DayDataBaseTransfer
 
 
 T = TypeVar("T", bound="DayPeriodDataPointData")
 
 
 @attr.s(auto_attribs=True)
 class DayPeriodDataPointData:
     """
     Attributes:
         discriminator (str):
         status (Union[Unset, None, str]):
         error_message (Union[Unset, None, str]):
         unit (Union[Unset, None, str]):
         number_of_entries (Union[Unset, int]):
-        day_data (Union[Unset, None, DayDataByHourTransfer]):
+        day_data (Union[Unset, None, DayDataBaseTransfer]):
         date (Union[Unset, None, datetime.datetime]):
     """
 
     discriminator: str
     status: Union[Unset, None, str] = UNSET
     error_message: Union[Unset, None, str] = UNSET
     unit: Union[Unset, None, str] = UNSET
     number_of_entries: Union[Unset, int] = UNSET
-    day_data: Union[Unset, None, "DayDataByHourTransfer"] = UNSET
+    day_data: Union[Unset, None, "DayDataBaseTransfer"] = UNSET
     date: Union[Unset, None, datetime.datetime] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         discriminator = self.discriminator
         status = self.status
         error_message = self.error_message
@@ -69,35 +69,35 @@
         if date is not UNSET:
             field_dict["date"] = date
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.day_data_by_hour_transfer import DayDataByHourTransfer
+        from ..models.day_data_base_transfer import DayDataBaseTransfer
 
         d = src_dict.copy()
         discriminator = d.pop("discriminator")
 
         status = d.pop("status", UNSET)
 
         error_message = d.pop("errorMessage", UNSET)
 
         unit = d.pop("unit", UNSET)
 
         number_of_entries = d.pop("numberOfEntries", UNSET)
 
         _day_data = d.pop("dayData", UNSET)
-        day_data: Union[Unset, None, DayDataByHourTransfer]
+        day_data: Union[Unset, None, DayDataBaseTransfer]
         if _day_data is None:
             day_data = None
         elif isinstance(_day_data, Unset):
             day_data = UNSET
         else:
-            day_data = DayDataByHourTransfer.from_dict(_day_data)
+            day_data = DayDataBaseTransfer.from_dict(_day_data)
 
         _date = d.pop("date", UNSET)
         date: Union[Unset, None, datetime.datetime]
         if _date is None:
             date = None
         elif isinstance(_date, Unset):
             date = UNSET
```

### Comparing `nista_library-4.5.0/data_point_client/models/file_origin.py` & `nista_library-5.0.0/data_point_client/models/file_origin.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/models/finish_execution_result_data_request.py` & `nista_library-5.0.0/data_point_client/models/finish_execution_result_data_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/models/get_constant_response.py` & `nista_library-5.0.0/data_point_client/models/get_constant_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/models/get_data_quality_request.py` & `nista_library-5.0.0/data_point_client/models/get_data_quality_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/models/get_data_request.py` & `nista_library-5.0.0/data_point_client/models/get_data_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/models/get_data_response.py` & `nista_library-5.0.0/data_point_client/models/get_data_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/models/get_day_period_response.py` & `nista_library-5.0.0/data_point_client/models/get_day_period_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,33 +3,33 @@
 
 import attr
 from dateutil.parser import isoparse
 
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
-    from ..models.day_data_by_hour_transfer import DayDataByHourTransfer
+    from ..models.day_data_base_transfer import DayDataBaseTransfer
     from ..models.gnista_unit_response import GnistaUnitResponse
 
 
 T = TypeVar("T", bound="GetDayPeriodResponse")
 
 
 @attr.s(auto_attribs=True)
 class GetDayPeriodResponse:
     """
     Attributes:
         discriminator (str):
-        day_data (Union[Unset, None, DayDataByHourTransfer]):
+        day_data (Union[Unset, None, DayDataBaseTransfer]):
         date (Union[Unset, None, datetime.datetime]):
         unit (Union[Unset, None, GnistaUnitResponse]):
     """
 
     discriminator: str
-    day_data: Union[Unset, None, "DayDataByHourTransfer"] = UNSET
+    day_data: Union[Unset, None, "DayDataBaseTransfer"] = UNSET
     date: Union[Unset, None, datetime.datetime] = UNSET
     unit: Union[Unset, None, "GnistaUnitResponse"] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         discriminator = self.discriminator
         day_data: Union[Unset, None, Dict[str, Any]] = UNSET
@@ -58,28 +58,28 @@
         if unit is not UNSET:
             field_dict["unit"] = unit
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.day_data_by_hour_transfer import DayDataByHourTransfer
+        from ..models.day_data_base_transfer import DayDataBaseTransfer
         from ..models.gnista_unit_response import GnistaUnitResponse
 
         d = src_dict.copy()
         discriminator = d.pop("discriminator")
 
         _day_data = d.pop("dayData", UNSET)
-        day_data: Union[Unset, None, DayDataByHourTransfer]
+        day_data: Union[Unset, None, DayDataBaseTransfer]
         if _day_data is None:
             day_data = None
         elif isinstance(_day_data, Unset):
             day_data = UNSET
         else:
-            day_data = DayDataByHourTransfer.from_dict(_day_data)
+            day_data = DayDataBaseTransfer.from_dict(_day_data)
 
         _date = d.pop("date", UNSET)
         date: Union[Unset, None, datetime.datetime]
         if _date is None:
             date = None
         elif isinstance(_date, Unset):
             date = UNSET
```

### Comparing `nista_library-4.5.0/data_point_client/models/get_quality_response.py` & `nista_library-5.0.0/data_point_client/models/get_quality_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/models/get_quality_statistic_response.py` & `nista_library-5.0.0/data_point_client/models/get_quality_statistic_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/models/get_series_response.py` & `nista_library-5.0.0/data_point_client/models/get_series_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/models/get_week_period_response.py` & `nista_library-5.0.0/data_point_client/models/get_week_period_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/models/gnista_unit_response.py` & `nista_library-5.0.0/data_point_client/models/gnista_unit_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/models/live_data_origin.py` & `nista_library-5.0.0/data_point_client/models/live_data_origin.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/models/location_rest.py` & `nista_library-5.0.0/data_point_client/models/location_rest.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/models/manual_input_request.py` & `nista_library-5.0.0/data_point_client/models/manual_input_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/models/manual_input_response.py` & `nista_library-5.0.0/data_point_client/models/manual_input_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/models/point_location_rest.py` & `nista_library-5.0.0/data_point_client/models/point_location_rest.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/models/problem_details.py` & `nista_library-5.0.0/data_point_client/models/problem_details.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/models/problem_details_extensions.py` & `nista_library-5.0.0/data_point_client/models/problem_details_extensions.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/models/remote_origin.py` & `nista_library-5.0.0/data_point_client/models/remote_origin.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/models/rule.py` & `nista_library-5.0.0/data_point_client/models/rule.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/models/series_data_bucket.py` & `nista_library-5.0.0/data_point_client/models/series_data_bucket.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/models/series_data_point_data.py` & `nista_library-5.0.0/data_point_client/models/series_data_point_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/models/sub_series_request.py` & `nista_library-5.0.0/data_point_client/models/sub_series_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/models/sub_series_request_values.py` & `nista_library-5.0.0/data_point_client/models/sub_series_request_values.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/models/time_series_period.py` & `nista_library-5.0.0/data_point_client/models/time_series_period.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/models/time_series_quality_response.py` & `nista_library-5.0.0/data_point_client/models/time_series_quality_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/models/time_series_quality_response_curve.py` & `nista_library-5.0.0/data_point_client/models/time_series_quality_response_curve.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/models/time_series_response.py` & `nista_library-5.0.0/data_point_client/models/time_series_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/models/time_series_response_curve.py` & `nista_library-5.0.0/data_point_client/models/time_series_response_curve.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/models/update_area_message_request.py` & `nista_library-5.0.0/data_point_client/models/update_area_message_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/models/update_area_request.py` & `nista_library-5.0.0/data_point_client/models/update_area_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/models/update_constant_data_request.py` & `nista_library-5.0.0/data_point_client/models/update_constant_data_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/models/update_day_period_request.py` & `nista_library-5.0.0/data_point_client/models/update_day_period_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/models/update_time_series_request.py` & `nista_library-5.0.0/data_point_client/models/update_time_series_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/models/update_week_period_request.py` & `nista_library-5.0.0/data_point_client/models/update_week_period_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/models/week_data_transfere.py` & `nista_library-5.0.0/data_point_client/models/week_data_transfere.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
-    from ..models.day_data_by_hour_transfer import DayDataByHourTransfer
+    from ..models.day_data_base_transfer import DayDataBaseTransfer
 
 
 T = TypeVar("T", bound="WeekDataTransfere")
 
 
 @attr.s(auto_attribs=True)
 class WeekDataTransfere:
     """
     Attributes:
         discriminator (str):
-        monday_data (Union[Unset, None, DayDataByHourTransfer]):
-        tuesday_data (Union[Unset, None, DayDataByHourTransfer]):
-        wednesday_data (Union[Unset, None, DayDataByHourTransfer]):
-        thursday_data (Union[Unset, None, DayDataByHourTransfer]):
-        friday_data (Union[Unset, None, DayDataByHourTransfer]):
-        saturday_data (Union[Unset, None, DayDataByHourTransfer]):
-        sunday_data (Union[Unset, None, DayDataByHourTransfer]):
+        monday_data (Union[Unset, None, DayDataBaseTransfer]):
+        tuesday_data (Union[Unset, None, DayDataBaseTransfer]):
+        wednesday_data (Union[Unset, None, DayDataBaseTransfer]):
+        thursday_data (Union[Unset, None, DayDataBaseTransfer]):
+        friday_data (Union[Unset, None, DayDataBaseTransfer]):
+        saturday_data (Union[Unset, None, DayDataBaseTransfer]):
+        sunday_data (Union[Unset, None, DayDataBaseTransfer]):
     """
 
     discriminator: str
-    monday_data: Union[Unset, None, "DayDataByHourTransfer"] = UNSET
-    tuesday_data: Union[Unset, None, "DayDataByHourTransfer"] = UNSET
-    wednesday_data: Union[Unset, None, "DayDataByHourTransfer"] = UNSET
-    thursday_data: Union[Unset, None, "DayDataByHourTransfer"] = UNSET
-    friday_data: Union[Unset, None, "DayDataByHourTransfer"] = UNSET
-    saturday_data: Union[Unset, None, "DayDataByHourTransfer"] = UNSET
-    sunday_data: Union[Unset, None, "DayDataByHourTransfer"] = UNSET
+    monday_data: Union[Unset, None, "DayDataBaseTransfer"] = UNSET
+    tuesday_data: Union[Unset, None, "DayDataBaseTransfer"] = UNSET
+    wednesday_data: Union[Unset, None, "DayDataBaseTransfer"] = UNSET
+    thursday_data: Union[Unset, None, "DayDataBaseTransfer"] = UNSET
+    friday_data: Union[Unset, None, "DayDataBaseTransfer"] = UNSET
+    saturday_data: Union[Unset, None, "DayDataBaseTransfer"] = UNSET
+    sunday_data: Union[Unset, None, "DayDataBaseTransfer"] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         discriminator = self.discriminator
         monday_data: Union[Unset, None, Dict[str, Any]] = UNSET
         if not isinstance(self.monday_data, Unset):
             monday_data = self.monday_data.to_dict() if self.monday_data else None
@@ -87,81 +87,81 @@
         if sunday_data is not UNSET:
             field_dict["sundayData"] = sunday_data
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.day_data_by_hour_transfer import DayDataByHourTransfer
+        from ..models.day_data_base_transfer import DayDataBaseTransfer
 
         d = src_dict.copy()
         discriminator = d.pop("discriminator")
 
         _monday_data = d.pop("mondayData", UNSET)
-        monday_data: Union[Unset, None, DayDataByHourTransfer]
+        monday_data: Union[Unset, None, DayDataBaseTransfer]
         if _monday_data is None:
             monday_data = None
         elif isinstance(_monday_data, Unset):
             monday_data = UNSET
         else:
-            monday_data = DayDataByHourTransfer.from_dict(_monday_data)
+            monday_data = DayDataBaseTransfer.from_dict(_monday_data)
 
         _tuesday_data = d.pop("tuesdayData", UNSET)
-        tuesday_data: Union[Unset, None, DayDataByHourTransfer]
+        tuesday_data: Union[Unset, None, DayDataBaseTransfer]
         if _tuesday_data is None:
             tuesday_data = None
         elif isinstance(_tuesday_data, Unset):
             tuesday_data = UNSET
         else:
-            tuesday_data = DayDataByHourTransfer.from_dict(_tuesday_data)
+            tuesday_data = DayDataBaseTransfer.from_dict(_tuesday_data)
 
         _wednesday_data = d.pop("wednesdayData", UNSET)
-        wednesday_data: Union[Unset, None, DayDataByHourTransfer]
+        wednesday_data: Union[Unset, None, DayDataBaseTransfer]
         if _wednesday_data is None:
             wednesday_data = None
         elif isinstance(_wednesday_data, Unset):
             wednesday_data = UNSET
         else:
-            wednesday_data = DayDataByHourTransfer.from_dict(_wednesday_data)
+            wednesday_data = DayDataBaseTransfer.from_dict(_wednesday_data)
 
         _thursday_data = d.pop("thursdayData", UNSET)
-        thursday_data: Union[Unset, None, DayDataByHourTransfer]
+        thursday_data: Union[Unset, None, DayDataBaseTransfer]
         if _thursday_data is None:
             thursday_data = None
         elif isinstance(_thursday_data, Unset):
             thursday_data = UNSET
         else:
-            thursday_data = DayDataByHourTransfer.from_dict(_thursday_data)
+            thursday_data = DayDataBaseTransfer.from_dict(_thursday_data)
 
         _friday_data = d.pop("fridayData", UNSET)
-        friday_data: Union[Unset, None, DayDataByHourTransfer]
+        friday_data: Union[Unset, None, DayDataBaseTransfer]
         if _friday_data is None:
             friday_data = None
         elif isinstance(_friday_data, Unset):
             friday_data = UNSET
         else:
-            friday_data = DayDataByHourTransfer.from_dict(_friday_data)
+            friday_data = DayDataBaseTransfer.from_dict(_friday_data)
 
         _saturday_data = d.pop("saturdayData", UNSET)
-        saturday_data: Union[Unset, None, DayDataByHourTransfer]
+        saturday_data: Union[Unset, None, DayDataBaseTransfer]
         if _saturday_data is None:
             saturday_data = None
         elif isinstance(_saturday_data, Unset):
             saturday_data = UNSET
         else:
-            saturday_data = DayDataByHourTransfer.from_dict(_saturday_data)
+            saturday_data = DayDataBaseTransfer.from_dict(_saturday_data)
 
         _sunday_data = d.pop("sundayData", UNSET)
-        sunday_data: Union[Unset, None, DayDataByHourTransfer]
+        sunday_data: Union[Unset, None, DayDataBaseTransfer]
         if _sunday_data is None:
             sunday_data = None
         elif isinstance(_sunday_data, Unset):
             sunday_data = UNSET
         else:
-            sunday_data = DayDataByHourTransfer.from_dict(_sunday_data)
+            sunday_data = DayDataBaseTransfer.from_dict(_sunday_data)
 
         week_data_transfere = cls(
             discriminator=discriminator,
             monday_data=monday_data,
             tuesday_data=tuesday_data,
             wednesday_data=wednesday_data,
             thursday_data=thursday_data,
```

### Comparing `nista_library-4.5.0/data_point_client/models/week_period_data_bucket.py` & `nista_library-5.0.0/data_point_client/models/week_period_data_bucket.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/models/week_period_data_point_data.py` & `nista_library-5.0.0/data_point_client/models/week_period_data_point_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/data_point_client/types.py` & `nista_library-5.0.0/data_point_client/types.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/nista_library/__init__.py` & `nista_library-5.0.0/nista_library/__init__.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/nista_library/nista_connetion.py` & `nista_library-5.0.0/nista_library/nista_connetion.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/nista_library/nista_credential_manager.py` & `nista_library-5.0.0/nista_library/nista_credential_manager.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/nista_library/nista_data_point.py` & `nista_library-5.0.0/nista_library/nista_data_point.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from data_point_client.models.append_execution_result_data_request import (
     AppendExecutionResultDataRequest,
 )
 from data_point_client.models.append_time_series_request import AppendTimeSeriesRequest
 from data_point_client.models.constant_data_bucket import ConstantDataBucket
 from data_point_client.models.data_point_request import DataPointRequest
 from data_point_client.models.data_point_response_base import DataPointResponseBase
-from data_point_client.models.day_data_by_hour_transfer import DayDataByHourTransfer
+from data_point_client.models.day_data_base_transfer import DayDataBaseTransfer
 from data_point_client.models.day_period_data_bucket import DayPeriodDataBucket
 from data_point_client.models.en_data_point_existence_dto import EnDataPointExistenceDTO
 from data_point_client.models.finish_execution_result_data_request import FinishExecutionResultDataRequest
 from data_point_client.models.get_data_quality_request import GetDataQualityRequest
 from data_point_client.models.get_data_request import GetDataRequest
 from data_point_client.models.get_day_period_response import GetDayPeriodResponse
 from data_point_client.models.get_quality_statistic_response import GetQualityStatisticResponse
@@ -311,15 +311,15 @@
     # pylint: disable=too-many-arguments
     # pylint: disable=too-many-branches
     def get_data_point_data(
         self,
         request: GetDataRequest,
         post_fix: bool = False,
         timeout: float = 30,
-    ) -> Union[List[DataFrame], float, Unset, WeekDataTransfere, DayDataByHourTransfer, None]:
+    ) -> Union[List[DataFrame], float, Unset, WeekDataTransfere, DayDataBaseTransfer, None]:
         """Retrieves the Data from a DataPoint
         :param request: Request details for retrieving Data
         :param post_fix: Append nista.io instance name after DataPoint Name
         :param timeout: How long to wait for response
         :return: The DataPoint Data
         """
```

### Comparing `nista_library-4.5.0/nista_library/nista_data_points.py` & `nista_library-5.0.0/nista_library/nista_data_points.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/nista_library/nista_date_range.py` & `nista_library-5.0.0/nista_library/nista_date_range.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.5.0/pyproject.toml` & `nista_library-5.0.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nista-library"
-version = "4.5.0"
+version = "5.0.0"
 description = "A client library for accessing nista.io"
 license = "MIT"
 
 authors = ["Markus Hoffmann <markus.hoffmann@nista.io>"]
 
 readme = "README.md"
 homepage = "https://nista.io"
```

### Comparing `nista_library-4.5.0/PKG-INFO` & `nista_library-5.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nista-library
-Version: 4.5.0
+Version: 5.0.0
 Summary: A client library for accessing nista.io
 Home-page: https://nista.io
 License: MIT
 Author: Markus Hoffmann
 Author-email: markus.hoffmann@nista.io
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

