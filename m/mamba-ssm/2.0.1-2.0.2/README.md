# Comparing `tmp/mamba_ssm-2.0.1.tar.gz` & `tmp/mamba_ssm-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mamba_ssm-2.0.1.tar", last modified: Mon Jun  3 12:23:00 2024, max compression
+gzip compressed data, was "mamba_ssm-2.0.2.tar", last modified: Mon Jun  3 14:02:07 2024, max compression
```

## Comparing `mamba_ssm-2.0.1.tar` & `mamba_ssm-2.0.2.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:23:00.689563 mamba_ssm-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-06-03 12:22:32.000000 mamba_ssm-2.0.1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)    11348 2024-06-03 12:22:32.000000 mamba_ssm-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10739 2024-06-03 12:23:00.689563 mamba_ssm-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10289 2024-06-03 12:22:32.000000 mamba_ssm-2.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:23:00.685563 mamba_ssm-2.0.1/mamba_ssm/
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-06-03 12:22:32.000000 mamba_ssm-2.0.1/mamba_ssm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:23:00.685563 mamba_ssm-2.0.1/mamba_ssm/distributed/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:22:32.000000 mamba_ssm-2.0.1/mamba_ssm/distributed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5825 2024-06-03 12:22:32.000000 mamba_ssm-2.0.1/mamba_ssm/distributed/distributed_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12001 2024-06-03 12:22:32.000000 mamba_ssm-2.0.1/mamba_ssm/distributed/tensor_parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:23:00.685563 mamba_ssm-2.0.1/mamba_ssm/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:22:32.000000 mamba_ssm-2.0.1/mamba_ssm/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-06-03 12:22:32.000000 mamba_ssm-2.0.1/mamba_ssm/models/config_mamba.py
--rw-r--r--   0 runner    (1001) docker     (127)    11651 2024-06-03 12:22:32.000000 mamba_ssm-2.0.1/mamba_ssm/models/mixer_seq_simple.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:23:00.685563 mamba_ssm-2.0.1/mamba_ssm/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:22:32.000000 mamba_ssm-2.0.1/mamba_ssm/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-06-03 12:22:32.000000 mamba_ssm-2.0.1/mamba_ssm/modules/block.py
--rw-r--r--   0 runner    (1001) docker     (127)    16051 2024-06-03 12:22:32.000000 mamba_ssm-2.0.1/mamba_ssm/modules/mamba2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7567 2024-06-03 12:22:32.000000 mamba_ssm-2.0.1/mamba_ssm/modules/mamba2_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)    11710 2024-06-03 12:22:32.000000 mamba_ssm-2.0.1/mamba_ssm/modules/mamba_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)    12969 2024-06-03 12:22:32.000000 mamba_ssm-2.0.1/mamba_ssm/modules/mha.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-06-03 12:22:32.000000 mamba_ssm-2.0.1/mamba_ssm/modules/mlp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:23:00.689563 mamba_ssm-2.0.1/mamba_ssm/ops/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:22:32.000000 mamba_ssm-2.0.1/mamba_ssm/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16835 2024-06-03 12:22:32.000000 mamba_ssm-2.0.1/mamba_ssm/ops/selective_scan_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:23:00.689563 mamba_ssm-2.0.1/mamba_ssm/ops/triton/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:22:32.000000 mamba_ssm-2.0.1/mamba_ssm/ops/triton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35020 2024-06-03 12:22:32.000000 mamba_ssm-2.0.1/mamba_ssm/ops/triton/layer_norm.py
--rw-r--r--   0 runner    (1001) docker     (127)    17763 2024-06-03 12:22:32.000000 mamba_ssm-2.0.1/mamba_ssm/ops/triton/layernorm_gated.py
--rw-r--r--   0 runner    (1001) docker     (127)    10720 2024-06-03 12:22:32.000000 mamba_ssm-2.0.1/mamba_ssm/ops/triton/selective_state_update.py
--rw-r--r--   0 runner    (1001) docker     (127)    13637 2024-06-03 12:22:32.000000 mamba_ssm-2.0.1/mamba_ssm/ops/triton/ssd_bmm.py
--rw-r--r--   0 runner    (1001) docker     (127)   104946 2024-06-03 12:22:32.000000 mamba_ssm-2.0.1/mamba_ssm/ops/triton/ssd_chunk_scan.py
--rw-r--r--   0 runner    (1001) docker     (127)    49075 2024-06-03 12:22:32.000000 mamba_ssm-2.0.1/mamba_ssm/ops/triton/ssd_chunk_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    51825 2024-06-03 12:22:32.000000 mamba_ssm-2.0.1/mamba_ssm/ops/triton/ssd_combined.py
--rw-r--r--   0 runner    (1001) docker     (127)    16377 2024-06-03 12:22:32.000000 mamba_ssm-2.0.1/mamba_ssm/ops/triton/ssd_state_passing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:23:00.689563 mamba_ssm-2.0.1/mamba_ssm/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:22:32.000000 mamba_ssm-2.0.1/mamba_ssm/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15363 2024-06-03 12:22:32.000000 mamba_ssm-2.0.1/mamba_ssm/utils/generation.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-06-03 12:22:32.000000 mamba_ssm-2.0.1/mamba_ssm/utils/hf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:23:00.685563 mamba_ssm-2.0.1/mamba_ssm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10739 2024-06-03 12:23:00.000000 mamba_ssm-2.0.1/mamba_ssm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-06-03 12:23:00.000000 mamba_ssm-2.0.1/mamba_ssm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 12:23:00.000000 mamba_ssm-2.0.1/mamba_ssm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-06-03 12:23:00.000000 mamba_ssm-2.0.1/mamba_ssm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-03 12:23:00.000000 mamba_ssm-2.0.1/mamba_ssm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 12:23:00.689563 mamba_ssm-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    10784 2024-06-03 12:22:32.000000 mamba_ssm-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:02:07.920966 mamba_ssm-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-06-03 14:01:35.000000 mamba_ssm-2.0.2/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)    11348 2024-06-03 14:01:35.000000 mamba_ssm-2.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10739 2024-06-03 14:02:07.920966 mamba_ssm-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10289 2024-06-03 14:01:35.000000 mamba_ssm-2.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:02:07.916966 mamba_ssm-2.0.2/mamba_ssm/
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-06-03 14:01:35.000000 mamba_ssm-2.0.2/mamba_ssm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:02:07.916966 mamba_ssm-2.0.2/mamba_ssm/distributed/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:01:35.000000 mamba_ssm-2.0.2/mamba_ssm/distributed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5825 2024-06-03 14:01:35.000000 mamba_ssm-2.0.2/mamba_ssm/distributed/distributed_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12001 2024-06-03 14:01:35.000000 mamba_ssm-2.0.2/mamba_ssm/distributed/tensor_parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:02:07.916966 mamba_ssm-2.0.2/mamba_ssm/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:01:35.000000 mamba_ssm-2.0.2/mamba_ssm/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-06-03 14:01:35.000000 mamba_ssm-2.0.2/mamba_ssm/models/config_mamba.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11651 2024-06-03 14:01:35.000000 mamba_ssm-2.0.2/mamba_ssm/models/mixer_seq_simple.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:02:07.920966 mamba_ssm-2.0.2/mamba_ssm/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:01:35.000000 mamba_ssm-2.0.2/mamba_ssm/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-06-03 14:01:35.000000 mamba_ssm-2.0.2/mamba_ssm/modules/block.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16051 2024-06-03 14:01:35.000000 mamba_ssm-2.0.2/mamba_ssm/modules/mamba2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7567 2024-06-03 14:01:35.000000 mamba_ssm-2.0.2/mamba_ssm/modules/mamba2_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11710 2024-06-03 14:01:35.000000 mamba_ssm-2.0.2/mamba_ssm/modules/mamba_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12969 2024-06-03 14:01:35.000000 mamba_ssm-2.0.2/mamba_ssm/modules/mha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-06-03 14:01:35.000000 mamba_ssm-2.0.2/mamba_ssm/modules/mlp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:02:07.920966 mamba_ssm-2.0.2/mamba_ssm/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:01:35.000000 mamba_ssm-2.0.2/mamba_ssm/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16835 2024-06-03 14:01:35.000000 mamba_ssm-2.0.2/mamba_ssm/ops/selective_scan_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:02:07.920966 mamba_ssm-2.0.2/mamba_ssm/ops/triton/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:01:35.000000 mamba_ssm-2.0.2/mamba_ssm/ops/triton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4877 2024-06-03 14:01:35.000000 mamba_ssm-2.0.2/mamba_ssm/ops/triton/k_activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35020 2024-06-03 14:01:35.000000 mamba_ssm-2.0.2/mamba_ssm/ops/triton/layer_norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17763 2024-06-03 14:01:35.000000 mamba_ssm-2.0.2/mamba_ssm/ops/triton/layernorm_gated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10720 2024-06-03 14:01:35.000000 mamba_ssm-2.0.2/mamba_ssm/ops/triton/selective_state_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13637 2024-06-03 14:01:35.000000 mamba_ssm-2.0.2/mamba_ssm/ops/triton/ssd_bmm.py
+-rw-r--r--   0 runner    (1001) docker     (127)   104946 2024-06-03 14:01:35.000000 mamba_ssm-2.0.2/mamba_ssm/ops/triton/ssd_chunk_scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49075 2024-06-03 14:01:35.000000 mamba_ssm-2.0.2/mamba_ssm/ops/triton/ssd_chunk_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51825 2024-06-03 14:01:35.000000 mamba_ssm-2.0.2/mamba_ssm/ops/triton/ssd_combined.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16377 2024-06-03 14:01:35.000000 mamba_ssm-2.0.2/mamba_ssm/ops/triton/ssd_state_passing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:02:07.920966 mamba_ssm-2.0.2/mamba_ssm/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:01:35.000000 mamba_ssm-2.0.2/mamba_ssm/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15363 2024-06-03 14:01:35.000000 mamba_ssm-2.0.2/mamba_ssm/utils/generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-06-03 14:01:35.000000 mamba_ssm-2.0.2/mamba_ssm/utils/hf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:02:07.916966 mamba_ssm-2.0.2/mamba_ssm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10739 2024-06-03 14:02:07.000000 mamba_ssm-2.0.2/mamba_ssm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-06-03 14:02:07.000000 mamba_ssm-2.0.2/mamba_ssm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 14:02:07.000000 mamba_ssm-2.0.2/mamba_ssm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-06-03 14:02:07.000000 mamba_ssm-2.0.2/mamba_ssm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-03 14:02:07.000000 mamba_ssm-2.0.2/mamba_ssm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 14:02:07.920966 mamba_ssm-2.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    10784 2024-06-03 14:01:35.000000 mamba_ssm-2.0.2/setup.py
```

### Comparing `mamba_ssm-2.0.1/LICENSE` & `mamba_ssm-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mamba_ssm-2.0.1/PKG-INFO` & `mamba_ssm-2.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mamba_ssm
-Version: 2.0.1
+Version: 2.0.2
 Summary: Mamba state-space model
 Home-page: https://github.com/state-spaces/mamba
 Author: Tri Dao, Albert Gu
 Author-email: tri@tridao.me, agu@cs.cmu.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: Unix
