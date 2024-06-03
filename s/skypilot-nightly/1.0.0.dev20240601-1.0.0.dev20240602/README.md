# Comparing `tmp/skypilot_nightly-1.0.0.dev20240601.tar.gz` & `tmp/skypilot_nightly-1.0.0.dev20240602.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skypilot_nightly-1.0.0.dev20240601.tar", last modified: Sat Jun  1 10:38:34 2024, max compression
+gzip compressed data, was "skypilot_nightly-1.0.0.dev20240602.tar", last modified: Sun Jun  2 10:38:08 2024, max compression
```

## Comparing `skypilot_nightly-1.0.0.dev20240601.tar` & `skypilot_nightly-1.0.0.dev20240602.tar`

### file list

```diff
@@ -1,339 +1,339 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:38:34.914598 skypilot_nightly-1.0.0.dev20240601/
--rw-r--r--   0 runner    (1001) docker     (127)    12170 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    18142 2024-06-01 10:38:34.914598 skypilot_nightly-1.0.0.dev20240601/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12079 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 10:38:34.914598 skypilot_nightly-1.0.0.dev20240601/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    12056 2024-06-01 10:38:31.000000 skypilot_nightly-1.0.0.dev20240601/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:38:34.854598 skypilot_nightly-1.0.0.dev20240601/sky/
--rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-06-01 10:38:34.000000 skypilot_nightly-1.0.0.dev20240601/sky/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:38:34.858598 skypilot_nightly-1.0.0.dev20240601/sky/adaptors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/adaptors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/adaptors/aws.py
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/adaptors/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     7594 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/adaptors/cloudflare.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/adaptors/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/adaptors/cudo.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/adaptors/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/adaptors/gcp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/adaptors/ibm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/adaptors/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/adaptors/oci.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/adaptors/runpod.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/adaptors/vsphere.py
--rw-r--r--   0 runner    (1001) docker     (127)    21408 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:38:34.858598 skypilot_nightly-1.0.0.dev20240601/sky/backends/
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/backends/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)   125856 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/backends/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)   231003 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/backends/cloud_vm_ray_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     8358 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/backends/docker_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16741 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/backends/local_docker_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:38:34.858598 skypilot_nightly-1.0.0.dev20240601/sky/backends/monkey_patches/
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/backends/monkey_patches/monkey_patch_ray_up.py
--rw-r--r--   0 runner    (1001) docker     (127)     7297 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/backends/wheel_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:38:34.858598 skypilot_nightly-1.0.0.dev20240601/sky/benchmark/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8723 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/benchmark/benchmark_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    26446 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/benchmark/benchmark_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9079 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/check.py
--rw-r--r--   0 runner    (1001) docker     (127)   200543 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    11806 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/cloud_stores.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:38:34.862598 skypilot_nightly-1.0.0.dev20240601/sky/clouds/
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/clouds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    44519 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/clouds/aws.py
--rw-r--r--   0 runner    (1001) docker     (127)    30929 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/clouds/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)    31840 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/clouds/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/clouds/cloud_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    12344 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/clouds/cudo.py
--rw-r--r--   0 runner    (1001) docker     (127)    12477 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/clouds/fluidstack.py
--rw-r--r--   0 runner    (1001) docker     (127)    47944 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/clouds/gcp.py
--rw-r--r--   0 runner    (1001) docker     (127)    20969 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/clouds/ibm.py
--rw-r--r--   0 runner    (1001) docker     (127)    20272 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/clouds/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (127)    11991 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/clouds/lambda_cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)    25136 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/clouds/oci.py
--rw-r--r--   0 runner    (1001) docker     (127)    10391 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/clouds/paperspace.py
--rw-r--r--   0 runner    (1001) docker     (127)    11000 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/clouds/runpod.py
--rw-r--r--   0 runner    (1001) docker     (127)    15383 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/clouds/scp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:38:34.866598 skypilot_nightly-1.0.0.dev20240601/sky/clouds/service_catalog/
--rw-r--r--   0 runner    (1001) docker     (127)    14546 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/clouds/service_catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12550 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/clouds/service_catalog/aws_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     7289 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/clouds/service_catalog/azure_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)    26837 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/clouds/service_catalog/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/clouds/service_catalog/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/clouds/service_catalog/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4335 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/clouds/service_catalog/cudo_catalog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:38:34.866598 skypilot_nightly-1.0.0.dev20240601/sky/clouds/service_catalog/data_fetchers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/clouds/service_catalog/data_fetchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22424 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/clouds/service_catalog/data_fetchers/fetch_aws.py
--rw-r--r--   0 runner    (1001) docker     (127)    11477 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/clouds/service_catalog/data_fetchers/fetch_azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/clouds/service_catalog/data_fetchers/fetch_cudo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/clouds/service_catalog/data_fetchers/fetch_fluidstack.py
--rw-r--r--   0 runner    (1001) docker     (127)    22243 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)    21462 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/clouds/service_catalog/data_fetchers/fetch_vsphere.py
--rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/clouds/service_catalog/fluidstack_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)    24120 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/clouds/service_catalog/gcp_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/clouds/service_catalog/ibm_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     7856 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/clouds/service_catalog/kubernetes_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/clouds/service_catalog/lambda_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     7542 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/clouds/service_catalog/oci_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/clouds/service_catalog/paperspace_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/clouds/service_catalog/runpod_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/clouds/service_catalog/scp_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/clouds/service_catalog/vsphere_catalog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:38:34.866598 skypilot_nightly-1.0.0.dev20240601/sky/clouds/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/clouds/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6968 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/clouds/utils/gcp_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9991 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/clouds/utils/lambda_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/clouds/utils/oci_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15781 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/clouds/utils/scp_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11802 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/clouds/vsphere.py
--rw-r--r--   0 runner    (1001) docker     (127)    34233 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/dag.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:38:34.870598 skypilot_nightly-1.0.0.dev20240601/sky/data/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/data/data_transfer.py
--rw-r--r--   0 runner    (1001) docker     (127)    21664 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/data/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8351 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/data/mounting_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)   118872 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/data/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     6867 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/data/storage_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8249 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    25107 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/execution.py
--rw-r--r--   0 runner    (1001) docker     (127)    28681 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/global_user_state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:38:34.870598 skypilot_nightly-1.0.0.dev20240601/sky/jobs/
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/jobs/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    26607 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/jobs/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    13426 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/jobs/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:38:34.870598 skypilot_nightly-1.0.0.dev20240601/sky/jobs/dashboard/
--rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/jobs/dashboard/dashboard.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:38:34.870598 skypilot_nightly-1.0.0.dev20240601/sky/jobs/dashboard/static/
--rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/jobs/dashboard/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:38:34.870598 skypilot_nightly-1.0.0.dev20240601/sky/jobs/dashboard/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/jobs/dashboard/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)    25556 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/jobs/recovery_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)    23041 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/jobs/state.py
--rw-r--r--   0 runner    (1001) docker     (127)    35652 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/jobs/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    56668 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:38:34.870598 skypilot_nightly-1.0.0.dev20240601/sky/provision/
--rw-r--r--   0 runner    (1001) docker     (127)     5951 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/provision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:38:34.874598 skypilot_nightly-1.0.0.dev20240601/sky/provision/aws/
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/provision/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22092 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/provision/aws/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    36307 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/provision/aws/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/provision/aws/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:38:34.874598 skypilot_nightly-1.0.0.dev20240601/sky/provision/azure/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/provision/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/provision/azure/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     9339 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/provision/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:38:34.874598 skypilot_nightly-1.0.0.dev20240601/sky/provision/cudo/
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/provision/cudo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/provision/cudo/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/provision/cudo/cudo_machine_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/provision/cudo/cudo_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/provision/cudo/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)    17540 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/provision/docker_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:38:34.874598 skypilot_nightly-1.0.0.dev20240601/sky/provision/fluidstack/
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/provision/fluidstack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/provision/fluidstack/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8262 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/provision/fluidstack/fluidstack_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14974 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/provision/fluidstack/instance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:38:34.874598 skypilot_nightly-1.0.0.dev20240601/sky/provision/gcp/
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/provision/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32964 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/provision/gcp/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7234 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/provision/gcp/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    24215 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/provision/gcp/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)    59069 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/provision/gcp/instance_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    22367 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/provision/instance_setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:38:34.874598 skypilot_nightly-1.0.0.dev20240601/sky/provision/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/provision/kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28319 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/provision/kubernetes/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    32724 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/provision/kubernetes/instance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:38:34.878598 skypilot_nightly-1.0.0.dev20240601/sky/provision/kubernetes/manifests/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/provision/kubernetes/manifests/smarter-device-manager-configmap.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/provision/kubernetes/manifests/smarter-device-manager-daemonset.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    10851 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/provision/kubernetes/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     9384 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/provision/kubernetes/network_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    62585 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/provision/kubernetes/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/provision/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/provision/metadata_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:38:34.878598 skypilot_nightly-1.0.0.dev20240601/sky/provision/paperspace/
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/provision/paperspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/provision/paperspace/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/provision/paperspace/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    12045 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/provision/paperspace/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     9428 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/provision/paperspace/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    25103 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/provision/provisioner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:38:34.878598 skypilot_nightly-1.0.0.dev20240601/sky/provision/runpod/
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/provision/runpod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/provision/runpod/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7905 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/provision/runpod/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/provision/runpod/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:38:34.878598 skypilot_nightly-1.0.0.dev20240601/sky/provision/vsphere/
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/provision/vsphere/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:38:34.878598 skypilot_nightly-1.0.0.dev20240601/sky/provision/vsphere/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/provision/vsphere/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/provision/vsphere/common/cls_api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    14096 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/provision/vsphere/common/cls_api_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/provision/vsphere/common/custom_script.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/provision/vsphere/common/id_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/provision/vsphere/common/metadata_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/provision/vsphere/common/service_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/provision/vsphere/common/service_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/provision/vsphere/common/ssl_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/provision/vsphere/common/vapiconnect.py
--rw-r--r--   0 runner    (1001) docker     (127)    17877 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/provision/vsphere/common/vim_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/provision/vsphere/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    24488 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/provision/vsphere/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)    15151 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/provision/vsphere/vsphere_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    65346 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:38:34.882598 skypilot_nightly-1.0.0.dev20240601/sky/serve/
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/serve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30136 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/serve/autoscalers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/serve/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     8022 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/serve/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    28710 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/serve/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    11548 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/serve/load_balancer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/serve/load_balancing_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)    57216 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/serve/replica_managers.py
--rw-r--r--   0 runner    (1001) docker     (127)    18830 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/serve/serve_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    37183 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/serve/serve_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10931 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/serve/service.py
--rw-r--r--   0 runner    (1001) docker     (127)    14469 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/serve/service_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:38:34.882598 skypilot_nightly-1.0.0.dev20240601/sky/setup_files/
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/setup_files/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12056 2024-06-01 10:38:31.000000 skypilot_nightly-1.0.0.dev20240601/sky/setup_files/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/sky_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:38:34.886598 skypilot_nightly-1.0.0.dev20240601/sky/skylet/
--rw-r--r--   0 runner    (1001) docker     (127)    12381 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/skylet/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/skylet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/skylet/attempt_skylet.py
--rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/skylet/autostop_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/skylet/configs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11411 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/skylet/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    12303 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/skylet/events.py
--rw-r--r--   0 runner    (1001) docker     (127)    35198 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/skylet/job_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    18824 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/skylet/log_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/skylet/log_lib.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:38:34.886598 skypilot_nightly-1.0.0.dev20240601/sky/skylet/providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/skylet/providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:38:34.886598 skypilot_nightly-1.0.0.dev20240601/sky/skylet/providers/azure/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/skylet/providers/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/skylet/providers/azure/azure-config-template.json
--rw-r--r--   0 runner    (1001) docker     (127)    10901 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/skylet/providers/azure/azure-vm-template.json
--rw-r--r--   0 runner    (1001) docker     (127)     6342 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/skylet/providers/azure/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    19215 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/skylet/providers/azure/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    16355 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/skylet/providers/command_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:38:34.886598 skypilot_nightly-1.0.0.dev20240601/sky/skylet/providers/ibm/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/skylet/providers/ibm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38280 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/skylet/providers/ibm/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/skylet/providers/ibm/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    34630 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/skylet/providers/ibm/vpc_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:38:34.886598 skypilot_nightly-1.0.0.dev20240601/sky/skylet/providers/lambda_cloud/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/skylet/providers/lambda_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13971 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/skylet/providers/lambda_cloud/node_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:38:34.886598 skypilot_nightly-1.0.0.dev20240601/sky/skylet/providers/oci/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/skylet/providers/oci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20492 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/skylet/providers/oci/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    17202 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/skylet/providers/oci/query_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/skylet/providers/oci/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:38:34.886598 skypilot_nightly-1.0.0.dev20240601/sky/skylet/providers/scp/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/skylet/providers/scp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4683 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/skylet/providers/scp/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    22411 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/skylet/providers/scp/node_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:38:34.890598 skypilot_nightly-1.0.0.dev20240601/sky/skylet/ray_patches/
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/skylet/ray_patches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/skylet/ray_patches/autoscaler.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/skylet/ray_patches/cli.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/skylet/ray_patches/command_runner.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/skylet/ray_patches/log_monitor.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/skylet/ray_patches/resource_demand_scheduler.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/skylet/ray_patches/updater.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/skylet/ray_patches/worker.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/skylet/skylet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/skylet/subprocess_daemon.py
--rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/skypilot_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/status_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    47807 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:38:34.890598 skypilot_nightly-1.0.0.dev20240601/sky/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     7477 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/templates/aws-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     9099 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/templates/azure-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/templates/cudo-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/templates/fluidstack-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     8880 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/templates/gcp-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     6669 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/templates/ibm-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/templates/jobs-controller.yaml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/templates/kubernetes-ingress.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/templates/kubernetes-loadbalancer.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/templates/kubernetes-port-forward-proxy-command.sh.j2
--rw-r--r--   0 runner    (1001) docker     (127)    15489 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/templates/kubernetes-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/templates/kubernetes-ssh-jump.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     5738 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/templates/lambda-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/templates/local-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     7032 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/templates/oci-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/templates/paperspace-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/templates/runpod-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     5608 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/templates/scp-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/templates/sky-serve-controller.yaml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/templates/vsphere-ray.yml.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:38:34.894598 skypilot_nightly-1.0.0.dev20240601/sky/usage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/usage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/usage/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    17807 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/usage/usage_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:38:34.894598 skypilot_nightly-1.0.0.dev20240601/sky/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/utils/accelerator_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:38:34.894598 skypilot_nightly-1.0.0.dev20240601/sky/utils/cli_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/utils/cli_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/utils/cli_utils/status_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/utils/cluster_yaml_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    23317 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/utils/command_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     5560 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/utils/command_runner.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    23848 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/utils/common_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    34620 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/utils/controller_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/utils/dag_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/utils/db_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/utils/env_options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:38:34.898598 skypilot_nightly-1.0.0.dev20240601/sky/utils/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/utils/kubernetes/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9759 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/utils/kubernetes/create_cluster.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      927 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/utils/kubernetes/delete_cluster.sh
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/utils/kubernetes/generate_kind_config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4422 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/utils/kubernetes/generate_static_kubeconfig.sh
--rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/utils/kubernetes/gpu_labeler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/utils/kubernetes/k8s_gpu_labeler_job.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/utils/kubernetes/k8s_gpu_labeler_setup.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6560 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/utils/kubernetes/ssh_jump_lifecycle_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/utils/kubernetes_enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     8139 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/utils/resources_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/utils/rich_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    23416 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/utils/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/utils/subprocess_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/utils/timeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/utils/ux_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/sky/utils/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:38:34.902598 skypilot_nightly-1.0.0.dev20240601/skypilot_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18142 2024-06-01 10:38:34.000000 skypilot_nightly-1.0.0.dev20240601/skypilot_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9353 2024-06-01 10:38:34.000000 skypilot_nightly-1.0.0.dev20240601/skypilot_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 10:38:34.000000 skypilot_nightly-1.0.0.dev20240601/skypilot_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-06-01 10:38:34.000000 skypilot_nightly-1.0.0.dev20240601/skypilot_nightly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-06-01 10:38:34.000000 skypilot_nightly-1.0.0.dev20240601/skypilot_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-06-01 10:38:34.000000 skypilot_nightly-1.0.0.dev20240601/skypilot_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:38:34.902598 skypilot_nightly-1.0.0.dev20240601/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3579 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     9592 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/tests/test_global_user_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     8789 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/tests/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)    17649 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/tests/test_jobs_and_serve.py
--rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/tests/test_list_accelerators.py
--rw-r--r--   0 runner    (1001) docker     (127)    27759 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/tests/test_optimizer_dryruns.py
--rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/tests/test_optimizer_random_dag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/tests/test_serve_autoscaler.py
--rw-r--r--   0 runner    (1001) docker     (127)   220340 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/tests/test_smoke.py
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/tests/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/tests/test_wheels.py
--rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-06-01 10:38:25.000000 skypilot_nightly-1.0.0.dev20240601/tests/test_yaml_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:38:08.352665 skypilot_nightly-1.0.0.dev20240602/
+-rw-r--r--   0 runner    (1001) docker     (127)    12170 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    18142 2024-06-02 10:38:08.352665 skypilot_nightly-1.0.0.dev20240602/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12079 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 10:38:08.352665 skypilot_nightly-1.0.0.dev20240602/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    12056 2024-06-02 10:38:05.000000 skypilot_nightly-1.0.0.dev20240602/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:38:08.296666 skypilot_nightly-1.0.0.dev20240602/sky/
+-rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-06-02 10:38:08.000000 skypilot_nightly-1.0.0.dev20240602/sky/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:38:08.296666 skypilot_nightly-1.0.0.dev20240602/sky/adaptors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/adaptors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/adaptors/aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/adaptors/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7594 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/adaptors/cloudflare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/adaptors/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/adaptors/cudo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/adaptors/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/adaptors/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/adaptors/ibm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/adaptors/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/adaptors/oci.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/adaptors/runpod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/adaptors/vsphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21408 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:38:08.296666 skypilot_nightly-1.0.0.dev20240602/sky/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/backends/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)   125856 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/backends/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)   231003 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/backends/cloud_vm_ray_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8358 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/backends/docker_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16741 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/backends/local_docker_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:38:08.300665 skypilot_nightly-1.0.0.dev20240602/sky/backends/monkey_patches/
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/backends/monkey_patches/monkey_patch_ray_up.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7297 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/backends/wheel_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:38:08.300665 skypilot_nightly-1.0.0.dev20240602/sky/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8723 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/benchmark/benchmark_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26446 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/benchmark/benchmark_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9079 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)   200543 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11806 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/cloud_stores.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:38:08.300665 skypilot_nightly-1.0.0.dev20240602/sky/clouds/
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/clouds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44519 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/clouds/aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30929 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/clouds/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31840 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/clouds/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/clouds/cloud_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12344 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/clouds/cudo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12477 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/clouds/fluidstack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47944 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/clouds/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20969 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/clouds/ibm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20272 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/clouds/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11991 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/clouds/lambda_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25136 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/clouds/oci.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10391 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/clouds/paperspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11000 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/clouds/runpod.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15383 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/clouds/scp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:38:08.304665 skypilot_nightly-1.0.0.dev20240602/sky/clouds/service_catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)    14546 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/clouds/service_catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12550 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/clouds/service_catalog/aws_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7289 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/clouds/service_catalog/azure_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26837 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/clouds/service_catalog/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/clouds/service_catalog/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/clouds/service_catalog/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4335 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/clouds/service_catalog/cudo_catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:38:08.304665 skypilot_nightly-1.0.0.dev20240602/sky/clouds/service_catalog/data_fetchers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/clouds/service_catalog/data_fetchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22424 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/clouds/service_catalog/data_fetchers/fetch_aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11477 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/clouds/service_catalog/data_fetchers/fetch_azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/clouds/service_catalog/data_fetchers/fetch_cudo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/clouds/service_catalog/data_fetchers/fetch_fluidstack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22243 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21462 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/clouds/service_catalog/data_fetchers/fetch_vsphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/clouds/service_catalog/fluidstack_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24120 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/clouds/service_catalog/gcp_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/clouds/service_catalog/ibm_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7856 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/clouds/service_catalog/kubernetes_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/clouds/service_catalog/lambda_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7542 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/clouds/service_catalog/oci_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/clouds/service_catalog/paperspace_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/clouds/service_catalog/runpod_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/clouds/service_catalog/scp_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/clouds/service_catalog/vsphere_catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:38:08.308665 skypilot_nightly-1.0.0.dev20240602/sky/clouds/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/clouds/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6968 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/clouds/utils/gcp_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9991 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/clouds/utils/lambda_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/clouds/utils/oci_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15781 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/clouds/utils/scp_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11802 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/clouds/vsphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34233 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/dag.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:38:08.308665 skypilot_nightly-1.0.0.dev20240602/sky/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/data/data_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21664 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/data/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8351 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/data/mounting_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)   118872 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/data/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6867 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/data/storage_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8249 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25107 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28681 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/global_user_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:38:08.308665 skypilot_nightly-1.0.0.dev20240602/sky/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/jobs/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26607 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/jobs/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13426 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/jobs/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:38:08.308665 skypilot_nightly-1.0.0.dev20240602/sky/jobs/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/jobs/dashboard/dashboard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:38:08.308665 skypilot_nightly-1.0.0.dev20240602/sky/jobs/dashboard/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/jobs/dashboard/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:38:08.308665 skypilot_nightly-1.0.0.dev20240602/sky/jobs/dashboard/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/jobs/dashboard/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)    25556 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/jobs/recovery_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23041 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/jobs/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35652 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/jobs/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56668 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:38:08.312666 skypilot_nightly-1.0.0.dev20240602/sky/provision/
+-rw-r--r--   0 runner    (1001) docker     (127)     5951 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/provision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:38:08.312666 skypilot_nightly-1.0.0.dev20240602/sky/provision/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/provision/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22092 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/provision/aws/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36307 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/provision/aws/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/provision/aws/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:38:08.312666 skypilot_nightly-1.0.0.dev20240602/sky/provision/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/provision/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/provision/azure/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9339 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/provision/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:38:08.312666 skypilot_nightly-1.0.0.dev20240602/sky/provision/cudo/
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/provision/cudo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/provision/cudo/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/provision/cudo/cudo_machine_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/provision/cudo/cudo_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/provision/cudo/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17540 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/provision/docker_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:38:08.312666 skypilot_nightly-1.0.0.dev20240602/sky/provision/fluidstack/
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/provision/fluidstack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/provision/fluidstack/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8262 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/provision/fluidstack/fluidstack_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14974 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/provision/fluidstack/instance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:38:08.312666 skypilot_nightly-1.0.0.dev20240602/sky/provision/gcp/
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/provision/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32964 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/provision/gcp/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7234 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/provision/gcp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24215 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/provision/gcp/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59069 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/provision/gcp/instance_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22367 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/provision/instance_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:38:08.316666 skypilot_nightly-1.0.0.dev20240602/sky/provision/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/provision/kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28319 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/provision/kubernetes/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32724 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/provision/kubernetes/instance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:38:08.316666 skypilot_nightly-1.0.0.dev20240602/sky/provision/kubernetes/manifests/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/provision/kubernetes/manifests/smarter-device-manager-configmap.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/provision/kubernetes/manifests/smarter-device-manager-daemonset.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    10851 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/provision/kubernetes/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9384 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/provision/kubernetes/network_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62585 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/provision/kubernetes/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/provision/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/provision/metadata_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:38:08.316666 skypilot_nightly-1.0.0.dev20240602/sky/provision/paperspace/
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/provision/paperspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/provision/paperspace/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/provision/paperspace/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12045 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/provision/paperspace/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9428 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/provision/paperspace/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25103 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/provision/provisioner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:38:08.316666 skypilot_nightly-1.0.0.dev20240602/sky/provision/runpod/
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/provision/runpod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/provision/runpod/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7905 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/provision/runpod/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/provision/runpod/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:38:08.316666 skypilot_nightly-1.0.0.dev20240602/sky/provision/vsphere/
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/provision/vsphere/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:38:08.320665 skypilot_nightly-1.0.0.dev20240602/sky/provision/vsphere/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/provision/vsphere/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/provision/vsphere/common/cls_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14096 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/provision/vsphere/common/cls_api_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/provision/vsphere/common/custom_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/provision/vsphere/common/id_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/provision/vsphere/common/metadata_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/provision/vsphere/common/service_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/provision/vsphere/common/service_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/provision/vsphere/common/ssl_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/provision/vsphere/common/vapiconnect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17877 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/provision/vsphere/common/vim_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/provision/vsphere/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24488 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/provision/vsphere/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15151 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/provision/vsphere/vsphere_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65346 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:38:08.320665 skypilot_nightly-1.0.0.dev20240602/sky/serve/
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/serve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30136 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/serve/autoscalers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/serve/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8022 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/serve/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28710 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/serve/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11548 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/serve/load_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/serve/load_balancing_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57216 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/serve/replica_managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18830 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/serve/serve_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37183 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/serve/serve_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10931 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/serve/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14469 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/serve/service_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:38:08.320665 skypilot_nightly-1.0.0.dev20240602/sky/setup_files/
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/setup_files/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12056 2024-06-02 10:38:05.000000 skypilot_nightly-1.0.0.dev20240602/sky/setup_files/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/sky_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:38:08.324665 skypilot_nightly-1.0.0.dev20240602/sky/skylet/
+-rw-r--r--   0 runner    (1001) docker     (127)    12381 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/skylet/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/skylet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/skylet/attempt_skylet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/skylet/autostop_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/skylet/configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11411 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/skylet/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12303 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/skylet/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35198 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/skylet/job_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18824 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/skylet/log_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/skylet/log_lib.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:38:08.324665 skypilot_nightly-1.0.0.dev20240602/sky/skylet/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/skylet/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:38:08.324665 skypilot_nightly-1.0.0.dev20240602/sky/skylet/providers/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/skylet/providers/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/skylet/providers/azure/azure-config-template.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10901 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/skylet/providers/azure/azure-vm-template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6342 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/skylet/providers/azure/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19215 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/skylet/providers/azure/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16355 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/skylet/providers/command_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:38:08.324665 skypilot_nightly-1.0.0.dev20240602/sky/skylet/providers/ibm/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/skylet/providers/ibm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38280 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/skylet/providers/ibm/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/skylet/providers/ibm/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34630 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/skylet/providers/ibm/vpc_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:38:08.328665 skypilot_nightly-1.0.0.dev20240602/sky/skylet/providers/lambda_cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/skylet/providers/lambda_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13971 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/skylet/providers/lambda_cloud/node_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:38:08.328665 skypilot_nightly-1.0.0.dev20240602/sky/skylet/providers/oci/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/skylet/providers/oci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20492 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/skylet/providers/oci/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17202 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/skylet/providers/oci/query_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/skylet/providers/oci/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:38:08.328665 skypilot_nightly-1.0.0.dev20240602/sky/skylet/providers/scp/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/skylet/providers/scp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4683 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/skylet/providers/scp/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22411 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/skylet/providers/scp/node_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:38:08.328665 skypilot_nightly-1.0.0.dev20240602/sky/skylet/ray_patches/
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/skylet/ray_patches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/skylet/ray_patches/autoscaler.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/skylet/ray_patches/cli.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/skylet/ray_patches/command_runner.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/skylet/ray_patches/log_monitor.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/skylet/ray_patches/resource_demand_scheduler.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/skylet/ray_patches/updater.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/skylet/ray_patches/worker.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/skylet/skylet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/skylet/subprocess_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/skypilot_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/status_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47807 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:38:08.332665 skypilot_nightly-1.0.0.dev20240602/sky/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     7477 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/templates/aws-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     9099 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/templates/azure-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/templates/cudo-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/templates/fluidstack-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     8880 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/templates/gcp-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     6669 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/templates/ibm-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/templates/jobs-controller.yaml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/templates/kubernetes-ingress.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/templates/kubernetes-loadbalancer.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/templates/kubernetes-port-forward-proxy-command.sh.j2
+-rw-r--r--   0 runner    (1001) docker     (127)    15489 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/templates/kubernetes-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/templates/kubernetes-ssh-jump.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     5738 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/templates/lambda-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/templates/local-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     7032 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/templates/oci-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/templates/paperspace-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/templates/runpod-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     5608 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/templates/scp-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/templates/sky-serve-controller.yaml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/templates/vsphere-ray.yml.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:38:08.332665 skypilot_nightly-1.0.0.dev20240602/sky/usage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/usage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/usage/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17807 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/usage/usage_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:38:08.336665 skypilot_nightly-1.0.0.dev20240602/sky/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/utils/accelerator_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:38:08.336665 skypilot_nightly-1.0.0.dev20240602/sky/utils/cli_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/utils/cli_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/utils/cli_utils/status_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/utils/cluster_yaml_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23317 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/utils/command_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5560 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/utils/command_runner.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    23848 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/utils/common_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34620 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/utils/controller_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/utils/dag_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/utils/db_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/utils/env_options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:38:08.336665 skypilot_nightly-1.0.0.dev20240602/sky/utils/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/utils/kubernetes/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9759 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/utils/kubernetes/create_cluster.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      927 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/utils/kubernetes/delete_cluster.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/utils/kubernetes/generate_kind_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4422 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/utils/kubernetes/generate_static_kubeconfig.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/utils/kubernetes/gpu_labeler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/utils/kubernetes/k8s_gpu_labeler_job.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/utils/kubernetes/k8s_gpu_labeler_setup.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6560 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/utils/kubernetes/ssh_jump_lifecycle_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/utils/kubernetes_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8139 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/utils/resources_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/utils/rich_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23416 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/utils/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/utils/subprocess_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/utils/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/utils/ux_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/sky/utils/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:38:08.340665 skypilot_nightly-1.0.0.dev20240602/skypilot_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18142 2024-06-02 10:38:08.000000 skypilot_nightly-1.0.0.dev20240602/skypilot_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9353 2024-06-02 10:38:08.000000 skypilot_nightly-1.0.0.dev20240602/skypilot_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 10:38:08.000000 skypilot_nightly-1.0.0.dev20240602/skypilot_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-06-02 10:38:08.000000 skypilot_nightly-1.0.0.dev20240602/skypilot_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-06-02 10:38:08.000000 skypilot_nightly-1.0.0.dev20240602/skypilot_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-06-02 10:38:08.000000 skypilot_nightly-1.0.0.dev20240602/skypilot_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:38:08.340665 skypilot_nightly-1.0.0.dev20240602/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3579 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9592 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/tests/test_global_user_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8789 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17649 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/tests/test_jobs_and_serve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/tests/test_list_accelerators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27759 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/tests/test_optimizer_dryruns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/tests/test_optimizer_random_dag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/tests/test_serve_autoscaler.py
+-rw-r--r--   0 runner    (1001) docker     (127)   220340 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/tests/test_smoke.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/tests/test_wheels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-06-02 10:38:03.000000 skypilot_nightly-1.0.0.dev20240602/tests/test_yaml_parser.py
```

### Comparing `skypilot_nightly-1.0.0.dev20240601/LICENSE` & `skypilot_nightly-1.0.0.dev20240602/LICENSE`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/MANIFEST.in` & `skypilot_nightly-1.0.0.dev20240602/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/PKG-INFO` & `skypilot_nightly-1.0.0.dev20240602/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skypilot-nightly
-Version: 1.0.0.dev20240601
+Version: 1.0.0.dev20240602
 Summary: SkyPilot: An intercloud broker for the clouds
 Author: SkyPilot Team
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/skypilot-org/skypilot
 Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
 Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
 Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
```

