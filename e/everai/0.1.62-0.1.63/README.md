# Comparing `tmp/everai-0.1.62-py3-none-any.whl.zip` & `tmp/everai-0.1.63-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 440667 bytes, number of entries: 424
+Zip file size: 350381 bytes, number of entries: 335
 -rw-r--r--  2.0 unx       66 b- defN 24-Apr-24 07:43 everai/__init__.py
--rw-r--r--  2.0 unx     1214 b- defN 24-Apr-28 08:33 everai/constants.py
--rw-r--r--  2.0 unx       24 b- defN 24-May-24 09:12 everai/version.py
+-rw-r--r--  2.0 unx     1269 b- defN 24-Jun-03 12:07 everai/constants.py
+-rw-r--r--  2.0 unx       24 b- defN 24-Jun-03 12:31 everai/version.py
 -rw-r--r--  2.0 unx       40 b- defN 24-Mar-15 10:09 everai/api/__init__.py
--rw-r--r--  2.0 unx    15133 b- defN 24-May-09 07:21 everai/api/api.py
+-rw-r--r--  2.0 unx    15186 b- defN 24-Jun-03 12:29 everai/api/api.py
 -rw-r--r--  2.0 unx      208 b- defN 24-Apr-15 11:24 everai/app/__init__.py
--rw-r--r--  2.0 unx     3732 b- defN 24-May-07 10:58 everai/app/app.py
--rw-r--r--  2.0 unx    12594 b- defN 24-May-21 04:29 everai/app/app_manager.py
+-rw-r--r--  2.0 unx     3726 b- defN 24-Jun-03 12:21 everai/app/app.py
+-rw-r--r--  2.0 unx    12746 b- defN 24-Jun-03 12:26 everai/app/app_manager.py
 -rw-r--r--  2.0 unx     1791 b- defN 24-Apr-24 07:37 everai/app/app_runner.py
 -rw-r--r--  2.0 unx     3486 b- defN 24-May-06 13:55 everai/app/app_runtime.py
 -rw-r--r--  2.0 unx     2568 b- defN 24-Apr-23 14:51 everai/app/app_setup.py
 -rw-r--r--  2.0 unx     1325 b- defN 24-May-13 12:03 everai/app/autocaling_handler.py
--rw-r--r--  2.0 unx     2650 b- defN 24-May-16 11:25 everai/app/context.py
+-rw-r--r--  2.0 unx     2779 b- defN 24-Jun-03 12:08 everai/app/context.py
 -rw-r--r--  2.0 unx     3004 b- defN 24-Apr-28 08:38 everai/app/service.py
 -rw-r--r--  2.0 unx      210 b- defN 24-Mar-28 12:25 everai/app/typing.py
 -rw-r--r--  2.0 unx      327 b- defN 24-Mar-12 08:39 everai/app/volume_request.py
 -rw-r--r--  2.0 unx      310 b- defN 24-Apr-23 15:52 everai/autoscaling/__init__.py
 -rw-r--r--  2.0 unx      901 b- defN 24-Apr-23 13:29 everai/autoscaling/action.py
 -rw-r--r--  2.0 unx      291 b- defN 24-Apr-23 15:51 everai/autoscaling/autoscaling_policy.py
 -rw-r--r--  2.0 unx      184 b- defN 24-Apr-23 13:29 everai/autoscaling/autoscaling_policy.pyi
@@ -31,14 +31,15 @@
 -rw-r--r--  2.0 unx     1407 b- defN 24-Apr-23 07:57 everai/commands/app/create.py
 -rw-r--r--  2.0 unx      676 b- defN 24-Apr-23 07:57 everai/commands/app/deploy.py
 -rw-r--r--  2.0 unx      765 b- defN 24-Apr-23 07:57 everai/commands/app/get.py
 -rw-r--r--  2.0 unx      791 b- defN 24-Apr-24 06:22 everai/commands/app/list.py
 -rw-r--r--  2.0 unx      773 b- defN 24-Apr-23 07:57 everai/commands/app/pause.py
 -rw-r--r--  2.0 unx      729 b- defN 24-May-21 04:02 everai/commands/app/prepare.py
 -rw-r--r--  2.0 unx      953 b- defN 24-Apr-25 09:11 everai/commands/app/queue.py
+-rw-r--r--  2.0 unx      753 b- defN 24-Jun-03 12:26 everai/commands/app/resume.py
 -rw-r--r--  2.0 unx     3004 b- defN 24-Apr-23 07:57 everai/commands/app/upgrade.py
 -rw-r--r--  2.0 unx     1262 b- defN 24-Apr-23 04:14 everai/commands/app/utils.py
 -rw-r--r--  2.0 unx      122 b- defN 24-Apr-23 06:45 everai/commands/auth/__init__.py
 -rw-r--r--  2.0 unx      889 b- defN 24-Apr-23 07:36 everai/commands/auth/login.py
 -rw-r--r--  2.0 unx      555 b- defN 24-Apr-23 07:03 everai/commands/auth/logout.py
 -rw-r--r--  2.0 unx       77 b- defN 24-Apr-23 06:48 everai/commands/autoscaling/__init__.py
 -rw-r--r--  2.0 unx      973 b- defN 24-Apr-23 08:02 everai/commands/autoscaling/autoscaling.py
@@ -91,15 +92,15 @@
 -rw-r--r--  2.0 unx     3317 b- defN 24-Apr-24 07:31 everai/image/builder.py
 -rw-r--r--  2.0 unx     1046 b- defN 24-Apr-17 14:47 everai/image/image.py
 -rw-r--r--  2.0 unx      223 b- defN 24-Apr-23 08:51 everai/logger/__init__.py
 -rw-r--r--  2.0 unx     1798 b- defN 24-Apr-23 08:57 everai/logger/logger.py
 -rw-r--r--  2.0 unx       70 b- defN 24-Apr-23 14:30 everai/placeholder/__init__.py
 -rw-r--r--  2.0 unx      720 b- defN 24-Apr-23 16:33 everai/placeholder/placeholder.py
 -rw-r--r--  2.0 unx       70 b- defN 24-Apr-25 09:05 everai/queue/__init__.py
--rw-r--r--  2.0 unx     1538 b- defN 24-May-07 11:05 everai/queue/queued_request.py
+-rw-r--r--  2.0 unx     1544 b- defN 24-Jun-03 12:23 everai/queue/queued_request.py
 -rw-r--r--  2.0 unx       79 b- defN 24-Apr-16 14:54 everai/resource_requests/__init__.py
 -rw-r--r--  2.0 unx     1829 b- defN 24-May-24 06:42 everai/resource_requests/resource_requests.py
 -rw-r--r--  2.0 unx      211 b- defN 24-Mar-29 07:26 everai/resource_requests/wellknown.py
 -rw-r--r--  2.0 unx       95 b- defN 24-Apr-23 03:58 everai/runner/__init__.py
 -rw-r--r--  2.0 unx     2595 b- defN 24-May-16 04:22 everai/runner/run.py
 -rw-r--r--  2.0 unx      109 b- defN 24-Apr-23 14:30 everai/secret/__init__.py
 -rw-r--r--  2.0 unx     2118 b- defN 24-Apr-23 13:11 everai/secret/secret.py
@@ -119,308 +120,218 @@
 -rw-r--r--  2.0 unx      616 b- defN 24-Mar-07 07:12 everai/utils/utils.py
 -rw-r--r--  2.0 unx      153 b- defN 24-Mar-14 15:31 everai/utils/verbose.py
 -rw-r--r--  2.0 unx      161 b- defN 24-May-09 07:29 everai/volume/__init__.py
 -rw-r--r--  2.0 unx     2070 b- defN 24-May-09 07:26 everai/volume/name_helper.py
 -rw-r--r--  2.0 unx     5811 b- defN 24-May-16 11:14 everai/volume/volume.py
 -rw-r--r--  2.0 unx    15178 b- defN 24-May-24 07:00 everai/volume/volume_manager.py
 -rw-r--r--  2.0 unx       55 b- defN 24-Apr-23 13:17 everai/worker/__init__.py
