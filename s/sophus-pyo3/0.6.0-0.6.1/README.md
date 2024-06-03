# Comparing `tmp/sophus_pyo3-0.6.0.tar.gz` & `tmp/sophus_pyo3-0.6.1.tar.gz`

## Comparing `sophus_pyo3-0.6.0.tar` & `sophus_pyo3-0.6.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0     1001      127      507 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_core/Cargo.toml
--rw-r--r--   0     1001      127    48009 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_core/src/calculus/dual/dual_matrix.rs
--rw-r--r--   0     1001      127    46150 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_core/src/calculus/dual/dual_scalar.rs
--rw-r--r--   0     1001      127    36168 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_core/src/calculus/dual/dual_vector.rs
--rw-r--r--   0     1001      127      485 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_core/src/calculus/dual.rs
--rw-r--r--   0     1001      127       35 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_core/src/calculus/manifold.rs
--rw-r--r--   0     1001      127     7425 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_core/src/calculus/maps/curves.rs
--rw-r--r--   0     1001      127    10602 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_core/src/calculus/maps/matrix_valued_maps.rs
--rw-r--r--   0     1001      127     7706 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_core/src/calculus/maps/scalar_valued_maps.rs
--rw-r--r--   0     1001      127    11249 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_core/src/calculus/maps/vector_valued_maps.rs
--rw-r--r--   0     1001      127     1035 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_core/src/calculus/maps.rs
--rw-r--r--   0     1001      127    11449 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_core/src/calculus/region.rs
--rw-r--r--   0     1001      127    12753 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_core/src/calculus/spline/spline_segment.rs
--rw-r--r--   0     1001      127     8135 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_core/src/calculus/spline.rs
--rw-r--r--   0     1001      127      531 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_core/src/calculus.rs
--rw-r--r--   0     1001      127     1787 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_core/src/lib.rs
--rw-r--r--   0     1001      127     1562 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_core/src/linalg/bool_mask.rs
--rw-r--r--   0     1001      127    12433 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_core/src/linalg/matrix.rs
--rw-r--r--   0     1001      127    16897 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_core/src/linalg/scalar.rs
--rw-r--r--   0     1001      127     9619 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_core/src/linalg/vector.rs
--rw-r--r--   0     1001      127     3245 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_core/src/linalg.rs
--rw-r--r--   0     1001      127     1532 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_core/src/manifold/traits.rs
--rw-r--r--   0     1001      127       30 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_core/src/manifold.rs
--rw-r--r--   0     1001      127     1509 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_core/src/params.rs
--rw-r--r--   0     1001      127     2871 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_core/src/points.rs
--rw-r--r--   0     1001      127    15058 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_core/src/tensor/arc_tensor.rs
--rw-r--r--   0     1001      127     4747 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_core/src/tensor/element.rs
--rw-r--r--   0     1001      127    18816 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_core/src/tensor/mut_tensor.rs
--rw-r--r--   0     1001      127     9210 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_core/src/tensor/mut_tensor_view.rs
--rw-r--r--   0     1001      127    14599 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_core/src/tensor/tensor_view.rs
--rw-r--r--   0     1001      127      441 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_core/src/tensor.rs
--rw-r--r--   0     1001      127      329 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/README.md
--rw-r--r--   0     1001      127      432 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_lie/Cargo.toml
--rw-r--r--   0     1001      127     6405 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_lie/src/factor_lie_group.rs
--rw-r--r--   0     1001      127     1636 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_lie/src/groups/isometry2.rs
--rw-r--r--   0     1001      127     1619 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_lie/src/groups/isometry3.rs
--rw-r--r--   0     1001      127    11299 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_lie/src/groups/rotation2.rs
--rw-r--r--   0     1001      127    22900 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_lie/src/groups/rotation3.rs
--rw-r--r--   0     1001      127    16984 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_lie/src/groups/translation_product_product.rs
--rw-r--r--   0     1001      127      202 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_lie/src/groups.rs
--rw-r--r--   0     1001      127      780 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_lie/src/lib.rs
--rw-r--r--   0     1001      127    11209 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_lie/src/lie_group.rs
--rw-r--r--   0     1001      127     2970 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_lie/src/lie_group_manifold.rs
--rw-r--r--   0     1001      127    22904 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_lie/src/real_lie_group.rs
--rw-r--r--   0     1001      127     9193 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_lie/src/traits.rs
--rw-r--r--   0        0        0      569 1970-01-01 00:00:00.000000 sophus_pyo3-0.6.0/crates/sophus_pyo3/Cargo.toml
--rw-r--r--   0     1001      127      693 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_pyo3/src/lib.rs
--rw-r--r--   0     1001      127     1249 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_pyo3/src/pyo3/errors.rs
--rw-r--r--   0     1001      127    15284 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_pyo3/src/pyo3/lie_groups.rs
--rw-r--r--   0     1001      127       70 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_pyo3/src/pyo3.rs
--rw-r--r--   0     1001      127   123832 2024-05-26 00:38:59.000000 sophus_pyo3-0.6.0/Cargo.lock
--rw-r--r--   0        0        0     1603 1970-01-01 00:00:00.000000 sophus_pyo3-0.6.0/Cargo.toml
--rw-r--r--   0        0        0      281 1970-01-01 00:00:00.000000 sophus_pyo3-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      637 1970-01-01 00:00:00.000000 sophus_pyo3-0.6.0/PKG-INFO
+-rw-r--r--   0     1001      127      432 2024-06-03 01:33:06.000000 sophus_pyo3-0.6.1/crates/sophus_lie/Cargo.toml
+-rw-r--r--   0     1001      127     6405 2024-06-03 01:33:06.000000 sophus_pyo3-0.6.1/crates/sophus_lie/src/factor_lie_group.rs
+-rw-r--r--   0     1001      127     1636 2024-06-03 01:33:06.000000 sophus_pyo3-0.6.1/crates/sophus_lie/src/groups/isometry2.rs
+-rw-r--r--   0     1001      127     1619 2024-06-03 01:33:06.000000 sophus_pyo3-0.6.1/crates/sophus_lie/src/groups/isometry3.rs
+-rw-r--r--   0     1001      127    11299 2024-06-03 01:33:06.000000 sophus_pyo3-0.6.1/crates/sophus_lie/src/groups/rotation2.rs
+-rw-r--r--   0     1001      127    22900 2024-06-03 01:33:06.000000 sophus_pyo3-0.6.1/crates/sophus_lie/src/groups/rotation3.rs
+-rw-r--r--   0     1001      127    16984 2024-06-03 01:33:06.000000 sophus_pyo3-0.6.1/crates/sophus_lie/src/groups/translation_product_product.rs
+-rw-r--r--   0     1001      127      202 2024-06-03 01:33:06.000000 sophus_pyo3-0.6.1/crates/sophus_lie/src/groups.rs
+-rw-r--r--   0     1001      127      780 2024-06-03 01:33:06.000000 sophus_pyo3-0.6.1/crates/sophus_lie/src/lib.rs
+-rw-r--r--   0     1001      127    11209 2024-06-03 01:33:06.000000 sophus_pyo3-0.6.1/crates/sophus_lie/src/lie_group.rs
+-rw-r--r--   0     1001      127     2970 2024-06-03 01:33:06.000000 sophus_pyo3-0.6.1/crates/sophus_lie/src/lie_group_manifold.rs
+-rw-r--r--   0     1001      127    22904 2024-06-03 01:33:06.000000 sophus_pyo3-0.6.1/crates/sophus_lie/src/real_lie_group.rs
+-rw-r--r--   0     1001      127     9193 2024-06-03 01:33:06.000000 sophus_pyo3-0.6.1/crates/sophus_lie/src/traits.rs
+-rw-r--r--   0     1001      127      329 2024-06-03 01:33:06.000000 sophus_pyo3-0.6.1/README.md
+-rw-r--r--   0     1001      127      507 2024-06-03 01:33:06.000000 sophus_pyo3-0.6.1/crates/sophus_core/Cargo.toml
+-rw-r--r--   0     1001      127    48009 2024-06-03 01:33:06.000000 sophus_pyo3-0.6.1/crates/sophus_core/src/calculus/dual/dual_matrix.rs
+-rw-r--r--   0     1001      127    46150 2024-06-03 01:33:06.000000 sophus_pyo3-0.6.1/crates/sophus_core/src/calculus/dual/dual_scalar.rs
+-rw-r--r--   0     1001      127    36168 2024-06-03 01:33:06.000000 sophus_pyo3-0.6.1/crates/sophus_core/src/calculus/dual/dual_vector.rs
+-rw-r--r--   0     1001      127      485 2024-06-03 01:33:06.000000 sophus_pyo3-0.6.1/crates/sophus_core/src/calculus/dual.rs
+-rw-r--r--   0     1001      127       35 2024-06-03 01:33:06.000000 sophus_pyo3-0.6.1/crates/sophus_core/src/calculus/manifold.rs
+-rw-r--r--   0     1001      127     7425 2024-06-03 01:33:06.000000 sophus_pyo3-0.6.1/crates/sophus_core/src/calculus/maps/curves.rs
+-rw-r--r--   0     1001      127    10602 2024-06-03 01:33:06.000000 sophus_pyo3-0.6.1/crates/sophus_core/src/calculus/maps/matrix_valued_maps.rs
+-rw-r--r--   0     1001      127     7706 2024-06-03 01:33:06.000000 sophus_pyo3-0.6.1/crates/sophus_core/src/calculus/maps/scalar_valued_maps.rs
+-rw-r--r--   0     1001      127    11249 2024-06-03 01:33:06.000000 sophus_pyo3-0.6.1/crates/sophus_core/src/calculus/maps/vector_valued_maps.rs
+-rw-r--r--   0     1001      127     1035 2024-06-03 01:33:06.000000 sophus_pyo3-0.6.1/crates/sophus_core/src/calculus/maps.rs
+-rw-r--r--   0     1001      127    11449 2024-06-03 01:33:06.000000 sophus_pyo3-0.6.1/crates/sophus_core/src/calculus/region.rs
+-rw-r--r--   0     1001      127    12753 2024-06-03 01:33:06.000000 sophus_pyo3-0.6.1/crates/sophus_core/src/calculus/spline/spline_segment.rs
+-rw-r--r--   0     1001      127     8135 2024-06-03 01:33:06.000000 sophus_pyo3-0.6.1/crates/sophus_core/src/calculus/spline.rs
+-rw-r--r--   0     1001      127      531 2024-06-03 01:33:06.000000 sophus_pyo3-0.6.1/crates/sophus_core/src/calculus.rs
+-rw-r--r--   0     1001      127     2855 2024-06-03 01:33:06.000000 sophus_pyo3-0.6.1/crates/sophus_core/src/lib.rs
+-rw-r--r--   0     1001      127     1562 2024-06-03 01:33:06.000000 sophus_pyo3-0.6.1/crates/sophus_core/src/linalg/bool_mask.rs
+-rw-r--r--   0     1001      127    12433 2024-06-03 01:33:06.000000 sophus_pyo3-0.6.1/crates/sophus_core/src/linalg/matrix.rs
+-rw-r--r--   0     1001      127    16897 2024-06-03 01:33:06.000000 sophus_pyo3-0.6.1/crates/sophus_core/src/linalg/scalar.rs
+-rw-r--r--   0     1001      127     9619 2024-06-03 01:33:06.000000 sophus_pyo3-0.6.1/crates/sophus_core/src/linalg/vector.rs
+-rw-r--r--   0     1001      127     3245 2024-06-03 01:33:06.000000 sophus_pyo3-0.6.1/crates/sophus_core/src/linalg.rs
+-rw-r--r--   0     1001      127     1532 2024-06-03 01:33:06.000000 sophus_pyo3-0.6.1/crates/sophus_core/src/manifold/traits.rs
+-rw-r--r--   0     1001      127       30 2024-06-03 01:33:06.000000 sophus_pyo3-0.6.1/crates/sophus_core/src/manifold.rs
+-rw-r--r--   0     1001      127     1509 2024-06-03 01:33:06.000000 sophus_pyo3-0.6.1/crates/sophus_core/src/params.rs
+-rw-r--r--   0     1001      127     2871 2024-06-03 01:33:06.000000 sophus_pyo3-0.6.1/crates/sophus_core/src/points.rs
+-rw-r--r--   0     1001      127    15058 2024-06-03 01:33:06.000000 sophus_pyo3-0.6.1/crates/sophus_core/src/tensor/arc_tensor.rs
+-rw-r--r--   0     1001      127     4747 2024-06-03 01:33:06.000000 sophus_pyo3-0.6.1/crates/sophus_core/src/tensor/element.rs
+-rw-r--r--   0     1001      127    18816 2024-06-03 01:33:06.000000 sophus_pyo3-0.6.1/crates/sophus_core/src/tensor/mut_tensor.rs
+-rw-r--r--   0     1001      127     9210 2024-06-03 01:33:06.000000 sophus_pyo3-0.6.1/crates/sophus_core/src/tensor/mut_tensor_view.rs
+-rw-r--r--   0     1001      127    14596 2024-06-03 01:33:06.000000 sophus_pyo3-0.6.1/crates/sophus_core/src/tensor/tensor_view.rs
+-rw-r--r--   0     1001      127      441 2024-06-03 01:33:06.000000 sophus_pyo3-0.6.1/crates/sophus_core/src/tensor.rs
+-rw-r--r--   0        0        0      569 1970-01-01 00:00:00.000000 sophus_pyo3-0.6.1/crates/sophus_pyo3/Cargo.toml
+-rw-r--r--   0     1001      127      693 2024-06-03 01:33:06.000000 sophus_pyo3-0.6.1/crates/sophus_pyo3/src/lib.rs
+-rw-r--r--   0     1001      127     1249 2024-06-03 01:33:06.000000 sophus_pyo3-0.6.1/crates/sophus_pyo3/src/pyo3/errors.rs
+-rw-r--r--   0     1001      127    15284 2024-06-03 01:33:06.000000 sophus_pyo3-0.6.1/crates/sophus_pyo3/src/pyo3/lie_groups.rs
+-rw-r--r--   0     1001      127       70 2024-06-03 01:33:06.000000 sophus_pyo3-0.6.1/crates/sophus_pyo3/src/pyo3.rs
+-rw-r--r--   0     1001      127   125309 2024-06-03 01:33:23.000000 sophus_pyo3-0.6.1/Cargo.lock
+-rw-r--r--   0        0        0     1627 1970-01-01 00:00:00.000000 sophus_pyo3-0.6.1/Cargo.toml
+-rw-r--r--   0        0        0      281 1970-01-01 00:00:00.000000 sophus_pyo3-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0      637 1970-01-01 00:00:00.000000 sophus_pyo3-0.6.1/PKG-INFO
```

### Comparing `sophus_pyo3-0.6.0/crates/sophus_core/src/calculus/dual/dual_matrix.rs` & `sophus_pyo3-0.6.1/crates/sophus_core/src/calculus/dual/dual_matrix.rs`

 * *Files identical despite different names*

### Comparing `sophus_pyo3-0.6.0/crates/sophus_core/src/calculus/dual/dual_scalar.rs` & `sophus_pyo3-0.6.1/crates/sophus_core/src/calculus/dual/dual_scalar.rs`

 * *Files identical despite different names*

### Comparing `sophus_pyo3-0.6.0/crates/sophus_core/src/calculus/dual/dual_vector.rs` & `sophus_pyo3-0.6.1/crates/sophus_core/src/calculus/dual/dual_vector.rs`

 * *Files identical despite different names*

### Comparing `sophus_pyo3-0.6.0/crates/sophus_core/src/calculus/maps/curves.rs` & `sophus_pyo3-0.6.1/crates/sophus_core/src/calculus/maps/curves.rs`

 * *Files identical despite different names*

### Comparing `sophus_pyo3-0.6.0/crates/sophus_core/src/calculus/maps/matrix_valued_maps.rs` & `sophus_pyo3-0.6.1/crates/sophus_core/src/calculus/maps/matrix_valued_maps.rs`

 * *Files identical despite different names*

### Comparing `sophus_pyo3-0.6.0/crates/sophus_core/src/calculus/maps/scalar_valued_maps.rs` & `sophus_pyo3-0.6.1/crates/sophus_core/src/calculus/maps/scalar_valued_maps.rs`

 * *Files identical despite different names*

### Comparing `sophus_pyo3-0.6.0/crates/sophus_core/src/calculus/maps/vector_valued_maps.rs` & `sophus_pyo3-0.6.1/crates/sophus_core/src/calculus/maps/vector_valued_maps.rs`

 * *Files identical despite different names*

### Comparing `sophus_pyo3-0.6.0/crates/sophus_core/src/calculus/maps.rs` & `sophus_pyo3-0.6.1/crates/sophus_core/src/calculus/maps.rs`

 * *Files identical despite different names*

### Comparing `sophus_pyo3-0.6.0/crates/sophus_core/src/calculus/region.rs` & `sophus_pyo3-0.6.1/crates/sophus_core/src/calculus/region.rs`

 * *Files identical despite different names*

### Comparing `sophus_pyo3-0.6.0/crates/sophus_core/src/calculus/spline/spline_segment.rs` & `sophus_pyo3-0.6.1/crates/sophus_core/src/calculus/spline/spline_segment.rs`

 * *Files identical despite different names*

### Comparing `sophus_pyo3-0.6.0/crates/sophus_core/src/calculus/spline.rs` & `sophus_pyo3-0.6.1/crates/sophus_core/src/calculus/spline.rs`

 * *Files identical despite different names*

### Comparing `sophus_pyo3-0.6.0/crates/sophus_core/src/calculus.rs` & `sophus_pyo3-0.6.1/crates/sophus_core/src/calculus.rs`

 * *Files identical despite different names*

### Comparing `sophus_pyo3-0.6.0/crates/sophus_core/src/linalg/bool_mask.rs` & `sophus_pyo3-0.6.1/crates/sophus_core/src/linalg/bool_mask.rs`

 * *Files identical despite different names*

### Comparing `sophus_pyo3-0.6.0/crates/sophus_core/src/linalg/matrix.rs` & `sophus_pyo3-0.6.1/crates/sophus_core/src/linalg/matrix.rs`

 * *Files identical despite different names*

### Comparing `sophus_pyo3-0.6.0/crates/sophus_core/src/linalg/scalar.rs` & `sophus_pyo3-0.6.1/crates/sophus_core/src/linalg/scalar.rs`

 * *Files identical despite different names*

### Comparing `sophus_pyo3-0.6.0/crates/sophus_core/src/linalg/vector.rs` & `sophus_pyo3-0.6.1/crates/sophus_core/src/linalg/vector.rs`

 * *Files identical despite different names*

### Comparing `sophus_pyo3-0.6.0/crates/sophus_core/src/linalg.rs` & `sophus_pyo3-0.6.1/crates/sophus_core/src/linalg.rs`

 * *Files identical despite different names*

### Comparing `sophus_pyo3-0.6.0/crates/sophus_core/src/manifold/traits.rs` & `sophus_pyo3-0.6.1/crates/sophus_core/src/manifold/traits.rs`

 * *Files identical despite different names*

### Comparing `sophus_pyo3-0.6.0/crates/sophus_core/src/params.rs` & `sophus_pyo3-0.6.1/crates/sophus_core/src/params.rs`

 * *Files identical despite different names*

### Comparing `sophus_pyo3-0.6.0/crates/sophus_core/src/points.rs` & `sophus_pyo3-0.6.1/crates/sophus_core/src/points.rs`

 * *Files identical despite different names*

### Comparing `sophus_pyo3-0.6.0/crates/sophus_core/src/tensor/arc_tensor.rs` & `sophus_pyo3-0.6.1/crates/sophus_core/src/tensor/arc_tensor.rs`

 * *Files identical despite different names*

### Comparing `sophus_pyo3-0.6.0/crates/sophus_core/src/tensor/element.rs` & `sophus_pyo3-0.6.1/crates/sophus_core/src/tensor/element.rs`

 * *Files identical despite different names*

### Comparing `sophus_pyo3-0.6.0/crates/sophus_core/src/tensor/mut_tensor.rs` & `sophus_pyo3-0.6.1/crates/sophus_core/src/tensor/mut_tensor.rs`

 * *Files identical despite different names*

### Comparing `sophus_pyo3-0.6.0/crates/sophus_core/src/tensor/mut_tensor_view.rs` & `sophus_pyo3-0.6.1/crates/sophus_core/src/tensor/mut_tensor_view.rs`

 * *Files identical despite different names*

### Comparing `sophus_pyo3-0.6.0/crates/sophus_core/src/tensor/tensor_view.rs` & `sophus_pyo3-0.6.1/crates/sophus_core/src/tensor/tensor_view.rs`

 * *Files 0% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 ///           number of ROWS.
 ///      - rank 2:
 ///         * A matrix ``SMat<Scalar, ROWS, COLS>`` aka ``nalgebra::SMatrix<Scalar, ROWS, COLS>``
 ///           with static shape (ROWS x COLS).
 ///  2. A scalar tensor of TOTAL_RANK = DRANK + SRANK.
 ///    *  ``self.scalar_dims()`` is used to access its dimensions of type
 ///        ``[usize: TOTAL_RANK]`` at runtime.
-///    *  - an individual element (= static tensor) can be accessed with
-///        ``self.scalar_get(idx)``, where idx is of type ``[usize: DRANK]``.
+///    *  an individual element (= static tensor) can be accessed with
+///       ``self.scalar_get(idx)``, where idx is of type ``[usize: DRANK]``.
 #[derive(Debug, Copy, Clone, PartialEq, Eq)]
 pub struct TensorView<
     'a,
     const TOTAL_RANK: usize,
     const DRANK: usize,
     const SRANK: usize,
     Scalar: IsCoreScalar + 'static,
```

