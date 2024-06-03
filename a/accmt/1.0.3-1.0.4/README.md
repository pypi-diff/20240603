# Comparing `tmp/accmt-1.0.3.tar.gz` & `tmp/accmt-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accmt-1.0.3.tar", last modified: Mon May  6 06:10:40 2024, max compression
+gzip compressed data, was "accmt-1.0.4.tar", last modified: Mon Jun  3 05:19:40 2024, max compression
```

## Comparing `accmt-1.0.3.tar` & `accmt-1.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 06:10:40.163909 accmt-1.0.3/
--rw-rw-rw-   0        0        0    11558 2024-03-31 07:36:29.000000 accmt-1.0.3/LICENSE
--rw-rw-rw-   0        0        0    14020 2024-05-06 06:10:40.162902 accmt-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0    13283 2024-05-02 22:06:41.000000 accmt-1.0.3/README.md
--rw-rw-rw-   0        0        0      108 2024-03-31 07:58:03.000000 accmt-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0      841 2024-05-06 06:10:40.166902 accmt-1.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-06 06:10:40.084369 accmt-1.0.3/src/
-drwxrwxrwx   0        0        0        0 2024-05-06 06:10:40.128901 accmt-1.0.3/src/accmt/
--rw-rw-rw-   0        0        0      552 2024-04-28 20:04:39.000000 accmt-1.0.3/src/accmt/__init__.py
--rw-rw-rw-   0        0        0    27404 2024-05-06 06:08:11.000000 accmt-1.0.3/src/accmt/accmt.py
--rw-rw-rw-   0        0        0     3130 2024-04-09 02:58:42.000000 accmt-1.0.3/src/accmt/collate_fns.py
--rw-rw-rw-   0        0        0      484 2024-04-01 00:09:51.000000 accmt-1.0.3/src/accmt/config.py
--rw-rw-rw-   0        0        0      161 2024-04-28 04:10:32.000000 accmt-1.0.3/src/accmt/events.py
--rw-rw-rw-   0        0        0      345 2024-04-28 20:04:47.000000 accmt-1.0.3/src/accmt/loggers.py
--rw-rw-rw-   0        0        0     4524 2024-04-29 15:38:32.000000 accmt-1.0.3/src/accmt/optimizations.py
--rw-rw-rw-   0        0        0      451 2024-05-06 05:59:07.000000 accmt-1.0.3/src/accmt/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-06 06:10:40.160903 accmt-1.0.3/src/accmt.egg-info/
--rw-rw-rw-   0        0        0    14020 2024-05-06 06:10:40.000000 accmt-1.0.3/src/accmt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      379 2024-05-06 06:10:40.000000 accmt-1.0.3/src/accmt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 06:10:40.000000 accmt-1.0.3/src/accmt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-05-06 06:10:40.000000 accmt-1.0.3/src/accmt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-06 06:10:40.000000 accmt-1.0.3/src/accmt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-03 05:19:40.549192 accmt-1.0.4/
+-rw-rw-rw-   0        0        0    11558 2024-03-31 07:36:29.000000 accmt-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0    14020 2024-06-03 05:19:40.547192 accmt-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0    13283 2024-05-02 22:06:41.000000 accmt-1.0.4/README.md
+-rw-rw-rw-   0        0        0      108 2024-03-31 07:58:03.000000 accmt-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0      841 2024-06-03 05:19:40.551192 accmt-1.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-06-03 05:19:40.491185 accmt-1.0.4/src/
+drwxrwxrwx   0        0        0        0 2024-06-03 05:19:40.520186 accmt-1.0.4/src/accmt/
+-rw-rw-rw-   0        0        0      552 2024-05-12 09:11:02.000000 accmt-1.0.4/src/accmt/__init__.py
+-rw-rw-rw-   0        0        0    30959 2024-06-03 05:16:29.000000 accmt-1.0.4/src/accmt/accmt.py
+-rw-rw-rw-   0        0        0     3130 2024-04-09 02:58:42.000000 accmt-1.0.4/src/accmt/collate_fns.py
+-rw-rw-rw-   0        0        0      484 2024-04-01 00:09:51.000000 accmt-1.0.4/src/accmt/config.py
+-rw-rw-rw-   0        0        0      161 2024-04-28 04:10:32.000000 accmt-1.0.4/src/accmt/events.py
+-rw-rw-rw-   0        0        0     5072 2024-05-08 19:42:59.000000 accmt-1.0.4/src/accmt/optimizations.py
+-rw-rw-rw-   0        0        0      352 2024-06-03 05:09:45.000000 accmt-1.0.4/src/accmt/tracker.py
+-rw-rw-rw-   0        0        0      451 2024-06-03 05:09:57.000000 accmt-1.0.4/src/accmt/utils.py
+drwxrwxrwx   0        0        0        0 2024-06-03 05:19:40.546196 accmt-1.0.4/src/accmt.egg-info/
+-rw-rw-rw-   0        0        0    14020 2024-06-03 05:19:40.000000 accmt-1.0.4/src/accmt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      379 2024-06-03 05:19:40.000000 accmt-1.0.4/src/accmt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 05:19:40.000000 accmt-1.0.4/src/accmt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-06-03 05:19:40.000000 accmt-1.0.4/src/accmt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-06-03 05:19:40.000000 accmt-1.0.4/src/accmt.egg-info/top_level.txt
```

### Comparing `accmt-1.0.3/LICENSE` & `accmt-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `accmt-1.0.3/PKG-INFO` & `accmt-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: accmt
-Version: 1.0.3
+Version: 1.0.4
 Summary: Accelerator Module and Trainer based on Accelerate library for simple distributed train processes, inspired by PyTorch Lightning.
 Home-page: https://github.com/ghanvert/AcceleratorModule
 Author: ghanvert
 Author-email: martin.pizarro@cenia.cl
 Project-URL: Bug Tracker, https://github.com/ghanvert/AcceleratorModule/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `accmt-1.0.3/README.md` & `accmt-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `accmt-1.0.3/setup.cfg` & `accmt-1.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 6363 6d74 0d0a 7665 7273 696f   = accmt..versio
-00000020: 6e20 3d20 312e 302e 330d 0a61 7574 686f  n = 1.0.3..autho
+00000020: 6e20 3d20 312e 302e 340d 0a61 7574 686f  n = 1.0.4..autho
 00000030: 7220 3d20 6768 616e 7665 7274 0d0a 6175  r = ghanvert..au
 00000040: 7468 6f72 5f65 6d61 696c 203d 206d 6172  thor_email = mar
 00000050: 7469 6e2e 7069 7a61 7272 6f40 6365 6e69  tin.pizarro@ceni
 00000060: 612e 636c 0d0a 6465 7363 7269 7074 696f  a.cl..descriptio
 00000070: 6e20 3d20 4163 6365 6c65 7261 746f 7220  n = Accelerator 
 00000080: 4d6f 6475 6c65 2061 6e64 2054 7261 696e  Module and Train
 00000090: 6572 2062 6173 6564 206f 6e20 4163 6365  er based on Acce
```

