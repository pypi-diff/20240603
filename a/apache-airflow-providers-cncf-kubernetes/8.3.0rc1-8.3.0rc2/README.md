# Comparing `tmp/apache_airflow_providers_cncf_kubernetes-8.3.0rc1.tar.gz` & `tmp/apache_airflow_providers_cncf_kubernetes-8.3.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_cncf_kubernetes-8.3.0rc1.tar", last modified: Tue May 21 10:24:02 2024, max compression
+gzip compressed data, was "apache_airflow_providers_cncf_kubernetes-8.3.0rc2.tar", last modified: Tue May 21 10:24:02 2024, max compression
```

## Comparing `apache_airflow_providers_cncf_kubernetes-8.3.0rc1.tar` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc2.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0     3341 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/README.rst
--rw-r--r--   0        0        0    13569 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/LICENSE
--rw-r--r--   0        0        0     1502 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/__init__.py
--rw-r--r--   0        0        0      785 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/backcompat/__init__.py
--rw-r--r--   0        0        0     4340 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/backcompat/backwards_compat_converters.py
--rw-r--r--   0        0        0     4094 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/callbacks.py
--rw-r--r--   0        0        0      785 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/cli/__init__.py
--rw-r--r--   0        0        0     6984 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/cli/kubernetes_command.py
--rw-r--r--   0        0        0      787 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/decorators/__init__.py
--rw-r--r--   0        0        0     5780 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/decorators/kubernetes.py
--rw-r--r--   0        0        0      787 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/executors/__init__.py
--rw-r--r--   0        0        0    33257 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor.py
--rw-r--r--   0        0        0     1673 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor_types.py
--rw-r--r--   0        0        0    23442 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor_utils.py
--rw-r--r--   0        0        0    10014 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/executors/local_kubernetes_executor.py
--rw-r--r--   0        0        0    17796 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/get_provider_info.py
--rw-r--r--   0        0        0      785 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/hooks/__init__.py
--rw-r--r--   0        0        0    31879 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/hooks/kubernetes.py
--rw-r--r--   0        0        0     2101 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/k8s_model.py
--rw-r--r--   0        0        0     5329 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/kube_client.py
--rw-r--r--   0        0        0     5225 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/kube_config.py
--rw-r--r--   0        0        0      785 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/kubernetes_executor_templates/__init__.py
--rw-r--r--   0        0        0     2567 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/kubernetes_executor_templates/basic_template.yaml
--rw-r--r--   0        0        0     6765 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/kubernetes_helper_functions.py
--rw-r--r--   0        0        0      787 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/operators/__init__.py
--rw-r--r--   0        0        0    15311 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/operators/custom_object_launcher.py
--rw-r--r--   0        0        0    21432 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/operators/job.py
--rw-r--r--   0        0        0     1269 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/operators/kubernetes_pod.py
--rw-r--r--   0        0        0    51654 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/operators/pod.py
--rw-r--r--   0        0        0     7570 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/operators/resource.py
--rw-r--r--   0        0        0    13262 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/operators/spark_kubernetes.py
--rw-r--r--   0        0        0    24380 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/pod_generator.py
--rw-r--r--   0        0        0    11998 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/pod_generator_deprecated.py
--rw-r--r--   0        0        0    12039 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/pod_launcher_deprecated.py
--rw-r--r--   0        0        0      785 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/pod_template_file_examples/__init__.py
--rw-r--r--   0        0        0     2256 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/pod_template_file_examples/dags_in_image_template.yaml
--rw-r--r--   0        0        0     2442 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/pod_template_file_examples/dags_in_volume_template.yaml
--rw-r--r--   0        0        0     3020 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/pod_template_file_examples/git_sync_template.yaml
--rw-r--r--   0        0        0     1741 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.jinja2
--rw-r--r--   0        0        0     3460 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.py
--rw-r--r--   0        0        0      785 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/resource_convert/__init__.py
--rw-r--r--   0        0        0     1873 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/resource_convert/configmap.py
--rw-r--r--   0        0        0     1464 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/resource_convert/env_variable.py
--rw-r--r--   0        0        0     1494 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/resource_convert/secret.py
--rw-r--r--   0        0        0     5209 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/secret.py
--rw-r--r--   0        0        0      785 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/sensors/__init__.py
--rw-r--r--   0        0        0     5552 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/sensors/spark_kubernetes.py
--rw-r--r--   0        0        0     2965 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/template_rendering.py
--rw-r--r--   0        0        0      785 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/triggers/__init__.py
--rw-r--r--   0        0        0     4060 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/triggers/job.py
--rw-r--r--   0        0        0     1266 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/triggers/kubernetes_pod.py
--rw-r--r--   0        0        0    13670 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/triggers/pod.py
--rw-r--r--   0        0        0      863 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/utils/__init__.py
--rw-r--r--   0        0        0     5195 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/utils/delete_from.py
--rw-r--r--   0        0        0     1928 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/utils/k8s_resource_iterator.py
--rw-r--r--   0        0        0    33608 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/utils/pod_manager.py
--rw-r--r--   0        0        0     2519 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/utils/xcom_sidecar.py
--rw-r--r--   0        0        0     3178 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/pyproject.toml
--rw-r--r--   0        0        0     5268 1970-01-01 00:00:00.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     3341 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc2/README.rst
+-rw-r--r--   0        0        0    13569 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/LICENSE
+-rw-r--r--   0        0        0     1502 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/__init__.py
+-rw-r--r--   0        0        0      785 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/backcompat/__init__.py
+-rw-r--r--   0        0        0     4340 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/backcompat/backwards_compat_converters.py
+-rw-r--r--   0        0        0     4094 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/callbacks.py
+-rw-r--r--   0        0        0      785 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/cli/__init__.py
+-rw-r--r--   0        0        0     6984 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/cli/kubernetes_command.py
+-rw-r--r--   0        0        0      787 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/decorators/__init__.py
+-rw-r--r--   0        0        0     5780 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/decorators/kubernetes.py
+-rw-r--r--   0        0        0      787 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/executors/__init__.py
+-rw-r--r--   0        0        0    33257 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/executors/kubernetes_executor.py
+-rw-r--r--   0        0        0     1673 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/executors/kubernetes_executor_types.py
+-rw-r--r--   0        0        0    23442 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/executors/kubernetes_executor_utils.py
+-rw-r--r--   0        0        0    10014 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/executors/local_kubernetes_executor.py
+-rw-r--r--   0        0        0    17796 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/get_provider_info.py
+-rw-r--r--   0        0        0      785 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/hooks/__init__.py
+-rw-r--r--   0        0        0    31879 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/hooks/kubernetes.py
+-rw-r--r--   0        0        0     2101 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/k8s_model.py
+-rw-r--r--   0        0        0     5329 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/kube_client.py
+-rw-r--r--   0        0        0     5225 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/kube_config.py
+-rw-r--r--   0        0        0      785 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/kubernetes_executor_templates/__init__.py
+-rw-r--r--   0        0        0     2567 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/kubernetes_executor_templates/basic_template.yaml
+-rw-r--r--   0        0        0     6765 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/kubernetes_helper_functions.py
+-rw-r--r--   0        0        0      787 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/operators/__init__.py
+-rw-r--r--   0        0        0    15311 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/operators/custom_object_launcher.py
+-rw-r--r--   0        0        0    21432 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/operators/job.py
+-rw-r--r--   0        0        0     1269 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/operators/kubernetes_pod.py
+-rw-r--r--   0        0        0    52102 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/operators/pod.py
+-rw-r--r--   0        0        0     7570 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/operators/resource.py
+-rw-r--r--   0        0        0    13262 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/operators/spark_kubernetes.py
+-rw-r--r--   0        0        0    24380 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/pod_generator.py
+-rw-r--r--   0        0        0    11998 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/pod_generator_deprecated.py
+-rw-r--r--   0        0        0    12039 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/pod_launcher_deprecated.py
+-rw-r--r--   0        0        0      785 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/pod_template_file_examples/__init__.py
+-rw-r--r--   0        0        0     2256 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/pod_template_file_examples/dags_in_image_template.yaml
+-rw-r--r--   0        0        0     2442 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/pod_template_file_examples/dags_in_volume_template.yaml
+-rw-r--r--   0        0        0     3020 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/pod_template_file_examples/git_sync_template.yaml
+-rw-r--r--   0        0        0     1741 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/python_kubernetes_script.jinja2
+-rw-r--r--   0        0        0     3460 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/python_kubernetes_script.py
+-rw-r--r--   0        0        0      785 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/resource_convert/__init__.py
+-rw-r--r--   0        0        0     1873 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/resource_convert/configmap.py
+-rw-r--r--   0        0        0     1464 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/resource_convert/env_variable.py
+-rw-r--r--   0        0        0     1494 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/resource_convert/secret.py
+-rw-r--r--   0        0        0     5209 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/secret.py
+-rw-r--r--   0        0        0      785 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/sensors/__init__.py
+-rw-r--r--   0        0        0     5552 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/sensors/spark_kubernetes.py
+-rw-r--r--   0        0        0     2965 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/template_rendering.py
+-rw-r--r--   0        0        0      785 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/triggers/__init__.py
+-rw-r--r--   0        0        0     4060 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/triggers/job.py
+-rw-r--r--   0        0        0     1266 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/triggers/kubernetes_pod.py
+-rw-r--r--   0        0        0    13670 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/triggers/pod.py
+-rw-r--r--   0        0        0      863 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/utils/__init__.py
+-rw-r--r--   0        0        0     5195 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/utils/delete_from.py
+-rw-r--r--   0        0        0     1928 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/utils/k8s_resource_iterator.py
+-rw-r--r--   0        0        0    33669 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/utils/pod_manager.py
+-rw-r--r--   0        0        0     2519 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/utils/xcom_sidecar.py
+-rw-r--r--   0        0        0     3178 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     5268 1970-01-01 00:00:00.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc2/PKG-INFO
```

