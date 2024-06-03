# Comparing `tmp/folx-0.2.6.tar.gz` & `tmp/folx-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "folx-0.2.6.tar", max compression
+gzip compressed data, was "folx-0.2.7.tar", max compression
```

## Comparing `folx-0.2.6.tar` & `folx-0.2.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1141 2023-12-12 15:39:39.316411 folx-0.2.6/LICENSE
--rw-r--r--   0        0        0    11302 2024-03-23 09:07:16.106122 folx-0.2.6/README.md
--rw-r--r--   0        0        0      743 2024-02-08 19:35:20.067248 folx-0.2.6/folx/__init__.py
--rw-r--r--   0        0        0     2812 2024-02-13 22:40:14.551068 folx-0.2.6/folx/ad.py
--rw-r--r--   0        0        0    13900 2024-03-15 13:17:04.011521 folx-0.2.6/folx/api.py
--rw-r--r--   0        0        0     3304 2024-04-25 12:26:02.179017 folx-0.2.6/folx/custom_hessian.py
--rw-r--r--   0        0        0    14208 2024-03-15 13:17:04.011521 folx-0.2.6/folx/hessian.py
--rw-r--r--   0        0        0    12236 2024-04-25 12:26:12.486944 folx-0.2.6/folx/interpreter.py
--rw-r--r--   0        0        0    17552 2024-04-25 12:25:16.227342 folx-0.2.6/folx/jvp.py
--rw-r--r--   0        0        0     1943 2024-03-23 09:06:28.458443 folx-0.2.6/folx/operators.py
--rw-r--r--   0        0        0     2226 2024-02-01 09:34:38.851198 folx-0.2.6/folx/tree_utils.py
--rw-r--r--   0        0        0    18755 2024-03-15 13:17:04.019521 folx-0.2.6/folx/utils.py
--rw-r--r--   0        0        0     2845 2024-02-01 09:34:38.855198 folx-0.2.6/folx/vmap.py
--rw-r--r--   0        0        0    15558 2024-04-25 12:26:12.486944 folx-0.2.6/folx/wrapped_functions.py
--rw-r--r--   0        0        0     5241 2024-02-14 16:24:35.312557 folx-0.2.6/folx/wrapper.py
--rw-r--r--   0        0        0     1388 2024-04-25 12:36:13.126698 folx-0.2.6/pyproject.toml
--rw-r--r--   0        0        0    12552 1970-01-01 00:00:00.000000 folx-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1141 2023-12-12 15:39:39.316411 folx-0.2.7/LICENSE
+-rw-r--r--   0        0        0    11302 2024-03-23 09:07:16.106122 folx-0.2.7/README.md
+-rw-r--r--   0        0        0      743 2024-02-08 19:35:20.067248 folx-0.2.7/folx/__init__.py
+-rw-r--r--   0        0        0     2812 2024-02-13 22:40:14.551068 folx-0.2.7/folx/ad.py
+-rw-r--r--   0        0        0    13963 2024-06-03 12:05:18.974563 folx-0.2.7/folx/api.py
+-rw-r--r--   0        0        0     2818 2024-04-25 14:52:22.842220 folx-0.2.7/folx/custom_hessian.py
+-rw-r--r--   0        0        0    14029 2024-06-03 12:32:10.213786 folx-0.2.7/folx/hessian.py
+-rw-r--r--   0        0        0    12236 2024-06-03 09:32:48.739210 folx-0.2.7/folx/interpreter.py
+-rw-r--r--   0        0        0    17542 2024-06-03 11:04:12.026597 folx-0.2.7/folx/jvp.py
+-rw-r--r--   0        0        0     1973 2024-04-25 13:04:03.799356 folx-0.2.7/folx/operators.py
+-rw-r--r--   0        0        0     2226 2024-02-01 09:34:38.851198 folx-0.2.7/folx/tree_utils.py
+-rw-r--r--   0        0        0    18755 2024-03-15 13:17:04.019521 folx-0.2.7/folx/utils.py
+-rw-r--r--   0        0        0     2845 2024-02-01 09:34:38.855198 folx-0.2.7/folx/vmap.py
+-rw-r--r--   0        0        0    18281 2024-06-03 12:16:47.574774 folx-0.2.7/folx/wrapped_functions.py
+-rw-r--r--   0        0        0     5241 2024-05-01 07:51:21.169929 folx-0.2.7/folx/wrapper.py
+-rw-r--r--   0        0        0     1388 2024-06-03 12:34:24.473063 folx-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0    12552 1970-01-01 00:00:00.000000 folx-0.2.7/PKG-INFO
```

### Comparing `folx-0.2.6/LICENSE` & `folx-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `folx-0.2.6/README.md` & `folx-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `folx-0.2.6/folx/__init__.py` & `folx-0.2.7/folx/__init__.py`

 * *Files identical despite different names*

### Comparing `folx-0.2.6/folx/ad.py` & `folx-0.2.7/folx/ad.py`

 * *Files identical despite different names*

### Comparing `folx-0.2.6/folx/api.py` & `folx-0.2.7/folx/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -421,16 +421,18 @@
         kwargs: dict[str, Any],
         sparsity_threshold: int,
     ) -> PyTree[ArrayOrFwdLaplArray]: ...
 
 
 class FunctionFlags(IntFlag):
     GENERAL = 0
