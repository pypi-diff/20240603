# Comparing `tmp/koku-nise-4.5.2.tar.gz` & `tmp/koku-nise-4.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "koku-nise-4.5.2.tar", last modified: Wed May 22 13:27:12 2024, max compression
+gzip compressed data, was "koku-nise-4.5.3.tar", last modified: Mon Jun  3 12:26:24 2024, max compression
```

## Comparing `koku-nise-4.5.2.tar` & `koku-nise-4.5.3.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:27:12.083281 koku-nise-4.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)    34520 2024-05-22 13:26:58.000000 koku-nise-4.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-22 13:26:58.000000 koku-nise-4.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-22 13:27:12.083281 koku-nise-4.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9834 2024-05-22 13:26:58.000000 koku-nise-4.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:27:12.071281 koku-nise-4.5.2/koku_nise.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-22 13:27:11.000000 koku-nise-4.5.2/koku_nise.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-05-22 13:27:12.000000 koku-nise-4.5.2/koku_nise.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 13:27:11.000000 koku-nise-4.5.2/koku_nise.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-22 13:27:11.000000 koku-nise-4.5.2/koku_nise.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 13:27:11.000000 koku-nise-4.5.2/koku_nise.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-22 13:27:11.000000 koku-nise-4.5.2/koku_nise.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-22 13:27:11.000000 koku-nise-4.5.2/koku_nise.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:27:12.071281 koku-nise-4.5.2/nise/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28971 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/aws-template-manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/copy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5677 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/extract.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:27:12.071281 koku-nise-4.5.2/nise/generators/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/generators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:27:12.075281 koku-nise-4.5.2/nise/generators/aws/
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/generators/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/generators/aws/aws_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    13560 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/generators/aws/aws_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5950 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/generators/aws/data_transfer_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/generators/aws/ebs_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7014 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/generators/aws/ec2_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7315 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/generators/aws/marketplace_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6495 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/generators/aws/rds_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/generators/aws/route53_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4009 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/generators/aws/s3_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4637 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/generators/aws/vpc_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:27:12.075281 koku-nise-4.5.2/nise/generators/azure/
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/generators/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17226 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/generators/azure/azure_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/generators/azure/bandwidth_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/generators/azure/ccsp_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/generators/azure/data_transfer_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/generators/azure/managed_disk_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/generators/azure/sql_database_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/generators/azure/storage_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/generators/azure/virtual_machine_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/generators/azure/virtual_network_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:27:12.079281 koku-nise-4.5.2/nise/generators/gcp/
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/generators/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7594 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/generators/gcp/cloud_storage_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9603 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/generators/gcp/compute_engine_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7860 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/generators/gcp/gcp_database_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    11867 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/generators/gcp/gcp_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8099 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/generators/gcp/gcp_network_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/generators/gcp/hcs_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/generators/gcp/project_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5287 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/generators/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:27:12.079281 koku-nise-4.5.2/nise/generators/oci/
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/generators/oci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/generators/oci/oci_block_storage_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/generators/oci/oci_compute_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/generators/oci/oci_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/generators/oci/oci_database_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    10817 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/generators/oci/oci_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/generators/oci/oci_network_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:27:12.079281 koku-nise-4.5.2/nise/generators/ocp/
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/generators/ocp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    43084 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/generators/ocp/ocp_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)    56331 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/report.py
--rw-r--r--   0 runner    (1001) docker     (127)    15635 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:27:12.079281 koku-nise-4.5.2/nise/util/
--rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/util/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     7688 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/yaml_gen.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:27:12.079281 koku-nise-4.5.2/nise/yaml_generators/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/yaml_generators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:27:12.079281 koku-nise-4.5.2/nise/yaml_generators/aws/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/yaml_generators/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    71376 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/yaml_generators/aws/ec2_instance_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     9814 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/yaml_generators/aws/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    13953 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/yaml_generators/aws/rds_instance_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/yaml_generators/aws/regions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:27:12.079281 koku-nise-4.5.2/nise/yaml_generators/azure/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/yaml_generators/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7923 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/yaml_generators/azure/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:27:12.079281 koku-nise-4.5.2/nise/yaml_generators/gcp/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/yaml_generators/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/yaml_generators/gcp/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/yaml_generators/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:27:12.083281 koku-nise-4.5.2/nise/yaml_generators/oci/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/yaml_generators/oci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5636 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/yaml_generators/oci/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/yaml_generators/oci/oci_yaml_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:27:12.083281 koku-nise-4.5.2/nise/yaml_generators/ocp/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/yaml_generators/ocp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12882 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/yaml_generators/ocp/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:27:12.083281 koku-nise-4.5.2/nise/yaml_generators/ocp_on_cloud/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/yaml_generators/ocp_on_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/yaml_generators/ocp_on_cloud/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:27:12.083281 koku-nise-4.5.2/nise/yaml_generators/static/
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/yaml_generators/static/aws_generator_config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/yaml_generators/static/aws_static_data.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/yaml_generators/static/azure_generator_config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/yaml_generators/static/azure_static_data.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/yaml_generators/static/gcp_generator_config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/yaml_generators/static/gcp_static_data.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/yaml_generators/static/oci_generator_config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/yaml_generators/static/oci_static_data.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/yaml_generators/static/ocp_generator_config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/yaml_generators/static/ocp_on_cloud_options.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/yaml_generators/static/ocp_static_data.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     4366 2024-05-22 13:26:58.000000 koku-nise-4.5.2/nise/yaml_generators/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 13:27:12.083281 koku-nise-4.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-05-22 13:26:58.000000 koku-nise-4.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:26:24.925447 koku-nise-4.5.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    34520 2024-06-03 12:26:06.000000 koku-nise-4.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-06-03 12:26:06.000000 koku-nise-4.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-06-03 12:26:24.925447 koku-nise-4.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9834 2024-06-03 12:26:06.000000 koku-nise-4.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:26:24.913447 koku-nise-4.5.3/koku_nise.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-06-03 12:26:24.000000 koku-nise-4.5.3/koku_nise.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-06-03 12:26:24.000000 koku-nise-4.5.3/koku_nise.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 12:26:24.000000 koku-nise-4.5.3/koku_nise.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-06-03 12:26:24.000000 koku-nise-4.5.3/koku_nise.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 12:26:24.000000 koku-nise-4.5.3/koku_nise.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-06-03 12:26:24.000000 koku-nise-4.5.3/koku_nise.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-06-03 12:26:24.000000 koku-nise-4.5.3/koku_nise.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:26:24.913447 koku-nise-4.5.3/nise/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28971 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/aws-template-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/copy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5677 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/extract.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:26:24.913447 koku-nise-4.5.3/nise/generators/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/generators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:26:24.917447 koku-nise-4.5.3/nise/generators/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/generators/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/generators/aws/aws_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13560 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/generators/aws/aws_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5950 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/generators/aws/data_transfer_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/generators/aws/ebs_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7014 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/generators/aws/ec2_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7315 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/generators/aws/marketplace_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6495 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/generators/aws/rds_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/generators/aws/route53_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4009 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/generators/aws/s3_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4637 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/generators/aws/vpc_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:26:24.917447 koku-nise-4.5.3/nise/generators/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/generators/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17226 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/generators/azure/azure_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/generators/azure/bandwidth_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/generators/azure/ccsp_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/generators/azure/data_transfer_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/generators/azure/managed_disk_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/generators/azure/sql_database_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/generators/azure/storage_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/generators/azure/virtual_machine_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/generators/azure/virtual_network_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:26:24.921447 koku-nise-4.5.3/nise/generators/gcp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/generators/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7594 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/generators/gcp/cloud_storage_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10226 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/generators/gcp/compute_engine_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7860 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/generators/gcp/gcp_database_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11867 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/generators/gcp/gcp_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8099 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/generators/gcp/gcp_network_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/generators/gcp/hcs_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/generators/gcp/project_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5287 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/generators/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:26:24.921447 koku-nise-4.5.3/nise/generators/oci/
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/generators/oci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/generators/oci/oci_block_storage_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/generators/oci/oci_compute_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/generators/oci/oci_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/generators/oci/oci_database_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10817 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/generators/oci/oci_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/generators/oci/oci_network_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:26:24.921447 koku-nise-4.5.3/nise/generators/ocp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/generators/ocp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43084 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/generators/ocp/ocp_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56331 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15635 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:26:24.921447 koku-nise-4.5.3/nise/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/util/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7688 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/yaml_gen.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:26:24.921447 koku-nise-4.5.3/nise/yaml_generators/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/yaml_generators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:26:24.921447 koku-nise-4.5.3/nise/yaml_generators/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/yaml_generators/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71376 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/yaml_generators/aws/ec2_instance_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9814 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/yaml_generators/aws/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13953 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/yaml_generators/aws/rds_instance_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/yaml_generators/aws/regions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:26:24.925447 koku-nise-4.5.3/nise/yaml_generators/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/yaml_generators/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7923 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/yaml_generators/azure/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:26:24.925447 koku-nise-4.5.3/nise/yaml_generators/gcp/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/yaml_generators/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/yaml_generators/gcp/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/yaml_generators/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:26:24.925447 koku-nise-4.5.3/nise/yaml_generators/oci/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/yaml_generators/oci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5636 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/yaml_generators/oci/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/yaml_generators/oci/oci_yaml_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:26:24.925447 koku-nise-4.5.3/nise/yaml_generators/ocp/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/yaml_generators/ocp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12882 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/yaml_generators/ocp/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:26:24.925447 koku-nise-4.5.3/nise/yaml_generators/ocp_on_cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/yaml_generators/ocp_on_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/yaml_generators/ocp_on_cloud/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:26:24.925447 koku-nise-4.5.3/nise/yaml_generators/static/
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/yaml_generators/static/aws_generator_config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/yaml_generators/static/aws_static_data.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/yaml_generators/static/azure_generator_config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/yaml_generators/static/azure_static_data.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/yaml_generators/static/gcp_generator_config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/yaml_generators/static/gcp_static_data.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/yaml_generators/static/oci_generator_config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/yaml_generators/static/oci_static_data.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/yaml_generators/static/ocp_generator_config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/yaml_generators/static/ocp_on_cloud_options.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/yaml_generators/static/ocp_static_data.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     4366 2024-06-03 12:26:06.000000 koku-nise-4.5.3/nise/yaml_generators/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 12:26:24.925447 koku-nise-4.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-06-03 12:26:06.000000 koku-nise-4.5.3/setup.py
```

### Comparing `koku-nise-4.5.2/LICENSE` & `koku-nise-4.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/README.md` & `koku-nise-4.5.3/README.md`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/koku_nise.egg-info/SOURCES.txt` & `koku-nise-4.5.3/koku_nise.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/__main__.py` & `koku-nise-4.5.3/nise/__main__.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/aws-template-manifest.json` & `koku-nise-4.5.3/nise/aws-template-manifest.json`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/copy.py` & `koku-nise-4.5.3/nise/copy.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/extract.py` & `koku-nise-4.5.3/nise/extract.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/generators/aws/__init__.py` & `koku-nise-4.5.3/nise/generators/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/generators/aws/aws_constants.py` & `koku-nise-4.5.3/nise/generators/aws/aws_constants.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/generators/aws/aws_generator.py` & `koku-nise-4.5.3/nise/generators/aws/aws_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/generators/aws/data_transfer_generator.py` & `koku-nise-4.5.3/nise/generators/aws/data_transfer_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/generators/aws/ebs_generator.py` & `koku-nise-4.5.3/nise/generators/aws/ebs_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/generators/aws/ec2_generator.py` & `koku-nise-4.5.3/nise/generators/aws/ec2_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/generators/aws/marketplace_generator.py` & `koku-nise-4.5.3/nise/generators/aws/marketplace_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/generators/aws/rds_generator.py` & `koku-nise-4.5.3/nise/generators/aws/rds_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/generators/aws/route53_generator.py` & `koku-nise-4.5.3/nise/generators/aws/route53_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/generators/aws/s3_generator.py` & `koku-nise-4.5.3/nise/generators/aws/s3_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/generators/aws/vpc_generator.py` & `koku-nise-4.5.3/nise/generators/aws/vpc_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/generators/azure/__init__.py` & `koku-nise-4.5.3/nise/generators/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/generators/azure/azure_generator.py` & `koku-nise-4.5.3/nise/generators/azure/azure_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/generators/azure/bandwidth_generator.py` & `koku-nise-4.5.3/nise/generators/azure/bandwidth_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/generators/azure/ccsp_generator.py` & `koku-nise-4.5.3/nise/generators/azure/ccsp_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/generators/azure/data_transfer_generator.py` & `koku-nise-4.5.3/nise/generators/azure/data_transfer_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/generators/azure/managed_disk_generator.py` & `koku-nise-4.5.3/nise/generators/azure/managed_disk_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/generators/azure/sql_database_generator.py` & `koku-nise-4.5.3/nise/generators/azure/sql_database_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/generators/azure/storage_generator.py` & `koku-nise-4.5.3/nise/generators/azure/storage_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/generators/azure/virtual_machine_generator.py` & `koku-nise-4.5.3/nise/generators/azure/virtual_machine_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/generators/azure/virtual_network_generator.py` & `koku-nise-4.5.3/nise/generators/azure/virtual_network_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/generators/gcp/__init__.py` & `koku-nise-4.5.3/nise/generators/gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/generators/gcp/cloud_storage_generator.py` & `koku-nise-4.5.3/nise/generators/gcp/cloud_storage_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/generators/gcp/compute_engine_generator.py` & `koku-nise-4.5.3/nise/generators/gcp/compute_engine_generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,24 +31,33 @@
         ("CF4E-A0C7-E3BF", "Instance Core running in Americas", "seconds", "hour"),
         ("D973-5D65-BAB2", "Storage PD Capacity", "byte-seconds", "gibibyte month"),
         ("D0CC-50DF-59D2", "Network Inter Zone Ingress", "bytes", "gibibyte"),
         ("F449-33EC-A5EF", "E2 Instance Ram running in Americas", "byte-seconds", "gibibyte hour"),
         ("CD20-B4CA-0F7C", "Licensing Fee for Debian 10 Buster (RAM cost)", "byte-seconds", "gibibyte hour"),
         ("236F-83FC-852C", "Licensing Fee for Red Hat Enterprise Linux 8 (RAM cost)", "byte-seconds", "gibibyte hour"),
         ("8C61-80B1-C43A", "Licensing Fee for Red Hat Enterprise Linux 8 on VM with 1 to 4 VCPU", "seconds", "hour"),