### Comparing `sophus_pyo3-0.6.0/crates/sophus_lie/src/factor_lie_group.rs` & `sophus_pyo3-0.6.1/crates/sophus_lie/src/factor_lie_group.rs`

 * *Files identical despite different names*

### Comparing `sophus_pyo3-0.6.0/crates/sophus_lie/src/groups/isometry2.rs` & `sophus_pyo3-0.6.1/crates/sophus_lie/src/groups/isometry2.rs`

 * *Files identical despite different names*

### Comparing `sophus_pyo3-0.6.0/crates/sophus_lie/src/groups/isometry3.rs` & `sophus_pyo3-0.6.1/crates/sophus_lie/src/groups/isometry3.rs`

 * *Files identical despite different names*

### Comparing `sophus_pyo3-0.6.0/crates/sophus_lie/src/groups/rotation2.rs` & `sophus_pyo3-0.6.1/crates/sophus_lie/src/groups/rotation2.rs`

 * *Files identical despite different names*

### Comparing `sophus_pyo3-0.6.0/crates/sophus_lie/src/groups/rotation3.rs` & `sophus_pyo3-0.6.1/crates/sophus_lie/src/groups/rotation3.rs`

 * *Files identical despite different names*

### Comparing `sophus_pyo3-0.6.0/crates/sophus_lie/src/groups/translation_product_product.rs` & `sophus_pyo3-0.6.1/crates/sophus_lie/src/groups/translation_product_product.rs`

 * *Files identical despite different names*

