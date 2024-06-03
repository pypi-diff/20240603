# Comparing `tmp/onediffx-1.1.0.dev202406010129.tar.gz` & `tmp/onediffx-1.1.0.dev202406020129.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onediffx-1.1.0.dev202406010129.tar", last modified: Sat Jun  1 01:30:22 2024, max compression
+gzip compressed data, was "onediffx-1.1.0.dev202406020129.tar", last modified: Sun Jun  2 01:30:30 2024, max compression
```

## Comparing `onediffx-1.1.0.dev202406010129.tar` & `onediffx-1.1.0.dev202406020129.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:30:22.964748 onediffx-1.1.0.dev202406010129/
--rw-r--r--   0 runner    (1001) docker     (127)    22324 2024-06-01 01:30:22.964748 onediffx-1.1.0.dev202406010129/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21267 2024-06-01 01:29:57.000000 onediffx-1.1.0.dev202406010129/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:30:22.956748 onediffx-1.1.0.dev202406010129/onediffx/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-06-01 01:29:57.000000 onediffx-1.1.0.dev202406010129/onediffx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:30:22.960748 onediffx-1.1.0.dev202406010129/onediffx/compilers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 01:29:57.000000 onediffx-1.1.0.dev202406010129/onediffx/compilers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-06-01 01:29:57.000000 onediffx-1.1.0.dev202406010129/onediffx/compilers/diffusion_pipeline_compiler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:30:22.960748 onediffx-1.1.0.dev202406010129/onediffx/deep_cache/
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-06-01 01:29:57.000000 onediffx-1.1.0.dev202406010129/onediffx/deep_cache/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:30:22.960748 onediffx-1.1.0.dev202406010129/onediffx/deep_cache/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 01:29:57.000000 onediffx-1.1.0.dev202406010129/onediffx/deep_cache/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24987 2024-06-01 01:29:57.000000 onediffx-1.1.0.dev202406010129/onediffx/deep_cache/models/fast_unet_2d_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)     8709 2024-06-01 01:29:57.000000 onediffx-1.1.0.dev202406010129/onediffx/deep_cache/models/fast_unet_spatio_temporal_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)     7907 2024-06-01 01:29:57.000000 onediffx-1.1.0.dev202406010129/onediffx/deep_cache/models/pipeline_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    25684 2024-06-01 01:29:57.000000 onediffx-1.1.0.dev202406010129/onediffx/deep_cache/models/unet_2d_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)    25800 2024-06-01 01:29:57.000000 onediffx-1.1.0.dev202406010129/onediffx/deep_cache/models/unet_2d_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)    11282 2024-06-01 01:29:57.000000 onediffx-1.1.0.dev202406010129/onediffx/deep_cache/models/unet_3d_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     8815 2024-06-01 01:29:57.000000 onediffx-1.1.0.dev202406010129/onediffx/deep_cache/models/unet_spatio_temporal_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)    79951 2024-06-01 01:29:57.000000 onediffx-1.1.0.dev202406010129/onediffx/deep_cache/pipeline_stable_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (127)    91202 2024-06-01 01:29:57.000000 onediffx-1.1.0.dev202406010129/onediffx/deep_cache/pipeline_stable_diffusion_xl.py
--rw-r--r--   0 runner    (1001) docker     (127)    14349 2024-06-01 01:29:57.000000 onediffx-1.1.0.dev202406010129/onediffx/deep_cache/pipeline_stable_video_diffusion.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:30:22.960748 onediffx-1.1.0.dev202406010129/onediffx/lora/
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-06-01 01:29:57.000000 onediffx-1.1.0.dev202406010129/onediffx/lora/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8378 2024-06-01 01:29:57.000000 onediffx-1.1.0.dev202406010129/onediffx/lora/lora.py
--rw-r--r--   0 runner    (1001) docker     (127)     9141 2024-06-01 01:29:57.000000 onediffx-1.1.0.dev202406010129/onediffx/lora/state_dict_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15093 2024-06-01 01:29:57.000000 onediffx-1.1.0.dev202406010129/onediffx/lora/text_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    11087 2024-06-01 01:29:57.000000 onediffx-1.1.0.dev202406010129/onediffx/lora/unet.py
--rw-r--r--   0 runner    (1001) docker     (127)    13907 2024-06-01 01:29:57.000000 onediffx-1.1.0.dev202406010129/onediffx/lora/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:30:22.960748 onediffx-1.1.0.dev202406010129/onediffx/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 01:29:57.000000 onediffx-1.1.0.dev202406010129/onediffx/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-06-01 01:29:57.000000 onediffx-1.1.0.dev202406010129/onediffx/utils/patch_image_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:30:22.964748 onediffx-1.1.0.dev202406010129/onediffx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22324 2024-06-01 01:30:22.000000 onediffx-1.1.0.dev202406010129/onediffx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-06-01 01:30:22.000000 onediffx-1.1.0.dev202406010129/onediffx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 01:30:22.000000 onediffx-1.1.0.dev202406010129/onediffx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-06-01 01:30:22.000000 onediffx-1.1.0.dev202406010129/onediffx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-06-01 01:30:22.000000 onediffx-1.1.0.dev202406010129/onediffx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 01:30:22.964748 onediffx-1.1.0.dev202406010129/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-06-01 01:29:57.000000 onediffx-1.1.0.dev202406010129/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:30:22.960748 onediffx-1.1.0.dev202406010129/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5730 2024-06-01 01:29:57.000000 onediffx-1.1.0.dev202406010129/tests/test_lora.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 01:30:30.913993 onediffx-1.1.0.dev202406020129/
+-rw-r--r--   0 runner    (1001) docker     (127)    22386 2024-06-02 01:30:30.913993 onediffx-1.1.0.dev202406020129/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21329 2024-06-02 01:29:58.000000 onediffx-1.1.0.dev202406020129/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 01:30:30.909993 onediffx-1.1.0.dev202406020129/onediffx/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-06-02 01:29:58.000000 onediffx-1.1.0.dev202406020129/onediffx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 01:30:30.909993 onediffx-1.1.0.dev202406020129/onediffx/compilers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 01:29:58.000000 onediffx-1.1.0.dev202406020129/onediffx/compilers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-06-02 01:29:58.000000 onediffx-1.1.0.dev202406020129/onediffx/compilers/diffusion_pipeline_compiler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 01:30:30.909993 onediffx-1.1.0.dev202406020129/onediffx/deep_cache/
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-06-02 01:29:58.000000 onediffx-1.1.0.dev202406020129/onediffx/deep_cache/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 01:30:30.913993 onediffx-1.1.0.dev202406020129/onediffx/deep_cache/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 01:29:58.000000 onediffx-1.1.0.dev202406020129/onediffx/deep_cache/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24987 2024-06-02 01:29:58.000000 onediffx-1.1.0.dev202406020129/onediffx/deep_cache/models/fast_unet_2d_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8709 2024-06-02 01:29:58.000000 onediffx-1.1.0.dev202406020129/onediffx/deep_cache/models/fast_unet_spatio_temporal_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7907 2024-06-02 01:29:58.000000 onediffx-1.1.0.dev202406020129/onediffx/deep_cache/models/pipeline_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25684 2024-06-02 01:29:58.000000 onediffx-1.1.0.dev202406020129/onediffx/deep_cache/models/unet_2d_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25800 2024-06-02 01:29:58.000000 onediffx-1.1.0.dev202406020129/onediffx/deep_cache/models/unet_2d_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11282 2024-06-02 01:29:58.000000 onediffx-1.1.0.dev202406020129/onediffx/deep_cache/models/unet_3d_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8815 2024-06-02 01:29:58.000000 onediffx-1.1.0.dev202406020129/onediffx/deep_cache/models/unet_spatio_temporal_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79951 2024-06-02 01:29:58.000000 onediffx-1.1.0.dev202406020129/onediffx/deep_cache/pipeline_stable_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91202 2024-06-02 01:29:58.000000 onediffx-1.1.0.dev202406020129/onediffx/deep_cache/pipeline_stable_diffusion_xl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14349 2024-06-02 01:29:58.000000 onediffx-1.1.0.dev202406020129/onediffx/deep_cache/pipeline_stable_video_diffusion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 01:30:30.913993 onediffx-1.1.0.dev202406020129/onediffx/lora/
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-06-02 01:29:58.000000 onediffx-1.1.0.dev202406020129/onediffx/lora/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8378 2024-06-02 01:29:58.000000 onediffx-1.1.0.dev202406020129/onediffx/lora/lora.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9141 2024-06-02 01:29:58.000000 onediffx-1.1.0.dev202406020129/onediffx/lora/state_dict_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15093 2024-06-02 01:29:58.000000 onediffx-1.1.0.dev202406020129/onediffx/lora/text_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11087 2024-06-02 01:29:58.000000 onediffx-1.1.0.dev202406020129/onediffx/lora/unet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13993 2024-06-02 01:29:58.000000 onediffx-1.1.0.dev202406020129/onediffx/lora/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 01:30:30.913993 onediffx-1.1.0.dev202406020129/onediffx/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 01:29:58.000000 onediffx-1.1.0.dev202406020129/onediffx/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-06-02 01:29:58.000000 onediffx-1.1.0.dev202406020129/onediffx/utils/patch_image_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 01:30:30.913993 onediffx-1.1.0.dev202406020129/onediffx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22386 2024-06-02 01:30:30.000000 onediffx-1.1.0.dev202406020129/onediffx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-06-02 01:30:30.000000 onediffx-1.1.0.dev202406020129/onediffx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 01:30:30.000000 onediffx-1.1.0.dev202406020129/onediffx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-06-02 01:30:30.000000 onediffx-1.1.0.dev202406020129/onediffx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-06-02 01:30:30.000000 onediffx-1.1.0.dev202406020129/onediffx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 01:30:30.913993 onediffx-1.1.0.dev202406020129/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-06-02 01:29:58.000000 onediffx-1.1.0.dev202406020129/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 01:30:30.913993 onediffx-1.1.0.dev202406020129/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7248 2024-06-02 01:29:58.000000 onediffx-1.1.0.dev202406020129/tests/test_lora.py
```

### Comparing `onediffx-1.1.0.dev202406010129/PKG-INFO` & `onediffx-1.1.0.dev202406020129/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onediffx
-Version: 1.1.0.dev202406010129
+Version: 1.1.0.dev202406020129
 Summary: onediff extensions for diffusers
 Home-page: https://github.com/siliconflow/onediff
 Author: OneDiff contributors
 Author-email: contact@siliconflow.com
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -305,19 +305,19 @@
 
 - pipeline (`LoraLoaderMixin`): The pipeline that will set adapters.
 - adapter_names(`str` or `List[str]`): The adapter name(s) of LoRA(s) to be set for the pipeline, must appear in the `adapter_name` parameter of the `load_and_fuse_lora` function, otherwise it will be ignored.
 - adapter_weights(`float` or `List[float]`, optional): The weight(s) of adapter(s), if is None, it will be set to 1.0.
 
 #### `onediffx.lora.delete_adapters`
 
