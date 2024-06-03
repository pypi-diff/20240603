# Comparing `tmp/akride-0.4.16-py3-none-any.whl.zip` & `tmp/akride-0.4.23-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,77 +1,98 @@
-Zip file size: 74166 bytes, number of entries: 75
--rw-r--r--  2.0 unx     2119 b- defN 24-May-13 06:03 akride/__init__.py
--rw-r--r--  2.0 unx     2499 b- defN 24-May-13 06:03 akride/background_task_manager.py
--rw-r--r--  2.0 unx    35983 b- defN 24-May-13 06:03 akride/client.py
--rw-r--r--  2.0 unx     2563 b- defN 24-May-13 06:03 akride/main.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-13 06:03 akride/_utils/__init__.py
--rw-r--r--  2.0 unx     2904 b- defN 24-May-13 06:03 akride/_utils/background_task_helper.py
--rw-r--r--  2.0 unx     1357 b- defN 24-May-13 06:03 akride/_utils/class_executor.py
--rw-r--r--  2.0 unx     2624 b- defN 24-May-13 06:03 akride/_utils/exception_utils.py
--rw-r--r--  2.0 unx      584 b- defN 24-May-13 06:03 akride/_utils/file_utils.py
--rw-r--r--  2.0 unx    14188 b- defN 24-May-13 06:03 akride/_utils/job_creator.py
--rw-r--r--  2.0 unx      278 b- defN 24-May-13 06:03 akride/_utils/platform.py
--rw-r--r--  2.0 unx      454 b- defN 24-May-13 06:03 akride/_utils/progress_bar_helper.py
--rw-r--r--  2.0 unx     1459 b- defN 24-May-13 06:03 akride/_utils/proxy_utils.py
--rw-r--r--  2.0 unx      172 b- defN 24-May-13 06:03 akride/_utils/resource_utils.py
--rw-r--r--  2.0 unx      595 b- defN 24-May-13 06:03 akride/_utils/retry_helper.py
--rw-r--r--  2.0 unx      811 b- defN 24-May-13 06:03 akride/_utils/store_utils.py
--rw-r--r--  2.0 unx      473 b- defN 24-May-13 06:03 akride/_utils/workflow_helper.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-13 06:03 akride/_utils/catalog/__init__.py
--rw-r--r--  2.0 unx      779 b- defN 24-May-13 06:03 akride/_utils/catalog/catalog_tables_helper.py
--rw-r--r--  2.0 unx      574 b- defN 24-May-13 06:03 akride/_utils/catalog/dataset_tables_info.py
--rw-r--r--  2.0 unx      194 b- defN 24-May-13 06:03 akride/_utils/catalog/enums.py
--rw-r--r--  2.0 unx      890 b- defN 24-May-13 06:03 akride/_utils/catalog/pipeline_tables_info.py
--rw-r--r--  2.0 unx      541 b- defN 24-May-13 06:03 akride/_utils/catalog/tables_info.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-13 06:03 akride/_utils/pipeline/__init__.py
--rw-r--r--  2.0 unx      250 b- defN 24-May-13 06:03 akride/_utils/pipeline/constants.py
--rw-r--r--  2.0 unx     1159 b- defN 24-May-13 06:03 akride/_utils/pipeline/pipeline_helper.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-13 06:03 akride/_utils/progress_manager/__init__.py
--rw-r--r--  2.0 unx     2037 b- defN 24-May-13 06:03 akride/_utils/progress_manager/manager.py
--rw-r--r--  2.0 unx     1646 b- defN 24-May-13 06:03 akride/_utils/progress_manager/progress_step.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-13 06:03 akride/_utils/rest/__init__.py
--rw-r--r--  2.0 unx      528 b- defN 24-May-13 06:03 akride/_utils/rest/requests_session_manager.py
--rw-r--r--  2.0 unx     3468 b- defN 24-May-13 06:03 akride/_utils/rest/rest_client.py
--rw-r--r--  2.0 unx      194 b- defN 24-May-13 06:03 akride/_utils/rest/utils.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-13 06:03 akride/core/__init__.py
--rw-r--r--  2.0 unx     1450 b- defN 24-May-13 06:03 akride/core/_log.py
--rw-r--r--  2.0 unx    15237 b- defN 24-May-13 06:03 akride/core/_pipeline_executor.py
--rw-r--r--  2.0 unx     1859 b- defN 24-May-13 06:03 akride/core/constants.py
--rw-r--r--  2.0 unx     2309 b- defN 24-May-13 06:03 akride/core/enums.py
--rw-r--r--  2.0 unx     1500 b- defN 24-May-13 06:03 akride/core/exceptions.py
--rw-r--r--  2.0 unx     9614 b- defN 24-May-13 06:03 akride/core/types.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-13 06:03 akride/core/_entity_managers/__init__.py
--rw-r--r--  2.0 unx    18527 b- defN 24-May-13 06:03 akride/core/_entity_managers/catalog_manager.py
--rw-r--r--  2.0 unx    16073 b- defN 24-May-13 06:03 akride/core/_entity_managers/dataset_manager.py
--rw-r--r--  2.0 unx    30350 b- defN 24-May-13 06:03 akride/core/_entity_managers/job_manager.py
--rw-r--r--  2.0 unx     2238 b- defN 24-May-13 06:03 akride/core/_entity_managers/manager.py
--rw-r--r--  2.0 unx     8702 b- defN 24-May-13 06:03 akride/core/_entity_managers/resultset_manager.py
--rw-r--r--  2.0 unx     1314 b- defN 24-May-13 06:03 akride/core/_entity_managers/subscriptions_manager.py
--rw-r--r--  2.0 unx      140 b- defN 24-May-13 06:03 akride/core/_filters/__init__.py
--rw-r--r--  2.0 unx      253 b- defN 24-May-13 06:03 akride/core/_filters/enums.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-13 06:03 akride/core/_filters/partitioners/__init__.py
--rw-r--r--  2.0 unx     6412 b- defN 24-May-13 06:03 akride/core/_filters/partitioners/ingest_partitioner_filter.py
--rw-r--r--  2.0 unx      696 b- defN 24-May-13 06:03 akride/core/_filters/partitioners/models.py
--rw-r--r--  2.0 unx      288 b- defN 24-May-13 06:03 akride/core/_filters/partitioners/partitioner_filter.py
--rw-r--r--  2.0 unx     6043 b- defN 24-May-13 06:03 akride/core/_filters/partitioners/process_partitioner_filter.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-13 06:03 akride/core/_filters/sink/__init__.py
--rw-r--r--  2.0 unx     1247 b- defN 24-May-13 06:03 akride/core/_filters/sink/models.py
--rw-r--r--  2.0 unx     9178 b- defN 24-May-13 06:03 akride/core/_filters/sink/sink_writer_filter.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-13 06:03 akride/core/conf/__init__.py
--rw-rw-r--  2.0 unx      493 b- defN 24-May-13 06:03 akride/core/conf/pylogconf.yaml
--rw-r--r--  2.0 unx        0 b- defN 24-May-13 06:03 akride/core/entities/__init__.py
--rw-r--r--  2.0 unx      796 b- defN 24-May-13 06:03 akride/core/entities/catalogs.py
--rw-r--r--  2.0 unx      736 b- defN 24-May-13 06:03 akride/core/entities/datasets.py
--rw-r--r--  2.0 unx     1549 b- defN 24-May-13 06:03 akride/core/entities/entity.py
--rw-r--r--  2.0 unx     5565 b- defN 24-May-13 06:03 akride/core/entities/jobs.py
--rw-r--r--  2.0 unx      436 b- defN 24-May-13 06:03 akride/core/entities/pipeline.py
--rw-r--r--  2.0 unx      955 b- defN 24-May-13 06:03 akride/core/entities/resultsets.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-13 06:03 akride/core/models/__init__.py
--rw-r--r--  2.0 unx      398 b- defN 24-May-13 06:03 akride/core/models/catalog_details.py
--rw-r--r--  2.0 unx      246 b- defN 24-May-13 06:03 akride/core/models/progress_info.py
--rw-rw-r--  2.0 unx      130 b- defN 24-May-13 06:08 akride-0.4.16.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     3490 b- defN 24-May-13 06:08 akride-0.4.16.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-13 06:08 akride-0.4.16.dist-info/WHEEL
--rw-r--r--  2.0 unx       44 b- defN 24-May-13 06:08 akride-0.4.16.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        7 b- defN 24-May-13 06:08 akride-0.4.16.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     6753 b- defN 24-May-13 06:08 akride-0.4.16.dist-info/RECORD
-75 files, 236443 bytes uncompressed, 63252 bytes compressed:  73.2%
+Zip file size: 91671 bytes, number of entries: 96
+-rw-r--r--  2.0 unx     2129 b- defN 24-Jun-03 04:26 akride/__init__.py
+-rw-r--r--  2.0 unx     2499 b- defN 24-Jun-03 04:26 akride/background_task_manager.py
+-rw-r--r--  2.0 unx    36516 b- defN 24-Jun-03 04:26 akride/client.py
+-rw-r--r--  2.0 unx     2706 b- defN 24-Jun-03 04:26 akride/main.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Jun-03 04:26 akride/_utils/__init__.py
+-rw-r--r--  2.0 unx     3015 b- defN 24-Jun-03 04:26 akride/_utils/background_task_helper.py
+-rw-r--r--  2.0 unx     1357 b- defN 24-Jun-03 04:26 akride/_utils/class_executor.py
+-rw-r--r--  2.0 unx      254 b- defN 24-Jun-03 04:26 akride/_utils/common_utils.py
+-rw-r--r--  2.0 unx      524 b- defN 24-Jun-03 04:26 akride/_utils/dataset_utils.py
+-rw-r--r--  2.0 unx     2624 b- defN 24-Jun-03 04:26 akride/_utils/exception_utils.py
+-rw-r--r--  2.0 unx     1668 b- defN 24-Jun-03 04:26 akride/_utils/file_utils.py
+-rw-r--r--  2.0 unx    14188 b- defN 24-Jun-03 04:26 akride/_utils/job_creator.py
+-rw-r--r--  2.0 unx      278 b- defN 24-Jun-03 04:26 akride/_utils/platform.py
+-rw-r--r--  2.0 unx      454 b- defN 24-Jun-03 04:26 akride/_utils/progress_bar_helper.py
+-rw-r--r--  2.0 unx     1459 b- defN 24-Jun-03 04:26 akride/_utils/proxy_utils.py
+-rw-r--r--  2.0 unx      413 b- defN 24-Jun-03 04:26 akride/_utils/resource_utils.py
+-rw-r--r--  2.0 unx      595 b- defN 24-Jun-03 04:26 akride/_utils/retry_helper.py
+-rw-r--r--  2.0 unx     1094 b- defN 24-Jun-03 04:26 akride/_utils/shell_utils.py
+-rw-r--r--  2.0 unx      811 b- defN 24-Jun-03 04:26 akride/_utils/store_utils.py
+-rw-r--r--  2.0 unx      473 b- defN 24-Jun-03 04:26 akride/_utils/workflow_helper.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Jun-03 04:26 akride/_utils/catalog/__init__.py
+-rw-r--r--  2.0 unx      779 b- defN 24-Jun-03 04:26 akride/_utils/catalog/catalog_tables_helper.py
+-rw-r--r--  2.0 unx      574 b- defN 24-Jun-03 04:26 akride/_utils/catalog/dataset_tables_info.py
+-rw-r--r--  2.0 unx      194 b- defN 24-Jun-03 04:26 akride/_utils/catalog/enums.py
+-rw-r--r--  2.0 unx      890 b- defN 24-Jun-03 04:26 akride/_utils/catalog/pipeline_tables_info.py
+-rw-r--r--  2.0 unx      193 b- defN 24-Jun-03 04:26 akride/_utils/catalog/string_utils.py
+-rw-r--r--  2.0 unx      541 b- defN 24-Jun-03 04:26 akride/_utils/catalog/tables_info.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Jun-03 04:26 akride/_utils/pipeline/__init__.py
+-rw-r--r--  2.0 unx      492 b- defN 24-Jun-03 04:26 akride/_utils/pipeline/constants.py
+-rw-r--r--  2.0 unx     3288 b- defN 24-Jun-03 04:26 akride/_utils/pipeline/pipeline_helper.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Jun-03 04:26 akride/_utils/progress_manager/__init__.py
+-rw-r--r--  2.0 unx     2214 b- defN 24-Jun-03 04:26 akride/_utils/progress_manager/manager.py
+-rw-r--r--  2.0 unx     1745 b- defN 24-Jun-03 04:26 akride/_utils/progress_manager/progress_step.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Jun-03 04:26 akride/_utils/rest/__init__.py
+-rw-r--r--  2.0 unx      528 b- defN 24-Jun-03 04:26 akride/_utils/rest/requests_session_manager.py
+-rw-r--r--  2.0 unx     3468 b- defN 24-Jun-03 04:26 akride/_utils/rest/rest_client.py
+-rw-r--r--  2.0 unx      194 b- defN 24-Jun-03 04:26 akride/_utils/rest/utils.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Jun-03 04:26 akride/_utils/video_splitter/__init__.py
+-rw-r--r--  2.0 unx      584 b- defN 24-Jun-03 04:26 akride/_utils/video_splitter/models.py
+-rwxrwxr-x  2.0 unx     3344 b- defN 24-Jun-03 04:26 akride/_utils/video_splitter/split_video.sh
+-rw-r--r--  2.0 unx     5581 b- defN 24-Jun-03 04:26 akride/_utils/video_splitter/splitter.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Jun-03 04:26 akride/core/__init__.py
+-rw-r--r--  2.0 unx     1728 b- defN 24-Jun-03 04:26 akride/core/_log.py
+-rw-r--r--  2.0 unx    16577 b- defN 24-Jun-03 04:26 akride/core/_pipeline_executor.py
+-rw-r--r--  2.0 unx     2456 b- defN 24-Jun-03 04:26 akride/core/constants.py
+-rw-r--r--  2.0 unx     2309 b- defN 24-Jun-03 04:26 akride/core/enums.py
+-rw-r--r--  2.0 unx     1634 b- defN 24-Jun-03 04:26 akride/core/exceptions.py
+-rw-r--r--  2.0 unx     9614 b- defN 24-Jun-03 04:26 akride/core/types.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Jun-03 04:26 akride/core/_entity_managers/__init__.py
+-rw-r--r--  2.0 unx    18527 b- defN 24-Jun-03 04:26 akride/core/_entity_managers/catalog_manager.py
+-rw-r--r--  2.0 unx    15339 b- defN 24-Jun-03 04:26 akride/core/_entity_managers/dataset_manager.py
+-rw-r--r--  2.0 unx    30350 b- defN 24-Jun-03 04:26 akride/core/_entity_managers/job_manager.py
+-rw-r--r--  2.0 unx     2238 b- defN 24-Jun-03 04:26 akride/core/_entity_managers/manager.py
+-rw-r--r--  2.0 unx     8702 b- defN 24-Jun-03 04:26 akride/core/_entity_managers/resultset_manager.py
+-rw-r--r--  2.0 unx     1314 b- defN 24-Jun-03 04:26 akride/core/_entity_managers/subscriptions_manager.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Jun-03 04:26 akride/core/_entity_managers/_models/__init__.py
+-rw-r--r--  2.0 unx     1349 b- defN 24-Jun-03 04:26 akride/core/_entity_managers/_models/datasets.py
+-rw-r--r--  2.0 unx      140 b- defN 24-Jun-03 04:26 akride/core/_filters/__init__.py
+-rw-r--r--  2.0 unx      253 b- defN 24-Jun-03 04:26 akride/core/_filters/enums.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Jun-03 04:26 akride/core/_filters/partitioners/__init__.py
+-rw-r--r--  2.0 unx     1035 b- defN 24-Jun-03 04:26 akride/core/_filters/partitioners/dtos.py
+-rw-r--r--  2.0 unx      773 b- defN 24-Jun-03 04:26 akride/core/_filters/partitioners/models.py
+-rw-r--r--  2.0 unx      849 b- defN 24-Jun-03 04:26 akride/core/_filters/partitioners/partitioner_filter.py
+-rw-r--r--  2.0 unx     3371 b- defN 24-Jun-03 04:26 akride/core/_filters/partitioners/partitioner_filter_factory.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Jun-03 04:26 akride/core/_filters/partitioners/ingest/__init__.py
+-rw-r--r--  2.0 unx     1055 b- defN 24-Jun-03 04:26 akride/core/_filters/partitioners/ingest/ingest_image_partitioner_filter.py
+-rw-r--r--  2.0 unx     6548 b- defN 24-Jun-03 04:26 akride/core/_filters/partitioners/ingest/ingest_partitioner_filter.py
+-rw-r--r--  2.0 unx     1055 b- defN 24-Jun-03 04:26 akride/core/_filters/partitioners/ingest/ingest_video_partitioner_filter.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Jun-03 04:26 akride/core/_filters/partitioners/process/__init__.py
+-rw-r--r--  2.0 unx     3591 b- defN 24-Jun-03 04:26 akride/core/_filters/partitioners/process/image_process_partitioner_filter.py
+-rw-r--r--  2.0 unx     9127 b- defN 24-Jun-03 04:26 akride/core/_filters/partitioners/process/process_partitioner_filter.py
+-rw-r--r--  2.0 unx     5216 b- defN 24-Jun-03 04:26 akride/core/_filters/partitioners/process/video_process_partitioner_filter.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Jun-03 04:26 akride/core/_filters/sink/__init__.py
+-rw-r--r--  2.0 unx     1590 b- defN 24-Jun-03 04:26 akride/core/_filters/sink/image_sink_writer_filter.py
+-rw-r--r--  2.0 unx     1247 b- defN 24-Jun-03 04:26 akride/core/_filters/sink/models.py
+-rw-r--r--  2.0 unx     1318 b- defN 24-Jun-03 04:26 akride/core/_filters/sink/sink_writer_factory.py
+-rw-r--r--  2.0 unx     9646 b- defN 24-Jun-03 04:26 akride/core/_filters/sink/sink_writer_filter.py
+-rw-r--r--  2.0 unx     2281 b- defN 24-Jun-03 04:26 akride/core/_filters/sink/video_sink_writer_filter.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Jun-03 04:26 akride/core/conf/__init__.py
+-rw-rw-r--  2.0 unx      533 b- defN 24-Jun-03 04:26 akride/core/conf/pylogconf.yaml
+-rw-r--r--  2.0 unx        0 b- defN 24-Jun-03 04:26 akride/core/entities/__init__.py
+-rw-r--r--  2.0 unx      796 b- defN 24-Jun-03 04:26 akride/core/entities/catalogs.py
+-rw-r--r--  2.0 unx      736 b- defN 24-Jun-03 04:26 akride/core/entities/datasets.py
+-rw-r--r--  2.0 unx     1549 b- defN 24-Jun-03 04:26 akride/core/entities/entity.py
+-rw-r--r--  2.0 unx     5565 b- defN 24-Jun-03 04:26 akride/core/entities/jobs.py
+-rw-r--r--  2.0 unx      436 b- defN 24-Jun-03 04:26 akride/core/entities/pipeline.py
+-rw-r--r--  2.0 unx      955 b- defN 24-Jun-03 04:26 akride/core/entities/resultsets.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Jun-03 04:26 akride/core/models/__init__.py
+-rw-r--r--  2.0 unx      398 b- defN 24-Jun-03 04:26 akride/core/models/catalog_details.py
+-rw-r--r--  2.0 unx      293 b- defN 24-Jun-03 04:26 akride/core/models/progress_info.py
+-rw-rw-r--  2.0 unx      130 b- defN 24-Jun-03 04:32 akride-0.4.23.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     3729 b- defN 24-Jun-03 04:32 akride-0.4.23.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Jun-03 04:32 akride-0.4.23.dist-info/WHEEL
+-rw-r--r--  2.0 unx       44 b- defN 24-Jun-03 04:32 akride-0.4.23.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 24-Jun-03 04:32 akride-0.4.23.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     8998 b- defN 24-Jun-03 04:32 akride-0.4.23.dist-info/RECORD
+96 files, 283159 bytes uncompressed, 77035 bytes compressed:  72.8%
```

## zipnote {}

```diff
@@ -15,14 +15,20 @@
 
 Filename: akride/_utils/background_task_helper.py
 Comment: 
 
 Filename: akride/_utils/class_executor.py
 Comment: 
 
