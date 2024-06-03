# Comparing `tmp/nadl-1.5.8.tar.gz` & `tmp/nadl-1.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nadl-1.5.8.tar", last modified: Fri May 31 22:44:44 2024, max compression
+gzip compressed data, was "nadl-1.5.9.tar", last modified: Sun Jun  2 03:12:45 2024, max compression
```

## Comparing `nadl-1.5.8.tar` & `nadl-1.5.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     2302 2024-05-31 22:44:44.812192 nadl-1.5.8/pyproject.toml
--rw-r--r--   0        0        0      596 2024-04-18 21:07:32.861885 nadl-1.5.8/readme.org
--rw-r--r--   0        0        0     6148 2024-05-22 06:49:46.036737 nadl-1.5.8/src/nadl/.DS_Store
--rw-r--r--   0        0        0     2113 2024-05-31 22:44:12.563851 nadl-1.5.8/src/nadl/__init__.py
--rw-r--r--   0        0        0     8364 2024-04-22 04:28:48.528762 nadl-1.5.8/src/nadl/blocks.py
--rw-r--r--   0        0        0     5812 2024-05-27 05:37:53.227894 nadl-1.5.8/src/nadl/data.py
--rw-r--r--   0        0        0     2180 2024-04-26 22:33:55.875764 nadl-1.5.8/src/nadl/images.py
--rw-r--r--   0        0        0     3564 2024-05-22 05:17:23.233277 nadl-1.5.8/src/nadl/keys.py
--rw-r--r--   0        0        0     5135 2024-05-21 15:18:23.436274 nadl-1.5.8/src/nadl/loops.py
--rw-r--r--   0        0        0     5237 2024-05-31 22:43:38.214948 nadl-1.5.8/src/nadl/metrics.py
--rw-r--r--   0        0        0     3629 2024-04-22 04:28:48.528396 nadl-1.5.8/src/nadl/nets.py
--rw-r--r--   0        0        0     3401 2024-04-19 20:04:00.936571 nadl-1.5.8/src/nadl/preprocessing.py
--rw-r--r--   0        0        0        0 2023-12-07 01:36:32.295961 nadl-1.5.8/src/nadl/py.typed
--rw-r--r--   0        0        0     3869 2024-05-31 22:41:24.111147 nadl-1.5.8/src/nadl/states.py
--rw-r--r--   0        0        0     1108 2024-04-22 04:28:48.527949 nadl-1.5.8/src/nadl/transformers.py
--rw-r--r--   0        0        0     2814 2024-05-30 17:32:52.960495 nadl-1.5.8/src/nadl/utils.py
--rw-r--r--   0        0        0     1403 1970-01-01 00:00:00.000000 nadl-1.5.8/PKG-INFO
+-rw-r--r--   0        0        0     2302 2024-06-02 03:12:45.074777 nadl-1.5.9/pyproject.toml
+-rw-r--r--   0        0        0      596 2024-04-18 21:07:32.861885 nadl-1.5.9/readme.org
+-rw-r--r--   0        0        0     6148 2024-05-22 06:49:46.036737 nadl-1.5.9/src/nadl/.DS_Store
+-rw-r--r--   0        0        0     2113 2024-06-02 03:12:15.539118 nadl-1.5.9/src/nadl/__init__.py
+-rw-r--r--   0        0        0     8364 2024-04-22 04:28:48.528762 nadl-1.5.9/src/nadl/blocks.py
+-rw-r--r--   0        0        0     5812 2024-05-27 05:37:53.227894 nadl-1.5.9/src/nadl/data.py
+-rw-r--r--   0        0        0     2180 2024-04-26 22:33:55.875764 nadl-1.5.9/src/nadl/images.py
+-rw-r--r--   0        0        0     3564 2024-05-22 05:17:23.233277 nadl-1.5.9/src/nadl/keys.py
+-rw-r--r--   0        0        0     5135 2024-05-21 15:18:23.436274 nadl-1.5.9/src/nadl/loops.py
+-rw-r--r--   0        0        0     5237 2024-05-31 22:43:38.214948 nadl-1.5.9/src/nadl/metrics.py
+-rw-r--r--   0        0        0     3629 2024-04-22 04:28:48.528396 nadl-1.5.9/src/nadl/nets.py
+-rw-r--r--   0        0        0     3401 2024-04-19 20:04:00.936571 nadl-1.5.9/src/nadl/preprocessing.py
+-rw-r--r--   0        0        0        0 2023-12-07 01:36:32.295961 nadl-1.5.9/src/nadl/py.typed
+-rw-r--r--   0        0        0     3995 2024-06-02 02:00:22.124011 nadl-1.5.9/src/nadl/states.py
+-rw-r--r--   0        0        0     1108 2024-04-22 04:28:48.527949 nadl-1.5.9/src/nadl/transformers.py
+-rw-r--r--   0        0        0     2814 2024-05-30 17:32:52.960495 nadl-1.5.9/src/nadl/utils.py
+-rw-r--r--   0        0        0     1403 1970-01-01 00:00:00.000000 nadl-1.5.9/PKG-INFO
```

### Comparing `nadl-1.5.8/pyproject.toml` & `nadl-1.5.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     "equinox>=0.11.4",
     "beartype>=0.18.5",
     "scikit-image>=0.23.2",
     "orbax-checkpoint>=0.5.14",
     "scikit-learn>=1.5.0",
 ]
 requires-python = ">=3.12"