```

### Comparing `mamba_ssm-2.0.1/README.md` & `mamba_ssm-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `mamba_ssm-2.0.1/mamba_ssm/distributed/distributed_utils.py` & `mamba_ssm-2.0.2/mamba_ssm/distributed/distributed_utils.py`

 * *Files identical despite different names*

### Comparing `mamba_ssm-2.0.1/mamba_ssm/distributed/tensor_parallel.py` & `mamba_ssm-2.0.2/mamba_ssm/distributed/tensor_parallel.py`

 * *Files identical despite different names*

### Comparing `mamba_ssm-2.0.1/mamba_ssm/models/mixer_seq_simple.py` & `mamba_ssm-2.0.2/mamba_ssm/models/mixer_seq_simple.py`

 * *Files identical despite different names*

### Comparing `mamba_ssm-2.0.1/mamba_ssm/modules/block.py` & `mamba_ssm-2.0.2/mamba_ssm/modules/block.py`

 * *Files identical despite different names*

### Comparing `mamba_ssm-2.0.1/mamba_ssm/modules/mamba2.py` & `mamba_ssm-2.0.2/mamba_ssm/modules/mamba2.py`

 * *Files identical despite different names*

### Comparing `mamba_ssm-2.0.1/mamba_ssm/modules/mamba2_simple.py` & `mamba_ssm-2.0.2/mamba_ssm/modules/mamba2_simple.py`

 * *Files identical despite different names*