-    LINEAR_IN_FIRST = 1
-    LINEAR_IN_ONE = 2 | LINEAR_IN_FIRST
-    LINEAR = 4 | LINEAR_IN_ONE
-    REDUCTION = 8
-    MULTIPLICATION = 16 | LINEAR_IN_ONE
-    DOT_PRODUCT = 32 | REDUCTION | MULTIPLICATION
-    INDEXING = 64 | LINEAR
-    SCATTER = 128
-    JOIN_JVP = 256
+    LINEAR_IN_FIRST = 1 << 0
+    LINEAR_IN_ONE = 1 << 1 | LINEAR_IN_FIRST
+    LINEAR = 1 << 2 | LINEAR_IN_ONE
+    REDUCTION = 1 << 3
+    MULTIPLICATION = 1 << 4 | LINEAR_IN_ONE
+    DOT_PRODUCT = 1 << 5 | REDUCTION | MULTIPLICATION
+
+    INDEXING = 1 << 6 | LINEAR
+    SCATTER = 1 << 7
+    JOIN_JVP = 1 << 8
+    SPARSE_JHJ = 1 << 9
```

### Comparing `folx-0.2.6/folx/custom_hessian.py` & `folx-0.2.7/folx/custom_hessian.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-import jax
 import jax.numpy as jnp
 
 from folx.ad import is_tree_complex
