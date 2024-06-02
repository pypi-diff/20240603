# Comparing `tmp/ml_extra-0.1.2.tar.gz` & `tmp/ml_extra-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml_extra-0.1.2.tar", max compression
+gzip compressed data, was "ml_extra-0.1.3.tar", max compression
```

## Comparing `ml_extra-0.1.2.tar` & `ml_extra-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,23 @@
--rw-r--r--   0        0        0        0 2024-05-14 01:52:40.485035 ml_extra-0.1.2/README.md
--rw-r--r--   0        0        0        0 2024-05-14 01:52:40.485035 ml_extra-0.1.2/ml_extra/__init__.py
--rw-r--r--   0        0        0        0 2024-05-14 01:52:40.485035 ml_extra-0.1.2/ml_extra/calculations/classification_metrics.py
--rw-r--r--   0        0        0        0 2024-05-14 01:52:40.485035 ml_extra-0.1.2/ml_extra/calculations/regression_metrics.py
--rw-r--r--   0        0        0      775 2024-05-14 01:52:40.485035 ml_extra-0.1.2/ml_extra/experiments/utils.py
--rw-r--r--   0        0        0        0 2024-05-14 01:52:40.485035 ml_extra-0.1.2/ml_extra/loggers/artifacts/classfication.py
--rw-r--r--   0        0        0        0 2024-05-14 01:52:40.485035 ml_extra-0.1.2/ml_extra/loggers/artifacts/regression.py
--rw-r--r--   0        0        0     3012 2024-05-14 01:52:40.485035 ml_extra-0.1.2/ml_extra/loggers/decorators/code.py
--rw-r--r--   0        0        0     1257 2024-05-14 01:52:40.485035 ml_extra-0.1.2/ml_extra/loggers/decorators/metrics.py
--rw-r--r--   0        0        0      673 2024-05-14 01:52:40.485035 ml_extra-0.1.2/ml_extra/loggers/decorators/params.py
--rw-r--r--   0        0        0     4392 2024-05-14 01:52:40.485035 ml_extra-0.1.2/ml_extra/loggers/decorators/utils.py
--rw-r--r--   0        0        0        0 2024-05-14 01:52:40.485035 ml_extra-0.1.2/ml_extra/loggers/metrics/classification.py
--rw-r--r--   0        0        0        0 2024-05-14 01:52:40.485035 ml_extra-0.1.2/ml_extra/loggers/metrics/regression.py
--rw-r--r--   0        0        0      665 2024-05-14 01:52:40.485035 ml_extra-0.1.2/ml_extra/tests/inner_test/dummy_module.py
--rw-r--r--   0        0        0     4648 2024-05-14 01:52:40.485035 ml_extra-0.1.2/ml_extra/tests/logging_metrics.py
--rw-r--r--   0        0        0      428 2024-05-14 01:52:40.485035 ml_extra-0.1.2/ml_extra/tests/testing_classes.py
--rw-r--r--   0        0        0      387 2024-05-14 01:52:40.485035 ml_extra-0.1.2/ml_extra/tests/testing_functions.py
--rw-r--r--   0        0        0      157 2024-05-14 01:52:40.485035 ml_extra-0.1.2/ml_extra/utils/utils.py
--rw-r--r--   0        0        0      477 2024-05-14 01:52:40.489035 ml_extra-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      538 1970-01-01 00:00:00.000000 ml_extra-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-06-02 22:11:46.082927 ml_extra-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2024-06-02 22:11:46.082927 ml_extra-0.1.3/ml_extra/__init__.py
+-rw-r--r--   0        0        0     1252 2024-06-02 22:11:46.082927 ml_extra-0.1.3/ml_extra/calculations/classification_metrics.py
+-rw-r--r--   0        0        0        0 2024-06-02 22:11:46.082927 ml_extra-0.1.3/ml_extra/calculations/regression_metrics.py
+-rw-r--r--   0        0        0      775 2024-06-02 22:11:46.082927 ml_extra-0.1.3/ml_extra/experiments/utils.py
+-rw-r--r--   0        0        0     1398 2024-06-02 22:11:46.082927 ml_extra-0.1.3/ml_extra/loggers/artifacts/classfication.py
+-rw-r--r--   0        0        0        0 2024-06-02 22:11:46.082927 ml_extra-0.1.3/ml_extra/loggers/artifacts/regression.py
+-rw-r--r--   0        0        0     2255 2024-06-02 22:11:46.082927 ml_extra-0.1.3/ml_extra/loggers/decorators/artifacts.py
+-rw-r--r--   0        0        0     3016 2024-06-02 22:11:46.082927 ml_extra-0.1.3/ml_extra/loggers/decorators/code.py
+-rw-r--r--   0        0        0     1257 2024-06-02 22:11:46.082927 ml_extra-0.1.3/ml_extra/loggers/decorators/metrics.py
+-rw-r--r--   0        0        0      674 2024-06-02 22:11:46.082927 ml_extra-0.1.3/ml_extra/loggers/decorators/params.py
+-rw-r--r--   0        0        0     5725 2024-06-02 22:11:46.082927 ml_extra-0.1.3/ml_extra/loggers/decorators/utils.py
+-rw-r--r--   0        0        0        0 2024-06-02 22:11:46.082927 ml_extra-0.1.3/ml_extra/loggers/metrics/classification.py
+-rw-r--r--   0        0        0        0 2024-06-02 22:11:46.082927 ml_extra-0.1.3/ml_extra/loggers/metrics/regression.py
+-rw-r--r--   0        0        0     2336 2024-06-02 22:11:46.082927 ml_extra-0.1.3/ml_extra/plots/classification.py
+-rw-r--r--   0        0        0      391 2024-06-02 22:11:46.082927 ml_extra-0.1.3/ml_extra/plots/validations.py
+-rw-r--r--   0        0        0      665 2024-06-02 22:11:46.086927 ml_extra-0.1.3/ml_extra/tests/inner_test/dummy_module.py
+-rw-r--r--   0        0        0     4932 2024-06-02 22:11:46.086927 ml_extra-0.1.3/ml_extra/tests/logging_metrics.py
+-rw-r--r--   0        0        0      428 2024-06-02 22:11:46.086927 ml_extra-0.1.3/ml_extra/tests/testing_classes.py
+-rw-r--r--   0        0        0      388 2024-06-02 22:11:46.086927 ml_extra-0.1.3/ml_extra/tests/testing_functions.py
+-rw-r--r--   0        0        0     2261 2024-06-02 22:11:46.086927 ml_extra-0.1.3/ml_extra/utils/utils.py
+-rw-r--r--   0        0        0      520 2024-06-02 22:11:46.086927 ml_extra-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      624 1970-01-01 00:00:00.000000 ml_extra-0.1.3/PKG-INFO
```

### Comparing `ml_extra-0.1.2/ml_extra/experiments/utils.py` & `ml_extra-0.1.3/ml_extra/experiments/utils.py`

 * *Files identical despite different names*

### Comparing `ml_extra-0.1.2/ml_extra/loggers/decorators/code.py` & `ml_extra-0.1.3/ml_extra/loggers/decorators/code.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,14 +78,15 @@
         mlflow.log_text(code, module_name.replace(".", "/") + ".py")
         orig_init(self, *args, **kws)
 
     cls.__init__ = __init__
 
     return cls
 