+Filename: akride/_utils/common_utils.py
+Comment: 
+
+Filename: akride/_utils/dataset_utils.py
+Comment: 
+
 Filename: akride/_utils/exception_utils.py
 Comment: 
 
 Filename: akride/_utils/file_utils.py
 Comment: 
 
 Filename: akride/_utils/job_creator.py
@@ -39,14 +45,17 @@
 
 Filename: akride/_utils/resource_utils.py
 Comment: 
 
 Filename: akride/_utils/retry_helper.py
 Comment: 
 
+Filename: akride/_utils/shell_utils.py
+Comment: 
+
 Filename: akride/_utils/store_utils.py
 Comment: 
 
 Filename: akride/_utils/workflow_helper.py
 Comment: 
 
 Filename: akride/_utils/catalog/__init__.py
@@ -60,14 +69,17 @@
 
 Filename: akride/_utils/catalog/enums.py
 Comment: 
 
 Filename: akride/_utils/catalog/pipeline_tables_info.py
 Comment: 
 
+Filename: akride/_utils/catalog/string_utils.py
+Comment: 
+
 Filename: akride/_utils/catalog/tables_info.py
 Comment: 
 
 Filename: akride/_utils/pipeline/__init__.py
 Comment: 
 
 Filename: akride/_utils/pipeline/constants.py
@@ -93,14 +105,26 @@
 
 Filename: akride/_utils/rest/rest_client.py
 Comment: 
 
 Filename: akride/_utils/rest/utils.py
 Comment: 
 
+Filename: akride/_utils/video_splitter/__init__.py
+Comment: 
+
+Filename: akride/_utils/video_splitter/models.py
+Comment: 
+
+Filename: akride/_utils/video_splitter/split_video.sh
+Comment: 
+
+Filename: akride/_utils/video_splitter/splitter.py
+Comment: 
+
 Filename: akride/core/__init__.py
 Comment: 
 
 Filename: akride/core/_log.py
 Comment: 
 
 Filename: akride/core/_pipeline_executor.py
@@ -135,44 +159,83 @@
 
 Filename: akride/core/_entity_managers/resultset_manager.py
 Comment: 
 
 Filename: akride/core/_entity_managers/subscriptions_manager.py
 Comment: 
 
+Filename: akride/core/_entity_managers/_models/__init__.py
+Comment: 
+
+Filename: akride/core/_entity_managers/_models/datasets.py
+Comment: 
+
 Filename: akride/core/_filters/__init__.py
 Comment: 
 
 Filename: akride/core/_filters/enums.py
 Comment: 
 
 Filename: akride/core/_filters/partitioners/__init__.py
 Comment: 
 
-Filename: akride/core/_filters/partitioners/ingest_partitioner_filter.py
+Filename: akride/core/_filters/partitioners/dtos.py
 Comment: 
 
 Filename: akride/core/_filters/partitioners/models.py
 Comment: 
 
 Filename: akride/core/_filters/partitioners/partitioner_filter.py
 Comment: 
 
-Filename: akride/core/_filters/partitioners/process_partitioner_filter.py
+Filename: akride/core/_filters/partitioners/partitioner_filter_factory.py
+Comment: 
+
+Filename: akride/core/_filters/partitioners/ingest/__init__.py
+Comment: 
+
+Filename: akride/core/_filters/partitioners/ingest/ingest_image_partitioner_filter.py
+Comment: 
+
+Filename: akride/core/_filters/partitioners/ingest/ingest_partitioner_filter.py
+Comment: 
+
+Filename: akride/core/_filters/partitioners/ingest/ingest_video_partitioner_filter.py
+Comment: 
+
+Filename: akride/core/_filters/partitioners/process/__init__.py
+Comment: 
+
+Filename: akride/core/_filters/partitioners/process/image_process_partitioner_filter.py
+Comment: 
+
+Filename: akride/core/_filters/partitioners/process/process_partitioner_filter.py
+Comment: 
+
+Filename: akride/core/_filters/partitioners/process/video_process_partitioner_filter.py
 Comment: 
 
 Filename: akride/core/_filters/sink/__init__.py
 Comment: 
 
+Filename: akride/core/_filters/sink/image_sink_writer_filter.py
+Comment: 
+
 Filename: akride/core/_filters/sink/models.py
 Comment: 
 
+Filename: akride/core/_filters/sink/sink_writer_factory.py
+Comment: 
+
 Filename: akride/core/_filters/sink/sink_writer_filter.py
 Comment: 
 
+Filename: akride/core/_filters/sink/video_sink_writer_filter.py
+Comment: 
+
 Filename: akride/core/conf/__init__.py
 Comment: 
 
 Filename: akride/core/conf/pylogconf.yaml
 Comment: 
 
 Filename: akride/core/entities/__init__.py
@@ -201,26 +264,26 @@
 
 Filename: akride/core/models/catalog_details.py
 Comment: 
 
 Filename: akride/core/models/progress_info.py
 Comment: 
 
-Filename: akride-0.4.16.dist-info/LICENSE.txt
+Filename: akride-0.4.23.dist-info/LICENSE.txt
 Comment: 
 
-Filename: akride-0.4.16.dist-info/METADATA
+Filename: akride-0.4.23.dist-info/METADATA
 Comment: 
 
-Filename: akride-0.4.16.dist-info/WHEEL
+Filename: akride-0.4.23.dist-info/WHEEL
 Comment: 
 
-Filename: akride-0.4.16.dist-info/entry_points.txt
+Filename: akride-0.4.23.dist-info/entry_points.txt
 Comment: 
 
-Filename: akride-0.4.16.dist-info/top_level.txt
+Filename: akride-0.4.23.dist-info/top_level.txt
 Comment: 
 
-Filename: akride-0.4.16.dist-info/RECORD
+Filename: akride-0.4.23.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## akride/__init__.py

```diff
@@ -1,14 +1,14 @@
 from typing import Optional, Tuple
 
-from akride._utils.resource_utils import get_absolute_path
+from akride._utils.resource_utils import get_conf_absolute_path
 from akride.core._log import get_logger
 from akride.core.constants import Constants
 
-logger_config_file = get_absolute_path(
+logger_config_file = get_conf_absolute_path(
     file_name=Constants.LOG_CONFIG_FILE_NAME
 )
 
 logger = get_logger(module=__name__, config_file_path=logger_config_file)
 
 
 from importlib_metadata import (  # noqa: E501, E402
```

## akride/client.py

```diff
@@ -12,14 +12,16 @@
 import pandas as pd
 import urllib3
 from akridata_akrimanager_v2.models.condition import Condition
 from PIL import Image
 from yarl import URL
 
 from akride._utils.background_task_helper import BackgroundTask
+from akride._utils.dataset_utils import get_dataset_type
+from akride._utils.pipeline.pipeline_helper import PipelineHelper
 from akride._utils.proxy_utils import get_env_proxy_for_url
 from akride._utils.retry_helper import get_http_retry
 from akride.background_task_manager import BackgroundTaskManager
 from akride.core import constants
 from akride.core._entity_managers.catalog_manager import CatalogManager
 from akride.core._entity_managers.dataset_manager import DatasetManager
 from akride.core._entity_managers.job_manager import JobManager
@@ -290,15 +292,19 @@
                 dataset_namespace : str, optional
                     The namespace for the dataset, by default 'default'.
                 data_type : DataType, optional
                     The type of data to store in the dataset, by default
                     DataType.IMAGE.
                 glob_pattern : str, optional
                     The glob pattern for the dataset, by default
-                    '*(png|jpg|gif|jpeg|tiff|tif|bmp)'.
+                    For image datasets: value ='*(png|jpg|gif|jpeg|tiff|tif|bmp)'.
+                    For video datasets: value = '*(mov|mp4|avi|wmv|mpg|mpeg|mkv)'
+                sample_frame_rate: float, optional
+                    The frame rate per second (fps) for videos.
+                    Applicable only for video datasets.
                 overwrite : bool, optional
                     Overwrite if a dataset with the same name exists.
 
         Returns
         -------
         Entity
             The created entity
@@ -415,16 +421,17 @@
             pipelines: List[Pipeline] = self.get_attached_pipelines(
                 dataset=dataset
             )
             image_pipeline = None
             if pipeline_name is None:
                 image_pipeline: Optional[
                     Pipeline
-                ] = self.datasets._get_default_image_pipeline(
-                    attached_pipelines=pipelines
+                ] = PipelineHelper.get_default_pipeline(
+                    attached_pipelines=pipelines,
+                    data_type=get_dataset_type(dataset.info.data_type),
                 )
             else:
                 for pipeline in pipelines:
                     pipeline: Pipeline
                     if pipeline.get_name() == pipeline_name:
                         image_pipeline = pipeline
                         break
@@ -713,16 +720,17 @@
         reference_job: Job, optional
             The reference job for this compare job
         """
         if pipeline is None:
             pipelines: List[Pipeline] = self.get_attached_pipelines(
                 dataset=dataset
             )
-            pipeline = self.datasets._get_default_image_pipeline(
-                attached_pipelines=pipelines
+            pipeline = PipelineHelper.get_default_pipeline(
+                attached_pipelines=pipelines,
+                data_type=get_dataset_type(dataset.info.data_type),
             )
         if catalog_table is None:
             catalog_table = CatalogTable(table_name="primary")
 
         is_compare = False
 
         if job_type == JobType.COMPARE:
```