-        ("6B8F-E63D-832B", "Network Internet Egress from Americas to APAC", "bytes", "gibibyte"),
-        ("DFA5-B5C6-36D6", "Network Internet Egress from Americas to EMEA", "bytes", "gibibyte"),
-        ("9DE9-9092-B3BC", "Network Internet Egress from Americas to China", "bytes", "gibibyte"),
-        ("7151-106A-2684", "Network Internet Ingress from APAC to Americas", "bytes", "gibibyte"),
-        ("2F99-3A90-373B", "Network Internet Ingress from EMEA to Americas", "bytes", "gibibyte"),
-        ("92CB-C25F-B1D1", "Network Google Egress from Americas to Americas", "bytes", "gibibyte"),
-        ("227B-5B2B-A75A", "Network Internet Ingress from China to Americas", "bytes", "gibibyte"),
-        ("123C-0EFC-B7C8", "Network Google Ingress from Americas to Americas", "bytes", "gibibyte"),
-        ("F274-1692-F213", "Network Internet Engress from Americas to Americas", "bytes", "gibibyte"),
-        ("92CB-C25F-B1D1", "Network Google Egress from Americas to Americas", "bytes", "gibibyte"),  # Left off at 125
+        ("BBF8-C07D-1DF4", "Network Inter Region Data Transfer In from APAC to Americas", "bytes", "gibibyte"),
+        ("0C3C-6B13-B1E8", "Network Inter Region Data Transfer Out from Americas to Los Angeles", "bytes", "gibibyte"),
+        ("FDBC-6E3B-D4D8", "Network Internet Data Transfer Out from Americas to Australia", "bytes", "gibibyte"),
+        ("B307-417F-4FD2", "Network Internet Data Transfer In from EMEA to Virginia", "bytes", "gibibyte"),
+        ("5A40-9F05-4385", "Network Inter Region Data Transfer In from Hong Kong to Virginia", "bytes", "gibibyte"),
+        ("6B8F-E63D-832B", "Network Internet Data Transfer Out from Americas to APAC", "bytes", "gibibyte"),
+        ("DFA5-B5C6-36D6", "Network Internet Data Transfer Out from Americas to EMEA", "bytes", "gibibyte"),
+        ("9DE9-9092-B3BC", "Network Internet Data Transfer Out from Americas to China", "bytes", "gibibyte"),
+        ("7151-106A-2684", "Network Internet Data Transfer In from APAC to Americas", "bytes", "gibibyte"),
+        ("2F99-3A90-373B", "Network Internet Data Transfer In from EMEA to Americas", "bytes", "gibibyte"),
+        ("92CB-C25F-B1D1", "Network Data Transfer to Google Services from Americas to Americas", "bytes", "gibibyte"),
+        ("227B-5B2B-A75A", "Network Internet Data Transfer In from China to Americas", "bytes", "gibibyte"),
+        (
+            "123C-0EFC-B7C8",
+            "Network Data Transfer In from Google Services from Americas to Americas",
+            "bytes",
+            "gibibyte",
+        ),
+        ("F274-1692-F213", "Network Internet Data Transfer Out from Americas to Americas", "bytes", "gibibyte"),
     )
 
     LABELS = (([{"key": "vm_key_proj2", "value": "vm_label_proj2"}]), ([]))
 
     def __init__(self, start_date, end_date, currency, project, attributes=None):  # noqa: C901
         """Initialize the cloud storage generator."""
         super().__init__(start_date, end_date, currency, project, attributes)