+
 def log_module_function(func):
     """
     Log the code of the module passed as argument.
     """
 
     @wraps(func)
     def wrapper(*args, **kwargs):
@@ -96,15 +97,16 @@
         code = inspect.getsource(module)
         module_name = module.__name__
         mlflow.log_text(code, module_name.replace(".", "/") + ".py")
         return func(*args, **kwargs)
 
     return wrapper
 
-def log_module_source(module)->None:
+
+def log_module_source(module) -> None:
     """
     Log the code of the module passed as argument.
     """
 
     if not check_run():
         return
     code = inspect.getsource(module)
```

### Comparing `ml_extra-0.1.2/ml_extra/loggers/decorators/metrics.py` & `ml_extra-0.1.3/ml_extra/loggers/decorators/metrics.py`

 * *Files identical despite different names*

### Comparing `ml_extra-0.1.2/ml_extra/loggers/decorators/params.py` & `ml_extra-0.1.3/ml_extra/loggers/decorators/params.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from ml_extra.loggers.decorators.utils import check_param
 from ml_extra.loggers.decorators.utils import check_params
 from ml_extra.loggers.decorators.utils import check_run
 
 from functools import wraps
 import mlflow
 
+
 def param(func):
 
     @wraps(func)
     def wrapper(*args, **kwargs):
         if not check_run():
             return func(*args, **kwargs)