### Comparing `sophus_pyo3-0.6.0/crates/sophus_lie/src/lib.rs` & `sophus_pyo3-0.6.1/crates/sophus_lie/src/lib.rs`

 * *Files identical despite different names*

### Comparing `sophus_pyo3-0.6.0/crates/sophus_lie/src/lie_group.rs` & `sophus_pyo3-0.6.1/crates/sophus_lie/src/lie_group.rs`

 * *Files identical despite different names*

### Comparing `sophus_pyo3-0.6.0/crates/sophus_lie/src/lie_group_manifold.rs` & `sophus_pyo3-0.6.1/crates/sophus_lie/src/lie_group_manifold.rs`

 * *Files identical despite different names*

### Comparing `sophus_pyo3-0.6.0/crates/sophus_lie/src/real_lie_group.rs` & `sophus_pyo3-0.6.1/crates/sophus_lie/src/real_lie_group.rs`

 * *Files identical despite different names*

### Comparing `sophus_pyo3-0.6.0/crates/sophus_lie/src/traits.rs` & `sophus_pyo3-0.6.1/crates/sophus_lie/src/traits.rs`

 * *Files identical despite different names*

### Comparing `sophus_pyo3-0.6.0/crates/sophus_pyo3/Cargo.toml` & `sophus_pyo3-0.6.1/crates/sophus_pyo3/Cargo.toml`

 * *Files identical despite different names*