### Comparing `skypilot_nightly-1.0.0.dev20240601/README.md` & `skypilot_nightly-1.0.0.dev20240602/README.md`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/pyproject.toml` & `skypilot_nightly-1.0.0.dev20240602/pyproject.toml`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/setup.py` & `skypilot_nightly-1.0.0.dev20240602/setup.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/__init__.py` & `skypilot_nightly-1.0.0.dev20240602/sky/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
             commit_hash += '-dirty'
         return commit_hash
     except Exception:  # pylint: disable=broad-except
         return _SKYPILOT_COMMIT_SHA
 
 
 __commit__ = _get_git_commit()
-__version__ = '1.0.0.dev20240601'
+__version__ = '1.0.0.dev20240602'
 __root_dir__ = os.path.dirname(os.path.abspath(__file__))
 
 
 # ---------------------- Proxy Configuration ---------------------- #
 def _set_http_proxy_env_vars() -> None:
     urllib_proxies = dict(urllib.request.getproxies())
```

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/adaptors/aws.py` & `skypilot_nightly-1.0.0.dev20240602/sky/adaptors/aws.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/adaptors/azure.py` & `skypilot_nightly-1.0.0.dev20240602/sky/adaptors/azure.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/adaptors/cloudflare.py` & `skypilot_nightly-1.0.0.dev20240602/sky/adaptors/cloudflare.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/adaptors/common.py` & `skypilot_nightly-1.0.0.dev20240602/sky/adaptors/common.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/adaptors/gcp.py` & `skypilot_nightly-1.0.0.dev20240602/sky/adaptors/gcp.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/adaptors/ibm.py` & `skypilot_nightly-1.0.0.dev20240602/sky/adaptors/ibm.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/adaptors/kubernetes.py` & `skypilot_nightly-1.0.0.dev20240602/sky/adaptors/kubernetes.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/adaptors/oci.py` & `skypilot_nightly-1.0.0.dev20240602/sky/adaptors/oci.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/adaptors/vsphere.py` & `skypilot_nightly-1.0.0.dev20240602/sky/adaptors/vsphere.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/authentication.py` & `skypilot_nightly-1.0.0.dev20240602/sky/authentication.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/backends/__init__.py` & `skypilot_nightly-1.0.0.dev20240602/sky/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/backends/backend.py` & `skypilot_nightly-1.0.0.dev20240602/sky/backends/backend.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/backends/backend_utils.py` & `skypilot_nightly-1.0.0.dev20240602/sky/backends/backend_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/backends/cloud_vm_ray_backend.py` & `skypilot_nightly-1.0.0.dev20240602/sky/backends/cloud_vm_ray_backend.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/backends/docker_utils.py` & `skypilot_nightly-1.0.0.dev20240602/sky/backends/docker_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/backends/local_docker_backend.py` & `skypilot_nightly-1.0.0.dev20240602/sky/backends/local_docker_backend.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/backends/monkey_patches/monkey_patch_ray_up.py` & `skypilot_nightly-1.0.0.dev20240602/sky/backends/monkey_patches/monkey_patch_ray_up.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/backends/wheel_utils.py` & `skypilot_nightly-1.0.0.dev20240602/sky/backends/wheel_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/benchmark/benchmark_state.py` & `skypilot_nightly-1.0.0.dev20240602/sky/benchmark/benchmark_state.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/benchmark/benchmark_utils.py` & `skypilot_nightly-1.0.0.dev20240602/sky/benchmark/benchmark_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/check.py` & `skypilot_nightly-1.0.0.dev20240602/sky/check.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/cli.py` & `skypilot_nightly-1.0.0.dev20240602/sky/cli.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/cloud_stores.py` & `skypilot_nightly-1.0.0.dev20240602/sky/cloud_stores.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/clouds/__init__.py` & `skypilot_nightly-1.0.0.dev20240602/sky/clouds/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/clouds/aws.py` & `skypilot_nightly-1.0.0.dev20240602/sky/clouds/aws.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/clouds/azure.py` & `skypilot_nightly-1.0.0.dev20240602/sky/clouds/azure.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/clouds/cloud.py` & `skypilot_nightly-1.0.0.dev20240602/sky/clouds/cloud.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/clouds/cloud_registry.py` & `skypilot_nightly-1.0.0.dev20240602/sky/clouds/cloud_registry.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/clouds/cudo.py` & `skypilot_nightly-1.0.0.dev20240602/sky/clouds/cudo.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/clouds/fluidstack.py` & `skypilot_nightly-1.0.0.dev20240602/sky/clouds/fluidstack.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/clouds/gcp.py` & `skypilot_nightly-1.0.0.dev20240602/sky/clouds/gcp.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/clouds/ibm.py` & `skypilot_nightly-1.0.0.dev20240602/sky/clouds/ibm.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/clouds/kubernetes.py` & `skypilot_nightly-1.0.0.dev20240602/sky/clouds/kubernetes.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/clouds/lambda_cloud.py` & `skypilot_nightly-1.0.0.dev20240602/sky/clouds/lambda_cloud.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/clouds/oci.py` & `skypilot_nightly-1.0.0.dev20240602/sky/clouds/oci.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/clouds/paperspace.py` & `skypilot_nightly-1.0.0.dev20240602/sky/clouds/paperspace.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/clouds/runpod.py` & `skypilot_nightly-1.0.0.dev20240602/sky/clouds/runpod.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/clouds/scp.py` & `skypilot_nightly-1.0.0.dev20240602/sky/clouds/scp.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/clouds/service_catalog/__init__.py` & `skypilot_nightly-1.0.0.dev20240602/sky/clouds/service_catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/clouds/service_catalog/aws_catalog.py` & `skypilot_nightly-1.0.0.dev20240602/sky/clouds/service_catalog/aws_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/clouds/service_catalog/azure_catalog.py` & `skypilot_nightly-1.0.0.dev20240602/sky/clouds/service_catalog/azure_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/clouds/service_catalog/common.py` & `skypilot_nightly-1.0.0.dev20240602/sky/clouds/service_catalog/common.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/clouds/service_catalog/config.py` & `skypilot_nightly-1.0.0.dev20240602/sky/clouds/service_catalog/config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/clouds/service_catalog/cudo_catalog.py` & `skypilot_nightly-1.0.0.dev20240602/sky/clouds/service_catalog/cudo_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/clouds/service_catalog/data_fetchers/fetch_aws.py` & `skypilot_nightly-1.0.0.dev20240602/sky/clouds/service_catalog/data_fetchers/fetch_aws.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/clouds/service_catalog/data_fetchers/fetch_azure.py` & `skypilot_nightly-1.0.0.dev20240602/sky/clouds/service_catalog/data_fetchers/fetch_azure.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/clouds/service_catalog/data_fetchers/fetch_cudo.py` & `skypilot_nightly-1.0.0.dev20240602/sky/clouds/service_catalog/data_fetchers/fetch_cudo.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/clouds/service_catalog/data_fetchers/fetch_fluidstack.py` & `skypilot_nightly-1.0.0.dev20240602/sky/clouds/service_catalog/data_fetchers/fetch_fluidstack.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py` & `skypilot_nightly-1.0.0.dev20240602/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py` & `skypilot_nightly-1.0.0.dev20240602/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/clouds/service_catalog/data_fetchers/fetch_vsphere.py` & `skypilot_nightly-1.0.0.dev20240602/sky/clouds/service_catalog/data_fetchers/fetch_vsphere.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/clouds/service_catalog/fluidstack_catalog.py` & `skypilot_nightly-1.0.0.dev20240602/sky/clouds/service_catalog/fluidstack_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/clouds/service_catalog/gcp_catalog.py` & `skypilot_nightly-1.0.0.dev20240602/sky/clouds/service_catalog/gcp_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/clouds/service_catalog/ibm_catalog.py` & `skypilot_nightly-1.0.0.dev20240602/sky/clouds/service_catalog/ibm_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/clouds/service_catalog/kubernetes_catalog.py` & `skypilot_nightly-1.0.0.dev20240602/sky/clouds/service_catalog/kubernetes_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/clouds/service_catalog/lambda_catalog.py` & `skypilot_nightly-1.0.0.dev20240602/sky/clouds/service_catalog/lambda_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/clouds/service_catalog/oci_catalog.py` & `skypilot_nightly-1.0.0.dev20240602/sky/clouds/service_catalog/oci_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/clouds/service_catalog/paperspace_catalog.py` & `skypilot_nightly-1.0.0.dev20240602/sky/clouds/service_catalog/paperspace_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/clouds/service_catalog/runpod_catalog.py` & `skypilot_nightly-1.0.0.dev20240602/sky/clouds/service_catalog/runpod_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/clouds/service_catalog/scp_catalog.py` & `skypilot_nightly-1.0.0.dev20240602/sky/clouds/service_catalog/scp_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/clouds/service_catalog/vsphere_catalog.py` & `skypilot_nightly-1.0.0.dev20240602/sky/clouds/service_catalog/vsphere_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/clouds/utils/gcp_utils.py` & `skypilot_nightly-1.0.0.dev20240602/sky/clouds/utils/gcp_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/clouds/utils/lambda_utils.py` & `skypilot_nightly-1.0.0.dev20240602/sky/clouds/utils/lambda_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/clouds/utils/oci_utils.py` & `skypilot_nightly-1.0.0.dev20240602/sky/clouds/utils/oci_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/clouds/utils/scp_utils.py` & `skypilot_nightly-1.0.0.dev20240602/sky/clouds/utils/scp_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/clouds/vsphere.py` & `skypilot_nightly-1.0.0.dev20240602/sky/clouds/vsphere.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/core.py` & `skypilot_nightly-1.0.0.dev20240602/sky/core.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/dag.py` & `skypilot_nightly-1.0.0.dev20240602/sky/dag.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/data/data_transfer.py` & `skypilot_nightly-1.0.0.dev20240602/sky/data/data_transfer.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/data/data_utils.py` & `skypilot_nightly-1.0.0.dev20240602/sky/data/data_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/data/mounting_utils.py` & `skypilot_nightly-1.0.0.dev20240602/sky/data/mounting_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/data/storage.py` & `skypilot_nightly-1.0.0.dev20240602/sky/data/storage.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/data/storage_utils.py` & `skypilot_nightly-1.0.0.dev20240602/sky/data/storage_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/exceptions.py` & `skypilot_nightly-1.0.0.dev20240602/sky/exceptions.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/execution.py` & `skypilot_nightly-1.0.0.dev20240602/sky/execution.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/global_user_state.py` & `skypilot_nightly-1.0.0.dev20240602/sky/global_user_state.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/jobs/__init__.py` & `skypilot_nightly-1.0.0.dev20240602/sky/jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/jobs/constants.py` & `skypilot_nightly-1.0.0.dev20240602/sky/jobs/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/jobs/controller.py` & `skypilot_nightly-1.0.0.dev20240602/sky/jobs/controller.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/jobs/core.py` & `skypilot_nightly-1.0.0.dev20240602/sky/jobs/core.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/jobs/dashboard/dashboard.py` & `skypilot_nightly-1.0.0.dev20240602/sky/jobs/dashboard/dashboard.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/jobs/dashboard/static/favicon.ico` & `skypilot_nightly-1.0.0.dev20240602/sky/jobs/dashboard/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/jobs/dashboard/templates/index.html` & `skypilot_nightly-1.0.0.dev20240602/sky/jobs/dashboard/templates/index.html`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/jobs/recovery_strategy.py` & `skypilot_nightly-1.0.0.dev20240602/sky/jobs/recovery_strategy.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/jobs/state.py` & `skypilot_nightly-1.0.0.dev20240602/sky/jobs/state.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/jobs/utils.py` & `skypilot_nightly-1.0.0.dev20240602/sky/jobs/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/optimizer.py` & `skypilot_nightly-1.0.0.dev20240602/sky/optimizer.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/provision/__init__.py` & `skypilot_nightly-1.0.0.dev20240602/sky/provision/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/provision/aws/__init__.py` & `skypilot_nightly-1.0.0.dev20240602/sky/provision/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/provision/aws/config.py` & `skypilot_nightly-1.0.0.dev20240602/sky/provision/aws/config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/provision/aws/instance.py` & `skypilot_nightly-1.0.0.dev20240602/sky/provision/aws/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/provision/aws/utils.py` & `skypilot_nightly-1.0.0.dev20240602/sky/provision/aws/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/provision/azure/instance.py` & `skypilot_nightly-1.0.0.dev20240602/sky/provision/azure/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/provision/common.py` & `skypilot_nightly-1.0.0.dev20240602/sky/provision/common.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/provision/cudo/__init__.py` & `skypilot_nightly-1.0.0.dev20240602/sky/provision/cudo/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/provision/cudo/cudo_machine_type.py` & `skypilot_nightly-1.0.0.dev20240602/sky/provision/cudo/cudo_machine_type.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/provision/cudo/cudo_wrapper.py` & `skypilot_nightly-1.0.0.dev20240602/sky/provision/cudo/cudo_wrapper.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/provision/cudo/instance.py` & `skypilot_nightly-1.0.0.dev20240602/sky/provision/cudo/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/provision/docker_utils.py` & `skypilot_nightly-1.0.0.dev20240602/sky/provision/docker_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/provision/fluidstack/__init__.py` & `skypilot_nightly-1.0.0.dev20240602/sky/provision/fluidstack/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/provision/fluidstack/fluidstack_utils.py` & `skypilot_nightly-1.0.0.dev20240602/sky/provision/fluidstack/fluidstack_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/provision/fluidstack/instance.py` & `skypilot_nightly-1.0.0.dev20240602/sky/provision/fluidstack/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/provision/gcp/__init__.py` & `skypilot_nightly-1.0.0.dev20240602/sky/provision/gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/provision/gcp/config.py` & `skypilot_nightly-1.0.0.dev20240602/sky/provision/gcp/config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/provision/gcp/constants.py` & `skypilot_nightly-1.0.0.dev20240602/sky/provision/gcp/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/provision/gcp/instance.py` & `skypilot_nightly-1.0.0.dev20240602/sky/provision/gcp/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/provision/gcp/instance_utils.py` & `skypilot_nightly-1.0.0.dev20240602/sky/provision/gcp/instance_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/provision/instance_setup.py` & `skypilot_nightly-1.0.0.dev20240602/sky/provision/instance_setup.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/provision/kubernetes/__init__.py` & `skypilot_nightly-1.0.0.dev20240602/sky/provision/kubernetes/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/provision/kubernetes/config.py` & `skypilot_nightly-1.0.0.dev20240602/sky/provision/kubernetes/config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/provision/kubernetes/instance.py` & `skypilot_nightly-1.0.0.dev20240602/sky/provision/kubernetes/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/provision/kubernetes/manifests/smarter-device-manager-daemonset.yaml` & `skypilot_nightly-1.0.0.dev20240602/sky/provision/kubernetes/manifests/smarter-device-manager-daemonset.yaml`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/provision/kubernetes/network.py` & `skypilot_nightly-1.0.0.dev20240602/sky/provision/kubernetes/network.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/provision/kubernetes/network_utils.py` & `skypilot_nightly-1.0.0.dev20240602/sky/provision/kubernetes/network_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/provision/kubernetes/utils.py` & `skypilot_nightly-1.0.0.dev20240602/sky/provision/kubernetes/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/provision/logging.py` & `skypilot_nightly-1.0.0.dev20240602/sky/provision/logging.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/provision/metadata_utils.py` & `skypilot_nightly-1.0.0.dev20240602/sky/provision/metadata_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/provision/paperspace/__init__.py` & `skypilot_nightly-1.0.0.dev20240602/sky/provision/paperspace/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/provision/paperspace/config.py` & `skypilot_nightly-1.0.0.dev20240602/sky/provision/paperspace/config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/provision/paperspace/constants.py` & `skypilot_nightly-1.0.0.dev20240602/sky/provision/paperspace/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/provision/paperspace/instance.py` & `skypilot_nightly-1.0.0.dev20240602/sky/provision/paperspace/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/provision/paperspace/utils.py` & `skypilot_nightly-1.0.0.dev20240602/sky/provision/paperspace/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/provision/provisioner.py` & `skypilot_nightly-1.0.0.dev20240602/sky/provision/provisioner.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/provision/runpod/instance.py` & `skypilot_nightly-1.0.0.dev20240602/sky/provision/runpod/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/provision/runpod/utils.py` & `skypilot_nightly-1.0.0.dev20240602/sky/provision/runpod/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/provision/vsphere/__init__.py` & `skypilot_nightly-1.0.0.dev20240602/sky/provision/vsphere/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/provision/vsphere/common/cls_api_client.py` & `skypilot_nightly-1.0.0.dev20240602/sky/provision/vsphere/common/cls_api_client.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/provision/vsphere/common/cls_api_helper.py` & `skypilot_nightly-1.0.0.dev20240602/sky/provision/vsphere/common/cls_api_helper.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/provision/vsphere/common/metadata_utils.py` & `skypilot_nightly-1.0.0.dev20240602/sky/provision/vsphere/common/metadata_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/provision/vsphere/common/service_manager.py` & `skypilot_nightly-1.0.0.dev20240602/sky/provision/vsphere/common/service_manager.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/provision/vsphere/common/service_manager_factory.py` & `skypilot_nightly-1.0.0.dev20240602/sky/provision/vsphere/common/service_manager_factory.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/provision/vsphere/common/ssl_helper.py` & `skypilot_nightly-1.0.0.dev20240602/sky/provision/vsphere/common/ssl_helper.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/provision/vsphere/common/vapiconnect.py` & `skypilot_nightly-1.0.0.dev20240602/sky/provision/vsphere/common/vapiconnect.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/provision/vsphere/common/vim_utils.py` & `skypilot_nightly-1.0.0.dev20240602/sky/provision/vsphere/common/vim_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/provision/vsphere/instance.py` & `skypilot_nightly-1.0.0.dev20240602/sky/provision/vsphere/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/provision/vsphere/vsphere_utils.py` & `skypilot_nightly-1.0.0.dev20240602/sky/provision/vsphere/vsphere_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/resources.py` & `skypilot_nightly-1.0.0.dev20240602/sky/resources.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/serve/__init__.py` & `skypilot_nightly-1.0.0.dev20240602/sky/serve/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/serve/autoscalers.py` & `skypilot_nightly-1.0.0.dev20240602/sky/serve/autoscalers.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/serve/constants.py` & `skypilot_nightly-1.0.0.dev20240602/sky/serve/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/serve/controller.py` & `skypilot_nightly-1.0.0.dev20240602/sky/serve/controller.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/serve/core.py` & `skypilot_nightly-1.0.0.dev20240602/sky/serve/core.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/serve/load_balancer.py` & `skypilot_nightly-1.0.0.dev20240602/sky/serve/load_balancer.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/serve/load_balancing_policies.py` & `skypilot_nightly-1.0.0.dev20240602/sky/serve/load_balancing_policies.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/serve/replica_managers.py` & `skypilot_nightly-1.0.0.dev20240602/sky/serve/replica_managers.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/serve/serve_state.py` & `skypilot_nightly-1.0.0.dev20240602/sky/serve/serve_state.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/serve/serve_utils.py` & `skypilot_nightly-1.0.0.dev20240602/sky/serve/serve_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/serve/service.py` & `skypilot_nightly-1.0.0.dev20240602/sky/serve/service.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/serve/service_spec.py` & `skypilot_nightly-1.0.0.dev20240602/sky/serve/service_spec.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/setup_files/MANIFEST.in` & `skypilot_nightly-1.0.0.dev20240602/sky/setup_files/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/setup_files/setup.py` & `skypilot_nightly-1.0.0.dev20240602/sky/setup_files/setup.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/sky_logging.py` & `skypilot_nightly-1.0.0.dev20240602/sky/sky_logging.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/skylet/LICENSE` & `skypilot_nightly-1.0.0.dev20240602/sky/skylet/LICENSE`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/skylet/attempt_skylet.py` & `skypilot_nightly-1.0.0.dev20240602/sky/skylet/attempt_skylet.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/skylet/autostop_lib.py` & `skypilot_nightly-1.0.0.dev20240602/sky/skylet/autostop_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/skylet/configs.py` & `skypilot_nightly-1.0.0.dev20240602/sky/skylet/configs.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/skylet/constants.py` & `skypilot_nightly-1.0.0.dev20240602/sky/skylet/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/skylet/events.py` & `skypilot_nightly-1.0.0.dev20240602/sky/skylet/events.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/skylet/job_lib.py` & `skypilot_nightly-1.0.0.dev20240602/sky/skylet/job_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/skylet/log_lib.py` & `skypilot_nightly-1.0.0.dev20240602/sky/skylet/log_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/skylet/log_lib.pyi` & `skypilot_nightly-1.0.0.dev20240602/sky/skylet/log_lib.pyi`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/skylet/providers/azure/azure-config-template.json` & `skypilot_nightly-1.0.0.dev20240602/sky/skylet/providers/azure/azure-config-template.json`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/skylet/providers/azure/azure-vm-template.json` & `skypilot_nightly-1.0.0.dev20240602/sky/skylet/providers/azure/azure-vm-template.json`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/skylet/providers/azure/config.py` & `skypilot_nightly-1.0.0.dev20240602/sky/skylet/providers/azure/config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/skylet/providers/azure/node_provider.py` & `skypilot_nightly-1.0.0.dev20240602/sky/skylet/providers/azure/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/skylet/providers/command_runner.py` & `skypilot_nightly-1.0.0.dev20240602/sky/skylet/providers/command_runner.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/skylet/providers/ibm/node_provider.py` & `skypilot_nightly-1.0.0.dev20240602/sky/skylet/providers/ibm/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/skylet/providers/ibm/utils.py` & `skypilot_nightly-1.0.0.dev20240602/sky/skylet/providers/ibm/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/skylet/providers/ibm/vpc_provider.py` & `skypilot_nightly-1.0.0.dev20240602/sky/skylet/providers/ibm/vpc_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/skylet/providers/lambda_cloud/node_provider.py` & `skypilot_nightly-1.0.0.dev20240602/sky/skylet/providers/lambda_cloud/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/skylet/providers/oci/node_provider.py` & `skypilot_nightly-1.0.0.dev20240602/sky/skylet/providers/oci/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/skylet/providers/oci/query_helper.py` & `skypilot_nightly-1.0.0.dev20240602/sky/skylet/providers/oci/query_helper.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/skylet/providers/scp/config.py` & `skypilot_nightly-1.0.0.dev20240602/sky/skylet/providers/scp/config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/skylet/providers/scp/node_provider.py` & `skypilot_nightly-1.0.0.dev20240602/sky/skylet/providers/scp/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/skylet/ray_patches/__init__.py` & `skypilot_nightly-1.0.0.dev20240602/sky/skylet/ray_patches/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/skylet/ray_patches/log_monitor.py.patch` & `skypilot_nightly-1.0.0.dev20240602/sky/skylet/ray_patches/log_monitor.py.patch`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/skylet/ray_patches/resource_demand_scheduler.py.patch` & `skypilot_nightly-1.0.0.dev20240602/sky/skylet/ray_patches/resource_demand_scheduler.py.patch`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/skylet/ray_patches/worker.py.patch` & `skypilot_nightly-1.0.0.dev20240602/sky/skylet/ray_patches/worker.py.patch`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/skylet/skylet.py` & `skypilot_nightly-1.0.0.dev20240602/sky/skylet/skylet.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/skylet/subprocess_daemon.py` & `skypilot_nightly-1.0.0.dev20240602/sky/skylet/subprocess_daemon.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/skypilot_config.py` & `skypilot_nightly-1.0.0.dev20240602/sky/skypilot_config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/status_lib.py` & `skypilot_nightly-1.0.0.dev20240602/sky/status_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/task.py` & `skypilot_nightly-1.0.0.dev20240602/sky/task.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/templates/aws-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240602/sky/templates/aws-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/templates/azure-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240602/sky/templates/azure-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/templates/cudo-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240602/sky/templates/cudo-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/templates/fluidstack-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240602/sky/templates/fluidstack-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/templates/gcp-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240602/sky/templates/gcp-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/templates/ibm-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240602/sky/templates/ibm-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/templates/jobs-controller.yaml.j2` & `skypilot_nightly-1.0.0.dev20240602/sky/templates/jobs-controller.yaml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/templates/kubernetes-ingress.yml.j2` & `skypilot_nightly-1.0.0.dev20240602/sky/templates/kubernetes-ingress.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/templates/kubernetes-port-forward-proxy-command.sh.j2` & `skypilot_nightly-1.0.0.dev20240602/sky/templates/kubernetes-port-forward-proxy-command.sh.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/templates/kubernetes-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240602/sky/templates/kubernetes-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/templates/kubernetes-ssh-jump.yml.j2` & `skypilot_nightly-1.0.0.dev20240602/sky/templates/kubernetes-ssh-jump.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/templates/lambda-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240602/sky/templates/lambda-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/templates/local-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240602/sky/templates/local-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/templates/oci-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240602/sky/templates/oci-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/templates/paperspace-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240602/sky/templates/paperspace-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/templates/runpod-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240602/sky/templates/runpod-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/templates/scp-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240602/sky/templates/scp-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/templates/sky-serve-controller.yaml.j2` & `skypilot_nightly-1.0.0.dev20240602/sky/templates/sky-serve-controller.yaml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/templates/vsphere-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240602/sky/templates/vsphere-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/usage/constants.py` & `skypilot_nightly-1.0.0.dev20240602/sky/usage/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/usage/usage_lib.py` & `skypilot_nightly-1.0.0.dev20240602/sky/usage/usage_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/utils/accelerator_registry.py` & `skypilot_nightly-1.0.0.dev20240602/sky/utils/accelerator_registry.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/utils/cli_utils/status_utils.py` & `skypilot_nightly-1.0.0.dev20240602/sky/utils/cli_utils/status_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/utils/cluster_yaml_utils.py` & `skypilot_nightly-1.0.0.dev20240602/sky/utils/cluster_yaml_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/utils/command_runner.py` & `skypilot_nightly-1.0.0.dev20240602/sky/utils/command_runner.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/utils/command_runner.pyi` & `skypilot_nightly-1.0.0.dev20240602/sky/utils/command_runner.pyi`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/utils/common_utils.py` & `skypilot_nightly-1.0.0.dev20240602/sky/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/utils/controller_utils.py` & `skypilot_nightly-1.0.0.dev20240602/sky/utils/controller_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/utils/dag_utils.py` & `skypilot_nightly-1.0.0.dev20240602/sky/utils/dag_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/utils/db_utils.py` & `skypilot_nightly-1.0.0.dev20240602/sky/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/utils/env_options.py` & `skypilot_nightly-1.0.0.dev20240602/sky/utils/env_options.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/utils/kubernetes/create_cluster.sh` & `skypilot_nightly-1.0.0.dev20240602/sky/utils/kubernetes/create_cluster.sh`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/utils/kubernetes/delete_cluster.sh` & `skypilot_nightly-1.0.0.dev20240602/sky/utils/kubernetes/delete_cluster.sh`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/utils/kubernetes/generate_kind_config.py` & `skypilot_nightly-1.0.0.dev20240602/sky/utils/kubernetes/generate_kind_config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/utils/kubernetes/generate_static_kubeconfig.sh` & `skypilot_nightly-1.0.0.dev20240602/sky/utils/kubernetes/generate_static_kubeconfig.sh`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/utils/kubernetes/gpu_labeler.py` & `skypilot_nightly-1.0.0.dev20240602/sky/utils/kubernetes/gpu_labeler.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/utils/kubernetes/k8s_gpu_labeler_job.yaml` & `skypilot_nightly-1.0.0.dev20240602/sky/utils/kubernetes/k8s_gpu_labeler_job.yaml`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/utils/kubernetes/k8s_gpu_labeler_setup.yaml` & `skypilot_nightly-1.0.0.dev20240602/sky/utils/kubernetes/k8s_gpu_labeler_setup.yaml`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/utils/kubernetes/ssh_jump_lifecycle_manager.py` & `skypilot_nightly-1.0.0.dev20240602/sky/utils/kubernetes/ssh_jump_lifecycle_manager.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/utils/kubernetes_enums.py` & `skypilot_nightly-1.0.0.dev20240602/sky/utils/kubernetes_enums.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/utils/log_utils.py` & `skypilot_nightly-1.0.0.dev20240602/sky/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/utils/resources_utils.py` & `skypilot_nightly-1.0.0.dev20240602/sky/utils/resources_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/utils/rich_utils.py` & `skypilot_nightly-1.0.0.dev20240602/sky/utils/rich_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/utils/schemas.py` & `skypilot_nightly-1.0.0.dev20240602/sky/utils/schemas.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/utils/subprocess_utils.py` & `skypilot_nightly-1.0.0.dev20240602/sky/utils/subprocess_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/utils/timeline.py` & `skypilot_nightly-1.0.0.dev20240602/sky/utils/timeline.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/utils/ux_utils.py` & `skypilot_nightly-1.0.0.dev20240602/sky/utils/ux_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/sky/utils/validator.py` & `skypilot_nightly-1.0.0.dev20240602/sky/utils/validator.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/skypilot_nightly.egg-info/PKG-INFO` & `skypilot_nightly-1.0.0.dev20240602/skypilot_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skypilot-nightly
-Version: 1.0.0.dev20240601
+Version: 1.0.0.dev20240602
 Summary: SkyPilot: An intercloud broker for the clouds
 Author: SkyPilot Team
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/skypilot-org/skypilot
 Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
 Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
 Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