--rw-r--r--  2.0 unx     3343 b- defN 24-May-07 10:58 everai/worker/worker.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-21 04:38 generated/__init__.py
--rw-r--r--  2.0 unx     1413 b- defN 24-May-21 04:38 generated/configmaps/__init__.py
--rw-r--r--  2.0 unx    29579 b- defN 24-May-21 04:38 generated/configmaps/api_client.py
--rw-r--r--  2.0 unx      852 b- defN 24-May-21 04:38 generated/configmaps/api_response.py
--rw-r--r--  2.0 unx    14419 b- defN 24-May-21 04:38 generated/configmaps/configuration.py
--rw-r--r--  2.0 unx     5462 b- defN 24-May-21 04:38 generated/configmaps/exceptions.py
--rw-r--r--  2.0 unx    12966 b- defN 24-May-21 04:38 generated/configmaps/rest.py
--rw-r--r--  2.0 unx      127 b- defN 24-May-21 04:38 generated/configmaps/api/__init__.py
--rw-r--r--  2.0 unx    32156 b- defN 24-May-21 04:38 generated/configmaps/api/configmap_service_api.py
--rw-r--r--  2.0 unx      736 b- defN 24-May-21 04:38 generated/configmaps/models/__init__.py
--rw-r--r--  2.0 unx     2555 b- defN 24-May-21 04:38 generated/configmaps/models/configmap_service_create_body.py
--rw-r--r--  2.0 unx     2555 b- defN 24-May-21 04:38 generated/configmaps/models/configmap_service_update_body.py
--rw-r--r--  2.0 unx     2764 b- defN 24-May-21 04:38 generated/configmaps/models/v1_configmap.py
--rw-r--r--  2.0 unx     2906 b- defN 24-May-21 04:38 generated/configmaps/models/v1_list_response.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-21 04:38 generated/configmaps/test/__init__.py
--rw-r--r--  2.0 unx     1357 b- defN 24-Apr-23 13:37 generated/configmaps/test/test_configmap_service_api.py
--rw-r--r--  2.0 unx     1824 b- defN 24-Apr-23 13:37 generated/configmaps/test/test_configmap_service_create_body.py
--rw-r--r--  2.0 unx     1824 b- defN 24-Apr-24 09:52 generated/configmaps/test/test_configmap_service_update_body.py
--rw-r--r--  2.0 unx     1775 b- defN 24-Apr-23 13:37 generated/configmaps/test/test_v1_configmap.py
--rw-r--r--  2.0 unx     1930 b- defN 24-Apr-23 13:37 generated/configmaps/test/test_v1_list_response.py
--rw-r--r--  2.0 unx     6829 b- defN 24-May-21 04:38 generated/schedulers/__init__.py
--rw-r--r--  2.0 unx    29587 b- defN 24-May-21 04:38 generated/schedulers/api_client.py
--rw-r--r--  2.0 unx      852 b- defN 24-May-21 04:38 generated/schedulers/api_response.py
--rw-r--r--  2.0 unx    14427 b- defN 24-May-21 04:38 generated/schedulers/configuration.py
--rw-r--r--  2.0 unx     5470 b- defN 24-May-21 04:38 generated/schedulers/exceptions.py
--rw-r--r--  2.0 unx    12974 b- defN 24-May-21 04:38 generated/schedulers/rest.py
--rw-r--r--  2.0 unx      115 b- defN 24-May-21 04:38 generated/schedulers/api/__init__.py
--rw-r--r--  2.0 unx    84166 b- defN 24-May-21 04:38 generated/schedulers/api/app_service_api.py
--rw-r--r--  2.0 unx     6164 b- defN 24-May-21 04:38 generated/schedulers/models/__init__.py
--rw-r--r--  2.0 unx     2744 b- defN 24-May-21 04:38 generated/schedulers/models/app_service_create_body.py
--rw-r--r--  2.0 unx     3417 b- defN 24-Apr-17 14:31 generated/schedulers/models/app_service_inference_body.py
--rw-r--r--  2.0 unx     2962 b- defN 24-Apr-09 08:31 generated/schedulers/models/app_service_resources_body.py
--rw-r--r--  2.0 unx     2951 b- defN 24-May-21 04:38 generated/schedulers/models/app_service_setup_auto_scaling_policy_body.py
--rw-r--r--  2.0 unx     2691 b- defN 24-Apr-02 07:19 generated/schedulers/models/app_service_setup_body.py
--rw-r--r--  2.0 unx     2978 b- defN 24-Apr-09 08:31 generated/schedulers/models/app_service_setup_resource_body.py
--rw-r--r--  2.0 unx     2859 b- defN 24-May-21 04:38 generated/schedulers/models/app_service_setup_resources_body.py
--rw-r--r--  2.0 unx     2532 b- defN 24-May-21 04:38 generated/schedulers/models/app_service_setup_secrets_body.py
--rw-r--r--  2.0 unx     3023 b- defN 24-May-21 04:38 generated/schedulers/models/app_service_setup_volumes_body.py
--rw-r--r--  2.0 unx     2523 b- defN 24-Mar-29 07:39 generated/schedulers/models/appsv1_cpu.py
--rw-r--r--  2.0 unx     2884 b- defN 24-Mar-29 07:39 generated/schedulers/models/appsv1_gpu.py
--rw-r--r--  2.0 unx     3074 b- defN 24-May-21 04:38 generated/schedulers/models/appsv1_setup_image.py
--rw-r--r--  2.0 unx     4049 b- defN 24-May-21 04:38 generated/schedulers/models/appsv1_worker.py
--rw-r--r--  2.0 unx     1146 b- defN 24-May-21 04:38 generated/schedulers/models/list_request_queues_response_queue_reason.py
--rw-r--r--  2.0 unx     2933 b- defN 24-May-21 04:38 generated/schedulers/models/list_request_queues_response_request_queue.py
--rw-r--r--  2.0 unx     6639 b- defN 24-May-21 04:38 generated/schedulers/models/protobuf_any.py
--rw-r--r--  2.0 unx      928 b- defN 24-May-21 04:38 generated/schedulers/models/rule_behavior.py
--rw-r--r--  2.0 unx     2872 b- defN 24-Mar-29 07:39 generated/schedulers/models/schedulerv1_cpu.py
--rw-r--r--  2.0 unx     3361 b- defN 24-Mar-29 07:39 generated/schedulers/models/schedulerv1_gpu.py
--rw-r--r--  2.0 unx     3551 b- defN 24-May-21 04:38 generated/schedulers/models/v1_app.py
--rw-r--r--  2.0 unx     2825 b- defN 24-May-21 04:38 generated/schedulers/models/v1_app_service_setup_image_body.py
--rw-r--r--  2.0 unx     1151 b- defN 24-May-21 04:38 generated/schedulers/models/v1_app_status.py
--rw-r--r--  2.0 unx     3371 b- defN 24-May-21 04:38 generated/schedulers/models/v1_autoscaling_policy.py
--rw-r--r--  2.0 unx     3073 b- defN 24-May-21 04:38 generated/schedulers/models/v1_bandwidth.py
--rw-r--r--  2.0 unx     2483 b- defN 24-May-21 04:38 generated/schedulers/models/v1_bandwidth_size.py
--rw-r--r--  2.0 unx     3086 b- defN 24-May-21 04:38 generated/schedulers/models/v1_basic_auth.py
--rw-r--r--  2.0 unx     3086 b- defN 24-Apr-09 08:31 generated/schedulers/models/v1_build_in_policy.py
--rw-r--r--  2.0 unx     2965 b- defN 24-May-21 04:38 generated/schedulers/models/v1_built_in_policy.py
--rw-r--r--  2.0 unx     2836 b- defN 24-May-21 04:38 generated/schedulers/models/v1_cpu.py
--rw-r--r--  2.0 unx     2984 b- defN 24-May-21 04:38 generated/schedulers/models/v1_create_volume_request.py
--rw-r--r--  2.0 unx     2876 b- defN 24-May-21 04:38 generated/schedulers/models/v1_create_volume_response.py
--rw-r--r--  2.0 unx     2849 b- defN 24-May-21 04:38 generated/schedulers/models/v1_custom_policy.py
--rw-r--r--  2.0 unx     2987 b- defN 24-May-21 04:38 generated/schedulers/models/v1_delete_volume_request.py
--rw-r--r--  2.0 unx     2612 b- defN 24-Mar-29 08:50 generated/schedulers/models/v1_delete_volume_response.py
--rw-r--r--  2.0 unx     4796 b- defN 24-May-21 04:38 generated/schedulers/models/v1_device_resource.py
--rw-r--r--  2.0 unx     2449 b- defN 24-May-21 04:38 generated/schedulers/models/v1_empty_response.py
--rw-r--r--  2.0 unx     2753 b- defN 24-May-21 04:38 generated/schedulers/models/v1_error_response.py
--rw-r--r--  2.0 unx     3247 b- defN 24-May-21 04:38 generated/schedulers/models/v1_filesystem.py
--rw-r--r--  2.0 unx     2546 b- defN 24-May-21 04:38 generated/schedulers/models/v1_get_image_request.py
--rw-r--r--  2.0 unx     2847 b- defN 24-May-21 04:38 generated/schedulers/models/v1_get_image_response.py
--rw-r--r--  2.0 unx     2624 b- defN 24-May-21 04:38 generated/schedulers/models/v1_get_volume_request.py
--rw-r--r--  2.0 unx     2864 b- defN 24-May-21 04:38 generated/schedulers/models/v1_get_volume_response.py
--rw-r--r--  2.0 unx     2518 b- defN 24-May-21 04:38 generated/schedulers/models/v1_get_worker_request.py
--rw-r--r--  2.0 unx     2900 b- defN 24-May-21 04:38 generated/schedulers/models/v1_get_worker_response.py
--rw-r--r--  2.0 unx     3325 b- defN 24-May-21 04:38 generated/schedulers/models/v1_gpu.py
--rw-r--r--  2.0 unx     2499 b- defN 24-May-21 04:38 generated/schedulers/models/v1_gpu_opts.py
--rw-r--r--  2.0 unx     2508 b- defN 24-May-21 04:38 generated/schedulers/models/v1_header_entry.py
--rw-r--r--  2.0 unx     3320 b- defN 24-May-21 04:38 generated/schedulers/models/v1_image.py
--rw-r--r--  2.0 unx     4574 b- defN 24-May-21 04:38 generated/schedulers/models/v1_image_request.py
--rw-r--r--  2.0 unx      917 b- defN 24-May-21 04:38 generated/schedulers/models/v1_image_status.py
--rw-r--r--  2.0 unx     3436 b- defN 24-Apr-17 14:31 generated/schedulers/models/v1_inference_response.py
--rw-r--r--  2.0 unx     2924 b- defN 24-May-21 04:38 generated/schedulers/models/v1_list_image_request.py
--rw-r--r--  2.0 unx     3033 b- defN 24-May-21 04:38 generated/schedulers/models/v1_list_image_response.py
--rw-r--r--  2.0 unx     3038 b- defN 24-May-21 04:38 generated/schedulers/models/v1_list_request_queues_response.py
--rw-r--r--  2.0 unx     2836 b- defN 24-May-21 04:38 generated/schedulers/models/v1_list_response.py
--rw-r--r--  2.0 unx     2863 b- defN 24-May-21 04:38 generated/schedulers/models/v1_list_volume_request.py
--rw-r--r--  2.0 unx     3050 b- defN 24-May-21 04:38 generated/schedulers/models/v1_list_volume_response.py
--rw-r--r--  2.0 unx     2731 b- defN 24-May-21 04:38 generated/schedulers/models/v1_list_worker_request.py
--rw-r--r--  2.0 unx     3086 b- defN 24-May-21 04:38 generated/schedulers/models/v1_list_worker_response.py
--rw-r--r--  2.0 unx     3790 b- defN 24-May-21 04:38 generated/schedulers/models/v1_list_workers_response.py
--rw-r--r--  2.0 unx     3274 b- defN 24-May-21 04:38 generated/schedulers/models/v1_pull_image_request.py
--rw-r--r--  2.0 unx     2851 b- defN 24-May-21 04:38 generated/schedulers/models/v1_pull_image_response.py
--rw-r--r--  2.0 unx     2875 b- defN 24-May-21 04:38 generated/schedulers/models/v1_remove_image_request.py
--rw-r--r--  2.0 unx     3828 b- defN 24-May-21 04:38 generated/schedulers/models/v1_resource_claim.py
--rw-r--r--  2.0 unx     3190 b- defN 24-May-21 04:38 generated/schedulers/models/v1_resources.py
--rw-r--r--  2.0 unx     2616 b- defN 24-May-21 04:38 generated/schedulers/models/v1_restart_worker_request.py
--rw-r--r--  2.0 unx     4381 b- defN 24-May-21 04:38 generated/schedulers/models/v1_route_request.py
--rw-r--r--  2.0 unx     3056 b- defN 24-May-21 04:38 generated/schedulers/models/v1_rule.py
--rw-r--r--  2.0 unx     4243 b- defN 24-May-21 04:38 generated/schedulers/models/v1_run_worker_request.py
--rw-r--r--  2.0 unx     2924 b- defN 24-May-21 04:38 generated/schedulers/models/v1_run_worker_response.py
--rw-r--r--  2.0 unx     4848 b- defN 24-Apr-02 07:19 generated/schedulers/models/v1_setting.py
--rw-r--r--  2.0 unx     3058 b- defN 24-Apr-02 07:19 generated/schedulers/models/v1_setup_image.py
--rw-r--r--  2.0 unx     2518 b- defN 24-Apr-02 07:19 generated/schedulers/models/v1_setup_secrets.py
--rw-r--r--  2.0 unx     2764 b- defN 24-May-21 04:38 generated/schedulers/models/v1_setup_volume.py
--rw-r--r--  2.0 unx     2925 b- defN 24-Apr-02 07:19 generated/schedulers/models/v1_setup_volumes.py
--rw-r--r--  2.0 unx     2890 b- defN 24-Apr-02 07:19 generated/schedulers/models/v1_setup_volumes_volume.py
--rw-r--r--  2.0 unx     2749 b- defN 24-May-21 04:38 generated/schedulers/models/v1_stop_worker_request.py
--rw-r--r--  2.0 unx     2475 b- defN 24-May-21 04:38 generated/schedulers/models/v1_storage_size.py
--rw-r--r--  2.0 unx     2966 b- defN 24-May-21 04:38 generated/schedulers/models/v1_sync_volume_request.py
--rw-r--r--  2.0 unx     2604 b- defN 24-Mar-29 08:50 generated/schedulers/models/v1_sync_volume_response.py
--rw-r--r--  2.0 unx     2504 b- defN 24-May-21 04:38 generated/schedulers/models/v1_value_from_secret.py
--rw-r--r--  2.0 unx     3517 b- defN 24-May-21 04:38 generated/schedulers/models/v1_volume.py
--rw-r--r--  2.0 unx     2576 b- defN 24-May-21 04:38 generated/schedulers/models/v1_volume_mount.py
--rw-r--r--  2.0 unx     5229 b- defN 24-May-21 04:38 generated/schedulers/models/v1_volume_request.py
--rw-r--r--  2.0 unx      970 b- defN 24-May-21 04:38 generated/schedulers/models/v1_volume_status.py
--rw-r--r--  2.0 unx     3049 b- defN 24-Apr-17 14:31 generated/schedulers/models/v1_worker.py
--rw-r--r--  2.0 unx     5201 b- defN 24-May-21 04:38 generated/schedulers/models/v1_worker_request.py
--rw-r--r--  2.0 unx     1052 b- defN 24-Apr-23 13:37 generated/schedulers/models/v1_worker_status.py
--rw-r--r--  2.0 unx     1210 b- defN 24-May-21 04:38 generated/schedulers/models/v1_worker_worker_status.py
--rw-r--r--  2.0 unx     3106 b- defN 24-May-21 04:38 generated/schedulers/models/v1workersv1_worker.py
--rw-r--r--  2.0 unx     3439 b- defN 24-Apr-02 07:19 generated/schedulers/models/volumesv1_volume.py
--rw-r--r--  2.0 unx     1192 b- defN 24-May-21 04:38 generated/schedulers/models/worker_worker_detail_status.py
--rw-r--r--  2.0 unx     1073 b- defN 24-May-21 04:38 generated/schedulers/models/workersv1_worker_status.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-21 04:38 generated/schedulers/test/__init__.py
--rw-r--r--  2.0 unx     1668 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_app_service_api.py
--rw-r--r--  2.0 unx     1602 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_app_service_create_body.py
--rw-r--r--  2.0 unx     1763 b- defN 24-Apr-17 14:12 generated/schedulers/test/test_app_service_inference_body.py
--rw-r--r--  2.0 unx     2887 b- defN 24-Apr-09 08:31 generated/schedulers/test/test_app_service_resources_body.py
--rw-r--r--  2.0 unx     3598 b- defN 24-Apr-09 08:31 generated/schedulers/test/test_app_service_setup_auto_scaling_policy_body.py
--rw-r--r--  2.0 unx     7883 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_app_service_setup_body.py
--rw-r--r--  2.0 unx     2936 b- defN 24-Apr-09 08:31 generated/schedulers/test/test_app_service_setup_resource_body.py
--rw-r--r--  2.0 unx     2948 b- defN 24-Apr-09 08:31 generated/schedulers/test/test_app_service_setup_resources_body.py
--rw-r--r--  2.0 unx     1708 b- defN 24-Apr-09 08:31 generated/schedulers/test/test_app_service_setup_secrets_body.py
--rw-r--r--  2.0 unx     2182 b- defN 24-Apr-09 08:31 generated/schedulers/test/test_app_service_setup_volumes_body.py
--rw-r--r--  2.0 unx     1450 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_appsv1_cpu.py
--rw-r--r--  2.0 unx     1562 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_appsv1_gpu.py
--rw-r--r--  2.0 unx     1981 b- defN 24-Apr-09 08:31 generated/schedulers/test/test_appsv1_setup_image.py
--rw-r--r--  2.0 unx     1723 b- defN 24-Apr-22 10:29 generated/schedulers/test/test_appsv1_worker.py
--rw-r--r--  2.0 unx      950 b- defN 24-Apr-25 08:31 generated/schedulers/test/test_list_request_queues_response_queue_reason.py
--rw-r--r--  2.0 unx     1912 b- defN 24-Apr-25 08:31 generated/schedulers/test/test_list_request_queues_response_request_queue.py
--rw-r--r--  2.0 unx     1438 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_protobuf_any.py
--rw-r--r--  2.0 unx      778 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_rule_behavior.py
--rw-r--r--  2.0 unx     1598 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_schedulerv1_cpu.py
--rw-r--r--  2.0 unx     1755 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_schedulerv1_gpu.py
--rw-r--r--  2.0 unx     1750 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_app.py
--rw-r--r--  2.0 unx     2857 b- defN 24-Apr-09 08:31 generated/schedulers/test/test_v1_app_service_setup_image_body.py
--rw-r--r--  2.0 unx      772 b- defN 24-Apr-02 07:19 generated/schedulers/test/test_v1_app_status.py
--rw-r--r--  2.0 unx     2194 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_autoscaling_policy.py
--rw-r--r--  2.0 unx     1723 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_bandwidth.py
--rw-r--r--  2.0 unx     1541 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_bandwidth_size.py
--rw-r--r--  2.0 unx     1474 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_basic_auth.py
--rw-r--r--  2.0 unx     1597 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_build_in_policy.py
--rw-r--r--  2.0 unx     1563 b- defN 24-Apr-09 08:31 generated/schedulers/test/test_v1_built_in_policy.py
--rw-r--r--  2.0 unx     1490 b- defN 24-Mar-29 08:50 generated/schedulers/test/test_v1_cpu.py
--rw-r--r--  2.0 unx     1569 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_create_volume_request.py
--rw-r--r--  2.0 unx     1831 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_create_volume_response.py
--rw-r--r--  2.0 unx     1820 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_custom_policy.py
--rw-r--r--  2.0 unx     1560 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_delete_volume_request.py
--rw-r--r--  2.0 unx     1606 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_delete_volume_response.py
--rw-r--r--  2.0 unx     4637 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_device_resource.py
--rw-r--r--  2.0 unx     1526 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_empty_response.py
--rw-r--r--  2.0 unx     1612 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_error_response.py
--rw-r--r--  2.0 unx     1755 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_filesystem.py
--rw-r--r--  2.0 unx     1617 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_get_image_request.py
--rw-r--r--  2.0 unx     2140 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_get_image_response.py
--rw-r--r--  2.0 unx     1524 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_get_volume_request.py
--rw-r--r--  2.0 unx     1735 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_get_volume_response.py
--rw-r--r--  2.0 unx     1613 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_get_worker_request.py
--rw-r--r--  2.0 unx     1938 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_get_worker_response.py
--rw-r--r--  2.0 unx     1647 b- defN 24-Mar-29 08:50 generated/schedulers/test/test_v1_gpu.py
--rw-r--r--  2.0 unx     1445 b- defN 24-Apr-23 15:39 generated/schedulers/test/test_v1_gpu_opts.py
--rw-r--r--  2.0 unx     1535 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_header_entry.py
--rw-r--r--  2.0 unx     1997 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_image.py
--rw-r--r--  2.0 unx     2660 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_image_request.py
--rw-r--r--  2.0 unx      786 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_image_status.py
--rw-r--r--  2.0 unx     1638 b- defN 24-Apr-17 14:12 generated/schedulers/test/test_v1_inference_response.py
--rw-r--r--  2.0 unx     1732 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_list_image_request.py
--rw-r--r--  2.0 unx     2249 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_list_image_response.py
--rw-r--r--  2.0 unx     1999 b- defN 24-Apr-25 08:31 generated/schedulers/test/test_v1_list_request_queues_response.py
--rw-r--r--  2.0 unx     2049 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_list_response.py
--rw-r--r--  2.0 unx     1545 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_list_volume_request.py
--rw-r--r--  2.0 unx     1808 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_list_volume_response.py
--rw-r--r--  2.0 unx     1634 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_list_worker_request.py
--rw-r--r--  2.0 unx     2019 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_list_worker_response.py
--rw-r--r--  2.0 unx     2006 b- defN 24-Apr-22 10:29 generated/schedulers/test/test_v1_list_workers_response.py
--rw-r--r--  2.0 unx     1864 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_pull_image_request.py
--rw-r--r--  2.0 unx     2152 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_pull_image_response.py
--rw-r--r--  2.0 unx     1801 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_remove_image_request.py
--rw-r--r--  2.0 unx     2534 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_resource_claim.py
--rw-r--r--  2.0 unx     1590 b- defN 24-Apr-17 14:12 generated/schedulers/test/test_v1_resources.py
--rw-r--r--  2.0 unx     1721 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_restart_worker_request.py
--rw-r--r--  2.0 unx     2189 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_route_request.py
--rw-r--r--  2.0 unx     1550 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_rule.py
--rw-r--r--  2.0 unx     2165 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_run_worker_request.py
--rw-r--r--  2.0 unx     1905 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_run_worker_response.py
--rw-r--r--  2.0 unx     4054 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_setting.py
--rw-r--r--  2.0 unx     1771 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_setup_image.py
--rw-r--r--  2.0 unx     1527 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_setup_secrets.py
--rw-r--r--  2.0 unx     1569 b- defN 24-Apr-09 08:31 generated/schedulers/test/test_v1_setup_volume.py
--rw-r--r--  2.0 unx     1715 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_setup_volumes.py
--rw-r--r--  2.0 unx     1709 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_setup_volumes_volume.py
--rw-r--r--  2.0 unx     1685 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_stop_worker_request.py
--rw-r--r--  2.0 unx     1517 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_storage_size.py
--rw-r--r--  2.0 unx     1578 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_sync_volume_request.py
--rw-r--r--  2.0 unx     1582 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_sync_volume_response.py
--rw-r--r--  2.0 unx     1538 b- defN 24-Apr-02 03:45 generated/schedulers/test/test_v1_value_from_secret.py
--rw-r--r--  2.0 unx     1838 b- defN 24-Apr-09 08:31 generated/schedulers/test/test_v1_volume.py
--rw-r--r--  2.0 unx     1608 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_volume_mount.py
--rw-r--r--  2.0 unx     2254 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_volume_request.py
--rw-r--r--  2.0 unx      793 b- defN 24-Apr-02 03:45 generated/schedulers/test/test_v1_volume_status.py
--rw-r--r--  2.0 unx     1891 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_worker.py
--rw-r--r--  2.0 unx     2991 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_worker_request.py
--rw-r--r--  2.0 unx      793 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_worker_status.py
--rw-r--r--  2.0 unx      836 b- defN 24-Apr-23 15:39 generated/schedulers/test/test_v1_worker_worker_status.py
--rw-r--r--  2.0 unx     1999 b- defN 24-Apr-22 10:29 generated/schedulers/test/test_v1workersv1_worker.py
--rw-r--r--  2.0 unx     1576 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_volumesv1_volume.py
--rw-r--r--  2.0 unx      864 b- defN 24-Apr-25 08:59 generated/schedulers/test/test_worker_worker_detail_status.py
--rw-r--r--  2.0 unx      842 b- defN 24-Apr-23 15:39 generated/schedulers/test/test_workersv1_worker_status.py
--rw-r--r--  2.0 unx     1344 b- defN 24-May-21 04:38 generated/secrets/__init__.py
--rw-r--r--  2.0 unx    29558 b- defN 24-May-21 04:38 generated/secrets/api_client.py
--rw-r--r--  2.0 unx      852 b- defN 24-May-21 04:38 generated/secrets/api_response.py
--rw-r--r--  2.0 unx    14413 b- defN 24-May-21 04:38 generated/secrets/configuration.py
--rw-r--r--  2.0 unx     5459 b- defN 24-May-21 04:38 generated/secrets/exceptions.py
--rw-r--r--  2.0 unx    12960 b- defN 24-May-21 04:38 generated/secrets/rest.py
--rw-r--r--  2.0 unx      118 b- defN 24-May-21 04:38 generated/secrets/api/__init__.py
--rw-r--r--  2.0 unx    31721 b- defN 24-May-21 04:38 generated/secrets/api/secret_service_api.py
--rw-r--r--  2.0 unx      703 b- defN 24-May-21 04:38 generated/secrets/models/__init__.py
--rw-r--r--  2.0 unx     2540 b- defN 24-May-21 04:38 generated/secrets/models/secret_service_create_body.py
--rw-r--r--  2.0 unx     2540 b- defN 24-May-21 04:38 generated/secrets/models/secret_service_update_body.py
--rw-r--r--  2.0 unx     2861 b- defN 24-May-21 04:38 generated/secrets/models/v1_list_response.py
--rw-r--r--  2.0 unx     2749 b- defN 24-May-21 04:38 generated/secrets/models/v1_secret.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-21 04:38 generated/secrets/test/__init__.py
--rw-r--r--  2.0 unx     1297 b- defN 24-Mar-28 14:39 generated/secrets/test/test_secret_service_api.py
--rw-r--r--  2.0 unx     1680 b- defN 24-Mar-28 14:39 generated/secrets/test/test_secret_service_create_body.py
--rw-r--r--  2.0 unx     1782 b- defN 24-Apr-24 09:52 generated/secrets/test/test_secret_service_update_body.py
--rw-r--r--  2.0 unx     1845 b- defN 24-Mar-28 14:39 generated/secrets/test/test_v1_list_response.py
--rw-r--r--  2.0 unx     1603 b- defN 24-Mar-28 14:39 generated/secrets/test/test_v1_secret.py
--rw-r--r--  2.0 unx     2997 b- defN 24-May-21 04:38 generated/volumes/__init__.py
--rw-r--r--  2.0 unx    29558 b- defN 24-May-21 04:38 generated/volumes/api_client.py
--rw-r--r--  2.0 unx      852 b- defN 24-May-21 04:38 generated/volumes/api_response.py
--rw-r--r--  2.0 unx    14413 b- defN 24-May-21 04:38 generated/volumes/configuration.py
--rw-r--r--  2.0 unx     5459 b- defN 24-May-21 04:38 generated/volumes/exceptions.py
--rw-r--r--  2.0 unx    12960 b- defN 24-May-21 04:38 generated/volumes/rest.py
--rw-r--r--  2.0 unx      118 b- defN 24-May-21 04:38 generated/volumes/api/__init__.py
--rw-r--r--  2.0 unx   143619 b- defN 24-May-21 04:38 generated/volumes/api/volume_service_api.py
--rw-r--r--  2.0 unx     2356 b- defN 24-May-21 04:38 generated/volumes/models/__init__.py
--rw-r--r--  2.0 unx     2991 b- defN 24-May-21 04:38 generated/volumes/models/file_information.py
--rw-r--r--  2.0 unx     2986 b- defN 24-May-21 04:38 generated/volumes/models/v1_file.py
--rw-r--r--  2.0 unx     2415 b- defN 24-May-21 04:38 generated/volumes/models/v1_header_value.py
--rw-r--r--  2.0 unx     2728 b- defN 24-May-21 04:38 generated/volumes/models/v1_initialize_multipart_upload_response.py
--rw-r--r--  2.0 unx     2855 b- defN 24-May-21 04:38 generated/volumes/models/v1_list_files_response.py
--rw-r--r--  2.0 unx     2855 b- defN 24-May-21 04:38 generated/volumes/models/v1_list_parts_response.py
--rw-r--r--  2.0 unx     2861 b- defN 24-May-21 04:38 generated/volumes/models/v1_list_response.py
--rw-r--r--  2.0 unx     2592 b- defN 24-May-21 04:38 generated/volumes/models/v1_part.py
--rw-r--r--  2.0 unx     2897 b- defN 24-May-21 04:38 generated/volumes/models/v1_revision.py
--rw-r--r--  2.0 unx     3193 b- defN 24-May-21 04:38 generated/volumes/models/v1_sign_response.py
--rw-r--r--  2.0 unx     2910 b- defN 24-May-21 04:38 generated/volumes/models/v1_sign_upload_response.py
--rw-r--r--  2.0 unx      901 b- defN 24-May-21 04:38 generated/volumes/models/v1_upload_action.py
--rw-r--r--  2.0 unx     3421 b- defN 24-May-21 04:38 generated/volumes/models/v1_volume.py
--rw-r--r--  2.0 unx      951 b- defN 24-May-21 04:38 generated/volumes/models/v1_volume_status.py
--rw-r--r--  2.0 unx     2517 b- defN 24-May-21 04:38 generated/volumes/models/volume_service_change_revision_body.py
--rw-r--r--  2.0 unx     2809 b- defN 24-May-21 04:38 generated/volumes/models/volume_service_commit_file_body.py
--rw-r--r--  2.0 unx     3055 b- defN 24-May-21 04:38 generated/volumes/models/volume_service_commit_file_body_file.py
--rw-r--r--  2.0 unx     2876 b- defN 24-May-21 04:38 generated/volumes/models/volume_service_commit_revision_body.py
--rw-r--r--  2.0 unx     3092 b- defN 24-May-21 04:38 generated/volumes/models/volume_service_complete_multipart_upload_body.py
--rw-r--r--  2.0 unx     2464 b- defN 24-May-21 04:38 generated/volumes/models/volume_service_create_body.py
--rw-r--r--  2.0 unx     2801 b- defN 24-May-21 04:38 generated/volumes/models/volume_service_initialize_multipart_upload_body.py
--rw-r--r--  2.0 unx     2527 b- defN 24-May-21 04:38 generated/volumes/models/volume_service_sign_multipart_upload_body.py
--rw-r--r--  2.0 unx     2741 b- defN 24-May-21 04:38 generated/volumes/models/volume_service_sign_upload_body.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-21 04:38 generated/volumes/test/__init__.py
--rw-r--r--  2.0 unx     1716 b- defN 24-Mar-28 14:39 generated/volumes/test/test_file_information.py
--rw-r--r--  2.0 unx     1718 b- defN 24-Mar-28 14:39 generated/volumes/test/test_v1_file.py
--rw-r--r--  2.0 unx     1494 b- defN 24-Mar-28 14:39 generated/volumes/test/test_v1_header_value.py
--rw-r--r--  2.0 unx     1755 b- defN 24-Mar-28 14:39 generated/volumes/test/test_v1_initialize_multipart_upload_response.py
--rw-r--r--  2.0 unx     1949 b- defN 24-Mar-28 14:39 generated/volumes/test/test_v1_list_files_response.py
--rw-r--r--  2.0 unx     1721 b- defN 24-Mar-28 14:39 generated/volumes/test/test_v1_list_parts_response.py
--rw-r--r--  2.0 unx     2073 b- defN 24-Mar-28 14:39 generated/volumes/test/test_v1_list_response.py
--rw-r--r--  2.0 unx     1486 b- defN 24-Mar-28 14:39 generated/volumes/test/test_v1_part.py
--rw-r--r--  2.0 unx     1609 b- defN 24-Mar-28 14:39 generated/volumes/test/test_v1_revision.py
--rw-r--r--  2.0 unx     1722 b- defN 24-Mar-28 14:39 generated/volumes/test/test_v1_sign_response.py
--rw-r--r--  2.0 unx     1952 b- defN 24-Mar-28 14:39 generated/volumes/test/test_v1_sign_upload_response.py
--rw-r--r--  2.0 unx      779 b- defN 24-Mar-28 14:39 generated/volumes/test/test_v1_upload_action.py
--rw-r--r--  2.0 unx     1795 b- defN 24-Mar-28 14:39 generated/volumes/test/test_v1_volume.py
--rw-r--r--  2.0 unx      779 b- defN 24-May-09 04:00 generated/volumes/test/test_v1_volume_status.py
--rw-r--r--  2.0 unx     3607 b- defN 24-Mar-28 14:39 generated/volumes/test/test_volume_service_api.py
--rw-r--r--  2.0 unx     1712 b- defN 24-Mar-28 14:39 generated/volumes/test/test_volume_service_change_revision_body.py
--rw-r--r--  2.0 unx     2004 b- defN 24-Mar-28 14:39 generated/volumes/test/test_volume_service_commit_file_body.py
--rw-r--r--  2.0 unx     1912 b- defN 24-Mar-28 14:39 generated/volumes/test/test_volume_service_commit_file_body_file.py
--rw-r--r--  2.0 unx     2548 b- defN 24-Mar-28 14:39 generated/volumes/test/test_volume_service_commit_revision_body.py
--rw-r--r--  2.0 unx     2233 b- defN 24-Mar-28 14:39 generated/volumes/test/test_volume_service_complete_multipart_upload_body.py
--rw-r--r--  2.0 unx     1624 b- defN 24-Mar-28 14:39 generated/volumes/test/test_volume_service_create_body.py
--rw-r--r--  2.0 unx     2149 b- defN 24-Mar-28 14:39 generated/volumes/test/test_volume_service_initialize_multipart_upload_body.py
--rw-r--r--  2.0 unx     1769 b- defN 24-Mar-28 14:39 generated/volumes/test/test_volume_service_sign_multipart_upload_body.py
--rw-r--r--  2.0 unx     1968 b- defN 24-Mar-28 14:39 generated/volumes/test/test_volume_service_sign_upload_body.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-24 09:12 everai-0.1.62.dist-info/LICENSE
--rw-r--r--  2.0 unx     1985 b- defN 24-May-24 09:12 everai-0.1.62.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-24 09:12 everai-0.1.62.dist-info/WHEEL
--rw-r--r--  2.0 unx       98 b- defN 24-May-24 09:12 everai-0.1.62.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       17 b- defN 24-May-24 09:12 everai-0.1.62.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    42349 b- defN 24-May-24 09:12 everai-0.1.62.dist-info/RECORD
-424 files, 1385102 bytes uncompressed, 371697 bytes compressed:  73.2%
+-rw-r--r--  2.0 unx     3315 b- defN 24-Jun-03 12:24 everai/worker/worker.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Jun-03 12:17 generated/__init__.py
+-rw-r--r--  2.0 unx     4955 b- defN 24-Jun-03 12:17 generated/apps/__init__.py
+-rw-r--r--  2.0 unx    29536 b- defN 24-Jun-03 12:17 generated/apps/api_client.py
+-rw-r--r--  2.0 unx      852 b- defN 24-Jun-03 12:17 generated/apps/api_response.py
+-rw-r--r--  2.0 unx    14406 b- defN 24-Jun-03 12:17 generated/apps/configuration.py
+-rw-r--r--  2.0 unx     5455 b- defN 24-Jun-03 12:17 generated/apps/exceptions.py
+-rw-r--r--  2.0 unx    12953 b- defN 24-Jun-03 12:17 generated/apps/rest.py
+-rw-r--r--  2.0 unx      109 b- defN 24-Jun-03 12:17 generated/apps/api/__init__.py
+-rw-r--r--  2.0 unx   108382 b- defN 24-Jun-03 12:17 generated/apps/api/app_service_api.py
+-rw-r--r--  2.0 unx     4350 b- defN 24-Jun-03 12:17 generated/apps/models/__init__.py
+-rw-r--r--  2.0 unx     1103 b- defN 24-Jun-03 12:17 generated/apps/models/app_route_auth_status.py
+-rw-r--r--  2.0 unx     2594 b- defN 24-Jun-03 12:17 generated/apps/models/app_runtimev1_request_queue.py
+-rw-r--r--  2.0 unx     2729 b- defN 24-Jun-03 12:17 generated/apps/models/app_service_create_body.py
+-rw-r--r--  2.0 unx     2470 b- defN 24-Jun-03 12:17 generated/apps/models/app_service_protect_app_body.py
+-rw-r--r--  2.0 unx     2930 b- defN 24-Jun-03 12:17 generated/apps/models/app_service_setup_auto_scaling_policy_body.py
+-rw-r--r--  2.0 unx     2838 b- defN 24-Jun-03 12:17 generated/apps/models/app_service_setup_resources_body.py
+-rw-r--r--  2.0 unx     2517 b- defN 24-Jun-03 12:17 generated/apps/models/app_service_setup_secrets_body.py
+-rw-r--r--  2.0 unx     3002 b- defN 24-Jun-03 12:17 generated/apps/models/app_service_setup_volumes_body.py
+-rw-r--r--  2.0 unx     3053 b- defN 24-Jun-03 12:17 generated/apps/models/appsv1_setup_image.py
+-rw-r--r--  2.0 unx     1131 b- defN 24-Jun-03 12:17 generated/apps/models/list_request_queues_response_queue_reason.py
+-rw-r--r--  2.0 unx     6624 b- defN 24-Jun-03 12:17 generated/apps/models/protobuf_any.py
+-rw-r--r--  2.0 unx      913 b- defN 24-Jun-03 12:17 generated/apps/models/rule_behavior.py
+-rw-r--r--  2.0 unx     1083 b- defN 24-Jun-03 12:17 generated/apps/models/scale_record_autoscaling_action.py
+-rw-r--r--  2.0 unx     4890 b- defN 24-Jun-03 12:17 generated/apps/models/v1_app.py
+-rw-r--r--  2.0 unx     5292 b- defN 24-Jun-03 12:17 generated/apps/models/v1_app_revision.py
+-rw-r--r--  2.0 unx     4353 b- defN 24-Jun-03 12:17 generated/apps/models/v1_app_runtime.py
+-rw-r--r--  2.0 unx     2804 b- defN 24-Jun-03 12:17 generated/apps/models/v1_app_service_setup_image_body.py
+-rw-r--r--  2.0 unx     1220 b- defN 24-Jun-03 12:17 generated/apps/models/v1_app_status.py
+-rw-r--r--  2.0 unx     3344 b- defN 24-Jun-03 12:17 generated/apps/models/v1_autoscaling_policy.py
+-rw-r--r--  2.0 unx     3065 b- defN 24-Jun-03 12:17 generated/apps/models/v1_basic_auth.py
+-rw-r--r--  2.0 unx     2950 b- defN 24-Jun-03 12:17 generated/apps/models/v1_built_in_policy.py
+-rw-r--r--  2.0 unx     2925 b- defN 24-Jun-03 12:17 generated/apps/models/v1_check_and_lock_worker_response.py
+-rw-r--r--  2.0 unx     2828 b- defN 24-Jun-03 12:17 generated/apps/models/v1_custom_policy.py
+-rw-r--r--  2.0 unx     2775 b- defN 24-Jun-03 12:17 generated/apps/models/v1_get_app_runtime_snapshot_response.py
+-rw-r--r--  2.0 unx     2447 b- defN 24-Jun-03 12:17 generated/apps/models/v1_get_route_path_response.py
+-rw-r--r--  2.0 unx     2495 b- defN 24-Jun-03 12:17 generated/apps/models/v1_get_safety_remove_workers_response.py
+-rw-r--r--  2.0 unx     2843 b- defN 24-Jun-03 12:17 generated/apps/models/v1_list_all_apps_response.py
+-rw-r--r--  2.0 unx     2887 b- defN 24-Jun-03 12:17 generated/apps/models/v1_list_all_apps_with_workers_response.py
+-rw-r--r--  2.0 unx     2894 b- defN 24-Jun-03 12:17 generated/apps/models/v1_list_all_workers_response.py
+-rw-r--r--  2.0 unx     2871 b- defN 24-Jun-03 12:17 generated/apps/models/v1_list_app_by_unique_ids_response.py
+-rw-r--r--  2.0 unx     2855 b- defN 24-Jun-03 12:17 generated/apps/models/v1_list_apps_by_user_response.py
+-rw-r--r--  2.0 unx     3026 b- defN 24-Jun-03 12:17 generated/apps/models/v1_list_request_queues_response.py
+-rw-r--r--  2.0 unx     2920 b- defN 24-Jun-03 12:17 generated/apps/models/v1_list_request_queues_response_request_queue.py
+-rw-r--r--  2.0 unx     2815 b- defN 24-Jun-03 12:17 generated/apps/models/v1_list_response.py
+-rw-r--r--  2.0 unx     2906 b- defN 24-Jun-03 12:17 generated/apps/models/v1_list_worker_details_response.py
+-rw-r--r--  2.0 unx     2930 b- defN 24-Jun-03 12:17 generated/apps/models/v1_list_workers_by_app_and_user_response.py
+-rw-r--r--  2.0 unx     2950 b- defN 24-Jun-03 12:17 generated/apps/models/v1_list_workers_by_device_and_status_response.py
+-rw-r--r--  2.0 unx     2914 b- defN 24-Jun-03 12:17 generated/apps/models/v1_list_workers_by_status_response.py
+-rw-r--r--  2.0 unx     3753 b- defN 24-Jun-03 12:17 generated/apps/models/v1_list_workers_response.py
+-rw-r--r--  2.0 unx     3813 b- defN 24-Jun-03 12:17 generated/apps/models/v1_resource_claim.py
+-rw-r--r--  2.0 unx     3029 b- defN 24-Jun-03 12:17 generated/apps/models/v1_rule.py
+-rw-r--r--  2.0 unx     2611 b- defN 24-Jun-03 12:17 generated/apps/models/v1_scale_record.py
+-rw-r--r--  2.0 unx     2925 b- defN 24-Jun-03 12:17 generated/apps/models/v1_setup_volume.py
+-rw-r--r--  2.0 unx     2489 b- defN 24-Jun-03 12:17 generated/apps/models/v1_value_from_secret.py
+-rw-r--r--  2.0 unx     5383 b- defN 24-Jun-03 12:17 generated/apps/models/v1_worker.py
+-rw-r--r--  2.0 unx     4115 b- defN 24-Jun-03 12:17 generated/apps/models/v1_worker_runtime.py
+-rw-r--r--  2.0 unx     1177 b- defN 24-Jun-03 12:17 generated/apps/models/worker_worker_detail_status.py
+-rw-r--r--  2.0 unx     1189 b- defN 24-Jun-03 12:17 generated/apps/models/worker_worker_status.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Jun-03 12:17 generated/apps/test/__init__.py
+-rw-r--r--  2.0 unx      801 b- defN 24-Jun-03 12:17 generated/apps/test/test_app_route_auth_status.py
+-rw-r--r--  2.0 unx     1604 b- defN 24-Jun-03 12:17 generated/apps/test/test_app_runtimev1_request_queue.py
+-rw-r--r--  2.0 unx     3183 b- defN 24-Jun-03 12:17 generated/apps/test/test_app_service_api.py
+-rw-r--r--  2.0 unx     1614 b- defN 24-Jun-03 12:17 generated/apps/test/test_app_service_create_body.py
+-rw-r--r--  2.0 unx     1615 b- defN 24-Jun-03 12:17 generated/apps/test/test_app_service_protect_app_body.py
+-rw-r--r--  2.0 unx     3573 b- defN 24-Jun-03 12:17 generated/apps/test/test_app_service_setup_auto_scaling_policy_body.py
+-rw-r--r--  2.0 unx     2959 b- defN 24-Jun-03 12:17 generated/apps/test/test_app_service_setup_resources_body.py
+-rw-r--r--  2.0 unx     1731 b- defN 24-Jun-03 12:17 generated/apps/test/test_app_service_setup_secrets_body.py
+-rw-r--r--  2.0 unx     2193 b- defN 24-Jun-03 12:17 generated/apps/test/test_app_service_setup_volumes_body.py
+-rw-r--r--  2.0 unx     1986 b- defN 24-Jun-03 12:17 generated/apps/test/test_appsv1_setup_image.py
+-rw-r--r--  2.0 unx      929 b- defN 24-Jun-03 12:17 generated/apps/test/test_list_request_queues_response_queue_reason.py
+-rw-r--r--  2.0 unx     1417 b- defN 24-Jun-03 12:17 generated/apps/test/test_protobuf_any.py
+-rw-r--r--  2.0 unx      757 b- defN 24-Jun-03 12:17 generated/apps/test/test_rule_behavior.py
+-rw-r--r--  2.0 unx      871 b- defN 24-Jun-03 12:17 generated/apps/test/test_scale_record_autoscaling_action.py
+-rw-r--r--  2.0 unx     6557 b- defN 24-Jun-03 12:17 generated/apps/test/test_v1_app.py
+-rw-r--r--  2.0 unx     5531 b- defN 24-Jun-03 12:17 generated/apps/test/test_v1_app_revision.py
+-rw-r--r--  2.0 unx     8184 b- defN 24-Jun-03 12:17 generated/apps/test/test_v1_app_runtime.py
+-rw-r--r--  2.0 unx     2832 b- defN 24-Jun-03 12:17 generated/apps/test/test_v1_app_service_setup_image_body.py
+-rw-r--r--  2.0 unx      751 b- defN 24-Jun-03 12:17 generated/apps/test/test_v1_app_status.py
+-rw-r--r--  2.0 unx     2243 b- defN 24-Jun-03 12:17 generated/apps/test/test_v1_autoscaling_policy.py
+-rw-r--r--  2.0 unx     1699 b- defN 24-Jun-03 12:17 generated/apps/test/test_v1_basic_auth.py
+-rw-r--r--  2.0 unx     1586 b- defN 24-Jun-03 12:17 generated/apps/test/test_v1_built_in_policy.py
+-rw-r--r--  2.0 unx     2862 b- defN 24-Jun-03 12:17 generated/apps/test/test_v1_check_and_lock_worker_response.py
+-rw-r--r--  2.0 unx     1793 b- defN 24-Jun-03 12:17 generated/apps/test/test_v1_custom_policy.py
+-rw-r--r--  2.0 unx     8812 b- defN 24-Jun-03 12:17 generated/apps/test/test_v1_get_app_runtime_snapshot_response.py
+-rw-r--r--  2.0 unx     1597 b- defN 24-Jun-03 12:17 generated/apps/test/test_v1_get_route_path_response.py
+-rw-r--r--  2.0 unx     1720 b- defN 24-Jun-03 12:17 generated/apps/test/test_v1_get_safety_remove_workers_response.py
+-rw-r--r--  2.0 unx     7552 b- defN 24-Jun-03 12:17 generated/apps/test/test_v1_list_all_apps_response.py
+-rw-r--r--  2.0 unx     7686 b- defN 24-Jun-03 12:17 generated/apps/test/test_v1_list_all_apps_with_workers_response.py
+-rw-r--r--  2.0 unx     2907 b- defN 24-Jun-03 12:17 generated/apps/test/test_v1_list_all_workers_response.py
+-rw-r--r--  2.0 unx     7638 b- defN 24-Jun-03 12:17 generated/apps/test/test_v1_list_app_by_unique_ids_response.py
+-rw-r--r--  2.0 unx     7589 b- defN 24-Jun-03 12:17 generated/apps/test/test_v1_list_apps_by_user_response.py
+-rw-r--r--  2.0 unx     1977 b- defN 24-Jun-03 12:17 generated/apps/test/test_v1_list_request_queues_response.py
+-rw-r--r--  2.0 unx     1916 b- defN 24-Jun-03 12:17 generated/apps/test/test_v1_list_request_queues_response_request_queue.py
+-rw-r--r--  2.0 unx     7466 b- defN 24-Jun-03 12:17 generated/apps/test/test_v1_list_response.py
+-rw-r--r--  2.0 unx     2943 b- defN 24-Jun-03 12:17 generated/apps/test/test_v1_list_worker_details_response.py
+-rw-r--r--  2.0 unx     3018 b- defN 24-Jun-03 12:17 generated/apps/test/test_v1_list_workers_by_app_and_user_response.py
+-rw-r--r--  2.0 unx     3078 b- defN 24-Jun-03 12:17 generated/apps/test/test_v1_list_workers_by_device_and_status_response.py
+-rw-r--r--  2.0 unx     2968 b- defN 24-Jun-03 12:17 generated/apps/test/test_v1_list_workers_by_status_response.py
+-rw-r--r--  2.0 unx     3209 b- defN 24-Jun-03 12:17 generated/apps/test/test_v1_list_workers_response.py
+-rw-r--r--  2.0 unx     1951 b- defN 24-Jun-03 12:17 generated/apps/test/test_v1_resource_claim.py
+-rw-r--r--  2.0 unx     1529 b- defN 24-Jun-03 12:17 generated/apps/test/test_v1_rule.py
+-rw-r--r--  2.0 unx     1504 b- defN 24-Jun-03 12:17 generated/apps/test/test_v1_scale_record.py
+-rw-r--r--  2.0 unx     1592 b- defN 24-Jun-03 12:17 generated/apps/test/test_v1_setup_volume.py
+-rw-r--r--  2.0 unx     1517 b- defN 24-Jun-03 12:17 generated/apps/test/test_v1_value_from_secret.py
+-rw-r--r--  2.0 unx     2400 b- defN 24-Jun-03 12:17 generated/apps/test/test_v1_worker.py
+-rw-r--r--  2.0 unx     2014 b- defN 24-Jun-03 12:17 generated/apps/test/test_v1_worker_runtime.py
+-rw-r--r--  2.0 unx      843 b- defN 24-Jun-03 12:17 generated/apps/test/test_worker_worker_detail_status.py
+-rw-r--r--  2.0 unx      800 b- defN 24-Jun-03 12:17 generated/apps/test/test_worker_worker_status.py
+-rw-r--r--  2.0 unx     1413 b- defN 24-Jun-03 12:17 generated/configmaps/__init__.py
+-rw-r--r--  2.0 unx    29579 b- defN 24-Jun-03 12:17 generated/configmaps/api_client.py
+-rw-r--r--  2.0 unx      852 b- defN 24-Jun-03 12:17 generated/configmaps/api_response.py
+-rw-r--r--  2.0 unx    14419 b- defN 24-Jun-03 12:17 generated/configmaps/configuration.py
+-rw-r--r--  2.0 unx     5462 b- defN 24-Jun-03 12:17 generated/configmaps/exceptions.py
+-rw-r--r--  2.0 unx    12966 b- defN 24-Jun-03 12:17 generated/configmaps/rest.py
+-rw-r--r--  2.0 unx      127 b- defN 24-Jun-03 12:17 generated/configmaps/api/__init__.py
+-rw-r--r--  2.0 unx    32156 b- defN 24-Jun-03 12:17 generated/configmaps/api/configmap_service_api.py
+-rw-r--r--  2.0 unx      736 b- defN 24-Jun-03 12:17 generated/configmaps/models/__init__.py
+-rw-r--r--  2.0 unx     2555 b- defN 24-Jun-03 12:17 generated/configmaps/models/configmap_service_create_body.py
+-rw-r--r--  2.0 unx     2555 b- defN 24-Jun-03 12:17 generated/configmaps/models/configmap_service_update_body.py
+-rw-r--r--  2.0 unx     2764 b- defN 24-Jun-03 12:17 generated/configmaps/models/v1_configmap.py
+-rw-r--r--  2.0 unx     2906 b- defN 24-Jun-03 12:17 generated/configmaps/models/v1_list_response.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Jun-03 12:17 generated/configmaps/test/__init__.py
+-rw-r--r--  2.0 unx     1510 b- defN 24-Jun-03 12:17 generated/configmaps/test/test_configmap_service_api.py
+-rw-r--r--  2.0 unx     1824 b- defN 24-Jun-03 12:17 generated/configmaps/test/test_configmap_service_create_body.py
+-rw-r--r--  2.0 unx     1824 b- defN 24-Jun-03 12:17 generated/configmaps/test/test_configmap_service_update_body.py
+-rw-r--r--  2.0 unx     1775 b- defN 24-Jun-03 12:17 generated/configmaps/test/test_v1_configmap.py
+-rw-r--r--  2.0 unx     1930 b- defN 24-Jun-03 12:17 generated/configmaps/test/test_v1_list_response.py
+-rw-r--r--  2.0 unx     1344 b- defN 24-Jun-03 12:17 generated/secrets/__init__.py
+-rw-r--r--  2.0 unx    29558 b- defN 24-Jun-03 12:17 generated/secrets/api_client.py
+-rw-r--r--  2.0 unx      852 b- defN 24-Jun-03 12:17 generated/secrets/api_response.py
+-rw-r--r--  2.0 unx    14413 b- defN 24-Jun-03 12:17 generated/secrets/configuration.py
+-rw-r--r--  2.0 unx     5459 b- defN 24-Jun-03 12:17 generated/secrets/exceptions.py
+-rw-r--r--  2.0 unx    12960 b- defN 24-Jun-03 12:17 generated/secrets/rest.py
+-rw-r--r--  2.0 unx      118 b- defN 24-Jun-03 12:17 generated/secrets/api/__init__.py
+-rw-r--r--  2.0 unx    31721 b- defN 24-Jun-03 12:17 generated/secrets/api/secret_service_api.py
+-rw-r--r--  2.0 unx      703 b- defN 24-Jun-03 12:17 generated/secrets/models/__init__.py
+-rw-r--r--  2.0 unx     2540 b- defN 24-Jun-03 12:17 generated/secrets/models/secret_service_create_body.py
+-rw-r--r--  2.0 unx     2540 b- defN 24-Jun-03 12:17 generated/secrets/models/secret_service_update_body.py
+-rw-r--r--  2.0 unx     2861 b- defN 24-Jun-03 12:17 generated/secrets/models/v1_list_response.py
+-rw-r--r--  2.0 unx     2749 b- defN 24-Jun-03 12:17 generated/secrets/models/v1_secret.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Jun-03 12:17 generated/secrets/test/__init__.py
+-rw-r--r--  2.0 unx     1441 b- defN 24-Jun-03 12:17 generated/secrets/test/test_secret_service_api.py
+-rw-r--r--  2.0 unx     1782 b- defN 24-Jun-03 12:17 generated/secrets/test/test_secret_service_create_body.py
+-rw-r--r--  2.0 unx     1782 b- defN 24-Jun-03 12:17 generated/secrets/test/test_secret_service_update_body.py
+-rw-r--r--  2.0 unx     1912 b- defN 24-Jun-03 12:17 generated/secrets/test/test_v1_list_response.py
+-rw-r--r--  2.0 unx     1733 b- defN 24-Jun-03 12:17 generated/secrets/test/test_v1_secret.py
+-rw-r--r--  2.0 unx     2997 b- defN 24-Jun-03 12:17 generated/volumes/__init__.py
+-rw-r--r--  2.0 unx    29558 b- defN 24-Jun-03 12:17 generated/volumes/api_client.py
+-rw-r--r--  2.0 unx      852 b- defN 24-Jun-03 12:17 generated/volumes/api_response.py
+-rw-r--r--  2.0 unx    14413 b- defN 24-Jun-03 12:17 generated/volumes/configuration.py
+-rw-r--r--  2.0 unx     5459 b- defN 24-Jun-03 12:17 generated/volumes/exceptions.py
+-rw-r--r--  2.0 unx    12960 b- defN 24-Jun-03 12:17 generated/volumes/rest.py
+-rw-r--r--  2.0 unx      118 b- defN 24-Jun-03 12:17 generated/volumes/api/__init__.py
+-rw-r--r--  2.0 unx   143619 b- defN 24-Jun-03 12:17 generated/volumes/api/volume_service_api.py
+-rw-r--r--  2.0 unx     2356 b- defN 24-Jun-03 12:17 generated/volumes/models/__init__.py
+-rw-r--r--  2.0 unx     2991 b- defN 24-Jun-03 12:17 generated/volumes/models/file_information.py
+-rw-r--r--  2.0 unx     2986 b- defN 24-Jun-03 12:17 generated/volumes/models/v1_file.py
+-rw-r--r--  2.0 unx     2415 b- defN 24-Jun-03 12:17 generated/volumes/models/v1_header_value.py
+-rw-r--r--  2.0 unx     2728 b- defN 24-Jun-03 12:17 generated/volumes/models/v1_initialize_multipart_upload_response.py
+-rw-r--r--  2.0 unx     2855 b- defN 24-Jun-03 12:17 generated/volumes/models/v1_list_files_response.py
+-rw-r--r--  2.0 unx     2855 b- defN 24-Jun-03 12:17 generated/volumes/models/v1_list_parts_response.py
+-rw-r--r--  2.0 unx     2861 b- defN 24-Jun-03 12:17 generated/volumes/models/v1_list_response.py
+-rw-r--r--  2.0 unx     2592 b- defN 24-Jun-03 12:17 generated/volumes/models/v1_part.py
+-rw-r--r--  2.0 unx     2897 b- defN 24-Jun-03 12:17 generated/volumes/models/v1_revision.py
+-rw-r--r--  2.0 unx     3193 b- defN 24-Jun-03 12:17 generated/volumes/models/v1_sign_response.py
+-rw-r--r--  2.0 unx     2910 b- defN 24-Jun-03 12:17 generated/volumes/models/v1_sign_upload_response.py
+-rw-r--r--  2.0 unx      901 b- defN 24-Jun-03 12:17 generated/volumes/models/v1_upload_action.py
+-rw-r--r--  2.0 unx     3421 b- defN 24-Jun-03 12:17 generated/volumes/models/v1_volume.py
+-rw-r--r--  2.0 unx      951 b- defN 24-Jun-03 12:17 generated/volumes/models/v1_volume_status.py
+-rw-r--r--  2.0 unx     2517 b- defN 24-Jun-03 12:17 generated/volumes/models/volume_service_change_revision_body.py
+-rw-r--r--  2.0 unx     2809 b- defN 24-Jun-03 12:17 generated/volumes/models/volume_service_commit_file_body.py
+-rw-r--r--  2.0 unx     3055 b- defN 24-Jun-03 12:17 generated/volumes/models/volume_service_commit_file_body_file.py
+-rw-r--r--  2.0 unx     2876 b- defN 24-Jun-03 12:17 generated/volumes/models/volume_service_commit_revision_body.py
+-rw-r--r--  2.0 unx     3092 b- defN 24-Jun-03 12:17 generated/volumes/models/volume_service_complete_multipart_upload_body.py
+-rw-r--r--  2.0 unx     2464 b- defN 24-Jun-03 12:17 generated/volumes/models/volume_service_create_body.py
+-rw-r--r--  2.0 unx     2801 b- defN 24-Jun-03 12:17 generated/volumes/models/volume_service_initialize_multipart_upload_body.py
+-rw-r--r--  2.0 unx     2527 b- defN 24-Jun-03 12:17 generated/volumes/models/volume_service_sign_multipart_upload_body.py
+-rw-r--r--  2.0 unx     2741 b- defN 24-Jun-03 12:17 generated/volumes/models/volume_service_sign_upload_body.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Jun-03 12:17 generated/volumes/test/__init__.py
+-rw-r--r--  2.0 unx     1716 b- defN 24-Jun-03 12:17 generated/volumes/test/test_file_information.py
+-rw-r--r--  2.0 unx     1718 b- defN 24-Jun-03 12:17 generated/volumes/test/test_v1_file.py
+-rw-r--r--  2.0 unx     1494 b- defN 24-Jun-03 12:17 generated/volumes/test/test_v1_header_value.py
+-rw-r--r--  2.0 unx     1755 b- defN 24-Jun-03 12:17 generated/volumes/test/test_v1_initialize_multipart_upload_response.py
+-rw-r--r--  2.0 unx     1949 b- defN 24-Jun-03 12:17 generated/volumes/test/test_v1_list_files_response.py
+-rw-r--r--  2.0 unx     1721 b- defN 24-Jun-03 12:17 generated/volumes/test/test_v1_list_parts_response.py
+-rw-r--r--  2.0 unx     2162 b- defN 24-Jun-03 12:17 generated/volumes/test/test_v1_list_response.py
+-rw-r--r--  2.0 unx     1486 b- defN 24-Jun-03 12:17 generated/volumes/test/test_v1_part.py
+-rw-r--r--  2.0 unx     1609 b- defN 24-Jun-03 12:17 generated/volumes/test/test_v1_revision.py
+-rw-r--r--  2.0 unx     1722 b- defN 24-Jun-03 12:17 generated/volumes/test/test_v1_sign_response.py
+-rw-r--r--  2.0 unx     1952 b- defN 24-Jun-03 12:17 generated/volumes/test/test_v1_sign_upload_response.py
+-rw-r--r--  2.0 unx      779 b- defN 24-Jun-03 12:17 generated/volumes/test/test_v1_upload_action.py
+-rw-r--r--  2.0 unx     1866 b- defN 24-Jun-03 12:17 generated/volumes/test/test_v1_volume.py
+-rw-r--r--  2.0 unx      779 b- defN 24-Jun-03 12:17 generated/volumes/test/test_v1_volume_status.py
+-rw-r--r--  2.0 unx     4249 b- defN 24-Jun-03 12:17 generated/volumes/test/test_volume_service_api.py
+-rw-r--r--  2.0 unx     1712 b- defN 24-Jun-03 12:17 generated/volumes/test/test_volume_service_change_revision_body.py
+-rw-r--r--  2.0 unx     2004 b- defN 24-Jun-03 12:17 generated/volumes/test/test_volume_service_commit_file_body.py
+-rw-r--r--  2.0 unx     1912 b- defN 24-Jun-03 12:17 generated/volumes/test/test_volume_service_commit_file_body_file.py
+-rw-r--r--  2.0 unx     2548 b- defN 24-Jun-03 12:17 generated/volumes/test/test_volume_service_commit_revision_body.py
+-rw-r--r--  2.0 unx     2233 b- defN 24-Jun-03 12:17 generated/volumes/test/test_volume_service_complete_multipart_upload_body.py
+-rw-r--r--  2.0 unx     1624 b- defN 24-Jun-03 12:17 generated/volumes/test/test_volume_service_create_body.py
+-rw-r--r--  2.0 unx     2149 b- defN 24-Jun-03 12:17 generated/volumes/test/test_volume_service_initialize_multipart_upload_body.py
+-rw-r--r--  2.0 unx     1769 b- defN 24-Jun-03 12:17 generated/volumes/test/test_volume_service_sign_multipart_upload_body.py
+-rw-r--r--  2.0 unx     1968 b- defN 24-Jun-03 12:17 generated/volumes/test/test_volume_service_sign_upload_body.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Jun-03 12:32 everai-0.1.63.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1985 b- defN 24-Jun-03 12:32 everai-0.1.63.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Jun-03 12:32 everai-0.1.63.dist-info/WHEEL
+-rw-r--r--  2.0 unx       98 b- defN 24-Jun-03 12:32 everai-0.1.63.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       17 b- defN 24-Jun-03 12:32 everai-0.1.63.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    32538 b- defN 24-Jun-03 12:32 everai-0.1.63.dist-info/RECORD
+335 files, 1232940 bytes uncompressed, 297659 bytes compressed:  75.9%
```

## zipnote {}

```diff
@@ -102,14 +102,17 @@
 
 Filename: everai/commands/app/prepare.py
 Comment: 
 
 Filename: everai/commands/app/queue.py
 Comment: 
 
