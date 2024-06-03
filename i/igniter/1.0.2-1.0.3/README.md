# Comparing `tmp/igniter-1.0.2.tar.gz` & `tmp/igniter-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "igniter-1.0.2.tar", last modified: Fri Apr 12 06:06:52 2024, max compression
+gzip compressed data, was "igniter-1.0.3.tar", last modified: Mon Jun  3 02:59:19 2024, max compression
```

## Comparing `igniter-1.0.2.tar` & `igniter-1.0.3.tar`

### file list

```diff
@@ -1,43 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:06:52.501770 igniter-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-12 06:06:42.000000 igniter-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-12 06:06:52.501770 igniter-1.0.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:06:52.497770 igniter-1.0.2/igniter/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-12 06:06:42.000000 igniter-1.0.2/igniter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11565 2024-04-12 06:06:42.000000 igniter-1.0.2/igniter/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-04-12 06:06:42.000000 igniter-1.0.2/igniter/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:06:52.497770 igniter-1.0.2/igniter/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-12 06:06:42.000000 igniter-1.0.2/igniter/configs/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:06:52.497770 igniter-1.0.2/igniter/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-12 06:06:42.000000 igniter-1.0.2/igniter/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-12 06:06:42.000000 igniter-1.0.2/igniter/datasets/coco.py
--rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-04-12 06:06:42.000000 igniter-1.0.2/igniter/datasets/s3_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:06:52.497770 igniter-1.0.2/igniter/defaults/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-12 06:06:42.000000 igniter-1.0.2/igniter/defaults/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-12 06:06:42.000000 igniter-1.0.2/igniter/defaults/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:06:52.501770 igniter-1.0.2/igniter/engine/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-12 06:06:42.000000 igniter-1.0.2/igniter/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3341 2024-04-12 06:06:42.000000 igniter-1.0.2/igniter/engine/inference_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     6638 2024-04-12 06:06:42.000000 igniter-1.0.2/igniter/engine/trainer_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-04-12 06:06:42.000000 igniter-1.0.2/igniter/engine/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:06:52.501770 igniter-1.0.2/igniter/io/
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-12 06:06:42.000000 igniter-1.0.2/igniter/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-04-12 06:06:42.000000 igniter-1.0.2/igniter/io/s3_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-04-12 06:06:42.000000 igniter-1.0.2/igniter/io/s3_io.py
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-12 06:06:42.000000 igniter-1.0.2/igniter/io/s3_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-12 06:06:42.000000 igniter-1.0.2/igniter/io/summary.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-12 06:06:42.000000 igniter-1.0.2/igniter/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     7108 2024-04-12 06:06:42.000000 igniter-1.0.2/igniter/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-12 06:06:42.000000 igniter-1.0.2/igniter/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-04-12 06:06:42.000000 igniter-1.0.2/igniter/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-12 06:06:42.000000 igniter-1.0.2/igniter/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:06:52.497770 igniter-1.0.2/igniter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-12 06:06:52.000000 igniter-1.0.2/igniter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-12 06:06:52.000000 igniter-1.0.2/igniter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 06:06:52.000000 igniter-1.0.2/igniter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-12 06:06:52.000000 igniter-1.0.2/igniter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-12 06:06:52.000000 igniter-1.0.2/igniter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-12 06:06:52.000000 igniter-1.0.2/igniter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 06:06:52.000000 igniter-1.0.2/igniter.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-12 06:06:42.000000 igniter-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 06:06:52.501770 igniter-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-12 06:06:42.000000 igniter-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 02:59:19.681475 igniter-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-06-03 02:59:11.000000 igniter-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-06-03 02:59:19.681475 igniter-1.0.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 02:59:19.677475 igniter-1.0.3/igniter/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-06-03 02:59:11.000000 igniter-1.0.3/igniter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11977 2024-06-03 02:59:11.000000 igniter-1.0.3/igniter/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7157 2024-06-03 02:59:11.000000 igniter-1.0.3/igniter/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 02:59:19.677475 igniter-1.0.3/igniter/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-06-03 02:59:11.000000 igniter-1.0.3/igniter/configs/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 02:59:19.677475 igniter-1.0.3/igniter/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-06-03 02:59:11.000000 igniter-1.0.3/igniter/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-06-03 02:59:11.000000 igniter-1.0.3/igniter/datasets/coco.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-06-03 02:59:11.000000 igniter-1.0.3/igniter/datasets/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-06-03 02:59:11.000000 igniter-1.0.3/igniter/datasets/s3_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 02:59:19.677475 igniter-1.0.3/igniter/defaults/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-06-03 02:59:11.000000 igniter-1.0.3/igniter/defaults/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-06-03 02:59:11.000000 igniter-1.0.3/igniter/defaults/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-06-03 02:59:11.000000 igniter-1.0.3/igniter/defaults/inference_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 02:59:19.677475 igniter-1.0.3/igniter/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-06-03 02:59:11.000000 igniter-1.0.3/igniter/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-06-03 02:59:11.000000 igniter-1.0.3/igniter/engine/inference_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7277 2024-06-03 02:59:11.000000 igniter-1.0.3/igniter/engine/trainer_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6006 2024-06-03 02:59:11.000000 igniter-1.0.3/igniter/engine/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 02:59:19.681475 igniter-1.0.3/igniter/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-06-03 02:59:11.000000 igniter-1.0.3/igniter/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-06-03 02:59:11.000000 igniter-1.0.3/igniter/io/ignite_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-06-03 02:59:11.000000 igniter-1.0.3/igniter/io/logger_handles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-06-03 02:59:11.000000 igniter-1.0.3/igniter/io/s3_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-06-03 02:59:11.000000 igniter-1.0.3/igniter/io/s3_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-06-03 02:59:11.000000 igniter-1.0.3/igniter/io/s3_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-06-03 02:59:11.000000 igniter-1.0.3/igniter/io/summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-06-03 02:59:11.000000 igniter-1.0.3/igniter/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7108 2024-06-03 02:59:11.000000 igniter-1.0.3/igniter/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-06-03 02:59:11.000000 igniter-1.0.3/igniter/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-06-03 02:59:11.000000 igniter-1.0.3/igniter/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-06-03 02:59:11.000000 igniter-1.0.3/igniter/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 02:59:19.677475 igniter-1.0.3/igniter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-06-03 02:59:19.000000 igniter-1.0.3/igniter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-06-03 02:59:19.000000 igniter-1.0.3/igniter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 02:59:19.000000 igniter-1.0.3/igniter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-06-03 02:59:19.000000 igniter-1.0.3/igniter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-06-03 02:59:19.000000 igniter-1.0.3/igniter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-06-03 02:59:19.000000 igniter-1.0.3/igniter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 02:59:19.000000 igniter-1.0.3/igniter.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-06-03 02:59:11.000000 igniter-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 02:59:19.681475 igniter-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-06-03 02:59:11.000000 igniter-1.0.3/setup.py
```

### Comparing `igniter-1.0.2/PKG-INFO` & `igniter-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: igniter
-Version: 1.0.2
+Version: 1.0.3
 Home-page: https://github.com/iKrishneel/igniter
 Author: Krishneel
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `igniter-1.0.2/igniter/builder.py` & `igniter-1.0.3/igniter/builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,27 +58,34 @@
         attrs = dict(transforms_cfg[key])
         if name and key != name or attrs is None:
             continue
 
         engine = attrs.pop('engine', 'torchvision.transforms')
         module = importlib.import_module(engine)
 
-        transform_list = []
+        try:
+            compose = module.v2.Compose
+        except AttributeError:
+            compose = module.Compose
+
+        transform_list = []        
         for obj, kwargs in attrs.items():
+            if 'compose' in obj.lower() and kwargs is not None:
+                compose = transform_registry.get(kwargs) or compose
+                continue
             transform = transform_registry[obj] if obj in transform_registry else getattr(module, obj)
             if inspect.isclass(transform):
                 kwargs = kwargs or {}
                 transform = transform(**kwargs)
             transform_list.append(transform)
-        transforms[key] = module.Compose(transform_list)
+        transforms[key] = compose(transform_list)
 
     return transforms[name] if name else transforms
 
 
-@torch.compile
 @configurable
 def build_dataloader(model_name: str, cfg: DictConfig, mode: str) -> DataLoader:
     logger.info(f'Building {mode} dataloader')
 
     key: str = 'transforms'
     build_kwargs = cfg.build[model_name]
     ds_name = build_kwargs.dataset
@@ -164,18 +171,21 @@
         engine = io_cfg.engine
         cls = io_registry[engine]
         cls = importlib.import_module(engine) if cls is None else cls
         try:
             return cls.build(io_cfg, cfg)
         except AttributeError:
             return cls(io_cfg, cfg)
-
     return {key: _build(cfg.io[key]) for key in cfg.io}
 
 
+def build_logger(cfg: DictConfig):
+    pass
+
+
 @configurable
 def build_validation(model_name: str, cfg: DictConfig, trainer_engine: Engine) -> Union[Engine, None]:
     if not cfg.build[model_name].get('val', None):
         logger.warning('Not validation config found. Validation will be skipped')
         return None
 
     logger.info('Adding validation')
@@ -315,15 +325,18 @@
     defaults = OmegaConf.create({'resume': False, 'eval': False, 'train': True, 'test': False})
     options = OmegaConf.merge(defaults, cfg.options)
     return options
 
 
 def _trainer(rank: Union[int, None], cfg: DictConfig) -> None:
     trainer = build_engine(cfg)
-    trainer()
+    if trainer:
+        trainer()
+    else:
+        logger.warning('Engine not available, Terminating execution!!')
 
 
 def trainer(cfg: DictConfig) -> None:
     if is_distributed(cfg):
         init_args = dict(cfg.distributed[cfg.distributed.type])
         with idist.Parallel(
             backend=cfg.distributed.backend, nproc_per_node=cfg.distributed.nproc_per_node, **init_args
```

