# Comparing `tmp/mamba_ssm-2.0.0.tar.gz` & `tmp/mamba_ssm-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mamba_ssm-2.0.0.tar", last modified: Mon Jun  3 07:46:07 2024, max compression
+gzip compressed data, was "mamba_ssm-2.0.1.tar", last modified: Mon Jun  3 12:23:00 2024, max compression
```

## Comparing `mamba_ssm-2.0.0.tar` & `mamba_ssm-2.0.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:46:07.289350 mamba_ssm-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-06-03 07:45:38.000000 mamba_ssm-2.0.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)    11348 2024-06-03 07:45:38.000000 mamba_ssm-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10738 2024-06-03 07:46:07.289350 mamba_ssm-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10288 2024-06-03 07:45:38.000000 mamba_ssm-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:46:07.285350 mamba_ssm-2.0.0/mamba_ssm/
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-06-03 07:45:38.000000 mamba_ssm-2.0.0/mamba_ssm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:46:07.285350 mamba_ssm-2.0.0/mamba_ssm/distributed/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 07:45:38.000000 mamba_ssm-2.0.0/mamba_ssm/distributed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5825 2024-06-03 07:45:38.000000 mamba_ssm-2.0.0/mamba_ssm/distributed/distributed_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11995 2024-06-03 07:45:38.000000 mamba_ssm-2.0.0/mamba_ssm/distributed/tensor_parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:46:07.285350 mamba_ssm-2.0.0/mamba_ssm/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 07:45:38.000000 mamba_ssm-2.0.0/mamba_ssm/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-06-03 07:45:38.000000 mamba_ssm-2.0.0/mamba_ssm/models/config_mamba.py
--rw-r--r--   0 runner    (1001) docker     (127)    11651 2024-06-03 07:45:38.000000 mamba_ssm-2.0.0/mamba_ssm/models/mixer_seq_simple.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:46:07.285350 mamba_ssm-2.0.0/mamba_ssm/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 07:45:38.000000 mamba_ssm-2.0.0/mamba_ssm/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-06-03 07:45:38.000000 mamba_ssm-2.0.0/mamba_ssm/modules/block.py
--rw-r--r--   0 runner    (1001) docker     (127)    16051 2024-06-03 07:45:38.000000 mamba_ssm-2.0.0/mamba_ssm/modules/mamba2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7567 2024-06-03 07:45:38.000000 mamba_ssm-2.0.0/mamba_ssm/modules/mamba2_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)    11710 2024-06-03 07:45:38.000000 mamba_ssm-2.0.0/mamba_ssm/modules/mamba_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)    12969 2024-06-03 07:45:38.000000 mamba_ssm-2.0.0/mamba_ssm/modules/mha.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-06-03 07:45:38.000000 mamba_ssm-2.0.0/mamba_ssm/modules/mlp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:46:07.289350 mamba_ssm-2.0.0/mamba_ssm/ops/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 07:45:38.000000 mamba_ssm-2.0.0/mamba_ssm/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16835 2024-06-03 07:45:38.000000 mamba_ssm-2.0.0/mamba_ssm/ops/selective_scan_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:46:07.289350 mamba_ssm-2.0.0/mamba_ssm/ops/triton/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 07:45:38.000000 mamba_ssm-2.0.0/mamba_ssm/ops/triton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35020 2024-06-03 07:45:38.000000 mamba_ssm-2.0.0/mamba_ssm/ops/triton/layer_norm.py
--rw-r--r--   0 runner    (1001) docker     (127)    17763 2024-06-03 07:45:38.000000 mamba_ssm-2.0.0/mamba_ssm/ops/triton/layernorm_gated.py
--rw-r--r--   0 runner    (1001) docker     (127)    10720 2024-06-03 07:45:38.000000 mamba_ssm-2.0.0/mamba_ssm/ops/triton/selective_state_update.py
--rw-r--r--   0 runner    (1001) docker     (127)    13637 2024-06-03 07:45:38.000000 mamba_ssm-2.0.0/mamba_ssm/ops/triton/ssd_bmm.py
--rw-r--r--   0 runner    (1001) docker     (127)   104940 2024-06-03 07:45:38.000000 mamba_ssm-2.0.0/mamba_ssm/ops/triton/ssd_chunk_scan.py
--rw-r--r--   0 runner    (1001) docker     (127)    49075 2024-06-03 07:45:38.000000 mamba_ssm-2.0.0/mamba_ssm/ops/triton/ssd_chunk_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    51735 2024-06-03 07:45:38.000000 mamba_ssm-2.0.0/mamba_ssm/ops/triton/ssd_combined.py
--rw-r--r--   0 runner    (1001) docker     (127)    16377 2024-06-03 07:45:38.000000 mamba_ssm-2.0.0/mamba_ssm/ops/triton/ssd_state_passing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:46:07.289350 mamba_ssm-2.0.0/mamba_ssm/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 07:45:38.000000 mamba_ssm-2.0.0/mamba_ssm/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15363 2024-06-03 07:45:38.000000 mamba_ssm-2.0.0/mamba_ssm/utils/generation.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-06-03 07:45:38.000000 mamba_ssm-2.0.0/mamba_ssm/utils/hf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:46:07.285350 mamba_ssm-2.0.0/mamba_ssm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10738 2024-06-03 07:46:07.000000 mamba_ssm-2.0.0/mamba_ssm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-06-03 07:46:07.000000 mamba_ssm-2.0.0/mamba_ssm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 07:46:07.000000 mamba_ssm-2.0.0/mamba_ssm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-06-03 07:46:07.000000 mamba_ssm-2.0.0/mamba_ssm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-03 07:46:07.000000 mamba_ssm-2.0.0/mamba_ssm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 07:46:07.289350 mamba_ssm-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    10784 2024-06-03 07:45:38.000000 mamba_ssm-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:23:00.689563 mamba_ssm-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-06-03 12:22:32.000000 mamba_ssm-2.0.1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)    11348 2024-06-03 12:22:32.000000 mamba_ssm-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10739 2024-06-03 12:23:00.689563 mamba_ssm-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10289 2024-06-03 12:22:32.000000 mamba_ssm-2.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:23:00.685563 mamba_ssm-2.0.1/mamba_ssm/
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-06-03 12:22:32.000000 mamba_ssm-2.0.1/mamba_ssm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:23:00.685563 mamba_ssm-2.0.1/mamba_ssm/distributed/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:22:32.000000 mamba_ssm-2.0.1/mamba_ssm/distributed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5825 2024-06-03 12:22:32.000000 mamba_ssm-2.0.1/mamba_ssm/distributed/distributed_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12001 2024-06-03 12:22:32.000000 mamba_ssm-2.0.1/mamba_ssm/distributed/tensor_parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:23:00.685563 mamba_ssm-2.0.1/mamba_ssm/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:22:32.000000 mamba_ssm-2.0.1/mamba_ssm/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-06-03 12:22:32.000000 mamba_ssm-2.0.1/mamba_ssm/models/config_mamba.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11651 2024-06-03 12:22:32.000000 mamba_ssm-2.0.1/mamba_ssm/models/mixer_seq_simple.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:23:00.685563 mamba_ssm-2.0.1/mamba_ssm/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:22:32.000000 mamba_ssm-2.0.1/mamba_ssm/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-06-03 12:22:32.000000 mamba_ssm-2.0.1/mamba_ssm/modules/block.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16051 2024-06-03 12:22:32.000000 mamba_ssm-2.0.1/mamba_ssm/modules/mamba2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7567 2024-06-03 12:22:32.000000 mamba_ssm-2.0.1/mamba_ssm/modules/mamba2_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11710 2024-06-03 12:22:32.000000 mamba_ssm-2.0.1/mamba_ssm/modules/mamba_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12969 2024-06-03 12:22:32.000000 mamba_ssm-2.0.1/mamba_ssm/modules/mha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-06-03 12:22:32.000000 mamba_ssm-2.0.1/mamba_ssm/modules/mlp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:23:00.689563 mamba_ssm-2.0.1/mamba_ssm/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:22:32.000000 mamba_ssm-2.0.1/mamba_ssm/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16835 2024-06-03 12:22:32.000000 mamba_ssm-2.0.1/mamba_ssm/ops/selective_scan_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:23:00.689563 mamba_ssm-2.0.1/mamba_ssm/ops/triton/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:22:32.000000 mamba_ssm-2.0.1/mamba_ssm/ops/triton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35020 2024-06-03 12:22:32.000000 mamba_ssm-2.0.1/mamba_ssm/ops/triton/layer_norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17763 2024-06-03 12:22:32.000000 mamba_ssm-2.0.1/mamba_ssm/ops/triton/layernorm_gated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10720 2024-06-03 12:22:32.000000 mamba_ssm-2.0.1/mamba_ssm/ops/triton/selective_state_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13637 2024-06-03 12:22:32.000000 mamba_ssm-2.0.1/mamba_ssm/ops/triton/ssd_bmm.py
+-rw-r--r--   0 runner    (1001) docker     (127)   104946 2024-06-03 12:22:32.000000 mamba_ssm-2.0.1/mamba_ssm/ops/triton/ssd_chunk_scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49075 2024-06-03 12:22:32.000000 mamba_ssm-2.0.1/mamba_ssm/ops/triton/ssd_chunk_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51825 2024-06-03 12:22:32.000000 mamba_ssm-2.0.1/mamba_ssm/ops/triton/ssd_combined.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16377 2024-06-03 12:22:32.000000 mamba_ssm-2.0.1/mamba_ssm/ops/triton/ssd_state_passing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:23:00.689563 mamba_ssm-2.0.1/mamba_ssm/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:22:32.000000 mamba_ssm-2.0.1/mamba_ssm/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15363 2024-06-03 12:22:32.000000 mamba_ssm-2.0.1/mamba_ssm/utils/generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-06-03 12:22:32.000000 mamba_ssm-2.0.1/mamba_ssm/utils/hf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:23:00.685563 mamba_ssm-2.0.1/mamba_ssm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10739 2024-06-03 12:23:00.000000 mamba_ssm-2.0.1/mamba_ssm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-06-03 12:23:00.000000 mamba_ssm-2.0.1/mamba_ssm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 12:23:00.000000 mamba_ssm-2.0.1/mamba_ssm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-06-03 12:23:00.000000 mamba_ssm-2.0.1/mamba_ssm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-03 12:23:00.000000 mamba_ssm-2.0.1/mamba_ssm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 12:23:00.689563 mamba_ssm-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    10784 2024-06-03 12:22:32.000000 mamba_ssm-2.0.1/setup.py
```

### Comparing `mamba_ssm-2.0.0/LICENSE` & `mamba_ssm-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mamba_ssm-2.0.0/PKG-INFO` & `mamba_ssm-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mamba_ssm
-Version: 2.0.0
+Version: 2.0.1
 Summary: Mamba state-space model
 Home-page: https://github.com/state-spaces/mamba
 Author: Tri Dao, Albert Gu
 Author-email: tri@tridao.me, agu@cs.cmu.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: Unix