## akride/main.py

```diff
@@ -1,8 +1,9 @@
 import argparse
+import sys
 
 from akride.client import AkriDEClient
 
 
 def main():
     # Create argument parser
     parser = argparse.ArgumentParser(description="Akride ingestion utility.")
@@ -80,17 +81,21 @@
     else:
         # Fetch dataset by name
         dataset = de_client.get_dataset_by_name(dataset_name)
         if not dataset:
             raise Exception(f"Dataset with name `{dataset_name}` is not found")
 
     # Start ingestion
-    de_client.ingest_dataset(
+    task = de_client.ingest_dataset(
         dataset=dataset,
         data_directory=input_dir,
         use_patch_featurizer=featurizer_type == "patch",
         with_clip_featurizer=with_clip == "yes",
+        async_req=False,
     )
+    # Exit with non-zero exit code if task has failed
+    if task.has_failed():
+        sys.exit(1)
 
 
 if __name__ == "__main__":
     main()
```

## akride/_utils/background_task_helper.py

```diff
@@ -1,13 +1,14 @@
 """
  Copyright (C) 2024, Akridata, Inc - All Rights Reserved.
  Unauthorized copying of this file, via any medium is strictly prohibited
 """
 
 import threading
+import traceback
 from typing import Optional
 
 from akride._utils.progress_manager.manager import ProgressManager
 from akride.core.models.progress_info import ProgressInfo
 
 
 class BackgroundTask:
@@ -43,29 +44,32 @@
         """
         Run the target function and handle any exceptions.
         """
         try:
             self._result = self.target_function(
                 self._progress_manager, *self.args, **self.kwargs
             )
-        except Exception as e:
-            self._progress_manager.set_error(error=e)
+        except Exception:
+            self._progress_manager.set_error(error=traceback.format_exc())
 
         self._progress_manager.set_completed()
 
     def start(self):
         """
         Start the background task in a separate thread.
         """
         self._thread = threading.Thread(target=self.run_task)
         self._thread.start()
 
     def has_completed(self):
         return self._progress_manager.is_completed()
 
+    def has_failed(self):
+        return self._progress_manager.has_failed()
+
     def get_result(self):
         """
         Get the result of the background task.
         :return: The result of the task
         """
 
         if self.has_completed():
```

## akride/_utils/file_utils.py

```diff
@@ -1,22 +1,62 @@
+import json
+import os.path
 import shutil
+import tempfile
 from pathlib import Path
-from typing import List
+from typing import Any, List, Optional
 
 from pyakri_de_utils.file_utils import create_directory
 
+from akride.core._filters.enums import FilterTypes
+
 
 def copy_files_to_dir(files: List[str], dst_dir: str):
     for file in files:
         # file[1:] -> to get the file path without "/"
         dest_file_path = Path(dst_dir, *Path(file).parts[1:])
 
         create_directory(str(dest_file_path.parent))
         shutil.copy(file, dest_file_path)
 
 
 def get_file_name_from_path(filepath: str) -> str:
     return Path(filepath).name
 
 
+def create_temp_directory(dir_path: str):
+    return tempfile.TemporaryDirectory(dir=dir_path)
+
+
+def remove_directory(directory: str):
+    if os.path.exists(directory):
+        shutil.rmtree(directory)
+
+
 def concat_file_paths(*file_path_list) -> str:
     return str(Path(*file_path_list))
+
+
+def get_filter_output_dir(
+    par_dir: str,
+    filter_type: FilterTypes,
+    token_number: Optional[int] = None,
+) -> str:
+    output_dir = concat_file_paths(par_dir, filter_type.value, "outputs")
+    if token_number is not None:
+        output_dir = concat_file_paths(output_dir, str(token_number), "o1")
+    return output_dir
+
+
+def get_sorted_dirs_from_path(path: str):
+    def get_creation_time(item):
+        item_path = concat_file_paths(path, item)
+        return os.path.getctime(item_path)
+
+    items = os.listdir(path)
+    sorted_items = sorted(items, key=get_creation_time)
+    return sorted_items
+
+
+def get_json_from_file(file: str, obj_hook: Optional[Any] = None) -> Any:
+    with open(file, "rb") as f:
+        return json.load(f, object_hook=obj_hook)
```

## akride/_utils/resource_utils.py

```diff
@@ -1,8 +1,17 @@
 import importlib.resources
 
+from akride._utils import video_splitter
 from akride.core import conf
 
 
-def get_absolute_path(file_name):
-    with importlib.resources.path(conf, file_name) as p:
+def _get_absolute_path(module, file_name):
+    with importlib.resources.path(module, file_name) as p:
         return str(p)
+
+
+def get_conf_absolute_path(file_name):
+    return _get_absolute_path(conf, file_name)
+
+
+def get_video_splitter_script(file_name):
+    return _get_absolute_path(video_splitter, file_name)
```

## akride/_utils/retry_helper.py

```diff
@@ -1,14 +1,14 @@
 from urllib3 import Retry
 
 
 def get_http_retry(
-    total=4,
+    total=6,
     backoff_factor=1,
-    status_forcelist=frozenset(range(503, 600)),
+    status_forcelist=frozenset(range(502, 600)),
     allowed_methods=frozenset(
         ["HEAD", "GET", "PUT", "DELETE", "OPTIONS", "TRACE", "POST", "PATCH"]
     ),
 ) -> Retry:
     """
     get_http_retry returns a Retry object which retries on 5XX status code
     for "HEAD", "GET", "PUT", "DELETE", "OPTIONS", "TRACE", "POST", "PATCH"
```

## akride/_utils/pipeline/constants.py

```diff
@@ -1,7 +1,14 @@
 class Constants:
     # "AkridataImagePipeline"
     FULL_IMAGE_PIPELINE_INTERNAL_ID = 3101
     # "AkridataImagePatchPipelineV2"
     PATCH_IMAGE_PIPELINE_INTERNAL_ID = 3103
     # "AkridataImageClipPipelineV2"
     CLIP_IMAGE_PIPELINE_INTERNAL_ID = 3112
+
+    # "AkridataVideoPipelineV2"
+    FULL_IMAGE_VIDEO_PIPELINE_INTERNAL_ID = 3206
+    # "AkridataVideoPatchPipelineV3"
+    PATCH_VIDEO_PIPELINE_INTERNAL_ID = 3207
+    # "AkridataVideoClipPipelineV2"
+    CLIP_VIDEO_PIPELINE_INTERNAL_ID = 3215
```

## akride/_utils/pipeline/pipeline_helper.py

```diff
@@ -1,20 +1,32 @@
+from typing import List, Optional
+
+from akride import logger
 from akride._utils.pipeline.constants import Constants
+from akride.core.entities.pipeline import Pipeline
 from akride.core.enums import DataType, FeaturizerType
+from akride.core.exceptions import UserError
 
 
 class PipelineHelper:
     FEATURIZER_TYPE_AND_PIPELINE_MAPPING = {
         DataType.IMAGE: {
             FeaturizerType.FULL_IMAGE: (
                 Constants.FULL_IMAGE_PIPELINE_INTERNAL_ID
             ),
             FeaturizerType.PATCH: Constants.PATCH_IMAGE_PIPELINE_INTERNAL_ID,
             FeaturizerType.CLIP: Constants.CLIP_IMAGE_PIPELINE_INTERNAL_ID,
-        }
+        },
+        DataType.VIDEO: {
+            FeaturizerType.FULL_IMAGE: (
+                Constants.FULL_IMAGE_VIDEO_PIPELINE_INTERNAL_ID
+            ),
+            FeaturizerType.PATCH: Constants.PATCH_VIDEO_PIPELINE_INTERNAL_ID,
+            FeaturizerType.CLIP: Constants.CLIP_VIDEO_PIPELINE_INTERNAL_ID,
+        },
     }
 
     @classmethod
     def get_pipeline_internal_id(
         cls,
         featurizer_type: FeaturizerType,
         data_type: DataType = DataType.IMAGE,
@@ -28,7 +40,57 @@
         pipeline_internal_id = featurizer_map_by_datatype.get(featurizer_type)
 
         if not pipeline_internal_id:
             raise ValueError(
                 f"Featurizer {featurizer_type} is not yet supported"
             )
         return pipeline_internal_id
+
+    @classmethod
+    def get_default_pipeline(
+        cls,
+        attached_pipelines: List[Pipeline],
+        data_type: DataType,
+    ) -> Optional[Pipeline]:
+        # Find the pipelines from the list of attached pipelines based on the dataset type,
+        # if both full/patch pipelines are present, prefer patch
+        # pipeline
+        patch_image_pipeline: Optional[Pipeline] = None
+        full_image_pipeline: Optional[Pipeline] = None
+
+        featurizer_pipeline_map = cls.FEATURIZER_TYPE_AND_PIPELINE_MAPPING.get(
+            data_type
+        )
+
+        patch_image_pipeline_id = featurizer_pipeline_map.get(
+            FeaturizerType.PATCH
+        )
+        full_image_pipeline_id = featurizer_pipeline_map.get(
+            FeaturizerType.FULL_IMAGE
+        )
+
+        logger.info(
+            f"Patch image pipeline id is {patch_image_pipeline_id},"
+            f"Full image pipeline id is {full_image_pipeline_id}"
+        )
+
+        for pipeline in attached_pipelines:
+            internal_id = pipeline.info.pipeline_internal_id
+
+            logger.info(f"Internal id is {internal_id}")
+            if internal_id == patch_image_pipeline_id:
+                patch_image_pipeline = pipeline
+                break
+
+            if internal_id == full_image_pipeline_id:
+                full_image_pipeline = pipeline
+
+        if patch_image_pipeline is None and full_image_pipeline is None:
+            raise UserError(
+                message="No default pipelines attached to the dataset"
+            )
+
+        return (
+            patch_image_pipeline
+            if patch_image_pipeline
+            else full_image_pipeline
+        )
```

## akride/_utils/progress_manager/manager.py

```diff
@@ -8,30 +8,36 @@
 
 class ProgressManager:
     def __init__(self):
         self._msg = None
         self._error = None
 
         self._complete = False
+        self._failed = False
+
         self._steps: List[ProgressStep] = []
 
         self._register_lock = threading.Lock()
 
     def set_msg(self, msg):
         self._msg = msg
 
     def set_error(self, error):
         self._error = error
+        self._failed = True
 
     def set_completed(self):
         self._complete = True
 
     def is_completed(self):
         return self._complete
 
+    def has_failed(self):
+        return self._failed
+
     def get_error(self):
         return self._error
 
     def register_step(self, step_name, weight: int = 1) -> ProgressStep:
         with self._register_lock:
             if step_name in self._steps:
                 raise ValueError("Step is already registered!")
@@ -62,8 +68,10 @@
 
         percentage_completed = float(total_percentage / total_weight)
 
         return ProgressInfo(
             percent_completed=percentage_completed,
             message=self._msg,
             completed=self._complete,
+            error=self._error,
+            failed=self._failed,
         )
```

## akride/_utils/progress_manager/progress_step.py

```diff
@@ -15,18 +15,22 @@
         self._completed_steps = 0
 
         self._update_lock = threading.Lock()
 
     def get_weight(self):
         return self._weight
 
+    def has_started(self):
+        return self._started
+
     def set_total_steps(self, total):
-        with self._update_lock:
-            self._total_steps = total
-            self._started = True
+        if not self._started:
+            with self._update_lock:
+                self._total_steps = total
+                self._started = True
 
     def increment_processed_steps(self, completed):
         if not self._started:
             raise ValueError(
                 "Cannot increment processed steps when not started!"
             )
```

## akride/core/_log.py

```diff
@@ -1,13 +1,14 @@
 """
  Copyright (C) 2024, Akridata, Inc - All Rights Reserved.
  Unauthorized copying of this file, via any medium is strictly prohibited
 """
 import logging
 import logging.config
+
 import yaml
 
 from akride.core.constants import Constants
 
 
 class PPrintFormatter(logging.Formatter):
     """Logging Formatter resembling pprint format"""
@@ -18,16 +19,24 @@
     def format(self, record):
         message = super().format(record)
         message = message.replace("(asctime)", "")
         message = message.replace("(levelname)", "")
         return message
 
 
+def remove_stream_handler(loggerr):
+    for handler in loggerr.handlers:
+        if type(handler) == logging.StreamHandler:  # noqa E721
+            loggerr.removeHandler(handler)
+            handler.close()
+
+
 def get_logger(module: str, config_file_path):
     logger = logging.getLogger(module)
+    root_logger = logging.getLogger()
 
     try:
         with open(config_file_path, "r") as file:
             config = yaml.safe_load(file.read())
             logging.config.dictConfig(config)
     except Exception:
         if config_file_path:
@@ -38,13 +47,13 @@
         stream_handler = logging.StreamHandler()
         logger.addHandler(stream_handler)
 
         logger.info(
             "No config found for logger. Redirecting to Standard output!"
         )
 
-    if Constants.DEBUGGING_ENABLED:
-        logger.setLevel(logging.DEBUG)
-        for handler in logger.handlers:
-            handler.setLevel(logging.DEBUG)
+    # Remove console handler from all loggers if debugging not set
+    if not Constants.DEBUGGING_ENABLED:
+        remove_stream_handler(logger)
+        remove_stream_handler(root_logger)
 
     return logger
```

## akride/core/_pipeline_executor.py