+Filename: everai/commands/app/resume.py
+Comment: 
+
 Filename: everai/commands/app/upgrade.py
 Comment: 
 
 Filename: everai/commands/app/utils.py
 Comment: 
 
 Filename: everai/commands/auth/__init__.py
@@ -372,660 +375,390 @@
 
 Filename: everai/worker/worker.py
 Comment: 
 
 Filename: generated/__init__.py
 Comment: 
 
-Filename: generated/configmaps/__init__.py
-Comment: 
-
-Filename: generated/configmaps/api_client.py
-Comment: 
-
-Filename: generated/configmaps/api_response.py
-Comment: 
-
-Filename: generated/configmaps/configuration.py
-Comment: 
-
-Filename: generated/configmaps/exceptions.py
-Comment: 
-
-Filename: generated/configmaps/rest.py
-Comment: 
-
-Filename: generated/configmaps/api/__init__.py
-Comment: 
-
-Filename: generated/configmaps/api/configmap_service_api.py
-Comment: 
-
-Filename: generated/configmaps/models/__init__.py
-Comment: 
-
-Filename: generated/configmaps/models/configmap_service_create_body.py
-Comment: 
-
-Filename: generated/configmaps/models/configmap_service_update_body.py
-Comment: 
-
-Filename: generated/configmaps/models/v1_configmap.py
-Comment: 
-
-Filename: generated/configmaps/models/v1_list_response.py
-Comment: 
-
-Filename: generated/configmaps/test/__init__.py
-Comment: 
-
-Filename: generated/configmaps/test/test_configmap_service_api.py
-Comment: 
-
-Filename: generated/configmaps/test/test_configmap_service_create_body.py
-Comment: 
-
-Filename: generated/configmaps/test/test_configmap_service_update_body.py
-Comment: 
-
-Filename: generated/configmaps/test/test_v1_configmap.py
-Comment: 
-
-Filename: generated/configmaps/test/test_v1_list_response.py
-Comment: 
-
-Filename: generated/schedulers/__init__.py
-Comment: 
-
-Filename: generated/schedulers/api_client.py
-Comment: 
-
-Filename: generated/schedulers/api_response.py
-Comment: 
-
-Filename: generated/schedulers/configuration.py
-Comment: 
-
-Filename: generated/schedulers/exceptions.py
-Comment: 
-
-Filename: generated/schedulers/rest.py
-Comment: 
-
-Filename: generated/schedulers/api/__init__.py
-Comment: 
-
-Filename: generated/schedulers/api/app_service_api.py
-Comment: 
-
-Filename: generated/schedulers/models/__init__.py
-Comment: 
-
-Filename: generated/schedulers/models/app_service_create_body.py
-Comment: 
-
-Filename: generated/schedulers/models/app_service_inference_body.py
-Comment: 
-
-Filename: generated/schedulers/models/app_service_resources_body.py
-Comment: 
-
-Filename: generated/schedulers/models/app_service_setup_auto_scaling_policy_body.py
-Comment: 
-
-Filename: generated/schedulers/models/app_service_setup_body.py
-Comment: 
-
-Filename: generated/schedulers/models/app_service_setup_resource_body.py
-Comment: 
-
-Filename: generated/schedulers/models/app_service_setup_resources_body.py
-Comment: 
-
-Filename: generated/schedulers/models/app_service_setup_secrets_body.py
-Comment: 
-
-Filename: generated/schedulers/models/app_service_setup_volumes_body.py
-Comment: 
-
-Filename: generated/schedulers/models/appsv1_cpu.py
-Comment: 
-
-Filename: generated/schedulers/models/appsv1_gpu.py
-Comment: 
-
-Filename: generated/schedulers/models/appsv1_setup_image.py
-Comment: 
-
-Filename: generated/schedulers/models/appsv1_worker.py
-Comment: 
-
-Filename: generated/schedulers/models/list_request_queues_response_queue_reason.py
-Comment: 
-
-Filename: generated/schedulers/models/list_request_queues_response_request_queue.py
-Comment: 
-
-Filename: generated/schedulers/models/protobuf_any.py
-Comment: 
-
-Filename: generated/schedulers/models/rule_behavior.py
-Comment: 
-
-Filename: generated/schedulers/models/schedulerv1_cpu.py
-Comment: 
-
-Filename: generated/schedulers/models/schedulerv1_gpu.py
-Comment: 
-
-Filename: generated/schedulers/models/v1_app.py
-Comment: 
-
-Filename: generated/schedulers/models/v1_app_service_setup_image_body.py
-Comment: 
-
-Filename: generated/schedulers/models/v1_app_status.py
-Comment: 
-
-Filename: generated/schedulers/models/v1_autoscaling_policy.py
-Comment: 
-
-Filename: generated/schedulers/models/v1_bandwidth.py
-Comment: 
-
-Filename: generated/schedulers/models/v1_bandwidth_size.py
-Comment: 
-
-Filename: generated/schedulers/models/v1_basic_auth.py
-Comment: 
-
-Filename: generated/schedulers/models/v1_build_in_policy.py
-Comment: 
-
-Filename: generated/schedulers/models/v1_built_in_policy.py
-Comment: 
-
-Filename: generated/schedulers/models/v1_cpu.py
-Comment: 
-
-Filename: generated/schedulers/models/v1_create_volume_request.py
-Comment: 
-
-Filename: generated/schedulers/models/v1_create_volume_response.py
-Comment: 
-
-Filename: generated/schedulers/models/v1_custom_policy.py
-Comment: 
-
-Filename: generated/schedulers/models/v1_delete_volume_request.py
-Comment: 
-
-Filename: generated/schedulers/models/v1_delete_volume_response.py
-Comment: 
-
-Filename: generated/schedulers/models/v1_device_resource.py
-Comment: 
-
-Filename: generated/schedulers/models/v1_empty_response.py
-Comment: 
-
-Filename: generated/schedulers/models/v1_error_response.py
-Comment: 
-
-Filename: generated/schedulers/models/v1_filesystem.py
-Comment: 
-
-Filename: generated/schedulers/models/v1_get_image_request.py
-Comment: 
-
-Filename: generated/schedulers/models/v1_get_image_response.py
-Comment: 
-
-Filename: generated/schedulers/models/v1_get_volume_request.py
-Comment: 
-
-Filename: generated/schedulers/models/v1_get_volume_response.py
-Comment: 
-
-Filename: generated/schedulers/models/v1_get_worker_request.py
-Comment: 
-
-Filename: generated/schedulers/models/v1_get_worker_response.py
-Comment: 
-
-Filename: generated/schedulers/models/v1_gpu.py
+Filename: generated/apps/__init__.py
 Comment: 
 
-Filename: generated/schedulers/models/v1_gpu_opts.py
+Filename: generated/apps/api_client.py
 Comment: 
 
-Filename: generated/schedulers/models/v1_header_entry.py
+Filename: generated/apps/api_response.py
 Comment: 
 
-Filename: generated/schedulers/models/v1_image.py
+Filename: generated/apps/configuration.py
 Comment: 
 
-Filename: generated/schedulers/models/v1_image_request.py
+Filename: generated/apps/exceptions.py
 Comment: 
 
-Filename: generated/schedulers/models/v1_image_status.py
+Filename: generated/apps/rest.py
 Comment: 
 
-Filename: generated/schedulers/models/v1_inference_response.py
+Filename: generated/apps/api/__init__.py
 Comment: 
 
-Filename: generated/schedulers/models/v1_list_image_request.py
+Filename: generated/apps/api/app_service_api.py
 Comment: 
 
-Filename: generated/schedulers/models/v1_list_image_response.py
+Filename: generated/apps/models/__init__.py
 Comment: 
 
-Filename: generated/schedulers/models/v1_list_request_queues_response.py
+Filename: generated/apps/models/app_route_auth_status.py
 Comment: 
 
-Filename: generated/schedulers/models/v1_list_response.py
+Filename: generated/apps/models/app_runtimev1_request_queue.py
 Comment: 
 
-Filename: generated/schedulers/models/v1_list_volume_request.py
+Filename: generated/apps/models/app_service_create_body.py
 Comment: 
 
-Filename: generated/schedulers/models/v1_list_volume_response.py
+Filename: generated/apps/models/app_service_protect_app_body.py
 Comment: 
 
-Filename: generated/schedulers/models/v1_list_worker_request.py
+Filename: generated/apps/models/app_service_setup_auto_scaling_policy_body.py
 Comment: 
 
-Filename: generated/schedulers/models/v1_list_worker_response.py
+Filename: generated/apps/models/app_service_setup_resources_body.py
 Comment: 
 
-Filename: generated/schedulers/models/v1_list_workers_response.py
+Filename: generated/apps/models/app_service_setup_secrets_body.py
 Comment: 
 
-Filename: generated/schedulers/models/v1_pull_image_request.py
+Filename: generated/apps/models/app_service_setup_volumes_body.py
 Comment: 
 
-Filename: generated/schedulers/models/v1_pull_image_response.py
+Filename: generated/apps/models/appsv1_setup_image.py
 Comment: 
 
-Filename: generated/schedulers/models/v1_remove_image_request.py
+Filename: generated/apps/models/list_request_queues_response_queue_reason.py
 Comment: 
 
-Filename: generated/schedulers/models/v1_resource_claim.py
+Filename: generated/apps/models/protobuf_any.py
 Comment: 
 
-Filename: generated/schedulers/models/v1_resources.py
+Filename: generated/apps/models/rule_behavior.py
 Comment: 
 
-Filename: generated/schedulers/models/v1_restart_worker_request.py
+Filename: generated/apps/models/scale_record_autoscaling_action.py
 Comment: 
 
-Filename: generated/schedulers/models/v1_route_request.py
+Filename: generated/apps/models/v1_app.py
 Comment: 
 
-Filename: generated/schedulers/models/v1_rule.py
+Filename: generated/apps/models/v1_app_revision.py
 Comment: 
 
-Filename: generated/schedulers/models/v1_run_worker_request.py
+Filename: generated/apps/models/v1_app_runtime.py
 Comment: 
 
-Filename: generated/schedulers/models/v1_run_worker_response.py
+Filename: generated/apps/models/v1_app_service_setup_image_body.py
 Comment: 
 
-Filename: generated/schedulers/models/v1_setting.py
+Filename: generated/apps/models/v1_app_status.py
 Comment: 
 
-Filename: generated/schedulers/models/v1_setup_image.py
+Filename: generated/apps/models/v1_autoscaling_policy.py
 Comment: 
 
-Filename: generated/schedulers/models/v1_setup_secrets.py
+Filename: generated/apps/models/v1_basic_auth.py
 Comment: 
 
-Filename: generated/schedulers/models/v1_setup_volume.py
+Filename: generated/apps/models/v1_built_in_policy.py
 Comment: 
 
-Filename: generated/schedulers/models/v1_setup_volumes.py
+Filename: generated/apps/models/v1_check_and_lock_worker_response.py
 Comment: 
 
-Filename: generated/schedulers/models/v1_setup_volumes_volume.py
+Filename: generated/apps/models/v1_custom_policy.py
 Comment: 
 
-Filename: generated/schedulers/models/v1_stop_worker_request.py
+Filename: generated/apps/models/v1_get_app_runtime_snapshot_response.py
 Comment: 
 
-Filename: generated/schedulers/models/v1_storage_size.py
+Filename: generated/apps/models/v1_get_route_path_response.py
 Comment: 
 
-Filename: generated/schedulers/models/v1_sync_volume_request.py
+Filename: generated/apps/models/v1_get_safety_remove_workers_response.py
 Comment: 
 
-Filename: generated/schedulers/models/v1_sync_volume_response.py
+Filename: generated/apps/models/v1_list_all_apps_response.py
 Comment: 
 
-Filename: generated/schedulers/models/v1_value_from_secret.py
+Filename: generated/apps/models/v1_list_all_apps_with_workers_response.py
 Comment: 
 
-Filename: generated/schedulers/models/v1_volume.py
+Filename: generated/apps/models/v1_list_all_workers_response.py
 Comment: 
 
-Filename: generated/schedulers/models/v1_volume_mount.py
+Filename: generated/apps/models/v1_list_app_by_unique_ids_response.py
 Comment: 
 
-Filename: generated/schedulers/models/v1_volume_request.py
+Filename: generated/apps/models/v1_list_apps_by_user_response.py
 Comment: 
 
-Filename: generated/schedulers/models/v1_volume_status.py
+Filename: generated/apps/models/v1_list_request_queues_response.py
 Comment: 
 
-Filename: generated/schedulers/models/v1_worker.py
+Filename: generated/apps/models/v1_list_request_queues_response_request_queue.py
 Comment: 
 
-Filename: generated/schedulers/models/v1_worker_request.py
+Filename: generated/apps/models/v1_list_response.py
 Comment: 
 
-Filename: generated/schedulers/models/v1_worker_status.py
+Filename: generated/apps/models/v1_list_worker_details_response.py
 Comment: 
 
-Filename: generated/schedulers/models/v1_worker_worker_status.py
+Filename: generated/apps/models/v1_list_workers_by_app_and_user_response.py
 Comment: 
 
-Filename: generated/schedulers/models/v1workersv1_worker.py
+Filename: generated/apps/models/v1_list_workers_by_device_and_status_response.py
 Comment: 
 
-Filename: generated/schedulers/models/volumesv1_volume.py
+Filename: generated/apps/models/v1_list_workers_by_status_response.py
 Comment: 
 
-Filename: generated/schedulers/models/worker_worker_detail_status.py
+Filename: generated/apps/models/v1_list_workers_response.py
 Comment: 
 
-Filename: generated/schedulers/models/workersv1_worker_status.py
+Filename: generated/apps/models/v1_resource_claim.py
 Comment: 
 
-Filename: generated/schedulers/test/__init__.py
+Filename: generated/apps/models/v1_rule.py
 Comment: 
 
-Filename: generated/schedulers/test/test_app_service_api.py
+Filename: generated/apps/models/v1_scale_record.py
 Comment: 
 
-Filename: generated/schedulers/test/test_app_service_create_body.py
+Filename: generated/apps/models/v1_setup_volume.py
 Comment: 
 
-Filename: generated/schedulers/test/test_app_service_inference_body.py
+Filename: generated/apps/models/v1_value_from_secret.py
 Comment: 
 
-Filename: generated/schedulers/test/test_app_service_resources_body.py
+Filename: generated/apps/models/v1_worker.py
 Comment: 
 
-Filename: generated/schedulers/test/test_app_service_setup_auto_scaling_policy_body.py
+Filename: generated/apps/models/v1_worker_runtime.py
 Comment: 
 
-Filename: generated/schedulers/test/test_app_service_setup_body.py
+Filename: generated/apps/models/worker_worker_detail_status.py
 Comment: 
 
-Filename: generated/schedulers/test/test_app_service_setup_resource_body.py
+Filename: generated/apps/models/worker_worker_status.py
 Comment: 
 
-Filename: generated/schedulers/test/test_app_service_setup_resources_body.py
+Filename: generated/apps/test/__init__.py
 Comment: 
 
-Filename: generated/schedulers/test/test_app_service_setup_secrets_body.py
+Filename: generated/apps/test/test_app_route_auth_status.py
 Comment: 
 
-Filename: generated/schedulers/test/test_app_service_setup_volumes_body.py
+Filename: generated/apps/test/test_app_runtimev1_request_queue.py
 Comment: 
 
-Filename: generated/schedulers/test/test_appsv1_cpu.py
+Filename: generated/apps/test/test_app_service_api.py
 Comment: 
 
-Filename: generated/schedulers/test/test_appsv1_gpu.py
+Filename: generated/apps/test/test_app_service_create_body.py
 Comment: 
 
-Filename: generated/schedulers/test/test_appsv1_setup_image.py
+Filename: generated/apps/test/test_app_service_protect_app_body.py
 Comment: 
 
-Filename: generated/schedulers/test/test_appsv1_worker.py
+Filename: generated/apps/test/test_app_service_setup_auto_scaling_policy_body.py
 Comment: 
 
-Filename: generated/schedulers/test/test_list_request_queues_response_queue_reason.py
+Filename: generated/apps/test/test_app_service_setup_resources_body.py
 Comment: 
 
-Filename: generated/schedulers/test/test_list_request_queues_response_request_queue.py
+Filename: generated/apps/test/test_app_service_setup_secrets_body.py
 Comment: 
 
-Filename: generated/schedulers/test/test_protobuf_any.py
+Filename: generated/apps/test/test_app_service_setup_volumes_body.py
 Comment: 
 
-Filename: generated/schedulers/test/test_rule_behavior.py
+Filename: generated/apps/test/test_appsv1_setup_image.py
 Comment: 
 
-Filename: generated/schedulers/test/test_schedulerv1_cpu.py
+Filename: generated/apps/test/test_list_request_queues_response_queue_reason.py
 Comment: 
 
-Filename: generated/schedulers/test/test_schedulerv1_gpu.py
+Filename: generated/apps/test/test_protobuf_any.py
 Comment: 
 
-Filename: generated/schedulers/test/test_v1_app.py
+Filename: generated/apps/test/test_rule_behavior.py
 Comment: 
 
-Filename: generated/schedulers/test/test_v1_app_service_setup_image_body.py
+Filename: generated/apps/test/test_scale_record_autoscaling_action.py
 Comment: 
 
-Filename: generated/schedulers/test/test_v1_app_status.py
+Filename: generated/apps/test/test_v1_app.py
 Comment: 
 
-Filename: generated/schedulers/test/test_v1_autoscaling_policy.py
+Filename: generated/apps/test/test_v1_app_revision.py
 Comment: 
 
-Filename: generated/schedulers/test/test_v1_bandwidth.py
+Filename: generated/apps/test/test_v1_app_runtime.py
 Comment: 
 
-Filename: generated/schedulers/test/test_v1_bandwidth_size.py
+Filename: generated/apps/test/test_v1_app_service_setup_image_body.py
 Comment: 
 
-Filename: generated/schedulers/test/test_v1_basic_auth.py
+Filename: generated/apps/test/test_v1_app_status.py
 Comment: 
 
-Filename: generated/schedulers/test/test_v1_build_in_policy.py
+Filename: generated/apps/test/test_v1_autoscaling_policy.py
 Comment: 
 
-Filename: generated/schedulers/test/test_v1_built_in_policy.py
+Filename: generated/apps/test/test_v1_basic_auth.py
 Comment: 
 
-Filename: generated/schedulers/test/test_v1_cpu.py
+Filename: generated/apps/test/test_v1_built_in_policy.py
 Comment: 
 
-Filename: generated/schedulers/test/test_v1_create_volume_request.py
+Filename: generated/apps/test/test_v1_check_and_lock_worker_response.py
 Comment: 
 
-Filename: generated/schedulers/test/test_v1_create_volume_response.py
+Filename: generated/apps/test/test_v1_custom_policy.py
 Comment: 
 
-Filename: generated/schedulers/test/test_v1_custom_policy.py
+Filename: generated/apps/test/test_v1_get_app_runtime_snapshot_response.py
 Comment: 
 
-Filename: generated/schedulers/test/test_v1_delete_volume_request.py
+Filename: generated/apps/test/test_v1_get_route_path_response.py
 Comment: 
 
-Filename: generated/schedulers/test/test_v1_delete_volume_response.py
+Filename: generated/apps/test/test_v1_get_safety_remove_workers_response.py
 Comment: 
 
-Filename: generated/schedulers/test/test_v1_device_resource.py
+Filename: generated/apps/test/test_v1_list_all_apps_response.py
 Comment: 
 
-Filename: generated/schedulers/test/test_v1_empty_response.py
+Filename: generated/apps/test/test_v1_list_all_apps_with_workers_response.py
 Comment: 
 
-Filename: generated/schedulers/test/test_v1_error_response.py
+Filename: generated/apps/test/test_v1_list_all_workers_response.py
 Comment: 
 
-Filename: generated/schedulers/test/test_v1_filesystem.py
+Filename: generated/apps/test/test_v1_list_app_by_unique_ids_response.py
 Comment: 
 
-Filename: generated/schedulers/test/test_v1_get_image_request.py
+Filename: generated/apps/test/test_v1_list_apps_by_user_response.py
 Comment: 
 
-Filename: generated/schedulers/test/test_v1_get_image_response.py
+Filename: generated/apps/test/test_v1_list_request_queues_response.py
 Comment: 
 
-Filename: generated/schedulers/test/test_v1_get_volume_request.py
+Filename: generated/apps/test/test_v1_list_request_queues_response_request_queue.py
 Comment: 
 
-Filename: generated/schedulers/test/test_v1_get_volume_response.py
+Filename: generated/apps/test/test_v1_list_response.py
 Comment: 
 
-Filename: generated/schedulers/test/test_v1_get_worker_request.py
+Filename: generated/apps/test/test_v1_list_worker_details_response.py
 Comment: 
 
-Filename: generated/schedulers/test/test_v1_get_worker_response.py
+Filename: generated/apps/test/test_v1_list_workers_by_app_and_user_response.py
 Comment: 
 
-Filename: generated/schedulers/test/test_v1_gpu.py
+Filename: generated/apps/test/test_v1_list_workers_by_device_and_status_response.py
 Comment: 
 
-Filename: generated/schedulers/test/test_v1_gpu_opts.py
+Filename: generated/apps/test/test_v1_list_workers_by_status_response.py
 Comment: 
 
-Filename: generated/schedulers/test/test_v1_header_entry.py
+Filename: generated/apps/test/test_v1_list_workers_response.py
 Comment: 
 
-Filename: generated/schedulers/test/test_v1_image.py
+Filename: generated/apps/test/test_v1_resource_claim.py
 Comment: 
 
-Filename: generated/schedulers/test/test_v1_image_request.py
+Filename: generated/apps/test/test_v1_rule.py
 Comment: 
 
-Filename: generated/schedulers/test/test_v1_image_status.py
+Filename: generated/apps/test/test_v1_scale_record.py
 Comment: 
 
-Filename: generated/schedulers/test/test_v1_inference_response.py
+Filename: generated/apps/test/test_v1_setup_volume.py
 Comment: 
 
-Filename: generated/schedulers/test/test_v1_list_image_request.py
+Filename: generated/apps/test/test_v1_value_from_secret.py
 Comment: 
 
-Filename: generated/schedulers/test/test_v1_list_image_response.py
+Filename: generated/apps/test/test_v1_worker.py
 Comment: 
 
-Filename: generated/schedulers/test/test_v1_list_request_queues_response.py
+Filename: generated/apps/test/test_v1_worker_runtime.py
 Comment: 
 
-Filename: generated/schedulers/test/test_v1_list_response.py
+Filename: generated/apps/test/test_worker_worker_detail_status.py
 Comment: 
 
-Filename: generated/schedulers/test/test_v1_list_volume_request.py
+Filename: generated/apps/test/test_worker_worker_status.py
 Comment: 
 
-Filename: generated/schedulers/test/test_v1_list_volume_response.py
-Comment: 
-
-Filename: generated/schedulers/test/test_v1_list_worker_request.py
-Comment: 
-
-Filename: generated/schedulers/test/test_v1_list_worker_response.py
-Comment: 
-
-Filename: generated/schedulers/test/test_v1_list_workers_response.py
-Comment: 
-
-Filename: generated/schedulers/test/test_v1_pull_image_request.py
-Comment: 
-
-Filename: generated/schedulers/test/test_v1_pull_image_response.py
-Comment: 
-
-Filename: generated/schedulers/test/test_v1_remove_image_request.py
-Comment: 
-
-Filename: generated/schedulers/test/test_v1_resource_claim.py
-Comment: 
-
-Filename: generated/schedulers/test/test_v1_resources.py
-Comment: 
-
-Filename: generated/schedulers/test/test_v1_restart_worker_request.py
-Comment: 
-
-Filename: generated/schedulers/test/test_v1_route_request.py
-Comment: 
-
-Filename: generated/schedulers/test/test_v1_rule.py
-Comment: 
-
-Filename: generated/schedulers/test/test_v1_run_worker_request.py
-Comment: 
-
-Filename: generated/schedulers/test/test_v1_run_worker_response.py
-Comment: 
-
-Filename: generated/schedulers/test/test_v1_setting.py
-Comment: 
-
-Filename: generated/schedulers/test/test_v1_setup_image.py
-Comment: 
-
-Filename: generated/schedulers/test/test_v1_setup_secrets.py
-Comment: 
-
-Filename: generated/schedulers/test/test_v1_setup_volume.py
-Comment: 
-
-Filename: generated/schedulers/test/test_v1_setup_volumes.py
+Filename: generated/configmaps/__init__.py
 Comment: 
 
-Filename: generated/schedulers/test/test_v1_setup_volumes_volume.py
+Filename: generated/configmaps/api_client.py
 Comment: 
 
-Filename: generated/schedulers/test/test_v1_stop_worker_request.py
+Filename: generated/configmaps/api_response.py
 Comment: 
 
-Filename: generated/schedulers/test/test_v1_storage_size.py
+Filename: generated/configmaps/configuration.py
 Comment: 
 
-Filename: generated/schedulers/test/test_v1_sync_volume_request.py
+Filename: generated/configmaps/exceptions.py
 Comment: 
 
-Filename: generated/schedulers/test/test_v1_sync_volume_response.py
+Filename: generated/configmaps/rest.py
 Comment: 
 
-Filename: generated/schedulers/test/test_v1_value_from_secret.py
+Filename: generated/configmaps/api/__init__.py
 Comment: 
 
-Filename: generated/schedulers/test/test_v1_volume.py
+Filename: generated/configmaps/api/configmap_service_api.py
 Comment: 
 
-Filename: generated/schedulers/test/test_v1_volume_mount.py
+Filename: generated/configmaps/models/__init__.py
 Comment: 
 
-Filename: generated/schedulers/test/test_v1_volume_request.py
+Filename: generated/configmaps/models/configmap_service_create_body.py
 Comment: 
 
-Filename: generated/schedulers/test/test_v1_volume_status.py
+Filename: generated/configmaps/models/configmap_service_update_body.py
 Comment: 
 
-Filename: generated/schedulers/test/test_v1_worker.py
+Filename: generated/configmaps/models/v1_configmap.py
 Comment: 
 
-Filename: generated/schedulers/test/test_v1_worker_request.py
+Filename: generated/configmaps/models/v1_list_response.py
 Comment: 
 
-Filename: generated/schedulers/test/test_v1_worker_status.py
+Filename: generated/configmaps/test/__init__.py
 Comment: 
 
-Filename: generated/schedulers/test/test_v1_worker_worker_status.py
+Filename: generated/configmaps/test/test_configmap_service_api.py
 Comment: 
 
-Filename: generated/schedulers/test/test_v1workersv1_worker.py
+Filename: generated/configmaps/test/test_configmap_service_create_body.py
 Comment: 
 
-Filename: generated/schedulers/test/test_volumesv1_volume.py
+Filename: generated/configmaps/test/test_configmap_service_update_body.py
 Comment: 
 
-Filename: generated/schedulers/test/test_worker_worker_detail_status.py
+Filename: generated/configmaps/test/test_v1_configmap.py
 Comment: 
 
-Filename: generated/schedulers/test/test_workersv1_worker_status.py
+Filename: generated/configmaps/test/test_v1_list_response.py
 Comment: 
 
 Filename: generated/secrets/__init__.py
 Comment: 
 
 Filename: generated/secrets/api_client.py
 Comment: 
@@ -1248,26 +981,26 @@
 
 Filename: generated/volumes/test/test_volume_service_sign_multipart_upload_body.py
 Comment: 
 
 Filename: generated/volumes/test/test_volume_service_sign_upload_body.py
 Comment: 
 
-Filename: everai-0.1.62.dist-info/LICENSE
+Filename: everai-0.1.63.dist-info/LICENSE
 Comment: 
 
-Filename: everai-0.1.62.dist-info/METADATA
+Filename: everai-0.1.63.dist-info/METADATA
 Comment: 
 
-Filename: everai-0.1.62.dist-info/WHEEL
+Filename: everai-0.1.63.dist-info/WHEEL
 Comment: 
 
-Filename: everai-0.1.62.dist-info/entry_points.txt
+Filename: everai-0.1.63.dist-info/entry_points.txt
 Comment: 
 
-Filename: everai-0.1.62.dist-info/top_level.txt
+Filename: everai-0.1.63.dist-info/top_level.txt
 Comment: 
 
-Filename: everai-0.1.62.dist-info/RECORD
+Filename: everai-0.1.63.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## everai/constants.py

```diff
@@ -43,7 +43,9 @@
 MAX_SINGLE_FILE_SIZE = 5 * 1024 * 1024
 
 DEFAULT_PART_SIZE = 32 * 1024 * 1024
 
 TIME_FORMAT = '%Y-%m-%d %H:%M:%S'
 
 PART_NUMBER_KEY = 'partNumber'
+
+EVERAI_IN_CLOUD = os.getenv('EVERAI_IN_CLOUD', '0')
```