### Comparing `igniter-1.0.2/igniter/configs/config.yaml` & `igniter-1.0.3/igniter/configs/config.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 driver:
 device: cpu
 dtype: float32
 
 workdir:
+  path: ./igniter_logs/
+  unqiue: False
 
 distributed:
   backend: nccl
   type: single  # single or multiple
   nproc_per_node: 1
   single:
     init_method: tcp://127.0.0.1:23456
@@ -27,14 +29,17 @@
 
 io:
   checkpoint:
     engine: 'file_writer'
     root: "./weights/"
     save: "all"  # or state, scheduler, optimizer
 
+  log_handler:
+    engine: 'tqdm'
+
 build:
 
 options:
   train: True
   eval: True
 
 flow:
```

### Comparing `igniter-1.0.2/igniter/datasets/coco.py` & `igniter-1.0.3/igniter/datasets/coco.py`

 * *Files identical despite different names*

### Comparing `igniter-1.0.2/igniter/datasets/s3_dataset.py` & `igniter-1.0.3/igniter/datasets/s3_dataset.py`

 * *Files identical despite different names*

### Comparing `igniter-1.0.2/igniter/defaults/defaults.py` & `igniter-1.0.3/igniter/defaults/defaults.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 
 @func_registry('default')
 def default_forward(engine, batch) -> None:
     engine._model.train()
     inputs, targets = batch
     losses = engine._model(inputs, targets)