```diff
@@ -1,38 +1,39 @@
 import tempfile
-from typing import List, Optional, Tuple
+from typing import List, Optional
 
 import akridata_akrimanager_v2 as am
 import akridata_dsp as dsp
 from pyakri_de_filters.data_ingest_filter.data_ingest_filter_wrapper import (
     DataIngestWrapper,
 )
 
 from akride import logger
 from akride._utils.catalog.catalog_tables_helper import CatalogTablesHelper
 from akride._utils.catalog.pipeline_tables_info import PipelineTablesInfo
 from akride._utils.class_executor import ClassExecutor
-from akride._utils.file_utils import concat_file_paths
+from akride._utils.dataset_utils import get_dataset_type
+from akride._utils.file_utils import concat_file_paths, get_filter_output_dir
 from akride._utils.platform import is_windows_os
 from akride._utils.progress_manager.manager import (
     ProgressManager,
     ProgressStep,
 )
 from akride._utils.workflow_helper import WorkflowHelper
 from akride.core._filters.enums import FilterTypes
-from akride.core._filters.partitioners.ingest_partitioner_filter import (
-    IngestPartitionerFilter,
-)
-from akride.core._filters.partitioners.process_partitioner_filter import (
-    ProcessPartitionerFilter,
-    ProcessTokenInfo,
+from akride.core._filters.partitioners.dtos import ProcessTokenInfo
+from akride.core._filters.partitioners.partitioner_filter_factory import (
+    PartitionerFilterFactory,
 )
 from akride.core._filters.sink.models import SinkWriterFilterInput
-from akride.core._filters.sink.sink_writer_filter import SinkWriterFilter
+from akride.core._filters.sink.sink_writer_factory import (
+    SinkWriterFilterFactory,
+)
 from akride.core.constants import Constants
+from akride.core.enums import DataType
 from akride.core.exceptions import ServerError
 
 
 class PipelineExecutor:
     INGEST_WORKFLOW_PROGRESS_WEIGHTAGE = 1
     PROCESS_WORKFLOW_PROGRESS_WEIGHTAGE = 3
 
@@ -86,203 +87,237 @@
         logger.debug("Ingestion completed!")
 
     def _run_ingest_workflow(self, ingest_step: ProgressStep):
         session_id, workflow_id = WorkflowHelper.get_session_and_workflow_id(
             workflow_id_prefix="reg", dataset_id=self._dataset.id
         )
 
-        IngestPartitionerFilter(
-            dataset=self._dataset,
-            data_dir=self._data_dir,
-            session_id=session_id,
-            workflow_id=workflow_id,
-            dataset_tables_info=(
-                self._catalog_tables_helper.get_dataset_tables_info()
-            ),
-            ccs_api=self._ccs_api,
-            ingest_step=ingest_step,
-        ).run()
+        ingest_partitioner_filter = (
+            PartitionerFilterFactory.get_ingest_partitioner(
+                dataset=self._dataset,
+                data_dir=self._data_dir,
+                session_id=session_id,
+                workflow_id=workflow_id,
+                dataset_tables_info=(
+                    self._catalog_tables_helper.get_dataset_tables_info()
+                ),
+                ccs_api=self._ccs_api,
+                ingest_step=ingest_step,
+                data_type=get_dataset_type(
+                    dataset_type=self._dataset.data_type
+                ),
+            )
+        )
+
+        ingest_partitioner_filter.run()
 
     def _run_process_workflow(self, process_steps: List[ProgressStep]):
         for index, pipeline_info in enumerate(
             self._catalog_tables_helper.get_pipelines()
         ):
+            logger.debug(
+                f"Running process workflow for pipeline "
+                f"{pipeline_info.get_pipeline_id()}"
+            )
             (
                 session_id,
                 workflow_id,
             ) = WorkflowHelper.get_session_and_workflow_id(
                 workflow_id_prefix="process", dataset_id=self._dataset.id
             )
             pipeline_filters_info = self._pipeline_filters_info_list[index]
             self._run_process_workflow_per_pipeline(
                 pipeline_info=pipeline_info,
                 pipeline_filters_info=pipeline_filters_info,
                 session_id=session_id,
                 workflow_id=workflow_id,
                 process_step=process_steps[index],
+                dataset_data_type=get_dataset_type(
+                    dataset_type=self._dataset.data_type
+                ),
             )
 
     def _run_process_workflow_per_pipeline(
         self,
         pipeline_info: PipelineTablesInfo,
         pipeline_filters_info: am.AkriSDKWorkflowResponse,
         session_id: str,
         workflow_id: str,
         process_step: ProgressStep,
+        dataset_data_type: DataType,
     ):
         dataset_tables_info = (
             self._catalog_tables_helper.get_dataset_tables_info()
         )
-        process_partitioner_filter = ProcessPartitionerFilter(
-            dataset_id=self._dataset.id,
-            pipeline_info=pipeline_info,
-            partitioned_abs_table=(
-                dataset_tables_info.get_partitioned_abs_table()
-            ),
-            ccs_api=self._ccs_api,
-            process_step=process_step,
+
+        process_partitioner_filter = (
+            PartitionerFilterFactory.get_process_partitioner(
+                dataset_id=self._dataset.id,
+                pipeline_tables_info=pipeline_info,
+                dataset_tables_info=dataset_tables_info,
+                ccs_api=self._ccs_api,
+                data_type=dataset_data_type,
+                sample_frame_rate=self._dataset.dataset_spec.sample_frame_rate,
+            )
         )
 
-        for process_token_info in process_partitioner_filter.run():
-            # Create temp folder per token
-            with tempfile.TemporaryDirectory() as tmp_dir:
-                (
-                    _,
-                    metadata_output_dir,
-                ) = self._prepare_partitioner_and_metadata_dir(
-                    process_token_info=process_token_info,
-                    tmp_dir=tmp_dir,
-                )
+        token_generator = process_partitioner_filter.run()
 
-                # Map to get filter output directory by filter type
-                filters_output_dir_map: dict = (
-                    self._get_filters_output_dir_map(
-                        parent_dir=tmp_dir,
-                        token_number=process_token_info.token_number,
-                    )
-                )
+        tokens_processed = 0
 
-                filter_execution_order_list: List[
-                    dict
-                ] = self._get_filter_execution_order_list(
-                    pipeline_filters_info=pipeline_filters_info,
-                    filters_output_dir_map=filters_output_dir_map,
-                )
-                for sdk_details in filter_execution_order_list:
-                    self._run_filter(
-                        filter_details=sdk_details["filter_details"],
-                        src_dir=sdk_details["src_dir"],
-                        dst_dir=sdk_details["dst_dir"],
-                        filter_type=sdk_details["filter_type"],
+        try:
+            while True:
+                try:
+                    process_token_info: ProcessTokenInfo = next(
+                        token_generator
                     )
 
-                # init params for data ingest would be same as featurizer
-                data_ingest_init_params = (
-                    pipeline_filters_info.featurizer.init_params
-                )
-                data_ingest_output_dir = filters_output_dir_map[
-                    FilterTypes.DataIngest
-                ]
-                # Run Data ingest filter
-                with tempfile.NamedTemporaryFile(dir=tmp_dir) as fp:
-                    logger.debug("Data ingestion filter is in progress!")
-                    fp_name = fp.name
-                    if is_windows_os():
-                        # windows does not allow already opened temp file.
-                        # fp will be deleted along with tmp_dir
-                        fp.close()
-                    ingest_filter = DataIngestWrapper()
-                    ingest_filter.init(**data_ingest_init_params)
-
-                    # Featurizer output will be input for data ingest filter
-                    ingest_src_dir = filters_output_dir_map[
-                        FilterTypes.Featurizer
-                    ]
+                    token_num = process_token_info.token_number
+                    parent_dir = process_token_info.parent_dir
+                    metadata_dir = process_token_info.metadata_dir
+                    out_dir = process_token_info.out_dir
+
+                    # Set total steps for the first run
+                    if not process_step.has_started():
+                        process_step.set_total_steps(
+                            process_token_info.total_num_tokens
+                        )
+
+                    # Map to get filter output directory by filter type
+                    filters_output_dir_map: dict = (
+                        self._get_filters_output_dir_map(
+                            partitioner_out_dir=out_dir,
+                            parent_dir=parent_dir,
+                            token_number=token_num,
+                        )
+                    )
 
-                    ingest_filter.run(
-                        src_dir=ingest_src_dir,
-                        dst_dir=data_ingest_output_dir,
-                        tmp_file=fp_name,
+                    filter_execution_order_list: List[
+                        dict
+                    ] = self._get_filter_execution_order_list(
+                        pipeline_filters_info=pipeline_filters_info,
+                        filters_output_dir_map=filters_output_dir_map,
                     )
+
                     logger.debug(
-                        "Data ingestion filter completed successfully!"
+                        f"Filter execution order list is {filter_execution_order_list}"
                     )
 
-                thumbnail_aggregator_output_dir = filters_output_dir_map[
-                    FilterTypes.ThumbnailAggregator
-                ]
-                # Run sink writer filter
-                logger.debug("Sync filter is in progress!")
-                SinkWriterFilter(
-                    filter_input=SinkWriterFilterInput(
-                        dataset_id=self._dataset.id,
-                        pipeline_tables_info=pipeline_info,
-                        workflow_id=workflow_id,
-                        session_id=session_id,
-                        file_metadata_list=(process_token_info.file_info_list),
-                    ),
-                    workflow_api=self._workflow_api,
-                    dsp_dataset_api=self._dsp_dataset_api,
-                    ccs_api=self._ccs_api,
-                ).run_from_input_dir(
-                    coreset_dir=concat_file_paths(
-                        data_ingest_output_dir,
-                        DataIngestWrapper.DEST_CORESET_SUB_DIR,
-                    ),  # noqa
-                    projections_dir=concat_file_paths(
-                        data_ingest_output_dir,
-                        DataIngestWrapper.DEST_PROJECTIONS_SUB_DIR,
-                    ),  # noqa
-                    sketch_dir=concat_file_paths(
-                        data_ingest_output_dir,
-                        DataIngestWrapper.DEST_SKETCH_SUB_DIR,
-                    ),  # noqa
-                    thumbnail_dir=thumbnail_aggregator_output_dir,
-                    blobs_dir=metadata_output_dir,
-                )
+                    for sdk_details in filter_execution_order_list:
+                        self._run_filter(
+                            filter_details=sdk_details["filter_details"],
+                            src_dir=sdk_details["src_dir"],
+                            dst_dir=sdk_details["dst_dir"],
+                            filter_type=sdk_details["filter_type"],
+                        )
+
+                    # init params for data ingest would be same as featurizer
+                    data_ingest_init_params = (
+                        pipeline_filters_info.featurizer.init_params
+                    )
+                    data_ingest_output_dir = filters_output_dir_map[
+                        FilterTypes.DataIngest
+                    ]
+                    # Run Data ingest filter
+                    with tempfile.NamedTemporaryFile(dir=parent_dir) as fp:
+                        logger.debug("Data ingestion filter is in progress!")
 
-                process_step.increment_processed_steps(completed=1)
+                        # windows does not allow already opened temp file.
+                        # fp will be deleted along with tmp_dir
+                        fp_name = fp.name
+                        if is_windows_os():
+                            fp.close()
+
+                        ingest_filter = DataIngestWrapper()
+                        ingest_filter.init(**data_ingest_init_params)
+
+                        # Featurizer output will be input for data ingest filter
+                        ingest_src_dir = filters_output_dir_map[
+                            FilterTypes.Featurizer
+                        ]
+
+                        ingest_filter.run(
+                            src_dir=ingest_src_dir,
+                            dst_dir=data_ingest_output_dir,
+                            tmp_file=fp_name,
+                        )
+                        logger.debug(
+                            "Data ingestion filter completed successfully!"
+                        )
 
-            #  Update dsp session
-            session_create_request = dsp.PipelineSessionCreateRequest(
-                status="COMPLETE"
-            )
-            self._dsp_dataset_api.update_dataset_session_state(
-                session_id=session_id,
-                pipeline_id=pipeline_info.get_pipeline_id(),
-                dataset_id=self._dataset.id,
-                pipeline_session_create_request=session_create_request,
-            )
+                    thumbnail_aggregator_output_dir = filters_output_dir_map[
+                        FilterTypes.ThumbnailAggregator
+                    ]
+                    # Run sink writer filter
+                    logger.debug("Sync filter is in progress!")
+                    sink_writer = SinkWriterFilterFactory.get_sink_writer(
+                        filter_input=SinkWriterFilterInput(
+                            dataset_id=self._dataset.id,
+                            pipeline_tables_info=pipeline_info,
+                            workflow_id=workflow_id,
+                            session_id=session_id,
+                            file_metadata_list=(
+                                process_token_info.file_info_list
+                            ),
+                        ),
+                        workflow_api=self._workflow_api,
+                        dsp_dataset_api=self._dsp_dataset_api,
+                        ccs_api=self._ccs_api,
+                        data_type=dataset_data_type,
+                    )
 
-    @classmethod
-    def _prepare_partitioner_and_metadata_dir(
-        cls, process_token_info: ProcessTokenInfo, tmp_dir: str
-    ) -> Tuple[str, str]:
-        token_number = process_token_info.token_number
-        partitioner_parent_output_dir = cls._get_output_dir(
-            par_dir=tmp_dir, filter_type=FilterTypes.Partitioner
-        )
+                    sink_writer.run_from_input_dir(
+                        coreset_dir=concat_file_paths(
+                            data_ingest_output_dir,
+                            DataIngestWrapper.DEST_CORESET_SUB_DIR,
+                        ),  # noqa
+                        projections_dir=concat_file_paths(
+                            data_ingest_output_dir,
+                            DataIngestWrapper.DEST_PROJECTIONS_SUB_DIR,
+                        ),  # noqa
+                        sketch_dir=concat_file_paths(
+                            data_ingest_output_dir,
+                            DataIngestWrapper.DEST_SKETCH_SUB_DIR,
+                        ),  # noqa
+                        thumbnail_dir=thumbnail_aggregator_output_dir,
+                        blobs_dir=metadata_dir,
+                    )
 
-        # Prepare partitioner output directory
-        partitioner_output_dir = concat_file_paths(
-            partitioner_parent_output_dir, str(token_number), "o1"
+                    if process_token_info.should_update_progress():
+                        process_step.increment_processed_steps(completed=1)
+
+                    process_partitioner_filter.cleanup_token(
+                        token_num=token_num,
+                        partition_num=process_token_info.partition_num,
+                    )
+
+                    tokens_processed += 1
+                except StopIteration:
+                    break
+        finally:
+            # If not tokens processed, set total steps to 0
+            if not tokens_processed:
+                process_step.set_total_steps(0)
+
+            process_partitioner_filter.cleanup()
+
+        # Update dsp session
+        session_create_request = dsp.PipelineSessionCreateRequest(
+            status="COMPLETE"
         )
-        ProcessPartitionerFilter.prepare_output_dir(
-            files=process_token_info.files, output_dir=partitioner_output_dir
+        self._dsp_dataset_api.update_dataset_session_state(
+            session_id=session_id,
+            pipeline_id=pipeline_info.get_pipeline_id(),
+            dataset_id=self._dataset.id,
+            pipeline_session_create_request=session_create_request,
         )
 
-        # Prepare metadata dir
-        metadata_output_dir = concat_file_paths(
-            partitioner_parent_output_dir, "metadata", str(token_number), "o1"
-        )
-        ProcessPartitionerFilter.prepare_metadata_dir(
-            filemeta_list=process_token_info.file_meta_list,
-            metadata_dir=metadata_output_dir,
+        logger.debug(
+            f"Session completed for pipeline {pipeline_info.get_pipeline_id()}!"
         )
-        return partitioner_output_dir, metadata_output_dir
 
     @classmethod
     def _get_filter_execution_order_list(
         cls,
         pipeline_filters_info: am.AkriSDKWorkflowResponse,
         filters_output_dir_map: dict,
     ) -> List[dict]:
@@ -323,37 +358,33 @@
             },
         ]
 
         return filter_execution_order_list
 
     @classmethod
     def _get_filters_output_dir_map(
-        cls, parent_dir: str, token_number: int
+        cls,
+        parent_dir: str,
+        token_number: int,
+        partitioner_out_dir: Optional[str] = None,
     ) -> dict:
         output_dir_map = {}
         for filter_type in FilterTypes:
-            output_dir_map[filter_type] = cls._get_output_dir(
+            if filter_type == FilterTypes.Partitioner and partitioner_out_dir:
+                output_dir_map[filter_type] = partitioner_out_dir
+                continue
+
+            output_dir_map[filter_type] = get_filter_output_dir(
                 par_dir=parent_dir,
                 token_number=token_number,
                 filter_type=filter_type,
             )
         return output_dir_map
 
     @staticmethod
-    def _get_output_dir(
-        par_dir: str,
-        filter_type: FilterTypes,
-        token_number: Optional[int] = None,
-    ) -> str:
-        output_dir = concat_file_paths(par_dir, filter_type.value, "outputs")
-        if token_number:
-            output_dir = concat_file_paths(output_dir, str(token_number), "o1")
-        return output_dir
-
-    @staticmethod
     def _run_filter(
         filter_details: am.AkriSDKFilterDetails,
         src_dir: str,
         dst_dir: str,
         filter_type: FilterTypes,
     ):
         try:
@@ -377,9 +408,11 @@
             run_method_params = {"src_dir": src_dir, "dst_dir": dst_dir}
             class_executor.call_method(run_method, **run_method_params)
 
             if cleanup_method:
                 class_executor.call_method(method_name=cleanup_method)
             logger.debug(f"{filter_type.value} filter completed successfully!")
         except Exception as ex:
-            logger.error(f"Failed to run sdk filter due to {ex}")
-            raise ServerError(f"Failed to run sdk filter due to {ex}")
+            logger.error(
+                f"Failed to run sdk filter due to {ex}. Filter details {filter_details}"
+            )
+            raise ServerError(f"Failed to run sdk filter with error: {ex}")
```

