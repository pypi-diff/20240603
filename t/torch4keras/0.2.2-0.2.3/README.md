# Comparing `tmp/torch4keras-0.2.2.tar.gz` & `tmp/torch4keras-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch4keras-0.2.2.tar", last modified: Thu Apr 18 15:35:17 2024, max compression
+gzip compressed data, was "torch4keras-0.2.3.tar", last modified: Mon Jun  3 15:01:34 2024, max compression
```

## Comparing `torch4keras-0.2.2.tar` & `torch4keras-0.2.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 lb        (1000) lb        (1000)        0 2024-04-18 15:35:17.554753 torch4keras-0.2.2/
--rw-rw-r--   0 lb        (1000) lb        (1000)    11357 2024-03-15 02:30:46.000000 torch4keras-0.2.2/LICENSE
--rw-r--r--   0 lb        (1000) lb        (1000)     5376 2024-04-18 15:35:17.554753 torch4keras-0.2.2/PKG-INFO
--rw-rw-r--   0 lb        (1000) lb        (1000)     5086 2024-04-18 15:28:12.000000 torch4keras-0.2.2/README.md
--rw-rw-r--   0 lb        (1000) lb        (1000)       38 2024-04-18 15:35:17.554753 torch4keras-0.2.2/setup.cfg
--rw-rw-r--   0 lb        (1000) lb        (1000)      524 2024-04-18 15:34:26.000000 torch4keras-0.2.2/setup.py
-drwxrwxr-x   0 lb        (1000) lb        (1000)        0 2024-04-18 15:35:17.554753 torch4keras-0.2.2/test/
--rw-rw-r--   0 lb        (1000) lb        (1000)      435 2024-03-15 02:30:46.000000 torch4keras-0.2.2/test/test_log.py
--rw-rw-r--   0 lb        (1000) lb        (1000)      842 2024-03-15 02:30:46.000000 torch4keras-0.2.2/test/test_time.py
-drwxrwxr-x   0 lb        (1000) lb        (1000)        0 2024-04-18 15:35:17.554753 torch4keras-0.2.2/torch4keras/
--rw-rw-r--   0 lb        (1000) lb        (1000)      254 2024-03-15 02:30:46.000000 torch4keras-0.2.2/torch4keras/__init__.py
--rw-rw-r--   0 lb        (1000) lb        (1000)    67636 2024-04-17 09:13:38.000000 torch4keras-0.2.2/torch4keras/callbacks.py
--rw-rw-r--   0 lb        (1000) lb        (1000)      759 2024-04-17 10:19:39.000000 torch4keras-0.2.2/torch4keras/model.py
-drwxrwxr-x   0 lb        (1000) lb        (1000)        0 2024-04-18 15:35:17.554753 torch4keras-0.2.2/torch4keras/snippets/
--rw-rw-r--   0 lb        (1000) lb        (1000)      117 2024-03-15 02:30:46.000000 torch4keras-0.2.2/torch4keras/snippets/__init__.py
--rw-rw-r--   0 lb        (1000) lb        (1000)     9337 2024-03-15 02:30:46.000000 torch4keras-0.2.2/torch4keras/snippets/data_process.py
--rw-rw-r--   0 lb        (1000) lb        (1000)     1210 2024-03-15 02:30:46.000000 torch4keras-0.2.2/torch4keras/snippets/import_utils.py
--rw-rw-r--   0 lb        (1000) lb        (1000)    12359 2024-04-09 07:03:51.000000 torch4keras-0.2.2/torch4keras/snippets/log.py
--rw-rw-r--   0 lb        (1000) lb        (1000)    13496 2024-04-17 09:15:00.000000 torch4keras-0.2.2/torch4keras/snippets/misc.py
--rw-rw-r--   0 lb        (1000) lb        (1000)    12175 2024-04-03 07:32:23.000000 torch4keras-0.2.2/torch4keras/snippets/monitor.py
-drwxrwxr-x   0 lb        (1000) lb        (1000)        0 2024-04-18 15:35:17.554753 torch4keras-0.2.2/torch4keras/trainer/
--rw-rw-r--   0 lb        (1000) lb        (1000)      128 2024-04-09 02:47:12.000000 torch4keras-0.2.2/torch4keras/trainer/__init__.py
--rw-rw-r--   0 lb        (1000) lb        (1000)     1872 2024-04-09 02:36:34.000000 torch4keras-0.2.2/torch4keras/trainer/accelerate.py
--rw-rw-r--   0 lb        (1000) lb        (1000)    35899 2024-04-17 10:27:39.000000 torch4keras-0.2.2/torch4keras/trainer/base.py
--rw-rw-r--   0 lb        (1000) lb        (1000)     2696 2024-04-09 02:37:24.000000 torch4keras-0.2.2/torch4keras/trainer/ddp.py
--rw-rw-r--   0 lb        (1000) lb        (1000)    12040 2024-04-17 10:52:28.000000 torch4keras-0.2.2/torch4keras/trainer/deepspeed.py
--rw-rw-r--   0 lb        (1000) lb        (1000)      403 2024-04-09 02:39:36.000000 torch4keras-0.2.2/torch4keras/trainer/dp.py
--rw-rw-r--   0 lb        (1000) lb        (1000)     3543 2024-04-09 02:39:24.000000 torch4keras-0.2.2/torch4keras/trainer/utils.py
-drwxrwxr-x   0 lb        (1000) lb        (1000)        0 2024-04-18 15:35:17.554753 torch4keras-0.2.2/torch4keras.egg-info/
--rw-r--r--   0 lb        (1000) lb        (1000)     5376 2024-04-18 15:35:17.000000 torch4keras-0.2.2/torch4keras.egg-info/PKG-INFO
--rw-rw-r--   0 lb        (1000) lb        (1000)      710 2024-04-18 15:35:17.000000 torch4keras-0.2.2/torch4keras.egg-info/SOURCES.txt
--rw-rw-r--   0 lb        (1000) lb        (1000)        1 2024-04-18 15:35:17.000000 torch4keras-0.2.2/torch4keras.egg-info/dependency_links.txt
--rw-rw-r--   0 lb        (1000) lb        (1000)       16 2024-04-18 15:35:17.000000 torch4keras-0.2.2/torch4keras.egg-info/requires.txt
--rw-rw-r--   0 lb        (1000) lb        (1000)       12 2024-04-18 15:35:17.000000 torch4keras-0.2.2/torch4keras.egg-info/top_level.txt
+drwxrwxr-x   0 lb        (1000) lb        (1000)        0 2024-06-03 15:01:34.387256 torch4keras-0.2.3/
+-rw-rw-r--   0 lb        (1000) lb        (1000)    11357 2024-03-15 02:30:46.000000 torch4keras-0.2.3/LICENSE
+-rw-r--r--   0 lb        (1000) lb        (1000)     5372 2024-06-03 15:01:34.387256 torch4keras-0.2.3/PKG-INFO
+-rw-rw-r--   0 lb        (1000) lb        (1000)     5107 2024-06-03 14:59:24.000000 torch4keras-0.2.3/README.md
+-rw-rw-r--   0 lb        (1000) lb        (1000)       38 2024-06-03 15:01:34.387256 torch4keras-0.2.3/setup.cfg
+-rw-rw-r--   0 lb        (1000) lb        (1000)      511 2024-06-03 14:57:12.000000 torch4keras-0.2.3/setup.py
+drwxrwxr-x   0 lb        (1000) lb        (1000)        0 2024-06-03 15:01:34.387256 torch4keras-0.2.3/test/
+-rw-rw-r--   0 lb        (1000) lb        (1000)      435 2024-03-15 02:30:46.000000 torch4keras-0.2.3/test/test_log.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)      842 2024-03-15 02:30:46.000000 torch4keras-0.2.3/test/test_time.py
+drwxrwxr-x   0 lb        (1000) lb        (1000)        0 2024-06-03 15:01:34.387256 torch4keras-0.2.3/torch4keras/
+-rw-rw-r--   0 lb        (1000) lb        (1000)      464 2024-05-24 01:03:25.000000 torch4keras-0.2.3/torch4keras/__init__.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)    67750 2024-05-24 02:09:51.000000 torch4keras-0.2.3/torch4keras/callbacks.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)      741 2024-05-24 01:59:37.000000 torch4keras-0.2.3/torch4keras/model.py
+drwxrwxr-x   0 lb        (1000) lb        (1000)        0 2024-06-03 15:01:34.387256 torch4keras-0.2.3/torch4keras/snippets/
+-rw-rw-r--   0 lb        (1000) lb        (1000)      117 2024-05-23 15:34:07.000000 torch4keras-0.2.3/torch4keras/snippets/__init__.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)     9470 2024-05-24 00:59:07.000000 torch4keras-0.2.3/torch4keras/snippets/data_process.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)     1279 2024-05-23 15:59:13.000000 torch4keras-0.2.3/torch4keras/snippets/import_utils.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)    12506 2024-05-24 02:10:48.000000 torch4keras-0.2.3/torch4keras/snippets/log.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)    17388 2024-05-24 02:03:54.000000 torch4keras-0.2.3/torch4keras/snippets/misc.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)    12219 2024-06-03 14:48:57.000000 torch4keras-0.2.3/torch4keras/snippets/monitor.py
+drwxrwxr-x   0 lb        (1000) lb        (1000)        0 2024-06-03 15:01:34.387256 torch4keras-0.2.3/torch4keras/trainer/
+-rw-rw-r--   0 lb        (1000) lb        (1000)      128 2024-04-09 02:47:12.000000 torch4keras-0.2.3/torch4keras/trainer/__init__.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)     1872 2024-04-09 02:36:34.000000 torch4keras-0.2.3/torch4keras/trainer/accelerate.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)    35900 2024-05-24 02:08:15.000000 torch4keras-0.2.3/torch4keras/trainer/base.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)     2696 2024-04-09 02:37:24.000000 torch4keras-0.2.3/torch4keras/trainer/ddp.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)    12040 2024-04-17 10:52:28.000000 torch4keras-0.2.3/torch4keras/trainer/deepspeed.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)      403 2024-04-09 02:39:36.000000 torch4keras-0.2.3/torch4keras/trainer/dp.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)     3543 2024-04-09 02:39:24.000000 torch4keras-0.2.3/torch4keras/trainer/utils.py
+drwxrwxr-x   0 lb        (1000) lb        (1000)        0 2024-06-03 15:01:34.387256 torch4keras-0.2.3/torch4keras.egg-info/
+-rw-r--r--   0 lb        (1000) lb        (1000)     5372 2024-06-03 15:01:34.000000 torch4keras-0.2.3/torch4keras.egg-info/PKG-INFO
+-rw-rw-r--   0 lb        (1000) lb        (1000)      710 2024-06-03 15:01:34.000000 torch4keras-0.2.3/torch4keras.egg-info/SOURCES.txt
+-rw-rw-r--   0 lb        (1000) lb        (1000)        1 2024-06-03 15:01:34.000000 torch4keras-0.2.3/torch4keras.egg-info/dependency_links.txt
+-rw-rw-r--   0 lb        (1000) lb        (1000)        6 2024-06-03 15:01:34.000000 torch4keras-0.2.3/torch4keras.egg-info/requires.txt
+-rw-rw-r--   0 lb        (1000) lb        (1000)       12 2024-06-03 15:01:34.000000 torch4keras-0.2.3/torch4keras.egg-info/top_level.txt
```

### Comparing `torch4keras-0.2.2/LICENSE` & `torch4keras-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `torch4keras-0.2.2/PKG-INFO` & `torch4keras-0.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: torch4keras
-Version: 0.2.2
+Version: 0.2.3
 Summary: Use torch like keras
 Home-page: https://github.com/Tongjilibo/torch4keras
 Author: Tongjilibo
 License: Apache License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
-Requires-Dist: torch>1.6
 
 ![torch4keras](./docs/pics/torch4keras.png)
 
 
 [![licence](https://img.shields.io/github/license/Tongjilibo/torch4keras.svg?maxAge=3600)](https://github.com/Tongjilibo/torch4keras/blob/master/LICENSE) 
 [![GitHub release](https://img.shields.io/github/release/Tongjilibo/torch4keras.svg?maxAge=3600)](https://github.com/Tongjilibo/torch4keras/releases) 
 [![PyPI](https://img.shields.io/pypi/v/torch4keras?label=pypi%20package)](https://pypi.org/project/torch4keras/) 
@@ -76,16 +75,16 @@
 ## 3. 快速上手
 - 参考[bert4torch](https://github.com/Tongjilibo/bert4torch)的训练过程
 - 简单示例: [turorials_mnist](https://github.com/Tongjilibo/torch4keras/blob/master/examples/turorials_mnist.py)
 
 ## 4. 版本历史
 |更新日期| 版本 | 版本说明 |
 |------| ----------------- |----------- |
+|20240603|v0.2.3|去除对torch依赖,snippets部分可用；移动bert4torch中snippets|
 |20240418|v0.2.2|增加YamlConfig和IniConfig, 优化deepspeed的使用，修复`_prepare_inputs`的bug，修复断点续训`SmoothMetricsCallback`起点错误的bug, Trainer断点续训记录batch数|
 |20240317|v0.2.1.post2     |训练异常时保存权重，避免空数据集error，默认指标使用滑窗平滑，BaseModelDDP修改的更易用，mapping允许是函数更易用，Checkpoint增加save_on_train_end，增加SystemCallback，修改run_callback=False的bug, 适配build_MiniLLM_from_scratch, 修复ddp中mix_precision和torch重名的bug|
-|20240221|v0.2.0           | fit中修改.train()逻辑较少耗时|
 
 [更多版本](https://github.com/Tongjilibo/torch4keras/blob/master/docs/Update.md)
 
 ## 5. 更新历史：
 
 [更多历史](https://github.com/Tongjilibo/torch4keras/blob/master/docs/History.md)
```