+    n_size = len(losses)
 
     if isinstance(losses, dict):
         loss_sum = sum(losses.values())
         losses['total_loss'] = loss_sum
     else:
         loss_sum = losses
         losses = {'total_loss': loss_sum}
@@ -29,14 +30,16 @@
     engine._optimizer.step()
     losses['lr'] = engine.get_lr()
 
     if torch.cuda.is_available():
         free, total = torch.cuda.mem_get_info()
         losses['gpu_mem'] = convert_bytes_to_human_readable(total - free)
 
+    if n_size == 1:
+        losses.pop('total_loss')
     engine.state.metrics = losses
 
 
 @func_registry('default_evaluation')
 @func_registry('default_val_forward')
 def default_val_forward(engine, batch) -> Dict[str, Any]:
     engine._model.eval()
```

### Comparing `igniter-1.0.2/igniter/engine/inference_engine.py` & `igniter-1.0.3/igniter/engine/inference_engine.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,14 +67,15 @@
         logger.info(f'Using device: {self.device}')
 
         model = build_model(cfg) if model is None else model
         load_weights(model, cfg, strict=kwargs.get('strict', True))
         model.to(self.device)
         model.to(getattr(torch, cfg.dtype))
         model.eval()
+        # self._model = torch.compile(model) if hasattr(torch, 'compile') else model
         self._model = model
 
         logger.info('Inference Engine is Ready!')
 
     @torch.inference_mode()
     def __call__(self, image: Union[np.ndarray, Image.Image, torch.Tensor], **kwargs: Dict[str, Any]):
         assert image is not None, 'Input image is required'