+from folx.vmap import batched_vmap
 
 from .api import Array, ExtraArgs, FwdLaplArgs, MergeFn, JAC_DIM
 from .utils import trace_of_product
 
 
 def slogdet_jac_hessian_jac(
     args: FwdLaplArgs,
@@ -26,42 +26,28 @@
     A_inv = jnp.linalg.inv(A)
     J = args.jacobian[0].construct_jac_for(materialize_idx)
     J = jnp.moveaxis(J, JAC_DIM, -1)
     leading_dims = A.shape[:-2]
     x0_dim = J.shape[-1]
 
     def elementwise(A_inv, J):
-        # Naive implementation
-        # @functools.partial(jax.vmap, in_axes=(-1, None), out_axes=-1)
-        # @functools.partial(jax.vmap, in_axes=(None, -1), out_axes=-1)
-        # def inner(v1, v2):
-        #     A_inv_v = A_inv@v1
-        #     v_A_inv = v2.T@A_inv.T
-        #     return -v_A_inv.reshape(-1)@A_inv_v.reshape(-1)
-        # vHv = inner(J, J)
-        # trace = jnp.trace(vHv)
-
         # We can do better and compute the trace more efficiently.
         A_inv_J = jnp.einsum('ij,jdk->idk', A_inv, J)
         trace = -trace_of_product(
             jnp.transpose(A_inv_J, (1, 0, 2)).reshape(-1, x0_dim),
             A_inv_J.reshape(-1, x0_dim),
         )
-        return jnp.zeros(()), trace
+        return jnp.zeros((), dtype=trace.dtype), trace
 
     A_inv = A_inv.reshape(-1, *A.shape[-2:])
     J = J.reshape(-1, *J.shape[-3:])
 
     # We can either use vmap or scan. Scan is slightly slower but uses less memory.
     # Here we assume that we will in general encounter larger determinants rather than many.
-    # signs, flat_out = jax.vmap(elementwise)(A_inv, J)
-    def scan_wrapper(_, x):
-        return None, elementwise(*x)
-
-    signs, flat_out = jax.lax.scan(scan_wrapper, None, (A_inv, J))[1]
+    signs, flat_out = batched_vmap(elementwise, 1)(A_inv, J)
     sign_out, log_abs_out = signs.reshape(leading_dims), flat_out.reshape(leading_dims)
 
     if is_tree_complex(A):
         # this is not the real Tr(JHJ^T) but a cached value we use later to compute the Tr(JHJ^T)
         return log_abs_out, log_abs_out.real
     return sign_out, log_abs_out.real
```

### Comparing `folx-0.2.6/folx/hessian.py` & `folx-0.2.7/folx/hessian.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import jax
 import jax.flatten_util as jfu
 import jax.numpy as jnp
 import jax.tree_util as jtu
 import jaxlib.xla_extension
 import numpy as np
 
+from .ad import hessian, jacrev
 from .api import (
     JAC_DIM,
     Array,
     Axes,
     CustomTraceJacHessianJac,
     ExtraArgs,
     ForwardFn,
@@ -29,15 +30,14 @@
     flat_wrap,
     get_reduced_jacobians,
     jac_jacT,
     trace_jac_jacT,
     trace_of_product,
     vmap_sequences_and_squeeze,
 )
-from .ad import hessian, jacrev
 
 
 def JHJ_via_hessian(flat_fn: Callable, flat_x: Array, grad_2d: Array):
     # We directly compute the hessian and then the trace of the product.
     flat_hessian = hessian(flat_fn)(flat_x)
     return trace_of_product(flat_hessian, grad_2d @ grad_2d.T)
 
@@ -100,17 +100,15 @@
     else:
         # Here we contract the Jacobian dimensions directly without computing the full Hessian.
         # This might be more efficient if the Jacobian is large and the Hessian is small.
         flat_out = JHJ_via_trace(flat_fn, flat_x, grad_2d)
     return unravel(flat_out)
 
 
-def off_diag_jac_hessian_jac(
-    fn: ForwardFn, args: FwdLaplArgs, materialize_idx: Array | None
-):
+def off_diag_jac_hessian_jac(fn: ForwardFn, args: FwdLaplArgs, out_idx: Array | None):
     # if we know that a function is linear in one arguments, it's hessian must be off diagonal
     # thus we can safe some computation by only computing the off diagonal part of the hessian.
     assert len(args) == 2, 'Off diag hessian only supports 2 args at the moment.'
 
     def flat_arr(x: FwdLaplArray) -> Array:
         return jfu.ravel_pytree(x.x)[0]
 
@@ -121,15 +119,15 @@
 
     hessian = jax.jacobian(jac_lhs, argnums=1)(
         flat_arr(args.arrays[0]), flat_arr(args.arrays[1])
     )
 
     flat_out = 2 * trace_of_product(
         hessian,
-        jac_jacT(args.arrays[0].jacobian, args.arrays[1].jacobian, materialize_idx),
+        jac_jacT(args.arrays[0].jacobian, args.arrays[1].jacobian, out_idx),
     )
     unravel = jfu.ravel_pytree(fn(*args.x))[1]
     return unravel(flat_out)
 
 
 def dot_product_jac_hessian_jac(
     fn: ForwardFn, args: FwdLaplArgs, shared_idx: Array | None
@@ -194,19 +192,17 @@
         lambda x: np.concatenate([x, np.full(max_size - x.size, -1, dtype=x.dtype)]),
         result,
         is_leaf=lambda x: isinstance(x, np.ndarray),
     )
     return np.asarray(result, dtype=int)
 
 
-def find_materialization_idx(
-    lapl_args: FwdLaplArgs, in_axes, flags: FunctionFlags, threshold: int
-):
+def find_out_idx(lapl_args: FwdLaplArgs, in_axes, flags: FunctionFlags, threshold: int):
     if not lapl_args.any_jacobian_weak:
-        return None
+        return None, True
     # TODO: Rewrite this!! This is quity messy and inefficient.
     # it assumes that we're only interested in the last dimension.
     with jax.ensure_compile_time_eval():
         vmap_seq, (inp,) = vmap_sequences_and_squeeze(
             ([j.mask for j in lapl_args.jacobian],),
             (
                 [
@@ -248,30 +244,34 @@
         # all arrays rather than their union.
         idx = merge_and_populate(filtered_arrs, np.intersect1d)  # type: ignore
     else:
         idx = merge_and_populate(filtered_arrs, np.union1d)  # type: ignore
     idx = np.moveaxis(idx, -1, JAC_DIM)
 
     if idx.shape[JAC_DIM] >= max_size or idx.shape[JAC_DIM] > threshold:
-        idx = None
-    return idx
+        return idx, True
+    return idx, False
 
 
-def remove_zero_entries(lapl_args: FwdLaplArgs, materialize_idx: np.ndarray | None):
-    if materialize_idx is None:
-        return lapl_args, None, None
+def remove_zero_entries(
+    lapl_args: FwdLaplArgs,
+    out_idx: np.ndarray,
+    dense_out: bool,
+):
+    if dense_out:
+        return lapl_args, out_idx, None
 
-    mask = (materialize_idx != -1).any(0)
+    mask = (out_idx != -1).any(0)
     if mask.sum() > 0.5 * mask.size:
         # this is a heuristic to avoid having unnecessary indexing overhead for
         # insufficiently sparse masks.
-        return lapl_args, materialize_idx, None
+        return lapl_args, out_idx, None
 
     indices = np.where(mask)
-    new_mat_idx = materialize_idx[(slice(None), *indices)]
+    new_mat_idx = out_idx[(slice(None), *indices)]
     new_arrs = []
     for arg in lapl_args.arrays:
         brdcast_dims = np.where(np.array(arg.x.shape) == 1)[0]
         idx = tuple(0 if i in brdcast_dims else x for i, x in enumerate(indices))
         new_arrs.append(
             FwdLaplArray(
                 x=arg.x[idx],
@@ -302,69 +302,63 @@
     # Determine output structure
     def merged_fn(*x: Array):
         return fwd(*merge(x, extra_args))
 
     out = merged_fn(*lapl_args.x)
     unravel = jfu.ravel_pytree(out)[1]
 
-    materialize_idx = find_materialization_idx(
-        lapl_args, in_axes, flags, sparsity_threshold
-    )
-    if materialize_idx is None:
+    out_idx, dense_out = find_out_idx(lapl_args, in_axes, flags, sparsity_threshold)
+
+    if dense_out and FunctionFlags.SPARSE_JHJ not in flags:
         lapl_args = lapl_args.dense
-    if materialize_idx is not None and materialize_idx.shape[JAC_DIM] == 0:
+    if out_idx is not None and out_idx.shape[JAC_DIM] == 0:
         return jnp.zeros(())
 
     # If we do a dot product (not a hadamard product) we can check for empty hessian entries
     if FunctionFlags.DOT_PRODUCT in flags and all(len(a) == 1 for a in in_axes):
-        lapl_args, materialize_idx, mask = remove_zero_entries(
-            lapl_args, materialize_idx
-        )
+        lapl_args, out_idx, mask = remove_zero_entries(lapl_args, out_idx, dense_out)
         in_axes = jtu.tree_map(lambda _: -1, in_axes)
     else:
         mask = None
 
     # Broadcast and flatten all arguments
     vmap_seq, (lapl_args, extra_args) = vmap_sequences_and_squeeze(
         (lapl_args, extra_args),
         (add_vmap_jacobian_dim(lapl_args, FwdLaplArgs(in_axes)), extra_in_axes),
     )
 
     # Hessian computation
-    def hess_transform(args: FwdLaplArgs, extra_args: ExtraArgs, materialize_idx):
+    def hess_transform(args: FwdLaplArgs, extra_args: ExtraArgs, out_idx):
         def merged_fn(*x):
             return fwd(*merge(x, extra_args))
 
         merged_fn.__name__ = fwd.__name__
 
+        if FunctionFlags.SPARSE_JHJ not in flags:
+            out_idx = None if dense_out else out_idx
+
         if custom_jac_hessian_jac is not None:
-            result = custom_jac_hessian_jac(args, extra_args, merge, materialize_idx)
+            result = custom_jac_hessian_jac(args, extra_args, merge, out_idx)
         elif FunctionFlags.MULTIPLICATION in flags:
-            result = dot_product_jac_hessian_jac(merged_fn, args, materialize_idx)
+            result = dot_product_jac_hessian_jac(merged_fn, args, out_idx)
         elif FunctionFlags.LINEAR_IN_ONE in flags:
-            result = off_diag_jac_hessian_jac(merged_fn, args, materialize_idx)
+            result = off_diag_jac_hessian_jac(merged_fn, args, out_idx)
         else:
-            result = general_jac_hessian_jac(merged_fn, args, materialize_idx)
+            result = general_jac_hessian_jac(merged_fn, args, out_idx)
         return result
 
     # TODO: this implementation also assumes that we only reduce the last dimension.
+    out_idx_ax = 1 if out_idx is not None else None
     for axes in vmap_seq[::-1]:
-        hess_transform = jax.vmap(
-            hess_transform, in_axes=(*axes, (None if materialize_idx is None else 1))
-        )
+        hess_transform = jax.vmap(hess_transform, in_axes=(*axes, out_idx_ax))
     # flatten to 1D and then unravel to the original structure
-    if mask is None:
-        flat_out = jfu.ravel_pytree(
-            hess_transform(lapl_args, extra_args, materialize_idx)
-        )[0]
-    else:
-        flat_out = hess_transform(lapl_args, extra_args, materialize_idx)
-        result = jnp.zeros_like(out).at[mask].set(flat_out)  # type: ignore
-        flat_out = jfu.ravel_pytree(result)[0]
-    return unravel(flat_out)
+    result = hess_transform(lapl_args, extra_args, out_idx)
+    if mask is not None:
+        result = jnp.zeros_like(out).at[mask].set(result)  # type: ignore
+    return unravel(jfu.ravel_pytree(result)[0])
 
 
 def get_jacobian_hessian_jacobian_trace(
     fwd: ForwardFn,
     flags: FunctionFlags,
     custom_jac_hessian_jac: CustomTraceJacHessianJac | None,
     extra_args: ExtraArgs,
```

### Comparing `folx-0.2.6/folx/interpreter.py` & `folx-0.2.7/folx/interpreter.py`

 * *Files identical despite different names*

### Comparing `folx-0.2.6/folx/jvp.py` & `folx-0.2.7/folx/jvp.py`

 * *Files 1% similar despite different names*

```diff
@@ -254,14 +254,15 @@
     extra_args: ExtraArgs,
     merge: MergeFn,
     flags: FunctionFlags,
     in_axes: Axes,
     kwargs,
     sparsity_threshold: int,
 ) -> tuple[Array, FwdJacobian, Array]:
+    updates: FwdLaplArray
     operand, scatter_indices, updates = merge(laplace_args.arrays, extra_args)  # type: ignore
     if isinstance(scatter_indices, FwdLaplArray):
         return dense_jvp(fwd, laplace_args, flags=flags, in_axes=in_axes)
     if not isinstance(updates, FwdLaplArray) and FunctionFlags.LINEAR in flags:
         # operand must be a fwdlapl array by exclusion since at least one has to be.
         y: Array = fwd(*laplace_args.x)  # type: ignore
         grad_y: FwdJacobian = operand.jacobian  # type: ignore
@@ -280,15 +281,14 @@
         or dimension_numbers.update_window_dims != ()
     ):
         logging.info(
             'Scatter: dimension numbers not supported. At the moment only segment sums are supported.'
         )
         return dense_jvp(fwd, laplace_args, flags=flags, in_axes=in_axes)
 
-    updates: FwdLaplArray = updates
     n = updates.jacobian.max_n + 1
     with jax.ensure_compile_time_eval():
         one_hot_mask = jax.nn.one_hot(
             updates.jacobian.x0_idx, n, axis=-1, dtype=jnp.int32
         ).sum(0)
         out_mask = np.array(jax.ops.segment_sum(one_hot_mask, scatter_indices[:, 0]))
         max_out = np.sum(out_mask.astype(bool), axis=-1).max()
```

### Comparing `folx-0.2.6/folx/operators.py` & `folx-0.2.7/folx/operators.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     @staticmethod
     def __call__(f):
         @jax.jit
         def laplacian(x: jax.Array):
             x_shape = x.shape
             x = x.reshape(-1)
             n = x.shape[0]
-            eye = jnp.eye(n)
+            eye = jnp.eye(n, dtype=x.dtype)
 
             def f_(x):
                 return f(x.reshape(x_shape))
 
             grad_f = jax.grad(f_)
             jacobian, dgrad_f = jax.linearize(grad_f, x)
 
@@ -66,15 +66,15 @@
 class ParallelLaplacianOperator(LaplacianOperator):
     @staticmethod
     def __call__(f):
         @jax.jit
         def laplacian(x: jax.Array):
             x = x.reshape(-1)
             n = x.shape[0]
-            eye = jnp.eye(n)
+            eye = jnp.eye(n, dtype=x.dtype)
             grad_f = jax.grad(f)
             jacobian, dgrad_f = jax.linearize(grad_f, x)
 
             laplacian = jnp.diagonal(jax.vmap(dgrad_f)(eye))
             return laplacian, jacobian
 
         return laplacian
```

### Comparing `folx-0.2.6/folx/tree_utils.py` & `folx-0.2.7/folx/tree_utils.py`

 * *Files identical despite different names*

### Comparing `folx-0.2.6/folx/utils.py` & `folx-0.2.7/folx/utils.py`

 * *Files identical despite different names*

### Comparing `folx-0.2.6/folx/vmap.py` & `folx-0.2.7/folx/vmap.py`

 * *Files identical despite different names*

### Comparing `folx-0.2.6/folx/wrapped_functions.py` & `folx-0.2.7/folx/wrapped_functions.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import functools
 import logging
 from typing import Any, Literal, ParamSpec, TypeVar, overload
 
 import jax
 import jax.numpy as jnp
 import jax.tree_util as jtu
+import numpy as np
 from jax.core import Primitive
 
 from folx.ad import is_tree_complex
 
 from .api import (
     Array,
     ArrayOrFwdLaplArray,
@@ -16,17 +17,17 @@
     FunctionFlags,
     FwdJacobian,
     FwdLaplArray,
     PyTree,
 )
 from .custom_hessian import complex_abs_jac_hessian_jac, slogdet_jac_hessian_jac
 from .wrapper import (
+    warp_without_fwd_laplacian,
     wrap_elementwise,
     wrap_forward_laplacian,
-    warp_without_fwd_laplacian,
 )
 
 R = TypeVar('R', bound=PyTree[Array])
 P = ParamSpec('P')
 
 
 @functools.partial(wrap_forward_laplacian, flags=FunctionFlags.INDEXING)
@@ -69,14 +70,21 @@
     lh_dims = tuple(range(lhs.ndim))
     rh_dims = tuple(range(rhs.ndim))
     lh_contract, rh_contract = dimension_numbers[0]
     lh_batch_dims, rh_batch_dims = dimension_numbers[1]
     lh_brdcast_dims = tuple(i for i in lh_dims if i not in lh_batch_dims + lh_contract)
     rh_brdcast_dims = tuple(i for i in rh_dims if i not in rh_batch_dims + rh_contract)
 
+    all_weak = (
+        isinstance(lhs, FwdLaplArray)
+        and isinstance(rhs, FwdLaplArray)
+        and lhs.jacobian.weak
+        and rhs.jacobian.weak
+    )
+
     left_inp = rearrange(
         (lhs,),
         dict(
             contract_dims=lh_contract,
             batch_dims=lh_batch_dims,
             brdcast_dims=lh_brdcast_dims,
             other_brdcast_dims=rh_brdcast_dims,
@@ -91,29 +99,80 @@
             brdcast_dims=rh_brdcast_dims,
             other_brdcast_dims=lh_brdcast_dims,
             rhs=True,
         ),
         sparsity_threshold=sparsity_threshold,
     )
 
+    # ====================================================================================
+    # Fast path for sparse solutions with reasonably small intermediate size
+    # ====================================================================================
+    # If the intermediate size is the same as the largest input size, we can also
+    # accelerate things by decomposing the dot product into a sum and a multiplication.
+    # This costs more memory but should generally be faster thanks to sparser operations.
+    inter_size = np.prod(jnp.broadcast_shapes(left_inp.shape, right_inp.shape))
+    in_size = max(left_inp.size, right_inp.size)
+
+    def fwd_lapl_mul_sum(
+        lhs: FwdLaplArray, rhs: FwdLaplArray, dims: tuple[int, ...] | int
+    ):
+        # Fwd Laplacian for multiply and sum
+        # lazy import to avoid circular imports
+        from .interpreter import forward_laplacian
+
+        return forward_laplacian(
+            lambda x, y: (x * y).sum(dims),
+            disable_jit=True,
+            sparsity_threshold=sparsity_threshold,
+        )(lhs, rhs)
+
+    if inter_size == in_size and all_weak:
+        neg_lh_batch_dims = tuple(np.array(lh_batch_dims) - lhs.ndim)
+        neg_rh_batch_dims = tuple(np.array(rh_batch_dims) - rhs.ndim)
+        neg_lh_contract = tuple(np.array(lh_contract) - lhs.ndim)
+        neg_rh_contract = tuple(np.array(rh_contract) - rhs.ndim)
+        if (
+            neg_lh_contract == neg_rh_contract
+            and neg_lh_batch_dims == neg_rh_batch_dims
+            and lh_brdcast_dims == tuple(range(len(lh_brdcast_dims)))
+            and rh_brdcast_dims == tuple(range(len(rh_brdcast_dims)))
+            and lh_batch_dims == tuple(sorted(lh_batch_dims))
+            and rh_batch_dims == tuple(sorted(rh_batch_dims))
+        ):
+            # The checks above do the following:
+            # * check that batch dims are identical in both
+            # * check that contract dim are identical in both
+            # * check that all brdcast dims are at the beginning
+            # * check that no transpositions are needed
+            # Special case where we can skip the transpositions
+            return fwd_lapl_mul_sum(lhs, rhs, lh_contract)  # type: ignore
+        return fwd_lapl_mul_sum(left_inp, right_inp, -1)
+
+    # ====================================================================================
+    # General solution
+    # ====================================================================================
     # this einsum is somewhat inefficient.
     # one should think about rewriting the hessian
     # computation and just use the regular dot product.
     def dot_last(lhs: Array, rhs: Array) -> Array:
         return jnp.einsum(
             '...i,...i->...',
             lhs,
             rhs,
             precision=precision,
             # This flag only exists in newer JAX versions.
             preferred_element_type=preferred_element_type,
         )
 
     result = wrap_forward_laplacian(
-        dot_last, flags=FunctionFlags.DOT_PRODUCT | FunctionFlags.JOIN_JVP, in_axes=-1
+        dot_last,
+        flags=FunctionFlags.DOT_PRODUCT
+        | FunctionFlags.JOIN_JVP
+        | FunctionFlags.SPARSE_JHJ,
+        in_axes=-1,
     )((left_inp, right_inp), {}, sparsity_threshold=sparsity_threshold)
     return result
 
 
 def dtype_conversion(
     args: tuple[ArrayOrFwdLaplArray],
     kwargs: dict[str, Any],
```

### Comparing `folx-0.2.6/folx/wrapper.py` & `folx-0.2.7/folx/wrapper.py`

 * *Files identical despite different names*

### Comparing `folx-0.2.6/pyproject.toml` & `folx-0.2.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = 'folx'
-version = '0.2.6'
+version = '0.2.7'
 description = 'Forward Laplacian for JAX'
 authors = [
     "Nicholas Gao <n.gao@tum.de>",
     "Jonas Koehler <jonas.koehler@microsoft.com>",
     "Adam Foster <adam.e.foster@microsoft.com>"
 ]
 maintainers = [
```

### Comparing `folx-0.2.6/PKG-INFO` & `folx-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: folx
-Version: 0.2.6
+Version: 0.2.7
 Summary: Forward Laplacian for JAX
 Home-page: https://github.com/microsoft/folx
 License: MIT
 Keywords: jax,laplacian,numeric
 Author: Nicholas Gao
 Author-email: n.gao@tum.de
 Maintainer: Nicholas Gao
```