### Comparing `torch4keras-0.2.2/README.md` & `torch4keras-0.2.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -64,16 +64,16 @@
 ## 3. 快速上手
 - 参考[bert4torch](https://github.com/Tongjilibo/bert4torch)的训练过程
 - 简单示例: [turorials_mnist](https://github.com/Tongjilibo/torch4keras/blob/master/examples/turorials_mnist.py)
 
 ## 4. 版本历史
 |更新日期| 版本 | 版本说明 |
 |------| ----------------- |----------- |
+|20240603|v0.2.3|去除对torch依赖,snippets部分可用；移动bert4torch中snippets|
 |20240418|v0.2.2|增加YamlConfig和IniConfig, 优化deepspeed的使用，修复`_prepare_inputs`的bug，修复断点续训`SmoothMetricsCallback`起点错误的bug, Trainer断点续训记录batch数|
 |20240317|v0.2.1.post2     |训练异常时保存权重，避免空数据集error，默认指标使用滑窗平滑，BaseModelDDP修改的更易用，mapping允许是函数更易用，Checkpoint增加save_on_train_end，增加SystemCallback，修改run_callback=False的bug, 适配build_MiniLLM_from_scratch, 修复ddp中mix_precision和torch重名的bug|
-|20240221|v0.2.0           | fit中修改.train()逻辑较少耗时|
 
 [更多版本](https://github.com/Tongjilibo/torch4keras/blob/master/docs/Update.md)
 
 ## 5. 更新历史：
 
 [更多历史](https://github.com/Tongjilibo/torch4keras/blob/master/docs/History.md)
```

### Comparing `torch4keras-0.2.2/test/test_time.py` & `torch4keras-0.2.3/test/test_time.py`

 * *Files identical despite different names*

### Comparing `torch4keras-0.2.2/torch4keras/callbacks.py` & `torch4keras-0.2.3/torch4keras/callbacks.py`

 * *Files 2% similar despite different names*

```diff
@@ -583,21 +583,22 @@
        :param patience: int, 最长等候的次数, 默认为0
        :param verbose: int, 是否打印, 默认为0表示不打印
        :param min_max: str, 控制监控指标monitor的大小方向, 默认为'auto', 可选{'auto', 'min', 'max'}
        :param epoch_or_step: str, 控制是按照epoch还是step来计算, 默认为'epoch', 可选{'step', 'epoch'}
        :param baseline: None/float, 基线, 默认为None 
        :param restore_best_weights: bool, stopping时候是否恢复最优的权重, 默认为False
 
-       Example
-       ----------------
+       Examples:
+       ```python
        >>> # 如果连续3个epoch, test_acc还没有继续增长则停止训练
        >>> early_stop = EarlyStopping(monitor='test_acc', verbose=1, epoch_or_step='epoch', patience=3, min_max='max')
-       >>>
+
        >>> # 如果连续100个steps, loss还未继续下降则停止训练
        >>> early_stop = EarlyStopping(monitor='loss', verbose=1, epoch_or_step='step', patience=100, min_max='min')
+       ```
 
     '''
     def __init__(self, monitor:str='perf', min_delta:float=0, patience:int=0, verbose:int=0, min_max:Literal['auto', 'min', 'max']='auto', 
                  epoch_or_step:Literal['epoch', 'step']='epoch', baseline:float=None, restore_best_weights:bool=False, **kwargs):
         super(EarlyStopping, self).__init__(**kwargs)
         assert epoch_or_step in {'step', 'epoch'}, 'Args `epoch_or_step` only support `step` or `epoch`'
         self.epoch_or_step = epoch_or_step  # 默认的epoch和原版一样
@@ -829,30 +830,31 @@
 
     > 可选参数, 用于具体指定每个文件保存, 一般推荐直接指定save_dir即可
     :param model_path: str, 模型保存路径(含文件名), 可以使用{epoch}和{step}占位符
     :param optimizer_path: str, 优化器保存路径(含文件名), 可以使用{epoch}和{step}占位符, 默认为None表示不保存
     :param scheduler_path: str, scheduler保存路径(含文件名), 可以使用{epoch}和{step}占位符, 默认为None表示不保存
     :param steps_params_path: str, 模型训练进度保存路径(含文件名), 可以使用{epoch}和{step}占位符, 默认为None表示不保存
     
-    Example
-    ---------------
+    Examples:
+    ```python
     >>> # 每个epoch结束时保存
     >>> ckpt = Checkpoint(save_dir='./ckpt/{epoch}', epoch_or_step='epoch')
-    >>>
+    
     >>> # 每隔1000个steps保存
     >>> ckpt = Checkpoint(save_dir='./ckpt/{step}', epoch_or_step='step', interval=1000)
-    >>>
+    
     >>> # 保存loss最小的3个权重
     >>> ckpt = Checkpoint(save_dir='./ckpt/{epoch}', epoch_or_step='epoch', monitor='loss', min_max='min', max_save_count=3)
-    >>>
+    
     >>> # 保存最近的3个权重
     >>> ckpt = Checkpoint(save_dir='./ckpt/{epoch}', epoch_or_step='epoch', monitor=None, max_save_count=3)
-    >>>
+    
     >>> # 保存文件夹名称中含指标名, 方便查看
     >>> ckpt = Checkpoint(save_dir='./ckpt/{epoch}_{loss}')
+    ```
     '''
     def __init__(self, save_dir:str=None, epoch_or_step:Literal['epoch', 'step']='epoch', interval:int=100, monitor:str=None, 
                  min_max:Literal['max', 'min']='min', verbose:int=0, max_save_count:int=None, max_save_count_path:str=None, 
                  save_on_train_end:bool=False, **kwargs):
         super().__init__(**kwargs)
         assert epoch_or_step in {'step', 'epoch'}, 'Args `epoch_or_step` only support `step` or `epoch`'
         self.epoch_or_step = epoch_or_step
@@ -973,26 +975,27 @@
     
     > 可选参数
     :param model_path: str, 模型保存路径(含文件名), 可以使用{epoch}和{step}占位符
     :param optimizer_path: str, 优化器保存路径(含文件名), 可以使用{epoch}和{step}占位符, 默认为None表示不保存
     :param scheduler_path: str, scheduler保存路径(含文件名), 可以使用{epoch}和{step}占位符, 默认为None表示不保存
     :param steps_params_path: str, 模型训练进度保存路径(含文件名), 可以使用{epoch}和{step}占位符, 默认为None表示不保存
     
-    Example
-    ------------------
+    Examples:
+    ```python
     >>> class MyEvaluator(Evaluator):
     >>> def evaluate(self):
     >>>     test_acc = random.random()  # 计算逻辑示例
     >>>     return {'test_acc': test_acc}
-    >>>
+    
     >>> # 每个epoch进行评估, 并保存test_acc最大的ckpt权重
     >>> evaluator = MyEvaluator(monitor='test_acc', save_dir='./ckpt/best/', min_max='max', epoch_or_step='epoch')
-    >>>
+    
     >>> # 每隔1000个steps进行评估, 并保存test_acc最大的ckpt权重
     >>> evaluator = MyEvaluator(monitor='test_acc', save_dir='./ckpt/best/', min_max='max', epoch_or_step='step', interval=1000)
+    ```
     '''
     def __init__(self, monitor:str='perf', min_max:Literal['max', 'min']='max', verbose:int=2, 
                  save_dir:str=None, epoch_or_step:Literal['epoch', 'step']='epoch', interval:int=100, **kwargs):
         super().__init__(save_dir, epoch_or_step, interval, **kwargs)
         self.monitor = monitor
         assert min_max in {'max', 'min'}, 'Compare performance only support `max/min`'
         self.min_max = min_max
@@ -1038,18 +1041,19 @@
 
     :param log_path: str, log文件的保存路径
     :param interval: int, 保存log的间隔
     :param mode: str, log保存的模式, 默认为'a'表示追加
     :param separator: str, 指标间分隔符
     :param level: str, DEBUG/INFO/WARNING/ERROR/CRITICAL, 指定log的level
 
-    Example
-    ---------------------
+    Examples:
+    ```python
     >>> # 每隔100个step记录下当前指标
     >>> logger = Logger('./ckpt/log.log', interval=100)
+    ```
     '''
     def __init__(self, log_path:str, interval:int=100, mode:Literal['a', 'w']='a', separator:str='\t', 
                  level:Literal['DEBUG','INFO','WARNING','ERROR','CRITICAL']='DEBUG', name:str='root', **kwargs):
         super(Logger, self).__init__(**kwargs)
         self.log_path = log_path
         self.interval = interval
         self.mode = mode
@@ -1095,17 +1099,18 @@
     赋值需要分栏目的用'/'进行分隔
     若每隔一定steps对验证集评估, 则Tensorboard的interval设置成和Evaluater一致或者约数, 保证Tensorboard能记录到
 
     :param log_dir: str, tensorboard文件的保存路径
     :param interval: int, 保存tensorboard的间隔
     :param prefix: str, tensorboard分栏的前缀, 默认为'train'
 
-    Example
-    --------------------
+    Examples:
+    ```python
     >>> ts_board = Tensorboard('./ckpt/tensorboard')
+    ```
     '''
     def __init__(self, log_dir:str, interval:int=100, prefix:str='Train', **kwargs):
         super(Tensorboard, self).__init__(**kwargs)
         self.log_dir = log_dir
         self.interval = interval
         self.prefix_step = prefix+'/' if len(prefix.strip()) > 0 else ''  # 控制默认的前缀, 用于区分栏目
         self.prefix_epoch = prefix+'_epoch/' if len(prefix.strip()) > 0 else 'Epoch/'  # 控制默认的前缀, 用于区分栏目
@@ -1149,17 +1154,18 @@
     '''监控system的状态
 
     :param log_dir: str, tensorboard文件的保存路径
     :param interval: int, 保存tensorboard的间隔
     :param gpu_id_list: List[int], 需要记录的gpuid列表
     :param pids: int/List[int], 需要记录的
 
-    Example
-    ---------------------------
+    Examples:
+    ```python
     >>> syscallback = SystemStateCallback('./ckpt/tensorboard/system')
+    ```
     '''
     def __init__(self, log_dir:str, interval:int=100, gpu_id_list:List[int]=None, pids:Union[int,List[int]]=None, **kwargs):
         super(SystemStateCallback, self).__init__(log_dir, interval, **kwargs)
         self.gpu_id_list = gpu_id_list
         self.pids = pids or os.getpid()
         self.pids = [self.pids] if isinstance(self.pids, int) else self.pids
 
@@ -1254,17 +1260,18 @@
 
     :param interval: int, log的的step间隔
     :param watch (:obj:`str`, `optional` defaults to :obj:`"gradients"`):
         Can be :obj:`"gradients"`, :obj:`"all"` or :obj:`"false"`. Set to :obj:`"false"` to disable gradient
         logging or :obj:`"all"` to log gradients and parameters.
     :param project: str, wandb的project name, 默认为bert4torch
     
-    Example
-    ---------------------
+    Examples:
+    ```python
     >>> wandb = WandbCallback(save_code=True)
+    ```
     '''
     def __init__(self, project:str='bert4torch', trial_name:str=None, run_name:str=None, watch:str='gradients', 
                  interval:int=100, save_code:bool=False, config:dict=None):
         try:
             import wandb
             self._wandb = wandb
         except ImportError:
@@ -1418,22 +1425,27 @@
     :param epoch_or_step: str, 控制是按照epoch还是step来发送邮件, 默认为'epoch', 可选{'step', 'epoch'}
     :param interval: int, 发送邮件的的step间隔
     :param mail_host: str, 发件服务器host
     :param mail_user: str, 发件人
     :param mail_pwd: str, smtp的第三方密码
     :param mail_sender: str, 发件人邮箱
 
-    Example
-    ----------------------
+    Examples:
+    ```python
     >>> # 每个epoch结束后, 使用默认邮箱把对应的指标发送到指定邮箱
     >>> email = EmailCallback(mail_receivers='tongjilibo@163.com', epoch_or_step='epoch')
-    >>>
+    
     >>> # 每个epoch结束后, 使用自定义邮箱把对应的指标发送到指定邮箱
-    >>> email = EmailCallback(mail_receivers='tongjilibo@163.com', epoch_or_step='epoch', 
-    mail_host='smtp.163.com', mail_user='bert4torch', mail_pwd='VDSGQEHFXDZOCVEH', mail_sender='bert4torch@163.com')
+    >>> email = EmailCallback(mail_receivers='tongjilibo@163.com', 
+    ...                       epoch_or_step='epoch', 
+    ...                       mail_host='smtp.163.com', 
+    ...                       mail_user='bert4torch', 
+    ...                       mail_pwd='VDSGQEHFXDZOCVEH', 
+    ...                       mail_sender='bert4torch@163.com')
+    ```
     '''
     def __init__(self, mail_receivers:Union[str,list], mail_subject:str='', epoch_or_step:Literal['epoch', 'step']='epoch', interval:int=100, 
                  mail_host:str=None, mail_user:str=None, mail_pwd:str=None, mail_sender:str=None, **kwargs):
         super(EmailCallback, self).__init__(**kwargs)
         self.epoch_or_step = epoch_or_step
         self.interval = interval
         self.mail_receivers = mail_receivers
```

### Comparing `torch4keras-0.2.2/torch4keras/snippets/data_process.py` & `torch4keras-0.2.3/torch4keras/snippets/data_process.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,40 @@
 import numpy as np
-import torch
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 from packaging import version
-from torch.utils.data import Dataset, IterableDataset
 import inspect
-from .import_utils import is_safetensors_available, is_sklearn_available
+from .import_utils import is_safetensors_available, is_sklearn_available, is_torch_available
 import os
-from torch import nn
+
+
+if is_torch_available():
+    import torch
+    from torch.utils.data import Dataset, IterableDataset
+    from torch import nn, Tensor
+    from torch.nn import Module
+else:
+    class Tensor: pass
+    class Module: pass
+    class Dataset: pass
+    class IterableDataset: pass
 
 
 if is_safetensors_available():
     from safetensors import safe_open
     from safetensors.torch import load_file as safe_load_file
     from safetensors.torch import save_file as safe_save_file
 
+
 if is_sklearn_available():
     from sklearn.metrics import roc_auc_score
 else:
     roc_auc_score = None
 
 
-def take_along_dim(input_tensor:torch.Tensor, indices:torch.Tensor, dim:int=None):
+def take_along_dim(input_tensor:Tensor, indices:Tensor, dim:int=None):
     '''兼容部分低版本pytorch没有torch.take_along_dim
     '''
     if version.parse(torch.__version__) > version.parse('1.8.1'):
         return torch.take_along_dim(input_tensor, indices, dim)
     else:
         # 该逻辑仅在少量数据上测试, 如有bug, 欢迎反馈
         if dim is None:
@@ -32,15 +42,15 @@
         else:
             res = np.take_along_axis(input_tensor.cpu().numpy(), indices.cpu().numpy(), axis=dim)
             res = torch.from_numpy(res).to(input_tensor.device)
         # assert res.equal(torch.take_along_dim(input_tensor, indices, dim))
         return res
 
 
-def torch_div(input:torch.Tensor, other:torch.Tensor, rounding_mode:Optional[str] = None):
+def torch_div(input:Tensor, other:Tensor, rounding_mode:Optional[str] = None):
     ''' torch.div兼容老版本
     '''
     if version.parse(torch.__version__) < version.parse('1.7.2'):
         indices = input // other  # 兼容老版本
     else:
         indices = torch.div(input, other, rounding_mode=rounding_mode)  # 行索引
     return indices
@@ -50,15 +60,15 @@
     '''numpy版softmax
     '''
     x = x - x.max(axis=axis, keepdims=True)
     x = np.exp(x)
     return x / x.sum(axis=axis, keepdims=True)
 
 
-def search_layer(model:nn.Module, layer_name:str, retrun_first:bool=True):
+def search_layer(model:Module, layer_name:str, retrun_first:bool=True):
     '''根据layer_name搜索并返回参数/参数list
     '''
     return_list = []
     for name, param in model.named_parameters():
         if param.requires_grad and layer_name in name:
             return_list.append(param)
     if len(return_list) == 0:
@@ -138,22 +148,22 @@
     precision = [1, 0.1, 0.01, 0.001, 0.0001, 0.00001, 0.000001]
     for len_, prec in enumerate(precision):
         if abs(num) >= prec:
             return round(num, len_ + dense_round)
     return num
 
 
-def metric_mapping(metric:str, func:Callable, y_pred:Union[torch.Tensor, List[torch.Tensor], Tuple[torch.Tensor]], 
-                   y_true:Union[torch.Tensor, List[torch.Tensor], Tuple[torch.Tensor]]):
+def metric_mapping(metric:str, func:Callable, y_pred:Union[Tensor, List[Tensor], Tuple[Tensor]], 
+                   y_true:Union[Tensor, List[Tensor], Tuple[Tensor]]):
     '''metric的计算
 
     :param metric: str, 自带metrics的名称
     :param func: function, 透传的用户自定的计算指标的函数
-    :param y_pred: torch.Tensor, 样本的预测结果
-    :param y_true: torch.Tensor, 样本的真实结果
+    :param y_pred: Tensor, 样本的预测结果
+    :param y_true: Tensor, 样本的真实结果
     '''
     # 自定义metrics
     if inspect.isfunction(func):
         metric_res = func(y_pred, y_true)
         if inspect.isfunction(metric):
             # 如果直接传入回调函数（无key）, 要求回调函数返回Dict[String: Int/Float]类型
             assert isinstance(metric_res, dict), 'Custom metrics callbacks should return `Dict[String: Int/Float]` value'
```

### Comparing `torch4keras-0.2.2/torch4keras/snippets/import_utils.py` & `torch4keras-0.2.3/torch4keras/snippets/import_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,13 +22,17 @@
         # print(f"Detected {pkg_name} version {package_version}")
     if return_version:
         return package_exists, package_version
     else:
         return package_exists
 
 
+def is_torch_available():
+    return is_package_available("torch")
+
+
 def is_safetensors_available():
     return is_package_available("safetensors")
 
 
 def is_sklearn_available():
     return is_package_available("sklearn")
```

### Comparing `torch4keras-0.2.2/torch4keras/snippets/log.py` & `torch4keras-0.2.3/torch4keras/snippets/log.py`

 * *Files 8% similar despite different names*

```diff
@@ -131,16 +131,16 @@
         elif self.date_format == 'prefix':
             self.file = os.path.join(self.save_dir, self.date + '_' + self.file_name)
         elif self.date_format == 'suffix':
             self.file = os.path.join(self.save_dir, self.file_name + '_' + self.date)
         else:
             raise ValueError('Args `date_format` only support subdir|prefix|suffix.')
 
-        if (save_dir := os.path.dirname(self.file)) != '':
-            os.makedirs(save_dir, exist_ok=True)
+        if os.path.dirname(self.file) != '':
+            os.makedirs(os.path.dirname(self.file), exist_ok=True)
 
         # 创建日志器
         self.log = logging.getLogger(self.file_name)
 
         # 日志器默认级别
         level_dict = {'DEBUG': logging.DEBUG, 'INFO': logging.INFO, 'WARNING': logging.WARNING, 
                       'ERROR': logging.ERROR, 'CRITICAL':logging.CRITICAL}
@@ -224,16 +224,16 @@
             self.addHandler(stream_handle)
             stream_handle.setLevel(level_dict[level])
             stream_handle.setFormatter(formatter)
 
         # 文件流输出
         if log_path is None:
             return
-        if (dirname := os.path.dirname(log_path)) != '':
-            os.makedirs(dirname, exist_ok=True)
+        if os.path.dirname(log_path) != '':
+            os.makedirs(os.path.dirname(log_path), exist_ok=True)
         if 'FileHander' in handles:
             file_handle = logging.FileHandler(filename=log_path, mode='a', encoding='utf-8')
         elif 'RotatingFileHandler' in handles:
             if handle_config is None:
                 handle_config = {'maxBytes': 1024*1024*10, 'backupCount': 30, 'encoding': 'utf-8'}
             from logging.handlers import RotatingFileHandler
             file_handle = RotatingFileHandler(log_path, **handle_config)
@@ -247,75 +247,75 @@
         self.addHandler(file_handle)
         file_handle.setLevel(level_dict[level])
         file_handle.setFormatter(formatter)
 
 
 def json_flat(config:dict, sep='.'):
     '''把嵌套的字典flat化
-    Example
-    ---------------
-    config = {'train_batch_size': 2,
-            "optimizer": {
-                "type": "AdamW",
-                "params": {
-                    "lr": 5e-4,
-                    "betas": [0.8, 0.999],
-                    "eps": 1e-8,
-                    "weight_decay": 3e-7
-                }
-            }
-            }
-    print_table(flat_config(config), headers=['config_name', 'config_value'])
-
-    >>> 结果输出
-    +----------------------------------------------------+
-    | config_name                         | config_value |
-    +----------------------------------------------------+
-    | train_batch_size                    | 2            |
-    | optimizer -> type                   | AdamW        |
-    | optimizer -> params -> lr           | 0.0005       |
-    | optimizer -> params -> betas        | [0.8, 0.999] |
-    | optimizer -> params -> eps          | 1e-08        |
-    | optimizer -> params -> weight_decay | 3e-07        |
-    +----------------------------------------------------+
+    Examples:
+    ```python
+    >>> config = {'train_batch_size': 2,
+    ...         "optimizer": {
+    ...             "type": "AdamW",
+    ...             "params": {
+    ...                 "lr": 5e-4,
+    ...                 "betas": [0.8, 0.999],
+    ...                 "eps": 1e-8,
+    ...                 "weight_decay": 3e-7
+    ...             }
+    ...         }
+    ...         }
+    >>> print_table(flat_config(config), headers=['config_name', 'config_value'])
+    ... # +----------------------------------------------------+
+    ... # | config_name                         | config_value |
+    ... # +----------------------------------------------------+
+    ... # | train_batch_size                    | 2            |
+    ... # | optimizer -> type                   | AdamW        |
+    ... # | optimizer -> params -> lr           | 0.0005       |
+    ... # | optimizer -> params -> betas        | [0.8, 0.999] |
+    ... # | optimizer -> params -> eps          | 1e-08        |
+    ... # | optimizer -> params -> weight_decay | 3e-07        |
+    ... # +----------------------------------------------------+
+    ```
     '''
     res = []
     def _flat_config(config, pre_k=''):
         for k, v in config.items():
             key = k if pre_k == '' else pre_k + sep + k
             if isinstance(v, dict):
                 _flat_config(v, key)
             else:
                 res.append([key, v])
     _flat_config(config)
     return res
-    
+
+
 def print_table(data:Union[List, List[List], List[Dict]], headers:List=None):
     '''格式化打印表格，不依赖第三方包
 
-    Example
-    ---------------
+    Examples:
+    ```python
     >>> # 示例数据  
     >>> data = [  
-    >>>     [1, "Alice", 25],  
-    >>>     [2, "Bob", 30],  
-    >>>     [3, "Charlie", 35]  
-    >>> ]  
+    ...     [1, "Alice", 25],  
+    ...     [2, "Bob", 30],  
+    ...     [3, "Charlie", 35]  
+    ... ]  
     >>> headers = ["ID", "Name", "Age"]  
     >>> # 打印表格  
     >>> print_table(data, headers)
-
-    结果输出：
-    +--------------------+
-    | ID | Name    | Age |
-    +--------------------+
-    | 1  | Alice   | 25  |
-    | 2  | Bob     | 30  |
-    | 3  | Charlie | 35  |
-    +--------------------+
+    ... # 结果输出：
+    ... # +--------------------+
+    ... # | ID | Name    | Age |
+    ... # +--------------------+
+    ... # | 1  | Alice   | 25  |
+    ... # | 2  | Bob     | 30  |
+    ... # | 3  | Charlie | 35  |
+    ... # +--------------------+
+    ```
     '''
     assert isinstance(data, list), 'Args `data` only accept list format'
     if isinstance(data[0], dict):
         headers = list(data[0].keys())
         data = [list(i.values()) for i in data]
 
     # 获取列的最大宽度
```

### Comparing `torch4keras-0.2.2/torch4keras/snippets/misc.py` & `torch4keras-0.2.3/torch4keras/snippets/misc.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,28 @@
 import numpy as np
-import torch
-from torch import nn, Tensor
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 import os
 import random
 from .log import log_info, log_warn, log_error, log_warn_once, print_table
 from .monitor import format_timestamp, format_time
+from .import_utils import is_torch_available
 import json
 import time
 import sys
+import shutil
+import re
+
+
+if is_torch_available():
+    import torch
+    from torch import Tensor
+    from torch.nn import Module
+else:
+    class Tensor: pass
+    class Module: pass
 
 
 def seed_everything(seed:int=None):
     '''固定seed
     
     :param seed: int, 随机种子
     '''
@@ -29,15 +39,15 @@
     torch.cuda.manual_seed(seed)
     torch.cuda.manual_seed_all(seed)
     torch.backends.cudnn.benchmark = False
     torch.backends.cudnn.deterministic = True
     return seed
 
 
-def print_trainable_parameters(module:nn.Module):
+def print_trainable_parameters(module:Module):
     '''打印可训练的参数量'''
     trainable_params = 0
     all_param = 0
     for _, param in module.named_parameters():
         num_params = param.numel()
         # if using DS Zero 3 and the weights are initialized empty
         if num_params == 0 and hasattr(param, "ds_numel"):
@@ -52,15 +62,15 @@
 def get_parameter_device(parameter):
     '''获取device, 从transformers包迁移过来'''
     try:
         return next(parameter.parameters()).device
     except StopIteration:
         # For nn.DataParallel compatibility in PyTorch 1.5
 
-        def find_tensor_attributes(module: nn.Module) -> List[Tuple[str, Tensor]]:
+        def find_tensor_attributes(module: Module) -> List[Tuple[str, Tensor]]:
             tuples = [(k, v) for k, v in module.__dict__.items() if torch.is_tensor(v)]
             return tuples
 
         gen = parameter._named_members(get_members_fn=find_tensor_attributes)
         first_tuple = next(gen)
         return first_tuple[1].device
 
@@ -178,41 +188,40 @@
     topk_idx_str = ",".join(map(str, topk_idx))
     log_info(f"SET CUDA_VISIBLE_DEVICES={topk_idx_str}")
     os.environ["CUDA_VISIBLE_DEVICES"] = topk_idx_str
 
     return topk_idx_str
 
 
-def find_tied_parameters(model: nn.Module, **kwargs):
+def find_tied_parameters(model: Module, **kwargs):
     """ copyed from accelerate
     Find the tied parameters in a given model.
 
     <Tip warning={true}>
 
     The signature accepts keyword arguments, but they are for the recursive part of this function and you should ignore
     them.
 
     </Tip>
 
     Args:
-        model (`torch.nn.Module`): The model to inspect.
+        model (`torch.Module`): The model to inspect.
 
     Returns:
         List[List[str]]: A list of lists of parameter names being all tied together.
 
-    Example:
-
-    ```py
+    Examples:
+    ```python
     >>> from collections import OrderedDict
     >>> import torch.nn as nn
 
     >>> model = nn.Sequential(OrderedDict([("linear1", nn.Linear(4, 4)), ("linear2", nn.Linear(4, 4))]))
     >>> model.linear2.weight = model.linear1.weight
     >>> find_tied_parameters(model)
-    [['linear1.weight', 'linear2.weight']]
+    ... # [['linear1.weight', 'linear2.weight']]
     ```
     """
     # Initialize result and named_parameters before recursing.
     named_parameters = kwargs.get("named_parameters", None)
     prefix = kwargs.get("prefix", "")
     result = kwargs.get("result", {})
 
@@ -315,20 +324,21 @@
 
 def argument_parse(arguments:Union[str, list, dict]=None, description='argument_parse', parse_known_args:bool=True, dot:bool=True):
     ''' 根据传入的参数接受命令行参数，生成argparse.ArgumentParser
     :param arguments: 参数设置，接受str, list, dict输入
     :param description: 描述
     :param parse_known_args: bool, 只解析命令行中认识的参数
 
-    Example
-    -----------------------
+    Examples:
+    ```python
     >>> args = argument_parse()
     >>> args = argument_parse('deepspeed')
     >>> args = argument_parse(['deepspeed'])
     >>> args = argument_parse({'deepspeed': {'type': str, 'help': 'deepspeed config path'}})
+    ```
     '''
     import argparse
     parser = argparse.ArgumentParser(description=description)
 
     if arguments is None:
         # 不预设，直接解析所有命令行参数
         arguments = [arg for arg in sys.argv[1:] if arg.startswith('-') and ('=' not in arg)]
@@ -348,8 +358,114 @@
     if parse_known_args:
         args, unknown_args = parser.parse_known_args()  # 允许其他参数不传入
     else:
         args = parser.parse_args()
     
     if dot is True:
         args = tran2dottableDict(vars(args))
-    return args
+    return args
+
+
+def cuda_empty_cache(device=None):
+    '''清理gpu显存'''
+    if torch.cuda.is_available():
+        if device is None:
+            torch.cuda.empty_cache()
+            torch.cuda.ipc_collect()
+            return
+        with torch.cuda.device(device):
+            torch.cuda.empty_cache()
+            torch.cuda.ipc_collect()
+    else:
+        log_warn_once('torch.cuda.is_available() = False')
+
+
+class WebServing(object):
+    """简单的Web接口，基于bottlepy简单封装，仅作为临时测试使用，不保证性能。
+
+    Examples:
+    ```python
+    >>> arguments = {'text': (None, True), 'n': (int, False)}
+    >>> web = WebServing(port=8864)
+    >>> web.route('/gen_synonyms', gen_synonyms, arguments)
+    >>> web.start()
+    >>> # 然后访问 http://127.0.0.1:8864/gen_synonyms?text=你好
+    ```
+    
+    ```shell
+    >>> # 依赖（如果不用 server='paste' 的话，可以不装paste库）:
+    >>> pip install bottle
+    >>> pip install paste
+    ```
+    """
+    def __init__(self, host='0.0.0.0', port=8000, server='paste'):
+
+        import bottle
+
+        self.host = host
+        self.port = port
+        self.server = server
+        self.bottle = bottle
+
+    def wraps(self, func, arguments, method='GET'):
+        """封装为接口函数
+
+        :param func: 要转换为接口的函数，需要保证输出可以json化，即需要保证 json.dumps(func(inputs)) 能被执行成功；
+        :param arguments: 声明func所需参数，其中key为参数名，value[0]为对应的转换函数（接口获取到的参数值都是字符串型），value[1]为该参数是否必须；
+        :param method: 'GET'或者'POST'。
+        """
+        def new_func():
+            outputs = {'code': 0, 'desc': u'succeeded', 'data': {}}
+            kwargs = {}
+            for key, value in arguments.items():
+                if method == 'GET':
+                    result = self.bottle.request.GET.getunicode(key)
+                else:
+                    result = self.bottle.request.POST.getunicode(key)
+                if result is None:
+                    if value[1]:
+                        outputs['code'] = 1
+                        outputs['desc'] = 'lack of "%s" argument' % key
+                        return json.dumps(outputs, ensure_ascii=False)
+                else:
+                    if value[0] is not None:
+                        result = value[0](result)
+                    kwargs[key] = result
+            try:
+                outputs['data'] = func(**kwargs)
+            except Exception as e:
+                outputs['code'] = 2
+                outputs['desc'] = str(e)
+            return json.dumps(outputs, ensure_ascii=False)
+
+        return new_func
+
+    def route(self, path, func, arguments, method='GET'):
+        """添加接口"""
+        func = self.wraps(func, arguments, method)
+        self.bottle.route(path, method=method)(func)
+
+    def start(self):
+        """启动服务"""
+        self.bottle.run(host=self.host, port=self.port, server=self.server)
+
+
+def copytree(src:str, dst:str, ignore_copy_files:str=None, dirs_exist_ok=False):
+    '''从一个文件夹copy到另一个文件夹
+    
+    :param src: str, copy from src
+    :param dst: str, copy to dst
+    '''
+    def _ignore_copy_files(path, content):
+        to_ignore = []
+        if ignore_copy_files is None:
+            return to_ignore
+        
+        for file_ in content:
+            for pattern in ignore_copy_files:
+                if re.search(pattern, file_):
+                    to_ignore.append(file_)
+        return to_ignore
+
+    if src:
+        os.makedirs(src, exist_ok=True)
+    shutil.copytree(src, dst, ignore=_ignore_copy_files, dirs_exist_ok=dirs_exist_ok)
```

### Comparing `torch4keras-0.2.2/torch4keras/snippets/monitor.py` & `torch4keras-0.2.3/torch4keras/snippets/monitor.py`

 * *Files 11% similar despite different names*

```diff
@@ -51,22 +51,23 @@
             eta_format = '%.0fus' % (eta * 1e6)
     return eta_format
 
 
 def timeit(func):
     '''装饰器, 计算函数消耗的时间
     
-    Example
-    --------------------------------------
+    Examples:
+    ```python
     >>> @timeit
     >>> def main(n=10):
-    >>>     for i in range(n):
-    >>>         time.sleep(0.01)
+    ...     for i in range(n):
+    ...         time.sleep(0.01)
 
     >>> main(10)
+    ```
     '''
     def warpper(*args, **kwargs):
         start = time.time()
         res = func(*args, **kwargs)
         end = time.time()
         consume = format_time(end - start, hhmmss=False)
         start1 = time.strftime("%Y-%m-%d %H:%M:%S", time.localtime(start))
@@ -76,24 +77,25 @@
         return res
     return warpper
 
 
 class Timeit:
     '''上下文管理器, 记录耗时/平均耗时
 
-    Example
-    ----------------------
+    Examples:
+    ```python
     >>> from torch4keras.snippets import Timeit
     >>> with Timeit() as ti:
-    >>>     for i in range(10):
-    >>>         time.sleep(0.1)
-    >>>         # ti.lap(name=i, reset=False)  # 统计累计耗时
-    >>>         # ti.lap(name=i, reset=True)  # 统计间隔耗时
-    >>>         # ti.lap(count=10, name=i, restart=True)  # 统计每段速度
-    >>>     # ti(10) # 统计速度
+    ...     for i in range(10):
+    ...         time.sleep(0.1)
+    ...         # ti.lap(name=i, reset=False)  # 统计累计耗时
+    ...         # ti.lap(name=i, reset=True)  # 统计间隔耗时
+    ...         # ti.lap(count=10, name=i, restart=True)  # 统计每段速度
+    ...     # ti(10) # 统计速度
+    ```
     '''
     def __enter__(self, template='Average speed: {:.2f}/s'):
         self.count = None
         self.start_tm = time.time()
         self.template = template
         return self
 
@@ -136,21 +138,22 @@
         self.lap()
         print()
 
 
 class Timeit2:
     '''记录耗时
 
-    Example
-    ----------------------
+    Examples:
+    ```python
     >>> ti = Timeit2()
     >>> for i in range(10):
-    >>>     time.sleep(0.1)
-    >>>     ti.lap(name=i)
+    ...     time.sleep(0.1)
+    ...     ti.lap(name=i)
     >>> ti.end() # 打印各个步骤时长
+    ```
     '''
     def __init__(self):
         self.reset()
 
     def __call__(self, *args, **kwargs):
         self.lap(*args, **kwargs)
 
@@ -181,20 +184,20 @@
 
     def end(self, verbose=1):
         for k, v in self.count.items():
             if v > 1:
                 self.cost['avg_' + k] = self.cost[k] / v
         
         if verbose > 0:
-            log_info('Cost detail')
-            pprint(self.cost)
-            print()
-
-        self.reset()
-        return self.cost
+            log_info(f'Cost detail: {self.cost}')
+            self.reset()
+        else:
+            cost = copy.deepcopy(self.cost)
+            self.reset()
+            return cost
 
 
 def send_email(mail_receivers:Union[str,list], mail_subject:str, mail_msg:str="", mail_host:str=None, 
                mail_user:str=None, mail_pwd:str=None, mail_sender:str=None):
     ''' 发送邮件(默认使用笔者自己注册的邮箱, 若含敏感信息请使用自己注册的邮箱)
 
     :param mail_subject: str, 邮件主题
@@ -231,20 +234,21 @@
     except smtplib.SMTPException as e:
         log_error('Send email error : '+str(e))
         return str(e)
 
 
 def email_when_error(receivers:Union[str,list], **configs):
     '''装饰器, 异常则发邮件
-    Example:
-    --------
+    Examples:
+    ```python
     >>> @email_when_error(receivers='tongjilibo@163.com')
     >>> def test():
-    >>>     return 1/0
+    ...     return 1/0
     >>> test()  # 调用
+    ```
     '''
     def actual_decorator(func):
         def new_func(*args, **kwargs):
             try:
                 res = func(*args, **kwargs)
             except Exception as e:
                 error_msg = traceback.format_exc()
@@ -258,17 +262,18 @@
 def watch_system_state(log_dir:str, gpu_id_list:List[int]=None, pids:Union[int,List[int]]=None, interval=1):
     '''监控system的状态
     
     :param log_dir: str, tensorboard的地址
     :param gpu_id_list: List[int], 监控的gpu
     :param pids: int/List[int], 监控的进程号
 
-    Example:
-    --------
+    Examples:
+    ```python
     >>> watch_system_state(log_dir='./system_states')
+    ```
     '''
     import psutil
     import pynvml
     from tensorboardX import SummaryWriter
 
     pynvml.nvmlInit()
     os.makedirs(log_dir, exist_ok=True)
```

### Comparing `torch4keras-0.2.2/torch4keras/trainer/accelerate.py` & `torch4keras-0.2.3/torch4keras/trainer/accelerate.py`

 * *Files identical despite different names*

### Comparing `torch4keras-0.2.2/torch4keras/trainer/base.py` & `torch4keras-0.2.3/torch4keras/trainer/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,44 +16,45 @@
 
 
 class Trainer:
     '''Trainer, 传入Module实例
 
     :param module: None/nn.Module, nn.Module()的模型实例
 
-    Example
-    -------------------
+    Examples:
+    ```python
     >>> import torch
     >>> import torch.nn as nn
     >>> import torch.optim as optim
     >>> import torchvision
     >>> from torch4keras.model import Trainer
     >>> from torch.utils.data import TensorDataset, DataLoader
-    >>> 
+     
     >>> device = 'cuda' if torch.cuda.is_available() else 'cpu'
-    >>> 
+     
     >>> # 读取数据
     >>> mnist = torchvision.datasets.MNIST(root='./', download=True)
     >>> x, y = mnist.train_data.unsqueeze(1).to(device).float() / 255.0, mnist.train_labels.to(device)
     >>> train_dataloader = DataLoader(TensorDataset(x, y), batch_size=8)
-    >>> 
+     
     >>> # 准备模型
     >>> net = torch.nn.Sequential(
-    >>>             nn.Conv2d(1, 32, kernel_size=3), nn.ReLU(),
-    >>>             nn.MaxPool2d(2, 2), 
-    >>>             nn.Conv2d(32, 64, kernel_size=3), nn.ReLU(),
-    >>>             nn.Flatten(),
-    >>>             nn.Linear(7744, 10)
-    >>>         )
-    >>> 
+    ...             nn.Conv2d(1, 32, kernel_size=3), nn.ReLU(),
+    ...             nn.MaxPool2d(2, 2), 
+    ...             nn.Conv2d(32, 64, kernel_size=3), nn.ReLU(),
+    ...             nn.Flatten(),
+    ...             nn.Linear(7744, 10)
+    ...         )
+     
     >>> model = Trainer(net.to(device))
     >>> model.compile(optimizer=optim.Adam(net.parameters()), loss=nn.CrossEntropyLoss())
-    >>>
+    
     >>> # 模型开始训练
     >>> model.fit(train_dataloader, steps_per_epoch=None, epochs=5)
+    ```
     '''
     def __init__(self, module:nn.Module=None):
         super(Trainer, self).__init__()
         self.initialize(module)
     
     def initialize(self, module:nn.Module=None):
         # 传入Module实例方式
@@ -402,19 +403,20 @@
                 mail_user_ = kwargs.get('mail_user_when_error')
                 mail_pwd_ = kwargs.get('mail_pwd_when_error')
                 mail_sender_ = kwargs.get('mail_sender_when_error')
                 send_email(mail_receivers_, mail_subject_, error_msg, mail_host=mail_host_, 
                            mail_user=mail_user_, mail_pwd=mail_pwd_, mail_sender=mail_sender_)
 
             # 训练异常则保存权重
-            if (save_ckpt_dir_when_error := kwargs.get('save_ckpt_dir_when_error')) is not None:
-                self.save_to_checkpoint(save_ckpt_dir_when_error, verbose=verbose, **kwargs)
+            if kwargs.get('save_ckpt_dir_when_error') is not None:
+                self.save_to_checkpoint(kwargs['save_ckpt_dir_when_error'], verbose=verbose, **kwargs)
 
             # 训练异常则打印当前batch
-            if (save_batch_path_when_error := kwargs.get('save_batch_path_when_error')) is not None:
+            save_batch_path_when_error = kwargs.get('save_batch_path_when_error')
+            if save_batch_path_when_error is not None:
                 os.makedirs(os.path.dirname(save_batch_path_when_error), exist_ok=True)
                 torch.save({'train_X': self.train_X.cpu(), 'train_y': self.train_y.cpu()}, save_batch_path_when_error)
             
             raise e
 
     def _fit(self, train_dataloader:DataLoader, steps_per_epoch:int=None, epochs:int=1, 
              callbacks:Union[Callback, List[Callback]]=None, verbose:int=1, **kwargs):
```

### Comparing `torch4keras-0.2.2/torch4keras/trainer/ddp.py` & `torch4keras-0.2.3/torch4keras/trainer/ddp.py`

 * *Files identical despite different names*

### Comparing `torch4keras-0.2.2/torch4keras/trainer/deepspeed.py` & `torch4keras-0.2.3/torch4keras/trainer/deepspeed.py`

 * *Files identical despite different names*

### Comparing `torch4keras-0.2.2/torch4keras/trainer/utils.py` & `torch4keras-0.2.3/torch4keras/trainer/utils.py`

 * *Files identical despite different names*

### Comparing `torch4keras-0.2.2/torch4keras.egg-info/PKG-INFO` & `torch4keras-0.2.3/torch4keras.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: torch4keras
-Version: 0.2.2
+Version: 0.2.3
 Summary: Use torch like keras
 Home-page: https://github.com/Tongjilibo/torch4keras
 Author: Tongjilibo
 License: Apache License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
-Requires-Dist: torch>1.6
 
 ![torch4keras](./docs/pics/torch4keras.png)
 
 
 [![licence](https://img.shields.io/github/license/Tongjilibo/torch4keras.svg?maxAge=3600)](https://github.com/Tongjilibo/torch4keras/blob/master/LICENSE) 
 [![GitHub release](https://img.shields.io/github/release/Tongjilibo/torch4keras.svg?maxAge=3600)](https://github.com/Tongjilibo/torch4keras/releases) 
 [![PyPI](https://img.shields.io/pypi/v/torch4keras?label=pypi%20package)](https://pypi.org/project/torch4keras/) 
@@ -76,16 +75,16 @@
 ## 3. 快速上手
 - 参考[bert4torch](https://github.com/Tongjilibo/bert4torch)的训练过程
 - 简单示例: [turorials_mnist](https://github.com/Tongjilibo/torch4keras/blob/master/examples/turorials_mnist.py)
 
 ## 4. 版本历史
 |更新日期| 版本 | 版本说明 |
 |------| ----------------- |----------- |
+|20240603|v0.2.3|去除对torch依赖,snippets部分可用；移动bert4torch中snippets|
 |20240418|v0.2.2|增加YamlConfig和IniConfig, 优化deepspeed的使用，修复`_prepare_inputs`的bug，修复断点续训`SmoothMetricsCallback`起点错误的bug, Trainer断点续训记录batch数|
 |20240317|v0.2.1.post2     |训练异常时保存权重，避免空数据集error，默认指标使用滑窗平滑，BaseModelDDP修改的更易用，mapping允许是函数更易用，Checkpoint增加save_on_train_end，增加SystemCallback，修改run_callback=False的bug, 适配build_MiniLLM_from_scratch, 修复ddp中mix_precision和torch重名的bug|
-|20240221|v0.2.0           | fit中修改.train()逻辑较少耗时|
 
 [更多版本](https://github.com/Tongjilibo/torch4keras/blob/master/docs/Update.md)
 
 ## 5. 更新历史：
 
 [更多历史](https://github.com/Tongjilibo/torch4keras/blob/master/docs/History.md)
```

### Comparing `torch4keras-0.2.2/torch4keras.egg-info/SOURCES.txt` & `torch4keras-0.2.3/torch4keras.egg-info/SOURCES.txt`

 * *Files identical despite different names*