```

### Comparing `skypilot_nightly-1.0.0.dev20240601/skypilot_nightly.egg-info/SOURCES.txt` & `skypilot_nightly-1.0.0.dev20240602/skypilot_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/skypilot_nightly.egg-info/requires.txt` & `skypilot_nightly-1.0.0.dev20240602/skypilot_nightly.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/tests/test_cli.py` & `skypilot_nightly-1.0.0.dev20240602/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/tests/test_config.py` & `skypilot_nightly-1.0.0.dev20240602/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/tests/test_jobs.py` & `skypilot_nightly-1.0.0.dev20240602/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/tests/test_jobs_and_serve.py` & `skypilot_nightly-1.0.0.dev20240602/tests/test_jobs_and_serve.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/tests/test_list_accelerators.py` & `skypilot_nightly-1.0.0.dev20240602/tests/test_list_accelerators.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/tests/test_optimizer_dryruns.py` & `skypilot_nightly-1.0.0.dev20240602/tests/test_optimizer_dryruns.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/tests/test_optimizer_random_dag.py` & `skypilot_nightly-1.0.0.dev20240602/tests/test_optimizer_random_dag.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/tests/test_serve_autoscaler.py` & `skypilot_nightly-1.0.0.dev20240602/tests/test_serve_autoscaler.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/tests/test_smoke.py` & `skypilot_nightly-1.0.0.dev20240602/tests/test_smoke.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/tests/test_storage.py` & `skypilot_nightly-1.0.0.dev20240602/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/tests/test_wheels.py` & `skypilot_nightly-1.0.0.dev20240602/tests/test_wheels.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240601/tests/test_yaml_parser.py` & `skypilot_nightly-1.0.0.dev20240602/tests/test_yaml_parser.py`

 * *Files identical despite different names*