## akride/core/constants.py

```diff
@@ -1,19 +1,37 @@
 import os
 
 import akridata_akrimanager_v2 as am
 
 
 class Constants:
+    AKRIDE_TMP_DIR = os.path.join("/", "tmp", ".akride")
+
+    DEFAULT_IMAGE_BLOB_EXPR = "*(png|jpg|gif|jpeg|tiff|tif|bmp)"
+    DEFAULT_VIDEO_BLOB_EXPR = "*(mov|mp4|avi|wmv|mpg|mpeg|mkv)"
+
     LOG_CONFIG_FILE_NAME = "pylogconf.yaml"
-    INGEST_WF_TOKEN_SIZE = 1024
+
     DEFAULT_SAAS_ENDPOINT = "https://app.akridata.ai"
-    INGEST_FILES_COUNT_IN_ONE_PARTITION = 10000
-    PARTITION_SIZE = 300000000
-    PROCESS_WF_TOKEN_SIZE = 1500
+
+    PARTITION_TIME_FRAME = 300000000
+
+    INGEST_IMAGE_WF_TOKEN_SIZE = 1024
+    INGEST_IMAGE_PARTITION_SIZE = 10000
+    PROCESS_IMAGE_WF_TOKEN_SIZE = 1500
+
+    # Only 1 video per token is supported.
+    # DO NOT MODIFY THIS VALUE
+    INGEST_VIDEO_PARTITION_SIZE = 10
+    INGEST_VIDEO_WF_TOKEN_SIZE = 1
+    PROCESS_VIDEO_WF_TOKEN_SIZE = 1
+    VIDEO_CHUNK_SIZE = 300
+
+    CCS_API_BATCH_SIZE = 1000
+
     FILE_TYPES = [
         am.DatastoreFileType.BLOBS,
         am.DatastoreFileType.CORESET,
         am.DatastoreFileType.PROJECTIONS,
         am.DatastoreFileType.SKETCH,
         am.DatastoreFileType.THUMBNAIL,
     ]
@@ -51,22 +69,28 @@
         "workflow_id",
         "session_id",
         "coreset",
         "projections",
         "sketch",
         "thumbnail",
     ]
-    PRIMARY_TABLE_COLUMNS = [
+    PRIMARY_TABLE_IMAGE_COLUMNS = [
         "partition_start",
         "partition_end",
         "workflow_id",
         "session_id",
         "frame_idx_in_blob",
         "blob_idx_in_partition",
         "file_path",
         "timestamp",
         "file_id",
         "frame_idx_in_file",
         "file_name",
         "total_frames_in_file",
+        "frame_height",
+        "frame_width",
+    ]
+
+    PRIMARY_TABLE_VIDEO_COLUMNS = PRIMARY_TABLE_IMAGE_COLUMNS + [
+        "native_fps",
     ]
-    DEBUGGING_ENABLED = os.getenv("ENABLE_LOGS", "").lower() == "true"
+    DEBUGGING_ENABLED = os.getenv("ENABLE_DEBUG_LOGS", "").lower() == "true"
```

## akride/core/exceptions.py

```diff
@@ -43,14 +43,20 @@
 
 class InvalidAuthConfigError(UserError):
     """Custom exception class defined to handle errors raised
     due to Invalid api-key
     """
 
 
+class InvalidInputError(UserError):
+    """Custom exception class defined to handle errors raised
+    due to Invalid inputs
+    """
+
+
 class ServerNotReachableError(BaseError):
     """Error thrown when the client is unable to connect to the server"""
 
 
 class ErrorMessages:  # pylint: disable=too-few-public-methods
     """Class that that holds all error messages used in the sdk"""
```

## akride/core/_entity_managers/dataset_manager.py

```diff
@@ -3,28 +3,30 @@
 
 import akridata_akrimanager_v2 as am
 import akridata_dsp as dsp
 
 from akride import logger
 from akride._utils.background_task_helper import BackgroundTask
 from akride._utils.catalog.catalog_tables_helper import CatalogTablesHelper
+from akride._utils.dataset_utils import get_dataset_type
 from akride._utils.exception_utils import translate_api_exceptions
-from akride._utils.pipeline.constants import Constants
 from akride._utils.pipeline.pipeline_helper import PipelineHelper
 from akride._utils.progress_bar_helper import ProgressBarHelper
 from akride._utils.progress_manager.manager import ProgressManager
+from akride.core._entity_managers._models.datasets import CreateDatasetIn
 from akride.core._entity_managers.catalog_manager import CatalogManager
 from akride.core._entity_managers.manager import Manager
 from akride.core._pipeline_executor import PipelineExecutor
 from akride.core.entities.datasets import Dataset
 from akride.core.entities.entity import Entity
 from akride.core.entities.pipeline import Pipeline
 from akride.core.enums import BackgroundTaskType, DataType, FeaturizerType
 from akride.core.exceptions import ServerError, UserError
 from akride.core.models.catalog_details import CatalogDetails
+from akride.core.models.progress_info import ProgressInfo
 from akride.core.types import ClientManager
 
 
 class DatasetManager(Manager):
     """
     Class Managing Dataset related operations on DataExplorer
     """
@@ -56,15 +58,16 @@
             The dataset spec.
 
         Returns
         -------
         Entity
             The created dataset
         """
-        return self._create_dataset(**spec)
+        input_spec = CreateDatasetIn(**spec)
+        return self._create_dataset(input_spec)
 
     @translate_api_exceptions
     def delete_entity(self, entity: Entity) -> bool:
         """
         Deletes an entity.
 
         Parameters
@@ -77,22 +80,15 @@
         bool
             Indicates whether this entity was successfully deleted
         """
         dataset_id = entity.get_id()
         api_response = self.dataset_api.delete_dataset(dataset_id)
         return api_response.success == "True"  # type: ignore
 
-    def _create_dataset(
-        self,
-        dataset_name: str,
-        dataset_namespace: str = "default",
-        data_type: DataType = DataType.IMAGE,
-        glob_pattern: str = "*(png|jpg|gif|jpeg|tiff|tif|bmp)",
-        overwrite: bool = False,
-    ) -> Dataset:
+    def _create_dataset(self, create_data: CreateDatasetIn) -> Dataset:
         """
         Method for creating a new dataset.
 
         Parameters
         ----------
         dataset_name : str
             The name of the new dataset.
@@ -102,47 +98,48 @@
             The type of data to store in the dataset, by default
             DataType.IMAGE.
         glob_pattern : str, optional
             The glob pattern for the dataset, by default
             '*(png|jpg|gif|jpeg|tiff|tif|bmp)'.
         overwrite : bool, optional
             Overwrite if a dataset with the same name exists.
-
+        sample_frame_rate: float, optional
+            The frame rate per second (fps) for videos.
+            Applicable only for video datasets.
         Returns
         -------
         Dataset
             The newly created dataset.
         """
-        logger.debug(
-            "Creating dataset %s in %s namespace of data_type %s, with file"
-            "pattern %s",
-            dataset_name,
-            dataset_namespace,
-            data_type,
-            glob_pattern,
-        )
-        logger.debug("overwrite set to %s", overwrite)
-        if overwrite:
+        logger.debug(f"Creating dataset with input {create_data}")
+
+        if create_data.overwrite:
             raise NotImplementedError
 
-        dataset_spec = {"access_type": "default", "glob": glob_pattern}
+        dataset_spec = {
+            "access_type": "default",
+            "glob": create_data.glob_pattern,
+        }
+
+        if create_data.data_type == DataType.VIDEO:
+            dataset_spec["sample_frame_rate"] = create_data.sample_frame_rate
 
         containers = {"source": {"local": True}, "sink": {"internal": True}}
         dataset_type = "basic"
         am_dataset = am.DataSet(
-            dataset_name=dataset_name,
-            namespace=dataset_namespace,
+            dataset_name=create_data.dataset_name,
+            namespace=create_data.dataset_namespace,
             type=dataset_type,
-            data_type=data_type.value,
+            data_type=create_data.data_type.value,
             containers=containers,
             dataset_spec=dataset_spec,
         )
         api_response = self.dataset_api.create_new_dataset(am_dataset)
-        assert api_response.dataset_id is not None
-        return self.get_entity_by_id(entity_id=api_response.dataset_id)
+        assert api_response._dataset_id is not None
+        return self.get_entity_by_id(entity_id=api_response._dataset_id)
 
     def _attach_pipeline(
         self,
         featurizer_type: FeaturizerType,
         dataset_id: str,
         data_type: DataType,
         with_clip_featurizer: bool,
@@ -253,15 +250,15 @@
             self._catalogs.import_catalog(
                 dataset=dataset,
                 csv_file_path=catalog_details.catalog_csv_file,
                 table_name=catalog_details.table_name,
             )
 
         self._attach_pipeline(
-            data_type=DataType(dataset.info.data_type),
+            data_type=get_dataset_type(dataset_type=dataset.info.data_type),
             dataset_id=dataset.get_id(),
             featurizer_type=featurizer_type,
             with_clip_featurizer=with_clip_featurizer,
         )
 
         dataset_json = self._get_dataset_json(
             dataset_id=dataset.get_id(), version=dataset.info.latest_version
@@ -308,15 +305,22 @@
         with ProgressBarHelper(total=100) as pbar:
             while not task.has_completed():
                 sleep(5)
                 percent_completed = task.get_progress_info().percent_completed
                 incremental_change = percent_completed - previous_completed
                 pbar.update(incremental_change)
                 previous_completed = percent_completed
-        task.wait_for_completion()
+
+        progress_info: ProgressInfo = task.wait_for_completion()
+        if progress_info.failed:
+            logger.error(
+                f"Failed to ingest dataset with error: {progress_info.error}"
+            )
+
+        return task
 
     @staticmethod
     def _run_workflow(
         progress_manager: ProgressManager,
         dataset_json: am.DataSetJSON,
         data_dir: str,
         catalog_tables_helper: CatalogTablesHelper,
@@ -432,36 +436,7 @@
         pipelines = []
         for pipeline in ds_json.pipelines:  # type: ignore
             pipeline: am.Pipeline
             if pipeline.is_attached:
                 pipelines.append(Pipeline(pipeline))
 
         return pipelines
-
-    def _get_default_image_pipeline(
-        self, attached_pipelines: List[Pipeline]
-    ) -> Optional[Pipeline]:
-        # Find the image pipelines from the list of attached pipelines,
-        # if both full/patch image pipelines are present, prefer patch image
-        # pipeline
-        patch_image_pipeline: Optional[Pipeline] = None
-        full_image_pipeline: Optional[Pipeline] = None
-
-        for pipeline in attached_pipelines:
-            internal_id = pipeline.info.pipeline_internal_id
-
-            if internal_id == Constants.PATCH_IMAGE_PIPELINE_INTERNAL_ID:
-                patch_image_pipeline = pipeline
-                break
-
-            if internal_id == Constants.FULL_IMAGE_PIPELINE_INTERNAL_ID:
-                full_image_pipeline = pipeline
-
-        if patch_image_pipeline is None and full_image_pipeline is None:
-            raise UserError(
-                message="No default pipelines attached to the dataset"
-            )
-        return (
-            patch_image_pipeline
-            if patch_image_pipeline
-            else full_image_pipeline
-        )
```

## akride/core/_filters/partitioners/models.py

```diff
@@ -14,19 +14,25 @@
 
 class ProcessFileInfo(NamedTuple):
     partition_start: int
     partition_end: int
     file_id: int
     file_path: str
     file_name: str
+    frame_height: int
+    frame_width: int
+
     frame_idx_in_blob: int
-    frame_idx_in_file: int = 0
-    total_frames_in_file: int = 1
+    frame_idx_in_file: int
+    total_frames_in_file: int
+
     blob_idx_in_partition: int = 0
 
+    native_fps: Optional[float] = None
+
 
 class DatasetTableInsertValues(NamedTuple):
     partition_start: int
     partition_end: int
     workflow_id: str
     session_id: str
     file_path: str
```

## akride/core/_filters/partitioners/partitioner_filter.py

```diff
@@ -1,13 +1,38 @@
 from abc import ABC, abstractmethod
+from typing import Optional
 
 import akridata_akrimanager_v2 as am
 
+from akride.core._filters.enums import FilterTypes
+from akride.core.constants import Constants
+
 
 class PartitionerFilter(ABC):
-    def __init__(self, dataset_id: str, ccs_api: am.CcsApi):
-        self.dataset_id = dataset_id
-        self.ccs_api = ccs_api
+    PARTITION_TIME_FRAME = Constants.PARTITION_TIME_FRAME
+
+    def __init__(
+        self,
+        dataset_id: str,
+        ccs_api: am.CcsApi,
+        token_size: int,
+        partition_size: Optional[int] = None,
+    ):
+        self._dataset_id = dataset_id
+        self._ccs_api = ccs_api
+
+        self._filter_type = FilterTypes.Partitioner
+
+        self._partition_size = partition_size
+        self._token_size = token_size
 
     @abstractmethod
     def run(self):
         pass
+
+    @abstractmethod
+    def cleanup_token(self, token_num: int):
+        pass
+
+    @abstractmethod
+    def cleanup(self):
+        pass
```

