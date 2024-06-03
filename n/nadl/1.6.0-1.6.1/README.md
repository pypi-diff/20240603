# Comparing `tmp/nadl-1.6.0.tar.gz` & `tmp/nadl-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nadl-1.6.0.tar", last modified: Mon Jun  3 00:58:41 2024, max compression
+gzip compressed data, was "nadl-1.6.1.tar", last modified: Mon Jun  3 07:08:56 2024, max compression
```

## Comparing `nadl-1.6.0.tar` & `nadl-1.6.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     2302 2024-06-03 00:58:41.438956 nadl-1.6.0/pyproject.toml
--rw-r--r--   0        0        0      596 2024-04-18 21:07:32.861885 nadl-1.6.0/readme.org
--rw-r--r--   0        0        0     6148 2024-05-22 06:49:46.036737 nadl-1.6.0/src/nadl/.DS_Store
--rw-r--r--   0        0        0     2113 2024-06-03 00:58:16.366662 nadl-1.6.0/src/nadl/__init__.py
--rw-r--r--   0        0        0     8364 2024-04-22 04:28:48.528762 nadl-1.6.0/src/nadl/blocks.py
--rw-r--r--   0        0        0     5817 2024-06-03 00:53:50.075125 nadl-1.6.0/src/nadl/data.py
--rw-r--r--   0        0        0     2180 2024-04-26 22:33:55.875764 nadl-1.6.0/src/nadl/images.py
--rw-r--r--   0        0        0     3138 2024-06-02 23:05:56.484283 nadl-1.6.0/src/nadl/keys.py
--rw-r--r--   0        0        0     5135 2024-05-21 15:18:23.436274 nadl-1.6.0/src/nadl/loops.py
--rw-r--r--   0        0        0     5237 2024-05-31 22:43:38.214948 nadl-1.6.0/src/nadl/metrics.py
--rw-r--r--   0        0        0     3629 2024-04-22 04:28:48.528396 nadl-1.6.0/src/nadl/nets.py
--rw-r--r--   0        0        0     3401 2024-04-19 20:04:00.936571 nadl-1.6.0/src/nadl/preprocessing.py
--rw-r--r--   0        0        0        0 2023-12-07 01:36:32.295961 nadl-1.6.0/src/nadl/py.typed
--rw-r--r--   0        0        0     3995 2024-06-02 02:00:22.124011 nadl-1.6.0/src/nadl/states.py
--rw-r--r--   0        0        0     1108 2024-04-22 04:28:48.527949 nadl-1.6.0/src/nadl/transformers.py
--rw-r--r--   0        0        0     2814 2024-05-30 17:32:52.960495 nadl-1.6.0/src/nadl/utils.py
--rw-r--r--   0        0        0     1403 1970-01-01 00:00:00.000000 nadl-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0     2331 2024-06-03 07:08:56.574160 nadl-1.6.1/pyproject.toml
+-rw-r--r--   0        0        0      596 2024-04-18 21:07:32.861885 nadl-1.6.1/readme.org
+-rw-r--r--   0        0        0     6148 2024-05-22 06:49:46.036737 nadl-1.6.1/src/nadl/.DS_Store
+-rw-r--r--   0        0        0     2113 2024-06-03 07:08:19.351957 nadl-1.6.1/src/nadl/__init__.py
+-rw-r--r--   0        0        0     8364 2024-04-22 04:28:48.528762 nadl-1.6.1/src/nadl/blocks.py
+-rw-r--r--   0        0        0     5613 2024-06-03 07:06:30.784121 nadl-1.6.1/src/nadl/data.py
+-rw-r--r--   0        0        0     2180 2024-04-26 22:33:55.875764 nadl-1.6.1/src/nadl/images.py
+-rw-r--r--   0        0        0     3138 2024-06-02 23:05:56.484283 nadl-1.6.1/src/nadl/keys.py
+-rw-r--r--   0        0        0     5183 2024-06-03 07:05:28.574440 nadl-1.6.1/src/nadl/loops.py
+-rw-r--r--   0        0        0     5237 2024-05-31 22:43:38.214948 nadl-1.6.1/src/nadl/metrics.py
+-rw-r--r--   0        0        0     3629 2024-04-22 04:28:48.528396 nadl-1.6.1/src/nadl/nets.py
+-rw-r--r--   0        0        0     3401 2024-04-19 20:04:00.936571 nadl-1.6.1/src/nadl/preprocessing.py
+-rw-r--r--   0        0        0        0 2023-12-07 01:36:32.295961 nadl-1.6.1/src/nadl/py.typed
+-rw-r--r--   0        0        0     3995 2024-06-02 02:00:22.124011 nadl-1.6.1/src/nadl/states.py
+-rw-r--r--   0        0        0     1108 2024-04-22 04:28:48.527949 nadl-1.6.1/src/nadl/transformers.py
+-rw-r--r--   0        0        0     2814 2024-05-30 17:32:52.960495 nadl-1.6.1/src/nadl/utils.py
+-rw-r--r--   0        0        0     1403 1970-01-01 00:00:00.000000 nadl-1.6.1/PKG-INFO
```

### Comparing `nadl-1.6.0/pyproject.toml` & `nadl-1.6.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     "equinox>=0.11.4",
     "beartype>=0.18.5",
     "scikit-image>=0.23.2",
     "orbax-checkpoint>=0.5.15",
     "scikit-learn>=1.5.0",
 ]
 requires-python = ">=3.12"
