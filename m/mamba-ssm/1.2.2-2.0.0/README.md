# Comparing `tmp/mamba_ssm-1.2.2.tar.gz` & `tmp/mamba_ssm-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mamba_ssm-1.2.2.tar", last modified: Sun May 26 21:17:35 2024, max compression
+gzip compressed data, was "mamba_ssm-2.0.0.tar", last modified: Mon Jun  3 07:46:07 2024, max compression
```

## Comparing `mamba_ssm-1.2.2.tar` & `mamba_ssm-2.0.0.tar`

### file list

```diff
@@ -1,33 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:17:35.503698 mamba_ssm-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-26 21:17:06.000000 mamba_ssm-1.2.2/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)    11348 2024-05-26 21:17:06.000000 mamba_ssm-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9003 2024-05-26 21:17:35.503698 mamba_ssm-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8553 2024-05-26 21:17:06.000000 mamba_ssm-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:17:35.499698 mamba_ssm-1.2.2/mamba_ssm/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-26 21:17:06.000000 mamba_ssm-1.2.2/mamba_ssm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:17:35.503698 mamba_ssm-1.2.2/mamba_ssm/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 21:17:06.000000 mamba_ssm-1.2.2/mamba_ssm/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-26 21:17:06.000000 mamba_ssm-1.2.2/mamba_ssm/models/config_mamba.py
--rw-r--r--   0 runner    (1001) docker     (127)     9972 2024-05-26 21:17:06.000000 mamba_ssm-1.2.2/mamba_ssm/models/mixer_seq_simple.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:17:35.503698 mamba_ssm-1.2.2/mamba_ssm/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 21:17:06.000000 mamba_ssm-1.2.2/mamba_ssm/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14291 2024-05-26 21:17:06.000000 mamba_ssm-1.2.2/mamba_ssm/modules/mamba_simple.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:17:35.503698 mamba_ssm-1.2.2/mamba_ssm/ops/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 21:17:06.000000 mamba_ssm-1.2.2/mamba_ssm/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16835 2024-05-26 21:17:06.000000 mamba_ssm-1.2.2/mamba_ssm/ops/selective_scan_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:17:35.503698 mamba_ssm-1.2.2/mamba_ssm/ops/triton/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 21:17:06.000000 mamba_ssm-1.2.2/mamba_ssm/ops/triton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21303 2024-05-26 21:17:06.000000 mamba_ssm-1.2.2/mamba_ssm/ops/triton/layernorm.py
--rw-r--r--   0 runner    (1001) docker     (127)    10720 2024-05-26 21:17:06.000000 mamba_ssm-1.2.2/mamba_ssm/ops/triton/selective_state_update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:17:35.503698 mamba_ssm-1.2.2/mamba_ssm/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 21:17:06.000000 mamba_ssm-1.2.2/mamba_ssm/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15363 2024-05-26 21:17:06.000000 mamba_ssm-1.2.2/mamba_ssm/utils/generation.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-26 21:17:06.000000 mamba_ssm-1.2.2/mamba_ssm/utils/hf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:17:35.499698 mamba_ssm-1.2.2/mamba_ssm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9003 2024-05-26 21:17:35.000000 mamba_ssm-1.2.2/mamba_ssm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-26 21:17:35.000000 mamba_ssm-1.2.2/mamba_ssm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 21:17:35.000000 mamba_ssm-1.2.2/mamba_ssm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-26 21:17:35.000000 mamba_ssm-1.2.2/mamba_ssm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-26 21:17:35.000000 mamba_ssm-1.2.2/mamba_ssm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 21:17:35.503698 mamba_ssm-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    10784 2024-05-26 21:17:06.000000 mamba_ssm-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:46:07.289350 mamba_ssm-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-06-03 07:45:38.000000 mamba_ssm-2.0.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)    11348 2024-06-03 07:45:38.000000 mamba_ssm-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10738 2024-06-03 07:46:07.289350 mamba_ssm-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10288 2024-06-03 07:45:38.000000 mamba_ssm-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:46:07.285350 mamba_ssm-2.0.0/mamba_ssm/
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-06-03 07:45:38.000000 mamba_ssm-2.0.0/mamba_ssm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:46:07.285350 mamba_ssm-2.0.0/mamba_ssm/distributed/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 07:45:38.000000 mamba_ssm-2.0.0/mamba_ssm/distributed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5825 2024-06-03 07:45:38.000000 mamba_ssm-2.0.0/mamba_ssm/distributed/distributed_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11995 2024-06-03 07:45:38.000000 mamba_ssm-2.0.0/mamba_ssm/distributed/tensor_parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:46:07.285350 mamba_ssm-2.0.0/mamba_ssm/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 07:45:38.000000 mamba_ssm-2.0.0/mamba_ssm/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-06-03 07:45:38.000000 mamba_ssm-2.0.0/mamba_ssm/models/config_mamba.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11651 2024-06-03 07:45:38.000000 mamba_ssm-2.0.0/mamba_ssm/models/mixer_seq_simple.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:46:07.285350 mamba_ssm-2.0.0/mamba_ssm/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 07:45:38.000000 mamba_ssm-2.0.0/mamba_ssm/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-06-03 07:45:38.000000 mamba_ssm-2.0.0/mamba_ssm/modules/block.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16051 2024-06-03 07:45:38.000000 mamba_ssm-2.0.0/mamba_ssm/modules/mamba2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7567 2024-06-03 07:45:38.000000 mamba_ssm-2.0.0/mamba_ssm/modules/mamba2_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11710 2024-06-03 07:45:38.000000 mamba_ssm-2.0.0/mamba_ssm/modules/mamba_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12969 2024-06-03 07:45:38.000000 mamba_ssm-2.0.0/mamba_ssm/modules/mha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-06-03 07:45:38.000000 mamba_ssm-2.0.0/mamba_ssm/modules/mlp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:46:07.289350 mamba_ssm-2.0.0/mamba_ssm/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 07:45:38.000000 mamba_ssm-2.0.0/mamba_ssm/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16835 2024-06-03 07:45:38.000000 mamba_ssm-2.0.0/mamba_ssm/ops/selective_scan_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:46:07.289350 mamba_ssm-2.0.0/mamba_ssm/ops/triton/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 07:45:38.000000 mamba_ssm-2.0.0/mamba_ssm/ops/triton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35020 2024-06-03 07:45:38.000000 mamba_ssm-2.0.0/mamba_ssm/ops/triton/layer_norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17763 2024-06-03 07:45:38.000000 mamba_ssm-2.0.0/mamba_ssm/ops/triton/layernorm_gated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10720 2024-06-03 07:45:38.000000 mamba_ssm-2.0.0/mamba_ssm/ops/triton/selective_state_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13637 2024-06-03 07:45:38.000000 mamba_ssm-2.0.0/mamba_ssm/ops/triton/ssd_bmm.py
+-rw-r--r--   0 runner    (1001) docker     (127)   104940 2024-06-03 07:45:38.000000 mamba_ssm-2.0.0/mamba_ssm/ops/triton/ssd_chunk_scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49075 2024-06-03 07:45:38.000000 mamba_ssm-2.0.0/mamba_ssm/ops/triton/ssd_chunk_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51735 2024-06-03 07:45:38.000000 mamba_ssm-2.0.0/mamba_ssm/ops/triton/ssd_combined.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16377 2024-06-03 07:45:38.000000 mamba_ssm-2.0.0/mamba_ssm/ops/triton/ssd_state_passing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:46:07.289350 mamba_ssm-2.0.0/mamba_ssm/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 07:45:38.000000 mamba_ssm-2.0.0/mamba_ssm/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15363 2024-06-03 07:45:38.000000 mamba_ssm-2.0.0/mamba_ssm/utils/generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-06-03 07:45:38.000000 mamba_ssm-2.0.0/mamba_ssm/utils/hf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:46:07.285350 mamba_ssm-2.0.0/mamba_ssm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10738 2024-06-03 07:46:07.000000 mamba_ssm-2.0.0/mamba_ssm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-06-03 07:46:07.000000 mamba_ssm-2.0.0/mamba_ssm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 07:46:07.000000 mamba_ssm-2.0.0/mamba_ssm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-06-03 07:46:07.000000 mamba_ssm-2.0.0/mamba_ssm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-03 07:46:07.000000 mamba_ssm-2.0.0/mamba_ssm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 07:46:07.289350 mamba_ssm-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    10784 2024-06-03 07:45:38.000000 mamba_ssm-2.0.0/setup.py
```

### Comparing `mamba_ssm-1.2.2/LICENSE` & `mamba_ssm-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mamba_ssm-1.2.2/PKG-INFO` & `mamba_ssm-2.0.0/mamba_ssm.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: mamba_ssm
-Version: 1.2.2
+Name: mamba-ssm
+Version: 2.0.0
 Summary: Mamba state-space model
 Home-page: https://github.com/state-spaces/mamba
 Author: Tri Dao, Albert Gu
 Author-email: tri@tridao.me, agu@cs.cmu.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: Unix
@@ -15,14 +15,17 @@
 
 # Mamba
 
 ![Mamba](assets/selection.png "Selective State Space")
 > **Mamba: Linear-Time Sequence Modeling with Selective State Spaces**\
 > Albert Gu*, Tri Dao*\
 > Paper: https://arxiv.org/abs/2312.00752
