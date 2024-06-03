# Comparing `tmp/nadl-1.5.9.tar.gz` & `tmp/nadl-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nadl-1.5.9.tar", last modified: Sun Jun  2 03:12:45 2024, max compression
+gzip compressed data, was "nadl-1.6.0.tar", last modified: Mon Jun  3 00:58:41 2024, max compression
```

## Comparing `nadl-1.5.9.tar` & `nadl-1.6.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     2302 2024-06-02 03:12:45.074777 nadl-1.5.9/pyproject.toml
--rw-r--r--   0        0        0      596 2024-04-18 21:07:32.861885 nadl-1.5.9/readme.org
--rw-r--r--   0        0        0     6148 2024-05-22 06:49:46.036737 nadl-1.5.9/src/nadl/.DS_Store
--rw-r--r--   0        0        0     2113 2024-06-02 03:12:15.539118 nadl-1.5.9/src/nadl/__init__.py
--rw-r--r--   0        0        0     8364 2024-04-22 04:28:48.528762 nadl-1.5.9/src/nadl/blocks.py
--rw-r--r--   0        0        0     5812 2024-05-27 05:37:53.227894 nadl-1.5.9/src/nadl/data.py
--rw-r--r--   0        0        0     2180 2024-04-26 22:33:55.875764 nadl-1.5.9/src/nadl/images.py
--rw-r--r--   0        0        0     3564 2024-05-22 05:17:23.233277 nadl-1.5.9/src/nadl/keys.py
--rw-r--r--   0        0        0     5135 2024-05-21 15:18:23.436274 nadl-1.5.9/src/nadl/loops.py
--rw-r--r--   0        0        0     5237 2024-05-31 22:43:38.214948 nadl-1.5.9/src/nadl/metrics.py
--rw-r--r--   0        0        0     3629 2024-04-22 04:28:48.528396 nadl-1.5.9/src/nadl/nets.py
--rw-r--r--   0        0        0     3401 2024-04-19 20:04:00.936571 nadl-1.5.9/src/nadl/preprocessing.py
--rw-r--r--   0        0        0        0 2023-12-07 01:36:32.295961 nadl-1.5.9/src/nadl/py.typed
--rw-r--r--   0        0        0     3995 2024-06-02 02:00:22.124011 nadl-1.5.9/src/nadl/states.py
--rw-r--r--   0        0        0     1108 2024-04-22 04:28:48.527949 nadl-1.5.9/src/nadl/transformers.py
--rw-r--r--   0        0        0     2814 2024-05-30 17:32:52.960495 nadl-1.5.9/src/nadl/utils.py
--rw-r--r--   0        0        0     1403 1970-01-01 00:00:00.000000 nadl-1.5.9/PKG-INFO
+-rw-r--r--   0        0        0     2302 2024-06-03 00:58:41.438956 nadl-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0      596 2024-04-18 21:07:32.861885 nadl-1.6.0/readme.org
+-rw-r--r--   0        0        0     6148 2024-05-22 06:49:46.036737 nadl-1.6.0/src/nadl/.DS_Store
+-rw-r--r--   0        0        0     2113 2024-06-03 00:58:16.366662 nadl-1.6.0/src/nadl/__init__.py
+-rw-r--r--   0        0        0     8364 2024-04-22 04:28:48.528762 nadl-1.6.0/src/nadl/blocks.py
+-rw-r--r--   0        0        0     5817 2024-06-03 00:53:50.075125 nadl-1.6.0/src/nadl/data.py
+-rw-r--r--   0        0        0     2180 2024-04-26 22:33:55.875764 nadl-1.6.0/src/nadl/images.py
+-rw-r--r--   0        0        0     3138 2024-06-02 23:05:56.484283 nadl-1.6.0/src/nadl/keys.py
+-rw-r--r--   0        0        0     5135 2024-05-21 15:18:23.436274 nadl-1.6.0/src/nadl/loops.py
+-rw-r--r--   0        0        0     5237 2024-05-31 22:43:38.214948 nadl-1.6.0/src/nadl/metrics.py
+-rw-r--r--   0        0        0     3629 2024-04-22 04:28:48.528396 nadl-1.6.0/src/nadl/nets.py
+-rw-r--r--   0        0        0     3401 2024-04-19 20:04:00.936571 nadl-1.6.0/src/nadl/preprocessing.py
+-rw-r--r--   0        0        0        0 2023-12-07 01:36:32.295961 nadl-1.6.0/src/nadl/py.typed
+-rw-r--r--   0        0        0     3995 2024-06-02 02:00:22.124011 nadl-1.6.0/src/nadl/states.py
+-rw-r--r--   0        0        0     1108 2024-04-22 04:28:48.527949 nadl-1.6.0/src/nadl/transformers.py
+-rw-r--r--   0        0        0     2814 2024-05-30 17:32:52.960495 nadl-1.6.0/src/nadl/utils.py
+-rw-r--r--   0        0        0     1403 1970-01-01 00:00:00.000000 nadl-1.6.0/PKG-INFO
```

### Comparing `nadl-1.5.9/pyproject.toml` & `nadl-1.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -12,19 +12,19 @@
     "numpy>=1.26.4",
     "rich>=13.7.1",
     "jaxtyping>=0.2.29",
     "optax>=0.2.2",
     "equinox>=0.11.4",
     "beartype>=0.18.5",
     "scikit-image>=0.23.2",