-version = "1.6.0"
+version = "1.6.1"
 
 [project.readme]
 content-type = "text/plain"
 file = "readme.org"
 
 [project.license]
 text = "GPLv3"
@@ -57,14 +57,15 @@
 type = "find_links"
 
 [tool.pdm.dev-dependencies]
 dev = [
     "scipy>=1.13.1",
     "scikit-learn>=1.5.0",
     "ipdb>=0.13.13",
+    "naipyext[all]>=0.10.0",
 ]
 
 [tool.mypy]
 exclude = [
     "__pypackages__/",
     "./typings",
 ]
```

### Comparing `nadl-1.6.0/readme.org` & `nadl-1.6.1/readme.org`

 * *Files identical despite different names*

### Comparing `nadl-1.6.0/src/nadl/.DS_Store` & `nadl-1.6.1/src/nadl/.DS_Store`

 * *Files identical despite different names*

### Comparing `nadl-1.6.0/src/nadl/__init__.py` & `nadl-1.6.1/src/nadl/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
   classit,
   filter_concat,
   pformat,
   rle,
   rle_array,
 )
 
-__version__ = "1.6.0"
+__version__ = "1.6.1"
 
 __all__ = [
   "PG",
   "RESC",
   "SCALER",
   "Accuracy",
   "BaseTrainState",
```

### Comparing `nadl-1.6.0/src/nadl/blocks.py` & `nadl-1.6.1/src/nadl/blocks.py`

 * *Files identical despite different names*

### Comparing `nadl-1.6.0/src/nadl/data.py` & `nadl-1.6.1/src/nadl/data.py`

 * *Files 23% similar despite different names*

```diff
@@ -31,149 +31,145 @@
 filename : data.py
 project  : nadl
 license  : GPL-3.0+
 
 Simple dataset and dataloader.
 """
 
-from collections.abc import Callable, Iterator
+from __future__ import annotations
 
-import equinox as eqx
 import jax
 import jax.numpy as jnp
-from equinox import field, tree_at
-import numpy as np
+from equinox import Module, filter_jit, filter_vmap
+
+from typing import TYPE_CHECKING, NamedTuple
 
-from typing import NamedTuple
+import numpy as np
 
 from .keys import Keys
 from .loops import PG, RESC, PGThread
 
+if TYPE_CHECKING:
+  from collections.abc import Iterator
 
-class DState[T](NamedTuple):
+
+class DState(NamedTuple):
   """Dataloader state."""
 
-  xs: T
+  xs: jax.Array
   pad: jax.Array
-  shape: tuple[int, ...]
-  epoch: jax.Array = field(default_factory=lambda: jnp.array(0))
-  step: jax.Array = field(default_factory=lambda: jnp.array(0))
+  epoch: jax.Array | None = None
+  step: jax.Array | None = None
   name: str | None = None
 
 
 def _np_sort(x: jax.Array, axis: int | None = None) -> np.ndarray:
   """Sort the array."""
   return np.argsort(np.asarray(x), axis=axis)
 
 
-@eqx.filter_jit
+@filter_jit
 def fallback_argsort(x: jax.Array, axis: int | None = None) -> jax.Array:
   """Fallback to numpy argsort when CPU."""
   if jax.devices()[0].platform == "cpu":
     return jax.pure_callback(
       _np_sort, jax.ShapeDtypeStruct(x.shape, jnp.int32), x, axis
     )
   return x.argsort(axis=axis)
 
 
-class IdxDataloader[T](eqx.Module):
+class IdxDataloader(Module):
   """Simple index dataloader."""
 
   length: int
   pad: int
   batch_size: int
-  drop_num: int = 0
-  transform: Callable[[jax.Array], T] = eqx.field(static=True, init=False)
+  drop_num: int
 
   def __init__(
     self,
     length: int,
     batch_size: int,
     drop_last: bool = False,
-    transform: Callable[[jax.Array], T] = lambda x: x,
   ) -> None:
     """Initiate the dataloader."""
     self.length = length
-
-    if drop_last:
-      self.drop_num = self.length % batch_size
-
     length = length if not drop_last else length - length % batch_size
     pad = (batch_size - r) % batch_size if (r := length % batch_size) else 0
-    self.pad = pad = pad if pad != batch_size else 0
-
+    self.pad = pad if pad != batch_size else 0
     self.batch_size = batch_size
-    self.transform = eqx.filter_jit(transform)
+    self.drop_num = self.length % batch_size if drop_last else 0
 
-  def __call__(self, key: jax.Array | None = None) -> DState[T]:
+  def __call__(self, key: jax.Array | None = None) -> DState:
     """Get the indexes."""
     idxes = jnp.arange(self.length)
     if key is not None:
       idxes = jnp.take_along_axis(
         idxes,
         # NOTE: Fallback to numpy argsort since it has performance isssue in CPU.
         # https://github.com/google/jax/issues/10434
         fallback_argsort(jax.random.uniform(key, (self.length,))),
         axis=0,
       )
     length = self.length if not self.drop_num else self.length - self.drop_num
 
     idxes = jnp.r_[idxes, jnp.full(self.pad, -1, idxes.dtype)]
     idxes = idxes[: length + self.pad].reshape(-1, self.batch_size)
-    return DState(
-      self.transform(idxes), jnp.where(idxes == -1, 1, 0).astype(bool), idxes.shape
+    return DState(idxes, jnp.where(idxes == -1, 1, 0).astype(bool))
+
+  def __len__(self) -> int:
+    """Length of the dataloader."""
+    return self.length // self.batch_size + (
+      1 if (not self.drop_num) and self.length % self.batch_size else 0
     )
 
 
-def es_loop[T](
-  loader: IdxDataloader[T],
+def es_loop(
+  dl: IdxDataloader,
   pg: PG,
   keys: Keys | None = None,
-  epochs: int = 2,
+  epochs: int = 1,
   start_epoch: int = 1,
   prefix: str = "L",
   es: str = "E",
   ss: str = "S",
-) -> Iterator[DState[T]]:
+) -> Iterator[DState]:
   """Simple epoch loop."""
-  es, ss = f"{prefix}-{es}", f"{prefix}-{ss}"
   assert epochs > 0, "Epochs should be greater than 0."
-  if keys:
-    keys = jax.vmap(keys.reserve(epochs))
 
-  vdl = eqx.filter_jit(eqx.filter_vmap(loader, axis_size=1))
-  ds: DState[T] = vdl() if keys is None else vdl(keys(jnp.arange(epochs)))
-  ds = tree_at(lambda d: d.name, ds, prefix, is_leaf=lambda x: x is None)
+  kf = filter_jit(filter_vmap(keys.reserve(epochs))) if keys else lambda _: None
+  df = filter_jit(filter_vmap(dl, axis_size=1))
+  ds = df() if keys is None else df(kf(jnp.arange(epochs)))
 
+  steps = len(dl)
+  es, ss = f"{prefix}-{es}", f"{prefix}-{ss}"
   if es in pg.tasks:
     pg.pg.reset(pg.tasks[es], total=epochs)
   else:
     pg.add_task(es, total=epochs, res="", visible=epochs > 1)
   pg.advance(pg.tasks[es], start_epoch - 1)
   if ss in pg.tasks:
-    pg.pg.reset(pg.tasks[ss], total=ds.shape[0] * epochs, res="")
+    pg.pg.reset(pg.tasks[ss], total=steps * epochs, res="")
   else:
-    pg.add_task(ss, total=ds.shape[0] * epochs, res="")
-  pg.advance(pg.tasks[ss], (start_epoch - 1) * ds.shape[0])
+    pg.add_task(ss, total=steps * epochs, res="")
+  pg.advance(pg.tasks[ss], (start_epoch - 1) * steps)
 
-  @eqx.filter_jit
-  def _select(i: jax.Array, ii: jax.Array) -> DState[T]:
-    return tree_at(
-      lambda x: (x.epoch, x.step),
-      jax.tree.map(lambda x: x[i, ii] if isinstance(x, jax.Array) else x, ds),
-      (i + 1, i * ds.shape[0] + ii + 1),
-    )
+  @jax.jit
+  def _form(i: jax.Array, ii: jax.Array) -> tuple[jax.Array, jax.Array]:
+    return i + 1, i * steps + ii + 1
 
   with PGThread(pg.pg, pg.tasks[ss]) as pts, PGThread(pg.pg, pg.tasks[es]) as pte:
     for i in jnp.arange(start_epoch - 1, epochs):
       if epochs > 1:
         pte.completed += 1
-      for ii in jnp.arange(ds.shape[0]):
+      for ii, x, p in zip(jnp.arange(steps), ds.xs[i], ds.pad[i]):
         pts.completed += 1
-        yield _select(i, ii)
+        yield DState(x, p, *_form(i, ii), name=prefix)
+
+    pte.completed, pts.completed = _form(i, ii)
 
 
 def __test() -> None:
   """Test."""
   pg = PG.init_progress(extra_columns=(RESC,))
   keys = Keys.from_int_or_key(42)
   with pg:
```

### Comparing `nadl-1.6.0/src/nadl/images.py` & `nadl-1.6.1/src/nadl/images.py`

 * *Files identical despite different names*

### Comparing `nadl-1.6.0/src/nadl/keys.py` & `nadl-1.6.1/src/nadl/keys.py`

 * *Files identical despite different names*

### Comparing `nadl-1.6.0/src/nadl/loops.py` & `nadl-1.6.1/src/nadl/loops.py`

 * *Files 8% similar despite different names*

```diff
@@ -83,24 +83,27 @@
     self.done = Event()
     self.completed = 0
     self.res: str | None = None
     super().__init__()
 
   def run(self) -> None:
     """Run."""
+    tid = self.tid
     last_completed = 0
     wait = self.done.wait
+    advance = self.pg.advance
+    update = self.pg.update
     while not wait(0.2):
       if (completed := self.completed) != last_completed:
-        self.pg.advance(self.tid, completed - last_completed)
+        advance(self.tid, completed - last_completed)
         last_completed = completed
         if self.res is not None:
-          self.pg.update(self.tid, res=self.res)
+          update(tid, res=self.res)
           self.res = None
-    self.pg.update(self.tid, completed=self.completed, refresh=True)
+    update(self.tid, completed=self.completed, refresh=True)
 
   def __enter__(self) -> Self:
     """Enter."""
     self.start()
     return self
 
   def __exit__(
```

### Comparing `nadl-1.6.0/src/nadl/metrics.py` & `nadl-1.6.1/src/nadl/metrics.py`

 * *Files identical despite different names*

### Comparing `nadl-1.6.0/src/nadl/nets.py` & `nadl-1.6.1/src/nadl/nets.py`

 * *Files identical despite different names*

### Comparing `nadl-1.6.0/src/nadl/preprocessing.py` & `nadl-1.6.1/src/nadl/preprocessing.py`

 * *Files identical despite different names*

### Comparing `nadl-1.6.0/src/nadl/states.py` & `nadl-1.6.1/src/nadl/states.py`

 * *Files identical despite different names*

### Comparing `nadl-1.6.0/src/nadl/transformers.py` & `nadl-1.6.1/src/nadl/transformers.py`

 * *Files identical despite different names*

### Comparing `nadl-1.6.0/src/nadl/utils.py` & `nadl-1.6.1/src/nadl/utils.py`

 * *Files identical despite different names*

### Comparing `nadl-1.6.0/PKG-INFO` & `nadl-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nadl
-Version: 1.6.0
+Version: 1.6.1
 Summary: Nasy's Deep Learning Toolkit
 Author-Email: Nasy <nasyxx+python@gmail.com>, Nasy <nasyxx+dl@gmail.com>, Nasy <nasyxx+git@gmail.com>
 License: GPLv3
 Requires-Python: >=3.12
 Requires-Dist: jax>=0.4.28
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: rich>=13.7.1
```