-version = "1.5.8"
+version = "1.5.9"
 
 [project.readme]
 content-type = "text/plain"
 file = "readme.org"
 
 [project.license]
 text = "GPLv3"
```

### Comparing `nadl-1.5.8/readme.org` & `nadl-1.5.9/readme.org`

 * *Files identical despite different names*

### Comparing `nadl-1.5.8/src/nadl/.DS_Store` & `nadl-1.5.9/src/nadl/.DS_Store`

 * *Files identical despite different names*

### Comparing `nadl-1.5.8/src/nadl/__init__.py` & `nadl-1.5.9/src/nadl/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
   classit,
   filter_concat,
   pformat,
   rle,
   rle_array,
 )
 
-__version__ = "1.5.8"
+__version__ = "1.5.9"
 
 __all__ = [
   "PG",
   "RESC",
   "SCALER",
   "Accuracy",
   "BaseTrainState",
```

### Comparing `nadl-1.5.8/src/nadl/blocks.py` & `nadl-1.5.9/src/nadl/blocks.py`

 * *Files identical despite different names*

### Comparing `nadl-1.5.8/src/nadl/data.py` & `nadl-1.5.9/src/nadl/data.py`

 * *Files identical despite different names*

### Comparing `nadl-1.5.8/src/nadl/images.py` & `nadl-1.5.9/src/nadl/images.py`

 * *Files identical despite different names*

### Comparing `nadl-1.5.8/src/nadl/keys.py` & `nadl-1.5.9/src/nadl/keys.py`

 * *Files identical despite different names*

### Comparing `nadl-1.5.8/src/nadl/loops.py` & `nadl-1.5.9/src/nadl/loops.py`

 * *Files identical despite different names*

### Comparing `nadl-1.5.8/src/nadl/metrics.py` & `nadl-1.5.9/src/nadl/metrics.py`

 * *Files identical despite different names*

### Comparing `nadl-1.5.8/src/nadl/nets.py` & `nadl-1.5.9/src/nadl/nets.py`

 * *Files identical despite different names*

### Comparing `nadl-1.5.8/src/nadl/preprocessing.py` & `nadl-1.5.9/src/nadl/preprocessing.py`

 * *Files identical despite different names*

### Comparing `nadl-1.5.8/src/nadl/states.py` & `nadl-1.5.9/src/nadl/states.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,14 +52,16 @@
 
   import jax
 
   from jaxtyping import PyTree
 
   from rich.console import Console
 
+  from .metrics import Metric
+
 
 class BaseTrainState[T, M](eqx.Module):
   """Train state."""
 
   model: M
   tx: optax.GradientTransformation
   opt_state: optax.OptState
@@ -93,23 +95,24 @@
   console: Console | None = None,
   keeps: int = 5,
   clean: bool = False,
   item_names: tuple[str, ...] | None = None,
   item_handlers: dict | None = None,
   best_fn: Callable[[PyTree], float] | None = None,
 ) -> tuple[
-  ocp.CheckpointManager, Callable[[int, BaseTrainState, dict[str, float] | None], None]
+  ocp.CheckpointManager,
+  Callable[[int, BaseTrainState, Metric | None, dict[str, float] | None], None],
 ]:
   """Get states manager."""
   match (item_names, item_handlers):
     case (None, None):
       item_names = ("state", "extra_metadata")
       item_handlers = {
         "state": ocp.PyTreeCheckpointHandler(),
-        "extra_metadata": ocp.JsonCheckpointHandler(),
+        "extra_metadata": ocp.PyTreeCheckpointHandler(),
       }
     case _ if item_names and item_handlers:
       for i in item_names:
         assert i in item_handlers, f"Item {i} not in item_handlers."
     case _:
       raise ValueError("item_names and item_handlers should be both None or not None.")
 
@@ -126,19 +129,23 @@
       max_to_keep=keeps, save_interval_steps=1, best_fn=best_fn
     ),
     item_names=item_names,
     item_handlers=item_handlers,
   )
 
   def save(
-    step: int, state: BaseTrainState, metadata: dict[str, float] | None = None
+    step: int,
+    state: BaseTrainState,
+    metadata: Metric | None = None,
+    metrics: dict[str, float] | None = None,
   ) -> None:
     """Save state."""
     mngr.save(
       step,
       args=ocp.args.Composite(
         state=ocp.args.PyTreeSave(state),  # type: ignore
-        extra_metadata=ocp.args.JsonSave(metadata or {}),  # type: ignore
+        extra_metadata=ocp.args.PyTreeSave(metadata or {}),  # type: ignore
       ),
+      metrics=metrics or {},
     )
 
   return mngr, save
```

### Comparing `nadl-1.5.8/src/nadl/transformers.py` & `nadl-1.5.9/src/nadl/transformers.py`

 * *Files identical despite different names*

### Comparing `nadl-1.5.8/src/nadl/utils.py` & `nadl-1.5.9/src/nadl/utils.py`

 * *Files identical despite different names*

### Comparing `nadl-1.5.8/PKG-INFO` & `nadl-1.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nadl
-Version: 1.5.8
+Version: 1.5.9
 Summary: Nasy's Deep Learning Toolkit
 Author-Email: Nasy <nasyxx+python@gmail.com>, Nasy <nasyxx+dl@gmail.com>, Nasy <nasyxx+git@gmail.com>
 License: GPLv3
 Requires-Python: >=3.12
 Requires-Dist: jax>=0.4.28
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: rich>=13.7.1
```