## everai/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "0.1.62"
+__version__ = "0.1.63"
```

## everai/api/api.py

```diff
@@ -3,31 +3,33 @@
 
 from everai.token_manager import TokenManager
 from generated.configmaps import (
     ApiClient as ConfigMapsClient,
     ConfigmapServiceApi, V1Configmap, ConfigmapServiceCreateBody, ConfigmapServiceUpdateBody
 )
 
-from generated.schedulers import (
-    ApiClient as SchedulersClient,
+from generated.apps import (
+    ApiClient as AppsClient,
     V1App,
     AppServiceCreateBody,
     V1AppServiceSetupImageBody,
     Appsv1SetupImage,
     V1BasicAuth,
     V1ValueFromSecret,
     AppServiceSetupVolumesBody,
     AppServiceApi,
     V1SetupVolume,
     AppServiceSetupSecretsBody,
     AppServiceSetupResourcesBody,
     V1ResourceClaim,
     AppServiceSetupAutoScalingPolicyBody,
     V1AutoscalingPolicy,
-    V1BuiltInPolicy, Appsv1Worker, ListRequestQueuesResponseRequestQueue,
+    V1BuiltInPolicy,
+    V1Worker, 
+    V1ListRequestQueuesResponseRequestQueue,
 )
 
 from generated.volumes import (
     ApiClient as VolumesClient,
     Configuration,
     V1Volume,
     V1File,
@@ -93,15 +95,15 @@
     service_api = svc_type(client)
     return client, service_api
 
 
 class API:
     token: typing.Optional[str]
     volumes_client: VolumesClient
-    schedulers_client: SchedulersClient
+    apps_client: AppsClient
     secrets_client: SecretsClient
     configmaps_client: ConfigMapsClient
 
     app_service_api: AppServiceApi
     secret_service_api: SecretServiceApi
     volume_service_api: VolumeServiceApi
     configmap_service_api: ConfigmapServiceApi
@@ -109,16 +111,16 @@
     def __init__(self, endpoint: str = None):
         endpoint = endpoint or EVERAI_ENDPOINT
         self.token = TokenManager().get_token()
 
         self.volumes_client, self.volume_service_api = (
             _create_api(VolumesClient, VolumeServiceApi, self.token, endpoint))
 
-        self.schedulers_client, self.app_service_api = (
-            _create_api(SchedulersClient, AppServiceApi, self.token, endpoint))
+        self.apps_client, self.app_service_api = (
+            _create_api(AppsClient, AppServiceApi, self.token, endpoint))
 
         self.secrets_client, self.secret_service_api = (
             _create_api(SecretsClient, SecretServiceApi, self.token, endpoint))
 
         self.configmaps_client, self.configmap_service_api = (
             _create_api(ConfigMapsClient, ConfigmapServiceApi, self.token, endpoint))
 
@@ -287,17 +289,20 @@
     def list_apps(self) -> typing.List[V1App]:
         apps = self.app_service_api.list_apps().apps
         return apps
 
     def pause_app(self, name: str) -> None:
         self.app_service_api.pause_app(app_name=name)
 
+    def resume_app(self, name: str) -> None:
+        self.app_service_api.resume_app(app_name=name)
+
     @check_token
     def create_app(self, name: str, route_name: typing.Optional[str] = None) -> V1App:
-        return AppServiceApi(self.schedulers_client).create_app(
+        return self.app_service_api.create_app(
             app_name=name,
             body=AppServiceCreateBody(
                 route_path=route_name or name,
             ),
         )
 
     def setup_image(self, app_name: str, repository: str, tag: str = None, digest: str = None,
@@ -354,15 +359,15 @@
                                                                )
                                                            ),
                                                        ))
 
     def list_worker(self, app_name: str,
                     show_all: bool = False,
                     recent_days: int = 2,
-                    ) -> typing.List[Appsv1Worker]:
+                    ) -> typing.List[V1Worker]:
         resp = self.app_service_api.list_workers(
             app_name=app_name,
             show_all=show_all,
             recent_days=recent_days,
         )
         return resp.workers or []
 
@@ -387,10 +392,10 @@
     def get_configmap(self, name: str) -> V1Configmap:
         resp = self.configmap_service_api.get_configmap(name)
         return resp
 
     def delete_configmap(self, name: str) -> None:
         self.configmap_service_api.delete_configmap(name)
 
-    def list_queue(self, app_name: str) -> typing.List[ListRequestQueuesResponseRequestQueue]:
+    def list_queue(self, app_name: str) -> typing.List[V1ListRequestQueuesResponseRequestQueue]:
         resp = self.app_service_api.list_request_queues(app_name=app_name)
         return resp.queues
```

## everai/app/app.py

```diff
@@ -7,15 +7,15 @@
 from everai.autoscaling.autoscaling_policy import AutoScalingPolicy
 from everai.image import Image
 from everai.resource_requests.resource_requests import ResourceRequests
 from everai.app.service import Service
 from everai.app.volume_request import VolumeRequest
 import typing
 
-from generated.schedulers import V1App, V1AppStatus
+from generated.apps import V1App, V1AppStatus
 from everai.app.app_runner import AppRunnerMixin
 from everai.utils.datetime import format_datetime
 
 
 class App(AppRunnerMixin, ShowMixin):
     _name: str
     _route_name: str
```

## everai/app/app_manager.py

```diff
@@ -25,18 +25,18 @@
 from gevent.pywsgi import WSGIServer
 import gevent.signal
 import signal
 
 from flask import Flask, Blueprint, Response
 
 from everai.worker.worker import Worker
-from generated.schedulers import (
+from generated.apps import (
     ApiException,
     V1SetupVolume,
-    V1ResourceClaim,
+    V1ResourceClaim, V1AppStatus,
 )
 from generated.volumes.exceptions import NotFoundException as VolumeNotFoundException
 
 autoscaling_warning = """
 You are deploying an app without autoscaling_policy, 
 that will cause the app to run only one worker and always one worker,
 if you want to setup an autoscaling_policy for this app after deploy,
@@ -55,14 +55,17 @@
     def create(self, app_name: str, app_route_name: typing.Optional[str] = None) -> App:
         resp = self.api.create_app(name=app_name, route_name=app_route_name)
         return App.from_proto(resp)
 
     def pause(self, app_name: str):
         self.api.pause_app(name=app_name)
 
+    def resume(self, app_name: str):
+        self.api.resume_app(name=app_name)
+
     def prepare_secrets(self, app: App, runtime: AppRuntime):
         prepared_secrets: typing.Dict[str, Secret] = {}
         for name in app.secret_requests:
             secret = self.secret_manager.get(name=name)
             prepared_secrets[secret.name] = secret
         runtime.secrets = prepared_secrets
 
@@ -264,20 +267,20 @@
     def setup_autoscaling_policy(self, app_name: str, autoscaling_policy: typing.Optional[AutoScalingPolicy]):
         ...
 
     def deploy(self, app: typing.Optional[App]):
         app = app or must_find_target(target_type=App)
 
         try:
-            self.api.get_app(app.name)
+            v1app = self.api.get_app(app.name)
         except ApiException as e:
-            if e.status == 404:
-                self.api.create_app(app.name)
-            else:
-                raise e
+            raise e
+
+        if v1app.status != V1AppStatus.STATUS_INIT:
+            raise ValueError(f'app only cloud be deploy once, current status is {v1app.status.value}')
 
         missed = []
         if app.resource_requests is None:
             missed.append("resource_requests")
         if app.image is None:
             missed.append("image")
```

## everai/app/context.py

```diff
@@ -5,14 +5,15 @@
 from contextvars import ContextVar
 
 from everai.configmap import ConfigMap
 from everai.secret import Secret
 from contextlib import contextmanager
 from typing import Optional
 from everai.volume import Volume, VolumeManager
+import everai.constants
 
 
 class Context:
     secrets: typing.Dict[str, Secret]
     configmaps: typing.Dict[str, ConfigMap]
     volumes: typing.Dict[str, Volume]
     _volume_manager: VolumeManager
@@ -64,14 +65,18 @@
     def volume_manager(self) -> VolumeManager:
         return self._volume_manager
 
     @property
     def is_prepare_mode(self) -> bool:
         return self._is_prepare_mode
 
+    @property
+    def is_in_cloud(self) -> bool:
+        return everai.constants.EVERAI_IN_CLOUD == '1'
+
 
 @contextmanager
 def service_context(ctx: Context):
     a = _everai_context.set(ctx)
     yield ctx
     _everai_context.reset(a)
```

## everai/queue/queued_request.py

```diff
@@ -1,14 +1,16 @@
 from __future__ import annotations
 from datetime import datetime
 import typing
 
 from everai.utils.datetime import format_datetime
 from everai.utils.show_mixin import ShowMixin, TableField
-from generated.schedulers import ListRequestQueuesResponseRequestQueue, ListRequestQueuesResponseQueueReason
+from generated.apps import (
+    V1ListRequestQueuesResponseRequestQueue, ListRequestQueuesResponseQueueReason
+)
 
 
 class QueuedRequest(ShowMixin):
     queue_index: typing.Optional[int]
     create_at: typing.Optional[datetime]
     queue_reason: typing.Optional[ListRequestQueuesResponseQueueReason]
 
@@ -23,15 +25,15 @@
                  create_at: typing.Optional[datetime],
                  queue_reason: typing.Optional[ListRequestQueuesResponseQueueReason]):
         self.queue_index = queue_index
         self.create_at = create_at
         self.queue_reason = queue_reason
 
     @staticmethod
-    def from_proto(queue: ListRequestQueuesResponseRequestQueue) -> QueuedRequest:
+    def from_proto(queue: V1ListRequestQueuesResponseRequestQueue) -> QueuedRequest:
         return QueuedRequest(
             queue_index=queue.index,
             create_at=queue.create_at,
             queue_reason=queue.reason,
         )
 
     def to_dict(self):
```

## everai/worker/worker.py

```diff
@@ -1,21 +1,21 @@
 from __future__ import annotations
 
 import typing
 from datetime import datetime
 
 from everai.utils.datetime import format_datetime
 from everai.utils.show_mixin import ShowMixin, TableField
-from generated.schedulers import Appsv1Worker, V1WorkerWorkerStatus
+from generated.apps import V1Worker, WorkerWorkerStatus
 
 
 class Worker(ShowMixin):
     worker_id: str
     device_id: str
-    status: V1WorkerWorkerStatus
+    status: WorkerWorkerStatus
     detail_status: str
     created_at: datetime
     last_serve_at: datetime
     deleted_at: typing.Optional[datetime]
     failed_count: int
     success_count: int
 
@@ -30,15 +30,15 @@
     wide_table_extra_fields: typing.List[TableField] = [
         TableField('device_id', "DEVICE"),
         TableField('last_serve_at', formatter=lambda dt: format_datetime(dt) if dt else ''),
         TableField('success_count'),
         TableField('failed_count'),
     ]
 
-    def __init__(self, worker_id: str, device_id: str, status: V1WorkerWorkerStatus,
+    def __init__(self, worker_id: str, device_id: str, status: WorkerWorkerStatus,
                  detail_status: str,
                  created_at: datetime,
                  last_serve_at: datetime,
                  success_count: int = 0,
                  failed_count: int = 0,
                  deleted_at: typing.Optional[datetime] = None,
                  ):
@@ -49,29 +49,29 @@
         self.created_at = created_at
         self.deleted_at = deleted_at
         self.last_serve_at = last_serve_at
         self.success_count = success_count
         self.failed_count = failed_count
 
     @staticmethod
-    def from_proto(worker: Appsv1Worker) -> Worker:
+    def from_proto(worker: V1Worker) -> Worker:
         return Worker(
             worker_id=worker.id,
             device_id=worker.device_id,
             status=worker.status,
             detail_status=worker.detail_status,
             created_at=worker.created_at,
             deleted_at=worker.deleted_at,
             last_serve_at=worker.last_serve_at,
             success_count=worker.success_count,
             failed_count=worker.failed_count,
         )
 
-    def to_proto(self) -> Appsv1Worker:
-        return Appsv1Worker(
+    def to_proto(self) -> V1Worker:
+        return V1Worker(
             id=self.worker_id,
             device_id=self.device_id,
             status=self.status,
             detail_status=self.detail_status,
             created_at=self.created_at,
             deleted_at=self.deleted_at,
             last_serve_at=self.last_serve_at,
```

## generated/configmaps/test/test_configmap_service_api.py

```diff
@@ -50,10 +50,17 @@
     def test_list_configmaps(self) -> None:
         """Test case for list_configmaps
 
         List configmaps  # noqa: E501
         """
         pass
 
+    def test_update_configmap(self) -> None:
+        """Test case for update_configmap
+
+        Update configmap  # noqa: E501
+        """
+        pass
+
 
 if __name__ == '__main__':
     unittest.main()
```

## generated/secrets/test/test_secret_service_api.py

```diff
@@ -50,10 +50,17 @@
     def test_list_secret(self) -> None:
         """Test case for list_secret
 
         List secret  # noqa: E501
         """
         pass
 
+    def test_update_secret(self) -> None:
+        """Test case for update_secret
+
+        Update secret  # noqa: E501
+        """
+        pass
+
 
 if __name__ == '__main__':
     unittest.main()
```

## generated/secrets/test/test_secret_service_create_body.py

```diff
@@ -32,22 +32,26 @@
             params are included, when True both required and
             optional params are included """
         # uncomment below to create an instance of `SecretServiceCreateBody`
         """
         model = SecretServiceCreateBody()  # noqa: E501
         if include_optional:
             return SecretServiceCreateBody(
-                value = '',
+                data = {
+                    'key' : ''
+                    },
                 labels = {
                     'key' : ''
                     }
             )
         else:
             return SecretServiceCreateBody(
-                value = '',
+                data = {
+                    'key' : ''
+                    },
         )
         """
 
     def testSecretServiceCreateBody(self):
         """Test SecretServiceCreateBody"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
```

## generated/secrets/test/test_v1_list_response.py

```diff
@@ -35,15 +35,17 @@
         """
         model = V1ListResponse()  # noqa: E501
         if include_optional:
             return V1ListResponse(
                 secrets = [
                     generated.secrets.models.v1_secret.v1Secret(
                         name = '', 
-                        value = '', 
+                        data = {
+                            'key' : ''
+                            }, 
                         create_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         labels = {
                             'key' : ''
                             }, )
                     ]
             )
         else:
```

## generated/secrets/test/test_v1_secret.py

```diff
@@ -33,22 +33,27 @@
             optional params are included """
         # uncomment below to create an instance of `V1Secret`
         """
         model = V1Secret()  # noqa: E501
         if include_optional:
             return V1Secret(
                 name = '',
-                value = '',
+                data = {
+                    'key' : ''
+                    },
                 create_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
                 labels = {
                     'key' : ''
                     }
             )
         else:
             return V1Secret(
+                data = {
+                    'key' : ''
+                    },
         )
         """
 
     def testV1Secret(self):
         """Test V1Secret"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
```

## generated/volumes/test/test_v1_list_response.py

```diff
@@ -43,15 +43,17 @@
                         revision = '', 
                         created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         modified_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         labels = {
                             'key' : ''
                             }, 
                         size = '', 
-                        files = '', )
+                        files = '', 
+                        status = 'Unspecified', 
+                        username = '', )
                     ]
             )
         else:
             return V1ListResponse(
         )
         """
```

## generated/volumes/test/test_v1_volume.py

```diff
@@ -41,15 +41,17 @@
                 revision = '',
                 created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
                 modified_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
                 labels = {
                     'key' : ''
                     },
                 size = '',
-                files = ''
+                files = '',
+                status = 'Unspecified',
+                username = ''
             )
         else:
             return V1Volume(
         )
         """
 
     def testV1Volume(self):
```

## generated/volumes/test/test_volume_service_api.py

```diff
@@ -92,49 +92,77 @@
     def test_get_volume(self) -> None:
         """Test case for get_volume
 
         Get a volume metadata  # noqa: E501
         """
         pass
 
+    def test_get_volume_0(self) -> None:
+        """Test case for get_volume_0
+
+        Get a volume metadata  # noqa: E501
+        """
+        pass
+
     def test_initialize_multipart_upload(self) -> None:
         """Test case for initialize_multipart_upload
 
         Initialize a multipart upload  # noqa: E501
         """
         pass
 
     def test_list_files(self) -> None:
         """Test case for list_files
 
         List files in a persistence volume of current revision  # noqa: E501
         """
         pass
 
+    def test_list_files_0(self) -> None:
+        """Test case for list_files_0
+
+        List files in a persistence volume of current revision  # noqa: E501
+        """
+        pass
+
     def test_list_parts(self) -> None:
         """Test case for list_parts
 
         List part of incomplete multipart upload  # noqa: E501
         """
         pass
 
     def test_list_volume(self) -> None:
         """Test case for list_volume
 
         List volume metadata  # noqa: E501
         """
         pass
 
+    def test_publish_volume(self) -> None:
+        """Test case for publish_volume
+
+        Publish volume  # noqa: E501
+        """
+        pass
+
     def test_sign_download(self) -> None:
         """Test case for sign_download
 
         Sign for download of a file  # noqa: E501
         """
         pass
 
+    def test_sign_download_0(self) -> None:
+        """Test case for sign_download_0
+
+        Sign for download of a file  # noqa: E501
+        """
+        pass
+
     def test_sign_multipart_upload(self) -> None:
         """Test case for sign_multipart_upload
 
         Sign a part of multipart upload  # noqa: E501
         """
         pass
```

## Comparing `generated/schedulers/api_client.py` & `generated/apps/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/comm/v1/messages.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
@@ -20,19 +20,19 @@
 from multiprocessing.pool import ThreadPool
 import os
 import re
 import tempfile
 
 from urllib.parse import quote
 
-from generated.schedulers.configuration import Configuration
-from generated.schedulers.api_response import ApiResponse
-import generated.schedulers.models
-from generated.schedulers import rest
-from generated.schedulers.exceptions import ApiValueError, ApiException
+from generated.apps.configuration import Configuration
+from generated.apps.api_response import ApiResponse
+import generated.apps.models
+from generated.apps import rest
+from generated.apps.exceptions import ApiValueError, ApiException
 
 
 class ApiClient:
     """Generic API client for OpenAPI client library builds.
 
     OpenAPI generic API client. This client handles the client-
     server communication, and is invariant across implementations. Specifics of
@@ -340,15 +340,15 @@
                 return {k: self.__deserialize(v, sub_kls)
                         for k, v in data.items()}
 
             # convert str to class
             if klass in self.NATIVE_TYPES_MAPPING:
                 klass = self.NATIVE_TYPES_MAPPING[klass]
             else:
-                klass = getattr(generated.schedulers.models, klass)
+                klass = getattr(generated.apps.models, klass)
 
         if klass in self.PRIMITIVE_TYPES:
             return self.__deserialize_primitive(data, klass)
         elif klass == object:
             return self.__deserialize_object(data)
         elif klass == datetime.date:
             return self.__deserialize_date(data)
```

## Comparing `generated/schedulers/api_response.py` & `generated/apps/api_response.py`

 * *Files identical despite different names*

## Comparing `generated/schedulers/configuration.py` & `generated/apps/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/comm/v1/messages.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
@@ -103,15 +103,15 @@
         """
         self.access_token = access_token
         """Access token
         """
         self.logger = {}
         """Logging Settings
         """
-        self.logger["package_logger"] = logging.getLogger("generated.schedulers")
+        self.logger["package_logger"] = logging.getLogger("generated.apps")
         self.logger["urllib3_logger"] = logging.getLogger("urllib3")
         self.logger_format = '%(asctime)s %(levelname)s %(message)s'
         """Log format
         """
         self.logger_stream_handler = None
         """Log stream handler
         """
```

## Comparing `generated/schedulers/exceptions.py` & `generated/apps/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/comm/v1/messages.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
```

## Comparing `generated/schedulers/rest.py` & `generated/apps/rest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/comm/v1/messages.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
@@ -17,15 +17,15 @@
 import logging
 import re
 import ssl
 
 from urllib.parse import urlencode, quote_plus
 import urllib3
 
-from generated.schedulers.exceptions import ApiException, UnauthorizedException, ForbiddenException, NotFoundException, ServiceException, ApiValueError, BadRequestException
+from generated.apps.exceptions import ApiException, UnauthorizedException, ForbiddenException, NotFoundException, ServiceException, ApiValueError, BadRequestException
 
 
 logger = logging.getLogger(__name__)
 
 
 class RESTResponse(io.IOBase):
```

## Comparing `generated/schedulers/api/app_service_api.py` & `generated/apps/api/app_service_api.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/comm/v1/messages.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
@@ -21,28 +21,29 @@
 
 from pydantic import Field
 from typing_extensions import Annotated
 from pydantic import StrictBool, StrictInt, StrictStr
 
 from typing import Any, Dict, Optional, Union
 
-from generated.schedulers.models.app_service_create_body import AppServiceCreateBody
-from generated.schedulers.models.app_service_setup_auto_scaling_policy_body import AppServiceSetupAutoScalingPolicyBody
-from generated.schedulers.models.app_service_setup_resources_body import AppServiceSetupResourcesBody
-from generated.schedulers.models.app_service_setup_secrets_body import AppServiceSetupSecretsBody
-from generated.schedulers.models.app_service_setup_volumes_body import AppServiceSetupVolumesBody
-from generated.schedulers.models.v1_app import V1App
-from generated.schedulers.models.v1_app_service_setup_image_body import V1AppServiceSetupImageBody
-from generated.schedulers.models.v1_list_request_queues_response import V1ListRequestQueuesResponse
-from generated.schedulers.models.v1_list_response import V1ListResponse
-from generated.schedulers.models.v1_list_workers_response import V1ListWorkersResponse
-
-from generated.schedulers.api_client import ApiClient
-from generated.schedulers.api_response import ApiResponse
-from generated.schedulers.exceptions import (  # noqa: F401
+from generated.apps.models.app_service_create_body import AppServiceCreateBody
+from generated.apps.models.app_service_protect_app_body import AppServiceProtectAppBody
+from generated.apps.models.app_service_setup_auto_scaling_policy_body import AppServiceSetupAutoScalingPolicyBody
+from generated.apps.models.app_service_setup_resources_body import AppServiceSetupResourcesBody
+from generated.apps.models.app_service_setup_secrets_body import AppServiceSetupSecretsBody
+from generated.apps.models.app_service_setup_volumes_body import AppServiceSetupVolumesBody
+from generated.apps.models.v1_app import V1App
+from generated.apps.models.v1_app_service_setup_image_body import V1AppServiceSetupImageBody
+from generated.apps.models.v1_list_request_queues_response import V1ListRequestQueuesResponse
+from generated.apps.models.v1_list_response import V1ListResponse
+from generated.apps.models.v1_list_workers_response import V1ListWorkersResponse
+
+from generated.apps.api_client import ApiClient
+from generated.apps.api_response import ApiResponse
+from generated.apps.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
 class AppServiceApi:
     """NOTE: This class is auto generated by OpenAPI Generator
@@ -1265,14 +1266,628 @@
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    def private_app(
+        self,
+        app_name: Annotated[StrictStr, Field(description="app name")],
+        **kwargs,
+    ) -> object:
+        """Private app  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.private_app(app_name, async_req=True)
+        >>> result = thread.get()
+
+        :param app_name: app name (required)
+        :type app_name: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _request_timeout: timeout setting for this request.
+               If one number provided, it will be total request
+               timeout. It can also be a pair (tuple) of
+               (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: object
+        """
+        kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            message = "Error! Please call the private_app_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
+            raise ValueError(message)
+
+        return self.private_app_with_http_info(
+            app_name,
+            **kwargs,
+        )
+
+    @validate_call
+    def private_app_with_http_info(
+        self,
+        app_name: Annotated[StrictStr, Field(description="app name")],
+        **kwargs,
+    ) -> ApiResponse:
+        """Private app  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.private_app_with_http_info(app_name, async_req=True)
+        >>> result = thread.get()
+
+        :param app_name: app name (required)
+        :type app_name: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
+        :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(object, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'app_name'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method private_app" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats: Dict[str, str] = {}
+
+        # process the path parameters
+        _path_params: Dict[str, str] = {}
+        if _params['app_name'] is not None:
+            _path_params['appName'] = _params['app_name']
+
+
+        # process the query parameters
+        _query_params: List[Tuple[str, str]] = []
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+        # process the form parameters
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, str] = {}
+        # process the body parameter
+        _body_params = None
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # authentication setting
+        _auth_settings: List[str] = []  # noqa: E501
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "object",
+        }
+
+        return self.api_client.call_api(
+            '/api/apps/v1/{appName}/private', 'POST',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    def protect_app(
+        self,
+        app_name: Annotated[StrictStr, Field(description="app name")],
+        body: AppServiceProtectAppBody,
+        **kwargs,
+    ) -> object:
+        """Protect app  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.protect_app(app_name, body, async_req=True)
+        >>> result = thread.get()
+
+        :param app_name: app name (required)
+        :type app_name: str
+        :param body: (required)
+        :type body: AppServiceProtectAppBody
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _request_timeout: timeout setting for this request.
+               If one number provided, it will be total request
+               timeout. It can also be a pair (tuple) of
+               (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: object
+        """
+        kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            message = "Error! Please call the protect_app_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
+            raise ValueError(message)
+
+        return self.protect_app_with_http_info(
+            app_name,
+            body,
+            **kwargs,
+        )
+
+    @validate_call
+    def protect_app_with_http_info(
+        self,
+        app_name: Annotated[StrictStr, Field(description="app name")],
+        body: AppServiceProtectAppBody,
+        **kwargs,
+    ) -> ApiResponse:
+        """Protect app  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.protect_app_with_http_info(app_name, body, async_req=True)
+        >>> result = thread.get()
+
+        :param app_name: app name (required)
+        :type app_name: str
+        :param body: (required)
+        :type body: AppServiceProtectAppBody
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
+        :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(object, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'app_name',
+            'body'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method protect_app" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats: Dict[str, str] = {}
+
+        # process the path parameters
+        _path_params: Dict[str, str] = {}
+        if _params['app_name'] is not None:
+            _path_params['appName'] = _params['app_name']
+
+
+        # process the query parameters
+        _query_params: List[Tuple[str, str]] = []
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+        # process the form parameters
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, str] = {}
+        # process the body parameter
+        _body_params = None
+        if _params['body'] is not None:
+            _body_params = _params['body']
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # set the HTTP header `Content-Type`
+        _content_types_list = _params.get('_content_type',
+            self.api_client.select_header_content_type(
+                ['application/json']))
+        if _content_types_list:
+                _header_params['Content-Type'] = _content_types_list
+
+        # authentication setting
+        _auth_settings: List[str] = []  # noqa: E501
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "object",
+        }
+
+        return self.api_client.call_api(
+            '/api/apps/v1/{appName}/protect', 'POST',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    def publish_app(
+        self,
+        app_name: Annotated[StrictStr, Field(description="app name")],
+        **kwargs,
+    ) -> object:
+        """Publish app  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.publish_app(app_name, async_req=True)
+        >>> result = thread.get()
+
+        :param app_name: app name (required)
+        :type app_name: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _request_timeout: timeout setting for this request.
+               If one number provided, it will be total request
+               timeout. It can also be a pair (tuple) of
+               (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: object
+        """
+        kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            message = "Error! Please call the publish_app_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
+            raise ValueError(message)
+
+        return self.publish_app_with_http_info(
+            app_name,
+            **kwargs,
+        )
+
+    @validate_call
+    def publish_app_with_http_info(
+        self,
+        app_name: Annotated[StrictStr, Field(description="app name")],
+        **kwargs,
+    ) -> ApiResponse:
+        """Publish app  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.publish_app_with_http_info(app_name, async_req=True)
+        >>> result = thread.get()
+
+        :param app_name: app name (required)
+        :type app_name: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
+        :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(object, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'app_name'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method publish_app" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats: Dict[str, str] = {}
+
+        # process the path parameters
+        _path_params: Dict[str, str] = {}
+        if _params['app_name'] is not None:
+            _path_params['appName'] = _params['app_name']
+
+
+        # process the query parameters
+        _query_params: List[Tuple[str, str]] = []
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+        # process the form parameters
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, str] = {}
+        # process the body parameter
+        _body_params = None
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # authentication setting
+        _auth_settings: List[str] = []  # noqa: E501
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "object",
+        }
+
+        return self.api_client.call_api(
+            '/api/apps/v1/{appName}/publish', 'POST',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    def resume_app(
+        self,
+        app_name: StrictStr,
+        **kwargs,
+    ) -> object:
+        """Resume the app  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.resume_app(app_name, async_req=True)
+        >>> result = thread.get()
+
+        :param app_name: (required)
+        :type app_name: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _request_timeout: timeout setting for this request.
+               If one number provided, it will be total request
+               timeout. It can also be a pair (tuple) of
+               (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: object
+        """
+        kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            message = "Error! Please call the resume_app_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
+            raise ValueError(message)
+
+        return self.resume_app_with_http_info(
+            app_name,
+            **kwargs,
+        )
+
+    @validate_call
+    def resume_app_with_http_info(
+        self,
+        app_name: StrictStr,
+        **kwargs,
+    ) -> ApiResponse:
+        """Resume the app  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.resume_app_with_http_info(app_name, async_req=True)
+        >>> result = thread.get()
+
+        :param app_name: (required)
+        :type app_name: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
+        :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(object, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'app_name'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method resume_app" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats: Dict[str, str] = {}
+
+        # process the path parameters
+        _path_params: Dict[str, str] = {}
+        if _params['app_name'] is not None:
+            _path_params['appName'] = _params['app_name']
+
+
+        # process the query parameters
+        _query_params: List[Tuple[str, str]] = []
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+        # process the form parameters
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, str] = {}
+        # process the body parameter
+        _body_params = None
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # authentication setting
+        _auth_settings: List[str] = []  # noqa: E501
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "object",
+        }
+
+        return self.api_client.call_api(
+            '/api/apps/v1/{appName}/resume', 'POST',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
             auth_settings=_auth_settings,
             async_req=_params.get('async_req'),
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
```

## Comparing `generated/schedulers/models/app_service_create_body.py` & `generated/apps/models/app_service_create_body.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/comm/v1/messages.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
```

## Comparing `generated/schedulers/models/app_service_inference_body.py` & `generated/apps/models/app_runtimev1_request_queue.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/comm/v1/messages.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
@@ -14,43 +14,30 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional, Union
-from pydantic import BaseModel, StrictInt, StrictStr, field_validator
+from typing import Optional
+from pydantic import BaseModel, StrictInt, StrictStr
 from pydantic import Field
-from typing_extensions import Annotated
 from typing import Dict, Any
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class AppServiceInferenceBody(BaseModel):
+class AppRuntimev1RequestQueue(BaseModel):
     """
-    AppServiceInferenceBody
+    AppRuntimev1RequestQueue
     """
-    method: Optional[StrictStr] = None
-    body: Optional[Union[Annotated[bytes, Field(strict=True)], Annotated[str, Field(strict=True)]]] = None
-    timeout_time: StrictInt = Field(alias="timeoutTime")
-    max_retry_times: StrictInt = Field(alias="maxRetryTimes")
-    __properties: ClassVar[List[str]] = ["method", "body", "timeoutTime", "maxRetryTimes"]
-
-    @field_validator('body')
-    def body_validate_regular_expression(cls, value):
-        """Validates the regular expression"""
-        if value is None:
-            return value
-
-        if not re.match(r"^(?:[A-Za-z0-9+\/]{4})*(?:[A-Za-z0-9+\/]{2}==|[A-Za-z0-9+\/]{3}=)?$", value):
-            raise ValueError(r"must validate the regular expression /^(?:[A-Za-z0-9+\/]{4})*(?:[A-Za-z0-9+\/]{2}==|[A-Za-z0-9+\/]{3}=)?$/")
-        return value
+    size: Optional[StrictInt] = None
+    q_name: Optional[StrictStr] = Field(default=None, alias="qName")
+    __properties: ClassVar[List[str]] = ["size", "qName"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True
     }
 
 
@@ -61,15 +48,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of AppServiceInferenceBody from a JSON string"""
+        """Create an instance of AppRuntimev1RequestQueue from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -84,23 +71,21 @@
             },
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> Self:
-        """Create an instance of AppServiceInferenceBody from a dict"""
+        """Create an instance of AppRuntimev1RequestQueue from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "method": obj.get("method"),
-            "body": obj.get("body"),
-            "timeoutTime": obj.get("timeoutTime"),
-            "maxRetryTimes": obj.get("maxRetryTimes")
+            "size": obj.get("size"),
+            "qName": obj.get("qName")
         })
         return _obj
```

## Comparing `generated/schedulers/models/app_service_resources_body.py` & `generated/apps/models/app_service_setup_resources_body.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/register_message.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
@@ -13,79 +13,81 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, Field
-from typing import Any, ClassVar, Dict, List
-from generated.schedulers.models.v1_resource_claim import V1ResourceClaim
-from typing import Optional, Set
-from typing_extensions import Self
 
-class AppServiceResourcesBody(BaseModel):
+
+from pydantic import BaseModel
+from pydantic import Field
+from generated.apps.models.v1_resource_claim import V1ResourceClaim
+from typing import Dict, Any
+try:
+    from typing import Self
+except ImportError:
+    from typing_extensions import Self
+
+class AppServiceSetupResourcesBody(BaseModel):
+    """
+    AppServiceSetupResourcesBody
     """
-    AppServiceResourcesBody
-    """ # noqa: E501
     resource_claim: V1ResourceClaim = Field(alias="resourceClaim")
     __properties: ClassVar[List[str]] = ["resourceClaim"]
 
-    model_config = ConfigDict(
-        populate_by_name=True,
-        validate_assignment=True,
-        protected_namespaces=(),
-    )
+    model_config = {
+        "populate_by_name": True,
+        "validate_assignment": True
+    }
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of AppServiceResourcesBody from a JSON string"""
+    def from_json(cls, json_str: str) -> Self:
+        """Create an instance of AppServiceSetupResourcesBody from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
         """
-        excluded_fields: Set[str] = set([
-        ])
-
         _dict = self.model_dump(
             by_alias=True,
-            exclude=excluded_fields,
+            exclude={
+            },
             exclude_none=True,
         )
         # override the default output from pydantic by calling `to_dict()` of resource_claim
         if self.resource_claim:
             _dict['resourceClaim'] = self.resource_claim.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of AppServiceResourcesBody from a dict"""
+    def from_dict(cls, obj: dict) -> Self:
+        """Create an instance of AppServiceSetupResourcesBody from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "resourceClaim": V1ResourceClaim.from_dict(obj["resourceClaim"]) if obj.get("resourceClaim") is not None else None
+            "resourceClaim": V1ResourceClaim.from_dict(obj.get("resourceClaim")) if obj.get("resourceClaim") is not None else None
         })
         return _obj