## akride/core/_filters/sink/sink_writer_filter.py

```diff
@@ -1,33 +1,37 @@
 # flake8: noqa  E501
+from abc import abstractmethod
 from datetime import datetime
 from typing import Dict, List, Tuple, Union
 
 import akridata_akrimanager_v2 as am
 import akridata_dsp as dsp
 from pyakri_de_utils.file_utils import get_input_files_dir
 
+from akride._utils.common_utils import get_values_in_batches
 from akride._utils.store_utils import upload_file_to_data_store
 from akride.core._filters.sink.models import SinkWriterFilterInput
 from akride.core.constants import Constants
 from akride.core.exceptions import ServerError
 
 
 class SinkWriterFilter:
     def __init__(
         self,
         filter_input: SinkWriterFilterInput,
         workflow_api: am.WorkflowsApi,
         dsp_dataset_api: dsp.DatasetApi,
         ccs_api: am.CcsApi,
+        ccs_api_batch_size: int = Constants.CCS_API_BATCH_SIZE,
     ):
         self._filter_input = filter_input
         self._workflow_api = workflow_api
         self._dsp_dataset_api: dsp.DatasetApi = dsp_dataset_api
         self._ccs_api = ccs_api
+        self._ccs_batch_size = ccs_api_batch_size
 
     def run_from_input_dir(
         self,
         blobs_dir: str,
         coreset_dir: str,
         sketch_dir: str,
         projections_dir: str,
@@ -144,24 +148,25 @@
     def _update_dataset_partition(
         self,
         partition_id: str,
         partition_start: int,
         partition_end: int,
         store_path_map: Dict[am.DatastoreFileType, str],
     ):
+
         partition_create_request = dsp.PipelinePartitionCreateRequest(
             partition_end=partition_end,
             partition_start=partition_start,
             projections=store_path_map[am.DatastoreFileType.PROJECTIONS],
             blobs=[store_path_map[am.DatastoreFileType.BLOBS]],
             sketch=store_path_map[am.DatastoreFileType.SKETCH],
             thumbnail_blobs=[store_path_map[am.DatastoreFileType.THUMBNAIL]],
             coreset=store_path_map[am.DatastoreFileType.CORESET],
-            start_frame_indices=[0],
-            img_end_indices=[len(self._filter_input.file_metadata_list) - 1],
+            start_frame_indices=[self._get_start_frame_indices()],
+            img_end_indices=[self._get_end_frame_indices()],
         )
 
         self._dsp_dataset_api.update_dataset_partition(
             partition_id=partition_id,
             session_id=self._filter_input.session_id,
             pipeline_id=(
                 self._filter_input.pipeline_tables_info.get_pipeline_id()
@@ -196,32 +201,21 @@
                 store_path_map[am.DatastoreFileType.PROJECTIONS],
                 store_path_map[am.DatastoreFileType.SKETCH],
                 store_path_map[am.DatastoreFileType.THUMBNAIL],
             ]
         ]
 
         # populate insert values for primary table
-        primary_table_insert_values: List[List[Union[int, str, datetime]]] = []
-        for file_info in self._filter_input.file_metadata_list:
-            primary_table_insert_values.append(
-                [
-                    partition_start,
-                    partition_end,
-                    self._filter_input.workflow_id,
-                    self._filter_input.session_id,
-                    file_info.frame_idx_in_blob,
-                    file_info.blob_idx_in_partition,
-                    file_info.file_path,
-                    datetime.now(),
-                    file_info.file_id,
-                    file_info.frame_idx_in_file,
-                    file_info.file_name,
-                    file_info.total_frames_in_file,
-                ]
-            )
+        primary_table_insert_values: List[
+            List[Union[int, str, datetime]]
+        ] = self._get_primary_table_values(
+            partition_start=partition_start,
+            partition_end=partition_end,
+            filter_input=self._filter_input,
+        )
 
         pipeline_tables_info = self._filter_input.pipeline_tables_info
         # Insert entries to db
         for abs_table_name, columns, values in [
             (
                 pipeline_tables_info.get_blobs_abs_table(),
                 Constants.BLOB_TABLE_COLUMNS,
@@ -230,19 +224,47 @@
             (
                 pipeline_tables_info.get_summary_abs_table(),
                 Constants.SUMMARY_TABLE_COLUMNS,
                 summary_table_insert_values,
             ),
             (
                 pipeline_tables_info.get_primary_abs_table(),
-                Constants.PRIMARY_TABLE_COLUMNS,
+                self._get_primary_table_columns(),
                 primary_table_insert_values,
             ),
         ]:
-            self._ccs_api.insert_data_in_catalog_table(
-                am.InsertCatalogData(
-                    dataset_id=self._filter_input.dataset_id,
-                    columns=columns,
-                    values=values,
-                    abs_table_name=abs_table_name,
+            if values and len(columns) != len(values[0]):
+                raise ServerError("Value length differs from column length!")
+
+            for values_batch in get_values_in_batches(
+                values=values, batch_size=self._ccs_batch_size
+            ):
+                self._ccs_api.insert_data_in_catalog_table(
+                    am.InsertCatalogData(
+                        dataset_id=self._filter_input.dataset_id,
+                        columns=columns,
+                        values=values_batch,
+                        abs_table_name=abs_table_name,
+                    )
                 )
-            )
+
+    @staticmethod
+    @abstractmethod
+    def _get_primary_table_columns():
+        pass
+
+    @abstractmethod
+    def _get_primary_table_values(
+        self,
+        partition_start: int,
+        partition_end: int,
+        filter_input: SinkWriterFilterInput,
+    ):
+        pass
+
+    @abstractmethod
+    def _get_start_frame_indices(self) -> int:
+        pass
+
+    @abstractmethod
+    def _get_end_frame_indices(self) -> int:
+        pass
```

## akride/core/conf/pylogconf.yaml

```diff
@@ -5,19 +5,21 @@
   standard:
     fmt: "%(asctime)s,%(msecs)d | %(levelname)-8s | %(filename)15s | %(threadName)10s | %(funcName)12s:%(lineno)d | %(message)s"
     (): "akride.core._log.PPrintFormatter"
 
 handlers:
   console:
     class: logging.StreamHandler
-    level: INFO
+    level: DEBUG
     formatter: standard
+  null_handler:
+    class: logging.NullHandler
+
+root:
+  level: DEBUG
+  handlers: [null_handler, console]
 
 loggers:
-  pyakri_de_filters:
-    level: INFO
-    handlers: [console]
-    propagate: yes
   akride:
-    level: INFO
-    handlers: [console]
-    propagate: yes
+    level: DEBUG
+    handlers: [null_handler, console]
+    propagate: no
```

## akride/core/models/progress_info.py

```diff
@@ -4,7 +4,9 @@
 
 # Class representing progress information for an operation.
 @dataclass
 class ProgressInfo:
     percent_completed: float
     message: Optional[str] = None
     completed: bool = False
+    error: str = None
+    failed: bool = False
```

## Comparing `akride/core/_filters/partitioners/ingest_partitioner_filter.py` & `akride/core/_filters/partitioners/ingest/ingest_partitioner_filter.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,23 +24,34 @@
         dataset: am.DataSetJSON,
         data_dir: str,
         session_id: str,
         workflow_id: str,
         dataset_tables_info: DatasetTablesInfo,
         ccs_api: am.CcsApi,
         ingest_step: ProgressStep,
+        partition_size: int,
+        token_size: int,
     ):
-        super().__init__(dataset_id=dataset.id, ccs_api=ccs_api)
+        super().__init__(
+            dataset_id=dataset.id,
+            ccs_api=ccs_api,
+            partition_size=partition_size,
+            token_size=token_size,
+        )
+
         self._data_dir = data_dir
         self._dataset = dataset
         self._dataset_tables_info = dataset_tables_info
         self._session_id = session_id
         self._workflow_id = workflow_id
         self._ingest_step_progress = ingest_step
 
+    def get_total_partitions(self, new_files: List) -> int:
+        return math.ceil(len(new_files) / self._partition_size)
+
     def run(self):
         new_files = []
         partition_start = 0
 
         (
             next_file_id,
             next_partition_id,
@@ -49,50 +60,49 @@
         glob_pattern = self._dataset.dataset_spec.glob
         glob_pattern = (
             glob_pattern.replace("*", ".*") if glob_pattern else None
         )
 
         files_generator = get_input_files_batch(
             directory=self._data_dir,
-            batch_size=Constants.INGEST_WF_TOKEN_SIZE,
+            batch_size=self._token_size,
             glob_pattern=glob_pattern,
         )
         for files in files_generator:
             new_files += self._get_new_files(files)
 
         logger.debug(f"Files to be ingested: {len(new_files)}")
 
-        total_tokens = math.ceil(
-            len(new_files) / Constants.INGEST_FILES_COUNT_IN_ONE_PARTITION
-        )
+        total_partitions = self.get_total_partitions(new_files)
 
-        self._ingest_step_progress.set_total_steps(total=total_tokens)
+        self._ingest_step_progress.set_total_steps(total=total_partitions)
 
         for partition_batch in get_files_in_batches(
             file_list=new_files,
-            batch_size=Constants.INGEST_FILES_COUNT_IN_ONE_PARTITION,
+            batch_size=self._partition_size,
         ):
             for token_batch in get_files_in_batches(
                 file_list=partition_batch,
-                batch_size=Constants.INGEST_WF_TOKEN_SIZE,
+                batch_size=self._token_size,
             ):
                 logger.debug(
                     f"Ingesting data for token size: {len(token_batch)}"
                 )
-                partition_end = partition_start + Constants.PARTITION_SIZE - 1
+                partition_end = partition_start + self.PARTITION_TIME_FRAME - 1
                 self._ingest_data_to_dataset_tables(
                     token_batch,
                     partition_start,
                     partition_end,
                     next_file_id,
                     next_partition_id,
                 )
-                next_file_id += Constants.INGEST_WF_TOKEN_SIZE
+                next_file_id += self._token_size
+
+            partition_start += self.PARTITION_TIME_FRAME
 
-            partition_start += Constants.PARTITION_SIZE
             next_partition_id += 1
             self._ingest_step_progress.increment_processed_steps(1)
 
     def _ingest_data_to_dataset_tables(
         self,
         files: List[str],
         partition_start: int,
@@ -136,27 +146,27 @@
             ),
             (
                 TableNames.PARTITIONER_FILES.value,
                 Constants.PARTITIONED_TABLE_COLUMNS,
                 partitioned_table_insert_values_list,
             ),
         ]:
-            self.ccs_api.insert_data_in_catalog_table(
+            self._ccs_api.insert_data_in_catalog_table(
                 insert_catalog_data=am.InsertCatalogData(
                     dataset_id=self._dataset.id,
                     table_name=table_name,
                     values=values,
                     columns=columns,
                 )
             )
 
     def _get_next_file_id_and_partition_id(self) -> Tuple:
         response: am.CCSFetchMaxFileIdPartitionIdResponse = (
-            self.ccs_api.fetch_max_fileid_partitionid(
-                dataset_id=self.dataset_id,
+            self._ccs_api.fetch_max_fileid_partitionid(
+                dataset_id=self._dataset_id,
                 abs_table_name=(
                     self._dataset_tables_info.get_partitioned_abs_table()
                 ),
                 is_fetch_max_partition=True,
             )
         )
         max_file_id = response.max_file_id
@@ -168,26 +178,26 @@
         )
 
         return next_file_id, next_partition_id
 
     def _get_new_files(self, filepath_objs: List[Path]) -> List[str]:
         file_paths = [str(filepath) for filepath in filepath_objs]
         checkpointing_response: am.RegisterCheckpointingResponse = (
-            self.ccs_api.register_checkpointing_query(
+            self._ccs_api.register_checkpointing_query(
                 am.RegisterCheckpointingRequest(
                     dataset_id=self._dataset.id,
                     file_paths=file_paths,
                 )
             )
         )
         new_files = []
         for index, file_path in enumerate(file_paths):
             if checkpointing_response.is_file_path_unprocessed[index]:
                 new_files.append(file_path)
 
         return new_files
 
-    def get_tokens_processed(self):
-        return self._tokens_processed
+    def cleanup(self):
+        pass
 
-    def get_total_tokens(self):
-        return self._total_tokens
+    def cleanup_token(self, token_num: int):
+        pass
```

## Comparing `akride/core/_filters/partitioners/process_partitioner_filter.py` & `akride/_utils/video_splitter/splitter.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,177 +1,184 @@
-import math
-import os
-from dataclasses import dataclass
-from typing import Any, List, Tuple
-
-import akridata_akrimanager_v2 as am
-import pandas as pd
-from pyakri_de_utils.arrow_utils import write_arrow_from_df
-from pyakri_de_utils.file_utils import create_directory
-
-from akride import logger
-from akride._utils.catalog.pipeline_tables_info import PipelineTablesInfo
-from akride._utils.file_utils import copy_files_to_dir, get_file_name_from_path
-from akride._utils.progress_manager.manager import ProgressStep
-from akride.core._filters.partitioners.models import ProcessFileInfo
-from akride.core._filters.partitioners.partitioner_filter import (
-    PartitionerFilter,
+import re
+from pathlib import Path
+from typing import List
+
+from pyakri_de_utils.file_utils import (
+    create_directories,
+    get_input_files_batch,
 )
-from akride.core.constants import Constants
 
+from akride import Constants, logger
+from akride._utils.common_utils import get_random_uuid
+from akride._utils.file_utils import (
+    concat_file_paths,
+    get_json_from_file,
+    get_sorted_dirs_from_path,
+)
+from akride._utils.resource_utils import get_video_splitter_script
+from akride._utils.shell_utils import run_subprocess
+from akride._utils.video_splitter.models import (
+    FrameInfo,
+    SplitterDirs,
+    VideoProps,
+    VideoSplitOut,
+    VideoSplitterPartition,
+)
+from akride.core._filters.enums import FilterTypes
+from akride.core.exceptions import ServerError
+
+
+class VideoSplitter:
+    METADATA_FILE = ".METADATA.txt"
 
-@dataclass
-class ProcessTokenInfo:
-    file_info_list: List[ProcessFileInfo]
-    file_meta_list: List[List[Any]]
-    files: List[str]
-    token_number: int
-    total_num_tokens: int
+    OUTPUT_PREFIX = concat_file_paths(
+        FilterTypes.Partitioner.value, "outputs", "o1"
+    )
 
+    METADATA_DIR = "metadata"
 
-class ProcessPartitionerFilter(PartitionerFilter):
-    DF_COLUMNS = ["file_id", "filename", "frame_idx_in_file"]
-    DEST_ARROW_FILE = "0-1"
+    SPLIT_VIDEO_SCRIPT = get_video_splitter_script("split_video.sh")
 
     def __init__(
         self,
-        dataset_id: str,
-        partitioned_abs_table: str,
-        pipeline_info: PipelineTablesInfo,
-        ccs_api: am.CcsApi,
-        process_step: ProgressStep,
+        sampling_rate: float,
+        output_format: str = "jpg",
+        output_file_name: str = "frame",
+        chunk_size: int = Constants.VIDEO_CHUNK_SIZE,
+        output_parent_dir: str = Constants.AKRIDE_TMP_DIR,
     ):
-        super().__init__(dataset_id=dataset_id, ccs_api=ccs_api)
-        self._pipeline_info = pipeline_info
-        self._partitioned_abs_table = partitioned_abs_table
+        self._output_format = output_format
+        self._output_file_name = output_file_name
+        self._sampling_rate = sampling_rate
+        self._chunk_size = chunk_size
 
-        self._process_step = process_step
+        self._output_parent_dir = output_parent_dir
 
-    def run(self):
-        pipeline_name = self._pipeline_info.get_pipeline_name()
-        logger.debug(
-            f"Getting un-processed files for pipeline {pipeline_name}"
+    def _get_output_dir_for_splitter(self, token_num: int):
+        return concat_file_paths(
+            self._output_parent_dir, get_random_uuid(), str(token_num)
         )
-        return self.get_tokenized_unprocessed_files()
 
-    def get_tokenized_unprocessed_files(self):
-        partition_start = 0
-        primary_table_name = self._pipeline_info.get_primary_abs_table()
+    def _get_dirs(
+        self, file: str, out_dir: str, token_num: int
+    ) -> SplitterDirs:
+        metadata_dir = concat_file_paths(out_dir, self.METADATA_DIR)
+        metadata_file = concat_file_paths(metadata_dir, self.METADATA_FILE)
 
-        next_file_id = self._get_next_file_id(primary_table_name)
+        output_parent_dir = self._get_output_dir_for_splitter(
+            token_num=token_num
+        )
+
+        create_directories([output_parent_dir, metadata_dir])
 
-        # Tokenize and return metadata details
-        token_count = self._get_token_count(
-            primary_table_name=primary_table_name
+        return SplitterDirs(
+            input_file=file,
+            out_parent_dir=output_parent_dir,
+            metadata_file=metadata_file,
         )
 
-        self._process_step.set_total_steps(token_count)
+    @staticmethod
+    def _get_file_index(file_path: Path):
+        # Input string
+        filename = file_path.name
+
+        # Search for the pattern in the input string
+        matches = re.findall(r"\d{7}", filename)
+        if matches:
+            return int(matches[0]) - 1
 
-        token_index = 0
-        while token_index < token_count:
-            files = self._get_unprocessed_files(primary_table_name)
-            token_number = token_index + 1
+        raise ValueError("Failed to get frame index")
 
-            (
-                file_info_list,
-                filemeta_arr_list,
-            ) = self._prepare_file_meta_and_file_info_list(
-                files=files,
-                partition_start=partition_start,
-                file_id=next_file_id,
+    @classmethod
+    def _get_video_partitions(
+        cls,
+        parent_dir: str,
+    ) -> (List[VideoSplitterPartition], int):
+        partitions: List[VideoSplitterPartition] = []
+        total_frames = 0
+
+        partition_dirs = get_sorted_dirs_from_path(path=parent_dir)
+
+        # Iterate through each item in the parent directory
+        for partition_num, subdir in enumerate(partition_dirs):
+            partition_dir = concat_file_paths(parent_dir, subdir)
+
+            output_dir = concat_file_paths(partition_dir, cls.OUTPUT_PREFIX)
+            metadata_dir = concat_file_paths(partition_dir, cls.METADATA_DIR)
+
+            file_paths = next(
+                get_input_files_batch(
+                    directory=partition_dir, extension=".jpg"
+                )
             )
 
-            yield ProcessTokenInfo(
-                file_info_list=file_info_list,
-                file_meta_list=filemeta_arr_list,
-                token_number=token_number,
-                total_num_tokens=token_count,
-                files=files,
-            )
+            frames = []
+            for file_path in file_paths:
+                frames.append(
+                    FrameInfo(
+                        index=cls._get_file_index(file_path), file=file_path
+                    )
+                )
 
-            partition_start += Constants.PARTITION_SIZE
-            next_file_id += Constants.PROCESS_WF_TOKEN_SIZE
-            token_index += 1
+            if frames:
+                partitions.append(
+                    VideoSplitterPartition(
+                        num=partition_num + 1,
+                        out_dir=output_dir,
+                        metadata_dir=metadata_dir,
+                        parent_dir=partition_dir,
+                        frames=frames,
+                    )
+                )
+                total_frames += len(file_paths)
 
-    @staticmethod
-    def prepare_output_dir(files: List[str], output_dir: str):
-        copy_files_to_dir(files, output_dir)
+        return partitions, total_frames
 
-    def _get_token_count(self, primary_table_name: str) -> int:
-        response: am.CCSFetchUnprocessedFileCntResponse = (
-            self.ccs_api.fetch_unprocessed_file_count(
-                dataset_id=self.dataset_id,
-                primary_table=primary_table_name,
-                partition_table=self._partitioned_abs_table,
-            )
-        )
-        token_count = math.ceil(
-            response.file_count / Constants.PROCESS_WF_TOKEN_SIZE
+    def _get_video_metadata(self, metadata_file: str) -> VideoProps:
+        metadata = get_json_from_file(file=metadata_file)
+
+        return VideoProps(
+            width=metadata["width"],
+            height=metadata["height"],
+            fps=metadata["fps"],
+            duration=metadata["duration"],
         )
-        return token_count
 
-    def _get_unprocessed_files(self, primary_table_name: str) -> List[str]:
-        response: am.CCSFetchUnprocessedFileNamesResponse = (
-            self.ccs_api.fetch_unprocessed_file_names(
-                dataset_id=self.dataset_id,
-                primary_table=primary_table_name,
-                partition_table=self._partitioned_abs_table,
-                batch_size=Constants.PROCESS_WF_TOKEN_SIZE,
-            )
+    def split(self, file: str, out_dir: str, token_num: int) -> VideoSplitOut:
+        directories: SplitterDirs = self._get_dirs(
+            file=file, out_dir=out_dir, token_num=token_num
         )
-        return response.file_names
 
-    @classmethod
-    def _prepare_file_meta_and_file_info_list(
-        cls,
-        files: List[str],
-        partition_start: int,
-        file_id: int,
-    ) -> Tuple[List[ProcessFileInfo], List[List[Any]]]:
-        filemeta_arr_list = []
-        file_info_list = []
-        frame_idx_in_blob = 0
-        partition_end = partition_start + Constants.PARTITION_SIZE - 1
-        frame_idx_in_file = 0
-
-        for file in files:
-            file_info_list.append(
-                ProcessFileInfo(
-                    file_path=file,
-                    file_id=file_id,
-                    frame_idx_in_blob=frame_idx_in_blob,
-                    partition_start=partition_start,
-                    partition_end=partition_end,
-                    file_name=get_file_name_from_path(file),
-                    frame_idx_in_file=frame_idx_in_file,
-                )
-            )
-            filemeta_arr_list.append([file_id, file, frame_idx_in_file])
-            frame_idx_in_blob += 1
-            file_id += 1
+        script_args = [
+            self._chunk_size,
+            self._sampling_rate,
+            directories.input_file,
+            directories.out_parent_dir,
+            directories.metadata_file,
+            out_dir,
+        ]
 
-        return file_info_list, filemeta_arr_list
+        result = run_subprocess(self.SPLIT_VIDEO_SCRIPT, *script_args)
 
-    @classmethod
-    def prepare_metadata_dir(
-        cls, metadata_dir: str, filemeta_list: List[List[Any]]
-    ):
-        data_frame_to_write = pd.DataFrame(
-            filemeta_list, columns=cls.DF_COLUMNS
+        # Raise exception if video splitter failed
+        if result.has_failed():
+            raise ServerError(
+                f"Failed to split video with error {result.stderr}"
+            )
+
+        # Read metadata
+        video_metadata: VideoProps = self._get_video_metadata(
+            directories.metadata_file
         )
-        create_directory(metadata_dir)
 
-        dst_arrow_file_path = os.path.join(metadata_dir, cls.DEST_ARROW_FILE)
+        # Get partitions
+        partitions, total_frames = self._get_video_partitions(
+            parent_dir=directories.out_parent_dir
+        )
 
-        write_arrow_from_df(data_frame_to_write, dst_arrow_file_path)
+        logger.debug(f"Num partitions are {len(partitions)}")
 
-    def _get_next_file_id(self, primary_table_name: str) -> int:
-        response: am.CCSFetchMaxFileIdPartitionIdResponse = (
-            self.ccs_api.fetch_max_fileid_partitionid(
-                dataset_id=self.dataset_id,
-                abs_table_name=primary_table_name,
-                is_fetch_max_partition=False,
-            )
+        return VideoSplitOut(
+            props=video_metadata,
+            total_frames=total_frames,
+            partitions=partitions,
         )
-        max_file_id = response.max_file_id
-        next_file_id = 0 if max_file_id is None else max_file_id + 1
-        return next_file_id
```

## Comparing `akride-0.4.16.dist-info/METADATA` & `akride-0.4.23.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akride
-Version: 0.4.16
+Version: 0.4.23
 Summary: Data Explorer Client SDK
 Home-page: https://github.com/akridata-ai/akride-examples
 License: Proprietary
 Project-URL: Documentation, https://akridata-akride.readthedocs-hosted.com/en/latest/
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
@@ -13,14 +13,15 @@
 Requires-Dist: importlib-metadata
 Requires-Dist: akridata-akrimanager-v2 <1.23.0.dev0,>=1.22.0.dev0
 Requires-Dist: akridata-dsp <2.15.0.dev0,>=2.14.0.dev0
 Requires-Dist: requests >=2.2
 Requires-Dist: attrs >=23.1.0
 Requires-Dist: yarl >=1.9.2
 Requires-Dist: tqdm >=4.66.1
+Requires-Dist: pydantic <3,>=2.7.1
 Requires-Dist: pyakri-de-utils <1.23.0.dev0,>=1.22.0.dev0
 Provides-Extra: cpu
 Requires-Dist: pyakri-de-filters[cpu] <1.23.0.dev0,>=1.22.0.dev0 ; extra == 'cpu'
 Provides-Extra: gpu
 Requires-Dist: pyakri-de-filters[gpu] <1.23.0.dev0,>=1.22.0.dev0 ; extra == 'gpu'
 Provides-Extra: testing
 Requires-Dist: setuptools ; extra == 'testing'
@@ -106,8 +107,12 @@
 
 ---
 
 For more information about AkriData, please visit [akridata.ai](https://www.akridata.ai).
 
 
 ## Docker command to ingest data
-docker run -it -v ${PWD}/data:/data akridata/akride:latest akride ingest -n <dataset_name> -d <dataset_id> -i /data -e <de_endpoint> -a <api_key>
+### CPU docker image
+docker run -v ${PWD}/data:/data akridata/akride:latest akride ingest [-n <dataset_name> | -d <dataset_id>] -i /data -e <de_endpoint> -a <api_key>
+
+### GPU docker image
+docker run --gpus=all -v ${PWD}/data:/data akridata/akride-gpu:latest akride ingest [-n <dataset_name> | -d <dataset_id>] -i /data -e <de_endpoint> -a <api_key>
```

## Comparing `akride-0.4.16.dist-info/RECORD` & `akride-0.4.23.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,75 +1,96 @@
-akride/__init__.py,sha256=_4QgfqdhPVgQ9Yl2QaPM_JYBfed0j5BxoIGN7tYkNeg,2119
+akride/__init__.py,sha256=zF_z0JTVySZPoRu3WRaeJdurbDaJyR7c_nfgA3NFiW8,2129
 akride/background_task_manager.py,sha256=f5mMGM8Ji8VxYGV8S7JRU2dkr4ygFVwiGK_pgnVNZik,2499
-akride/client.py,sha256=YiehxpjHTh7ZIdZqPEMYjXaCs1mRxsXZqO4oB8Ko8MU,35983
-akride/main.py,sha256=LS-Y2ucIn_GTzd73Tw0ruCsg4vMxQvFLgLpKSOclMCo,2563
+akride/client.py,sha256=sUYroUYezTE9ODIvC-P1Vae3A2qaeKYOJHJQih3DV50,36516
+akride/main.py,sha256=PtZnFSIIyCHB8t61k5JQ2b-wDaxoq0fqE9DsXF4KjtQ,2706
 akride/_utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-akride/_utils/background_task_helper.py,sha256=Yl-LOZ9abwVA-0owda81lrEgRNLkl4kJ2xF1sNrJFSo,2904
+akride/_utils/background_task_helper.py,sha256=SmjPfcY8MjZPdZ1N9x8Lo4CBwGwkly1nv8VuDXItJjI,3015
 akride/_utils/class_executor.py,sha256=y7qV7IRDiz0Gb1BM5oI2s7pcBUObj3B46mHdiTwc62o,1357
+akride/_utils/common_utils.py,sha256=_RCEkoh8T6JX8a9zLeuop1ZJqqwclg-ZdEE7esZcWqI,254
+akride/_utils/dataset_utils.py,sha256=2AiEqTVK6tmSFyeOA2PoigU7X0B-O4rOG5UEkojPA6g,524
 akride/_utils/exception_utils.py,sha256=ElOf5shueLzmC0YCD1p7PmsPhN1ZWXWZDZ56Frp4Q5k,2624
-akride/_utils/file_utils.py,sha256=zmiooZXaFziN6jaK4b3aI1hDKWUQqN8LWguew-I0_Gw,584
+akride/_utils/file_utils.py,sha256=B4UxkuujiGdUhiA-J4GduxHE73eU_zy9ubq5JRJTwvE,1668
 akride/_utils/job_creator.py,sha256=0vPVSr51N_4cspxz_TAuCL58ZHyuXQbFl0Px8cIp5-s,14188
 akride/_utils/platform.py,sha256=nutg_fRstZOGVryc3L78tZeuSG3H8eH_c3Pjyt41gIA,278
 akride/_utils/progress_bar_helper.py,sha256=68mwZAUFYM372AMEbNve5r7Tip4CUHUpkxYA1amp2AA,454
 akride/_utils/proxy_utils.py,sha256=QgRh4HGXisU0sbp-xN8eDvtS5Ic6HGgSKQ9ZRlaRE_k,1459
-akride/_utils/resource_utils.py,sha256=rN00dPs3vxu73m27xTeC-KWsRg6B0jTykkb_KKemeQ0,172
-akride/_utils/retry_helper.py,sha256=80_KOJPAGaSKxduWSsQoim0RqA1W_gUjmomrFe-dT1U,595
+akride/_utils/resource_utils.py,sha256=hKACjKitnqn-Kgc7Ve_t2SOUO8hKhrd7PeeU7LkIWzs,413
+akride/_utils/retry_helper.py,sha256=luV4yY8QxjeZRu687uySlyUBNq6j_dNgjgKkKkZ1r-w,595
+akride/_utils/shell_utils.py,sha256=R5xA2XlHUHznoH2-4uoFPF1uOKYIFFy6xibdVN-mITQ,1094
 akride/_utils/store_utils.py,sha256=8FDHFXACLAh8jNKNfjkhCyJ2j89LZ8V6uKz7zeNYAxQ,811
 akride/_utils/workflow_helper.py,sha256=9oCxx4cU1UcClMaEB5jMe5NZXRChg4gXGXVJTpsimSQ,473
 akride/_utils/catalog/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 akride/_utils/catalog/catalog_tables_helper.py,sha256=V6CPCRLD50yTfc02dU9eB3IbvSh1vfx8rgWfqqZT3do,779
 akride/_utils/catalog/dataset_tables_info.py,sha256=em9hogSeLs1xzsQNo3ITiEGGyZzHZziJDE09LQmhZlE,574
 akride/_utils/catalog/enums.py,sha256=2pV69NLp4Z4dQHgM7prOFXyiLv1PR0Car_7fCn_6Fik,194
 akride/_utils/catalog/pipeline_tables_info.py,sha256=0HvVx9BdCgqNkESveqEcEhEsOj3BOJVrtOhanO0p5hs,890
+akride/_utils/catalog/string_utils.py,sha256=i33FUA3ZoBETHILkecvklQ0g5SqCsrsKuN2MsaR06Qw,193
 akride/_utils/catalog/tables_info.py,sha256=PCgCghF5RacYd6GA0YpmCwVpCavQ0M8i80F1BqmkJvY,541
 akride/_utils/pipeline/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-akride/_utils/pipeline/constants.py,sha256=JkCjLeuK9RT9ubxviRDfXIjFFHxvixJNi9axBJ5kHqk,250
-akride/_utils/pipeline/pipeline_helper.py,sha256=u79lyt-TQXCvb_83uyAv3zx8PH0J-7TwMfo4DWxs0Hg,1159
+akride/_utils/pipeline/constants.py,sha256=2THadI9j2G2BwfjEZAeQwLNiOCVzm2xfSzfthXt_WnQ,492
+akride/_utils/pipeline/pipeline_helper.py,sha256=EejHTVPVbpCpsxVlQmDDHGOk-KPoLMQqiwaeVFEQVm4,3288
 akride/_utils/progress_manager/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-akride/_utils/progress_manager/manager.py,sha256=CxqdeYzLczU_DFQ7lK90AxJKX47e-QTyOVE2FsTTkoQ,2037
-akride/_utils/progress_manager/progress_step.py,sha256=FU4Ni4Qmo6GdPdrYfl2JUOZG_D-U7j0EQv7BCn6Fdy4,1646
+akride/_utils/progress_manager/manager.py,sha256=9bA3rTDSi6U9mFZsNJGal-9aRHXRw-9E44E00G3DQ7Q,2214
+akride/_utils/progress_manager/progress_step.py,sha256=15vb_bDeW79Z9Lyiajr-605MgS0ft63p3gambtuuQ8E,1745
 akride/_utils/rest/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 akride/_utils/rest/requests_session_manager.py,sha256=4c1-g0mkLo_MvMjjKDPlMbNajeQZe8IzDcfzzV6JmEk,528
 akride/_utils/rest/rest_client.py,sha256=MNA42NaJCeDR0A85fzJUgJqFon-LxBDEseVmdR6BJeM,3468
 akride/_utils/rest/utils.py,sha256=5w20_GIqHkgvD08l1zF3xMwefbo2eiJhMiSkg4qTIGs,194
+akride/_utils/video_splitter/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+akride/_utils/video_splitter/models.py,sha256=3qOJidVgAnGokmlzqNNcUckVgrgvjF4sxh6wWW9ppWk,584
+akride/_utils/video_splitter/split_video.sh,sha256=SbO4ysJx0YyfVnE3AQTYBNHdguRe-WFs9f3N0vI9YW4,3344
+akride/_utils/video_splitter/splitter.py,sha256=4yc3a2r7T4WsEwgcLNIQUACVnqUj8BRr0uOi-vYz8EU,5581
 akride/core/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-akride/core/_log.py,sha256=r-ywYP4tuQBSy1OpYz_4hVDOPiOCiWarb_W5ADeytk4,1450
-akride/core/_pipeline_executor.py,sha256=CqIWR_qTVNP4FTl612mWwfVsdDmFbR1ASP0CPj4V43o,15237
-akride/core/constants.py,sha256=deN_w44brWZvvB_YAw6wQ3yfBalIL9s1IDHddIzF-wU,1859
+akride/core/_log.py,sha256=wRyu7-Mw9PtpvqpscXzHGNTWgQGuhNGiSN4DnXRbp24,1728
+akride/core/_pipeline_executor.py,sha256=lOmilHZH0qGKzg3zq9lXXuOcRaz_fjNQ7W_Jhi9u1J8,16577
+akride/core/constants.py,sha256=pXTDgqIkw7O3TCpZw9lFSGAZei-NfuD4kJnwD0GDcOc,2456
 akride/core/enums.py,sha256=oBbLtTjMNVJounpdWaSnTTBZpFeO6RAuJfDvWcmyrho,2309
-akride/core/exceptions.py,sha256=17Xmy_nxzhT8coMaID9ioRhQhOcaaoq9f7lvMoOilxo,1500
+akride/core/exceptions.py,sha256=4uM25NLVCkNDRfynHieA27y4tLGQikhlF7qBNhSj31I,1634
 akride/core/types.py,sha256=hyz3CWVVcPyGK47JJnUumpc6oMfPvZ0tPajdSGyu-vQ,9614
 akride/core/_entity_managers/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 akride/core/_entity_managers/catalog_manager.py,sha256=6JyeJF-metpdxNFSA8HigdCjEgilb9TdpNVt_U43rh8,18527
-akride/core/_entity_managers/dataset_manager.py,sha256=Qxu9lStk9K4l_RLqtHxFlavybKhKn4wODsj9ksZtISo,16073
+akride/core/_entity_managers/dataset_manager.py,sha256=dvRBJBVwjWp5mCu65h44J3-AWhN7Ue6vQmLGCsDihOk,15339
 akride/core/_entity_managers/job_manager.py,sha256=OWrJtyL89ppXzcpQ8bCFNZWwytNrCNBpUv_6x0aoooM,30350
 akride/core/_entity_managers/manager.py,sha256=GxUe0oBhNbXyrrThs9S6j7AYF7qJI3FaXjXRbZl3MOo,2238
 akride/core/_entity_managers/resultset_manager.py,sha256=ToNDisHBP6Xb-L5OSEIPDlMvoiCSSErs8b6tV6t8VBI,8702
 akride/core/_entity_managers/subscriptions_manager.py,sha256=q66WO0bmrxJhsHdgFd9dui1EaIxqtkU0a7cIfLRlZSc,1314
+akride/core/_entity_managers/_models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+akride/core/_entity_managers/_models/datasets.py,sha256=VWlxUmOt2EubRTmHiL1DhcU_GMw6ggxK6TvRamlsjW0,1349
 akride/core/_filters/__init__.py,sha256=6CgtXVd_M0GUNJsbv9G939UenkUt91Nu28WDUq3_xwM,140
 akride/core/_filters/enums.py,sha256=NvVxgm3rkWJS0zMxbj7Cyxu2q3ExkYsUTfOedac7dQw,253
 akride/core/_filters/partitioners/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-akride/core/_filters/partitioners/ingest_partitioner_filter.py,sha256=P5Gc_DZUexU5i4k71HRFMXZTyGAxAp7z8aaBW_3CVKg,6412
-akride/core/_filters/partitioners/models.py,sha256=ZIqpYx-4JUfAO60YTG_AFAa6ooFFjJ9N8OpSO098bv4,696
-akride/core/_filters/partitioners/partitioner_filter.py,sha256=fgzkq45fnSWO_ctJY9wxunad3FWcpN0OtvrCV7xaY2M,288
-akride/core/_filters/partitioners/process_partitioner_filter.py,sha256=6giTjKGInXAOTiMNJ_QJxTl1pno20XYAFtXACY2U2w4,6043
+akride/core/_filters/partitioners/dtos.py,sha256=BNyho_KRZ-G9dip0CJdpuWSi3Ujw0zh11Ih0Ca6rRo0,1035
+akride/core/_filters/partitioners/models.py,sha256=7yzOzhgOBOn9Mloks3tx_IN3Tv4SckuEH53-gzqpPII,773
+akride/core/_filters/partitioners/partitioner_filter.py,sha256=KBg_nZYmPT6wyQ-dqvAXXg0mJSX7kqjqUy7M9WCI73Y,849
+akride/core/_filters/partitioners/partitioner_filter_factory.py,sha256=XYp872tnRGXXOiv51cVG0_vY437KwNR2E-Q3iZ8y4rI,3371
+akride/core/_filters/partitioners/ingest/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+akride/core/_filters/partitioners/ingest/ingest_image_partitioner_filter.py,sha256=hyDE2Mn0vNQzPEzyPWS9NI9eYBGfV7mOTnWb403u4sU,1055
+akride/core/_filters/partitioners/ingest/ingest_partitioner_filter.py,sha256=yOLALE4HPpKKKCHtP80xIb_t2v7GbrB870TQy2W6nfM,6548
+akride/core/_filters/partitioners/ingest/ingest_video_partitioner_filter.py,sha256=J37-3ycy-eEvEoS4QA7f3-18N9a9HGvV0AT9jD8sQGY,1055
+akride/core/_filters/partitioners/process/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+akride/core/_filters/partitioners/process/image_process_partitioner_filter.py,sha256=vX3Ui5yu0dy1lG8ids3xKnlmy5jdB4wrU-z5izJKcn0,3591
+akride/core/_filters/partitioners/process/process_partitioner_filter.py,sha256=7YqOQgbZ_5top-IV31w7OUSVvPrFOL5lpXGGYC_vMTM,9127
+akride/core/_filters/partitioners/process/video_process_partitioner_filter.py,sha256=2gqmnp1wfczwawPwEeHPlkK2iEGG-r9XjSdpExp4uSw,5216
 akride/core/_filters/sink/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+akride/core/_filters/sink/image_sink_writer_filter.py,sha256=NZJIklGYswWT2R5yjz9VZkg30xcHVuPO1Xp1XRWUrlg,1590
 akride/core/_filters/sink/models.py,sha256=0YEzbZ-BpAI17yP3hA8i3yNHjVOvtAk5TXLqVLODcgY,1247
-akride/core/_filters/sink/sink_writer_filter.py,sha256=OHOzjNl5QMpDQFvyrF8fhKvqeTKC27YyjbkYdiJazRc,9178
+akride/core/_filters/sink/sink_writer_factory.py,sha256=ScdGUGgmOBjd1hK9idHjNCSmvkU_EAidWiCOy_isXOA,1318
+akride/core/_filters/sink/sink_writer_filter.py,sha256=Rf4ctYsiBATqwe-OpNhD6bL7jcuu1GLHbt8k3jnQyvY,9646
+akride/core/_filters/sink/video_sink_writer_filter.py,sha256=jqEmLBbORBukW8gPslMMKuRvLlj6kfbwjOocCQHurwg,2281
 akride/core/conf/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-akride/core/conf/pylogconf.yaml,sha256=fS9hD9BqxZePlDCISZUpma-7oKkFKbdhTFkm_BsbsRA,493
+akride/core/conf/pylogconf.yaml,sha256=-AW3PiV47bE1-IRI5vUf-bWt_eZHo5Gfuicpk9zYM4k,533
 akride/core/entities/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 akride/core/entities/catalogs.py,sha256=L1OcKZcL0EC3EOgAfJLIss7ptgJ3-QVDn5jvYgybmVM,796
 akride/core/entities/datasets.py,sha256=4mPUpPOJekjIrIpe_INEH6z9Yq-Q1VcXAkIeQHrIksE,736
 akride/core/entities/entity.py,sha256=sIRYQ69xM6Hrasn7edwgF-J6LjFG6hF7S95zTKe005g,1549
 akride/core/entities/jobs.py,sha256=zaAiYcxmNkmF_ADuGk215K_W81YyO2uoZNQQTJUL844,5565
 akride/core/entities/pipeline.py,sha256=CF9hqAUIET75JhWc0nUm9oRDFIPf7lXOnMosbrIlfyw,436
 akride/core/entities/resultsets.py,sha256=6ZiJGB_MGOfrgoSQgMyreLhxXH60Ygz7scLohGTpue0,955
 akride/core/models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 akride/core/models/catalog_details.py,sha256=JGDYdWM5EmF0f0vRHGaH6XtixqJkfH1b93Fgj3t3A1U,398
-akride/core/models/progress_info.py,sha256=5QBfsMe74CpYmmbnjYtr8CWsjhlhgb6yuwbS1srr_YQ,246
-akride-0.4.16.dist-info/LICENSE.txt,sha256=rCByYn1oXQOgnl6cQSmp1uiJlT4E0QM0PDchFzJimjo,130
-akride-0.4.16.dist-info/METADATA,sha256=bBQ3cJngbSIaR7iCszEJ2FczLrg8dE83epZRtA5RRlI,3490
-akride-0.4.16.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-akride-0.4.16.dist-info/entry_points.txt,sha256=fD59ZhGa6sPkQd4H45zttMqxPXTHzJM7vQVJRLpGZns,44
-akride-0.4.16.dist-info/top_level.txt,sha256=qhymMhnBUjXghMz0FSS8l-t6VRF_MXcHLtW9nIP26c0,7
-akride-0.4.16.dist-info/RECORD,,
+akride/core/models/progress_info.py,sha256=OGvquLvhZezVHlBiod5BtrJab85_nMxeVgCHKttn8Ws,293
+akride-0.4.23.dist-info/LICENSE.txt,sha256=rCByYn1oXQOgnl6cQSmp1uiJlT4E0QM0PDchFzJimjo,130
+akride-0.4.23.dist-info/METADATA,sha256=g-659Sf78ptOmjcA_O_TRJjABn7PZPHzGdD1JTqgKQ8,3729
+akride-0.4.23.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+akride-0.4.23.dist-info/entry_points.txt,sha256=fD59ZhGa6sPkQd4H45zttMqxPXTHzJM7vQVJRLpGZns,44
+akride-0.4.23.dist-info/top_level.txt,sha256=qhymMhnBUjXghMz0FSS8l-t6VRF_MXcHLtW9nIP26c0,7
+akride-0.4.23.dist-info/RECORD,,
```