### Comparing `sophus_pyo3-0.6.0/crates/sophus_pyo3/src/lib.rs` & `sophus_pyo3-0.6.1/crates/sophus_pyo3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `sophus_pyo3-0.6.0/crates/sophus_pyo3/src/pyo3/errors.rs` & `sophus_pyo3-0.6.1/crates/sophus_pyo3/src/pyo3/errors.rs`

 * *Files identical despite different names*

### Comparing `sophus_pyo3-0.6.0/crates/sophus_pyo3/src/pyo3/lie_groups.rs` & `sophus_pyo3-0.6.1/crates/sophus_pyo3/src/pyo3/lie_groups.rs`

 * *Files identical despite different names*

### Comparing `sophus_pyo3-0.6.0/Cargo.lock` & `sophus_pyo3-0.6.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -91,17 +91,17 @@
  "accesskit_unix",
  "accesskit_windows",
  "winit",
 ]
 
 [[package]]
 name = "addr2line"
-version = "0.21.0"
+version = "0.22.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a30b2e23b9e17a9f90641c7ab1549cd9b44f296d3ccbf309d2863cfe398a0cb"
+checksum = "6e4503c46a5c0c7844e948c9a4d6acd9f50cccb4de1c48eb9e291ea17470c678"
 dependencies = [
  "gimli",
 ]
 
 [[package]]
 name = "adler"
 version = "1.0.2"
@@ -298,15 +298,15 @@
 [[package]]
 name = "async-channel"
 version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "89b47800b0be77592da0afd425cc03468052844aff33b84e33cc696f64e77b6a"
 dependencies = [
  "concurrent-queue",
- "event-listener-strategy 0.5.2",
+ "event-listener-strategy",
  "futures-core",
  "pin-project-lite",
 ]
 
 [[package]]
 name = "async-executor"
 version = "1.12.0"
@@ -350,25 +350,25 @@
  "slab",
  "socket2 0.4.10",
  "waker-fn",
 ]
 
 [[package]]
 name = "async-io"