```

### Comparing `ml_extra-0.1.2/ml_extra/loggers/decorators/utils.py` & `ml_extra-0.1.3/ml_extra/loggers/decorators/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,15 +2,24 @@
 from typing import Dict
 import mlflow
 from typing import Optional
 import tempfile
 from pathlib import Path
 import inspect
 
+def check_valid_json(json: Dict) -> bool:
+    """
+    Check if the json is a dictionary with string keys and string values.
 
+    :param json: The json to check.
+    :return: True if the json is a dictionary with string keys and string values, False otherwise.
+    """
+    if isinstance(json, dict) and all(isinstance(k, str) for k in json.keys()):
+        return True
+    return False
 def check_metrics(metrics: Dict[str, float]) -> bool:
     """
     Check if the metrics are a dictionary with string keys and int/float values.
 
     :param metrics: The metrics to check.
     :return: True if the metrics are a dictionary with string keys and int/float values, False otherwise.
     """
@@ -97,14 +106,44 @@
     if not isinstance(artifact_path, str):
         raise TypeError("The artifact path must be a string.")
 
     if not artifact_path.endswith(".py"):
         return artifact_path.replace(".", "/") + ".py"
     return artifact_path
 
+def get_valid_artifact_path_for_json(artifact_path: str) -> str:
+    """
+    Get a valid artifact path for a json file.
+
+    :param artifact_path: The artifact path.
+    :return: A valid artifact path for a json file.
+    """
+    if not isinstance(artifact_path, str):
+        raise TypeError("The artifact path must be a string.")
+    suffix = artifact_path.split(".")[-1]
+    if not suffix in ["json"]:
+        return artifact_path + ".json"
+
+    return artifact_path
+
+def get_valid_artifact_path_for_yaml(artifact_path: str) -> str:
+    """
+    Get a valid artifact path for a yaml file.
+
+    :param artifact_path: The artifact path.
+    :return: A valid artifact path for a yaml file.
+    """
+    if not isinstance(artifact_path, str):
+        raise TypeError("The artifact path must be a string.")
+    suffix = artifact_path.split(".")[-1]
+    if not suffix in ["yaml", "yml"]:
+        return artifact_path + ".yaml"
+
+    return artifact_path
+
 
 def check_logged_code(run, func) -> bool:
     """
     Check if the code of the function has already been logged.
 
     :param run: The active run.
     :param func: The function to check.
```

### Comparing `ml_extra-0.1.2/ml_extra/tests/inner_test/dummy_module.py` & `ml_extra-0.1.3/ml_extra/tests/inner_test/dummy_module.py`

 * *Files identical despite different names*

### Comparing `ml_extra-0.1.2/ml_extra/tests/logging_metrics.py` & `ml_extra-0.1.3/ml_extra/tests/logging_metrics.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from ml_extra.experiments.utils import get_or_create_experiment
 from ml_extra.loggers.decorators.metrics import metric
 from ml_extra.loggers.decorators.code import log_function
 from ml_extra.loggers.decorators.code import log_function_path
 from ml_extra.loggers.decorators.code import log_module_source
+from ml_extra.loggers.decorators.artifacts import log_yaml
+from ml_extra.loggers.decorators.artifacts import log_json
 from ml_extra.tests.testing_functions import do_something
 from ml_extra.tests.testing_functions import do_something_else
 from ml_extra.tests.inner_test.dummy_module import do_something as ds
 from ml_extra.tests.inner_test.dummy_module import dummy_function
 from ml_extra.tests.testing_classes import DummyClass
 from ml_extra.tests.testing_classes import DummyClass2
 from ml_extra.tests.inner_test.dummy_module import AnotherClass
@@ -93,14 +95,22 @@
     # dst = mlflow.artifacts.download_artifacts(run_id=run_id, artifact_path="custom_code", dst_path="custom_code")
     # print(dst)
     # # add custom code to sys.path
     # sys.path.append(os.path.abspath(dst))
     # from mlflow_extra.tests.inner_test.dummy_module import do_something as ds
 
 
+@log_yaml("configs/config.yml")
+def return_config():
+    return {"a": 1, "b": 2, "c": 3, "d": {"e": 4, "f": 5}}
+
+@log_json("configs/config.json")
+def return_config2():
+    return {"a": 1, "b": 2, "c": 3, "d": {"e": 4, "f": 5}}
+
 def main():
     # print(inspect.getabsfile(dummy_module))
     # print(inspect.getsourcefile(dummy_module))
     # print(inspect.getmodule(dummy_module).__name__)
     experiment = get_or_create_experiment(name="example_experiment")
     # print(inspect.getsource(dummy_module))
 
@@ -109,28 +119,22 @@
     # print(calculate_metrics.__module__)
     # str1 = inspect.getsource(get_or_create_experiment)
     # str2 = inspect.getsource(log_code)
     # total = "\n \n".join([str1,str2])
 
     # print(total)
     # print(type(inspect.getsource(get_or_create_experiment)))
-
     with mlflow.start_run(experiment_id=experiment.experiment_id) as run:
-        custom_metric = calculate_metrics()
-        result = testing_function(1, 2)
-        print(result)
-        my_class = DummyClass()
-        my_class.say_something("Hello")
-
-        my_class2 = DummyClass2()
-        my_class2.say_something("Hello")
-
-    #     another_class = AnotherClass()
-    #     another_class.say_something("Hello")
-    #     calculate_metrics()
-    #     testing_function(1, 2)
-        do_something()
-        do_something_else()
-        log_module_source(code)
-
-    #     ds()
-    #     dummy_function()
+        # custom_metric = calculate_metrics()
+        # result = testing_function(1, 2)
+        # print(result)
+        # my_class = DummyClass()
+        # my_class.say_something("Hello")
+        config = return_config2()
+        print(config)
+        # my_class2 = DummyClass2()
+        # my_class2.say_something("Hello")
+        # config = return_config()
+        # print(config)
+        # do_something()
+        # do_something_else()
+        # log_module_source(code)
```

### Comparing `ml_extra-0.1.2/PKG-INFO` & `ml_extra-0.1.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: ml-extra
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: Manuel Gil
 Author-email: manuelgilsitio@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: coverage (>=7.5.3,<8.0.0)
 Requires-Dist: dill (>=0.3.8,<0.4.0)
 Requires-Dist: ipython (>=8.24.0,<9.0.0)
 Requires-Dist: jupyter (>=1.0.0,<2.0.0)
 Requires-Dist: mlflow (>=2.12.1,<3.0.0)
 Requires-Dist: pytest (>=8.2.0,<9.0.0)
+Requires-Dist: setuptools (>=70.0.0,<71.0.0)
 Description-Content-Type: text/markdown
```