-    "orbax-checkpoint>=0.5.14",
+    "orbax-checkpoint>=0.5.15",
     "scikit-learn>=1.5.0",
 ]
 requires-python = ">=3.12"
-version = "1.5.9"
+version = "1.6.0"
 
 [project.readme]
 content-type = "text/plain"
 file = "readme.org"
 
 [project.license]
 text = "GPLv3"
```

### Comparing `nadl-1.5.9/readme.org` & `nadl-1.6.0/readme.org`

 * *Files identical despite different names*

### Comparing `nadl-1.5.9/src/nadl/.DS_Store` & `nadl-1.6.0/src/nadl/.DS_Store`

 * *Files identical despite different names*

### Comparing `nadl-1.5.9/src/nadl/__init__.py` & `nadl-1.6.0/src/nadl/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
   classit,
   filter_concat,
   pformat,
   rle,
   rle_array,
 )
 
-__version__ = "1.5.9"
+__version__ = "1.6.0"
 
 __all__ = [
   "PG",
   "RESC",
   "SCALER",
   "Accuracy",
   "BaseTrainState",
```

### Comparing `nadl-1.5.9/src/nadl/blocks.py` & `nadl-1.6.0/src/nadl/blocks.py`

 * *Files identical despite different names*

### Comparing `nadl-1.5.9/src/nadl/data.py` & `nadl-1.6.0/src/nadl/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,14 @@
     length = length if not drop_last else length - length % batch_size
     pad = (batch_size - r) % batch_size if (r := length % batch_size) else 0
     self.pad = pad = pad if pad != batch_size else 0
 
     self.batch_size = batch_size
     self.transform = eqx.filter_jit(transform)
 
-  @eqx.filter_jit
   def __call__(self, key: jax.Array | None = None) -> DState[T]:
     """Get the indexes."""
     idxes = jnp.arange(self.length)
     if key is not None:
       idxes = jnp.take_along_axis(
         idxes,
         # NOTE: Fallback to numpy argsort since it has performance isssue in CPU.
@@ -135,15 +134,15 @@
   es: str = "E",
   ss: str = "S",
 ) -> Iterator[DState[T]]:
   """Simple epoch loop."""
   es, ss = f"{prefix}-{es}", f"{prefix}-{ss}"
   assert epochs > 0, "Epochs should be greater than 0."
   if keys:
-    keys.reserve(epochs)
+    keys = jax.vmap(keys.reserve(epochs))
 
   vdl = eqx.filter_jit(eqx.filter_vmap(loader, axis_size=1))
   ds: DState[T] = vdl() if keys is None else vdl(keys(jnp.arange(epochs)))
   ds = tree_at(lambda d: d.name, ds, prefix, is_leaf=lambda x: x is None)
 
   if es in pg.tasks:
     pg.pg.reset(pg.tasks[es], total=epochs)
@@ -178,17 +177,17 @@
   pg = PG.init_progress(extra_columns=(RESC,))
   keys = Keys.from_int_or_key(42)
   with pg:
     pg.console.print("Drop Last: False, Auto Pad: True")
     dl = IdxDataloader(314430, 256, drop_last=False)
 
     for i in es_loop(dl, pg, epochs=300, keys=keys, prefix="DFAT", start_epoch=10):
-      pg.update_res(
-        "DFAT-S", {"epoch": i.epoch.item(), "step": i.step.item(), "name": i.name}
-      )
+      # pg.update_res(
+      #   "DFAT-S", {"epoch": i.epoch.item(), "step": i.step.item(), "name": i.name}
+      # )
       continue
     pg.console.print(i)
     pg.console.print("Drop Last: True, Auto Pad: True")
     dl = IdxDataloader(10, 3, drop_last=True)
     for i in es_loop(dl, pg, keys, prefix="DTAT"):
       pg.console.print(i)
```

### Comparing `nadl-1.5.9/src/nadl/images.py` & `nadl-1.6.0/src/nadl/images.py`

 * *Files identical despite different names*

### Comparing `nadl-1.5.9/src/nadl/loops.py` & `nadl-1.6.0/src/nadl/loops.py`

 * *Files identical despite different names*

### Comparing `nadl-1.5.9/src/nadl/metrics.py` & `nadl-1.6.0/src/nadl/metrics.py`

 * *Files identical despite different names*

### Comparing `nadl-1.5.9/src/nadl/nets.py` & `nadl-1.6.0/src/nadl/nets.py`

 * *Files identical despite different names*

### Comparing `nadl-1.5.9/src/nadl/preprocessing.py` & `nadl-1.6.0/src/nadl/preprocessing.py`

 * *Files identical despite different names*

### Comparing `nadl-1.5.9/src/nadl/states.py` & `nadl-1.6.0/src/nadl/states.py`

 * *Files identical despite different names*

### Comparing `nadl-1.5.9/src/nadl/transformers.py` & `nadl-1.6.0/src/nadl/transformers.py`

 * *Files identical despite different names*

### Comparing `nadl-1.5.9/src/nadl/utils.py` & `nadl-1.6.0/src/nadl/utils.py`

 * *Files identical despite different names*

### Comparing `nadl-1.5.9/PKG-INFO` & `nadl-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: nadl
-Version: 1.5.9
+Version: 1.6.0
 Summary: Nasy's Deep Learning Toolkit
 Author-Email: Nasy <nasyxx+python@gmail.com>, Nasy <nasyxx+dl@gmail.com>, Nasy <nasyxx+git@gmail.com>
 License: GPLv3
 Requires-Python: >=3.12
 Requires-Dist: jax>=0.4.28
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: rich>=13.7.1
 Requires-Dist: jaxtyping>=0.2.29
 Requires-Dist: optax>=0.2.2
 Requires-Dist: equinox>=0.11.4
 Requires-Dist: beartype>=0.18.5
 Requires-Dist: scikit-image>=0.23.2
-Requires-Dist: orbax-checkpoint>=0.5.14
+Requires-Dist: orbax-checkpoint>=0.5.15
 Requires-Dist: scikit-learn>=1.5.0
 Requires-Dist: mkdocs-material>=9.5.25; extra == "doc"
 Requires-Dist: mkdocs>=1.6.0; extra == "doc"
 Requires-Dist: mike>=2.1.1; extra == "doc"
 Requires-Dist: mkdocstrings[python]>=0.25.1; extra == "doc"
 Provides-Extra: doc
 Description-Content-Type: text/plain
```