-version = "2.3.2"
+version = "2.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dcccb0f599cfa2f8ace422d3555572f47424da5648a4382a9dd0310ff8210884"
+checksum = "0d6baa8f0178795da0e71bc42c9e5d13261aac7ee549853162e66a241ba17964"
 dependencies = [
- "async-lock 3.3.0",
+ "async-lock 3.4.0",
  "cfg-if",
  "concurrent-queue",
  "futures-io",
  "futures-lite 2.3.0",
  "parking",
- "polling 3.7.0",
+ "polling 3.7.1",
  "rustix 0.38.34",
  "slab",
  "tracing",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
@@ -378,20 +378,20 @@
 checksum = "287272293e9d8c41773cec55e365490fe034813a2f172f502d6ddcf75b2f582b"
 dependencies = [
  "event-listener 2.5.3",
 ]
 
 [[package]]
 name = "async-lock"
-version = "3.3.0"
+version = "3.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d034b430882f8381900d3fe6f0aaa3ad94f2cb4ac519b429692a1bc2dda4ae7b"
+checksum = "ff6e472cdea888a4bd64f342f09b3f50e1886d32afe8df3d663c01140b811b18"
 dependencies = [
- "event-listener 4.0.3",
- "event-listener-strategy 0.4.0",
+ "event-listener 5.3.1",
+ "event-listener-strategy",
  "pin-project-lite",
 ]
 
 [[package]]
 name = "async-once-cell"
 version = "0.5.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -423,20 +423,20 @@
  "proc-macro2",
  "quote",
  "syn 2.0.66",
 ]
 
 [[package]]
 name = "async-signal"
-version = "0.2.6"
+version = "0.2.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "afe66191c335039c7bb78f99dc7520b0cbb166b3a1cb33a03f53d8a1c6f2afda"
+checksum = "329972aa325176e89114919f2a80fdae4f4c040f66a370b1a1159c6c0f94e7aa"
 dependencies = [
- "async-io 2.3.2",
- "async-lock 3.3.0",
+ "async-io 2.3.3",
+ "async-lock 3.4.0",
  "atomic-waker",
  "cfg-if",
  "futures-core",
  "futures-io",
  "rustix 0.38.34",
  "signal-hook-registry",
  "slab",
@@ -518,17 +518,17 @@
 name = "autocfg"
 version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0c4b4d0bd25bd0b74681c0ad21497610ce1b7c91b1022cd21c80c6fbdd9476b0"
 
 [[package]]
 name = "backtrace"
-version = "0.3.71"
+version = "0.3.72"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "26b05800d2e817c8b3b4b54abd461726265fa9789ae34330622f2db9ee696f9d"
+checksum = "17c6a35df3749d2e8bb1b7b21a976d82b15548788d2735b9d82f329268f71a11"
 dependencies = [
  "addr2line",
  "cc",
  "cfg-if",
  "libc",
  "miniz_oxide",
  "object",
@@ -622,20 +622,19 @@
 checksum = "2c132eebf10f5cad5289222520a4a058514204aed6d791f1cf4fe8088b82d15f"
 dependencies = [
  "objc2 0.5.2",
 ]
 
 [[package]]
 name = "blocking"
-version = "1.6.0"
+version = "1.6.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "495f7104e962b7356f0aeb34247aca1fe7d2e783b346582db7f2904cb5717e88"
+checksum = "703f41c54fc768e63e091340b424302bb1c29ef4aa0c7f10fe849dfb114d29ea"
 dependencies = [
  "async-channel",
- "async-lock 3.3.0",
  "async-task",
  "futures-io",
  "futures-lite 2.3.0",
  "piper",
 ]
 
 [[package]]
@@ -651,17 +650,17 @@
 checksum = "78834c15cb5d5efe3452d58b1e8ba890dd62d21907f867f383358198e56ebca5"
 dependencies = [
  "bytemuck_derive",
 ]
 
 [[package]]
 name = "bytemuck_derive"
-version = "1.6.1"
+version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "369cfaf2a5bed5d8f8202073b2e093c9f508251de1551a0deb4253e4c7d80909"
+checksum = "1ee891b04274a59bd38b412188e24b849617b2e45a0fd8d057deb63e7403761b"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.66",
 ]
 
 [[package]]
@@ -680,15 +679,15 @@
 name = "calloop"
 version = "0.12.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fba7adb4dd5aa98e5553510223000e7148f621165ec5f9acd7113f6ca4995298"
 dependencies = [
  "bitflags 2.5.0",
  "log",
- "polling 3.7.0",
+ "polling 3.7.1",
  "rustix 0.38.34",
  "slab",
  "thiserror",
 ]
 
 [[package]]
 name = "calloop-wayland-source"
@@ -1345,26 +1344,26 @@
  "nohash-hasher",
  "parking_lot",
  "serde",
 ]
 
 [[package]]
 name = "equator"
-version = "0.1.10"
+version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a3b0a88aa91d0ad2b9684e4479aed31a17d3f9051bdbbc634bd2c01bc5a5eee8"
+checksum = "c35da53b5a021d2484a7cc49b2ac7f2d840f8236a286f84202369bd338d761ea"
 dependencies = [
  "equator-macro",
 ]
 
 [[package]]
 name = "equator-macro"
-version = "0.1.9"
+version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "60d08acb9849f7fb4401564f251be5a526829183a3645a90197dea8e786cf3ae"
+checksum = "3bf679796c0322556351f287a51b49e48f7c4986e727b5dd78c972d30e2e16cc"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.66",
 ]
 
 [[package]]
@@ -1404,86 +1403,66 @@
  "concurrent-queue",
  "parking",
  "pin-project-lite",
 ]
 
 [[package]]
 name = "event-listener"
-version = "4.0.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "67b215c49b2b248c855fb73579eb1f4f26c38ffdc12973e20e07b91d78d5646e"
-dependencies = [
- "concurrent-queue",
- "parking",
- "pin-project-lite",
-]
-
-[[package]]
-name = "event-listener"
-version = "5.3.0"
+version = "5.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6d9944b8ca13534cdfb2800775f8dd4902ff3fc75a50101466decadfdf322a24"
+checksum = "6032be9bd27023a771701cc49f9f053c751055f71efb2e0ae5c15809093675ba"
 dependencies = [
  "concurrent-queue",
  "parking",
  "pin-project-lite",
 ]
 
 [[package]]
 name = "event-listener-strategy"
-version = "0.4.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "958e4d70b6d5e81971bebec42271ec641e7ff4e170a6fa605f2b8a8b65cb97d3"
-dependencies = [
- "event-listener 4.0.3",
- "pin-project-lite",
-]
-
-[[package]]
-name = "event-listener-strategy"
 version = "0.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0f214dc438f977e6d4e3500aaa277f5ad94ca83fbbd9b1a15713ce2344ccc5a1"
 dependencies = [
- "event-listener 5.3.0",
+ "event-listener 5.3.1",
  "pin-project-lite",
 ]
 
 [[package]]
 name = "faer"