@@ -14,16 +14,16 @@
 License-File: AUTHORS
 
 # Mamba
 
 ![Mamba](assets/selection.png "Selective State Space")
 > **Mamba: Linear-Time Sequence Modeling with Selective State Spaces**\
 > Albert Gu*, Tri Dao*\
-> Paper: https://arxiv.org/abs/2312.00752
-> **Transformers are {SSM}s: Generalized Models and Efficient Algorithms Through Structured State Space Duality**\
+> Paper: https://arxiv.org/abs/2312.00752\ 
+> **Transformers are SSMs: Generalized Models and Efficient Algorithms Through Structured State Space Duality**\ 
 > Tri Dao*, Albert Gu*\
 > Paper: https://arxiv.org/abs/2405.21060
 
 ## About
 
 Mamba is a new state space model architecture showing promising performance on information-dense data such as language modeling, where previous subquadratic models fall short of Transformers.
 It is based on the line of progress on [structured state space models](https://github.com/state-spaces/s4),
```

### Comparing `mamba_ssm-2.0.0/README.md` & `mamba_ssm-2.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Mamba
 
 ![Mamba](assets/selection.png "Selective State Space")
 > **Mamba: Linear-Time Sequence Modeling with Selective State Spaces**\
 > Albert Gu*, Tri Dao*\
-> Paper: https://arxiv.org/abs/2312.00752
-> **Transformers are {SSM}s: Generalized Models and Efficient Algorithms Through Structured State Space Duality**\
+> Paper: https://arxiv.org/abs/2312.00752\ 
+> **Transformers are SSMs: Generalized Models and Efficient Algorithms Through Structured State Space Duality**\ 
 > Tri Dao*, Albert Gu*\
 > Paper: https://arxiv.org/abs/2405.21060
 
 ## About
 
 Mamba is a new state space model architecture showing promising performance on information-dense data such as language modeling, where previous subquadratic models fall short of Transformers.
 It is based on the line of progress on [structured state space models](https://github.com/state-spaces/s4),
```

### Comparing `mamba_ssm-2.0.0/mamba_ssm/distributed/distributed_utils.py` & `mamba_ssm-2.0.1/mamba_ssm/distributed/distributed_utils.py`

 * *Files identical despite different names*

### Comparing `mamba_ssm-2.0.0/mamba_ssm/distributed/tensor_parallel.py` & `mamba_ssm-2.0.1/mamba_ssm/distributed/tensor_parallel.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import torch.nn.functional as F
 from torch import Tensor
 from torch.cuda.amp import custom_bwd, custom_fwd
 from torch.distributed import ProcessGroup
 
 from einops import rearrange
 
-from src.distributed.distributed_utils import (
+from mamba_ssm.distributed.distributed_utils import (
     all_gather_raw,
     all_reduce,
     all_reduce_raw,
     reduce_scatter,
     reduce_scatter_raw,
 )
```

### Comparing `mamba_ssm-2.0.0/mamba_ssm/models/mixer_seq_simple.py` & `mamba_ssm-2.0.1/mamba_ssm/models/mixer_seq_simple.py`

 * *Files identical despite different names*

### Comparing `mamba_ssm-2.0.0/mamba_ssm/modules/block.py` & `mamba_ssm-2.0.1/mamba_ssm/modules/block.py`

 * *Files identical despite different names*

### Comparing `mamba_ssm-2.0.0/mamba_ssm/modules/mamba2.py` & `mamba_ssm-2.0.1/mamba_ssm/modules/mamba2.py`

 * *Files identical despite different names*

### Comparing `mamba_ssm-2.0.0/mamba_ssm/modules/mamba2_simple.py` & `mamba_ssm-2.0.1/mamba_ssm/modules/mamba2_simple.py`

 * *Files identical despite different names*

### Comparing `mamba_ssm-2.0.0/mamba_ssm/modules/mamba_simple.py` & `mamba_ssm-2.0.1/mamba_ssm/modules/mamba_simple.py`

 * *Files identical despite different names*

### Comparing `mamba_ssm-2.0.0/mamba_ssm/modules/mha.py` & `mamba_ssm-2.0.1/mamba_ssm/modules/mha.py`

 * *Files identical despite different names*

### Comparing `mamba_ssm-2.0.0/mamba_ssm/modules/mlp.py` & `mamba_ssm-2.0.1/mamba_ssm/modules/mlp.py`

 * *Files identical despite different names*

### Comparing `mamba_ssm-2.0.0/mamba_ssm/ops/selective_scan_interface.py` & `mamba_ssm-2.0.1/mamba_ssm/ops/selective_scan_interface.py`

 * *Files identical despite different names*

### Comparing `mamba_ssm-2.0.0/mamba_ssm/ops/triton/layer_norm.py` & `mamba_ssm-2.0.1/mamba_ssm/ops/triton/layer_norm.py`

 * *Files identical despite different names*

### Comparing `mamba_ssm-2.0.0/mamba_ssm/ops/triton/layernorm_gated.py` & `mamba_ssm-2.0.1/mamba_ssm/ops/triton/layernorm_gated.py`

 * *Files identical despite different names*

### Comparing `mamba_ssm-2.0.0/mamba_ssm/ops/triton/selective_state_update.py` & `mamba_ssm-2.0.1/mamba_ssm/ops/triton/selective_state_update.py`

 * *Files identical despite different names*

### Comparing `mamba_ssm-2.0.0/mamba_ssm/ops/triton/ssd_bmm.py` & `mamba_ssm-2.0.1/mamba_ssm/ops/triton/ssd_bmm.py`

 * *Files identical despite different names*

### Comparing `mamba_ssm-2.0.0/mamba_ssm/ops/triton/ssd_chunk_scan.py` & `mamba_ssm-2.0.1/mamba_ssm/ops/triton/ssd_chunk_scan.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import torch.nn.functional as F
 
 import triton
 import triton.language as tl
 
 from einops import rearrange, repeat
 
-from src.ops.triton.ssd_bmm import _bmm_chunk_fwd, _bmm_chunk_bwd
+from mamba_ssm.ops.triton.ssd_bmm import _bmm_chunk_fwd, _bmm_chunk_bwd
 
 TRITON_22 = version.parse(triton.__version__) >= version.parse('2.2.0')
 
 
 def init_to_zero(names):
     return lambda nargs: [nargs[name].zero_() for name in names if nargs[name] is not None]
```

### Comparing `mamba_ssm-2.0.0/mamba_ssm/ops/triton/ssd_chunk_state.py` & `mamba_ssm-2.0.1/mamba_ssm/ops/triton/ssd_chunk_state.py`

 * *Files identical despite different names*

### Comparing `mamba_ssm-2.0.0/mamba_ssm/ops/triton/ssd_combined.py` & `mamba_ssm-2.0.1/mamba_ssm/ops/triton/ssd_combined.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,28 +20,28 @@
 
 try:
     from causal_conv1d import causal_conv1d_fn
     import causal_conv1d_cuda
 except ImportError:
     causal_conv1d_fn, causal_conv1d_cuda = None, None
 
-from src.ops.triton.ssd_bmm import _bmm_chunk_fwd, _bmm_chunk_bwd
-from src.ops.triton.ssd_chunk_state import _chunk_cumsum_fwd, _chunk_cumsum_bwd
-from src.ops.triton.ssd_chunk_state import _chunk_state_fwd, _chunk_state_bwd_db
-from src.ops.triton.ssd_chunk_state import _chunk_state_bwd_ddAcs_stable
-from src.ops.triton.ssd_chunk_state import chunk_state, chunk_state_ref
-from src.ops.triton.ssd_state_passing import _state_passing_fwd, _state_passing_bwd
-from src.ops.triton.ssd_state_passing import state_passing, state_passing_ref
-from src.ops.triton.ssd_chunk_scan import _chunk_scan_fwd, _chunk_scan_bwd_dz, _chunk_scan_bwd_dstates
-from src.ops.triton.ssd_chunk_scan import _chunk_scan_bwd_dC, _chunk_scan_bwd_dcb
-from src.ops.triton.ssd_chunk_scan import _chunk_scan_bwd_ddAcs_stable
-from src.ops.triton.ssd_chunk_scan import chunk_scan, chunk_scan_ref
-from src.ops.triton.ssd_chunk_scan import _chunk_scan_bwd_ddAcs_prev
-from src.ops.triton.layernorm_gated import rmsnorm_fn, _layer_norm_fwd, _layer_norm_bwd
-from src.ops.triton.k_activations import _swiglu_fwd, _swiglu_bwd
+from mamba_ssm.ops.triton.ssd_bmm import _bmm_chunk_fwd, _bmm_chunk_bwd
+from mamba_ssm.ops.triton.ssd_chunk_state import _chunk_cumsum_fwd, _chunk_cumsum_bwd
+from mamba_ssm.ops.triton.ssd_chunk_state import _chunk_state_fwd, _chunk_state_bwd_db
+from mamba_ssm.ops.triton.ssd_chunk_state import _chunk_state_bwd_ddAcs_stable
+from mamba_ssm.ops.triton.ssd_chunk_state import chunk_state, chunk_state_ref
+from mamba_ssm.ops.triton.ssd_state_passing import _state_passing_fwd, _state_passing_bwd
+from mamba_ssm.ops.triton.ssd_state_passing import state_passing, state_passing_ref
+from mamba_ssm.ops.triton.ssd_chunk_scan import _chunk_scan_fwd, _chunk_scan_bwd_dz, _chunk_scan_bwd_dstates
+from mamba_ssm.ops.triton.ssd_chunk_scan import _chunk_scan_bwd_dC, _chunk_scan_bwd_dcb
+from mamba_ssm.ops.triton.ssd_chunk_scan import _chunk_scan_bwd_ddAcs_stable
+from mamba_ssm.ops.triton.ssd_chunk_scan import chunk_scan, chunk_scan_ref
+from mamba_ssm.ops.triton.ssd_chunk_scan import _chunk_scan_bwd_ddAcs_prev
+from mamba_ssm.ops.triton.layernorm_gated import rmsnorm_fn, _layer_norm_fwd, _layer_norm_bwd
+from mamba_ssm.ops.triton.k_activations import _swiglu_fwd, _swiglu_bwd
 
 TRITON_22 = version.parse(triton.__version__) >= version.parse('2.2.0')
 
 
 def init_to_zero(names):
     return lambda nargs: [nargs[name].zero_() for name in names if nargs[name] is not None]
 
@@ -647,15 +647,15 @@
         C: (batch, seqlen, ngroups, dstate)
         D: (nheads, headdim) or (nheads,)
         z: (batch, seqlen, nheads, headdim)
         dt_bias: (nheads,) or (nheads, headdim)
     Return:
         out: (batch, seqlen, nheads, headdim)
     """
-    from src.ops.selective_scan_interface import selective_scan_fn
+    from mamba_ssm.ops.selective_scan_interface import selective_scan_fn
 
     batch, seqlen, nheads, headdim = x.shape
     _, _, ngroups, dstate = B.shape
     x = rearrange(x, "b l h p -> b (h p) l")
     if dt.dim() == 3:
         dt = repeat(dt, "b l h -> b l h p", p=headdim)
     dt = rearrange(dt, "b l h p -> b (h p) l")
```

### Comparing `mamba_ssm-2.0.0/mamba_ssm/ops/triton/ssd_state_passing.py` & `mamba_ssm-2.0.1/mamba_ssm/ops/triton/ssd_state_passing.py`

 * *Files identical despite different names*

### Comparing `mamba_ssm-2.0.0/mamba_ssm/utils/generation.py` & `mamba_ssm-2.0.1/mamba_ssm/utils/generation.py`

 * *Files identical despite different names*

### Comparing `mamba_ssm-2.0.0/mamba_ssm/utils/hf.py` & `mamba_ssm-2.0.1/mamba_ssm/utils/hf.py`

 * *Files identical despite different names*

### Comparing `mamba_ssm-2.0.0/mamba_ssm.egg-info/PKG-INFO` & `mamba_ssm-2.0.1/mamba_ssm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mamba-ssm
-Version: 2.0.0
+Version: 2.0.1
 Summary: Mamba state-space model
 Home-page: https://github.com/state-spaces/mamba
 Author: Tri Dao, Albert Gu
 Author-email: tri@tridao.me, agu@cs.cmu.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: Unix
@@ -14,16 +14,16 @@
 License-File: AUTHORS
 
 # Mamba
 
 ![Mamba](assets/selection.png "Selective State Space")
 > **Mamba: Linear-Time Sequence Modeling with Selective State Spaces**\
 > Albert Gu*, Tri Dao*\
-> Paper: https://arxiv.org/abs/2312.00752
-> **Transformers are {SSM}s: Generalized Models and Efficient Algorithms Through Structured State Space Duality**\
+> Paper: https://arxiv.org/abs/2312.00752\ 
+> **Transformers are SSMs: Generalized Models and Efficient Algorithms Through Structured State Space Duality**\ 
 > Tri Dao*, Albert Gu*\
 > Paper: https://arxiv.org/abs/2405.21060
 
 ## About
 
 Mamba is a new state space model architecture showing promising performance on information-dense data such as language modeling, where previous subquadratic models fall short of Transformers.
 It is based on the line of progress on [structured state space models](https://github.com/state-spaces/s4),
```

### Comparing `mamba_ssm-2.0.0/mamba_ssm.egg-info/SOURCES.txt` & `mamba_ssm-2.0.1/mamba_ssm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mamba_ssm-2.0.0/setup.py` & `mamba_ssm-2.0.1/setup.py`

 * *Files identical despite different names*