-`onediffx.lora.delete_adapters(pipeline: LoraLoaderMixin, adapter_names: Union[List[str], str])`
+`onediffx.lora.delete_adapters(pipeline: LoraLoaderMixin, adapter_names: Union[List[str], str] = None)`
 
 Deletes the LoRA layers of `adapter_name` for the unet and text-encoder(s).
 
-- adapter_names (`str` or `List[str]`): The names of the adapter to delete. Can be a single string or a list of strings
+- adapter_names (`str` or `List[str]`, *optional*): The names of the adapter to delete. Can be a single string or a list of strings. If is None, all adapters will be deleted.
 
 #### `onediffx.lora.update_graph_with_constant_folding_info`
 
 `onediffx.lora.update_graph_with_constant_folding_info(module: torch.nn.Module, info: Dict[str, flow.Tensor] = None)`
 
 Update the weights of graph after loading LoRA. (If OneDiff has enabled constant folding optimization during compilation, some parameters in the static graph may not be updated correctly after loading lora. Invoke this function manually to update the weights of the static graph correctly.)
```

### Comparing `onediffx-1.1.0.dev202406010129/README.md` & `onediffx-1.1.0.dev202406020129/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -277,19 +277,19 @@
 
 - pipeline (`LoraLoaderMixin`): The pipeline that will set adapters.
 - adapter_names(`str` or `List[str]`): The adapter name(s) of LoRA(s) to be set for the pipeline, must appear in the `adapter_name` parameter of the `load_and_fuse_lora` function, otherwise it will be ignored.
 - adapter_weights(`float` or `List[float]`, optional): The weight(s) of adapter(s), if is None, it will be set to 1.0.
 
 #### `onediffx.lora.delete_adapters`
 