```

## Comparing `generated/schedulers/models/app_service_setup_auto_scaling_policy_body.py` & `generated/apps/models/app_service_setup_auto_scaling_policy_body.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/comm/v1/messages.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
@@ -17,15 +17,15 @@
 import re  # noqa: F401
 import json
 
 
 
 from pydantic import BaseModel
 from pydantic import Field
-from generated.schedulers.models.v1_autoscaling_policy import V1AutoscalingPolicy
+from generated.apps.models.v1_autoscaling_policy import V1AutoscalingPolicy
 from typing import Dict, Any
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
 class AppServiceSetupAutoScalingPolicyBody(BaseModel):
```

## Comparing `generated/schedulers/models/app_service_setup_body.py` & `generated/apps/models/v1_get_route_path_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/register_message.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
@@ -14,29 +14,28 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-
-from pydantic import BaseModel
-from generated.schedulers.models.v1_setting import V1Setting
+from typing import List, Optional
+from pydantic import BaseModel, StrictStr
 from typing import Dict, Any
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class AppServiceSetupBody(BaseModel):
+class V1GetRoutePathResponse(BaseModel):
     """
-    AppServiceSetupBody
+    V1GetRoutePathResponse
     """
-    settings: V1Setting
-    __properties: ClassVar[List[str]] = ["settings"]
+    paths: Optional[List[StrictStr]] = None
+    __properties: ClassVar[List[str]] = ["paths"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True
     }
 
 
@@ -47,15 +46,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of AppServiceSetupBody from a JSON string"""
+        """Create an instance of V1GetRoutePathResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -66,27 +65,24 @@
         """
         _dict = self.model_dump(
             by_alias=True,
             exclude={
             },
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of settings
-        if self.settings:
-            _dict['settings'] = self.settings.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> Self:
-        """Create an instance of AppServiceSetupBody from a dict"""
+        """Create an instance of V1GetRoutePathResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "settings": V1Setting.from_dict(obj.get("settings")) if obj.get("settings") is not None else None
+            "paths": obj.get("paths")
         })
         return _obj
```

## Comparing `generated/schedulers/models/app_service_setup_resource_body.py` & `generated/apps/models/v1_list_all_workers_response.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/register_message.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
@@ -13,79 +13,84 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, Field
-from typing import Any, ClassVar, Dict, List
-from generated.schedulers.models.v1_resource_claim import V1ResourceClaim
-from typing import Optional, Set
-from typing_extensions import Self
 
-class AppServiceSetupResourceBody(BaseModel):
+from typing import List, Optional
+from pydantic import BaseModel
+from generated.apps.models.v1_worker import V1Worker
+from typing import Dict, Any
+try:
+    from typing import Self
+except ImportError:
+    from typing_extensions import Self
+
+class V1ListAllWorkersResponse(BaseModel):
+    """
+    V1ListAllWorkersResponse
     """
-    AppServiceSetupResourceBody
-    """ # noqa: E501
-    resource_claim: V1ResourceClaim = Field(alias="resourceClaim")
-    __properties: ClassVar[List[str]] = ["resourceClaim"]
-
-    model_config = ConfigDict(
-        populate_by_name=True,
-        validate_assignment=True,
-        protected_namespaces=(),
-    )
+    workers: Optional[List[V1Worker]] = None
+    __properties: ClassVar[List[str]] = ["workers"]
+
+    model_config = {
+        "populate_by_name": True,
+        "validate_assignment": True
+    }
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of AppServiceSetupResourceBody from a JSON string"""
+    def from_json(cls, json_str: str) -> Self:
+        """Create an instance of V1ListAllWorkersResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
         """
-        excluded_fields: Set[str] = set([
-        ])
-
         _dict = self.model_dump(
             by_alias=True,
-            exclude=excluded_fields,
+            exclude={
+            },
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of resource_claim
-        if self.resource_claim:
-            _dict['resourceClaim'] = self.resource_claim.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of each item in workers (list)
+        _items = []
+        if self.workers:
+            for _item in self.workers:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['workers'] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of AppServiceSetupResourceBody from a dict"""
+    def from_dict(cls, obj: dict) -> Self:
+        """Create an instance of V1ListAllWorkersResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "resourceClaim": V1ResourceClaim.from_dict(obj["resourceClaim"]) if obj.get("resourceClaim") is not None else None
+            "workers": [V1Worker.from_dict(_item) for _item in obj.get("workers")] if obj.get("workers") is not None else None
         })
         return _obj
```

## Comparing `generated/schedulers/models/app_service_setup_resources_body.py` & `generated/apps/models/v1_value_from_secret.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/comm/v1/messages.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
@@ -14,30 +14,29 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-
-from pydantic import BaseModel
-from pydantic import Field
-from generated.schedulers.models.v1_resource_claim import V1ResourceClaim
+from typing import Optional
+from pydantic import BaseModel, StrictStr
 from typing import Dict, Any
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class AppServiceSetupResourcesBody(BaseModel):
+class V1ValueFromSecret(BaseModel):
     """
-    AppServiceSetupResourcesBody
+    V1ValueFromSecret
     """
-    resource_claim: V1ResourceClaim = Field(alias="resourceClaim")
-    __properties: ClassVar[List[str]] = ["resourceClaim"]
+    name: Optional[StrictStr] = None
+    key: Optional[StrictStr] = None
+    __properties: ClassVar[List[str]] = ["name", "key"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True
     }
 
 
@@ -48,15 +47,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of AppServiceSetupResourcesBody from a JSON string"""
+        """Create an instance of V1ValueFromSecret from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -67,27 +66,25 @@
         """
         _dict = self.model_dump(
             by_alias=True,
             exclude={
             },
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of resource_claim
-        if self.resource_claim:
-            _dict['resourceClaim'] = self.resource_claim.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> Self:
-        """Create an instance of AppServiceSetupResourcesBody from a dict"""
+        """Create an instance of V1ValueFromSecret from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "resourceClaim": V1ResourceClaim.from_dict(obj.get("resourceClaim")) if obj.get("resourceClaim") is not None else None
+            "name": obj.get("name"),
+            "key": obj.get("key")
         })
         return _obj
```

## Comparing `generated/schedulers/models/app_service_setup_secrets_body.py` & `generated/apps/models/app_service_setup_secrets_body.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/comm/v1/messages.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
```

## Comparing `generated/schedulers/models/app_service_setup_volumes_body.py` & `generated/apps/models/app_service_setup_volumes_body.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/comm/v1/messages.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
@@ -17,15 +17,15 @@
 import re  # noqa: F401
 import json
 
 
 from typing import List
 from pydantic import BaseModel
 from pydantic import Field
-from generated.schedulers.models.v1_setup_volume import V1SetupVolume
+from generated.apps.models.v1_setup_volume import V1SetupVolume
 from typing import Dict, Any
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
 class AppServiceSetupVolumesBody(BaseModel):
```

## Comparing `generated/schedulers/models/appsv1_cpu.py` & `generated/apps/models/v1_scale_record.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/register_message.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
@@ -15,28 +15,29 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, StrictInt, StrictStr
+from pydantic import BaseModel, StrictStr
+from generated.apps.models.scale_record_autoscaling_action import ScaleRecordAutoscalingAction
 from typing import Dict, Any
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class Appsv1CPU(BaseModel):
+class V1ScaleRecord(BaseModel):
     """
-    Appsv1CPU
+    V1ScaleRecord
     """
-    cores: Optional[StrictInt] = None
-    architecture: Optional[StrictStr] = None
-    __properties: ClassVar[List[str]] = ["cores", "architecture"]
+    action: Optional[ScaleRecordAutoscalingAction] = None
+    message: Optional[StrictStr] = None
+    __properties: ClassVar[List[str]] = ["action", "message"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True
     }
 
 
@@ -47,15 +48,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of Appsv1CPU from a JSON string"""
+        """Create an instance of V1ScaleRecord from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -70,21 +71,21 @@
             },
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> Self:
-        """Create an instance of Appsv1CPU from a dict"""
+        """Create an instance of V1ScaleRecord from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "cores": obj.get("cores"),
-            "architecture": obj.get("architecture")
+            "action": obj.get("action"),
+            "message": obj.get("message")
         })
         return _obj
```

## Comparing `generated/schedulers/models/appsv1_gpu.py` & `generated/apps/models/v1_list_all_apps_response.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/register_message.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
@@ -14,32 +14,29 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
-from pydantic import BaseModel, StrictStr
-from pydantic import Field
+from typing import List, Optional
+from pydantic import BaseModel
+from generated.apps.models.v1_app import V1App
 from typing import Dict, Any
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class Appsv1GPU(BaseModel):
+class V1ListAllAppsResponse(BaseModel):
     """
-    Appsv1GPU
+    V1ListAllAppsResponse
     """
-    model: StrictStr
-    number: Optional[StrictStr] = None
-    required_driver_version: Optional[StrictStr] = Field(default=None, alias="requiredDriverVersion")
-    required_cuda_version: Optional[StrictStr] = Field(default=None, alias="requiredCUDAVersion")
-    __properties: ClassVar[List[str]] = ["model", "number", "requiredDriverVersion", "requiredCUDAVersion"]
+    apps: Optional[List[V1App]] = None
+    __properties: ClassVar[List[str]] = ["apps"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True
     }
 
 
@@ -50,15 +47,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of Appsv1GPU from a JSON string"""
+        """Create an instance of V1ListAllAppsResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -69,27 +66,31 @@
         """
         _dict = self.model_dump(
             by_alias=True,
             exclude={
             },
             exclude_none=True,
         )
+        # override the default output from pydantic by calling `to_dict()` of each item in apps (list)
+        _items = []
+        if self.apps:
+            for _item in self.apps:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['apps'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> Self:
-        """Create an instance of Appsv1GPU from a dict"""
+        """Create an instance of V1ListAllAppsResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "model": obj.get("model"),
-            "number": obj.get("number"),
-            "requiredDriverVersion": obj.get("requiredDriverVersion"),
-            "requiredCUDAVersion": obj.get("requiredCUDAVersion")
+            "apps": [V1App.from_dict(_item) for _item in obj.get("apps")] if obj.get("apps") is not None else None
         })
         return _obj
```

## Comparing `generated/schedulers/models/appsv1_setup_image.py` & `generated/apps/models/appsv1_setup_image.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/comm/v1/messages.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
@@ -17,15 +17,15 @@
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel, StrictStr
 from pydantic import Field
-from generated.schedulers.models.v1_basic_auth import V1BasicAuth
+from generated.apps.models.v1_basic_auth import V1BasicAuth
 from typing import Dict, Any
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
 class Appsv1SetupImage(BaseModel):
```

## Comparing `generated/schedulers/models/appsv1_worker.py` & `generated/apps/models/v1_app.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/comm/v1/messages.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
@@ -14,41 +14,46 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
-from typing import Optional
-from pydantic import BaseModel, StrictInt, StrictStr
+from typing import Dict, Optional
+from pydantic import BaseModel, StrictBool, StrictStr
 from pydantic import Field
-from generated.schedulers.models.v1_worker_worker_status import V1WorkerWorkerStatus
-from generated.schedulers.models.worker_worker_detail_status import WorkerWorkerDetailStatus
+from generated.apps.models.app_route_auth_status import AppRouteAuthStatus
+from generated.apps.models.v1_app_revision import V1AppRevision
+from generated.apps.models.v1_app_status import V1AppStatus
 from typing import Dict, Any
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class Appsv1Worker(BaseModel):
+class V1App(BaseModel):
     """
-    Appsv1Worker
+    V1App
     """
     id: Optional[StrictStr] = None
-    device_id: Optional[StrictStr] = Field(default=None, alias="deviceId")
-    status: Optional[V1WorkerWorkerStatus] = None
-    detail_status: Optional[WorkerWorkerDetailStatus] = Field(default=None, alias="detailStatus")
+    name: Optional[StrictStr] = None
+    user_id: Optional[StrictStr] = Field(default=None, alias="userId")
+    route_path: Optional[StrictStr] = Field(default=None, description="default route path is same with app_name. While app_name has conflict, route_path is required.", alias="routePath")
+    status: Optional[V1AppStatus] = None
+    error_msg: Optional[StrictStr] = Field(default=None, alias="errorMsg")
+    username: Optional[StrictStr] = None
+    route_auth_status: Optional[AppRouteAuthStatus] = Field(default=None, alias="routeAuthStatus")
+    route_public_key: Optional[StrictStr] = Field(default=None, alias="routePublicKey")
     created_at: Optional[datetime] = Field(default=None, alias="createdAt")
-    deleted_at: Optional[datetime] = Field(default=None, alias="deletedAt")
-    launch_at: Optional[datetime] = Field(default=None, alias="launchAt")
-    last_serve_at: Optional[datetime] = Field(default=None, alias="lastServeAt")
-    success_count: Optional[StrictInt] = Field(default=None, alias="successCount")
-    failed_count: Optional[StrictInt] = Field(default=None, alias="failedCount")
-    session_number: Optional[StrictInt] = Field(default=None, alias="sessionNumber")
-    __properties: ClassVar[List[str]] = ["id", "deviceId", "status", "detailStatus", "createdAt", "deletedAt", "launchAt", "lastServeAt", "successCount", "failedCount", "sessionNumber"]
+    modified_at: Optional[datetime] = Field(default=None, alias="modifiedAt")
+    labels: Optional[Dict[str, StrictStr]] = None
+    current_revision: Optional[StrictStr] = Field(default=None, alias="currentRevision")
+    revision: Optional[V1AppRevision] = None
+    deployed: Optional[StrictBool] = None
+    __properties: ClassVar[List[str]] = ["id", "name", "userId", "routePath", "status", "errorMsg", "username", "routeAuthStatus", "routePublicKey", "createdAt", "modifiedAt", "labels", "currentRevision", "revision", "deployed"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True
     }
 
 
@@ -59,53 +64,64 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of Appsv1Worker from a JSON string"""
+        """Create an instance of V1App from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
+        * OpenAPI `readOnly` fields are excluded.
+        * OpenAPI `readOnly` fields are excluded.
         """
         _dict = self.model_dump(
             by_alias=True,
             exclude={
+                "current_revision",
+                "deployed",
             },
             exclude_none=True,
         )
+        # override the default output from pydantic by calling `to_dict()` of revision
+        if self.revision:
+            _dict['revision'] = self.revision.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> Self:
-        """Create an instance of Appsv1Worker from a dict"""
+        """Create an instance of V1App from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "id": obj.get("id"),
-            "deviceId": obj.get("deviceId"),
+            "name": obj.get("name"),
+            "userId": obj.get("userId"),
+            "routePath": obj.get("routePath"),
             "status": obj.get("status"),
-            "detailStatus": obj.get("detailStatus"),
+            "errorMsg": obj.get("errorMsg"),
+            "username": obj.get("username"),
+            "routeAuthStatus": obj.get("routeAuthStatus"),
+            "routePublicKey": obj.get("routePublicKey"),
             "createdAt": obj.get("createdAt"),
-            "deletedAt": obj.get("deletedAt"),
-            "launchAt": obj.get("launchAt"),
-            "lastServeAt": obj.get("lastServeAt"),
-            "successCount": obj.get("successCount"),
-            "failedCount": obj.get("failedCount"),
-            "sessionNumber": obj.get("sessionNumber")
+            "modifiedAt": obj.get("modifiedAt"),
+            "labels": obj.get("labels"),
+            "currentRevision": obj.get("currentRevision"),
+            "revision": V1AppRevision.from_dict(obj.get("revision")) if obj.get("revision") is not None else None,
+            "deployed": obj.get("deployed")
         })
         return _obj
```

## Comparing `generated/schedulers/models/list_request_queues_response_queue_reason.py` & `generated/apps/models/list_request_queues_response_queue_reason.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/comm/v1/messages.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
```

## Comparing `generated/schedulers/models/list_request_queues_response_request_queue.py` & `generated/apps/models/v1_list_request_queues_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/comm/v1/messages.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
@@ -13,33 +13,30 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from datetime import datetime
-from typing import Optional
-from pydantic import BaseModel, StrictInt
-from pydantic import Field
-from generated.schedulers.models.list_request_queues_response_queue_reason import ListRequestQueuesResponseQueueReason
+
+from typing import List, Optional
+from pydantic import BaseModel
+from generated.apps.models.v1_list_request_queues_response_request_queue import V1ListRequestQueuesResponseRequestQueue
 from typing import Dict, Any
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class ListRequestQueuesResponseRequestQueue(BaseModel):
+class V1ListRequestQueuesResponse(BaseModel):
     """
-    ListRequestQueuesResponseRequestQueue
+    V1ListRequestQueuesResponse
     """
-    index: Optional[StrictInt] = None
-    reason: Optional[ListRequestQueuesResponseQueueReason] = None
-    create_at: Optional[datetime] = Field(default=None, alias="createAt")
-    __properties: ClassVar[List[str]] = ["index", "reason", "createAt"]
+    queues: Optional[List[V1ListRequestQueuesResponseRequestQueue]] = None
+    __properties: ClassVar[List[str]] = ["queues"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True
     }
 
 
@@ -50,15 +47,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of ListRequestQueuesResponseRequestQueue from a JSON string"""
+        """Create an instance of V1ListRequestQueuesResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -69,26 +66,31 @@
         """
         _dict = self.model_dump(
             by_alias=True,
             exclude={
             },
             exclude_none=True,
         )
+        # override the default output from pydantic by calling `to_dict()` of each item in queues (list)
+        _items = []
+        if self.queues:
+            for _item in self.queues:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['queues'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> Self:
-        """Create an instance of ListRequestQueuesResponseRequestQueue from a dict"""
+        """Create an instance of V1ListRequestQueuesResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "index": obj.get("index"),
-            "reason": obj.get("reason"),
-            "createAt": obj.get("createAt")
+            "queues": [V1ListRequestQueuesResponseRequestQueue.from_dict(_item) for _item in obj.get("queues")] if obj.get("queues") is not None else None
         })
         return _obj
```

## Comparing `generated/schedulers/models/protobuf_any.py` & `generated/apps/models/protobuf_any.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/comm/v1/messages.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
```

## Comparing `generated/schedulers/models/rule_behavior.py` & `generated/apps/models/rule_behavior.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/comm/v1/messages.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
```

## Comparing `generated/schedulers/models/schedulerv1_cpu.py` & `generated/apps/models/app_service_protect_app_body.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/register_message.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
@@ -14,33 +14,29 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
-from pydantic import BaseModel, StrictInt, StrictStr
+
+from pydantic import BaseModel, StrictStr
 from pydantic import Field
 from typing import Dict, Any
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class Schedulerv1CPU(BaseModel):
+class AppServiceProtectAppBody(BaseModel):
     """
-    Schedulerv1CPU
+    AppServiceProtectAppBody
     """
-    model: Optional[StrictStr] = None
-    cores: Optional[StrictInt] = None
-    threads: Optional[StrictInt] = None
-    architecture: Optional[StrictStr] = None
-    cpu_num: Optional[StrictInt] = Field(default=None, alias="cpuNum")
-    __properties: ClassVar[List[str]] = ["model", "cores", "threads", "architecture", "cpuNum"]
+    public_key: StrictStr = Field(alias="publicKey")
+    __properties: ClassVar[List[str]] = ["publicKey"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True
     }
 
 
@@ -51,15 +47,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of Schedulerv1CPU from a JSON string"""
+        """Create an instance of AppServiceProtectAppBody from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -74,24 +70,20 @@
             },
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> Self:
-        """Create an instance of Schedulerv1CPU from a dict"""
+        """Create an instance of AppServiceProtectAppBody from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "model": obj.get("model"),
-            "cores": obj.get("cores"),
-            "threads": obj.get("threads"),
-            "architecture": obj.get("architecture"),
-            "cpuNum": obj.get("cpuNum")
+            "publicKey": obj.get("publicKey")
         })
         return _obj
```

## Comparing `generated/schedulers/models/schedulerv1_gpu.py` & `generated/apps/models/v1_list_response.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/register_message.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
@@ -14,35 +14,29 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
-from pydantic import BaseModel, StrictInt, StrictStr
-from pydantic import Field
-from generated.schedulers.models.v1_storage_size import V1StorageSize
+from typing import List, Optional
+from pydantic import BaseModel
+from generated.apps.models.v1_app import V1App
 from typing import Dict, Any
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class Schedulerv1GPU(BaseModel):
+class V1ListResponse(BaseModel):
     """
-    Schedulerv1GPU
+    V1ListResponse
     """
-    model: Optional[StrictStr] = None
-    driver_version: Optional[StrictStr] = Field(default=None, alias="driverVersion")
-    cuda_version: Optional[StrictStr] = Field(default=None, alias="CUDAVersion")
-    memory: Optional[V1StorageSize] = None
-    power: Optional[StrictStr] = None
-    gpu_num: Optional[StrictInt] = Field(default=None, alias="gpuNum")
-    __properties: ClassVar[List[str]] = ["model", "driverVersion", "CUDAVersion", "memory", "power", "gpuNum"]
+    apps: Optional[List[V1App]] = None
+    __properties: ClassVar[List[str]] = ["apps"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True
     }
 
 
@@ -53,15 +47,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of Schedulerv1GPU from a JSON string"""
+        """Create an instance of V1ListResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -72,32 +66,31 @@
         """
         _dict = self.model_dump(
             by_alias=True,
             exclude={
             },
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of memory
-        if self.memory:
-            _dict['memory'] = self.memory.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of each item in apps (list)
+        _items = []
+        if self.apps:
+            for _item in self.apps:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['apps'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> Self:
-        """Create an instance of Schedulerv1GPU from a dict"""
+        """Create an instance of V1ListResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "model": obj.get("model"),
-            "driverVersion": obj.get("driverVersion"),
-            "CUDAVersion": obj.get("CUDAVersion"),
-            "memory": V1StorageSize.from_dict(obj.get("memory")) if obj.get("memory") is not None else None,
-            "power": obj.get("power"),
-            "gpuNum": obj.get("gpuNum")
+            "apps": [V1App.from_dict(_item) for _item in obj.get("apps")] if obj.get("apps") is not None else None
         })
         return _obj
```

## Comparing `generated/schedulers/models/v1_app.py` & `generated/apps/models/v1_resource_claim.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/comm/v1/messages.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
@@ -13,39 +13,38 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from datetime import datetime
-from typing import Dict, Optional
-from pydantic import BaseModel, StrictStr
+
+from typing import List, Optional
+from pydantic import BaseModel, StrictInt, StrictStr
 from pydantic import Field
-from generated.schedulers.models.v1_app_status import V1AppStatus
 from typing import Dict, Any
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class V1App(BaseModel):
+class V1ResourceClaim(BaseModel):
     """
-    V1App
+    V1ResourceClaim
     """
-    id: Optional[StrictStr] = None
-    name: Optional[StrictStr] = None
-    user_id: Optional[StrictStr] = Field(default=None, alias="userId")
-    route_path: Optional[StrictStr] = Field(default=None, description="default route path is same with app_name. While app_name has conflict, route_path is required.", alias="routePath")
-    status: Optional[V1AppStatus] = None
-    error_msg: Optional[StrictStr] = Field(default=None, alias="errorMsg")
-    created_at: Optional[datetime] = Field(default=None, alias="createdAt")
-    modified_at: Optional[datetime] = Field(default=None, alias="modifiedAt")
-    labels: Optional[Dict[str, StrictStr]] = None
-    __properties: ClassVar[List[str]] = ["id", "name", "userId", "routePath", "status", "errorMsg", "createdAt", "modifiedAt", "labels"]
+    cpu_num: Optional[StrictInt] = Field(default=None, alias="cpuNum")
+    gpu_num: Optional[StrictInt] = Field(default=None, alias="gpuNum")
+    memory_mb: Optional[StrictInt] = Field(default=None, alias="memoryMb")
+    region_constraints: Optional[List[StrictStr]] = Field(default=None, alias="regionConstraints")
+    cpu_constraints: Optional[List[StrictStr]] = Field(default=None, alias="cpuConstraints")
+    cpu_architecture: Optional[List[StrictStr]] = Field(default=None, alias="cpuArchitecture")
+    gpu_constraints: Optional[List[StrictStr]] = Field(default=None, alias="gpuConstraints")
+    cuda_constraints: Optional[StrictStr] = Field(default=None, alias="cudaConstraints")
+    driver_version_constraints: Optional[StrictStr] = Field(default=None, alias="driverVersionConstraints")
+    __properties: ClassVar[List[str]] = ["cpuNum", "gpuNum", "memoryMb", "regionConstraints", "cpuConstraints", "cpuArchitecture", "gpuConstraints", "cudaConstraints", "driverVersionConstraints"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True
     }
 
 
@@ -56,15 +55,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of V1App from a JSON string"""
+        """Create an instance of V1ResourceClaim from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -79,28 +78,28 @@
             },
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> Self:
-        """Create an instance of V1App from a dict"""
+        """Create an instance of V1ResourceClaim from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "id": obj.get("id"),
-            "name": obj.get("name"),
-            "userId": obj.get("userId"),
-            "routePath": obj.get("routePath"),
-            "status": obj.get("status"),
-            "errorMsg": obj.get("errorMsg"),
-            "createdAt": obj.get("createdAt"),
-            "modifiedAt": obj.get("modifiedAt"),
-            "labels": obj.get("labels")
+            "cpuNum": obj.get("cpuNum"),
+            "gpuNum": obj.get("gpuNum"),
+            "memoryMb": obj.get("memoryMb"),
+            "regionConstraints": obj.get("regionConstraints"),
+            "cpuConstraints": obj.get("cpuConstraints"),
+            "cpuArchitecture": obj.get("cpuArchitecture"),
+            "gpuConstraints": obj.get("gpuConstraints"),
+            "cudaConstraints": obj.get("cudaConstraints"),
+            "driverVersionConstraints": obj.get("driverVersionConstraints")
         })
         return _obj
```

## Comparing `generated/schedulers/models/v1_app_service_setup_image_body.py` & `generated/apps/models/v1_app_service_setup_image_body.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/comm/v1/messages.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
@@ -17,15 +17,15 @@
 import re  # noqa: F401
 import json
 
 
 
 from pydantic import BaseModel
 from pydantic import Field
-from generated.schedulers.models.appsv1_setup_image import Appsv1SetupImage
+from generated.apps.models.appsv1_setup_image import Appsv1SetupImage
 from typing import Dict, Any
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
 class V1AppServiceSetupImageBody(BaseModel):
```

## Comparing `generated/schedulers/models/v1_app_status.py` & `generated/apps/models/v1_app_status.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/comm/v1/messages.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
@@ -38,14 +38,16 @@
     STATUS_INIT = 'STATUS_INIT'
     STATUS_PREPARING = 'STATUS_PREPARING'
     STATUS_READY = 'STATUS_READY'
     STATUS_DEPLOYED = 'STATUS_DEPLOYED'
     STATUS_PAUSED = 'STATUS_PAUSED'
     STATUS_NOT_READY = 'STATUS_NOT_READY'
     STATUS_ERROR = 'STATUS_ERROR'
+    STATUS_TERMINATING = 'STATUS_TERMINATING'
+    STATUS_DELETED = 'STATUS_DELETED'
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
         """Create an instance of V1AppStatus from a JSON string"""
         return cls(json.loads(json_str))
```

## Comparing `generated/schedulers/models/v1_autoscaling_policy.py` & `generated/apps/models/v1_autoscaling_policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/comm/v1/messages.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
@@ -17,16 +17,16 @@
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel
 from pydantic import Field
-from generated.schedulers.models.v1_built_in_policy import V1BuiltInPolicy
-from generated.schedulers.models.v1_custom_policy import V1CustomPolicy
+from generated.apps.models.v1_built_in_policy import V1BuiltInPolicy
+from generated.apps.models.v1_custom_policy import V1CustomPolicy
 from typing import Dict, Any
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
 class V1AutoscalingPolicy(BaseModel):
```

## Comparing `generated/schedulers/models/v1_bandwidth.py` & `generated/apps/models/v1_get_app_runtime_snapshot_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/comm/v1/messages.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
@@ -16,28 +16,27 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel
-from generated.schedulers.models.v1_bandwidth_size import V1BandwidthSize
+from generated.apps.models.v1_app_runtime import V1AppRuntime
 from typing import Dict, Any
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class V1Bandwidth(BaseModel):
+class V1GetAppRuntimeSnapshotResponse(BaseModel):
     """
-    V1Bandwidth
+    V1GetAppRuntimeSnapshotResponse
     """
-    incoming: Optional[V1BandwidthSize] = None
-    outgoing: Optional[V1BandwidthSize] = None
-    __properties: ClassVar[List[str]] = ["incoming", "outgoing"]
+    snapshot: Optional[V1AppRuntime] = None
+    __properties: ClassVar[List[str]] = ["snapshot"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True
     }
 
 
@@ -48,15 +47,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of V1Bandwidth from a JSON string"""
+        """Create an instance of V1GetAppRuntimeSnapshotResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -67,31 +66,27 @@
         """
         _dict = self.model_dump(
             by_alias=True,
             exclude={
             },
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of incoming
-        if self.incoming:
-            _dict['incoming'] = self.incoming.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of outgoing
-        if self.outgoing:
-            _dict['outgoing'] = self.outgoing.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of snapshot
+        if self.snapshot:
+            _dict['snapshot'] = self.snapshot.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> Self:
-        """Create an instance of V1Bandwidth from a dict"""
+        """Create an instance of V1GetAppRuntimeSnapshotResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "incoming": V1BandwidthSize.from_dict(obj.get("incoming")) if obj.get("incoming") is not None else None,
-            "outgoing": V1BandwidthSize.from_dict(obj.get("outgoing")) if obj.get("outgoing") is not None else None
+            "snapshot": V1AppRuntime.from_dict(obj.get("snapshot")) if obj.get("snapshot") is not None else None
         })
         return _obj
```

## Comparing `generated/schedulers/models/v1_bandwidth_size.py` & `generated/apps/models/v1_get_safety_remove_workers_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/comm/v1/messages.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
@@ -14,29 +14,28 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
+from typing import List, Optional
 from pydantic import BaseModel, StrictStr
 from typing import Dict, Any
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class V1BandwidthSize(BaseModel):
+class V1GetSafetyRemoveWorkersResponse(BaseModel):
     """
-    V1BandwidthSize
+    V1GetSafetyRemoveWorkersResponse
     """
-    size: Optional[StrictStr] = None
-    unit: StrictStr
-    __properties: ClassVar[List[str]] = ["size", "unit"]
+    workers: Optional[List[StrictStr]] = None
+    __properties: ClassVar[List[str]] = ["workers"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True
     }
 
 
@@ -47,15 +46,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of V1BandwidthSize from a JSON string"""
+        """Create an instance of V1GetSafetyRemoveWorkersResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -70,21 +69,20 @@
             },
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> Self:
-        """Create an instance of V1BandwidthSize from a dict"""
+        """Create an instance of V1GetSafetyRemoveWorkersResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "size": obj.get("size"),
-            "unit": obj.get("unit")
+            "workers": obj.get("workers")
         })
         return _obj
```

## Comparing `generated/schedulers/models/v1_basic_auth.py` & `generated/apps/models/v1_basic_auth.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/comm/v1/messages.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
@@ -16,15 +16,15 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel
-from generated.schedulers.models.v1_value_from_secret import V1ValueFromSecret
+from generated.apps.models.v1_value_from_secret import V1ValueFromSecret
 from typing import Dict, Any
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
 class V1BasicAuth(BaseModel):
```

## Comparing `generated/schedulers/models/v1_build_in_policy.py` & `generated/apps/models/v1_built_in_policy.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/register_message.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
@@ -13,73 +13,75 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, Field, StrictInt, StrictStr
-from typing import Any, ClassVar, Dict, List, Optional
-from typing import Optional, Set
-from typing_extensions import Self
 
-class V1BuildInPolicy(BaseModel):
+from typing import Optional
+from pydantic import BaseModel, StrictInt
+from pydantic import Field
+from typing import Dict, Any
+try:
+    from typing import Self
+except ImportError:
+    from typing_extensions import Self
+
+class V1BuiltInPolicy(BaseModel):
+    """
+    V1BuiltInPolicy
     """
-    V1BuildInPolicy
-    """ # noqa: E501
     min_worker_num: Optional[StrictInt] = Field(default=None, alias="minWorkerNum")
     max_worker_num: Optional[StrictInt] = Field(default=None, alias="maxWorkerNum")
     max_queue_num: Optional[StrictInt] = Field(default=None, alias="maxQueueNum")
-    max_idle_time: Optional[StrictStr] = Field(default=None, alias="maxIdleTime")
+    max_idle_time: Optional[StrictInt] = Field(default=None, alias="maxIdleTime")
     __properties: ClassVar[List[str]] = ["minWorkerNum", "maxWorkerNum", "maxQueueNum", "maxIdleTime"]
 
-    model_config = ConfigDict(
-        populate_by_name=True,
-        validate_assignment=True,
-        protected_namespaces=(),
-    )
+    model_config = {
+        "populate_by_name": True,
+        "validate_assignment": True
+    }
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of V1BuildInPolicy from a JSON string"""
+    def from_json(cls, json_str: str) -> Self:
+        """Create an instance of V1BuiltInPolicy from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
         """