### Comparing `mamba_ssm-2.0.1/mamba_ssm/modules/mamba_simple.py` & `mamba_ssm-2.0.2/mamba_ssm/modules/mamba_simple.py`

 * *Files identical despite different names*

### Comparing `mamba_ssm-2.0.1/mamba_ssm/modules/mha.py` & `mamba_ssm-2.0.2/mamba_ssm/modules/mha.py`

 * *Files identical despite different names*

### Comparing `mamba_ssm-2.0.1/mamba_ssm/modules/mlp.py` & `mamba_ssm-2.0.2/mamba_ssm/modules/mlp.py`

 * *Files identical despite different names*

### Comparing `mamba_ssm-2.0.1/mamba_ssm/ops/selective_scan_interface.py` & `mamba_ssm-2.0.2/mamba_ssm/ops/selective_scan_interface.py`

 * *Files identical despite different names*

### Comparing `mamba_ssm-2.0.1/mamba_ssm/ops/triton/layer_norm.py` & `mamba_ssm-2.0.2/mamba_ssm/ops/triton/layer_norm.py`

 * *Files identical despite different names*

### Comparing `mamba_ssm-2.0.1/mamba_ssm/ops/triton/layernorm_gated.py` & `mamba_ssm-2.0.2/mamba_ssm/ops/triton/layernorm_gated.py`

 * *Files identical despite different names*