-version = "0.18.2"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e547492d9b55c4ea882584e691ed092228981e337d0c800bc721301d7e61e40a"
+checksum = "91ef9e1a4098a9e3a03c47bc5061406c04820552d869fd0fcd92587d07b271f0"
 dependencies = [
  "bytemuck",
  "coe-rs",
  "dbgf",
  "dyn-stack",
  "equator",
  "faer-entity",
  "gemm",
  "libm",
  "matrixcompare",
  "matrixcompare-core",
+ "nano-gemm",
  "npyz",
  "num-complex",
  "num-traits",
  "paste",
  "rand",
  "rand_distr",
  "rayon",
  "reborrow",
  "serde",
 ]
 
 [[package]]
 name = "faer-entity"
-version = "0.18.0"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "22ea5c06233193392c614a46aa3bbe3de29c1404692c8053abd9c2765a1cd159"
+checksum = "ab968a02be27be95de0f1ad0af901b865fa0866b6a9b553a6cc9cf7f19c2ce71"
 dependencies = [
  "bytemuck",
  "coe-rs",
  "libm",
  "num-complex",
  "num-traits",
  "pulp",
@@ -1638,17 +1617,17 @@
  "pin-project-lite",
  "pin-utils",
  "slab",
 ]
 
 [[package]]
 name = "gemm"
-version = "0.17.1"
+version = "0.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6ab24cc62135b40090e31a76a9b2766a501979f3070fa27f689c27ec04377d32"
+checksum = "e400f2ffd14e7548356236c35dc39cad6666d833a852cb8a8f3f28029359bb03"
 dependencies = [
  "dyn-stack",
  "gemm-c32",
  "gemm-c64",
  "gemm-common",
  "gemm-f16",
  "gemm-f32",
@@ -1658,47 +1637,47 @@
  "paste",
  "raw-cpuid",
  "seq-macro",
 ]
 
 [[package]]
 name = "gemm-c32"
-version = "0.17.1"
+version = "0.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b9c030d0b983d1e34a546b86e08f600c11696fde16199f971cd46c12e67512c0"
+checksum = "10dc4a6176c8452d60eac1a155b454c91c668f794151a303bf3c75ea2874812d"
 dependencies = [
  "dyn-stack",
  "gemm-common",
  "num-complex",
  "num-traits",
  "paste",
  "raw-cpuid",
  "seq-macro",
 ]
 
 [[package]]
 name = "gemm-c64"
-version = "0.17.1"
+version = "0.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fbb5f2e79fefb9693d18e1066a557b4546cd334b226beadc68b11a8f9431852a"
+checksum = "cc2032ce2c0bb150da0256338759a6fb01ca056f6dfe28c4d14af32d7f878f6f"
 dependencies = [
  "dyn-stack",
  "gemm-common",
  "num-complex",
  "num-traits",
  "paste",
  "raw-cpuid",
  "seq-macro",
 ]
 
 [[package]]
 name = "gemm-common"
-version = "0.17.1"
+version = "0.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a2e7ea062c987abcd8db95db917b4ffb4ecdfd0668471d8dc54734fdff2354e8"
+checksum = "90fd234fc525939654f47b39325fd5f55e552ceceea9135f3aa8bdba61eabef6"
 dependencies = [
  "bytemuck",
  "dyn-stack",
  "half",
  "num-complex",
  "num-traits",
  "once_cell",
@@ -1708,17 +1687,17 @@
  "rayon",
  "seq-macro",
  "sysctl",
 ]
 
 [[package]]
 name = "gemm-f16"
-version = "0.17.1"
+version = "0.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ca4c06b9b11952071d317604acb332e924e817bd891bec8dfb494168c7cedd4"
+checksum = "3fc3652651f96a711d46b8833e1fac27a864be4bdfa81a374055f33ddd25c0c6"
 dependencies = [
  "dyn-stack",
  "gemm-common",
  "gemm-f32",
  "half",
  "num-complex",
  "num-traits",
@@ -1726,32 +1705,32 @@
  "raw-cpuid",
  "rayon",
  "seq-macro",
 ]
 
 [[package]]
 name = "gemm-f32"
-version = "0.17.1"
+version = "0.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e9a69f51aaefbd9cf12d18faf273d3e982d9d711f60775645ed5c8047b4ae113"
+checksum = "acbc51c44ae3defd207e6d9416afccb3c4af1e7cef5e4960e4c720ac4d6f998e"
 dependencies = [
  "dyn-stack",
  "gemm-common",
  "num-complex",
  "num-traits",
  "paste",
  "raw-cpuid",
  "seq-macro",
 ]
 
 [[package]]
 name = "gemm-f64"