-`onediffx.lora.delete_adapters(pipeline: LoraLoaderMixin, adapter_names: Union[List[str], str])`
+`onediffx.lora.delete_adapters(pipeline: LoraLoaderMixin, adapter_names: Union[List[str], str] = None)`
 
 Deletes the LoRA layers of `adapter_name` for the unet and text-encoder(s).
 
-- adapter_names (`str` or `List[str]`): The names of the adapter to delete. Can be a single string or a list of strings
+- adapter_names (`str` or `List[str]`, *optional*): The names of the adapter to delete. Can be a single string or a list of strings. If is None, all adapters will be deleted.
 
 #### `onediffx.lora.update_graph_with_constant_folding_info`
 
 `onediffx.lora.update_graph_with_constant_folding_info(module: torch.nn.Module, info: Dict[str, flow.Tensor] = None)`
 
 Update the weights of graph after loading LoRA. (If OneDiff has enabled constant folding optimization during compilation, some parameters in the static graph may not be updated correctly after loading lora. Invoke this function manually to update the weights of the static graph correctly.)
```

### Comparing `onediffx-1.1.0.dev202406010129/onediffx/compilers/diffusion_pipeline_compiler.py` & `onediffx-1.1.0.dev202406020129/onediffx/compilers/diffusion_pipeline_compiler.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.1.0.dev202406010129/onediffx/deep_cache/__init__.py` & `onediffx-1.1.0.dev202406020129/onediffx/deep_cache/__init__.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.1.0.dev202406010129/onediffx/deep_cache/models/fast_unet_2d_condition.py` & `onediffx-1.1.0.dev202406020129/onediffx/deep_cache/models/fast_unet_2d_condition.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.1.0.dev202406010129/onediffx/deep_cache/models/fast_unet_spatio_temporal_condition.py` & `onediffx-1.1.0.dev202406020129/onediffx/deep_cache/models/fast_unet_spatio_temporal_condition.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.1.0.dev202406010129/onediffx/deep_cache/models/pipeline_utils.py` & `onediffx-1.1.0.dev202406020129/onediffx/deep_cache/models/pipeline_utils.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.1.0.dev202406010129/onediffx/deep_cache/models/unet_2d_blocks.py` & `onediffx-1.1.0.dev202406020129/onediffx/deep_cache/models/unet_2d_blocks.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.1.0.dev202406010129/onediffx/deep_cache/models/unet_2d_condition.py` & `onediffx-1.1.0.dev202406020129/onediffx/deep_cache/models/unet_2d_condition.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.1.0.dev202406010129/onediffx/deep_cache/models/unet_3d_blocks.py` & `onediffx-1.1.0.dev202406020129/onediffx/deep_cache/models/unet_3d_blocks.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.1.0.dev202406010129/onediffx/deep_cache/models/unet_spatio_temporal_condition.py` & `onediffx-1.1.0.dev202406020129/onediffx/deep_cache/models/unet_spatio_temporal_condition.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.1.0.dev202406010129/onediffx/deep_cache/pipeline_stable_diffusion.py` & `onediffx-1.1.0.dev202406020129/onediffx/deep_cache/pipeline_stable_diffusion.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.1.0.dev202406010129/onediffx/deep_cache/pipeline_stable_diffusion_xl.py` & `onediffx-1.1.0.dev202406020129/onediffx/deep_cache/pipeline_stable_diffusion_xl.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.1.0.dev202406010129/onediffx/deep_cache/pipeline_stable_video_diffusion.py` & `onediffx-1.1.0.dev202406020129/onediffx/deep_cache/pipeline_stable_video_diffusion.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.1.0.dev202406010129/onediffx/lora/lora.py` & `onediffx-1.1.0.dev202406020129/onediffx/lora/lora.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.1.0.dev202406010129/onediffx/lora/state_dict_utils.py` & `onediffx-1.1.0.dev202406020129/onediffx/lora/state_dict_utils.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.1.0.dev202406010129/onediffx/lora/text_encoder.py` & `onediffx-1.1.0.dev202406020129/onediffx/lora/text_encoder.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.1.0.dev202406010129/onediffx/lora/unet.py` & `onediffx-1.1.0.dev202406020129/onediffx/lora/unet.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.1.0.dev202406010129/onediffx/lora/utils.py` & `onediffx-1.1.0.dev202406020129/onediffx/lora/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,16 @@
     self.lora_A = {}
     self.lora_B = {}
     self.adapter_names = set()
     self.active_adapter_names = {}
 
 
 def delete_lora_infos(self, adapter_names):