### Comparing `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/README.rst` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-cncf-kubernetes``
 
-Release: ``8.3.0.rc1``
+Release: ``8.3.0.rc2``
 
 
 `Kubernetes <https://kubernetes.io/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/LICENSE` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/__init__.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/backcompat/__init__.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/backcompat/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/backcompat/backwards_compat_converters.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/backcompat/backwards_compat_converters.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/callbacks.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/callbacks.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/cli/__init__.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/cli/kubernetes_command.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/cli/kubernetes_command.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/decorators/__init__.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/decorators/kubernetes.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/decorators/kubernetes.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/executors/__init__.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/executors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/executors/kubernetes_executor.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor_types.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/executors/kubernetes_executor_types.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor_utils.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/executors/kubernetes_executor_utils.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/executors/local_kubernetes_executor.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/executors/local_kubernetes_executor.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/get_provider_info.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/hooks/__init__.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/hooks/kubernetes.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/hooks/kubernetes.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/k8s_model.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/k8s_model.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/kube_client.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/kube_client.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/kube_config.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/kube_config.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/kubernetes_executor_templates/__init__.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/kubernetes_executor_templates/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/kubernetes_executor_templates/basic_template.yaml` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/kubernetes_executor_templates/basic_template.yaml`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/kubernetes_helper_functions.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/kubernetes_helper_functions.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/operators/__init__.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/operators/custom_object_launcher.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/operators/custom_object_launcher.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/operators/job.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/operators/job.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/operators/kubernetes_pod.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/operators/kubernetes_pod.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/operators/pod.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/operators/pod.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 from functools import cached_property
 from typing import TYPE_CHECKING, Any, Callable, Iterable, Sequence
 
 import kubernetes
 import tenacity
 from deprecated import deprecated
 from kubernetes.client import CoreV1Api, V1Pod, models as k8s