### Comparing `accmt-1.0.3/src/accmt/__init__.py` & `accmt-1.0.4/src/accmt/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     EpochStart,
     EpochEnd,
     BeforeBackward,
     AfterBackward,
     OnBatch,
     OnLoss
 )
-from .loggers import (
+from .tracker import (
     TensorBoard,
     WandB,
     CometML,
     Aim,
     MLFlow,
     ClearML,
     DVCLive
```

### Comparing `accmt-1.0.3/src/accmt/accmt.py` & `accmt-1.0.4/src/accmt/accmt.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 import numpy as np
 import torch
 
 from abc import ABC
 from accelerate import Accelerator
-from accelerate.utils import ProjectConfiguration, tqdm
-from .loggers import TensorBoard, MLFlow
+from accelerate.utils import ProjectConfiguration, InitProcessGroupKwargs, tqdm
+from .tracker import TensorBoard, MLFlow
 from .events import *
 from .config import read, save_status, read_status
-import torch.optim
+import torch
 import torch.optim.lr_scheduler as lr_scheduler
 from torch.utils.data import Dataset
 from typing import Any
 from typing_extensions import override
 from transformers import (
     get_cosine_schedule_with_warmup,
     get_constant_schedule,
     get_constant_schedule_with_warmup,
     get_cosine_with_hard_restarts_schedule_with_warmup,
     get_inverse_sqrt_schedule,
     get_linear_schedule_with_warmup,
     get_polynomial_decay_schedule_with_warmup,
     Adafactor
 )
+from datetime import timedelta
 
 OPTIMIZERS = {
     "Adam": torch.optim.Adam,
     "Adadelta": torch.optim.Adadelta,
     "Adagrad": torch.optim.Adagrad,
     "Adamax": torch.optim.Adamax,
     "AdamW": torch.optim.AdamW,
@@ -53,15 +54,16 @@
     "ConstantWithWarmup": get_constant_schedule_with_warmup,
     "CosineWithHardRestartsWithWarmup": get_cosine_with_hard_restarts_schedule_with_warmup,
     "InverseSQRT": get_inverse_sqrt_schedule,
     "LinearWithWarmup": get_linear_schedule_with_warmup,
     "PolynomialDecayWithWarmup": get_polynomial_decay_schedule_with_warmup
 }
 
-accelerator = Accelerator()
+init_kwargs = InitProcessGroupKwargs(timeout=timedelta(seconds=86400))
+accelerator = Accelerator(kwargs_handlers=[init_kwargs])
 
 
 class AcceleratorModule(ABC):
     """
     Super class to define training and validation logic without the need
     to write a training loop.
 
@@ -164,15 +166,17 @@
     """
 
     def __init__(self,
                 hps_file_config: str = None,
                 checkpoint = "checkpoint1",
                 resume = False,
                 model_path: str = None,
+                saving_strategy="epoch",
                 model_saving = "best_valid_loss",
+                evaluate_every_n_steps: int = None,
                 enable_checkpointing = True,
                 checkpoint_every = 1,
                 logging_dir = "logs",
                 log_with = TensorBoard,
                 log_every = 1,
                 grad_accumulation_steps=None,
                 set_to_none=True,
@@ -186,28 +190,32 @@
     ):
         """
         Trainer constructor to set configuration.
 
         Args:
             hps_file_config (`str`):
                 YAML hyperparameters file path.
-            checkpoint (`str`, *optional*, default to `checkpoint1`):
+            checkpoint (`str`, *optional*, defaults to `checkpoint1`):
                 Folder path where to save the checkpoint.
             resume (`bool`, *optional*, defaults to `False`):
                 Whether to resume from checkpoint or not.
             model_path (`str`, *optional*, defaults to `None`):
                 Folder path to save model. If not specified, it will name
                 the model path based on the `hps_file_config` name (without the .yaml extension).
+            saving_strategy (`str`, *optional*, defaults to `epoch`):
+                Saving strategy to implement. Valid options are `epoch` and `step`.
             model_saving (`str`, *optional*, defaults to `best_valid_loss`):
                 Type of model saving. It can be one of the following values:
 
                 - `"best_valid_loss"`: Saves the model whenever the validation loss is the best recorded.
                 - `"best_train_loss"`: Saves the model whenever the training loss is the best recorded.
                 - `"always"`: Saves the model always at the end of every epoch.
-            
+            evaluate_every_n_steps (`int`, *optional*, defaults to `None`):
+                Evaluate model in validation dataset (if implemented) every N steps. If this is set 
+                to `None` (default option), evaluation will happen at the end of every epoch.
             enable_checkpointing (`bool`, *optional*, defaults to `True`):
                 Whether to save checkpoint or not.
             checkpoint_every (`int`, *optional*, defaults to `1`):
                 Checkpoint every N steps. Only works if `enable_checkpointing` is set to `True`.
             logging_dir (`str`, *optional*, defaults to `logs`):
                 Path where to save logs to show progress.
             log_with (`str`, *optional*, defaults to `accmt.TensorBoard`):
@@ -241,15 +249,17 @@
                 Optimizations from `accmt.optimizations` to be applied during training.
         """
 
         self.hps_config = hps_file_config
         self.checkpoint = checkpoint
         self.resume = resume
         self.model_path = model_path
+        self.saving_strategy = saving_strategy
         self.model_saving = model_saving.lower()
+        self.evaluate_every_n_steps = evaluate_every_n_steps
         self.enable_checkpointing = enable_checkpointing
         self.checkpoint_every = checkpoint_every
         self.logging_dir = logging_dir
         self.log_every = log_every
         self.grad_accumulation_steps = grad_accumulation_steps if grad_accumulation_steps is not None else 1
         self.set_to_none = set_to_none
         self.shuffle_train = shuffle_train
@@ -260,16 +270,16 @@
         self.safe_serialization = safe_serialization
         self.optimizations = optimizations if optimizations is not None else []
 
         self.accelerator = accelerator
         self.accelerator.project_configuration = ProjectConfiguration(project_dir=".", logging_dir=logging_dir, total_limit=1)
         
         if not isinstance(log_with, list): log_with = [log_with]
-        self.accelerator.log_with = [logger.logger for logger in log_with]
-        self.log_with = self.accelerator.log_with
+        self.accelerator.log_with = [tracker.tracker for tracker in log_with]
+        self.log_with = [tracker for tracker in log_with]
 
     def fit(self,
             module: AcceleratorModule,
             train_dataset: Dataset,
             val_dataset: Dataset = None
     ):
         """
@@ -284,14 +294,15 @@
                 `Dataset` class from PyTorch containing the validation dataset logic. If this
                 dataset is not specified, then the validation logic of `AcceleratorModule`
                 (if specified) will be skipped. If `model_saving` parameter in the constructor is set
                 to `best_valid_loss`, this will be converted to `best_train_loss` in the background.
         """
         import os
         import torch
+        from datetime import datetime
 
         self._initialize_loggers()
 
         from torch.utils.data import DataLoader
 
         if self.hps_config is None:
             raise AttributeError("Cannot train without HPS file config.")
@@ -306,15 +317,15 @@
         hps = cfg["hps"]
         optim = hps["optim"]
         schlr = hps["scheduler"] if "scheduler" in hps else None
 
         if self.model_path is None:
             self.model_path = cfg["version"]
 
-        if self.model_saving:
+        if self.model_saving is not None:
             os.makedirs(self.model_path, exist_ok=True)
 
         best_train_loss = float("inf")
         best_valid_loss = float("inf")
         status_epoch = 0
         current_epoch_step = 0
         global_step = 0
@@ -342,67 +353,105 @@
         if schlr is not None:
             scheduler = self._get_scheduler(schlr, optimizer, -1, len(train_dataloader), hps["epochs"])
             # -1 for last_epoch since Accelerate will take care of recovering the progress
 
         model, train_dataloader, val_dataloader, optimizer, scheduler, teacher = self.accelerator.prepare(
             model, train_dataloader, val_dataloader, optimizer, scheduler, teacher
         )
-        self.model = model # TODO: see if this works properly
+        self.model = model
 
         if scheduler:
             self.accelerator.register_for_checkpointing(scheduler)
-        self.accelerator.init_trackers(self.model_path.split("/")[-1], config=hps)
+
+        experiment_name = datetime.now().strftime("%Y-%m-%d_%H:%M")
+        self.accelerator.init_trackers(self.model_path.split("/")[-1], config=hps, init_kwargs={"experiment_name": experiment_name})
 
         if self.resume:
             if os.path.exists(self.checkpoint):
                 self.accelerator.load_state(self.checkpoint)
             else:
                 raise FileNotFoundError(f"{self.checkpoint} was not found.")
 
         epochs = hps["epochs"]
         eval_step = (len(train_dataloader) // len(val_dataloader)) if val_dataloader else None
 
         self._apply_start_optimizations()
         for epoch in range(status_epoch, epochs):
+            torch.cuda.empty_cache()
             eval_global_step = global_step
             model.train()
             train_losses = [] 
             for step, batch in tqdm(
                 iterable=enumerate(train_dataloader, current_epoch_step+1),
                 total=len(train_dataloader),
                 desc=f"Epoch {epoch}/{epochs}",
                 unit="batch"
             ):
                 global_step, current_epoch_step = self._train_logic(
                     module, optimizer, batch, train_losses, step, scheduler, train_dataloader, global_step, current_epoch_step
                 )
+
+                if (
+                    all([val_dataloader, getattr(module, "validation_step", False)]) and
+                    self.evaluate_every_n_steps is not None and
+                    global_step % self.evaluate_every_n_steps == 0
+                ):
+                    model.eval()
+                    eval_losses = []
+                    with torch.no_grad():
+                        for step, batch in tqdm(
+                            iterable=enumerate(val_dataloader, 1),
+                            total=len(val_dataloader),
+                            desc=f"Evaluating",
+                            unit="batch"
+                        ):
+                            self._validation_logic(module, batch, eval_losses, step, eval_step, 1)
+                    
+                    if self.accelerator.is_main_process:
+                        best_valid_loss, best_train_loss = self._save_model_on_criteria(
+                            model, eval_losses, train_losses, best_valid_loss, best_train_loss
+                        )
+                    
+                    model.train()
+                else:
+                    if self.model_saving is not None and self.saving_strategy == "step":
+                        self.accelerator.wait_for_everyone()
+                        avg_train_loss = np.mean(train_losses)
+                        if avg_train_loss < best_train_loss:
+                            self.accelerator.print("Saving model...")
+                            self._save_model(model, best_valid_loss, best_train_loss, wait_for_everyone=False)
+                            best_train_loss = avg_train_loss
             
-            if all([val_dataloader, getattr(module, "validation_step", False)]):
+            if (
+                all([val_dataloader, getattr(module, "validation_step", False)]) and
+                self.evaluate_every_n_steps is None
+            ):
                 model.eval()
                 eval_losses = []
                 with torch.no_grad():
                     for step, batch in tqdm(
                         iterable=enumerate(val_dataloader, 1),
                         total=len(val_dataloader),
                         desc=f"Epoch {epoch}/{epochs}",
                         unit="batch"
                     ):
                         eval_global_step = self._validation_logic(
                             module, batch, eval_losses, step, eval_step, eval_global_step
                         )
 
-                best_valid_loss, best_train_loss = self._save_model_on_criteria(
-                    model, eval_losses, train_losses, best_valid_loss, best_train_loss
-                )
+                if self.accelerator.is_main_process and self.saving_strategy == "epoch":
+                    best_valid_loss, best_train_loss = self._save_model_on_criteria(
+                        model, eval_losses, train_losses, best_valid_loss, best_train_loss
+                    )
             else:
-                if self.model_saving:
+                if self.model_saving is not None and self.saving_strategy == "epoch":
+                    self.accelerator.wait_for_everyone()
                     avg_train_loss = np.mean(train_losses)
                     if avg_train_loss < best_train_loss:
-                        self.accelerator.print("Saving model...")
-                        self._save_model(model, best_valid_loss, best_train_loss)
+                        self._save_model(model, best_valid_loss, best_train_loss, wait_for_everyone=False)
                         best_train_loss = avg_train_loss
 
             self._save_checkpoint(epoch+1, best_valid_loss, best_train_loss, global_step)
 
         self.accelerator.end_training()
 
     def eval(self, module, val_dataset: Dataset, batch_size=1) -> float:
@@ -475,55 +524,61 @@
         if step % self.log_every == 0:
             self.accelerator.log({"val_loss": loss_item}, step=eval_global_step)
 
         eval_global_step += eval_step
 
         return eval_global_step
 
-    def _save_model(self, model, best_valid_loss, best_train_loss):
+    def _save_model(self, model, best_valid_loss, best_train_loss, wait_for_everyone=True):
+        if wait_for_everyone:
+            self.accelerator.wait_for_everyone()
+
+        self.accelerator.print("Saving model...")
         state_dict = self.accelerator.get_state_dict(model)
         unwrapped_model = self.accelerator.unwrap_model(model)
         if getattr(unwrapped_model, "save_pretrained", None) is not None:
             unwrapped_model.save_pretrained(
                 self.model_path,
                 is_main_process=self.accelerator.is_main_process,
                 state_dict=state_dict,
                 max_shard_size=self.max_shard_size,
                 save_function=self.accelerator.save,
                 safe_serialization=self.safe_serialization
             )
         else:
             self.accelerator.save(
-                unwrapped_model,
-                f"{self.model_path}/pytorch_model.bin",
+                state_dict,
+                f"{self.model_path}/pytorch_model.pt",
                 safe_serialization=self.safe_serialization
             )
 
         save_status({
             "best_valid_loss": best_valid_loss,
             "best_train_loss": best_train_loss,
         }, to=f"{self.model_path}/status.json")
 
     
     def _save_model_on_criteria(self, model, eval_losses, train_losses, best_valid_loss, best_train_loss):
         if self.model_saving is None:
             return
+        
+        self.accelerator.wait_for_everyone()
 
         avg_valid_loss = np.mean(eval_losses)
         avg_train_loss = np.mean(train_losses)
 
         saving_criteria = {
             "best_valid_loss": avg_valid_loss < best_valid_loss and avg_valid_loss < self.model_saving_below_loss,
             "best_train_loss": avg_train_loss < best_train_loss and avg_train_loss < self.model_saving_below_loss,
             "always": True
         }
 
         if self.model_saving in saving_criteria:
             if saving_criteria[self.model_saving]:
-                self._save_model(model, best_valid_loss, best_train_loss)
+                self._save_model(model, best_valid_loss, best_train_loss, wait_for_everyone=False)
         else:
             raise ValueError("Invalid type of model saving. Value must be: "
                               "'best_valid_train_loss', "
                               "'best_train_loss', or "
                               "'always'.")
         
         return (
@@ -539,14 +594,15 @@
                 try:
                     dictionary[k] = float(v)
                 except ValueError:
                     continue
 
     def _save_checkpoint(self, epoch, best_valid_loss, best_train_loss, global_step):
         if (self.enable_checkpointing and epoch % self.checkpoint_every == 0):
+            self.accelerator.wait_for_everyone()
             self.accelerator.print("Saving checkpoint...")
             self.accelerator.save_state(self.checkpoint, safe_serialization=self.safe_serialization)
             save_status({
                 "best_valid_loss": best_valid_loss,
                 "best_train_loss": best_train_loss,
                 "epoch": epoch,
                 "global_step": global_step
@@ -557,24 +613,31 @@
         optim_kwargs = optim.copy()
         del optim_kwargs["type"]
         self._fix_kwargs(optim_kwargs)
 
         return OPTIMIZERS[t](model.parameters(), **optim_kwargs)
 
     def _filter_kwargs(self, _kwargs: dict, fn):
-        return {k:v for k,v in _kwargs.items() if k in fn.__init__.__code__.co_varnames}
+        try:
+            return {k:v for k,v in _kwargs.items() if k in fn.__init__.__code__.co_varnames}
+        except AttributeError:
+            import inspect
+            signature = inspect.signature(fn)
+            parameters = list(signature.parameters.keys())
+            return {k:v for k,v in _kwargs.items() if k in parameters}
 
     def _get_scheduler(self, schlr: dict, optimizer, last_epoch, steps_per_epoch, epochs):
         t = schlr["type"]
         schlr_kwargs = schlr.copy()
         del schlr_kwargs["type"]
         self._fix_kwargs(schlr_kwargs)
 
         schlr_kwargs["last_epoch"] = last_epoch
         schlr_kwargs["steps_per_epoch"] = steps_per_epoch
+        schlr_kwargs["num_training_steps"] = steps_per_epoch
         schlr_kwargs["epochs"] = epochs
         filtered_kwargs = self._filter_kwargs(schlr_kwargs, SCHEDULERS[t])
 
         return SCHEDULERS[t](optimizer, **filtered_kwargs)
 
     def _apply_start_optimizations(self):
         if self.accelerator.is_main_process:
@@ -617,15 +680,16 @@
 
     def _apply_after_backward_optimizations(self, parameters):
         for optimization in self.optimizations:
             type = optimization.__class__.__bases__[0]
             if isinstance(type, AfterBackward):
                 optimization(parameters)
 
-    def _initialize_loggers(self):
-        from .utils import is_url
-
-        for logger in self.log_with:
-            if isinstance(logger, MLFlow) and is_url(self.logging_dir):
-                import mlflow
-                mlflow.set_tracking_uri(self.logging_dir)
-                break
+    def _initialize_trackers(self):
+        if accelerator.is_main_process:
+            from .utils import is_url
+
+            for logger in self.log_with:
+                if isinstance(logger, MLFlow) and is_url(self.logging_dir):
+                    import mlflow
+                    mlflow.set_tracking_uri(self.logging_dir)
+                    break
```

### Comparing `accmt-1.0.3/src/accmt/collate_fns.py` & `accmt-1.0.4/src/accmt/collate_fns.py`

 * *Files identical despite different names*

### Comparing `accmt-1.0.3/src/accmt/optimizations.py` & `accmt-1.0.4/src/accmt/optimizations.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,19 +58,32 @@
 
         return random.sample(modules, num_selected)
 
 class LabelSmoothing(OnBatch):
     """
     Applies label smoothing regulatization technique for one-hot target tensors.
     """
-    def __init__(self, smoothing=0.1):
+    def __init__(self, smoothing=0.1, key: str = None):
+        """
+        Args:
+            smoothing (`float`, *optional*, defaults to `0.1`):
+                Smoothing or alpha value to smooth one hot vectors.
+            key (`str`, *optional*, defaults to `None`):
+                In case that every batch is a dictionary, this will be the labels key.
+        """
         self.smoothing = smoothing
+        self.key = key
 
     def __call__(self, batch):
-        _, target = batch
+        if isinstance(batch, dict):
+            assert self.key in batch.keys(), f"'{self.key}' is not a valid key."
+            target = batch[self.key]
+        else:
+            _, target = batch
+        
         if getattr(target, "shape", None) is not None:
             K = target.shape[-1]
         else:
             K = len(target)
         
         return (1 - self.smoothing) * target + self.smoothing / K
```

### Comparing `accmt-1.0.3/src/accmt.egg-info/PKG-INFO` & `accmt-1.0.4/src/accmt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: accmt
-Version: 1.0.3
+Version: 1.0.4
 Summary: Accelerator Module and Trainer based on Accelerate library for simple distributed train processes, inspired by PyTorch Lightning.
 Home-page: https://github.com/ghanvert/AcceleratorModule
 Author: ghanvert
 Author-email: martin.pizarro@cenia.cl
 Project-URL: Bug Tracker, https://github.com/ghanvert/AcceleratorModule/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