+> **Transformers are {SSM}s: Generalized Models and Efficient Algorithms Through Structured State Space Duality**\
+> Tri Dao*, Albert Gu*\
+> Paper: https://arxiv.org/abs/2405.21060
 
 ## About
 
 Mamba is a new state space model architecture showing promising performance on information-dense data such as language modeling, where previous subquadratic models fall short of Transformers.
 It is based on the line of progress on [structured state space models](https://github.com/state-spaces/s4),
 with an efficient hardware-aware design and implementation in the spirit of [FlashAttention](https://github.com/Dao-AILab/flash-attention).
 
@@ -54,15 +57,15 @@
 ### Mamba Block
 
 The main module of this repository is the Mamba architecture block wrapping the selective SSM.
 
 Source: [modules/mamba_simple.py](mamba_ssm/modules/mamba_simple.py).
 
 Usage:
-```
+``` python
 import torch
 from mamba_ssm import Mamba
 
 batch, length, dim = 2, 64, 16
 x = torch.randn(batch, length, dim).to("cuda")
 model = Mamba(
     # This module uses roughly 3 * expand * d_model^2 parameters
@@ -71,30 +74,48 @@
     d_conv=4,    # Local convolution width
     expand=2,    # Block expansion factor
 ).to("cuda")
 y = model(x)
 assert y.shape == x.shape
 ```
 
+The Mamba-2 block is implemented at [modules/mamba2.py](mamba_ssm/modules/mamba2.py).
+
+A simpler version is at [modules/mamba2_simple.py](mamba_ssm/modules/mamba2_simple.py)
+
+The usage is similar to Mamba(-1):
+``` python
+from mamba_ssm import Mamba2
+model = Mamba(
+    # This module uses roughly 3 * expand * d_model^2 parameters
+    d_model=dim, # Model dimension d_model
+    d_state=64,  # SSM state expansion factor, typically 64 or 128
+    d_conv=4,    # Local convolution width
+    expand=2,    # Block expansion factor
+).to("cuda")
+y = model(x)
+assert y.shape == x.shape
+```
+
 ### Mamba Language Model
 
 Finally, we provide an example of a complete language model: a deep sequence model backbone (with repeating Mamba blocks) + language model head.
 
 Source: [models/mixer_seq_simple.py](mamba_ssm/models/mixer_seq_simple.py).
 
 This is an example of how to integrate Mamba into an end-to-end neural network.
 This example is used in the generation scripts below.
 
 
-
 ## Pretrained Models
 
 Pretrained models are uploaded to
 [Hugging Face](https://huggingface.co/state-spaces): `mamba-130m`, `mamba-370m`,
-`mamba-790m`, `mamba-1.4b`, `mamba-2.8b`, trained on 300B tokens on the Pile, as well as `mamba-2.8b-slimpj`
+`mamba-790m`, `mamba-1.4b`, `mamba-2.8b`, `mamba2-130m`, `mamba2-370m`,
+`mamba2-780m`, `mamba2-1.3b`, `mamba2-2.7b`, `transformerpp-2.7b`, `mamba2attn-2.7b`, trained on 300B tokens on the Pile, as well as `mamba-2.8b-slimpj`
 (trained on 600B tokens on the SlimPajama dataset).
 
 
 The models will be autodownloaded by the generation script below.
 
 These models were trained on the [Pile](https://huggingface.co/datasets/EleutherAI/pile), and follow the standard model dimensions described by GPT-3 and followed by many open source models:
 
@@ -112,31 +133,35 @@
 Performance is expected to be comparable or better than other architectures trained on similar data, but not to match larger or fine-tuned models.
 
 
 ## Evaluations
 
 To run zero-shot evaluations of models (corresponding to Table 3 of the paper),
 we use the
-[lm-evaluation-harness](https://github.com/EleutherAI/lm-evaluation-harness/tree/big-refactor)
+[lm-evaluation-harness](https://github.com/EleutherAI/lm-evaluation-harness)
 library.
 
-1. Pull the `lm-evaluation-harness` repo by `git submodule update --init
-   --recursive`. We use the `big-refactor` branch.
-2. Install `lm-evaluation-harness`: `pip install -e 3rdparty/lm-evaluation-harness`.
-On Python 3.10 you might need to manually install the latest version of `promptsource`: `pip install git+https://github.com/bigscience-workshop/promptsource.git`.
-3. Run evaluation with (more documentation at the [lm-evaluation-harness](https://github.com/EleutherAI/lm-evaluation-harness/tree/big-refactor) repo):
-```
-python evals/lm_harness_eval.py --model mamba --model_args pretrained=state-spaces/mamba-130m --tasks lambada_openai,hellaswag,piqa,arc_easy,arc_challenge,winogrande --device cuda --batch_size 64
+1. Install `lm-evaluation-harness` by `pip install lm-eval==0.4.2`.
+2. Run evaluation with (more documentation at the [lm-evaluation-harness](https://github.com/EleutherAI/lm-evaluation-harness/tree/big-refactor) repo):
+``` sh
+lm_eval --model mamba_ssm --model_args pretrained=state-spaces/mamba-130m --tasks lambada_openai,hellaswag,piqa,arc_easy,arc_challenge,winogrande,openbookqa --device cuda --batch_size 256
 python evals/lm_harness_eval.py --model hf --model_args pretrained=EleutherAI/pythia-160m --tasks lambada_openai,hellaswag,piqa,arc_easy,arc_challenge,winogrande --device cuda --batch_size 64
 ```
 
 To reproduce the results on the `mamba-2.8b-slimpj` model reported in the blogposts:
+``` sh
+lm_eval --model mamba_ssm --model_args pretrained=state-spaces/mamba-2.8b-slimpj --tasks boolq,piqa,hellaswag,winogrande,arc_easy,arc_challenge,openbookqa,race,truthfulqa_mc2 --device cuda --batch_size 256
+lm_eval --model mamba_ssm --model_args pretrained=state-spaces/mamba-2.8b-slimpj --tasks mmlu --num_fewshot 5 --device cuda --batch_size 256
 ```
-python evals/lm_harness_eval.py --model mamba --model_args pretrained=state-spaces/mamba-2.8b-slimpj --tasks boolq,piqa,hellaswag,winogrande,arc_easy,arc_challenge,openbookqa,race,truthfulqa_mc2 --device cuda --batch_size 64
-python evals/lm_harness_eval.py --model mamba --model_args pretrained=state-spaces/mamba-2.8b-slimpj --tasks mmlu --num_fewshot 5 --device cuda --batch_size 64
+
+To run evaluations on Mamba-2 models, simply replace the model names:
+``` sh
+lm_eval --model mamba_ssm --model_args pretrained=state-spaces/mamba2-2.7b --tasks lambada_openai,hellaswag,piqa,arc_easy,arc_challenge,winogrande,openbookqa --device cuda --batch_size 256
+lm_eval --model mamba_ssm --model_args pretrained=state-spaces/transformerpp-2.7b --tasks lambada_openai,hellaswag,piqa,arc_easy,arc_challenge,winogrande,openbookqa --device cuda --batch_size 256
+lm_eval --model mamba_ssm --model_args pretrained=state-spaces/mamba2attn-2.7b --tasks lambada_openai,hellaswag,piqa,arc_easy,arc_challenge,winogrande,openbookqa --device cuda --batch_size 256
 ```
 
 Note that the result of each task might differ from reported values by 0.1-0.3 due to noise in the evaluation process.
 
 ## Inference
 
 The script [benchmarks/benchmark_generation_mamba_simple.py](benchmarks/benchmark_generation_mamba_simple.py)
@@ -146,24 +171,29 @@
 
 Other configurable options include the top-p (nucleus sampling) probability, and the softmax temperature.
 
 ### Examples
 
 To test generation latency (e.g. batch size = 1) with different sampling strategies:
 
-```
+``` sh
 python benchmarks/benchmark_generation_mamba_simple.py --model-name "state-spaces/mamba-2.8b" --prompt "My cat wrote all this CUDA code for a new language model and" --topp 0.9 --temperature 0.7 --repetition-penalty 1.2
 python benchmarks/benchmark_generation_mamba_simple.py --model-name "EleutherAI/pythia-2.8b" --prompt "My cat wrote all this CUDA code for a new language model and" --topp 0.9 --temperature 0.7 --repetition-penalty 1.2
 python benchmarks/benchmark_generation_mamba_simple.py --model-name "state-spaces/mamba-2.8b" --prompt "My cat wrote all this CUDA code for a new language model and" --minp 0.05 --topk 0 --temperature 0.7 --repetition-penalty 1.2
 ```
 
 To test generation throughput with random prompts (e.g. large batch size):
+``` sh
+python benchmarks/benchmark_generation_mamba_simple.py --model-name "state-spaces/mamba-2.8b" --batch 64
+python benchmarks/benchmark_generation_mamba_simple.py --model-name "EleutherAI/pythia-2.8b" --batch 64
 ```
-python benchmarks/benchmark_generation_mamba_simple.py --model-name "state-spaces/mamba-2.8b" --batch 128
-python benchmarks/benchmark_generation_mamba_simple.py --model-name "EleutherAI/pythia-2.8b" --batch 128
+
+With Mamba-2, you just need to change the model name:
+``` sh
+python benchmarks/benchmark_generation_mamba_simple.py --model-name "state-spaces/mamba2-2.7b" --prompt "My cat wrote all this CUDA code for a new language model and" --topp 0.9 --temperature 0.7 --repetition-penalty 1.2
 ```
 
 
 ## Troubleshooting
 
 ### Precision
 Our models were trained using PyTorch [AMP](https://pytorch.org/docs/stable/amp.html) for mixed precision. AMP keeps model parameters in float32 and casts to half precision when necessary.
@@ -178,16 +208,23 @@
 However, some frameworks may have post-initialization hooks (e.g. setting all bias terms in `nn.Linear` modules to zero).
 If this is the case, you may have to add custom logic (e.g. this [line](https://github.com/state-spaces/mamba/blob/f0affcf69f06d1d06cef018ff640bf080a11c421/mamba_ssm/modules/mamba_simple.py#L104) turns off re-initializing in our trainer, but would be a no-op in any other framework)
 that is specific to the training framework.
 
 
 ## Citation
 
-If you use this codebase, or otherwise found our work valuable, please cite Mamba:
+If you use this codebase, or otherwise find our work valuable, please cite Mamba:
 ```
 @article{mamba,
   title={Mamba: Linear-Time Sequence Modeling with Selective State Spaces},
   author={Gu, Albert and Dao, Tri},
   journal={arXiv preprint arXiv:2312.00752},
   year={2023}
 }
+@inproceedings{mamba2,
+  title={Transformers are {SSM}s: Generalized Models and Efficient Algorithms Through Structured State Space Duality},
+  author={Dao, Tri and Gu, Albert},
+  booktitle={International Conference on Machine Learning (ICML)},
+  year={2024}
+}
+
 ```
```

### Comparing `mamba_ssm-1.2.2/README.md` & `mamba_ssm-2.0.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # Mamba
 
 ![Mamba](assets/selection.png "Selective State Space")
 > **Mamba: Linear-Time Sequence Modeling with Selective State Spaces**\
 > Albert Gu*, Tri Dao*\
 > Paper: https://arxiv.org/abs/2312.00752
+> **Transformers are {SSM}s: Generalized Models and Efficient Algorithms Through Structured State Space Duality**\
+> Tri Dao*, Albert Gu*\
+> Paper: https://arxiv.org/abs/2405.21060
 
 ## About
 
 Mamba is a new state space model architecture showing promising performance on information-dense data such as language modeling, where previous subquadratic models fall short of Transformers.
 It is based on the line of progress on [structured state space models](https://github.com/state-spaces/s4),
 with an efficient hardware-aware design and implementation in the spirit of [FlashAttention](https://github.com/Dao-AILab/flash-attention).
 
@@ -39,15 +42,15 @@
 ### Mamba Block
 
 The main module of this repository is the Mamba architecture block wrapping the selective SSM.
 
 Source: [modules/mamba_simple.py](mamba_ssm/modules/mamba_simple.py).
 
 Usage:
-```
+``` python
 import torch
 from mamba_ssm import Mamba
 
 batch, length, dim = 2, 64, 16
 x = torch.randn(batch, length, dim).to("cuda")
 model = Mamba(
     # This module uses roughly 3 * expand * d_model^2 parameters
@@ -56,30 +59,48 @@
     d_conv=4,    # Local convolution width
     expand=2,    # Block expansion factor
 ).to("cuda")
 y = model(x)
 assert y.shape == x.shape
 ```
 
+The Mamba-2 block is implemented at [modules/mamba2.py](mamba_ssm/modules/mamba2.py).
+
+A simpler version is at [modules/mamba2_simple.py](mamba_ssm/modules/mamba2_simple.py)
+
+The usage is similar to Mamba(-1):
+``` python
+from mamba_ssm import Mamba2
+model = Mamba(
+    # This module uses roughly 3 * expand * d_model^2 parameters
+    d_model=dim, # Model dimension d_model
+    d_state=64,  # SSM state expansion factor, typically 64 or 128
+    d_conv=4,    # Local convolution width
+    expand=2,    # Block expansion factor
+).to("cuda")
+y = model(x)
+assert y.shape == x.shape
+```
+
 ### Mamba Language Model
 
 Finally, we provide an example of a complete language model: a deep sequence model backbone (with repeating Mamba blocks) + language model head.
 
 Source: [models/mixer_seq_simple.py](mamba_ssm/models/mixer_seq_simple.py).
 
 This is an example of how to integrate Mamba into an end-to-end neural network.
 This example is used in the generation scripts below.
 
 
-
 ## Pretrained Models
 
 Pretrained models are uploaded to
 [Hugging Face](https://huggingface.co/state-spaces): `mamba-130m`, `mamba-370m`,
-`mamba-790m`, `mamba-1.4b`, `mamba-2.8b`, trained on 300B tokens on the Pile, as well as `mamba-2.8b-slimpj`
+`mamba-790m`, `mamba-1.4b`, `mamba-2.8b`, `mamba2-130m`, `mamba2-370m`,
+`mamba2-780m`, `mamba2-1.3b`, `mamba2-2.7b`, `transformerpp-2.7b`, `mamba2attn-2.7b`, trained on 300B tokens on the Pile, as well as `mamba-2.8b-slimpj`
 (trained on 600B tokens on the SlimPajama dataset).
 
 
 The models will be autodownloaded by the generation script below.
 
 These models were trained on the [Pile](https://huggingface.co/datasets/EleutherAI/pile), and follow the standard model dimensions described by GPT-3 and followed by many open source models:
 
@@ -97,31 +118,35 @@
 Performance is expected to be comparable or better than other architectures trained on similar data, but not to match larger or fine-tuned models.
 
 
 ## Evaluations
 
 To run zero-shot evaluations of models (corresponding to Table 3 of the paper),
 we use the
-[lm-evaluation-harness](https://github.com/EleutherAI/lm-evaluation-harness/tree/big-refactor)
+[lm-evaluation-harness](https://github.com/EleutherAI/lm-evaluation-harness)
 library.
 
-1. Pull the `lm-evaluation-harness` repo by `git submodule update --init
-   --recursive`. We use the `big-refactor` branch.
-2. Install `lm-evaluation-harness`: `pip install -e 3rdparty/lm-evaluation-harness`.
-On Python 3.10 you might need to manually install the latest version of `promptsource`: `pip install git+https://github.com/bigscience-workshop/promptsource.git`.
-3. Run evaluation with (more documentation at the [lm-evaluation-harness](https://github.com/EleutherAI/lm-evaluation-harness/tree/big-refactor) repo):
-```
-python evals/lm_harness_eval.py --model mamba --model_args pretrained=state-spaces/mamba-130m --tasks lambada_openai,hellaswag,piqa,arc_easy,arc_challenge,winogrande --device cuda --batch_size 64
+1. Install `lm-evaluation-harness` by `pip install lm-eval==0.4.2`.
+2. Run evaluation with (more documentation at the [lm-evaluation-harness](https://github.com/EleutherAI/lm-evaluation-harness/tree/big-refactor) repo):
+``` sh
+lm_eval --model mamba_ssm --model_args pretrained=state-spaces/mamba-130m --tasks lambada_openai,hellaswag,piqa,arc_easy,arc_challenge,winogrande,openbookqa --device cuda --batch_size 256
 python evals/lm_harness_eval.py --model hf --model_args pretrained=EleutherAI/pythia-160m --tasks lambada_openai,hellaswag,piqa,arc_easy,arc_challenge,winogrande --device cuda --batch_size 64
 ```
 
 To reproduce the results on the `mamba-2.8b-slimpj` model reported in the blogposts:
+``` sh
+lm_eval --model mamba_ssm --model_args pretrained=state-spaces/mamba-2.8b-slimpj --tasks boolq,piqa,hellaswag,winogrande,arc_easy,arc_challenge,openbookqa,race,truthfulqa_mc2 --device cuda --batch_size 256
+lm_eval --model mamba_ssm --model_args pretrained=state-spaces/mamba-2.8b-slimpj --tasks mmlu --num_fewshot 5 --device cuda --batch_size 256
 ```
-python evals/lm_harness_eval.py --model mamba --model_args pretrained=state-spaces/mamba-2.8b-slimpj --tasks boolq,piqa,hellaswag,winogrande,arc_easy,arc_challenge,openbookqa,race,truthfulqa_mc2 --device cuda --batch_size 64
-python evals/lm_harness_eval.py --model mamba --model_args pretrained=state-spaces/mamba-2.8b-slimpj --tasks mmlu --num_fewshot 5 --device cuda --batch_size 64
+
+To run evaluations on Mamba-2 models, simply replace the model names:
+``` sh
+lm_eval --model mamba_ssm --model_args pretrained=state-spaces/mamba2-2.7b --tasks lambada_openai,hellaswag,piqa,arc_easy,arc_challenge,winogrande,openbookqa --device cuda --batch_size 256
+lm_eval --model mamba_ssm --model_args pretrained=state-spaces/transformerpp-2.7b --tasks lambada_openai,hellaswag,piqa,arc_easy,arc_challenge,winogrande,openbookqa --device cuda --batch_size 256
+lm_eval --model mamba_ssm --model_args pretrained=state-spaces/mamba2attn-2.7b --tasks lambada_openai,hellaswag,piqa,arc_easy,arc_challenge,winogrande,openbookqa --device cuda --batch_size 256
 ```
 
 Note that the result of each task might differ from reported values by 0.1-0.3 due to noise in the evaluation process.
 
 ## Inference
 
 The script [benchmarks/benchmark_generation_mamba_simple.py](benchmarks/benchmark_generation_mamba_simple.py)
@@ -131,24 +156,29 @@
 
 Other configurable options include the top-p (nucleus sampling) probability, and the softmax temperature.
 
 ### Examples
 
 To test generation latency (e.g. batch size = 1) with different sampling strategies:
 
-```
+``` sh
 python benchmarks/benchmark_generation_mamba_simple.py --model-name "state-spaces/mamba-2.8b" --prompt "My cat wrote all this CUDA code for a new language model and" --topp 0.9 --temperature 0.7 --repetition-penalty 1.2
 python benchmarks/benchmark_generation_mamba_simple.py --model-name "EleutherAI/pythia-2.8b" --prompt "My cat wrote all this CUDA code for a new language model and" --topp 0.9 --temperature 0.7 --repetition-penalty 1.2
 python benchmarks/benchmark_generation_mamba_simple.py --model-name "state-spaces/mamba-2.8b" --prompt "My cat wrote all this CUDA code for a new language model and" --minp 0.05 --topk 0 --temperature 0.7 --repetition-penalty 1.2
 ```
 
 To test generation throughput with random prompts (e.g. large batch size):
+``` sh
+python benchmarks/benchmark_generation_mamba_simple.py --model-name "state-spaces/mamba-2.8b" --batch 64
+python benchmarks/benchmark_generation_mamba_simple.py --model-name "EleutherAI/pythia-2.8b" --batch 64
 ```
-python benchmarks/benchmark_generation_mamba_simple.py --model-name "state-spaces/mamba-2.8b" --batch 128
-python benchmarks/benchmark_generation_mamba_simple.py --model-name "EleutherAI/pythia-2.8b" --batch 128
+
+With Mamba-2, you just need to change the model name:
+``` sh
+python benchmarks/benchmark_generation_mamba_simple.py --model-name "state-spaces/mamba2-2.7b" --prompt "My cat wrote all this CUDA code for a new language model and" --topp 0.9 --temperature 0.7 --repetition-penalty 1.2
 ```
 
 
 ## Troubleshooting
 
 ### Precision
 Our models were trained using PyTorch [AMP](https://pytorch.org/docs/stable/amp.html) for mixed precision. AMP keeps model parameters in float32 and casts to half precision when necessary.
@@ -163,16 +193,23 @@
 However, some frameworks may have post-initialization hooks (e.g. setting all bias terms in `nn.Linear` modules to zero).
 If this is the case, you may have to add custom logic (e.g. this [line](https://github.com/state-spaces/mamba/blob/f0affcf69f06d1d06cef018ff640bf080a11c421/mamba_ssm/modules/mamba_simple.py#L104) turns off re-initializing in our trainer, but would be a no-op in any other framework)
 that is specific to the training framework.
 
 
 ## Citation
 
-If you use this codebase, or otherwise found our work valuable, please cite Mamba:
+If you use this codebase, or otherwise find our work valuable, please cite Mamba:
 ```
 @article{mamba,
   title={Mamba: Linear-Time Sequence Modeling with Selective State Spaces},
   author={Gu, Albert and Dao, Tri},
   journal={arXiv preprint arXiv:2312.00752},
   year={2023}
 }
+@inproceedings{mamba2,
+  title={Transformers are {SSM}s: Generalized Models and Efficient Algorithms Through Structured State Space Duality},
+  author={Dao, Tri and Gu, Albert},
+  booktitle={International Conference on Machine Learning (ICML)},
+  year={2024}
+}
+
 ```
```

### Comparing `mamba_ssm-1.2.2/mamba_ssm/models/mixer_seq_simple.py` & `mamba_ssm-2.0.0/mamba_ssm/models/mixer_seq_simple.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,51 +1,83 @@
 # Copyright (c) 2023, Albert Gu, Tri Dao.
 
 import math
 from functools import partial
 import json
 import os
+import copy
 
 from collections import namedtuple
 
 import torch
 import torch.nn as nn
 
 from mamba_ssm.models.config_mamba import MambaConfig
-from mamba_ssm.modules.mamba_simple import Mamba, Block
+from mamba_ssm.modules.mamba_simple import Mamba
+from mamba_ssm.modules.mamba2 import Mamba2
+from mamba_ssm.modules.mha import MHA
+from mamba_ssm.modules.mlp import GatedMLP
+from mamba_ssm.modules.block import Block
 from mamba_ssm.utils.generation import GenerationMixin
 from mamba_ssm.utils.hf import load_config_hf, load_state_dict_hf
 
 try:
-    from mamba_ssm.ops.triton.layernorm import RMSNorm, layer_norm_fn, rms_norm_fn
+    from mamba_ssm.ops.triton.layer_norm import RMSNorm, layer_norm_fn, rms_norm_fn
 except ImportError:
     RMSNorm, layer_norm_fn, rms_norm_fn = None, None, None
 
 
 def create_block(
     d_model,
+    d_intermediate,
     ssm_cfg=None,
+    attn_layer_idx=None,
+    attn_cfg=None,
     norm_epsilon=1e-5,
     rms_norm=False,
     residual_in_fp32=False,
     fused_add_norm=False,
     layer_idx=None,
     device=None,
     dtype=None,
 ):
     if ssm_cfg is None:
         ssm_cfg = {}
+    if attn_layer_idx is None:
+        attn_layer_idx = []
+    if attn_cfg is None:
+        attn_cfg = {}
     factory_kwargs = {"device": device, "dtype": dtype}
-    mixer_cls = partial(Mamba, layer_idx=layer_idx, **ssm_cfg, **factory_kwargs)
+    if layer_idx not in attn_layer_idx:
+        # Create a copy of the config to modify
+        ssm_cfg = copy.deepcopy(ssm_cfg) if ssm_cfg is not None else {}
+        ssm_layer = ssm_cfg.pop("layer", "Mamba1")
+        if ssm_layer not in ["Mamba1", "Mamba2"]:
+            raise ValueError(f"Invalid ssm_layer: {ssm_layer}, only support Mamba1 and Mamba2")
+        mixer_cls = partial(
+            Mamba2 if ssm_layer == "Mamba2" else Mamba,
+            layer_idx=layer_idx,
+            **ssm_cfg,
+            **factory_kwargs
+        )
+    else:
+        mixer_cls = partial(MHA, layer_idx=layer_idx, **attn_cfg, **factory_kwargs)
     norm_cls = partial(
         nn.LayerNorm if not rms_norm else RMSNorm, eps=norm_epsilon, **factory_kwargs
     )
+    if d_intermediate == 0:
+        mlp_cls = nn.Identity
+    else:
+        mlp_cls = partial(
+            GatedMLP, hidden_features=d_intermediate, out_features=d_model, **factory_kwargs
+        )
     block = Block(
         d_model,
         mixer_cls,
+        mlp_cls,
         norm_cls=norm_cls,
         fused_add_norm=fused_add_norm,
         residual_in_fp32=residual_in_fp32,
     )
     block.layer_idx = layer_idx
     return block
 
@@ -84,16 +116,19 @@
 
 
 class MixerModel(nn.Module):
     def __init__(
         self,
         d_model: int,
         n_layer: int,
+        d_intermediate: int,
         vocab_size: int,
         ssm_cfg=None,
+        attn_layer_idx=None,
+        attn_cfg=None,
         norm_epsilon: float = 1e-5,
         rms_norm: bool = False,
         initializer_cfg=None,
         fused_add_norm=False,
         residual_in_fp32=False,
         device=None,
         dtype=None,
@@ -114,15 +149,18 @@
             if layer_norm_fn is None or rms_norm_fn is None:
                 raise ImportError("Failed to import Triton LayerNorm / RMSNorm kernels")
 
         self.layers = nn.ModuleList(
             [
                 create_block(
                     d_model,
+                    d_intermediate=d_intermediate,
                     ssm_cfg=ssm_cfg,
+                    attn_layer_idx=attn_layer_idx,
+                    attn_cfg=attn_cfg,
                     norm_epsilon=norm_epsilon,
                     rms_norm=rms_norm,
                     residual_in_fp32=residual_in_fp32,
                     fused_add_norm=fused_add_norm,
                     layer_idx=i,
                     **factory_kwargs,
                 )
@@ -135,44 +173,45 @@
         )
 
         self.apply(
             partial(
                 _init_weights,
                 n_layer=n_layer,
                 **(initializer_cfg if initializer_cfg is not None else {}),
+                n_residuals_per_layer=1 if d_intermediate == 0 else 2,  # 2 if we have MLP
             )
         )
 
     def allocate_inference_cache(self, batch_size, max_seqlen, dtype=None, **kwargs):
         return {
             i: layer.allocate_inference_cache(batch_size, max_seqlen, dtype=dtype, **kwargs)
             for i, layer in enumerate(self.layers)
         }
 
-    def forward(self, input_ids, inference_params=None):
+    def forward(self, input_ids, inference_params=None, **mixer_kwargs):
         hidden_states = self.embedding(input_ids)
         residual = None
         for layer in self.layers:
             hidden_states, residual = layer(
                 hidden_states, residual, inference_params=inference_params
             )
         if not self.fused_add_norm:
             residual = (hidden_states + residual) if residual is not None else hidden_states
             hidden_states = self.norm_f(residual.to(dtype=self.norm_f.weight.dtype))
         else:
             # Set prenorm=False here since we don't need the residual
-            fused_add_norm_fn = rms_norm_fn if isinstance(self.norm_f, RMSNorm) else layer_norm_fn
-            hidden_states = fused_add_norm_fn(
+            hidden_states = layer_norm_fn(
                 hidden_states,
                 self.norm_f.weight,
                 self.norm_f.bias,
                 eps=self.norm_f.eps,
                 residual=residual,
                 prenorm=False,
                 residual_in_fp32=self.residual_in_fp32,
+                is_rms_norm=isinstance(self.norm_f, RMSNorm)
             )
         return hidden_states
 
 
 class MambaLMHeadModel(nn.Module, GenerationMixin):
 
     def __init__(
@@ -181,30 +220,36 @@
         initializer_cfg=None,
         device=None,
         dtype=None,
     ) -> None:
         self.config = config
         d_model = config.d_model
         n_layer = config.n_layer
+        d_intermediate = config.d_intermediate
         vocab_size = config.vocab_size
         ssm_cfg = config.ssm_cfg
+        attn_layer_idx = config.attn_layer_idx
+        attn_cfg = config.attn_cfg
         rms_norm = config.rms_norm
         residual_in_fp32 = config.residual_in_fp32
         fused_add_norm = config.fused_add_norm
         pad_vocab_size_multiple = config.pad_vocab_size_multiple
         factory_kwargs = {"device": device, "dtype": dtype}
 
         super().__init__()
         if vocab_size % pad_vocab_size_multiple != 0:
             vocab_size += pad_vocab_size_multiple - (vocab_size % pad_vocab_size_multiple)
         self.backbone = MixerModel(
             d_model=d_model,
             n_layer=n_layer,
+            d_intermediate=d_intermediate,
             vocab_size=vocab_size,
             ssm_cfg=ssm_cfg,
+            attn_layer_idx=attn_layer_idx,
+            attn_cfg=attn_cfg,
             rms_norm=rms_norm,
             initializer_cfg=initializer_cfg,
             fused_add_norm=fused_add_norm,
             residual_in_fp32=residual_in_fp32,
             **factory_kwargs,
         )
         self.lm_head = nn.Linear(d_model, vocab_size, bias=False, **factory_kwargs)
@@ -218,24 +263,24 @@
             )
         )
         self.tie_weights()
 
     def tie_weights(self):
         if self.config.tie_embeddings:
             self.lm_head.weight = self.backbone.embedding.weight
-    
+
     def allocate_inference_cache(self, batch_size, max_seqlen, dtype=None, **kwargs):
         return self.backbone.allocate_inference_cache(batch_size, max_seqlen, dtype=dtype, **kwargs)
 
-    def forward(self, input_ids, position_ids=None, inference_params=None, num_last_tokens=0):
+    def forward(self, input_ids, position_ids=None, inference_params=None, num_last_tokens=0, **mixer_kwargs):
         """
         "position_ids" is just to be compatible with Transformer generation. We don't use it.
         num_last_tokens: if > 0, only return the logits for the last n tokens
         """
-        hidden_states = self.backbone(input_ids, inference_params=inference_params)
+        hidden_states = self.backbone(input_ids, inference_params=inference_params, **mixer_kwargs)
         if num_last_tokens > 0:
             hidden_states = hidden_states[:, -num_last_tokens:]
         lm_logits = self.lm_head(hidden_states)
         CausalLMOutput = namedtuple("CausalLMOutput", ["logits"])
         return CausalLMOutput(logits=lm_logits)
 
     @classmethod
@@ -257,8 +302,8 @@
         # Save the model's state_dict
         model_path = os.path.join(save_directory, 'pytorch_model.bin')
         torch.save(self.state_dict(), model_path)
 
         # Save the configuration of the model
         config_path = os.path.join(save_directory, 'config.json')
         with open(config_path, 'w') as f:
-            json.dump(self.config.__dict__, f)
+            json.dump(self.config.__dict__, f, indent=4)
```

### Comparing `mamba_ssm-1.2.2/mamba_ssm/modules/mamba_simple.py` & `mamba_ssm-2.0.0/mamba_ssm/modules/mamba_simple.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 try:
     from mamba_ssm.ops.triton.selective_state_update import selective_state_update
 except ImportError:
     selective_state_update = None
 
 try:
-    from mamba_ssm.ops.triton.layernorm import RMSNorm, layer_norm_fn, rms_norm_fn
+    from mamba_ssm.ops.triton.layer_norm import RMSNorm, layer_norm_fn, rms_norm_fn
 except ImportError:
     RMSNorm, layer_norm_fn, rms_norm_fn = None, None, None
 
 
 class Mamba(nn.Module):
     def __init__(
         self,
@@ -288,66 +288,7 @@
         else:
             conv_state, ssm_state = inference_params.key_value_memory_dict[self.layer_idx]
             # TODO: What if batch size changes between generation, and we reuse the same states?
             if initialize_states:
                 conv_state.zero_()
                 ssm_state.zero_()
         return conv_state, ssm_state
-
-
-class Block(nn.Module):
-    def __init__(
-        self, dim, mixer_cls, norm_cls=nn.LayerNorm, fused_add_norm=False, residual_in_fp32=False
-    ):
-        """
-        Simple block wrapping a mixer class with LayerNorm/RMSNorm and residual connection"
-
-        This Block has a slightly different structure compared to a regular
-        prenorm Transformer block.
-        The standard block is: LN -> MHA/MLP -> Add.
-        [Ref: https://arxiv.org/abs/2002.04745]
-        Here we have: Add -> LN -> Mixer, returning both
-        the hidden_states (output of the mixer) and the residual.
-        This is purely for performance reasons, as we can fuse add and LayerNorm.
-        The residual needs to be provided (except for the very first block).
-        """
-        super().__init__()
-        self.residual_in_fp32 = residual_in_fp32
-        self.fused_add_norm = fused_add_norm
-        self.mixer = mixer_cls(dim)
-        self.norm = norm_cls(dim)
-        if self.fused_add_norm:
-            assert RMSNorm is not None, "RMSNorm import fails"
-            assert isinstance(
-                self.norm, (nn.LayerNorm, RMSNorm)
-            ), "Only LayerNorm and RMSNorm are supported for fused_add_norm"
-
-    def forward(
-        self, hidden_states: Tensor, residual: Optional[Tensor] = None, inference_params=None
-    ):
-        r"""Pass the input through the encoder layer.
-
-        Args:
-            hidden_states: the sequence to the encoder layer (required).
-            residual: hidden_states = Mixer(LN(residual))
-        """
-        if not self.fused_add_norm:
-            residual = (hidden_states + residual) if residual is not None else hidden_states
-            hidden_states = self.norm(residual.to(dtype=self.norm.weight.dtype))
-            if self.residual_in_fp32:
-                residual = residual.to(torch.float32)
-        else:
-            fused_add_norm_fn = rms_norm_fn if isinstance(self.norm, RMSNorm) else layer_norm_fn
-            hidden_states, residual = fused_add_norm_fn(
-                hidden_states,
-                self.norm.weight,
-                self.norm.bias,
-                residual=residual,
-                prenorm=True,
-                residual_in_fp32=self.residual_in_fp32,
-                eps=self.norm.eps,
-            )
-        hidden_states = self.mixer(hidden_states, inference_params=inference_params)
-        return hidden_states, residual
-
-    def allocate_inference_cache(self, batch_size, max_seqlen, dtype=None, **kwargs):
-        return self.mixer.allocate_inference_cache(batch_size, max_seqlen, dtype=dtype, **kwargs)
```

### Comparing `mamba_ssm-1.2.2/mamba_ssm/ops/selective_scan_interface.py` & `mamba_ssm-2.0.0/mamba_ssm/ops/selective_scan_interface.py`

 * *Files identical despite different names*

### Comparing `mamba_ssm-1.2.2/mamba_ssm/ops/triton/layernorm.py` & `mamba_ssm-2.0.0/mamba_ssm/ops/triton/layer_norm.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Copyright (c) 2023, Tri Dao.
-# Implement residual + layer_norm / rms_norm.
+# Copyright (c) 2024, Tri Dao.
+# Implement dropout + residual + layer_norm / rms_norm.
 
 # Based on the Triton LayerNorm tutorial: https://triton-lang.org/main/getting-started/tutorials/05-layer-norm.html
 # For the backward pass, we keep weight_grad and bias_grad in registers and accumulate.
 # This is faster for dimensions up to 8k, but after that it's much slower due to register spilling.
 # The models we train have hidden dim up to 8k anyway (e.g. Llama 70B), so this is fine.
 
 import math
@@ -12,44 +12,121 @@
 import torch.nn.functional as F
 from torch.cuda.amp import custom_fwd, custom_bwd
 
 import triton
 import triton.language as tl
 
 
-def layer_norm_ref(x, weight, bias, residual=None, eps=1e-6, prenorm=False, upcast=False):
+def layer_norm_ref(
+    x,
+    weight,
+    bias,
+    residual=None,
+    x1=None,
+    weight1=None,
+    bias1=None,
+    eps=1e-6,
+    dropout_p=0.0,
+    rowscale=None,
+    prenorm=False,
+    dropout_mask=None,
+    dropout_mask1=None,
+    upcast=False,
+):
     dtype = x.dtype
     if upcast:
+        x = x.float()
         weight = weight.float()
         bias = bias.float() if bias is not None else None
-    if upcast:
-        x = x.float()
         residual = residual.float() if residual is not None else residual
+        x1 = x1.float() if x1 is not None else None
+        weight1 = weight1.float() if weight1 is not None else None
+        bias1 = bias1.float() if bias1 is not None else None
+    if x1 is not None:
+        assert rowscale is None, "rowscale is not supported with parallel LayerNorm"
+    if rowscale is not None:
+        x = x * rowscale[..., None]
+    if dropout_p > 0.0:
+        if dropout_mask is not None:
+            x = x.masked_fill(~dropout_mask, 0.0) / (1.0 - dropout_p)
+        else:
+            x = F.dropout(x, p=dropout_p)
+        if x1 is not None:
+            if dropout_mask1 is not None:
+                x1 = x1.masked_fill(~dropout_mask1, 0.0) / (1.0 - dropout_p)
+            else:
+                x1 = F.dropout(x1, p=dropout_p)
+    if x1 is not None:
+        x = x + x1
     if residual is not None:
         x = (x + residual).to(x.dtype)
     out = F.layer_norm(x.to(weight.dtype), x.shape[-1:], weight=weight, bias=bias, eps=eps).to(
         dtype
     )
-    return out if not prenorm else (out, x)
+    if weight1 is None:
+        return out if not prenorm else (out, x)
+    else:
+        out1 = F.layer_norm(
+            x.to(weight1.dtype), x.shape[-1:], weight=weight1, bias=bias1, eps=eps
+        ).to(dtype)
+        return (out, out1) if not prenorm else (out, out1, x)
 
 
-def rms_norm_ref(x, weight, bias, residual=None, eps=1e-6, prenorm=False, upcast=False):
+def rms_norm_ref(
+    x,
+    weight,
+    bias,
+    residual=None,
+    x1=None,
+    weight1=None,
+    bias1=None,
+    eps=1e-6,
+    dropout_p=0.0,
+    rowscale=None,
+    prenorm=False,
+    dropout_mask=None,
+    dropout_mask1=None,
+    upcast=False,
+):
     dtype = x.dtype
     if upcast:
+        x = x.float()
         weight = weight.float()
         bias = bias.float() if bias is not None else None
-    if upcast:
-        x = x.float()
         residual = residual.float() if residual is not None else residual
+        x1 = x1.float() if x1 is not None else None
+        weight1 = weight1.float() if weight1 is not None else None
+        bias1 = bias1.float() if bias1 is not None else None
+    if x1 is not None:
+        assert rowscale is None, "rowscale is not supported with parallel LayerNorm"
+    if rowscale is not None:
+        x = x * rowscale[..., None]
+    if dropout_p > 0.0:
+        if dropout_mask is not None:
+            x = x.masked_fill(~dropout_mask, 0.0) / (1.0 - dropout_p)
+        else:
+            x = F.dropout(x, p=dropout_p)
+        if x1 is not None:
+            if dropout_mask1 is not None:
+                x1 = x1.masked_fill(~dropout_mask1, 0.0) / (1.0 - dropout_p)
+            else:
+                x1 = F.dropout(x1, p=dropout_p)
+    if x1 is not None:
+        x = x + x1
     if residual is not None:
         x = (x + residual).to(x.dtype)
     rstd = 1 / torch.sqrt((x.square()).mean(dim=-1, keepdim=True) + eps)
-    out = (x * rstd * weight) + bias if bias is not None else (x * rstd * weight)
-    out = out.to(dtype)
-    return out if not prenorm else (out, x)
+    out = ((x * rstd * weight) + bias if bias is not None else (x * rstd * weight)).to(dtype)
+    if weight1 is None:
+        return out if not prenorm else (out, x)
+    else:
+        out1 = ((x * rstd * weight1) + bias1 if bias1 is not None else (x * rstd * weight1)).to(
+            dtype
+        )
+        return (out, out1) if not prenorm else (out, out1, x)
 
 
 @triton.autotune(
     configs=[
         triton.Config({}, num_warps=1),
         triton.Config({}, num_warps=2),
         triton.Config({}, num_warps=4),
@@ -57,47 +134,96 @@
         triton.Config({}, num_warps=16),
         triton.Config({}, num_warps=32),
     ],
     key=["N", "HAS_RESIDUAL", "STORE_RESIDUAL_OUT", "IS_RMS_NORM", "HAS_BIAS"],
 )
 # @triton.heuristics({"HAS_BIAS": lambda args: args["B"] is not None})
 # @triton.heuristics({"HAS_RESIDUAL": lambda args: args["RESIDUAL"] is not None})
+@triton.heuristics({"HAS_X1": lambda args: args["X1"] is not None})
+@triton.heuristics({"HAS_W1": lambda args: args["W1"] is not None})
+@triton.heuristics({"HAS_B1": lambda args: args["B1"] is not None})
 @triton.jit
 def _layer_norm_fwd_1pass_kernel(
     X,  # pointer to the input
     Y,  # pointer to the output
     W,  # pointer to the weights
     B,  # pointer to the biases
     RESIDUAL,  # pointer to the residual
+    X1,
+    W1,
+    B1,
+    Y1,
     RESIDUAL_OUT,  # pointer to the residual
+    ROWSCALE,
+    SEEDS,  # Dropout seeds for each row
+    DROPOUT_MASK,
     Mean,  # pointer to the mean
     Rstd,  # pointer to the 1/std
     stride_x_row,  # how much to increase the pointer when moving by 1 row
     stride_y_row,
     stride_res_row,
     stride_res_out_row,
+    stride_x1_row,
+    stride_y1_row,
+    M,  # number of rows in X
     N,  # number of columns in X
     eps,  # epsilon to avoid division by zero
+    dropout_p,  # Dropout probability
     IS_RMS_NORM: tl.constexpr,
     BLOCK_N: tl.constexpr,
     HAS_RESIDUAL: tl.constexpr,
     STORE_RESIDUAL_OUT: tl.constexpr,
     HAS_BIAS: tl.constexpr,
+    HAS_DROPOUT: tl.constexpr,
+    STORE_DROPOUT_MASK: tl.constexpr,
+    HAS_ROWSCALE: tl.constexpr,
+    HAS_X1: tl.constexpr,
+    HAS_W1: tl.constexpr,
+    HAS_B1: tl.constexpr,
 ):
     # Map the program id to the row of X and Y it should compute.
     row = tl.program_id(0)
     X += row * stride_x_row
     Y += row * stride_y_row
     if HAS_RESIDUAL:
         RESIDUAL += row * stride_res_row
     if STORE_RESIDUAL_OUT:
         RESIDUAL_OUT += row * stride_res_out_row
+    if HAS_X1:
+        X1 += row * stride_x1_row
+    if HAS_W1:
+        Y1 += row * stride_y1_row
     # Compute mean and variance
     cols = tl.arange(0, BLOCK_N)
     x = tl.load(X + cols, mask=cols < N, other=0.0).to(tl.float32)
+    if HAS_ROWSCALE:
+        rowscale = tl.load(ROWSCALE + row).to(tl.float32)
+        x *= rowscale
+    if HAS_DROPOUT:
+        # Compute dropout mask
+        # 7 rounds is good enough, and reduces register pressure
+        keep_mask = tl.rand(tl.load(SEEDS + row).to(tl.uint32), cols, n_rounds=7) > dropout_p
+        x = tl.where(keep_mask, x / (1.0 - dropout_p), 0.0)
+        if STORE_DROPOUT_MASK:
+            tl.store(DROPOUT_MASK + row * N + cols, keep_mask, mask=cols < N)
+    if HAS_X1:
+        x1 = tl.load(X1 + cols, mask=cols < N, other=0.0).to(tl.float32)
+        if HAS_ROWSCALE:
+            rowscale = tl.load(ROWSCALE + M + row).to(tl.float32)
+            x1 *= rowscale
+        if HAS_DROPOUT:
+            # Compute dropout mask
+            # 7 rounds is good enough, and reduces register pressure
+            keep_mask = (
+                tl.rand(tl.load(SEEDS + M + row).to(tl.uint32), cols, n_rounds=7) > dropout_p
+            )
+            x1 = tl.where(keep_mask, x1 / (1.0 - dropout_p), 0.0)
+            if STORE_DROPOUT_MASK:
+                tl.store(DROPOUT_MASK + (M + row) * N + cols, keep_mask, mask=cols < N)
+        x += x1
     if HAS_RESIDUAL:
         residual = tl.load(RESIDUAL + cols, mask=cols < N, other=0.0).to(tl.float32)
         x += residual
     if STORE_RESIDUAL_OUT:
         tl.store(RESIDUAL_OUT + cols, x, mask=cols < N)
     if not IS_RMS_NORM:
         mean = tl.sum(x, axis=0) / N
@@ -114,196 +240,344 @@
     w = tl.load(W + cols, mask=mask).to(tl.float32)
     if HAS_BIAS:
         b = tl.load(B + cols, mask=mask).to(tl.float32)
     x_hat = (x - mean) * rstd if not IS_RMS_NORM else x * rstd
     y = x_hat * w + b if HAS_BIAS else x_hat * w
     # Write output
     tl.store(Y + cols, y, mask=mask)
+    if HAS_W1:
+        w1 = tl.load(W1 + cols, mask=mask).to(tl.float32)
+        if HAS_B1:
+            b1 = tl.load(B1 + cols, mask=mask).to(tl.float32)
+        y1 = x_hat * w1 + b1 if HAS_B1 else x_hat * w1
+        tl.store(Y1 + cols, y1, mask=mask)
 
 
 def _layer_norm_fwd(
-    x, weight, bias, eps, residual=None, out_dtype=None, residual_dtype=None, is_rms_norm=False
+    x,
+    weight,
+    bias,
+    eps,
+    residual=None,
+    x1=None,
+    weight1=None,
+    bias1=None,
+    dropout_p=0.0,
+    rowscale=None,
+    out_dtype=None,
+    residual_dtype=None,
+    is_rms_norm=False,
+    return_dropout_mask=False,
 ):
     if residual is not None:
         residual_dtype = residual.dtype
     M, N = x.shape
     assert x.stride(-1) == 1
     if residual is not None:
         assert residual.stride(-1) == 1
         assert residual.shape == (M, N)
     assert weight.shape == (N,)
     assert weight.stride(-1) == 1
     if bias is not None:
         assert bias.stride(-1) == 1
         assert bias.shape == (N,)
+    if x1 is not None:
+        assert x1.shape == x.shape
+        assert rowscale is None
+        assert x1.stride(-1) == 1
+    if weight1 is not None:
+        assert weight1.shape == (N,)
+        assert weight1.stride(-1) == 1
+    if bias1 is not None:
+        assert bias1.shape == (N,)
+        assert bias1.stride(-1) == 1
+    if rowscale is not None:
+        assert rowscale.is_contiguous()
+        assert rowscale.shape == (M,)
     # allocate output
     y = torch.empty_like(x, dtype=x.dtype if out_dtype is None else out_dtype)
     assert y.stride(-1) == 1
-    if residual is not None or (residual_dtype is not None and residual_dtype != x.dtype):
-        residual_out = torch.empty(M, N, device=x.device, dtype=residual_dtype)
+    if weight1 is not None:
+        y1 = torch.empty_like(y)
+        assert y1.stride(-1) == 1
+    else:
+        y1 = None
+    if (
+        residual is not None
+        or (residual_dtype is not None and residual_dtype != x.dtype)
+        or dropout_p > 0.0
+        or rowscale is not None
+        or x1 is not None
+    ):
+        residual_out = torch.empty(
+            M, N, device=x.device, dtype=residual_dtype if residual_dtype is not None else x.dtype
+        )
         assert residual_out.stride(-1) == 1
     else:
         residual_out = None
     mean = torch.empty((M,), dtype=torch.float32, device=x.device) if not is_rms_norm else None
     rstd = torch.empty((M,), dtype=torch.float32, device=x.device)
+    if dropout_p > 0.0:
+        seeds = torch.randint(
+            2**32, (M if x1 is None else 2 * M,), device=x.device, dtype=torch.int64
+        )
+    else:
+        seeds = None
+    if return_dropout_mask and dropout_p > 0.0:
+        dropout_mask = torch.empty(M if x1 is None else 2 * M, N, device=x.device, dtype=torch.bool)
+    else:
+        dropout_mask = None
     # Less than 64KB per feature: enqueue fused kernel
     MAX_FUSED_SIZE = 65536 // x.element_size()
     BLOCK_N = min(MAX_FUSED_SIZE, triton.next_power_of_2(N))
     if N > BLOCK_N:
         raise RuntimeError("This layer norm doesn't support feature dim >= 64KB.")
-    # heuristics for number of warps
     with torch.cuda.device(x.device.index):
         _layer_norm_fwd_1pass_kernel[(M,)](
             x,
             y,
             weight,
             bias,
             residual,
+            x1,
+            weight1,
+            bias1,
+            y1,
             residual_out,
+            rowscale,
+            seeds,
+            dropout_mask,
             mean,
             rstd,
             x.stride(0),
             y.stride(0),
             residual.stride(0) if residual is not None else 0,
             residual_out.stride(0) if residual_out is not None else 0,
+            x1.stride(0) if x1 is not None else 0,
+            y1.stride(0) if y1 is not None else 0,
+            M,
             N,
             eps,
+            dropout_p,
             is_rms_norm,
             BLOCK_N,
             residual is not None,
             residual_out is not None,
             bias is not None,
+            dropout_p > 0.0,
+            dropout_mask is not None,
+            rowscale is not None,
         )
-    # residual_out is None if residual is None and residual_dtype == input_dtype
-    return y, mean, rstd, residual_out if residual_out is not None else x
+    # residual_out is None if residual is None and residual_dtype == input_dtype and dropout_p == 0.0
+    if dropout_mask is not None and x1 is not None:
+        dropout_mask, dropout_mask1 = dropout_mask.tensor_split(2, dim=0)
+    else:
+        dropout_mask1 = None
+    return (
+        y,
+        y1,
+        mean,
+        rstd,
+        residual_out if residual_out is not None else x,
+        seeds,
+        dropout_mask,
+        dropout_mask1,
+    )
 
 
 @triton.autotune(
     configs=[
         triton.Config({}, num_warps=1),
         triton.Config({}, num_warps=2),
         triton.Config({}, num_warps=4),
         triton.Config({}, num_warps=8),
         triton.Config({}, num_warps=16),
         triton.Config({}, num_warps=32),
     ],
-    key=["N", "HAS_DRESIDUAL", "STORE_DRESIDUAL", "IS_RMS_NORM", "HAS_BIAS"],
+    key=["N", "HAS_DRESIDUAL", "STORE_DRESIDUAL", "IS_RMS_NORM", "HAS_BIAS", "HAS_DROPOUT"],
 )
 # @triton.heuristics({"HAS_BIAS": lambda args: args["B"] is not None})
 # @triton.heuristics({"HAS_DRESIDUAL": lambda args: args["DRESIDUAL"] is not None})
 # @triton.heuristics({"STORE_DRESIDUAL": lambda args: args["DRESIDUAL_IN"] is not None})
+@triton.heuristics({"HAS_ROWSCALE": lambda args: args["ROWSCALE"] is not None})
+@triton.heuristics({"HAS_DY1": lambda args: args["DY1"] is not None})
+@triton.heuristics({"HAS_DX1": lambda args: args["DX1"] is not None})
+@triton.heuristics({"HAS_B1": lambda args: args["DB1"] is not None})
 @triton.heuristics({"RECOMPUTE_OUTPUT": lambda args: args["Y"] is not None})
 @triton.jit
 def _layer_norm_bwd_kernel(
     X,  # pointer to the input
     W,  # pointer to the weights
     B,  # pointer to the biases
     Y,  # pointer to the output to be recomputed
     DY,  # pointer to the output gradient
     DX,  # pointer to the input gradient
     DW,  # pointer to the partial sum of weights gradient
     DB,  # pointer to the partial sum of biases gradient
     DRESIDUAL,
+    W1,
+    DY1,
+    DX1,
+    DW1,
+    DB1,
     DRESIDUAL_IN,
+    ROWSCALE,
+    SEEDS,
     Mean,  # pointer to the mean
     Rstd,  # pointer to the 1/std
     stride_x_row,  # how much to increase the pointer when moving by 1 row
     stride_y_row,
     stride_dy_row,
     stride_dx_row,
     stride_dres_row,
+    stride_dy1_row,
+    stride_dx1_row,
     stride_dres_in_row,
     M,  # number of rows in X
     N,  # number of columns in X
     eps,  # epsilon to avoid division by zero
+    dropout_p,
     rows_per_program,
     IS_RMS_NORM: tl.constexpr,
     BLOCK_N: tl.constexpr,
     HAS_DRESIDUAL: tl.constexpr,
     STORE_DRESIDUAL: tl.constexpr,
     HAS_BIAS: tl.constexpr,
+    HAS_DROPOUT: tl.constexpr,
+    HAS_ROWSCALE: tl.constexpr,
+    HAS_DY1: tl.constexpr,
+    HAS_DX1: tl.constexpr,
+    HAS_B1: tl.constexpr,
     RECOMPUTE_OUTPUT: tl.constexpr,
 ):
     # Map the program id to the elements of X, DX, and DY it should compute.
     row_block_id = tl.program_id(0)
     row_start = row_block_id * rows_per_program
+    # Do not early exit if row_start >= M, because we need to write DW and DB
     cols = tl.arange(0, BLOCK_N)
     mask = cols < N
     X += row_start * stride_x_row
     if HAS_DRESIDUAL:
         DRESIDUAL += row_start * stride_dres_row
     if STORE_DRESIDUAL:
         DRESIDUAL_IN += row_start * stride_dres_in_row
     DY += row_start * stride_dy_row
     DX += row_start * stride_dx_row
+    if HAS_DY1:
+        DY1 += row_start * stride_dy1_row
+    if HAS_DX1:
+        DX1 += row_start * stride_dx1_row
     if RECOMPUTE_OUTPUT:
         Y += row_start * stride_y_row
     w = tl.load(W + cols, mask=mask).to(tl.float32)
     if RECOMPUTE_OUTPUT and HAS_BIAS:
         b = tl.load(B + cols, mask=mask, other=0.0).to(tl.float32)
+    if HAS_DY1:
+        w1 = tl.load(W1 + cols, mask=mask).to(tl.float32)
     dw = tl.zeros((BLOCK_N,), dtype=tl.float32)
     if HAS_BIAS:
         db = tl.zeros((BLOCK_N,), dtype=tl.float32)
+    if HAS_DY1:
+        dw1 = tl.zeros((BLOCK_N,), dtype=tl.float32)
+        if HAS_B1:
+            db1 = tl.zeros((BLOCK_N,), dtype=tl.float32)
     row_end = min((row_block_id + 1) * rows_per_program, M)
     for row in range(row_start, row_end):
         # Load data to SRAM
         x = tl.load(X + cols, mask=mask, other=0).to(tl.float32)
         dy = tl.load(DY + cols, mask=mask, other=0).to(tl.float32)
+        if HAS_DY1:
+            dy1 = tl.load(DY1 + cols, mask=mask, other=0).to(tl.float32)
         if not IS_RMS_NORM:
             mean = tl.load(Mean + row)
         rstd = tl.load(Rstd + row)
         # Compute dx
         xhat = (x - mean) * rstd if not IS_RMS_NORM else x * rstd
         xhat = tl.where(mask, xhat, 0.0)
         if RECOMPUTE_OUTPUT:
             y = xhat * w + b if HAS_BIAS else xhat * w
             tl.store(Y + cols, y, mask=mask)
         wdy = w * dy
         dw += dy * xhat
         if HAS_BIAS:
             db += dy
+        if HAS_DY1:
+            wdy += w1 * dy1
+            dw1 += dy1 * xhat
+            if HAS_B1:
+                db1 += dy1
         if not IS_RMS_NORM:
             c1 = tl.sum(xhat * wdy, axis=0) / N
             c2 = tl.sum(wdy, axis=0) / N
             dx = (wdy - (xhat * c1 + c2)) * rstd
         else:
             c1 = tl.sum(xhat * wdy, axis=0) / N
             dx = (wdy - xhat * c1) * rstd
         if HAS_DRESIDUAL:
             dres = tl.load(DRESIDUAL + cols, mask=mask, other=0).to(tl.float32)
             dx += dres
         # Write dx
         if STORE_DRESIDUAL:
             tl.store(DRESIDUAL_IN + cols, dx, mask=mask)
+        if HAS_DX1:
+            if HAS_DROPOUT:
+                keep_mask = (
+                    tl.rand(tl.load(SEEDS + M + row).to(tl.uint32), cols, n_rounds=7) > dropout_p
+                )
+                dx1 = tl.where(keep_mask, dx / (1.0 - dropout_p), 0.0)
+            else:
+                dx1 = dx
+            tl.store(DX1 + cols, dx1, mask=mask)
+        if HAS_DROPOUT:
+            keep_mask = tl.rand(tl.load(SEEDS + row).to(tl.uint32), cols, n_rounds=7) > dropout_p
+            dx = tl.where(keep_mask, dx / (1.0 - dropout_p), 0.0)
+        if HAS_ROWSCALE:
+            rowscale = tl.load(ROWSCALE + row).to(tl.float32)
+            dx *= rowscale
         tl.store(DX + cols, dx, mask=mask)
 
         X += stride_x_row
         if HAS_DRESIDUAL:
             DRESIDUAL += stride_dres_row
         if STORE_DRESIDUAL:
             DRESIDUAL_IN += stride_dres_in_row
         if RECOMPUTE_OUTPUT:
             Y += stride_y_row
         DY += stride_dy_row
         DX += stride_dx_row
+        if HAS_DY1:
+            DY1 += stride_dy1_row
+        if HAS_DX1:
+            DX1 += stride_dx1_row
     tl.store(DW + row_block_id * N + cols, dw, mask=mask)
     if HAS_BIAS:
         tl.store(DB + row_block_id * N + cols, db, mask=mask)
+    if HAS_DY1:
+        tl.store(DW1 + row_block_id * N + cols, dw1, mask=mask)
+        if HAS_B1:
+            tl.store(DB1 + row_block_id * N + cols, db1, mask=mask)
 
 
 def _layer_norm_bwd(
     dy,
     x,
     weight,
     bias,
     eps,
     mean,
     rstd,
     dresidual=None,
+    dy1=None,
+    weight1=None,
+    bias1=None,
+    seeds=None,
+    dropout_p=0.0,
+    rowscale=None,
     has_residual=False,
+    has_x1=False,
     is_rms_norm=False,
     x_dtype=None,
     recompute_output=False,
 ):
     M, N = x.shape
     assert x.stride(-1) == 1
     assert dy.stride(-1) == 1
@@ -312,195 +586,372 @@
         assert dresidual.stride(-1) == 1
         assert dresidual.shape == (M, N)
     assert weight.shape == (N,)
     assert weight.stride(-1) == 1
     if bias is not None:
         assert bias.stride(-1) == 1
         assert bias.shape == (N,)
+    if dy1 is not None:
+        assert weight1 is not None
+        assert dy1.shape == dy.shape
+        assert dy1.stride(-1) == 1
+    if weight1 is not None:
+        assert weight1.shape == (N,)
+        assert weight1.stride(-1) == 1
+    if bias1 is not None:
+        assert bias1.shape == (N,)
+        assert bias1.stride(-1) == 1
+    if seeds is not None:
+        assert seeds.is_contiguous()
+        assert seeds.shape == (M if not has_x1 else M * 2,)
+    if rowscale is not None:
+        assert rowscale.is_contiguous()
+        assert rowscale.shape == (M,)
     # allocate output
     dx = (
         torch.empty_like(x)
         if x_dtype is None
         else torch.empty(M, N, dtype=x_dtype, device=x.device)
     )
-    dresidual_in = torch.empty_like(x) if has_residual and dx.dtype != x.dtype else None
+    dresidual_in = (
+        torch.empty_like(x)
+        if has_residual
+        and (dx.dtype != x.dtype or dropout_p > 0.0 or rowscale is not None or has_x1)
+        else None
+    )
+    dx1 = torch.empty_like(dx) if (has_x1 and dropout_p > 0.0) else None
     y = torch.empty(M, N, dtype=dy.dtype, device=dy.device) if recompute_output else None
+    if recompute_output:
+        assert weight1 is None, "recompute_output is not supported with parallel LayerNorm"
 
     # Less than 64KB per feature: enqueue fused kernel
     MAX_FUSED_SIZE = 65536 // x.element_size()
     BLOCK_N = min(MAX_FUSED_SIZE, triton.next_power_of_2(N))
     if N > BLOCK_N:
         raise RuntimeError("This layer norm doesn't support feature dim >= 64KB.")
     sm_count = torch.cuda.get_device_properties(x.device).multi_processor_count
     _dw = torch.empty((sm_count, N), dtype=torch.float32, device=weight.device)
     _db = (
         torch.empty((sm_count, N), dtype=torch.float32, device=bias.device)
         if bias is not None
         else None
     )
+    _dw1 = torch.empty_like(_dw) if weight1 is not None else None
+    _db1 = torch.empty_like(_db) if bias1 is not None else None
     rows_per_program = math.ceil(M / sm_count)
     grid = (sm_count,)
     with torch.cuda.device(x.device.index):
         _layer_norm_bwd_kernel[grid](
             x,
             weight,
             bias,
             y,
             dy,
             dx,
             _dw,
             _db,
             dresidual,
+            weight1,
+            dy1,
+            dx1,
+            _dw1,
+            _db1,
             dresidual_in,
+            rowscale,
+            seeds,
             mean,
             rstd,
             x.stride(0),
             0 if not recompute_output else y.stride(0),
             dy.stride(0),
             dx.stride(0),
             dresidual.stride(0) if dresidual is not None else 0,
+            dy1.stride(0) if dy1 is not None else 0,
+            dx1.stride(0) if dx1 is not None else 0,
             dresidual_in.stride(0) if dresidual_in is not None else 0,
             M,
             N,
             eps,
+            dropout_p,
             rows_per_program,
             is_rms_norm,
             BLOCK_N,
             dresidual is not None,
             dresidual_in is not None,
             bias is not None,
+            dropout_p > 0.0,
         )
     dw = _dw.sum(0).to(weight.dtype)
     db = _db.sum(0).to(bias.dtype) if bias is not None else None
+    dw1 = _dw1.sum(0).to(weight1.dtype) if weight1 is not None else None
+    db1 = _db1.sum(0).to(bias1.dtype) if bias1 is not None else None
     # Don't need to compute dresidual_in separately in this case
-    if has_residual and dx.dtype == x.dtype:
+    if has_residual and dx.dtype == x.dtype and dropout_p == 0.0 and rowscale is None:
         dresidual_in = dx
-    return (dx, dw, db, dresidual_in) if not recompute_output else (dx, dw, db, dresidual_in, y)
+    if has_x1 and dropout_p == 0.0:
+        dx1 = dx
+    return (
+        (dx, dw, db, dresidual_in, dx1, dw1, db1)
+        if not recompute_output
+        else (dx, dw, db, dresidual_in, dx1, dw1, db1, y)
+    )
 
 
 class LayerNormFn(torch.autograd.Function):
     @staticmethod
     def forward(
         ctx,
         x,
         weight,
         bias,
         residual=None,
+        x1=None,
+        weight1=None,
+        bias1=None,
         eps=1e-6,
+        dropout_p=0.0,
+        rowscale=None,
         prenorm=False,
         residual_in_fp32=False,
         is_rms_norm=False,
+        return_dropout_mask=False,
     ):
         x_shape_og = x.shape
         # reshape input data into 2D tensor
         x = x.reshape(-1, x.shape[-1])
         if x.stride(-1) != 1:
             x = x.contiguous()
         if residual is not None:
             assert residual.shape == x_shape_og
             residual = residual.reshape(-1, residual.shape[-1])
             if residual.stride(-1) != 1:
                 residual = residual.contiguous()
+        if x1 is not None:
+            assert x1.shape == x_shape_og
+            assert rowscale is None, "rowscale is not supported with parallel LayerNorm"
+            x1 = x1.reshape(-1, x1.shape[-1])
+            if x1.stride(-1) != 1:
+                x1 = x1.contiguous()
         weight = weight.contiguous()
         if bias is not None:
             bias = bias.contiguous()
+        if weight1 is not None:
+            weight1 = weight1.contiguous()
+        if bias1 is not None:
+            bias1 = bias1.contiguous()
+        if rowscale is not None:
+            rowscale = rowscale.reshape(-1).contiguous()
         residual_dtype = (
             residual.dtype
             if residual is not None
             else (torch.float32 if residual_in_fp32 else None)
         )
-        y, mean, rstd, residual_out = _layer_norm_fwd(
-            x, weight, bias, eps, residual, residual_dtype=residual_dtype, is_rms_norm=is_rms_norm
+        y, y1, mean, rstd, residual_out, seeds, dropout_mask, dropout_mask1 = _layer_norm_fwd(
+            x,
+            weight,
+            bias,
+            eps,
+            residual,
+            x1,
+            weight1,
+            bias1,
+            dropout_p=dropout_p,
+            rowscale=rowscale,
+            residual_dtype=residual_dtype,
+            is_rms_norm=is_rms_norm,
+            return_dropout_mask=return_dropout_mask,
+        )
+        ctx.save_for_backward(
+            residual_out, weight, bias, weight1, bias1, rowscale, seeds, mean, rstd
         )
-        ctx.save_for_backward(residual_out, weight, bias, mean, rstd)
         ctx.x_shape_og = x_shape_og
         ctx.eps = eps
+        ctx.dropout_p = dropout_p
         ctx.is_rms_norm = is_rms_norm
         ctx.has_residual = residual is not None
+        ctx.has_x1 = x1 is not None
         ctx.prenorm = prenorm
         ctx.x_dtype = x.dtype
         y = y.reshape(x_shape_og)
-        return y if not prenorm else (y, residual_out.reshape(x_shape_og))
+        y1 = y1.reshape(x_shape_og) if y1 is not None else None
+        residual_out = residual_out.reshape(x_shape_og) if residual_out is not None else None
+        dropout_mask = dropout_mask.reshape(x_shape_og) if dropout_mask is not None else None
+        dropout_mask1 = dropout_mask1.reshape(x_shape_og) if dropout_mask1 is not None else None
+        if not return_dropout_mask:
+            if weight1 is None:
+                return y if not prenorm else (y, residual_out)
+            else:
+                return (y, y1) if not prenorm else (y, y1, residual_out)
+        else:
+            if weight1 is None:
+                return (
+                    (y, dropout_mask, dropout_mask1)
+                    if not prenorm
+                    else (y, residual_out, dropout_mask, dropout_mask1)
+                )
+            else:
+                return (
+                    (y, y1, dropout_mask, dropout_mask1)
+                    if not prenorm
+                    else (y, y1, residual_out, dropout_mask, dropout_mask1)
+                )
 
     @staticmethod
     def backward(ctx, dy, *args):
-        x, weight, bias, mean, rstd = ctx.saved_tensors
+        x, weight, bias, weight1, bias1, rowscale, seeds, mean, rstd = ctx.saved_tensors
         dy = dy.reshape(-1, dy.shape[-1])
         if dy.stride(-1) != 1:
             dy = dy.contiguous()
         assert dy.shape == x.shape
+        if weight1 is not None:
+            dy1, args = args[0], args[1:]
+            dy1 = dy1.reshape(-1, dy1.shape[-1])
+            if dy1.stride(-1) != 1:
+                dy1 = dy1.contiguous()
+            assert dy1.shape == x.shape
+        else:
+            dy1 = None
         if ctx.prenorm:
             dresidual = args[0]
             dresidual = dresidual.reshape(-1, dresidual.shape[-1])
             if dresidual.stride(-1) != 1:
                 dresidual = dresidual.contiguous()
             assert dresidual.shape == x.shape
         else:
             dresidual = None
-        dx, dw, db, dresidual_in = _layer_norm_bwd(
+        dx, dw, db, dresidual_in, dx1, dw1, db1 = _layer_norm_bwd(
             dy,
             x,
             weight,
             bias,
             ctx.eps,
             mean,
             rstd,
             dresidual,
+            dy1,
+            weight1,
+            bias1,
+            seeds,
+            ctx.dropout_p,
+            rowscale,
             ctx.has_residual,
+            ctx.has_x1,
             ctx.is_rms_norm,
             x_dtype=ctx.x_dtype,
         )
         return (
             dx.reshape(ctx.x_shape_og),
             dw,
             db,
             dresidual_in.reshape(ctx.x_shape_og) if ctx.has_residual else None,
+            dx1.reshape(ctx.x_shape_og) if dx1 is not None else None,
+            dw1,
+            db1,
+            None,
+            None,
+            None,
             None,
             None,
             None,
             None,
         )
 
 
 def layer_norm_fn(
     x,
     weight,
     bias,
     residual=None,
+    x1=None,
+    weight1=None,
+    bias1=None,
     eps=1e-6,
+    dropout_p=0.0,
+    rowscale=None,
     prenorm=False,
     residual_in_fp32=False,
     is_rms_norm=False,
+    return_dropout_mask=False,
 ):
-    return LayerNormFn.apply(x, weight, bias, residual, eps, prenorm, residual_in_fp32, is_rms_norm)
+    return LayerNormFn.apply(
+        x,
+        weight,
+        bias,
+        residual,
+        x1,
+        weight1,
+        bias1,
+        eps,
+        dropout_p,
+        rowscale,
+        prenorm,
+        residual_in_fp32,
+        is_rms_norm,
+        return_dropout_mask,
+    )
 
 
-def rms_norm_fn(x, weight, bias, residual=None, prenorm=False, residual_in_fp32=False, eps=1e-6):
-    return LayerNormFn.apply(x, weight, bias, residual, eps, prenorm, residual_in_fp32, True)
+def rms_norm_fn(
+    x,
+    weight,
+    bias,
+    residual=None,
+    x1=None,
+    weight1=None,
+    bias1=None,
+    eps=1e-6,
+    dropout_p=0.0,
+    rowscale=None,
+    prenorm=False,
+    residual_in_fp32=False,
+    return_dropout_mask=False,
+):
+    return LayerNormFn.apply(
+        x,
+        weight,
+        bias,
+        residual,
+        x1,
+        weight1,
+        bias1,
+        eps,
+        dropout_p,
+        rowscale,
+        prenorm,
+        residual_in_fp32,
+        True,
+        return_dropout_mask,
+    )
 
 
 class RMSNorm(torch.nn.Module):
-    def __init__(self, hidden_size, eps=1e-5, device=None, dtype=None):
+
+    def __init__(self, hidden_size, eps=1e-5, dropout_p=0.0, device=None, dtype=None):
         factory_kwargs = {"device": device, "dtype": dtype}
         super().__init__()
         self.eps = eps
+        if dropout_p > 0.0:
+            self.drop = torch.nn.Dropout(dropout_p)
+        else:
+            self.drop = None
         self.weight = torch.nn.Parameter(torch.empty(hidden_size, **factory_kwargs))
         self.register_parameter("bias", None)
         self.reset_parameters()
 
     def reset_parameters(self):
         torch.nn.init.ones_(self.weight)
 
     def forward(self, x, residual=None, prenorm=False, residual_in_fp32=False):
         return rms_norm_fn(
             x,
             self.weight,
             self.bias,
             residual=residual,
             eps=self.eps,
+            dropout_p=self.drop.p if self.drop is not None and self.training else 0.0,
             prenorm=prenorm,
             residual_in_fp32=residual_in_fp32,
         )
 
 
 class LayerNormLinearFn(torch.autograd.Function):
     @staticmethod
@@ -532,15 +983,15 @@
         if norm_bias is not None:
             norm_bias = norm_bias.contiguous()
         residual_dtype = (
             residual.dtype
             if residual is not None
             else (torch.float32 if residual_in_fp32 else None)
         )
-        y, mean, rstd, residual_out = _layer_norm_fwd(
+        y, _, mean, rstd, residual_out, *rest = _layer_norm_fwd(
             x,
             norm_weight,
             norm_bias,
             eps,
             residual,
             out_dtype=None if not torch.is_autocast_enabled() else torch.get_autocast_gpu_dtype(),
             residual_dtype=residual_dtype,
@@ -576,25 +1027,25 @@
             dresidual = args[0]
             dresidual = dresidual.reshape(-1, dresidual.shape[-1])
             if dresidual.stride(-1) != 1:
                 dresidual = dresidual.contiguous()
             assert dresidual.shape == x.shape
         else:
             dresidual = None
-        dx, dnorm_weight, dnorm_bias, dresidual_in, y = _layer_norm_bwd(
+        dx, dnorm_weight, dnorm_bias, dresidual_in, _, _, _, y = _layer_norm_bwd(
             dy,
             x,
             norm_weight,
             norm_bias,
             ctx.eps,
             mean,
             rstd,
-            dresidual,
-            ctx.has_residual,
-            ctx.is_rms_norm,
+            dresidual=dresidual,
+            has_residual=ctx.has_residual,
+            is_rms_norm=ctx.is_rms_norm,
             x_dtype=ctx.x_dtype,
             recompute_output=True,
         )
         dlinear_weight = torch.einsum("bo,bi->oi", dout, y)
         return (
             dx.reshape(ctx.x_shape_og),
             dnorm_weight,
```

### Comparing `mamba_ssm-1.2.2/mamba_ssm/ops/triton/selective_state_update.py` & `mamba_ssm-2.0.0/mamba_ssm/ops/triton/selective_state_update.py`

 * *Files identical despite different names*

### Comparing `mamba_ssm-1.2.2/mamba_ssm/utils/generation.py` & `mamba_ssm-2.0.0/mamba_ssm/utils/generation.py`

 * *Files identical despite different names*

### Comparing `mamba_ssm-1.2.2/mamba_ssm/utils/hf.py` & `mamba_ssm-2.0.0/mamba_ssm/utils/hf.py`

 * *Files identical despite different names*

### Comparing `mamba_ssm-1.2.2/mamba_ssm.egg-info/PKG-INFO` & `mamba_ssm-2.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: mamba-ssm
-Version: 1.2.2
+Name: mamba_ssm
+Version: 2.0.0
 Summary: Mamba state-space model
 Home-page: https://github.com/state-spaces/mamba
 Author: Tri Dao, Albert Gu
 Author-email: tri@tridao.me, agu@cs.cmu.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: Unix
@@ -15,14 +15,17 @@
 
 # Mamba
 
 ![Mamba](assets/selection.png "Selective State Space")
 > **Mamba: Linear-Time Sequence Modeling with Selective State Spaces**\
 > Albert Gu*, Tri Dao*\
 > Paper: https://arxiv.org/abs/2312.00752
+> **Transformers are {SSM}s: Generalized Models and Efficient Algorithms Through Structured State Space Duality**\
+> Tri Dao*, Albert Gu*\
+> Paper: https://arxiv.org/abs/2405.21060
 
 ## About
 
 Mamba is a new state space model architecture showing promising performance on information-dense data such as language modeling, where previous subquadratic models fall short of Transformers.
 It is based on the line of progress on [structured state space models](https://github.com/state-spaces/s4),
 with an efficient hardware-aware design and implementation in the spirit of [FlashAttention](https://github.com/Dao-AILab/flash-attention).
 
@@ -54,15 +57,15 @@
 ### Mamba Block
 
 The main module of this repository is the Mamba architecture block wrapping the selective SSM.
 
 Source: [modules/mamba_simple.py](mamba_ssm/modules/mamba_simple.py).
 
 Usage:
-```
+``` python
 import torch
 from mamba_ssm import Mamba
 
 batch, length, dim = 2, 64, 16
 x = torch.randn(batch, length, dim).to("cuda")
 model = Mamba(
     # This module uses roughly 3 * expand * d_model^2 parameters
@@ -71,30 +74,48 @@
     d_conv=4,    # Local convolution width
     expand=2,    # Block expansion factor
 ).to("cuda")
 y = model(x)
 assert y.shape == x.shape
 ```
 
+The Mamba-2 block is implemented at [modules/mamba2.py](mamba_ssm/modules/mamba2.py).
+
+A simpler version is at [modules/mamba2_simple.py](mamba_ssm/modules/mamba2_simple.py)
+
+The usage is similar to Mamba(-1):
+``` python
+from mamba_ssm import Mamba2
+model = Mamba(
+    # This module uses roughly 3 * expand * d_model^2 parameters
+    d_model=dim, # Model dimension d_model
+    d_state=64,  # SSM state expansion factor, typically 64 or 128
+    d_conv=4,    # Local convolution width
+    expand=2,    # Block expansion factor
+).to("cuda")
+y = model(x)
+assert y.shape == x.shape
+```
+
 ### Mamba Language Model
 
 Finally, we provide an example of a complete language model: a deep sequence model backbone (with repeating Mamba blocks) + language model head.
 
 Source: [models/mixer_seq_simple.py](mamba_ssm/models/mixer_seq_simple.py).
 
 This is an example of how to integrate Mamba into an end-to-end neural network.
 This example is used in the generation scripts below.
 
 
-
 ## Pretrained Models
 
 Pretrained models are uploaded to
 [Hugging Face](https://huggingface.co/state-spaces): `mamba-130m`, `mamba-370m`,
-`mamba-790m`, `mamba-1.4b`, `mamba-2.8b`, trained on 300B tokens on the Pile, as well as `mamba-2.8b-slimpj`
+`mamba-790m`, `mamba-1.4b`, `mamba-2.8b`, `mamba2-130m`, `mamba2-370m`,
+`mamba2-780m`, `mamba2-1.3b`, `mamba2-2.7b`, `transformerpp-2.7b`, `mamba2attn-2.7b`, trained on 300B tokens on the Pile, as well as `mamba-2.8b-slimpj`
 (trained on 600B tokens on the SlimPajama dataset).
 
 
 The models will be autodownloaded by the generation script below.
 
 These models were trained on the [Pile](https://huggingface.co/datasets/EleutherAI/pile), and follow the standard model dimensions described by GPT-3 and followed by many open source models:
 
@@ -112,31 +133,35 @@
 Performance is expected to be comparable or better than other architectures trained on similar data, but not to match larger or fine-tuned models.
 
 
 ## Evaluations
 
 To run zero-shot evaluations of models (corresponding to Table 3 of the paper),
 we use the
-[lm-evaluation-harness](https://github.com/EleutherAI/lm-evaluation-harness/tree/big-refactor)
+[lm-evaluation-harness](https://github.com/EleutherAI/lm-evaluation-harness)
 library.
 
-1. Pull the `lm-evaluation-harness` repo by `git submodule update --init
-   --recursive`. We use the `big-refactor` branch.
-2. Install `lm-evaluation-harness`: `pip install -e 3rdparty/lm-evaluation-harness`.
-On Python 3.10 you might need to manually install the latest version of `promptsource`: `pip install git+https://github.com/bigscience-workshop/promptsource.git`.
-3. Run evaluation with (more documentation at the [lm-evaluation-harness](https://github.com/EleutherAI/lm-evaluation-harness/tree/big-refactor) repo):
-```
-python evals/lm_harness_eval.py --model mamba --model_args pretrained=state-spaces/mamba-130m --tasks lambada_openai,hellaswag,piqa,arc_easy,arc_challenge,winogrande --device cuda --batch_size 64
+1. Install `lm-evaluation-harness` by `pip install lm-eval==0.4.2`.
+2. Run evaluation with (more documentation at the [lm-evaluation-harness](https://github.com/EleutherAI/lm-evaluation-harness/tree/big-refactor) repo):
+``` sh
+lm_eval --model mamba_ssm --model_args pretrained=state-spaces/mamba-130m --tasks lambada_openai,hellaswag,piqa,arc_easy,arc_challenge,winogrande,openbookqa --device cuda --batch_size 256
 python evals/lm_harness_eval.py --model hf --model_args pretrained=EleutherAI/pythia-160m --tasks lambada_openai,hellaswag,piqa,arc_easy,arc_challenge,winogrande --device cuda --batch_size 64
 ```
 
 To reproduce the results on the `mamba-2.8b-slimpj` model reported in the blogposts:
+``` sh
+lm_eval --model mamba_ssm --model_args pretrained=state-spaces/mamba-2.8b-slimpj --tasks boolq,piqa,hellaswag,winogrande,arc_easy,arc_challenge,openbookqa,race,truthfulqa_mc2 --device cuda --batch_size 256
+lm_eval --model mamba_ssm --model_args pretrained=state-spaces/mamba-2.8b-slimpj --tasks mmlu --num_fewshot 5 --device cuda --batch_size 256
 ```
-python evals/lm_harness_eval.py --model mamba --model_args pretrained=state-spaces/mamba-2.8b-slimpj --tasks boolq,piqa,hellaswag,winogrande,arc_easy,arc_challenge,openbookqa,race,truthfulqa_mc2 --device cuda --batch_size 64
-python evals/lm_harness_eval.py --model mamba --model_args pretrained=state-spaces/mamba-2.8b-slimpj --tasks mmlu --num_fewshot 5 --device cuda --batch_size 64
+
+To run evaluations on Mamba-2 models, simply replace the model names:
+``` sh
+lm_eval --model mamba_ssm --model_args pretrained=state-spaces/mamba2-2.7b --tasks lambada_openai,hellaswag,piqa,arc_easy,arc_challenge,winogrande,openbookqa --device cuda --batch_size 256
+lm_eval --model mamba_ssm --model_args pretrained=state-spaces/transformerpp-2.7b --tasks lambada_openai,hellaswag,piqa,arc_easy,arc_challenge,winogrande,openbookqa --device cuda --batch_size 256
+lm_eval --model mamba_ssm --model_args pretrained=state-spaces/mamba2attn-2.7b --tasks lambada_openai,hellaswag,piqa,arc_easy,arc_challenge,winogrande,openbookqa --device cuda --batch_size 256
 ```
 
 Note that the result of each task might differ from reported values by 0.1-0.3 due to noise in the evaluation process.
 
 ## Inference
 
 The script [benchmarks/benchmark_generation_mamba_simple.py](benchmarks/benchmark_generation_mamba_simple.py)
@@ -146,24 +171,29 @@
 
 Other configurable options include the top-p (nucleus sampling) probability, and the softmax temperature.
 
 ### Examples
 
 To test generation latency (e.g. batch size = 1) with different sampling strategies:
 
-```
+``` sh
 python benchmarks/benchmark_generation_mamba_simple.py --model-name "state-spaces/mamba-2.8b" --prompt "My cat wrote all this CUDA code for a new language model and" --topp 0.9 --temperature 0.7 --repetition-penalty 1.2
 python benchmarks/benchmark_generation_mamba_simple.py --model-name "EleutherAI/pythia-2.8b" --prompt "My cat wrote all this CUDA code for a new language model and" --topp 0.9 --temperature 0.7 --repetition-penalty 1.2
 python benchmarks/benchmark_generation_mamba_simple.py --model-name "state-spaces/mamba-2.8b" --prompt "My cat wrote all this CUDA code for a new language model and" --minp 0.05 --topk 0 --temperature 0.7 --repetition-penalty 1.2
 ```
 
 To test generation throughput with random prompts (e.g. large batch size):
+``` sh
+python benchmarks/benchmark_generation_mamba_simple.py --model-name "state-spaces/mamba-2.8b" --batch 64
+python benchmarks/benchmark_generation_mamba_simple.py --model-name "EleutherAI/pythia-2.8b" --batch 64
 ```
-python benchmarks/benchmark_generation_mamba_simple.py --model-name "state-spaces/mamba-2.8b" --batch 128
-python benchmarks/benchmark_generation_mamba_simple.py --model-name "EleutherAI/pythia-2.8b" --batch 128
+
+With Mamba-2, you just need to change the model name:
+``` sh
+python benchmarks/benchmark_generation_mamba_simple.py --model-name "state-spaces/mamba2-2.7b" --prompt "My cat wrote all this CUDA code for a new language model and" --topp 0.9 --temperature 0.7 --repetition-penalty 1.2
 ```
 
 
 ## Troubleshooting
 
 ### Precision
 Our models were trained using PyTorch [AMP](https://pytorch.org/docs/stable/amp.html) for mixed precision. AMP keeps model parameters in float32 and casts to half precision when necessary.
@@ -178,16 +208,23 @@
 However, some frameworks may have post-initialization hooks (e.g. setting all bias terms in `nn.Linear` modules to zero).
 If this is the case, you may have to add custom logic (e.g. this [line](https://github.com/state-spaces/mamba/blob/f0affcf69f06d1d06cef018ff640bf080a11c421/mamba_ssm/modules/mamba_simple.py#L104) turns off re-initializing in our trainer, but would be a no-op in any other framework)
 that is specific to the training framework.
 
 
 ## Citation
 
-If you use this codebase, or otherwise found our work valuable, please cite Mamba:
+If you use this codebase, or otherwise find our work valuable, please cite Mamba:
 ```
 @article{mamba,
   title={Mamba: Linear-Time Sequence Modeling with Selective State Spaces},
   author={Gu, Albert and Dao, Tri},
   journal={arXiv preprint arXiv:2312.00752},
   year={2023}
 }
+@inproceedings{mamba2,
+  title={Transformers are {SSM}s: Generalized Models and Efficient Algorithms Through Structured State Space Duality},
+  author={Dao, Tri and Gu, Albert},
+  booktitle={International Conference on Machine Learning (ICML)},
+  year={2024}
+}
+
 ```
```

### Comparing `mamba_ssm-1.2.2/setup.py` & `mamba_ssm-2.0.0/setup.py`

 * *Files identical despite different names*