```

### Comparing `igniter-1.0.2/igniter/engine/trainer_engine.py` & `igniter-1.0.3/igniter/engine/trainer_engine.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,26 +4,44 @@
 import os
 from datetime import datetime
 from typing import Any, Callable, Dict, Optional, Union
 
 import ignite.distributed as idist
 import torch
 import torch.nn as nn
-from ignite.contrib.handlers import ProgressBar
-from ignite.engine import Engine, Events
+from ignite.engine import Engine as _Engine
+from ignite.engine import Events
+from ignite.handlers import Checkpoint
 from omegaconf import DictConfig, OmegaConf
 from torch.utils.data import DataLoader
 
 from igniter.logger import logger
 from igniter.registry import engine_registry, io_registry
 from igniter.utils import get_device, is_distributed, model_name
 
+try:
+    from ignite.handlers import ProgressBar
+except ImportError:
+    from ignite.contrib.handlers import ProgressBar
+
+
 __all__ = ['TrainerEngine', 'EvaluationEngine']
 
 
+def get_datetime(fmt: str = '%Y-%m-%dT%H-%M-%S') -> str:
+    return str(datetime.now().strftime(fmt))
+
+
+class Engine(_Engine):
+    def add_persistent_logger(self) -> None:
+        if hasattr(self, 'log_handler'):
+            kwargs = getattr(self.log_handler, '_attach_kwargs', {})
+            self.log_handler.attach(self, **kwargs)
+
+
 @engine_registry('default_trainer')
 class TrainerEngine(Engine):
     def __init__(
         self,
         cfg: DictConfig,
         process_func: Callable,
         model: nn.Module,
@@ -48,20 +66,21 @@
             model = model.to(get_device(cfg))
 
         self._cfg = cfg
         self._model = model
         self._optimizer = optimizer
         self._dataloader = dataloader
 
+        self.log_handler = ProgressBar(persist=False)
         self.checkpoint = None
         if io_ops:
             self.__dict__.update(io_ops)
 
         if cfg.workdir.get('unique', False):
-            name = 'run_' + str(datetime.now().strftime('%Y-%m-%d_%H-%M-%S'))
+            name = 'run_' + get_datetime()
             self.log_dir = os.path.join(str(cfg.workdir.path), name)
         else:
             self.log_dir = str(cfg.workdir.path)
 
         self._writer = io_registry['summary_writer'](log_dir=self.log_dir)
 
         # TODO: better way to handle the event type
@@ -70,15 +89,15 @@
             if isinstance(self._scheduler, torch.optim.lr_scheduler.OneCycleLR)
             else Events.EPOCH_COMPLETED
         )
         self.add_event_handler(scheduler_event, self.scheduler)
         self.add_event_handler(Events.ITERATION_COMPLETED, self.summary)
 
         self.checkpoint_handler()