+from kubernetes.client.exceptions import ApiException
 from kubernetes.stream import stream
 from urllib3.exceptions import HTTPError
 
 from airflow.configuration import conf
 from airflow.exceptions import (
     AirflowException,
     AirflowProviderDeprecationWarning,
@@ -784,17 +785,26 @@
     def _clean(self, event: dict[str, Any]) -> None:
         if event["status"] == "running":
             return
         istio_enabled = self.is_istio_enabled(self.pod)
         # Skip await_pod_completion when the event is 'timeout' due to the pod can hang
         # on the ErrImagePull or ContainerCreating step and it will never complete
         if event["status"] != "timeout":
-            self.pod = self.pod_manager.await_pod_completion(
-                self.pod, istio_enabled, self.base_container_name
-            )
+            try:
+                self.pod = self.pod_manager.await_pod_completion(
+                    self.pod, istio_enabled, self.base_container_name
+                )
+            except ApiException as e:
+                if e.status == 404:
+                    self.pod = None
+                    self.log.warning(
+                        "Pod not found while waiting for completion. The last status was %r", event["status"]
+                    )
+                else:
+                    raise e
         if self.pod is not None:
             self.post_complete_action(
                 pod=self.pod,
                 remote_pod=self.pod,
             )
 
     def _write_logs(self, pod: k8s.V1Pod, follow: bool = False, since_time: DateTime | None = None) -> None:
@@ -803,30 +813,29 @@
                 math.ceil((datetime.datetime.now(tz=datetime.timezone.utc) - since_time).total_seconds())
                 if since_time
                 else None
             )
             logs = self.client.read_namespaced_pod_log(
                 name=pod.metadata.name,
                 namespace=pod.metadata.namespace,
-                pod=pod,
-                container_name=self.base_container_name,
+                container=self.base_container_name,
                 follow=follow,
                 timestamps=False,
                 since_seconds=since_seconds,
                 _preload_content=False,
             )
             for raw_line in logs:
                 line = raw_line.decode("utf-8", errors="backslashreplace").rstrip("\n")
                 if line:
                     self.log.info("[%s] logs: %s", self.base_container_name, line)