-        excluded_fields: Set[str] = set([
-        ])
-
         _dict = self.model_dump(
             by_alias=True,
-            exclude=excluded_fields,
+            exclude={
+            },
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of V1BuildInPolicy from a dict"""
+    def from_dict(cls, obj: dict) -> Self:
+        """Create an instance of V1BuiltInPolicy from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
```

## Comparing `generated/schedulers/models/v1_built_in_policy.py` & `generated/apps/models/v1_setup_volume.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/comm/v1/messages.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
@@ -15,31 +15,31 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, StrictInt
+from pydantic import BaseModel, StrictBool, StrictStr
 from pydantic import Field
 from typing import Dict, Any
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class V1BuiltInPolicy(BaseModel):
+class V1SetupVolume(BaseModel):
     """
-    V1BuiltInPolicy
+    V1SetupVolume
     """
-    min_worker_num: Optional[StrictInt] = Field(default=None, alias="minWorkerNum")
-    max_worker_num: Optional[StrictInt] = Field(default=None, alias="maxWorkerNum")
-    max_queue_num: Optional[StrictInt] = Field(default=None, alias="maxQueueNum")
-    max_idle_time: Optional[StrictInt] = Field(default=None, alias="maxIdleTime")
-    __properties: ClassVar[List[str]] = ["minWorkerNum", "maxWorkerNum", "maxQueueNum", "maxIdleTime"]
+    volume_name: StrictStr = Field(alias="volumeName")
+    revision: Optional[StrictStr] = None
+    optional: Optional[StrictBool] = None
+    create_if_not_exists: Optional[StrictBool] = Field(default=None, alias="createIfNotExists")
+    __properties: ClassVar[List[str]] = ["volumeName", "revision", "optional", "createIfNotExists"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True
     }
 
 
@@ -50,46 +50,48 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of V1BuiltInPolicy from a JSON string"""
+        """Create an instance of V1SetupVolume from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
+        * OpenAPI `readOnly` fields are excluded.
         """
         _dict = self.model_dump(
             by_alias=True,
             exclude={
+                "revision",
             },
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> Self:
-        """Create an instance of V1BuiltInPolicy from a dict"""
+        """Create an instance of V1SetupVolume from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "minWorkerNum": obj.get("minWorkerNum"),
-            "maxWorkerNum": obj.get("maxWorkerNum"),
-            "maxQueueNum": obj.get("maxQueueNum"),
-            "maxIdleTime": obj.get("maxIdleTime")
+            "volumeName": obj.get("volumeName"),
+            "revision": obj.get("revision"),
+            "optional": obj.get("optional"),
+            "createIfNotExists": obj.get("createIfNotExists")
         })
         return _obj
```

## Comparing `generated/schedulers/models/v1_cpu.py` & `generated/apps/models/v1_custom_policy.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/comm/v1/messages.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
@@ -14,33 +14,29 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
-from pydantic import BaseModel, StrictInt, StrictStr
-from pydantic import Field
+from typing import List, Optional
+from pydantic import BaseModel
+from generated.apps.models.v1_rule import V1Rule
 from typing import Dict, Any
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class V1CPU(BaseModel):
+class V1CustomPolicy(BaseModel):
     """
-    V1CPU
+    V1CustomPolicy
     """
-    model: Optional[StrictStr] = None
-    cores: Optional[StrictInt] = None
-    threads: Optional[StrictInt] = None
-    architecture: Optional[StrictStr] = None
-    cpu_num: Optional[StrictInt] = Field(default=None, alias="cpuNum")
-    __properties: ClassVar[List[str]] = ["model", "cores", "threads", "architecture", "cpuNum"]
+    rules: Optional[List[V1Rule]] = None
+    __properties: ClassVar[List[str]] = ["rules"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True
     }
 
 
@@ -51,15 +47,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of V1CPU from a JSON string"""
+        """Create an instance of V1CustomPolicy from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -70,28 +66,31 @@
         """
         _dict = self.model_dump(
             by_alias=True,
             exclude={
             },
             exclude_none=True,
         )
+        # override the default output from pydantic by calling `to_dict()` of each item in rules (list)
+        _items = []
+        if self.rules:
+            for _item in self.rules:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['rules'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> Self:
-        """Create an instance of V1CPU from a dict"""
+        """Create an instance of V1CustomPolicy from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "model": obj.get("model"),
-            "cores": obj.get("cores"),
-            "threads": obj.get("threads"),
-            "architecture": obj.get("architecture"),
-            "cpuNum": obj.get("cpuNum")
+            "rules": [V1Rule.from_dict(_item) for _item in obj.get("rules")] if obj.get("rules") is not None else None
         })
         return _obj
```

## Comparing `generated/schedulers/models/v1_create_volume_request.py` & `generated/apps/models/v1_list_workers_by_status_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/comm/v1/messages.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
@@ -14,35 +14,29 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
-from pydantic import BaseModel, StrictStr
-from pydantic import Field
+from typing import List, Optional
+from pydantic import BaseModel
+from generated.apps.models.v1_worker import V1Worker
 from typing import Dict, Any
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class V1CreateVolumeRequest(BaseModel):
+class V1ListWorkersByStatusResponse(BaseModel):
     """
-    V1CreateVolumeRequest
+    V1ListWorkersByStatusResponse
     """
-    request_id: StrictStr = Field(alias="requestId")
-    user_id: StrictStr = Field(alias="userId")
-    app_id: StrictStr = Field(alias="appId")
-    name: StrictStr
-    size: StrictStr
-    mode: StrictStr
-    revision: Optional[StrictStr] = None
-    __properties: ClassVar[List[str]] = ["requestId", "userId", "appId", "name", "size", "mode", "revision"]
+    workers: Optional[List[V1Worker]] = None
+    __properties: ClassVar[List[str]] = ["workers"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True
     }
 
 
@@ -53,15 +47,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of V1CreateVolumeRequest from a JSON string"""
+        """Create an instance of V1ListWorkersByStatusResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -72,30 +66,31 @@
         """
         _dict = self.model_dump(
             by_alias=True,
             exclude={
             },
             exclude_none=True,
         )
+        # override the default output from pydantic by calling `to_dict()` of each item in workers (list)
+        _items = []
+        if self.workers:
+            for _item in self.workers:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['workers'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> Self:
-        """Create an instance of V1CreateVolumeRequest from a dict"""
+        """Create an instance of V1ListWorkersByStatusResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "requestId": obj.get("requestId"),
-            "userId": obj.get("userId"),
-            "appId": obj.get("appId"),
-            "name": obj.get("name"),
-            "size": obj.get("size"),
-            "mode": obj.get("mode"),
-            "revision": obj.get("revision")
+            "workers": [V1Worker.from_dict(_item) for _item in obj.get("workers")] if obj.get("workers") is not None else None
         })
         return _obj
```

## Comparing `generated/schedulers/models/v1_create_volume_response.py` & `generated/apps/models/v1_list_workers_by_app_and_user_response.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/comm/v1/messages.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
@@ -14,31 +14,29 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
-from pydantic import BaseModel, StrictStr
-from pydantic import Field
-from generated.schedulers.models.v1_volume import V1Volume
+from typing import List, Optional
+from pydantic import BaseModel
+from generated.apps.models.v1_worker import V1Worker
 from typing import Dict, Any
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class V1CreateVolumeResponse(BaseModel):
+class V1ListWorkersByAppAndUserResponse(BaseModel):
     """
-    V1CreateVolumeResponse
+    V1ListWorkersByAppAndUserResponse
     """
-    request_id: StrictStr = Field(alias="requestId")
-    volume: Optional[V1Volume] = None
-    __properties: ClassVar[List[str]] = ["requestId", "volume"]
+    workers: Optional[List[V1Worker]] = None
+    __properties: ClassVar[List[str]] = ["workers"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True
     }
 
 
@@ -49,15 +47,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of V1CreateVolumeResponse from a JSON string"""
+        """Create an instance of V1ListWorkersByAppAndUserResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -68,28 +66,31 @@
         """
         _dict = self.model_dump(
             by_alias=True,
             exclude={
             },
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of volume
-        if self.volume:
-            _dict['volume'] = self.volume.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of each item in workers (list)
+        _items = []
+        if self.workers:
+            for _item in self.workers:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['workers'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> Self:
-        """Create an instance of V1CreateVolumeResponse from a dict"""
+        """Create an instance of V1ListWorkersByAppAndUserResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "requestId": obj.get("requestId"),
-            "volume": V1Volume.from_dict(obj.get("volume")) if obj.get("volume") is not None else None
+            "workers": [V1Worker.from_dict(_item) for _item in obj.get("workers")] if obj.get("workers") is not None else None
         })
         return _obj
```

## Comparing `generated/schedulers/models/v1_custom_policy.py` & `generated/apps/models/v1_list_worker_details_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/comm/v1/messages.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
@@ -16,27 +16,27 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
 from pydantic import BaseModel
-from generated.schedulers.models.v1_rule import V1Rule
+from generated.apps.models.v1_worker import V1Worker
 from typing import Dict, Any
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class V1CustomPolicy(BaseModel):
+class V1ListWorkerDetailsResponse(BaseModel):
     """
-    V1CustomPolicy
+    V1ListWorkerDetailsResponse
     """
-    rules: Optional[List[V1Rule]] = None
-    __properties: ClassVar[List[str]] = ["rules"]
+    workers: Optional[List[V1Worker]] = None
+    __properties: ClassVar[List[str]] = ["workers"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True
     }
 
 
@@ -47,15 +47,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of V1CustomPolicy from a JSON string"""
+        """Create an instance of V1ListWorkerDetailsResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -66,31 +66,31 @@
         """
         _dict = self.model_dump(
             by_alias=True,
             exclude={
             },
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of each item in rules (list)
+        # override the default output from pydantic by calling `to_dict()` of each item in workers (list)
         _items = []
-        if self.rules:
-            for _item in self.rules:
+        if self.workers:
+            for _item in self.workers:
                 if _item:
                     _items.append(_item.to_dict())
-            _dict['rules'] = _items
+            _dict['workers'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> Self:
-        """Create an instance of V1CustomPolicy from a dict"""
+        """Create an instance of V1ListWorkerDetailsResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "rules": [V1Rule.from_dict(_item) for _item in obj.get("rules")] if obj.get("rules") is not None else None
+            "workers": [V1Worker.from_dict(_item) for _item in obj.get("workers")] if obj.get("workers") is not None else None
         })
         return _obj
```

## Comparing `generated/schedulers/models/v1_delete_volume_request.py` & `generated/apps/models/v1_list_request_queues_response_request_queue.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/comm/v1/messages.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
@@ -13,35 +13,33 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-
+from datetime import datetime
 from typing import Optional
-from pydantic import BaseModel, StrictBool, StrictStr
+from pydantic import BaseModel, StrictInt
 from pydantic import Field
+from generated.apps.models.list_request_queues_response_queue_reason import ListRequestQueuesResponseQueueReason
 from typing import Dict, Any
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class V1DeleteVolumeRequest(BaseModel):
+class V1ListRequestQueuesResponseRequestQueue(BaseModel):
     """
-    V1DeleteVolumeRequest
+    V1ListRequestQueuesResponseRequestQueue
     """
-    request_id: StrictStr = Field(alias="requestId")
-    user_id: StrictStr = Field(alias="userId")
-    app_id: StrictStr = Field(alias="appId")
-    name: StrictStr
-    worker_id: Optional[StrictStr] = Field(default=None, alias="workerId")
-    force: Optional[StrictBool] = None
-    __properties: ClassVar[List[str]] = ["requestId", "userId", "appId", "name", "workerId", "force"]
+    index: Optional[StrictInt] = None
+    reason: Optional[ListRequestQueuesResponseQueueReason] = None
+    create_at: Optional[datetime] = Field(default=None, alias="createAt")
+    __properties: ClassVar[List[str]] = ["index", "reason", "createAt"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True
     }
 
 
@@ -52,15 +50,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of V1DeleteVolumeRequest from a JSON string"""
+        """Create an instance of V1ListRequestQueuesResponseRequestQueue from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -75,25 +73,22 @@
             },
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> Self:
-        """Create an instance of V1DeleteVolumeRequest from a dict"""
+        """Create an instance of V1ListRequestQueuesResponseRequestQueue from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "requestId": obj.get("requestId"),
-            "userId": obj.get("userId"),
-            "appId": obj.get("appId"),
-            "name": obj.get("name"),
-            "workerId": obj.get("workerId"),
-            "force": obj.get("force")
+            "index": obj.get("index"),
+            "reason": obj.get("reason"),
+            "createAt": obj.get("createAt")
         })
         return _obj
```

## Comparing `generated/schedulers/models/v1_delete_volume_response.py` & `generated/apps/models/v1_rule.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/register_message.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
@@ -14,30 +14,33 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
+from typing import List, Optional
 from pydantic import BaseModel, StrictStr
 from pydantic import Field
+from generated.apps.models.protobuf_any import ProtobufAny
+from generated.apps.models.rule_behavior import RuleBehavior
 from typing import Dict, Any
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class V1DeleteVolumeResponse(BaseModel):
+class V1Rule(BaseModel):
     """
-    V1DeleteVolumeResponse
+    V1Rule
     """
-    ret_code: Optional[StrictStr] = Field(default=None, alias="retCode")
-    message: Optional[StrictStr] = None
-    __properties: ClassVar[List[str]] = ["retCode", "message"]
+    factor: Optional[List[StrictStr]] = None
+    behavior: Optional[RuleBehavior] = None
+    custom_func: Optional[ProtobufAny] = Field(default=None, alias="customFunc")
+    __properties: ClassVar[List[str]] = ["factor", "behavior", "customFunc"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True
     }
 
 
@@ -48,15 +51,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of V1DeleteVolumeResponse from a JSON string"""
+        """Create an instance of V1Rule from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -67,25 +70,29 @@
         """
         _dict = self.model_dump(
             by_alias=True,
             exclude={
             },
             exclude_none=True,
         )
+        # override the default output from pydantic by calling `to_dict()` of custom_func
+        if self.custom_func:
+            _dict['customFunc'] = self.custom_func.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> Self:
-        """Create an instance of V1DeleteVolumeResponse from a dict"""
+        """Create an instance of V1Rule from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "retCode": obj.get("retCode"),
-            "message": obj.get("message")
+            "factor": obj.get("factor"),
+            "behavior": obj.get("behavior"),
+            "customFunc": ProtobufAny.from_dict(obj.get("customFunc")) if obj.get("customFunc") is not None else None
         })
         return _obj
```

## Comparing `generated/schedulers/models/v1_device_resource.py` & `generated/apps/models/v1_app_revision.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/comm/v1/messages.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
@@ -13,42 +13,42 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-
+from datetime import datetime
 from typing import List, Optional
 from pydantic import BaseModel, StrictStr
 from pydantic import Field
-from generated.schedulers.models.v1_bandwidth import V1Bandwidth
-from generated.schedulers.models.v1_cpu import V1CPU
-from generated.schedulers.models.v1_filesystem import V1Filesystem
-from generated.schedulers.models.v1_gpu import V1GPU
-from generated.schedulers.models.v1_storage_size import V1StorageSize
+from generated.apps.models.appsv1_setup_image import Appsv1SetupImage
+from generated.apps.models.v1_autoscaling_policy import V1AutoscalingPolicy
+from generated.apps.models.v1_resource_claim import V1ResourceClaim
+from generated.apps.models.v1_setup_volume import V1SetupVolume
+from generated.apps.models.v1_worker import V1Worker
 from typing import Dict, Any
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class V1DeviceResource(BaseModel):
+class V1AppRevision(BaseModel):
     """