-        self.add_persistent_logger(self)
+        self.add_persistent_logger()
 
         OmegaConf.save(cfg, os.path.join(self.log_dir, 'config.yaml'))
 
     def __call__(self) -> None:
         train_cfg = self._cfg.build[model_name(self._cfg)].train
         epoch_length = train_cfg.get('iters_per_epoch', len(self._dataloader))
         self.run(self._dataloader, train_cfg.epochs, epoch_length=epoch_length)
@@ -96,61 +115,62 @@
             value = self.state.metrics[key]
             value = torch.Tensor([value]) if isinstance(value, (float, int)) else value
             if torch.isnan(value.detach().cpu()).any():
                 raise ValueError(f'{key} is NaN. Terminating on iteration {self.state.iteration}')
 
             self._writer.add_scalar(f'train/{key}', value, self.state.iteration)
 
-    def checkpoint_handler(self) -> None:
+    def checkpoint_handler(self, prefix: str = '%s') -> None:
         if self._cfg.solvers.snapshot <= 0:
-            return
-
-        prefix = '%s'
-        if self.checkpoint is None:
-            logger.warning(f'Using default checkpoint saver to directory {self.log_dir}')
-            self.checkpoint = importlib.import_module('torch').save
-            prefix = os.path.join(self.log_dir, '%s')
+            logger.warning('Not model checkpoint will be saved because snapshot <= 0')
             return
 
         def _checkpointer():
             filename = prefix % f'model_{str(self.state.epoch).zfill(7)}.pt'
             self.checkpoint(self.get_state_dict(), filename)
 
+        if self.checkpoint is None:
+            default_path = f'./logs/{self._cfg.build.model}/models/{get_datetime()}'
+            logger.info(f'No checkpoint handler! Using default and saving {default_path}')
+
+            _checkpointer = Checkpoint(
+                {'model': self._model},
+                default_path,
+                n_saved=2,
+                filename_prefix=prefix % '',
+            )
+
         self.add_event_handler(
             Events.ITERATION_COMPLETED(every=self._cfg.solvers.snapshot) | Events.EPOCH_COMPLETED, _checkpointer
         )
 
     def get_lr(self) -> float:
         lr = self._optimizer.param_groups[0]['lr']
         return lr[0] if isinstance(lr, list) else lr
 
     def get_state_dict(self) -> Dict[str, Any]:
         state_dict = {
             'model': self._model.state_dict(),
             'cfg': self._cfg,
             'optimizer': self._optimizer.state_dict(),
-            'scheduler': self._scheduler.state_dict(),
+            'scheduler': self._scheduler.state_dict() if self._scheduler is not None else None,
             'state': self.state,
         }
 
-        save_options = self._cfg.io.checkpoint.get('save', 'all')
+        save_options = self._cfg.io.checkpoint.get('save', 'all') if hasattr(self._cfg.io, 'checkpoint') else 'state'
         if save_options == 'all':
             return state_dict
 
         for key in ['optimizer', 'scheduler', 'state']:
             if key in save_options:
                 continue
             state_dict.pop(key)
 
         return state_dict
 