### Comparing `mamba_ssm-2.0.1/mamba_ssm/ops/triton/selective_state_update.py` & `mamba_ssm-2.0.2/mamba_ssm/ops/triton/selective_state_update.py`

 * *Files identical despite different names*

### Comparing `mamba_ssm-2.0.1/mamba_ssm/ops/triton/ssd_bmm.py` & `mamba_ssm-2.0.2/mamba_ssm/ops/triton/ssd_bmm.py`

 * *Files identical despite different names*

### Comparing `mamba_ssm-2.0.1/mamba_ssm/ops/triton/ssd_chunk_scan.py` & `mamba_ssm-2.0.2/mamba_ssm/ops/triton/ssd_chunk_scan.py`

 * *Files identical despite different names*

### Comparing `mamba_ssm-2.0.1/mamba_ssm/ops/triton/ssd_chunk_state.py` & `mamba_ssm-2.0.2/mamba_ssm/ops/triton/ssd_chunk_state.py`

 * *Files identical despite different names*

### Comparing `mamba_ssm-2.0.1/mamba_ssm/ops/triton/ssd_combined.py` & `mamba_ssm-2.0.2/mamba_ssm/ops/triton/ssd_combined.py`

 * *Files identical despite different names*

### Comparing `mamba_ssm-2.0.1/mamba_ssm/ops/triton/ssd_state_passing.py` & `mamba_ssm-2.0.2/mamba_ssm/ops/triton/ssd_state_passing.py`

 * *Files identical despite different names*

### Comparing `mamba_ssm-2.0.1/mamba_ssm/utils/generation.py` & `mamba_ssm-2.0.2/mamba_ssm/utils/generation.py`

 * *Files identical despite different names*

### Comparing `mamba_ssm-2.0.1/mamba_ssm/utils/hf.py` & `mamba_ssm-2.0.2/mamba_ssm/utils/hf.py`

 * *Files identical despite different names*

### Comparing `mamba_ssm-2.0.1/mamba_ssm.egg-info/PKG-INFO` & `mamba_ssm-2.0.2/mamba_ssm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mamba-ssm
-Version: 2.0.1
+Version: 2.0.2
 Summary: Mamba state-space model
 Home-page: https://github.com/state-spaces/mamba
 Author: Tri Dao, Albert Gu
 Author-email: tri@tridao.me, agu@cs.cmu.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: Unix
```

### Comparing `mamba_ssm-2.0.1/mamba_ssm.egg-info/SOURCES.txt` & `mamba_ssm-2.0.2/mamba_ssm.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 mamba_ssm/modules/mamba2_simple.py
 mamba_ssm/modules/mamba_simple.py
 mamba_ssm/modules/mha.py
 mamba_ssm/modules/mlp.py
 mamba_ssm/ops/__init__.py
 mamba_ssm/ops/selective_scan_interface.py
 mamba_ssm/ops/triton/__init__.py
+mamba_ssm/ops/triton/k_activation.py
 mamba_ssm/ops/triton/layer_norm.py
 mamba_ssm/ops/triton/layernorm_gated.py
 mamba_ssm/ops/triton/selective_state_update.py
 mamba_ssm/ops/triton/ssd_bmm.py
 mamba_ssm/ops/triton/ssd_chunk_scan.py
 mamba_ssm/ops/triton/ssd_chunk_state.py
 mamba_ssm/ops/triton/ssd_combined.py
```

### Comparing `mamba_ssm-2.0.1/setup.py` & `mamba_ssm-2.0.2/setup.py`

 * *Files identical despite different names*