-version = "0.17.1"
+version = "0.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "aa397a48544fadf0b81ec8741e5c0fba0043008113f71f2034def1935645d2b0"
+checksum = "3f37fc86e325c2415a4d0cab8324a0c5371ec06fc7d2f9cb1636fcfc9536a8d8"
 dependencies = [
  "dyn-stack",
  "gemm-common",
  "num-complex",
  "num-traits",
  "paste",
  "raw-cpuid",
@@ -1787,17 +1766,17 @@
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
 name = "gimli"
-version = "0.28.1"
+version = "0.29.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4271d37baee1b8c7e4b708028c57d816cf9d2434acb33a549475f78c181f6253"
+checksum = "40ecd4077b5ae9fd2e9e169b102c6c330d0605168eb0e8bf79952b256dbefffd"
 
 [[package]]
 name = "gl_generator"
 version = "0.14.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1a95dfc23a2b4a9a2f5ab41d194f8bfda3cabec42af4e39f08c339eb2a0c124d"
 dependencies = [
@@ -2238,14 +2217,20 @@
 [[package]]
 name = "linear_type"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fe1b1db2093ba1db1b494c2f29526b6ee00c89343744210cad6c5a04466e8526"
 
 [[package]]
+name = "linked-hash-map"
+version = "0.5.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0717cef1bc8b636c6e1c1bbdefc09e6322da8a9321966e8928ef80d20f7f770f"
+
+[[package]]
 name = "linux-raw-sys"
 version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ef53942eb7bf7ff43a617b3e2c1c4a5ecf5944a7c1bc12d7ee39bbb15e5c1519"
 
 [[package]]
 name = "linux-raw-sys"
@@ -2441,14 +2426,84 @@
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
+name = "nano-gemm"
+version = "0.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f563548d38f390ef9893e4883ec38c1fb312f569e98d76bededdd91a3b41a043"
+dependencies = [
+ "equator",
+ "nano-gemm-c32",
+ "nano-gemm-c64",
+ "nano-gemm-codegen",
+ "nano-gemm-core",
+ "nano-gemm-f32",
+ "nano-gemm-f64",
+ "num-complex",
+]
+
+[[package]]
+name = "nano-gemm-c32"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a40449e57a5713464c3a1208c4c3301c8d29ee1344711822cf022bc91373a91b"
+dependencies = [
+ "nano-gemm-codegen",
+ "nano-gemm-core",
+ "num-complex",
+]
+
+[[package]]
+name = "nano-gemm-c64"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "743a6e6211358fba85d1009616751e4107da86f4c95b24e684ce85f25c25b3bf"
+dependencies = [
+ "nano-gemm-codegen",
+ "nano-gemm-core",
+ "num-complex",
+]
+
+[[package]]
+name = "nano-gemm-codegen"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "963bf7c7110d55430169dc74c67096375491ed580cd2ef84842550ac72e781fa"
+
+[[package]]
+name = "nano-gemm-core"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "fe3fc4f83ae8861bad79dc3c016bd6b0220da5f9de302e07d3112d16efc24aa6"
+
+[[package]]
+name = "nano-gemm-f32"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4e3681b7ce35658f79da94b7f62c60a005e29c373c7111ed070e3bf64546a8bb"
+dependencies = [
+ "nano-gemm-codegen",
+ "nano-gemm-core",
+]
+
+[[package]]
+name = "nano-gemm-f64"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bc1e619ed04d801809e1f63e61b669d380c4119e8b0cdd6ed184c6b111f046d8"
+dependencies = [
+ "nano-gemm-codegen",
+ "nano-gemm-core",
+]
+
+[[package]]
 name = "ndarray"
 version = "0.15.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "adb12d4e967ec485a5f71c6311fe28158e9d6f4bc4a447b474184d0f91a8fa32"
 dependencies = [
  "approx",
  "matrixmultiply",
@@ -2554,14 +2609,15 @@
 name = "num-complex"
 version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "73f88a1307638156682bada9d7604135552957b7818057dcef22705b4d509495"
 dependencies = [
  "bytemuck",
  "num-traits",
+ "rand",
 ]
 
 [[package]]
 name = "num-integer"
 version = "0.1.46"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7969661fd2958a5cb096e56c8e1ad0444ac2bbcd0061bd28660485a44879858f"
@@ -2793,17 +2849,17 @@
 checksum = "ad970fb455818ad6cba4c122ad012fae53ae8b4795f86378bce65e4f6bab2ca4"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "object"
-version = "0.32.2"
+version = "0.35.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a6a622008b6e321afc04970976f62ee297fdbaa6f95318ca343e3eebb9648441"
+checksum = "b8ec7ab813848ba4522158d5517a6093db1ded27575b070f4177b8d12b41db5e"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "once_cell"
 version = "1.19.0"
@@ -2950,17 +3006,17 @@
 name = "pin-utils"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b870d8c151b6f2fb93e84a13146138f05d02ed11c7e7c54f8826aaaf7c9f184"
 
 [[package]]
 name = "piper"
-version = "0.2.2"
+version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "464db0c665917b13ebb5d453ccdec4add5658ee1adc7affc7677615356a8afaf"
+checksum = "ae1d5c74c9876f070d3e8fd503d748c7d974c3e48da8f41350fa5222ef9b4391"
 dependencies = [
  "atomic-waker",
  "fastrand 2.1.0",
  "futures-io",
 ]
 
 [[package]]
@@ -2996,17 +3052,17 @@
  "log",
  "pin-project-lite",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "polling"
-version = "3.7.0"
+version = "3.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "645493cf344456ef24219d02a768cf1fb92ddf8c92161679ae3d91b91a637be3"
+checksum = "5e6a007746f34ed64099e88783b0ae369eaa3da6392868ba262e2af9b8fbaea1"
 dependencies = [
  "cfg-if",
  "concurrent-queue",
  "hermit-abi",
  "pin-project-lite",
  "rustix 0.38.34",
  "tracing",
@@ -3054,17 +3110,17 @@
 checksum = "6d37c51ca738a55da99dc0c4a34860fd675453b8b36209178c2249bb13651284"
 dependencies = [
  "toml_edit 0.21.1",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.84"
+version = "1.0.85"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ec96c6a92621310b51366f1e28d05ef11489516e93be030060e5fc12024a49d6"
+checksum = "22244ce15aa966053a896d1accb3a6e68469b97c7f33f284b99f0d576879fc23"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "profiling"
 version = "1.0.15"
@@ -3612,15 +3668,15 @@
 dependencies = [
  "libc",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "sophus"
-version = "0.6.0"
+version = "0.6.1"
 dependencies = [
  "approx",
  "assertables",
  "bytemuck",
  "eframe",
  "egui_extras",
  "env_logger",
@@ -3636,54 +3692,54 @@
  "sophus_viewer",
  "tokio",
  "wgpu",
 ]
 
 [[package]]
 name = "sophus_core"
-version = "0.6.0"
+version = "0.6.1"
 dependencies = [
  "approx",
  "assertables",
  "concat-arrays",
  "nalgebra",
  "ndarray",
  "num-traits",
  "sleef",
  "typenum",
 ]
 
 [[package]]
 name = "sophus_image"
-version = "0.6.0"
+version = "0.6.1"
 dependencies = [
  "approx",
  "assertables",
  "bytemuck",
  "nalgebra",
  "ndarray",
  "num-traits",
  "png",
  "sophus_core",
 ]
 
 [[package]]
 name = "sophus_lie"
-version = "0.6.0"
+version = "0.6.1"
 dependencies = [
  "approx",
  "assertables",
  "nalgebra",
  "num-traits",
  "sophus_core",
 ]
 
 [[package]]
 name = "sophus_opt"
-version = "0.6.0"
+version = "0.6.1"
 dependencies = [
  "approx",
  "as-any",
  "assertables",
  "dyn-clone",
  "faer",
  "nalgebra",
@@ -3693,47 +3749,48 @@
  "sophus_image",
  "sophus_lie",
  "sophus_sensor",
 ]
 
 [[package]]
 name = "sophus_pyo3"
-version = "0.6.0"
+version = "0.6.1"
 dependencies = [
  "nalgebra",
  "numpy",
  "pyo3",
  "sophus_core",
  "sophus_lie",
 ]
 
 [[package]]
 name = "sophus_sensor"
-version = "0.6.0"
+version = "0.6.1"
 dependencies = [
  "approx",
  "assertables",
  "nalgebra",
  "ndarray",
  "num-traits",
  "sophus_core",
  "sophus_image",
 ]
 
 [[package]]
 name = "sophus_viewer"
-version = "0.6.0"
+version = "0.6.1"
 dependencies = [
  "approx",
  "assertables",
  "bytemuck",
  "eframe",
  "egui_extras",
  "env_logger",
  "hollywood",
+ "linked-hash-map",
  "nalgebra",
  "ndarray",
  "sophus_core",
  "sophus_image",
  "sophus_lie",
  "sophus_sensor",
  "tokio",
@@ -3892,17 +3949,17 @@
 name = "tinyvec_macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
 
 [[package]]
 name = "tokio"
-version = "1.37.0"
+version = "1.38.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1adbebffeca75fcfd058afa480fb6c0b81e165a0323f9c9d39c9697e37c46787"
+checksum = "ba4f4a02a7a80d6f274636f0aa95c7e383b912d41fe721a31f29e29698585a4a"
 dependencies = [
  "backtrace",
  "bytes",
  "libc",
  "mio",
  "num_cpus",
  "parking_lot",
@@ -3911,17 +3968,17 @@
  "socket2 0.5.7",
  "tokio-macros",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "tokio-macros"
-version = "2.2.0"
+version = "2.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5b8a1e28f2deaa14e508979454cb3a223b10b938b45af148bc0986de36f1923b"
+checksum = "5f5ae998a069d4b5aba8ee9dad856af7d520c3699e6159b185c2acd48155d39a"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.66",
 ]
 
 [[package]]
@@ -4227,31 +4284,31 @@
 name = "wasm-bindgen-shared"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "af190c94f2773fdb3729c55b007a722abb5384da03bc0986df4c289bf5567e96"
 
 [[package]]
 name = "wayland-backend"
-version = "0.3.3"
+version = "0.3.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9d50fa61ce90d76474c87f5fc002828d81b32677340112b4ef08079a9d459a40"
+checksum = "34e9e6b6d4a2bb4e7e69433e0b35c7923b95d4dc8503a84d25ec917a4bbfdf07"
 dependencies = [
  "cc",
  "downcast-rs",
  "rustix 0.38.34",
  "scoped-tls",
  "smallvec",
  "wayland-sys",
 ]
 
 [[package]]
 name = "wayland-client"
-version = "0.31.2"
+version = "0.31.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "82fb96ee935c2cea6668ccb470fb7771f6215d1691746c2d896b447a00ad3f1f"
+checksum = "1e63801c85358a431f986cffa74ba9599ff571fc5774ac113ed3b490c19a1133"
 dependencies = [
  "bitflags 2.5.0",
  "rustix 0.38.34",
  "wayland-backend",
  "wayland-scanner",
 ]
 
@@ -4264,17 +4321,17 @@
  "bitflags 2.5.0",
  "cursor-icon",
  "wayland-backend",
 ]
 
 [[package]]
 name = "wayland-cursor"
-version = "0.31.1"
+version = "0.31.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "71ce5fa868dd13d11a0d04c5e2e65726d0897be8de247c0c5a65886e283231ba"
+checksum = "a206e8b2b53b1d3fcb9428fec72bc278ce539e2fa81fe2bfc1ab27703d5187b9"
 dependencies = [
  "rustix 0.38.34",
  "wayland-client",
  "xcursor",
 ]
 
 [[package]]
@@ -4313,28 +4370,28 @@
  "wayland-client",
  "wayland-protocols",
  "wayland-scanner",
 ]
 
 [[package]]
 name = "wayland-scanner"
-version = "0.31.1"
+version = "0.31.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "63b3a62929287001986fb58c789dce9b67604a397c15c611ad9f747300b6c283"
+checksum = "67da50b9f80159dec0ea4c11c13e24ef9e7574bd6ce24b01860a175010cea565"
 dependencies = [
  "proc-macro2",
  "quick-xml",
  "quote",
 ]
 
 [[package]]
 name = "wayland-sys"
-version = "0.31.1"
+version = "0.31.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "15a0c8eaff5216d07f226cb7a549159267f3467b289d9a2e52fd3ef5aae2b7af"
+checksum = "105b1842da6554f91526c14a2a2172897b7f745a805d62af4ce698706be79c12"
 dependencies = [
  "dlib",
  "log",
  "once_cell",
  "pkg-config",
 ]
```

### Comparing `sophus_pyo3-0.6.0/Cargo.toml` & `sophus_pyo3-0.6.1/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -8,43 +8,44 @@
   "**/*.rs",
   "**/*.wgsl",
   "Cargo.toml",
 ]
 keywords = ["robotics", "optimization"]
 license = "MIT OR Apache-2.0"
 repository = "https://github.com/farm-ng/sophus-rs/"
-version = "0.6.0"
+version = "0.6.1"
 
 [workspace.dependencies]
-sophus = {path = "crates/sophus", version = "0.6.0"}
-sophus_core = {path = "crates/sophus_core", version = "0.6.0"}
-sophus_image = {path = "crates/sophus_image", version = "0.6.0"}
-sophus_lie = {path = "crates/sophus_lie", version = "0.6.0"}
-sophus_opt = {path = "crates/sophus_opt", version = "0.6.0"}
-sophus_pyo3 = {path = "crates/sophus_pyo3", version = "0.6.0"}
-sophus_sensor = {path = "crates/sophus_sensor", version = "0.6.0"}
-sophus_viewer = {path = "crates/sophus_viewer", version = "0.6.0"}
+sophus = {path = "crates/sophus", version = "0.6.1"}
+sophus_core = {path = "crates/sophus_core", version = "0.6.1"}
+sophus_image = {path = "crates/sophus_image", version = "0.6.1"}
+sophus_lie = {path = "crates/sophus_lie", version = "0.6.1"}
+sophus_opt = {path = "crates/sophus_opt", version = "0.6.1"}
+sophus_pyo3 = {path = "crates/sophus_pyo3", version = "0.6.1"}
+sophus_sensor = {path = "crates/sophus_sensor", version = "0.6.1"}
+sophus_viewer = {path = "crates/sophus_viewer", version = "0.6.1"}
 
 approx = "0.5"
 as-any = "0.3"
 assertables = "7.0"
 async-trait = "0.1"
 bytemuck = {version = "1.14", features = ["derive"]}
 concat-arrays = "0.1"
 dyn-clone = "1.0"
 eframe = {version = "0.27", features = ["wgpu"]}
 egui_extras = "0.27"
 env_logger = "0.11"
-faer = "0.18"
+faer = "0.19"
 hollywood = {version = "0.7.0"}
 image = {version = "0.25", features = [
   "jpeg",
   "png",
   "tiff",
 ]}
+linked-hash-map = "0.5"
 log = "0.4"
 nalgebra = {version = "0.32", features = ["rand"]}
 ndarray = {version = "0.15", features = ["approx-0_5"]}
 num-traits = "0.2"
 numpy = "0.21"
 png = "0.17"
 rand = "0.8"
```

### Comparing `sophus_pyo3-0.6.0/PKG-INFO` & `sophus_pyo3-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sophus_pyo3
-Version: 0.6.0
+Version: 0.6.1
 Summary: sophus - geometry for robotics and computer vision
 Keywords: robotics,optimization
 License: MIT OR Apache-2.0
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source Code, https://github.com/farm-ng/sophus-rs/
 
 # sophus-rs
```