-    @staticmethod
-    def add_persistent_logger(engine, **kwargs) -> None:
-        ProgressBar(persist=False).attach(engine, metric_names='all', output_transform=None)
-
 
 @engine_registry('default_evaluation')
 class EvaluationEngine(Engine):
     def __init__(
         self,
         cfg: DictConfig,
         process_func: Callable,
@@ -177,14 +197,14 @@
         self._model = model
         self._dataloader = dataloader
 
         if io_ops:
             self.__dict__.update(io_ops)
 
         self._iter = 0
-        TrainerEngine.add_persistent_logger(self)
+        self.add_persistent_logger()
 
     def __call__(self):
         self._iter = 0
         val_cfg = self._cfg.build[model_name(self._cfg)].val
         epoch_length = val_cfg.get('iters_per_epoch', len(self._dataloader))
         self.run(self._dataloader, getattr(val_cfg, 'epochs', 1), epoch_length=epoch_length)
```

### Comparing `igniter-1.0.2/igniter/io/s3_client.py` & `igniter-1.0.3/igniter/io/s3_client.py`

 * *Files identical despite different names*

### Comparing `igniter-1.0.2/igniter/io/s3_io.py` & `igniter-1.0.3/igniter/io/s3_io.py`

 * *Files identical despite different names*

### Comparing `igniter-1.0.2/igniter/io/s3_utils.py` & `igniter-1.0.3/igniter/io/s3_utils.py`

 * *Files identical despite different names*

### Comparing `igniter-1.0.2/igniter/logger.py` & `igniter-1.0.3/igniter/logger.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,8 +23,9 @@
 console_handler.setFormatter(formatter)
 
 # file_handler = logging.FileHandler('/tmp/logs.log')
 # file_handler.setLevel(level)
 # file_handler.setFormatter(logging.Formatter(format_style))
 
 logger.addHandler(console_handler)
+logger.setLevel(level)
 # logger.addHandler(file_handler)
```

### Comparing `igniter-1.0.2/igniter/main.py` & `igniter-1.0.3/igniter/main.py`

 * *Files identical despite different names*

### Comparing `igniter-1.0.2/igniter/registry.py` & `igniter-1.0.3/igniter/registry.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,55 +1,77 @@
 #!/usr/bin/env python
 
 from dataclasses import dataclass, field
 from typing import Any, Callable, Dict, Optional, Union
 
 from tabulate import tabulate
 
+from igniter.logger import logger
+
 
 @dataclass
 class Registry(object):
     name: str = 'REGISTRY'
     overwrite: bool = False
+    strict: bool = True
     __REGISTRY: Dict[str, object] = field(default_factory=lambda: {})
 
+    def __post_init__(self):
+        if self.overwrite and self.strict:
+            logger.warning('Both stict and overwrite flags are set. Not strict will take precedence!')
+
     def __call__(self, name_or_cls: Union[str, object] = None, prefix: Optional[str] = None):
         def _wrapper(cls):
             assert callable(cls)
             name = cls.__name__ if name_or_cls is None or not isinstance(name_or_cls, str) else name_or_cls
             name = prefix + name if prefix else name
-            if name in self.__REGISTRY and not self.overwrite:
-                raise ValueError(f'{cls} is already registered {self.__REGISTRY}')
+            if name in self.__REGISTRY:
+                if self.strict:
+                    raise ValueError(f'{cls} is already registered {self.__REGISTRY}')
+
+                if not self.overwrite:
+                    return
+                else:
+                    logger.warning(f'⚠️  Overwriting {name} ...')
             self.__REGISTRY[name] = cls
             return cls
 
         if callable(name_or_cls):
             name = str(name_or_cls.__name__)  # NOQA: F841
             return _wrapper(name_or_cls)
         return _wrapper
 
     def __getitem__(self, name: str):
-        return self.__REGISTRY.get(name, None)
+        if name not in self.__REGISTRY:
+            print(self)
+            raise KeyError(f'Key {name} not found in the {self.name}')
+        return self.__REGISTRY.get(name)
 
     def __contains__(self, key: str):
         return key in self.__REGISTRY.keys()
 
     def register(self, name_or_cls: Union[str, object] = None):
         return self(name_or_cls=name_or_cls)
 
     def get(self, name: str) -> Callable:
-        return self[name]
+        return self[name] if name in self else None
 
     def remove(self, name: str) -> Any:
+        logger.warning(f'⚠️  Removing {name}')        
         return self.__REGISTRY.pop(name, None)
 
     def deregister(self, name: str) -> Any:
         return self.remove(name)
 
-    def clear(self):
+    def clear(self) -> None:
+        if self.strict:
+            logger.warning('⚠️ Cannot clear registry with strict flag set')
+            return
+
+        logger.warning(f'⚠️ Clearning {self.name}')
         self.__REGISTRY.clear()
 
     def __repr__(self):
         title = f'Registry for {self.name}\n'
         return title + tabulate(
             [[k, v] for k, v in self.__REGISTRY.items()], headers=['Name', 'Objects'], tablefmt="fancy_grid"
         )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `igniter-1.0.2/igniter/utils.py` & `igniter-1.0.3/igniter/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #!/usr/bin/env python
 
 import os.path as osp
+import re
 from enum import Enum
 from typing import Tuple, Union
 
 import torch
 from omegaconf import DictConfig, ListConfig, OmegaConf
 
 from .logger import logger
@@ -81,7 +82,20 @@
 
 
 def get_dir_and_file_name(path: str, abs_path: bool = True, remove_ext: bool = True) -> Tuple[str, str]:
     dirname, filename = osp.dirname(path), osp.basename(path)
     filename = osp.splitext(filename)[0] if remove_ext else filename
     dirname = osp.abspath(dirname) if abs_path and not osp.isabs(dirname) else dirname
     return dirname, filename
+
+
+def find_pattern(text: str, pattern: str):
+    assert all(isinstance(arg, str) for arg in (text, pattern))    
+
+    matches = re.finditer(pattern, text)
+    return matches
+
+
+def find_replace_pattern(text: str, replacement: str, pattern: str):
+    assert all(isinstance(arg, str) for arg in (text, pattern, replacement))
+
+    return re.sub(pattern, replacement, text)
```

### Comparing `igniter-1.0.2/igniter/visualizer.py` & `igniter-1.0.3/igniter/visualizer.py`

 * *Files identical despite different names*

### Comparing `igniter-1.0.2/igniter.egg-info/PKG-INFO` & `igniter-1.0.3/igniter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: igniter
-Version: 1.0.2
+Version: 1.0.3
 Home-page: https://github.com/iKrishneel/igniter
 Author: Krishneel
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `igniter-1.0.2/igniter.egg-info/SOURCES.txt` & `igniter-1.0.3/igniter.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -15,19 +15,23 @@
 igniter.egg-info/entry_points.txt
 igniter.egg-info/requires.txt
 igniter.egg-info/top_level.txt
 igniter.egg-info/zip-safe
 igniter/configs/config.yaml
 igniter/datasets/__init__.py
 igniter/datasets/coco.py
+igniter/datasets/dataset.py
 igniter/datasets/s3_dataset.py
 igniter/defaults/__init__.py
 igniter/defaults/defaults.py
+igniter/defaults/inference_runner.py
 igniter/engine/__init__.py
 igniter/engine/inference_engine.py
 igniter/engine/trainer_engine.py
 igniter/engine/utils.py
 igniter/io/__init__.py
+igniter/io/ignite_logger.py
+igniter/io/logger_handles.py
 igniter/io/s3_client.py
 igniter/io/s3_io.py
 igniter/io/s3_utils.py
 igniter/io/summary.py
```

### Comparing `igniter-1.0.2/setup.py` & `igniter-1.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,16 @@
     'omegaconf',
     'colorlog',
     'boto3',
     'pytest',
     'pytest-mock',
     'pytorch-ignite>=0.4.12',
     'tensorboard',
+    'argcomplete',
+    'safetensors',
 ]
 
 
 __name__ = 'igniter'
 
 with open(f'{__name__}/__init__.py', 'r') as init_file:
     for line in init_file:
@@ -53,15 +55,15 @@
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',        
+        'Programming Language :: Python :: 3.11',
     ],
     entry_points={
         'console_scripts': {
             'igniter=igniter.cli:main',
         },
     },
 )
```