-        except HTTPError as e:
+        except (HTTPError, ApiException) as e:
             self.log.warning(
                 "Reading of logs interrupted with error %r; will retry. "
                 "Set log level to DEBUG for traceback.",
-                e,
+                e if not isinstance(e, ApiException) else e.reason,
             )
 
     def post_complete_action(self, *, pod, remote_pod, **kwargs) -> None:
         """Actions that must be done after operator finishes logic of the deferrable_execution."""
         self.cleanup(
             pod=pod,
             remote_pod=remote_pod,
```

### Comparing `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/operators/resource.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/operators/resource.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/operators/spark_kubernetes.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/operators/spark_kubernetes.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/pod_generator.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/pod_generator.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/pod_generator_deprecated.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/pod_generator_deprecated.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/pod_launcher_deprecated.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/pod_launcher_deprecated.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/pod_template_file_examples/__init__.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/pod_template_file_examples/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/pod_template_file_examples/dags_in_image_template.yaml` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/pod_template_file_examples/dags_in_image_template.yaml`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/pod_template_file_examples/dags_in_volume_template.yaml` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/pod_template_file_examples/dags_in_volume_template.yaml`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/pod_template_file_examples/git_sync_template.yaml` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/pod_template_file_examples/git_sync_template.yaml`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.jinja2` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/python_kubernetes_script.jinja2`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/python_kubernetes_script.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/resource_convert/__init__.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/resource_convert/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/resource_convert/configmap.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/resource_convert/configmap.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/resource_convert/env_variable.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/resource_convert/env_variable.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/resource_convert/secret.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/resource_convert/secret.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/secret.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/secret.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/sensors/__init__.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/sensors/spark_kubernetes.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/sensors/spark_kubernetes.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/template_rendering.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/template_rendering.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/triggers/__init__.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/triggers/job.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/triggers/job.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/triggers/kubernetes_pod.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/triggers/kubernetes_pod.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/triggers/pod.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/triggers/pod.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/utils/__init__.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/utils/delete_from.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/utils/delete_from.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/utils/k8s_resource_iterator.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/utils/k8s_resource_iterator.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/utils/pod_manager.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/utils/pod_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -512,15 +512,15 @@
                 return PodLoggingStatus(running=False, last_log_time=last_log_time)
             if not follow:
                 return PodLoggingStatus(running=True, last_log_time=last_log_time)
             else:
                 # a timeout is a normal thing and we ignore it and resume following logs
                 if not isinstance(exc, TimeoutError):
                     self.log.warning(
-                        "Pod %s log read interrupted but container %s still running",
+                        "Pod %s log read interrupted but container %s still running. Logs generated in the last one second might get duplicated.",
                         pod.metadata.name,
                         container_name,
                     )
                 time.sleep(1)
 
     def _reconcile_requested_log_containers(
         self, requested: Iterable[str] | str | bool, actual: list[str], pod_name
```

### Comparing `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/utils/xcom_sidecar.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc2/airflow/providers/cncf/kubernetes/utils/xcom_sidecar.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/pyproject.toml` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-cncf-kubernetes"
-version = "8.3.0.rc1"
+version = "8.3.0.rc2"
 description = "Provider package apache-airflow-providers-cncf-kubernetes for Apache Airflow"
 readme = "README.rst"
 authors = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
 ]
 maintainers = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
```

### Comparing `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/PKG-INFO` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-cncf-kubernetes
-Version: 8.3.0rc1
+Version: 8.3.0rc2
 Summary: Provider package apache-airflow-providers-cncf-kubernetes for Apache Airflow
 Keywords: airflow-provider,cncf.kubernetes,airflow,integration
 Author-email: Apache Software Foundation <dev@airflow.apache.org>
 Maintainer-email: Apache Software Foundation <dev@airflow.apache.org>
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
@@ -76,15 +76,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-cncf-kubernetes``
 
-Release: ``8.3.0.rc1``
+Release: ``8.3.0.rc2``
 
 
 `Kubernetes <https://kubernetes.io/>`__
 
 
 Provider package
 ----------------
```