-    V1DeviceResource
+    V1AppRevision
     """
-    device_id: Optional[StrictStr] = Field(default=None, alias="deviceId")
-    cpu: V1CPU
-    memory: V1StorageSize
-    gpu: Optional[V1GPU] = None
-    filesystems: Optional[List[V1Filesystem]] = None
-    bandwidth: Optional[V1Bandwidth] = None
-    timezone: Optional[StrictStr] = None
-    public_address: Optional[StrictStr] = Field(default=None, alias="publicAddress")
-    __properties: ClassVar[List[str]] = ["deviceId", "cpu", "memory", "gpu", "filesystems", "bandwidth", "timezone", "publicAddress"]
+    name: Optional[StrictStr] = None
+    volumes: Optional[List[V1SetupVolume]] = None
+    image: Optional[Appsv1SetupImage] = None
+    resource_claim: Optional[V1ResourceClaim] = Field(default=None, alias="resourceClaim")
+    secret_names: Optional[List[StrictStr]] = Field(default=None, alias="secretNames")
+    autoscaling_policy: Optional[V1AutoscalingPolicy] = Field(default=None, alias="autoscalingPolicy")
+    workers: Optional[List[V1Worker]] = None
+    create_at: Optional[datetime] = Field(default=None, alias="createAt")
+    __properties: ClassVar[List[str]] = ["name", "volumes", "image", "resourceClaim", "secretNames", "autoscalingPolicy", "workers", "createAt"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True
     }
 
 
@@ -59,15 +59,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of V1DeviceResource from a JSON string"""
+        """Create an instance of V1AppRevision from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -78,50 +78,54 @@
         """
         _dict = self.model_dump(
             by_alias=True,
             exclude={
             },
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of cpu
-        if self.cpu:
-            _dict['cpu'] = self.cpu.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of memory
-        if self.memory:
-            _dict['memory'] = self.memory.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of gpu
-        if self.gpu:
-            _dict['gpu'] = self.gpu.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of each item in filesystems (list)
+        # override the default output from pydantic by calling `to_dict()` of each item in volumes (list)
+        _items = []
+        if self.volumes:
+            for _item in self.volumes:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['volumes'] = _items
+        # override the default output from pydantic by calling `to_dict()` of image
+        if self.image:
+            _dict['image'] = self.image.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of resource_claim
+        if self.resource_claim:
+            _dict['resourceClaim'] = self.resource_claim.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of autoscaling_policy
+        if self.autoscaling_policy:
+            _dict['autoscalingPolicy'] = self.autoscaling_policy.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of each item in workers (list)
         _items = []
-        if self.filesystems:
-            for _item in self.filesystems:
+        if self.workers:
+            for _item in self.workers:
                 if _item:
                     _items.append(_item.to_dict())
-            _dict['filesystems'] = _items
-        # override the default output from pydantic by calling `to_dict()` of bandwidth
-        if self.bandwidth:
-            _dict['bandwidth'] = self.bandwidth.to_dict()
+            _dict['workers'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> Self:
-        """Create an instance of V1DeviceResource from a dict"""
+        """Create an instance of V1AppRevision from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "deviceId": obj.get("deviceId"),
-            "cpu": V1CPU.from_dict(obj.get("cpu")) if obj.get("cpu") is not None else None,
-            "memory": V1StorageSize.from_dict(obj.get("memory")) if obj.get("memory") is not None else None,
-            "gpu": V1GPU.from_dict(obj.get("gpu")) if obj.get("gpu") is not None else None,
-            "filesystems": [V1Filesystem.from_dict(_item) for _item in obj.get("filesystems")] if obj.get("filesystems") is not None else None,
-            "bandwidth": V1Bandwidth.from_dict(obj.get("bandwidth")) if obj.get("bandwidth") is not None else None,
-            "timezone": obj.get("timezone"),
-            "publicAddress": obj.get("publicAddress")
+            "name": obj.get("name"),
+            "volumes": [V1SetupVolume.from_dict(_item) for _item in obj.get("volumes")] if obj.get("volumes") is not None else None,
+            "image": Appsv1SetupImage.from_dict(obj.get("image")) if obj.get("image") is not None else None,
+            "resourceClaim": V1ResourceClaim.from_dict(obj.get("resourceClaim")) if obj.get("resourceClaim") is not None else None,
+            "secretNames": obj.get("secretNames"),
+            "autoscalingPolicy": V1AutoscalingPolicy.from_dict(obj.get("autoscalingPolicy")) if obj.get("autoscalingPolicy") is not None else None,
+            "workers": [V1Worker.from_dict(_item) for _item in obj.get("workers")] if obj.get("workers") is not None else None,
+            "createAt": obj.get("createAt")
         })
         return _obj
```

## Comparing `generated/schedulers/models/v1_empty_response.py` & `generated/apps/models/v1_check_and_lock_worker_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/comm/v1/messages.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
@@ -14,29 +14,31 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-
-from pydantic import BaseModel, StrictStr
+from typing import Optional
+from pydantic import BaseModel, StrictBool
 from pydantic import Field
+from generated.apps.models.v1_worker import V1Worker
 from typing import Dict, Any
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class V1EmptyResponse(BaseModel):
+class V1CheckAndLockWorkerResponse(BaseModel):
     """
-    V1EmptyResponse
+    V1CheckAndLockWorkerResponse
     """
-    request_id: StrictStr = Field(alias="requestId")
-    __properties: ClassVar[List[str]] = ["requestId"]
+    is_distributed: Optional[StrictBool] = Field(default=None, alias="isDistributed")
+    worker: Optional[V1Worker] = None
+    __properties: ClassVar[List[str]] = ["isDistributed", "worker"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True
     }
 
 
@@ -47,15 +49,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of V1EmptyResponse from a JSON string"""
+        """Create an instance of V1CheckAndLockWorkerResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -66,24 +68,28 @@
         """
         _dict = self.model_dump(
             by_alias=True,
             exclude={
             },
             exclude_none=True,
         )
+        # override the default output from pydantic by calling `to_dict()` of worker
+        if self.worker:
+            _dict['worker'] = self.worker.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> Self:
-        """Create an instance of V1EmptyResponse from a dict"""
+        """Create an instance of V1CheckAndLockWorkerResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "requestId": obj.get("requestId")
+            "isDistributed": obj.get("isDistributed"),
+            "worker": V1Worker.from_dict(obj.get("worker")) if obj.get("worker") is not None else None
         })
         return _obj
```

## Comparing `generated/schedulers/models/v1_error_response.py` & `generated/apps/models/v1_list_workers_by_device_and_status_response.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/comm/v1/messages.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
@@ -14,32 +14,29 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
-from pydantic import BaseModel, StrictInt, StrictStr
-from pydantic import Field
+from typing import List, Optional
+from pydantic import BaseModel
+from generated.apps.models.v1_worker import V1Worker
 from typing import Dict, Any
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class V1ErrorResponse(BaseModel):
+class V1ListWorkersByDeviceAndStatusResponse(BaseModel):
     """
-    V1ErrorResponse
+    V1ListWorkersByDeviceAndStatusResponse
     """
-    request_id: StrictStr = Field(alias="requestId")
-    method: Optional[StrictStr] = None
-    code: Optional[StrictInt] = None
-    message: Optional[StrictStr] = None
-    __properties: ClassVar[List[str]] = ["requestId", "method", "code", "message"]
+    workers: Optional[List[V1Worker]] = None
+    __properties: ClassVar[List[str]] = ["workers"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True
     }
 
 
@@ -50,15 +47,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of V1ErrorResponse from a JSON string"""
+        """Create an instance of V1ListWorkersByDeviceAndStatusResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -69,27 +66,31 @@
         """
         _dict = self.model_dump(
             by_alias=True,
             exclude={
             },
             exclude_none=True,
         )
+        # override the default output from pydantic by calling `to_dict()` of each item in workers (list)
+        _items = []
+        if self.workers:
+            for _item in self.workers:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['workers'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> Self:
-        """Create an instance of V1ErrorResponse from a dict"""
+        """Create an instance of V1ListWorkersByDeviceAndStatusResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "requestId": obj.get("requestId"),
-            "method": obj.get("method"),
-            "code": obj.get("code"),
-            "message": obj.get("message")
+            "workers": [V1Worker.from_dict(_item) for _item in obj.get("workers")] if obj.get("workers") is not None else None
         })
         return _obj
```

## Comparing `generated/schedulers/models/v1_filesystem.py` & `generated/apps/models/v1_list_all_apps_with_workers_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/comm/v1/messages.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
@@ -14,35 +14,29 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
-from pydantic import BaseModel, StrictBool, StrictStr
-from pydantic import Field
-from generated.schedulers.models.v1_storage_size import V1StorageSize
+from typing import List, Optional
+from pydantic import BaseModel
+from generated.apps.models.v1_app import V1App
 from typing import Dict, Any
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class V1Filesystem(BaseModel):
+class V1ListAllAppsWithWorkersResponse(BaseModel):
     """
-    V1Filesystem
+    V1ListAllAppsWithWorkersResponse
     """
-    device: Optional[StrictStr] = None
-    mount_point: Optional[StrictStr] = Field(default=None, alias="mountPoint")
-    size: Optional[V1StorageSize] = None
-    type: StrictStr
-    bootable: Optional[StrictBool] = None
-    media_type: StrictStr = Field(alias="mediaType")
-    __properties: ClassVar[List[str]] = ["device", "mountPoint", "size", "type", "bootable", "mediaType"]
+    apps: Optional[List[V1App]] = None
+    __properties: ClassVar[List[str]] = ["apps"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True
     }
 
 
@@ -53,15 +47,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of V1Filesystem from a JSON string"""
+        """Create an instance of V1ListAllAppsWithWorkersResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -72,32 +66,31 @@
         """
         _dict = self.model_dump(
             by_alias=True,
             exclude={
             },
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of size
-        if self.size:
-            _dict['size'] = self.size.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of each item in apps (list)
+        _items = []
+        if self.apps:
+            for _item in self.apps:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['apps'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> Self:
-        """Create an instance of V1Filesystem from a dict"""
+        """Create an instance of V1ListAllAppsWithWorkersResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "device": obj.get("device"),
-            "mountPoint": obj.get("mountPoint"),
-            "size": V1StorageSize.from_dict(obj.get("size")) if obj.get("size") is not None else None,
-            "type": obj.get("type"),
-            "bootable": obj.get("bootable"),
-            "mediaType": obj.get("mediaType")
+            "apps": [V1App.from_dict(_item) for _item in obj.get("apps")] if obj.get("apps") is not None else None
         })
         return _obj
```

## Comparing `generated/schedulers/models/v1_get_image_request.py` & `generated/apps/models/v1_list_app_by_unique_ids_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/comm/v1/messages.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
@@ -14,30 +14,29 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-
-from pydantic import BaseModel, StrictStr
-from pydantic import Field
+from typing import List, Optional
+from pydantic import BaseModel
+from generated.apps.models.v1_app import V1App
 from typing import Dict, Any
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class V1GetImageRequest(BaseModel):
+class V1ListAppByUniqueIDsResponse(BaseModel):
     """
-    V1GetImageRequest
+    V1ListAppByUniqueIDsResponse
     """
-    request_id: StrictStr = Field(alias="requestId")
-    repository: StrictStr
-    __properties: ClassVar[List[str]] = ["requestId", "repository"]
+    apps: Optional[List[V1App]] = None
+    __properties: ClassVar[List[str]] = ["apps"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True
     }
 
 
@@ -48,15 +47,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of V1GetImageRequest from a JSON string"""
+        """Create an instance of V1ListAppByUniqueIDsResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -67,25 +66,31 @@
         """
         _dict = self.model_dump(
             by_alias=True,
             exclude={
             },
             exclude_none=True,
         )
+        # override the default output from pydantic by calling `to_dict()` of each item in apps (list)
+        _items = []
+        if self.apps:
+            for _item in self.apps:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['apps'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> Self:
-        """Create an instance of V1GetImageRequest from a dict"""
+        """Create an instance of V1ListAppByUniqueIDsResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "requestId": obj.get("requestId"),
-            "repository": obj.get("repository")
+            "apps": [V1App.from_dict(_item) for _item in obj.get("apps")] if obj.get("apps") is not None else None
         })
         return _obj
```

## Comparing `generated/schedulers/models/v1_get_image_response.py` & `generated/apps/models/v1_list_apps_by_user_response.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/comm/v1/messages.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
@@ -14,31 +14,29 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
-from pydantic import BaseModel, StrictStr
-from pydantic import Field
-from generated.schedulers.models.v1_image import V1Image
+from typing import List, Optional
+from pydantic import BaseModel
+from generated.apps.models.v1_app import V1App
 from typing import Dict, Any
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class V1GetImageResponse(BaseModel):
+class V1ListAppsByUserResponse(BaseModel):
     """
-    V1GetImageResponse
+    V1ListAppsByUserResponse
     """
-    request_id: StrictStr = Field(alias="requestId")
-    image: Optional[V1Image] = None
-    __properties: ClassVar[List[str]] = ["requestId", "image"]
+    apps: Optional[List[V1App]] = None
+    __properties: ClassVar[List[str]] = ["apps"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True
     }
 
 
@@ -49,15 +47,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of V1GetImageResponse from a JSON string"""
+        """Create an instance of V1ListAppsByUserResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -68,28 +66,31 @@
         """
         _dict = self.model_dump(
             by_alias=True,
             exclude={
             },
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of image
-        if self.image:
-            _dict['image'] = self.image.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of each item in apps (list)
+        _items = []
+        if self.apps:
+            for _item in self.apps:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['apps'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> Self:
-        """Create an instance of V1GetImageResponse from a dict"""
+        """Create an instance of V1ListAppsByUserResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "requestId": obj.get("requestId"),
-            "image": V1Image.from_dict(obj.get("image")) if obj.get("image") is not None else None
+            "apps": [V1App.from_dict(_item) for _item in obj.get("apps")] if obj.get("apps") is not None else None
         })
         return _obj
```

## Comparing `generated/schedulers/models/v1_gpu.py` & `generated/apps/models/v1_list_workers_response.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/comm/v1/messages.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
@@ -13,36 +13,36 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-
-from typing import Optional
+from datetime import datetime
+from typing import List, Optional
 from pydantic import BaseModel, StrictInt, StrictStr
 from pydantic import Field
-from generated.schedulers.models.v1_storage_size import V1StorageSize
+from generated.apps.models.v1_worker import V1Worker
 from typing import Dict, Any
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class V1GPU(BaseModel):
+class V1ListWorkersResponse(BaseModel):
     """
-    V1GPU
+    V1ListWorkersResponse
     """
-    model: Optional[StrictStr] = None
-    driver_version: Optional[StrictStr] = Field(default=None, alias="driverVersion")
-    cuda_version: Optional[StrictStr] = Field(default=None, alias="CUDAVersion")
-    memory: Optional[V1StorageSize] = None
-    power: Optional[StrictStr] = None
-    gpu_num: Optional[StrictInt] = Field(default=None, alias="gpuNum")
-    __properties: ClassVar[List[str]] = ["model", "driverVersion", "CUDAVersion", "memory", "power", "gpuNum"]
+    workers: Optional[List[V1Worker]] = None
+    queue_size: Optional[StrictInt] = Field(default=None, alias="queueSize")
+    queue_name: Optional[StrictStr] = Field(default=None, alias="queueName")
+    last_scale_up_time: Optional[datetime] = Field(default=None, alias="lastScaleUpTime")
+    last_scale_down_delete_time: Optional[datetime] = Field(default=None, alias="lastScaleDownDeleteTime")
+    max_workers: Optional[StrictInt] = Field(default=None, alias="maxWorkers")
+    __properties: ClassVar[List[str]] = ["workers", "queueSize", "queueName", "lastScaleUpTime", "lastScaleDownDeleteTime", "maxWorkers"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True
     }
 
 
@@ -53,15 +53,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of V1GPU from a JSON string"""
+        """Create an instance of V1ListWorkersResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -72,32 +72,36 @@
         """
         _dict = self.model_dump(
             by_alias=True,
             exclude={
             },
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of memory
-        if self.memory:
-            _dict['memory'] = self.memory.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of each item in workers (list)
+        _items = []
+        if self.workers:
+            for _item in self.workers:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['workers'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> Self:
-        """Create an instance of V1GPU from a dict"""
+        """Create an instance of V1ListWorkersResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "model": obj.get("model"),
-            "driverVersion": obj.get("driverVersion"),
-            "CUDAVersion": obj.get("CUDAVersion"),
-            "memory": V1StorageSize.from_dict(obj.get("memory")) if obj.get("memory") is not None else None,
-            "power": obj.get("power"),
-            "gpuNum": obj.get("gpuNum")
+            "workers": [V1Worker.from_dict(_item) for _item in obj.get("workers")] if obj.get("workers") is not None else None,
+            "queueSize": obj.get("queueSize"),
+            "queueName": obj.get("queueName"),
+            "lastScaleUpTime": obj.get("lastScaleUpTime"),
+            "lastScaleDownDeleteTime": obj.get("lastScaleDownDeleteTime"),
+            "maxWorkers": obj.get("maxWorkers")
         })
         return _obj
```

## Comparing `generated/schedulers/models/v1_list_workers_response.py` & `generated/apps/models/v1_app_runtime.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/comm/v1/messages.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
@@ -13,36 +13,39 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from datetime import datetime
-from typing import List, Optional
-from pydantic import BaseModel, StrictInt, StrictStr
+
+from typing import Dict, List, Optional
+from pydantic import BaseModel, StrictBool, StrictInt, StrictStr
 from pydantic import Field
-from generated.schedulers.models.appsv1_worker import Appsv1Worker
+from generated.apps.models.app_runtimev1_request_queue import AppRuntimev1RequestQueue
+from generated.apps.models.v1_app import V1App
+from generated.apps.models.v1_worker_runtime import V1WorkerRuntime
 from typing import Dict, Any
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class V1ListWorkersResponse(BaseModel):
+class V1AppRuntime(BaseModel):
     """
-    V1ListWorkersResponse
+    V1AppRuntime
     """
-    workers: Optional[List[Appsv1Worker]] = None
-    queue_size: Optional[StrictInt] = Field(default=None, alias="queueSize")
-    queue_name: Optional[StrictStr] = Field(default=None, alias="queueName")
-    last_scale_up_time: Optional[datetime] = Field(default=None, alias="lastScaleUpTime")
-    last_scale_down_delete_time: Optional[datetime] = Field(default=None, alias="lastScaleDownDeleteTime")
-    max_workers: Optional[StrictInt] = Field(default=None, alias="maxWorkers")
-    __properties: ClassVar[List[str]] = ["workers", "queueSize", "queueName", "lastScaleUpTime", "lastScaleDownDeleteTime", "maxWorkers"]
+    app: Optional[V1App] = None
+    workers: Optional[List[V1WorkerRuntime]] = None
+    prefer_revision: Optional[StrictStr] = Field(default=None, alias="preferRevision")
+    max_workers: Optional[StrictInt] = Field(default=None, alias="MaxWorkers")
+    graceful_remove_workers: Optional[StrictBool] = Field(default=None, alias="gracefulRemoveWorkers")
+    rollout_plan: Optional[Dict[str, StrictStr]] = Field(default=None, alias="rolloutPlan")
+    queue: Optional[AppRuntimev1RequestQueue] = None
+    __properties: ClassVar[List[str]] = ["app", "workers", "preferRevision", "MaxWorkers", "gracefulRemoveWorkers", "rolloutPlan", "queue"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True
     }
 
 
@@ -53,15 +56,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of V1ListWorkersResponse from a JSON string"""
+        """Create an instance of V1AppRuntime from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -72,36 +75,43 @@
         """
         _dict = self.model_dump(
             by_alias=True,
             exclude={
             },
             exclude_none=True,
         )
+        # override the default output from pydantic by calling `to_dict()` of app
+        if self.app:
+            _dict['app'] = self.app.to_dict()
         # override the default output from pydantic by calling `to_dict()` of each item in workers (list)
         _items = []
         if self.workers:
             for _item in self.workers:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['workers'] = _items
+        # override the default output from pydantic by calling `to_dict()` of queue
+        if self.queue:
+            _dict['queue'] = self.queue.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> Self:
-        """Create an instance of V1ListWorkersResponse from a dict"""
+        """Create an instance of V1AppRuntime from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "workers": [Appsv1Worker.from_dict(_item) for _item in obj.get("workers")] if obj.get("workers") is not None else None,
-            "queueSize": obj.get("queueSize"),
-            "queueName": obj.get("queueName"),
-            "lastScaleUpTime": obj.get("lastScaleUpTime"),
-            "lastScaleDownDeleteTime": obj.get("lastScaleDownDeleteTime"),
-            "maxWorkers": obj.get("maxWorkers")
+            "app": V1App.from_dict(obj.get("app")) if obj.get("app") is not None else None,
+            "workers": [V1WorkerRuntime.from_dict(_item) for _item in obj.get("workers")] if obj.get("workers") is not None else None,
+            "preferRevision": obj.get("preferRevision"),
+            "MaxWorkers": obj.get("MaxWorkers"),
+            "gracefulRemoveWorkers": obj.get("gracefulRemoveWorkers"),
+            "rolloutPlan": obj.get("rolloutPlan"),
+            "queue": AppRuntimev1RequestQueue.from_dict(obj.get("queue")) if obj.get("queue") is not None else None
         })
         return _obj
```

## Comparing `generated/schedulers/models/v1_volume_status.py` & `generated/apps/models/scale_record_autoscaling_action.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/comm/v1/messages.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
@@ -22,27 +22,25 @@
 
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
 
-class V1VolumeStatus(str, Enum):
+class ScaleRecordAutoscalingAction(str, Enum):
     """
-    V1VolumeStatus
+    ScaleRecordAutoscalingAction
     """
 
     """
     allowed enum values
     """
-    UNKNOWN = 'Unknown'
-    SYNCING = 'Syncing'
-    FAILED = 'Failed'
-    READY = 'Ready'
-    CLEANING = 'Cleaning'
+    AUTOSCALING_ACTION_UNSPECIFIED = 'AUTOSCALING_ACTION_UNSPECIFIED'
+    AUTOSCALING_ACTION_SCALE_UP = 'AUTOSCALING_ACTION_SCALE_UP'
+    AUTOSCALING_ACTION_SCALE_DOWN = 'AUTOSCALING_ACTION_SCALE_DOWN'
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of V1VolumeStatus from a JSON string"""
+        """Create an instance of ScaleRecordAutoscalingAction from a JSON string"""
         return cls(json.loads(json_str))
```

## Comparing `generated/schedulers/models/v1_worker_status.py` & `generated/apps/models/worker_worker_status.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/comm/v1/messages.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
@@ -22,29 +22,30 @@
 
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
 
-class V1WorkerStatus(str, Enum):
+class WorkerWorkerStatus(str, Enum):
     """
-    V1WorkerStatus
+    WorkerWorkerStatus
     """
 
     """
     allowed enum values
     """
-    UNKNOWN = 'Unknown'
-    PREPARING = 'Preparing'
-    STARTING = 'Starting'
-    APPPREPARING = 'AppPreparing'
-    APPRUNNING = 'AppRunning'
-    APPCLEANING = 'AppCleaning'
-    STOPPED = 'Stopped'
+    STATUS_UNSPECIFIED = 'STATUS_UNSPECIFIED'
+    STATUS_INITIALIZED = 'STATUS_INITIALIZED'
+    STATUS_PENDING = 'STATUS_PENDING'
+    STATUS_RUNNING = 'STATUS_RUNNING'
+    STATUS_TERMINATING = 'STATUS_TERMINATING'
+    STATUS_ERROR = 'STATUS_ERROR'
+    STATUS_UNAVAILABLE = 'STATUS_UNAVAILABLE'
+    STATUS_TERMINATED = 'STATUS_TERMINATED'
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of V1WorkerStatus from a JSON string"""
+        """Create an instance of WorkerWorkerStatus from a JSON string"""
         return cls(json.loads(json_str))
```

## Comparing `generated/schedulers/models/worker_worker_detail_status.py` & `generated/apps/models/worker_worker_detail_status.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/comm/v1/messages.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
```

## Comparing `generated/schedulers/test/test_app_service_create_body.py` & `generated/apps/test/test_app_service_create_body.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/register_message.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 import datetime
 
-from generated.schedulers.models.app_service_create_body import AppServiceCreateBody  # noqa: E501
+from generated.apps.models.app_service_create_body import AppServiceCreateBody  # noqa: E501
 
 class TestAppServiceCreateBody(unittest.TestCase):
     """AppServiceCreateBody unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -34,15 +34,16 @@
         # uncomment below to create an instance of `AppServiceCreateBody`
         """
         model = AppServiceCreateBody()  # noqa: E501
         if include_optional:
             return AppServiceCreateBody(
                 labels = {
                     'key' : ''
-                    }
+                    },
+                route_path = ''
             )
         else:
             return AppServiceCreateBody(
         )
         """
 
     def testAppServiceCreateBody(self):
```

## Comparing `generated/schedulers/test/test_app_service_inference_body.py` & `generated/apps/test/test_app_service_protect_app_body.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,57 +1,53 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/comm/v1/messages.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 import datetime
 
-from generated.schedulers.models.app_service_inference_body import AppServiceInferenceBody  # noqa: E501
+from generated.apps.models.app_service_protect_app_body import AppServiceProtectAppBody  # noqa: E501
 
-class TestAppServiceInferenceBody(unittest.TestCase):
-    """AppServiceInferenceBody unit test stubs"""
+class TestAppServiceProtectAppBody(unittest.TestCase):
+    """AppServiceProtectAppBody unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> AppServiceInferenceBody:
-        """Test AppServiceInferenceBody
+    def make_instance(self, include_optional) -> AppServiceProtectAppBody:
+        """Test AppServiceProtectAppBody
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `AppServiceInferenceBody`
+        # uncomment below to create an instance of `AppServiceProtectAppBody`
         """
-        model = AppServiceInferenceBody()  # noqa: E501
+        model = AppServiceProtectAppBody()  # noqa: E501
         if include_optional:
-            return AppServiceInferenceBody(
-                method = '',
-                body = 'YQ==',
-                timeout_time = 56,
-                max_retry_times = 56
+            return AppServiceProtectAppBody(
+                public_key = ''
             )
         else:
-            return AppServiceInferenceBody(
-                timeout_time = 56,
-                max_retry_times = 56,
+            return AppServiceProtectAppBody(
+                public_key = '',
         )
         """
 
-    def testAppServiceInferenceBody(self):
-        """Test AppServiceInferenceBody"""
+    def testAppServiceProtectAppBody(self):
+        """Test AppServiceProtectAppBody"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

## Comparing `generated/schedulers/test/test_app_service_resources_body.py` & `generated/apps/test/test_app_service_setup_resources_body.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,48 +1,49 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/register_message.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
+import datetime
 
-from generated.schedulers.models.app_service_resources_body import AppServiceResourcesBody
+from generated.apps.models.app_service_setup_resources_body import AppServiceSetupResourcesBody  # noqa: E501
 
-class TestAppServiceResourcesBody(unittest.TestCase):
-    """AppServiceResourcesBody unit test stubs"""
+class TestAppServiceSetupResourcesBody(unittest.TestCase):
+    """AppServiceSetupResourcesBody unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> AppServiceResourcesBody:
-        """Test AppServiceResourcesBody
+    def make_instance(self, include_optional) -> AppServiceSetupResourcesBody:
+        """Test AppServiceSetupResourcesBody
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `AppServiceResourcesBody`
+        # uncomment below to create an instance of `AppServiceSetupResourcesBody`
         """
-        model = AppServiceResourcesBody()
+        model = AppServiceSetupResourcesBody()  # noqa: E501
         if include_optional:
-            return AppServiceResourcesBody(
-                resource_claim = generated.schedulers.models.resource_request.resource request(
+            return AppServiceSetupResourcesBody(
+                resource_claim = generated.apps.models.resource_request.resource request(
                     cpu_num = 56, 
                     gpu_num = 56, 
-                    memory_mb = '', 
+                    memory_mb = 56, 
                     region_constraints = [
                         ''
                         ], 
                     cpu_constraints = [
                         ''
                         ], 
                     cpu_architecture = [
@@ -51,19 +52,19 @@
                     gpu_constraints = [
                         ''
                         ], 
                     cuda_constraints = '', 
                     driver_version_constraints = '', )
             )
         else:
-            return AppServiceResourcesBody(
-                resource_claim = generated.schedulers.models.resource_request.resource request(
+            return AppServiceSetupResourcesBody(
+                resource_claim = generated.apps.models.resource_request.resource request(
                     cpu_num = 56, 
                     gpu_num = 56, 
-                    memory_mb = '', 
+                    memory_mb = 56, 
                     region_constraints = [
                         ''
                         ], 
                     cpu_constraints = [
                         ''
                         ], 
                     cpu_architecture = [
@@ -73,14 +74,14 @@
                         ''
                         ], 
                     cuda_constraints = '', 
                     driver_version_constraints = '', ),
         )
         """
 
-    def testAppServiceResourcesBody(self):
-        """Test AppServiceResourcesBody"""
+    def testAppServiceSetupResourcesBody(self):
+        """Test AppServiceSetupResourcesBody"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

## Comparing `generated/schedulers/test/test_app_service_setup_auto_scaling_policy_body.py` & `generated/apps/test/test_app_service_setup_auto_scaling_policy_body.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/register_message.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
+import datetime
 
-from generated.schedulers.models.app_service_setup_auto_scaling_policy_body import AppServiceSetupAutoScalingPolicyBody
+from generated.apps.models.app_service_setup_auto_scaling_policy_body import AppServiceSetupAutoScalingPolicyBody  # noqa: E501
 
 class TestAppServiceSetupAutoScalingPolicyBody(unittest.TestCase):
     """AppServiceSetupAutoScalingPolicyBody unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -28,46 +29,46 @@
     def make_instance(self, include_optional) -> AppServiceSetupAutoScalingPolicyBody:
         """Test AppServiceSetupAutoScalingPolicyBody
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
         # uncomment below to create an instance of `AppServiceSetupAutoScalingPolicyBody`
         """
-        model = AppServiceSetupAutoScalingPolicyBody()
+        model = AppServiceSetupAutoScalingPolicyBody()  # noqa: E501
         if include_optional:
             return AppServiceSetupAutoScalingPolicyBody(
-                auto_scaling_policy = generated.schedulers.models.autoscaling_policy_setting.autoscaling policy setting(
-                    build_in_policy = generated.schedulers.models.v1_build_in_policy.v1BuildInPolicy(
+                auto_scaling_policy = generated.apps.models.autoscaling_policy_setting.autoscaling policy setting(
+                    built_in_policy = generated.apps.models.v1_built_in_policy.v1BuiltInPolicy(
                         min_worker_num = 56, 
                         max_worker_num = 56, 
                         max_queue_num = 56, 
-                        max_idle_time = '', ), 
-                    custom_policy = generated.schedulers.models.v1_custom_policy.v1CustomPolicy(
+                        max_idle_time = 56, ), 
+                    custom_policy = generated.apps.models.v1_custom_policy.v1CustomPolicy(
                         rules = [
-                            generated.schedulers.models.v1_rule.v1Rule(
+                            generated.apps.models.v1_rule.v1Rule(
                                 factor = [
                                     ''
                                     ], 
                                 behavior = 'HOLD_ON', 
                                 custom_func = {
                                     'key' : None
                                     }, )
                             ], ), )
             )
         else:
             return AppServiceSetupAutoScalingPolicyBody(
-                auto_scaling_policy = generated.schedulers.models.autoscaling_policy_setting.autoscaling policy setting(
-                    build_in_policy = generated.schedulers.models.v1_build_in_policy.v1BuildInPolicy(
+                auto_scaling_policy = generated.apps.models.autoscaling_policy_setting.autoscaling policy setting(
+                    built_in_policy = generated.apps.models.v1_built_in_policy.v1BuiltInPolicy(
                         min_worker_num = 56, 
                         max_worker_num = 56, 
                         max_queue_num = 56, 
-                        max_idle_time = '', ), 
-                    custom_policy = generated.schedulers.models.v1_custom_policy.v1CustomPolicy(
+                        max_idle_time = 56, ), 
+                    custom_policy = generated.apps.models.v1_custom_policy.v1CustomPolicy(
                         rules = [
-                            generated.schedulers.models.v1_rule.v1Rule(
+                            generated.apps.models.v1_rule.v1Rule(
                                 factor = [
                                     ''
                                     ], 
                                 behavior = 'HOLD_ON', 
                                 custom_func = {
                                     'key' : None
                                     }, )
```

## Comparing `generated/schedulers/test/test_app_service_setup_secrets_body.py` & `generated/apps/test/test_app_service_setup_secrets_body.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/register_message.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
+import datetime
 
-from generated.schedulers.models.app_service_setup_secrets_body import AppServiceSetupSecretsBody
+from generated.apps.models.app_service_setup_secrets_body import AppServiceSetupSecretsBody  # noqa: E501
 
 class TestAppServiceSetupSecretsBody(unittest.TestCase):
     """AppServiceSetupSecretsBody unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -28,15 +29,15 @@
     def make_instance(self, include_optional) -> AppServiceSetupSecretsBody:
         """Test AppServiceSetupSecretsBody
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
         # uncomment below to create an instance of `AppServiceSetupSecretsBody`
         """
-        model = AppServiceSetupSecretsBody()
+        model = AppServiceSetupSecretsBody()  # noqa: E501
         if include_optional:
             return AppServiceSetupSecretsBody(
                 secret_names = [
                     ''
                     ]
             )
         else:
```

## Comparing `generated/schedulers/test/test_app_service_setup_volumes_body.py` & `generated/apps/test/test_app_service_setup_volumes_body.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/register_message.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
+import datetime
 
-from generated.schedulers.models.app_service_setup_volumes_body import AppServiceSetupVolumesBody
+from generated.apps.models.app_service_setup_volumes_body import AppServiceSetupVolumesBody  # noqa: E501
 
 class TestAppServiceSetupVolumesBody(unittest.TestCase):
     """AppServiceSetupVolumesBody unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -28,29 +29,29 @@
     def make_instance(self, include_optional) -> AppServiceSetupVolumesBody:
         """Test AppServiceSetupVolumesBody
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
         # uncomment below to create an instance of `AppServiceSetupVolumesBody`
         """
-        model = AppServiceSetupVolumesBody()
+        model = AppServiceSetupVolumesBody()  # noqa: E501
         if include_optional:
             return AppServiceSetupVolumesBody(
                 setup_volumes = [
-                    generated.schedulers.models.v1_setup_volume.v1SetupVolume(
+                    generated.apps.models.v1_setup_volume.v1SetupVolume(
                         volume_name = '', 
                         revision = '', 
                         optional = True, 
                         create_if_not_exists = True, )
                     ]
             )
         else:
             return AppServiceSetupVolumesBody(
                 setup_volumes = [
-                    generated.schedulers.models.v1_setup_volume.v1SetupVolume(
+                    generated.apps.models.v1_setup_volume.v1SetupVolume(
                         volume_name = '', 
                         revision = '', 
                         optional = True, 
                         create_if_not_exists = True, )
                     ],
         )
         """
```

## Comparing `generated/schedulers/test/test_appsv1_cpu.py` & `generated/apps/test/test_v1_rule.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,53 +1,58 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/register_message.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 import datetime
 
-from generated.schedulers.models.appsv1_cpu import Appsv1CPU  # noqa: E501
+from generated.apps.models.v1_rule import V1Rule  # noqa: E501
 
-class TestAppsv1CPU(unittest.TestCase):
-    """Appsv1CPU unit test stubs"""
+class TestV1Rule(unittest.TestCase):
+    """V1Rule unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> Appsv1CPU:
-        """Test Appsv1CPU
+    def make_instance(self, include_optional) -> V1Rule:
+        """Test V1Rule
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `Appsv1CPU`
+        # uncomment below to create an instance of `V1Rule`
         """
-        model = Appsv1CPU()  # noqa: E501
+        model = V1Rule()  # noqa: E501
         if include_optional:
-            return Appsv1CPU(
-                cores = 56,
-                architecture = ''
+            return V1Rule(
+                factor = [
+                    ''
+                    ],
+                behavior = 'HOLD_ON',
+                custom_func = {
+                    'key' : None
+                    }
             )
         else:
-            return Appsv1CPU(
+            return V1Rule(
         )
         """
 
-    def testAppsv1CPU(self):
-        """Test Appsv1CPU"""
+    def testV1Rule(self):
+        """Test V1Rule"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

## Comparing `generated/schedulers/test/test_appsv1_gpu.py` & `generated/apps/test/test_v1_scale_record.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,56 +1,53 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/register_message.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 import datetime
 
-from generated.schedulers.models.appsv1_gpu import Appsv1GPU  # noqa: E501
+from generated.apps.models.v1_scale_record import V1ScaleRecord  # noqa: E501
 
-class TestAppsv1GPU(unittest.TestCase):
-    """Appsv1GPU unit test stubs"""
+class TestV1ScaleRecord(unittest.TestCase):
+    """V1ScaleRecord unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> Appsv1GPU:
-        """Test Appsv1GPU
+    def make_instance(self, include_optional) -> V1ScaleRecord:
+        """Test V1ScaleRecord
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `Appsv1GPU`
+        # uncomment below to create an instance of `V1ScaleRecord`
         """
-        model = Appsv1GPU()  # noqa: E501
+        model = V1ScaleRecord()  # noqa: E501
         if include_optional:
-            return Appsv1GPU(
-                model = '',
-                number = '',
-                required_driver_version = '',
-                required_cuda_version = ''
+            return V1ScaleRecord(
+                action = 'AUTOSCALING_ACTION_UNSPECIFIED',
+                message = ''
             )
         else:
-            return Appsv1GPU(
-                model = '',
+            return V1ScaleRecord(
         )
         """
 
-    def testAppsv1GPU(self):
-        """Test Appsv1GPU"""
+    def testV1ScaleRecord(self):
+        """Test V1ScaleRecord"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

## Comparing `generated/schedulers/test/test_appsv1_setup_image.py` & `generated/apps/test/test_appsv1_setup_image.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/register_message.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
+import datetime
 
-from generated.schedulers.models.appsv1_setup_image import Appsv1SetupImage
+from generated.apps.models.appsv1_setup_image import Appsv1SetupImage  # noqa: E501
 
 class TestAppsv1SetupImage(unittest.TestCase):
     """Appsv1SetupImage unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -28,25 +29,25 @@
     def make_instance(self, include_optional) -> Appsv1SetupImage:
         """Test Appsv1SetupImage
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
         # uncomment below to create an instance of `Appsv1SetupImage`
         """
-        model = Appsv1SetupImage()
+        model = Appsv1SetupImage()  # noqa: E501
         if include_optional:
             return Appsv1SetupImage(
                 repository = '',
                 tag = '',
                 digest = '',
-                basic_auth = generated.schedulers.models.v1_basic_auth.v1BasicAuth(
-                    username = generated.schedulers.models.v1_value_from_secret.v1ValueFromSecret(
+                basic_auth = generated.apps.models.v1_basic_auth.v1BasicAuth(
+                    username = generated.apps.models.v1_value_from_secret.v1ValueFromSecret(
                         name = '', 
                         key = '', ), 
-                    password = generated.schedulers.models.v1_value_from_secret.v1ValueFromSecret(
+                    password = generated.apps.models.v1_value_from_secret.v1ValueFromSecret(
                         name = '', 
                         key = '', ), )
             )
         else:
             return Appsv1SetupImage(
                 repository = '',
         )
```

## Comparing `generated/schedulers/test/test_appsv1_worker.py` & `generated/apps/test/test_v1_worker.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,56 +1,73 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/comm/v1/messages.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 import datetime
 
-from generated.schedulers.models.appsv1_worker import Appsv1Worker  # noqa: E501
+from generated.apps.models.v1_worker import V1Worker  # noqa: E501
 
-class TestAppsv1Worker(unittest.TestCase):
-    """Appsv1Worker unit test stubs"""
+class TestV1Worker(unittest.TestCase):
+    """V1Worker unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> Appsv1Worker:
-        """Test Appsv1Worker
+    def make_instance(self, include_optional) -> V1Worker:
+        """Test V1Worker
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `Appsv1Worker`
+        # uncomment below to create an instance of `V1Worker`
         """
-        model = Appsv1Worker()  # noqa: E501
+        model = V1Worker()  # noqa: E501
         if include_optional:
-            return Appsv1Worker(
+            return V1Worker(
                 id = '',
                 device_id = '',
-                status = '',
+                status = 'STATUS_UNSPECIFIED',
+                detail_status = 'DETAIL_STATUS_UNSPECIFIED',
                 created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
-                deleted_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f')
+                deleted_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
+                launch_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
+                last_serve_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
+                success_count = 56,
+                failed_count = 56,
+                session_number = 56,
+                cpus = 56,
+                memory = 56,
+                gpu_name = '',
+                gpus = 56,
+                app_id = '',
+                app_revision = '',
+                replace_worker_id = '',
+                user_id = '',
+                request_id = '',
+                gpu_model = '',
+                gpu_num = 56
             )
         else:
-            return Appsv1Worker(
+            return V1Worker(
         )
         """
 
-    def testAppsv1Worker(self):
-        """Test Appsv1Worker"""
+    def testV1Worker(self):
+        """Test V1Worker"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

## Comparing `generated/schedulers/test/test_list_request_queues_response_queue_reason.py` & `generated/apps/test/test_list_request_queues_response_queue_reason.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/comm/v1/messages.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 import datetime
 
-from generated.schedulers.models.list_request_queues_response_queue_reason import ListRequestQueuesResponseQueueReason  # noqa: E501
+from generated.apps.models.list_request_queues_response_queue_reason import ListRequestQueuesResponseQueueReason  # noqa: E501
 
 class TestListRequestQueuesResponseQueueReason(unittest.TestCase):
     """ListRequestQueuesResponseQueueReason unit test stubs"""
 
     def setUp(self):
         pass
```

## Comparing `generated/schedulers/test/test_list_request_queues_response_request_queue.py` & `generated/apps/test/test_v1_list_request_queues_response_request_queue.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/comm/v1/messages.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 import datetime
 
-from generated.schedulers.models.list_request_queues_response_request_queue import ListRequestQueuesResponseRequestQueue  # noqa: E501
+from generated.apps.models.v1_list_request_queues_response_request_queue import V1ListRequestQueuesResponseRequestQueue  # noqa: E501
 
-class TestListRequestQueuesResponseRequestQueue(unittest.TestCase):
-    """ListRequestQueuesResponseRequestQueue unit test stubs"""
+class TestV1ListRequestQueuesResponseRequestQueue(unittest.TestCase):
+    """V1ListRequestQueuesResponseRequestQueue unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> ListRequestQueuesResponseRequestQueue:
-        """Test ListRequestQueuesResponseRequestQueue
+    def make_instance(self, include_optional) -> V1ListRequestQueuesResponseRequestQueue:
+        """Test V1ListRequestQueuesResponseRequestQueue
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `ListRequestQueuesResponseRequestQueue`
+        # uncomment below to create an instance of `V1ListRequestQueuesResponseRequestQueue`
         """
-        model = ListRequestQueuesResponseRequestQueue()  # noqa: E501
+        model = V1ListRequestQueuesResponseRequestQueue()  # noqa: E501
         if include_optional:
-            return ListRequestQueuesResponseRequestQueue(
+            return V1ListRequestQueuesResponseRequestQueue(
                 index = 56,
                 reason = 'QueueReasonUnspecified',
                 create_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f')
             )
         else:
-            return ListRequestQueuesResponseRequestQueue(
+            return V1ListRequestQueuesResponseRequestQueue(
         )
         """
 
-    def testListRequestQueuesResponseRequestQueue(self):
-        """Test ListRequestQueuesResponseRequestQueue"""
+    def testV1ListRequestQueuesResponseRequestQueue(self):
+        """Test V1ListRequestQueuesResponseRequestQueue"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

## Comparing `generated/schedulers/test/test_protobuf_any.py` & `generated/apps/test/test_protobuf_any.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/register_message.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 import datetime
 
-from generated.schedulers.models.protobuf_any import ProtobufAny  # noqa: E501
+from generated.apps.models.protobuf_any import ProtobufAny  # noqa: E501
 
 class TestProtobufAny(unittest.TestCase):
     """ProtobufAny unit test stubs"""
 
     def setUp(self):
         pass
```

## Comparing `generated/schedulers/test/test_rule_behavior.py` & `generated/apps/test/test_rule_behavior.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/register_message.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 import datetime
 
-from generated.schedulers.models.rule_behavior import RuleBehavior  # noqa: E501
+from generated.apps.models.rule_behavior import RuleBehavior  # noqa: E501
 
 class TestRuleBehavior(unittest.TestCase):
     """RuleBehavior unit test stubs"""
 
     def setUp(self):
         pass
```

## Comparing `generated/schedulers/test/test_schedulerv1_cpu.py` & `generated/apps/test/test_v1_built_in_policy.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,56 +1,55 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/register_message.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 import datetime
 
-from generated.schedulers.models.schedulerv1_cpu import Schedulerv1CPU  # noqa: E501
+from generated.apps.models.v1_built_in_policy import V1BuiltInPolicy  # noqa: E501
 
-class TestSchedulerv1CPU(unittest.TestCase):
-    """Schedulerv1CPU unit test stubs"""
+class TestV1BuiltInPolicy(unittest.TestCase):
+    """V1BuiltInPolicy unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> Schedulerv1CPU:
-        """Test Schedulerv1CPU
+    def make_instance(self, include_optional) -> V1BuiltInPolicy:
+        """Test V1BuiltInPolicy
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `Schedulerv1CPU`
+        # uncomment below to create an instance of `V1BuiltInPolicy`
         """
-        model = Schedulerv1CPU()  # noqa: E501
+        model = V1BuiltInPolicy()  # noqa: E501
         if include_optional:
-            return Schedulerv1CPU(
-                model = '',
-                cores = 56,
-                threads = 56,
-                architecture = '',
-                cpu_num = 56
+            return V1BuiltInPolicy(
+                min_worker_num = 56,
+                max_worker_num = 56,
+                max_queue_num = 56,
+                max_idle_time = 56
             )
         else:
-            return Schedulerv1CPU(
+            return V1BuiltInPolicy(
         )
         """
 
-    def testSchedulerv1CPU(self):
-        """Test Schedulerv1CPU"""
+    def testV1BuiltInPolicy(self):
+        """Test V1BuiltInPolicy"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

## Comparing `generated/schedulers/test/test_schedulerv1_gpu.py` & `generated/apps/test/test_v1_get_route_path_response.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,59 +1,54 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/register_message.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 import datetime
 
-from generated.schedulers.models.schedulerv1_gpu import Schedulerv1GPU  # noqa: E501
+from generated.apps.models.v1_get_route_path_response import V1GetRoutePathResponse  # noqa: E501
 
-class TestSchedulerv1GPU(unittest.TestCase):
-    """Schedulerv1GPU unit test stubs"""
+class TestV1GetRoutePathResponse(unittest.TestCase):
+    """V1GetRoutePathResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> Schedulerv1GPU:
-        """Test Schedulerv1GPU
+    def make_instance(self, include_optional) -> V1GetRoutePathResponse:
+        """Test V1GetRoutePathResponse
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `Schedulerv1GPU`
+        # uncomment below to create an instance of `V1GetRoutePathResponse`
         """
-        model = Schedulerv1GPU()  # noqa: E501
+        model = V1GetRoutePathResponse()  # noqa: E501
         if include_optional:
-            return Schedulerv1GPU(
-                model = '',
-                driver_version = '',
-                cuda_version = '',
-                memory = generated.schedulers.models.v1_storage_size.v1StorageSize(
-                    size = '', 
-                    unit = '', ),
-                power = '',
-                gpu_num = 56
+            return V1GetRoutePathResponse(
+                paths = [
+                    ''
+                    ]
             )
         else:
-            return Schedulerv1GPU(
+            return V1GetRoutePathResponse(
         )
         """
 
-    def testSchedulerv1GPU(self):
-        """Test Schedulerv1GPU"""
+    def testV1GetRoutePathResponse(self):
+        """Test V1GetRoutePathResponse"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

## Comparing `generated/schedulers/test/test_v1_app.py` & `generated/apps/test/test_v1_setup_volume.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,60 +1,56 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/register_message.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 import datetime
 
-from generated.schedulers.models.v1_app import V1App  # noqa: E501
+from generated.apps.models.v1_setup_volume import V1SetupVolume  # noqa: E501
 
-class TestV1App(unittest.TestCase):
-    """V1App unit test stubs"""
+class TestV1SetupVolume(unittest.TestCase):
+    """V1SetupVolume unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> V1App:
-        """Test V1App
+    def make_instance(self, include_optional) -> V1SetupVolume:
+        """Test V1SetupVolume
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `V1App`
+        # uncomment below to create an instance of `V1SetupVolume`
         """
-        model = V1App()  # noqa: E501
+        model = V1SetupVolume()  # noqa: E501
         if include_optional:
-            return V1App(
-                id = '',
-                name = '',
-                user_id = '',
-                route_path = '',
-                created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
-                modified_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
-                labels = {
-                    'key' : ''
-                    }
+            return V1SetupVolume(
+                volume_name = '',
+                revision = '',
+                optional = True,
+                create_if_not_exists = True
             )
         else:
-            return V1App(
+            return V1SetupVolume(
+                volume_name = '',
         )
         """
 
-    def testV1App(self):
-        """Test V1App"""
+    def testV1SetupVolume(self):
+        """Test V1SetupVolume"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

## Comparing `generated/schedulers/test/test_v1_app_service_setup_image_body.py` & `generated/apps/test/test_v1_app_service_setup_image_body.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/register_message.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
+import datetime
 
-from generated.schedulers.models.v1_app_service_setup_image_body import V1AppServiceSetupImageBody
+from generated.apps.models.v1_app_service_setup_image_body import V1AppServiceSetupImageBody  # noqa: E501
 
 class TestV1AppServiceSetupImageBody(unittest.TestCase):
     """V1AppServiceSetupImageBody unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -28,40 +29,40 @@
     def make_instance(self, include_optional) -> V1AppServiceSetupImageBody:
         """Test V1AppServiceSetupImageBody
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
         # uncomment below to create an instance of `V1AppServiceSetupImageBody`
         """
-        model = V1AppServiceSetupImageBody()
+        model = V1AppServiceSetupImageBody()  # noqa: E501
         if include_optional:
             return V1AppServiceSetupImageBody(
-                setup_image = generated.schedulers.models.image_setting.image setting(
+                setup_image = generated.apps.models.image_setting.image setting(
                     repository = '', 
                     tag = '', 
                     digest = '', 
-                    basic_auth = generated.schedulers.models.v1_basic_auth.v1BasicAuth(
-                        username = generated.schedulers.models.v1_value_from_secret.v1ValueFromSecret(
+                    basic_auth = generated.apps.models.v1_basic_auth.v1BasicAuth(
+                        username = generated.apps.models.v1_value_from_secret.v1ValueFromSecret(
                             name = '', 
                             key = '', ), 
-                        password = generated.schedulers.models.v1_value_from_secret.v1ValueFromSecret(
+                        password = generated.apps.models.v1_value_from_secret.v1ValueFromSecret(
                             name = '', 
                             key = '', ), ), )
             )
         else:
             return V1AppServiceSetupImageBody(
-                setup_image = generated.schedulers.models.image_setting.image setting(
+                setup_image = generated.apps.models.image_setting.image setting(
                     repository = '', 
                     tag = '', 
                     digest = '', 
-                    basic_auth = generated.schedulers.models.v1_basic_auth.v1BasicAuth(
-                        username = generated.schedulers.models.v1_value_from_secret.v1ValueFromSecret(
+                    basic_auth = generated.apps.models.v1_basic_auth.v1BasicAuth(
+                        username = generated.apps.models.v1_value_from_secret.v1ValueFromSecret(
                             name = '', 
                             key = '', ), 
-                        password = generated.schedulers.models.v1_value_from_secret.v1ValueFromSecret(
+                        password = generated.apps.models.v1_value_from_secret.v1ValueFromSecret(
                             name = '', 
                             key = '', ), ), ),
         )
         """
 
     def testV1AppServiceSetupImageBody(self):
         """Test V1AppServiceSetupImageBody"""
```

## Comparing `generated/schedulers/test/test_v1_app_status.py` & `generated/apps/test/test_app_route_auth_status.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/register_message.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 import datetime
 
-from generated.schedulers.models.v1_app_status import V1AppStatus  # noqa: E501
+from generated.apps.models.app_route_auth_status import AppRouteAuthStatus  # noqa: E501
 
-class TestV1AppStatus(unittest.TestCase):
-    """V1AppStatus unit test stubs"""
+class TestAppRouteAuthStatus(unittest.TestCase):
+    """AppRouteAuthStatus unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testV1AppStatus(self):
-        """Test V1AppStatus"""
-        # inst = V1AppStatus()
+    def testAppRouteAuthStatus(self):
+        """Test AppRouteAuthStatus"""
+        # inst = AppRouteAuthStatus()
 
 if __name__ == '__main__':
     unittest.main()
```

## Comparing `generated/schedulers/test/test_v1_autoscaling_policy.py` & `generated/apps/test/test_v1_basic_auth.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,65 +1,57 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/register_message.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 import datetime
 
-from generated.schedulers.models.v1_autoscaling_policy import V1AutoscalingPolicy  # noqa: E501
+from generated.apps.models.v1_basic_auth import V1BasicAuth  # noqa: E501
 
-class TestV1AutoscalingPolicy(unittest.TestCase):
-    """V1AutoscalingPolicy unit test stubs"""
+class TestV1BasicAuth(unittest.TestCase):
+    """V1BasicAuth unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> V1AutoscalingPolicy:
-        """Test V1AutoscalingPolicy
+    def make_instance(self, include_optional) -> V1BasicAuth:
+        """Test V1BasicAuth
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `V1AutoscalingPolicy`
+        # uncomment below to create an instance of `V1BasicAuth`
         """
-        model = V1AutoscalingPolicy()  # noqa: E501
+        model = V1BasicAuth()  # noqa: E501
         if include_optional:
-            return V1AutoscalingPolicy(
-                build_in_policy = generated.schedulers.models.v1_build_in_policy.v1BuildInPolicy(
-                    min_workers = 56, 
-                    max_workers = 56, ),
-                custom_policy = generated.schedulers.models.v1_custom_policy.v1CustomPolicy(
-                    rules = [
-                        generated.schedulers.models.v1_rule.v1Rule(
-                            factor = [
-                                ''
-                                ], 
-                            behavior = 'HOLD_ON', 
-                            custom_func = {
-                                'key' : None
-                                }, )
-                        ], )
+            return V1BasicAuth(
+                username = generated.apps.models.v1_value_from_secret.v1ValueFromSecret(
+                    name = '', 
+                    key = '', ),
+                password = generated.apps.models.v1_value_from_secret.v1ValueFromSecret(
+                    name = '', 
+                    key = '', )
             )
         else:
-            return V1AutoscalingPolicy(
+            return V1BasicAuth(
         )
         """
 
-    def testV1AutoscalingPolicy(self):
-        """Test V1AutoscalingPolicy"""
+    def testV1BasicAuth(self):
+        """Test V1BasicAuth"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

## Comparing `generated/schedulers/test/test_v1_bandwidth_size.py` & `generated/apps/test/test_v1_resource_claim.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,54 +1,68 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/register_message.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 import datetime
 
-from generated.schedulers.models.v1_bandwidth_size import V1BandwidthSize  # noqa: E501
+from generated.apps.models.v1_resource_claim import V1ResourceClaim  # noqa: E501
 
-class TestV1BandwidthSize(unittest.TestCase):
-    """V1BandwidthSize unit test stubs"""
+class TestV1ResourceClaim(unittest.TestCase):
+    """V1ResourceClaim unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> V1BandwidthSize:
-        """Test V1BandwidthSize
+    def make_instance(self, include_optional) -> V1ResourceClaim:
+        """Test V1ResourceClaim
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `V1BandwidthSize`
+        # uncomment below to create an instance of `V1ResourceClaim`
         """
-        model = V1BandwidthSize()  # noqa: E501
+        model = V1ResourceClaim()  # noqa: E501
         if include_optional:
-            return V1BandwidthSize(
-                size = '',
-                unit = ''
+            return V1ResourceClaim(
+                cpu_num = 56,
+                gpu_num = 56,
+                memory_mb = 56,
+                region_constraints = [
+                    ''
+                    ],
+                cpu_constraints = [
+                    ''
+                    ],
+                cpu_architecture = [
+                    ''
+                    ],
+                gpu_constraints = [
+                    ''
+                    ],
+                cuda_constraints = '',
+                driver_version_constraints = ''
             )
         else:
-            return V1BandwidthSize(
-                unit = '',
+            return V1ResourceClaim(
         )
         """
 
-    def testV1BandwidthSize(self):
-        """Test V1BandwidthSize"""
+    def testV1ResourceClaim(self):
+        """Test V1ResourceClaim"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

## Comparing `generated/schedulers/test/test_v1_basic_auth.py` & `generated/apps/test/test_v1_get_safety_remove_workers_response.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,53 +1,54 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/register_message.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 import datetime
 
-from generated.schedulers.models.v1_basic_auth import V1BasicAuth  # noqa: E501
+from generated.apps.models.v1_get_safety_remove_workers_response import V1GetSafetyRemoveWorkersResponse  # noqa: E501
 
-class TestV1BasicAuth(unittest.TestCase):
-    """V1BasicAuth unit test stubs"""
+class TestV1GetSafetyRemoveWorkersResponse(unittest.TestCase):
+    """V1GetSafetyRemoveWorkersResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> V1BasicAuth:
-        """Test V1BasicAuth
+    def make_instance(self, include_optional) -> V1GetSafetyRemoveWorkersResponse:
+        """Test V1GetSafetyRemoveWorkersResponse
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `V1BasicAuth`
+        # uncomment below to create an instance of `V1GetSafetyRemoveWorkersResponse`
         """
-        model = V1BasicAuth()  # noqa: E501
+        model = V1GetSafetyRemoveWorkersResponse()  # noqa: E501
         if include_optional:
-            return V1BasicAuth(
-                username = '',
-                password = ''
+            return V1GetSafetyRemoveWorkersResponse(
+                workers = [
+                    ''
+                    ]
             )
         else:
-            return V1BasicAuth(
+            return V1GetSafetyRemoveWorkersResponse(
         )
         """
 
-    def testV1BasicAuth(self):
-        """Test V1BasicAuth"""
+    def testV1GetSafetyRemoveWorkersResponse(self):
+        """Test V1GetSafetyRemoveWorkersResponse"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

## Comparing `generated/schedulers/test/test_v1_built_in_policy.py` & `generated/apps/test/test_v1_value_from_secret.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,54 +1,53 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/register_message.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
+import datetime
 
-from generated.schedulers.models.v1_built_in_policy import V1BuiltInPolicy
+from generated.apps.models.v1_value_from_secret import V1ValueFromSecret  # noqa: E501
 
-class TestV1BuiltInPolicy(unittest.TestCase):
-    """V1BuiltInPolicy unit test stubs"""
+class TestV1ValueFromSecret(unittest.TestCase):
+    """V1ValueFromSecret unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> V1BuiltInPolicy:
-        """Test V1BuiltInPolicy
+    def make_instance(self, include_optional) -> V1ValueFromSecret:
+        """Test V1ValueFromSecret
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `V1BuiltInPolicy`
+        # uncomment below to create an instance of `V1ValueFromSecret`
         """
-        model = V1BuiltInPolicy()
+        model = V1ValueFromSecret()  # noqa: E501
         if include_optional:
-            return V1BuiltInPolicy(
-                min_worker_num = 56,
-                max_worker_num = 56,
-                max_queue_num = 56,
-                max_idle_time = ''
+            return V1ValueFromSecret(
+                name = '',
+                key = ''
             )
         else:
-            return V1BuiltInPolicy(
+            return V1ValueFromSecret(
         )
         """
 
-    def testV1BuiltInPolicy(self):
-        """Test V1BuiltInPolicy"""
+    def testV1ValueFromSecret(self):
+        """Test V1ValueFromSecret"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

## Comparing `generated/schedulers/test/test_v1_cpu.py` & `generated/apps/test/test_v1_custom_policy.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,56 +1,61 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/register_message.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 import datetime
 
-from generated.schedulers.models.v1_cpu import V1CPU  # noqa: E501
+from generated.apps.models.v1_custom_policy import V1CustomPolicy  # noqa: E501
 
-class TestV1CPU(unittest.TestCase):
-    """V1CPU unit test stubs"""
+class TestV1CustomPolicy(unittest.TestCase):
+    """V1CustomPolicy unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> V1CPU:
-        """Test V1CPU
+    def make_instance(self, include_optional) -> V1CustomPolicy:
+        """Test V1CustomPolicy
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `V1CPU`
+        # uncomment below to create an instance of `V1CustomPolicy`
         """
-        model = V1CPU()  # noqa: E501
+        model = V1CustomPolicy()  # noqa: E501
         if include_optional:
-            return V1CPU(
-                model = '',
-                cores = 56,
-                threads = 56,
-                architecture = '',
-                cpu_num = 56
+            return V1CustomPolicy(
+                rules = [
+                    generated.apps.models.v1_rule.v1Rule(
+                        factor = [
+                            ''
+                            ], 
+                        behavior = 'HOLD_ON', 
+                        custom_func = {
+                            'key' : None
+                            }, )
+                    ]
             )
         else:
-            return V1CPU(
+            return V1CustomPolicy(
         )
         """
 
-    def testV1CPU(self):
-        """Test V1CPU"""
+    def testV1CustomPolicy(self):
+        """Test V1CustomPolicy"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

## Comparing `generated/schedulers/test/test_v1_create_volume_response.py` & `generated/apps/test/test_v1_autoscaling_policy.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,58 +1,67 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/register_message.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 import datetime
 
-from generated.schedulers.models.v1_create_volume_response import V1CreateVolumeResponse  # noqa: E501
+from generated.apps.models.v1_autoscaling_policy import V1AutoscalingPolicy  # noqa: E501
 
-class TestV1CreateVolumeResponse(unittest.TestCase):
-    """V1CreateVolumeResponse unit test stubs"""
+class TestV1AutoscalingPolicy(unittest.TestCase):
+    """V1AutoscalingPolicy unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> V1CreateVolumeResponse:
-        """Test V1CreateVolumeResponse
+    def make_instance(self, include_optional) -> V1AutoscalingPolicy:
+        """Test V1AutoscalingPolicy
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `V1CreateVolumeResponse`
+        # uncomment below to create an instance of `V1AutoscalingPolicy`
         """
-        model = V1CreateVolumeResponse()  # noqa: E501
+        model = V1AutoscalingPolicy()  # noqa: E501
         if include_optional:
-            return V1CreateVolumeResponse(
-                retcode = '',
-                message = '',
-                volume = generated.schedulers.models.volumesv1_volume.volumesv1Volume(
-                    deployment_id = '', 
-                    name = '', 
-                    path = '', 
-                    size = '', )
+            return V1AutoscalingPolicy(
+                built_in_policy = generated.apps.models.v1_built_in_policy.v1BuiltInPolicy(
+                    min_worker_num = 56, 
+                    max_worker_num = 56, 
+                    max_queue_num = 56, 
+                    max_idle_time = 56, ),
+                custom_policy = generated.apps.models.v1_custom_policy.v1CustomPolicy(
+                    rules = [
+                        generated.apps.models.v1_rule.v1Rule(
+                            factor = [
+                                ''
+                                ], 
+                            behavior = 'HOLD_ON', 
+                            custom_func = {
+                                'key' : None
+                                }, )
+                        ], )
             )
         else:
-            return V1CreateVolumeResponse(
+            return V1AutoscalingPolicy(
         )
         """
 
-    def testV1CreateVolumeResponse(self):
-        """Test V1CreateVolumeResponse"""
+    def testV1AutoscalingPolicy(self):
+        """Test V1AutoscalingPolicy"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

## Comparing `generated/schedulers/test/test_v1_custom_policy.py` & `generated/apps/test/test_app_runtimev1_request_queue.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,61 +1,53 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/register_message.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 import datetime
 
-from generated.schedulers.models.v1_custom_policy import V1CustomPolicy  # noqa: E501
+from generated.apps.models.app_runtimev1_request_queue import AppRuntimev1RequestQueue  # noqa: E501
 
-class TestV1CustomPolicy(unittest.TestCase):
-    """V1CustomPolicy unit test stubs"""
+class TestAppRuntimev1RequestQueue(unittest.TestCase):
+    """AppRuntimev1RequestQueue unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> V1CustomPolicy:
-        """Test V1CustomPolicy
+    def make_instance(self, include_optional) -> AppRuntimev1RequestQueue:
+        """Test AppRuntimev1RequestQueue
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `V1CustomPolicy`
+        # uncomment below to create an instance of `AppRuntimev1RequestQueue`
         """
-        model = V1CustomPolicy()  # noqa: E501
+        model = AppRuntimev1RequestQueue()  # noqa: E501
         if include_optional:
-            return V1CustomPolicy(
-                rules = [
-                    generated.schedulers.models.v1_rule.v1Rule(
-                        factor = [
-                            ''
-                            ], 
-                        behavior = 'HOLD_ON', 
-                        custom_func = {
-                            'key' : None
-                            }, )
-                    ]
+            return AppRuntimev1RequestQueue(
+                size = 56,
+                q_name = ''
             )
         else:
-            return V1CustomPolicy(
+            return AppRuntimev1RequestQueue(
         )
         """
 
-    def testV1CustomPolicy(self):
-        """Test V1CustomPolicy"""
+    def testAppRuntimev1RequestQueue(self):
+        """Test AppRuntimev1RequestQueue"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

## Comparing `generated/schedulers/test/test_v1_empty_response.py` & `generated/apps/test/test_v1_list_request_queues_response.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,53 +1,57 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/register_message.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 import datetime
 
-from generated.schedulers.models.v1_empty_response import V1EmptyResponse  # noqa: E501
+from generated.apps.models.v1_list_request_queues_response import V1ListRequestQueuesResponse  # noqa: E501
 
-class TestV1EmptyResponse(unittest.TestCase):
-    """V1EmptyResponse unit test stubs"""
+class TestV1ListRequestQueuesResponse(unittest.TestCase):
+    """V1ListRequestQueuesResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> V1EmptyResponse:
-        """Test V1EmptyResponse
+    def make_instance(self, include_optional) -> V1ListRequestQueuesResponse:
+        """Test V1ListRequestQueuesResponse
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `V1EmptyResponse`
+        # uncomment below to create an instance of `V1ListRequestQueuesResponse`
         """
-        model = V1EmptyResponse()  # noqa: E501
+        model = V1ListRequestQueuesResponse()  # noqa: E501
         if include_optional:
-            return V1EmptyResponse(
-                request_id = ''
+            return V1ListRequestQueuesResponse(
+                queues = [
+                    generated.apps.models.v1_list_request_queues_response_request_queue.v1ListRequestQueuesResponseRequestQueue(
+                        index = 56, 
+                        reason = 'QueueReasonUnspecified', 
+                        create_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), )
+                    ]
             )
         else:
-            return V1EmptyResponse(
-                request_id = '',
+            return V1ListRequestQueuesResponse(
         )
         """
 
-    def testV1EmptyResponse(self):
-        """Test V1EmptyResponse"""
+    def testV1ListRequestQueuesResponse(self):
+        """Test V1ListRequestQueuesResponse"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

## Comparing `generated/schedulers/test/test_v1_get_image_request.py` & `generated/apps/test/test_v1_worker_runtime.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,55 +1,62 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/register_message.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 import datetime
 
-from generated.schedulers.models.v1_get_image_request import V1GetImageRequest  # noqa: E501
+from generated.apps.models.v1_worker_runtime import V1WorkerRuntime  # noqa: E501
 
-class TestV1GetImageRequest(unittest.TestCase):
-    """V1GetImageRequest unit test stubs"""
+class TestV1WorkerRuntime(unittest.TestCase):
+    """V1WorkerRuntime unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> V1GetImageRequest:
-        """Test V1GetImageRequest
+    def make_instance(self, include_optional) -> V1WorkerRuntime:
+        """Test V1WorkerRuntime
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `V1GetImageRequest`
+        # uncomment below to create an instance of `V1WorkerRuntime`
         """
-        model = V1GetImageRequest()  # noqa: E501
+        model = V1WorkerRuntime()  # noqa: E501
         if include_optional:
-            return V1GetImageRequest(
-                request_id = '',
-                repository = ''
+            return V1WorkerRuntime(
+                worker_id = '',
+                device_id = '',
+                revision = '',
+                launch_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
+                last_serve_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
+                success_count = '',
+                failed_count = '',
+                replace_worker_id = '',
+                status = 'STATUS_UNSPECIFIED',
+                detail_status = 'DETAIL_STATUS_UNSPECIFIED',
+                number_of_sessions = 56
             )
         else:
-            return V1GetImageRequest(
-                request_id = '',
-                repository = '',
+            return V1WorkerRuntime(
         )
         """
 
-    def testV1GetImageRequest(self):
-        """Test V1GetImageRequest"""
+    def testV1WorkerRuntime(self):
+        """Test V1WorkerRuntime"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

## Comparing `generated/schedulers/test/test_v1_get_image_response.py` & `generated/apps/test/test_v1_check_and_lock_worker_response.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,67 +1,75 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/register_message.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 import datetime
 
-from generated.schedulers.models.v1_get_image_response import V1GetImageResponse  # noqa: E501
+from generated.apps.models.v1_check_and_lock_worker_response import V1CheckAndLockWorkerResponse  # noqa: E501
 
-class TestV1GetImageResponse(unittest.TestCase):
-    """V1GetImageResponse unit test stubs"""
+class TestV1CheckAndLockWorkerResponse(unittest.TestCase):
+    """V1CheckAndLockWorkerResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> V1GetImageResponse:
-        """Test V1GetImageResponse
+    def make_instance(self, include_optional) -> V1CheckAndLockWorkerResponse:
+        """Test V1CheckAndLockWorkerResponse
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `V1GetImageResponse`
+        # uncomment below to create an instance of `V1CheckAndLockWorkerResponse`
         """
-        model = V1GetImageResponse()  # noqa: E501
+        model = V1CheckAndLockWorkerResponse()  # noqa: E501
         if include_optional:
-            return V1GetImageResponse(
-                request_id = '',
-                image = generated.schedulers.models.v1_image.v1Image(
+            return V1CheckAndLockWorkerResponse(
+                is_distributed = True,
+                worker = generated.apps.models.v1_worker.v1Worker(
                     id = '', 
-                    repository = '', 
-                    tag = '', 
-                    digest = '', 
-                    timestep = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                    size = '', 
-                    status = 'Pulling', 
-                    reference_users = [
-                        ''
-                        ], 
-                    reference_apps = [
-                        ''
-                        ], )
+                    device_id = '', 
+                    status = 'STATUS_UNSPECIFIED', 
+                    detail_status = 'DETAIL_STATUS_UNSPECIFIED', 
+                    created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                    deleted_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                    launch_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                    last_serve_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                    success_count = 56, 
+                    failed_count = 56, 
+                    session_number = 56, 
+                    cpus = 56, 
+                    memory = 56, 
+                    gpu_name = '', 
+                    gpus = 56, 
+                    app_id = '', 
+                    app_revision = '', 
+                    replace_worker_id = '', 
+                    user_id = '', 
+                    request_id = '', 
+                    gpu_model = '', 
+                    gpu_num = 56, )
             )
         else:
-            return V1GetImageResponse(
-                request_id = '',
+            return V1CheckAndLockWorkerResponse(
         )
         """
 
-    def testV1GetImageResponse(self):
-        """Test V1GetImageResponse"""
+    def testV1CheckAndLockWorkerResponse(self):
+        """Test V1CheckAndLockWorkerResponse"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

## Comparing `generated/schedulers/test/test_v1_image.py` & `generated/apps/test/test_v1_list_all_workers_response.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,68 +1,76 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/register_message.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 import datetime
 
-from generated.schedulers.models.v1_image import V1Image  # noqa: E501
+from generated.apps.models.v1_list_all_workers_response import V1ListAllWorkersResponse  # noqa: E501
 
-class TestV1Image(unittest.TestCase):
-    """V1Image unit test stubs"""
+class TestV1ListAllWorkersResponse(unittest.TestCase):
+    """V1ListAllWorkersResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> V1Image:
-        """Test V1Image
+    def make_instance(self, include_optional) -> V1ListAllWorkersResponse:
+        """Test V1ListAllWorkersResponse
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `V1Image`
+        # uncomment below to create an instance of `V1ListAllWorkersResponse`
         """
-        model = V1Image()  # noqa: E501
+        model = V1ListAllWorkersResponse()  # noqa: E501
         if include_optional:
-            return V1Image(
-                id = '',
-                repository = '',
-                tag = '',
-                digest = '',
-                timestep = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
-                size = '',
-                status = 'Pulling',
-                reference_users = [
-                    ''
-                    ],
-                reference_apps = [
-                    ''
+            return V1ListAllWorkersResponse(
+                workers = [
+                    generated.apps.models.v1_worker.v1Worker(
+                        id = '', 
+                        device_id = '', 
+                        status = 'STATUS_UNSPECIFIED', 
+                        detail_status = 'DETAIL_STATUS_UNSPECIFIED', 
+                        created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                        deleted_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                        launch_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                        last_serve_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                        success_count = 56, 
+                        failed_count = 56, 
+                        session_number = 56, 
+                        cpus = 56, 
+                        memory = 56, 
+                        gpu_name = '', 
+                        gpus = 56, 
+                        app_id = '', 
+                        app_revision = '', 
+                        replace_worker_id = '', 
+                        user_id = '', 
+                        request_id = '', 
+                        gpu_model = '', 
+                        gpu_num = 56, )
                     ]
             )
         else:
-            return V1Image(
-                id = '',
-                repository = '',
-                timestep = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
-                size = '',
+            return V1ListAllWorkersResponse(
         )
         """
 
-    def testV1Image(self):
-        """Test V1Image"""
+    def testV1ListAllWorkersResponse(self):
+        """Test V1ListAllWorkersResponse"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

## Comparing `generated/schedulers/test/test_v1_image_status.py` & `generated/apps/test/test_v1_app_status.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/register_message.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 import datetime
 
-from generated.schedulers.models.v1_image_status import V1ImageStatus  # noqa: E501
+from generated.apps.models.v1_app_status import V1AppStatus  # noqa: E501
 
-class TestV1ImageStatus(unittest.TestCase):
-    """V1ImageStatus unit test stubs"""
+class TestV1AppStatus(unittest.TestCase):
+    """V1AppStatus unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testV1ImageStatus(self):
-        """Test V1ImageStatus"""
-        # inst = V1ImageStatus()
+    def testV1AppStatus(self):
+        """Test V1AppStatus"""
+        # inst = V1AppStatus()
 
 if __name__ == '__main__':
     unittest.main()
```

## Comparing `generated/schedulers/test/test_v1_list_image_response.py` & `generated/apps/test/test_v1_list_worker_details_response.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,69 +1,76 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/register_message.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 import datetime
 
-from generated.schedulers.models.v1_list_image_response import V1ListImageResponse  # noqa: E501
+from generated.apps.models.v1_list_worker_details_response import V1ListWorkerDetailsResponse  # noqa: E501
 
-class TestV1ListImageResponse(unittest.TestCase):
-    """V1ListImageResponse unit test stubs"""
+class TestV1ListWorkerDetailsResponse(unittest.TestCase):
+    """V1ListWorkerDetailsResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> V1ListImageResponse:
-        """Test V1ListImageResponse
+    def make_instance(self, include_optional) -> V1ListWorkerDetailsResponse:
+        """Test V1ListWorkerDetailsResponse
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `V1ListImageResponse`
+        # uncomment below to create an instance of `V1ListWorkerDetailsResponse`
         """
-        model = V1ListImageResponse()  # noqa: E501
+        model = V1ListWorkerDetailsResponse()  # noqa: E501
         if include_optional:
-            return V1ListImageResponse(
-                request_id = '',
-                images = [
-                    generated.schedulers.models.v1_image.v1Image(
+            return V1ListWorkerDetailsResponse(
+                workers = [
+                    generated.apps.models.v1_worker.v1Worker(
                         id = '', 
-                        repository = '', 
-                        tag = '', 
-                        digest = '', 
-                        timestep = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                        size = '', 
-                        status = 'Pulling', 
-                        reference_users = [
-                            ''
-                            ], 
-                        reference_apps = [
-                            ''
-                            ], )
+                        device_id = '', 
+                        status = 'STATUS_UNSPECIFIED', 
+                        detail_status = 'DETAIL_STATUS_UNSPECIFIED', 
+                        created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                        deleted_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                        launch_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                        last_serve_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                        success_count = 56, 
+                        failed_count = 56, 
+                        session_number = 56, 
+                        cpus = 56, 
+                        memory = 56, 
+                        gpu_name = '', 
+                        gpus = 56, 
+                        app_id = '', 
+                        app_revision = '', 
+                        replace_worker_id = '', 
+                        user_id = '', 
+                        request_id = '', 
+                        gpu_model = '', 
+                        gpu_num = 56, )
                     ]
             )
         else:
-            return V1ListImageResponse(
-                request_id = '',
+            return V1ListWorkerDetailsResponse(
         )
         """
 
-    def testV1ListImageResponse(self):
-        """Test V1ListImageResponse"""
+    def testV1ListWorkerDetailsResponse(self):
+        """Test V1ListWorkerDetailsResponse"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

## Comparing `generated/schedulers/test/test_v1_list_response.py` & `generated/apps/test/test_v1_list_workers_by_app_and_user_response.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,63 +1,76 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/register_message.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 import datetime
 
-from generated.schedulers.models.v1_list_response import V1ListResponse  # noqa: E501
+from generated.apps.models.v1_list_workers_by_app_and_user_response import V1ListWorkersByAppAndUserResponse  # noqa: E501
 
-class TestV1ListResponse(unittest.TestCase):
-    """V1ListResponse unit test stubs"""
+class TestV1ListWorkersByAppAndUserResponse(unittest.TestCase):
+    """V1ListWorkersByAppAndUserResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> V1ListResponse:
-        """Test V1ListResponse
+    def make_instance(self, include_optional) -> V1ListWorkersByAppAndUserResponse:
+        """Test V1ListWorkersByAppAndUserResponse
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `V1ListResponse`
+        # uncomment below to create an instance of `V1ListWorkersByAppAndUserResponse`
         """
-        model = V1ListResponse()  # noqa: E501
+        model = V1ListWorkersByAppAndUserResponse()  # noqa: E501
         if include_optional:
-            return V1ListResponse(
-                apps = [
-                    generated.schedulers.models.v1_app.v1App(
+            return V1ListWorkersByAppAndUserResponse(
+                workers = [
+                    generated.apps.models.v1_worker.v1Worker(
                         id = '', 
-                        name = '', 
-                        user_id = '', 
-                        route_path = '', 
+                        device_id = '', 
+                        status = 'STATUS_UNSPECIFIED', 
+                        detail_status = 'DETAIL_STATUS_UNSPECIFIED', 
                         created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                        modified_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                        labels = {
-                            'key' : ''
-                            }, )
+                        deleted_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                        launch_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                        last_serve_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                        success_count = 56, 
+                        failed_count = 56, 
+                        session_number = 56, 
+                        cpus = 56, 
+                        memory = 56, 
+                        gpu_name = '', 
+                        gpus = 56, 
+                        app_id = '', 
+                        app_revision = '', 
+                        replace_worker_id = '', 
+                        user_id = '', 
+                        request_id = '', 
+                        gpu_model = '', 
+                        gpu_num = 56, )
                     ]
             )
         else:
-            return V1ListResponse(
+            return V1ListWorkersByAppAndUserResponse(
         )
         """
 
-    def testV1ListResponse(self):
-        """Test V1ListResponse"""
+    def testV1ListWorkersByAppAndUserResponse(self):
+        """Test V1ListWorkersByAppAndUserResponse"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

## Comparing `generated/schedulers/test/test_v1_list_workers_response.py` & `generated/apps/test/test_v1_list_workers_by_device_and_status_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,59 +1,76 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/comm/v1/messages.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 import datetime
 
-from generated.schedulers.models.v1_list_workers_response import V1ListWorkersResponse  # noqa: E501
+from generated.apps.models.v1_list_workers_by_device_and_status_response import V1ListWorkersByDeviceAndStatusResponse  # noqa: E501
 
-class TestV1ListWorkersResponse(unittest.TestCase):
-    """V1ListWorkersResponse unit test stubs"""
+class TestV1ListWorkersByDeviceAndStatusResponse(unittest.TestCase):
+    """V1ListWorkersByDeviceAndStatusResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> V1ListWorkersResponse:
-        """Test V1ListWorkersResponse
+    def make_instance(self, include_optional) -> V1ListWorkersByDeviceAndStatusResponse:
+        """Test V1ListWorkersByDeviceAndStatusResponse
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `V1ListWorkersResponse`
+        # uncomment below to create an instance of `V1ListWorkersByDeviceAndStatusResponse`
         """
-        model = V1ListWorkersResponse()  # noqa: E501
+        model = V1ListWorkersByDeviceAndStatusResponse()  # noqa: E501
         if include_optional:
-            return V1ListWorkersResponse(
+            return V1ListWorkersByDeviceAndStatusResponse(
                 workers = [
-                    generated.schedulers.models.appsv1_worker.appsv1Worker(
+                    generated.apps.models.v1_worker.v1Worker(
                         id = '', 
                         device_id = '', 
-                        status = '', 
+                        status = 'STATUS_UNSPECIFIED', 
+                        detail_status = 'DETAIL_STATUS_UNSPECIFIED', 
                         created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                        deleted_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), )
+                        deleted_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                        launch_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                        last_serve_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                        success_count = 56, 
+                        failed_count = 56, 
+                        session_number = 56, 
+                        cpus = 56, 
+                        memory = 56, 
+                        gpu_name = '', 
+                        gpus = 56, 
+                        app_id = '', 
+                        app_revision = '', 
+                        replace_worker_id = '', 
+                        user_id = '', 
+                        request_id = '', 
+                        gpu_model = '', 
+                        gpu_num = 56, )
                     ]
             )
         else:
-            return V1ListWorkersResponse(
+            return V1ListWorkersByDeviceAndStatusResponse(
         )
         """
 
-    def testV1ListWorkersResponse(self):
-        """Test V1ListWorkersResponse"""
+    def testV1ListWorkersByDeviceAndStatusResponse(self):
+        """Test V1ListWorkersByDeviceAndStatusResponse"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

## Comparing `generated/schedulers/test/test_v1_volume_status.py` & `generated/apps/test/test_worker_worker_status.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/register_message.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 import datetime
 
-from generated.schedulers.models.v1_volume_status import V1VolumeStatus  # noqa: E501
+from generated.apps.models.worker_worker_status import WorkerWorkerStatus  # noqa: E501
 
-class TestV1VolumeStatus(unittest.TestCase):
-    """V1VolumeStatus unit test stubs"""
+class TestWorkerWorkerStatus(unittest.TestCase):
+    """WorkerWorkerStatus unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testV1VolumeStatus(self):
-        """Test V1VolumeStatus"""
-        # inst = V1VolumeStatus()
+    def testWorkerWorkerStatus(self):
+        """Test WorkerWorkerStatus"""
+        # inst = WorkerWorkerStatus()
 
 if __name__ == '__main__':
     unittest.main()
```

## Comparing `generated/schedulers/test/test_v1_worker_status.py` & `generated/apps/test/test_worker_worker_detail_status.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 # coding: utf-8
 
 """
-    everai/scheduler/v1/register_message.proto
+    everai/apps/v1/worker.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 import datetime
 
-from generated.schedulers.models.v1_worker_status import V1WorkerStatus  # noqa: E501
+from generated.apps.models.worker_worker_detail_status import WorkerWorkerDetailStatus  # noqa: E501
 
-class TestV1WorkerStatus(unittest.TestCase):
-    """V1WorkerStatus unit test stubs"""
+class TestWorkerWorkerDetailStatus(unittest.TestCase):
+    """WorkerWorkerDetailStatus unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testV1WorkerStatus(self):
-        """Test V1WorkerStatus"""
-        # inst = V1WorkerStatus()
+    def testWorkerWorkerDetailStatus(self):
+        """Test WorkerWorkerDetailStatus"""
+        # inst = WorkerWorkerDetailStatus()
 
 if __name__ == '__main__':
     unittest.main()
```

## Comparing `everai-0.1.62.dist-info/METADATA` & `everai-0.1.63.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: everai
-Version: 0.1.62
+Version: 0.1.63
 Summary: Client library to manage everai infrastructure
 Author-email: mc <mc@expvent.com>
 Maintainer-email: mc <mc@expvent.com>
 Project-URL: Homepage, https://everai.expvent.com
 Project-URL: Documentation, https://everai.expvent.com
 Project-URL: Repository, https://github.com/expvent/everai
 Project-URL: Issues, https://github.com/expvent/everai/issues
```