+    if adapter_names is None:
+        adapter_names = list(self.adapter_names.copy())
     curr_adapter_names = self.adapter_names.copy()
     for adapter_name in adapter_names:
         if adapter_name not in curr_adapter_names:
             continue
         self.r.pop(adapter_name)
         self.lora_alpha.pop(adapter_name)
         self.scaling.pop(adapter_name)
```

### Comparing `onediffx-1.1.0.dev202406010129/onediffx/utils/patch_image_processor.py` & `onediffx-1.1.0.dev202406020129/onediffx/utils/patch_image_processor.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.1.0.dev202406010129/onediffx.egg-info/PKG-INFO` & `onediffx-1.1.0.dev202406020129/onediffx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onediffx
-Version: 1.1.0.dev202406010129
+Version: 1.1.0.dev202406020129
 Summary: onediff extensions for diffusers
 Home-page: https://github.com/siliconflow/onediff
 Author: OneDiff contributors
 Author-email: contact@siliconflow.com
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -305,19 +305,19 @@
 
 - pipeline (`LoraLoaderMixin`): The pipeline that will set adapters.
 - adapter_names(`str` or `List[str]`): The adapter name(s) of LoRA(s) to be set for the pipeline, must appear in the `adapter_name` parameter of the `load_and_fuse_lora` function, otherwise it will be ignored.
 - adapter_weights(`float` or `List[float]`, optional): The weight(s) of adapter(s), if is None, it will be set to 1.0.
 
 #### `onediffx.lora.delete_adapters`
 