```

### Comparing `koku-nise-4.5.2/nise/generators/gcp/gcp_database_generator.py` & `koku-nise-4.5.3/nise/generators/gcp/gcp_database_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/generators/gcp/gcp_generator.py` & `koku-nise-4.5.3/nise/generators/gcp/gcp_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/generators/gcp/gcp_network_generator.py` & `koku-nise-4.5.3/nise/generators/gcp/gcp_network_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/generators/gcp/hcs_generator.py` & `koku-nise-4.5.3/nise/generators/gcp/hcs_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/generators/gcp/project_generator.py` & `koku-nise-4.5.3/nise/generators/gcp/project_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/generators/generator.py` & `koku-nise-4.5.3/nise/generators/generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/generators/oci/__init__.py` & `koku-nise-4.5.3/nise/generators/oci/__init__.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/generators/oci/oci_block_storage_generator.py` & `koku-nise-4.5.3/nise/generators/oci/oci_block_storage_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/generators/oci/oci_compute_generator.py` & `koku-nise-4.5.3/nise/generators/oci/oci_compute_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/generators/oci/oci_constants.py` & `koku-nise-4.5.3/nise/generators/oci/oci_constants.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/generators/oci/oci_database_generator.py` & `koku-nise-4.5.3/nise/generators/oci/oci_database_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/generators/oci/oci_generator.py` & `koku-nise-4.5.3/nise/generators/oci/oci_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/generators/oci/oci_network_generator.py` & `koku-nise-4.5.3/nise/generators/oci/oci_network_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/generators/ocp/__init__.py` & `koku-nise-4.5.3/nise/generators/ocp/__init__.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/generators/ocp/ocp_generator.py` & `koku-nise-4.5.3/nise/generators/ocp/ocp_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/manifest.py` & `koku-nise-4.5.3/nise/manifest.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/report.py` & `koku-nise-4.5.3/nise/report.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/upload.py` & `koku-nise-4.5.3/nise/upload.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/util/__init__.py` & `koku-nise-4.5.3/nise/util/__init__.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/util/log.py` & `koku-nise-4.5.3/nise/util/log.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/yaml_gen.py` & `koku-nise-4.5.3/nise/yaml_gen.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/yaml_generators/aws/ec2_instance_types.py` & `koku-nise-4.5.3/nise/yaml_generators/aws/ec2_instance_types.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/yaml_generators/aws/generator.py` & `koku-nise-4.5.3/nise/yaml_generators/aws/generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/yaml_generators/aws/rds_instance_types.py` & `koku-nise-4.5.3/nise/yaml_generators/aws/rds_instance_types.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/yaml_generators/aws/regions.py` & `koku-nise-4.5.3/nise/yaml_generators/aws/regions.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/yaml_generators/azure/generator.py` & `koku-nise-4.5.3/nise/yaml_generators/azure/generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/yaml_generators/gcp/generator.py` & `koku-nise-4.5.3/nise/yaml_generators/gcp/generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/yaml_generators/generator.py` & `koku-nise-4.5.3/nise/yaml_generators/generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/yaml_generators/oci/generator.py` & `koku-nise-4.5.3/nise/yaml_generators/oci/generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/yaml_generators/oci/oci_yaml_constants.py` & `koku-nise-4.5.3/nise/yaml_generators/oci/oci_yaml_constants.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/yaml_generators/ocp/generator.py` & `koku-nise-4.5.3/nise/yaml_generators/ocp/generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/yaml_generators/ocp_on_cloud/generator.py` & `koku-nise-4.5.3/nise/yaml_generators/ocp_on_cloud/generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/yaml_generators/static/aws_generator_config.yml` & `koku-nise-4.5.3/nise/yaml_generators/static/aws_generator_config.yml`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/yaml_generators/static/aws_static_data.yml.j2` & `koku-nise-4.5.3/nise/yaml_generators/static/aws_static_data.yml.j2`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/yaml_generators/static/azure_generator_config.yml` & `koku-nise-4.5.3/nise/yaml_generators/static/azure_generator_config.yml`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/yaml_generators/static/azure_static_data.yml.j2` & `koku-nise-4.5.3/nise/yaml_generators/static/azure_static_data.yml.j2`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/yaml_generators/static/gcp_static_data.yml.j2` & `koku-nise-4.5.3/nise/yaml_generators/static/gcp_static_data.yml.j2`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/yaml_generators/static/oci_static_data.yml.j2` & `koku-nise-4.5.3/nise/yaml_generators/static/oci_static_data.yml.j2`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/yaml_generators/static/ocp_generator_config.yml` & `koku-nise-4.5.3/nise/yaml_generators/static/ocp_generator_config.yml`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/yaml_generators/static/ocp_on_cloud_options.yml` & `koku-nise-4.5.3/nise/yaml_generators/static/ocp_on_cloud_options.yml`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/yaml_generators/static/ocp_static_data.yml.j2` & `koku-nise-4.5.3/nise/yaml_generators/static/ocp_static_data.yml.j2`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/nise/yaml_generators/utils.py` & `koku-nise-4.5.3/nise/yaml_generators/utils.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.2/setup.py` & `koku-nise-4.5.3/setup.py`

 * *Files identical despite different names*