-`onediffx.lora.delete_adapters(pipeline: LoraLoaderMixin, adapter_names: Union[List[str], str])`
+`onediffx.lora.delete_adapters(pipeline: LoraLoaderMixin, adapter_names: Union[List[str], str] = None)`
 
 Deletes the LoRA layers of `adapter_name` for the unet and text-encoder(s).
 
-- adapter_names (`str` or `List[str]`): The names of the adapter to delete. Can be a single string or a list of strings
+- adapter_names (`str` or `List[str]`, *optional*): The names of the adapter to delete. Can be a single string or a list of strings. If is None, all adapters will be deleted.
 
 #### `onediffx.lora.update_graph_with_constant_folding_info`
 
 `onediffx.lora.update_graph_with_constant_folding_info(module: torch.nn.Module, info: Dict[str, flow.Tensor] = None)`
 
 Update the weights of graph after loading LoRA. (If OneDiff has enabled constant folding optimization during compilation, some parameters in the static graph may not be updated correctly after loading lora. Invoke this function manually to update the weights of the static graph correctly.)
```

### Comparing `onediffx-1.1.0.dev202406010129/onediffx.egg-info/SOURCES.txt` & `onediffx-1.1.0.dev202406020129/onediffx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onediffx-1.1.0.dev202406010129/setup.py` & `onediffx-1.1.0.dev202406020129/setup.py`

 * *Files identical despite different names*

