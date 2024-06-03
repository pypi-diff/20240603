# Comparing `tmp/itkwasm_mesh_io_emscripten-1.2.0.tar.gz` & `tmp/itkwasm_mesh_io_emscripten-1.2.1.tar.gz`

## Comparing `itkwasm_mesh_io_emscripten-1.2.0.tar` & `itkwasm_mesh_io_emscripten-1.2.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 itkwasm_mesh_io_emscripten-1.2.0/itkwasm_mesh_io_emscripten/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm_mesh_io_emscripten-1.2.0/itkwasm_mesh_io_emscripten/_version.py
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 itkwasm_mesh_io_emscripten-1.2.0/itkwasm_mesh_io_emscripten/byu_read_mesh_async.py
--rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 itkwasm_mesh_io_emscripten-1.2.0/itkwasm_mesh_io_emscripten/byu_write_mesh_async.py
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 itkwasm_mesh_io_emscripten-1.2.0/itkwasm_mesh_io_emscripten/extension_to_mesh_io.py
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 itkwasm_mesh_io_emscripten-1.2.0/itkwasm_mesh_io_emscripten/free_surfer_ascii_read_mesh_async.py
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 itkwasm_mesh_io_emscripten-1.2.0/itkwasm_mesh_io_emscripten/free_surfer_ascii_write_mesh_async.py
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 itkwasm_mesh_io_emscripten-1.2.0/itkwasm_mesh_io_emscripten/free_surfer_binary_read_mesh_async.py
--rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 itkwasm_mesh_io_emscripten-1.2.0/itkwasm_mesh_io_emscripten/free_surfer_binary_write_mesh_async.py
--rw-r--r--   0        0        0   204113 2020-02-02 00:00:00.000000 itkwasm_mesh_io_emscripten-1.2.0/itkwasm_mesh_io_emscripten/js_package.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 itkwasm_mesh_io_emscripten-1.2.0/itkwasm_mesh_io_emscripten/mesh_io_index.py
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 itkwasm_mesh_io_emscripten-1.2.0/itkwasm_mesh_io_emscripten/obj_read_mesh_async.py
--rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 itkwasm_mesh_io_emscripten-1.2.0/itkwasm_mesh_io_emscripten/obj_write_mesh_async.py
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 itkwasm_mesh_io_emscripten-1.2.0/itkwasm_mesh_io_emscripten/off_read_mesh_async.py
--rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 itkwasm_mesh_io_emscripten-1.2.0/itkwasm_mesh_io_emscripten/off_write_mesh_async.py
--rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 itkwasm_mesh_io_emscripten-1.2.0/itkwasm_mesh_io_emscripten/read_mesh_async.py
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 itkwasm_mesh_io_emscripten-1.2.0/itkwasm_mesh_io_emscripten/stl_read_mesh_async.py
--rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 itkwasm_mesh_io_emscripten-1.2.0/itkwasm_mesh_io_emscripten/stl_write_mesh_async.py
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 itkwasm_mesh_io_emscripten-1.2.0/itkwasm_mesh_io_emscripten/swc_read_mesh_async.py
--rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 itkwasm_mesh_io_emscripten-1.2.0/itkwasm_mesh_io_emscripten/swc_write_mesh_async.py
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 itkwasm_mesh_io_emscripten-1.2.0/itkwasm_mesh_io_emscripten/vtk_poly_data_read_mesh_async.py
--rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 itkwasm_mesh_io_emscripten-1.2.0/itkwasm_mesh_io_emscripten/vtk_poly_data_write_mesh_async.py
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 itkwasm_mesh_io_emscripten-1.2.0/itkwasm_mesh_io_emscripten/wasm_read_mesh_async.py
--rw-r--r--   0        0        0     2135 2020-02-02 00:00:00.000000 itkwasm_mesh_io_emscripten-1.2.0/itkwasm_mesh_io_emscripten/wasm_write_mesh_async.py
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 itkwasm_mesh_io_emscripten-1.2.0/itkwasm_mesh_io_emscripten/wasm_zstd_read_mesh_async.py
--rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 itkwasm_mesh_io_emscripten-1.2.0/itkwasm_mesh_io_emscripten/wasm_zstd_write_mesh_async.py
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 itkwasm_mesh_io_emscripten-1.2.0/itkwasm_mesh_io_emscripten/wasm_ztd_read_mesh_async.py
--rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 itkwasm_mesh_io_emscripten-1.2.0/itkwasm_mesh_io_emscripten/wasm_ztd_write_mesh_async.py
--rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 itkwasm_mesh_io_emscripten-1.2.0/itkwasm_mesh_io_emscripten/write_mesh_async.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 itkwasm_mesh_io_emscripten-1.2.0/.gitignore
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 itkwasm_mesh_io_emscripten-1.2.0/README.md
--rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 itkwasm_mesh_io_emscripten-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 itkwasm_mesh_io_emscripten-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 itkwasm_mesh_io_emscripten-1.2.1/itkwasm_mesh_io_emscripten/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm_mesh_io_emscripten-1.2.1/itkwasm_mesh_io_emscripten/_version.py
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 itkwasm_mesh_io_emscripten-1.2.1/itkwasm_mesh_io_emscripten/byu_read_mesh_async.py
+-rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 itkwasm_mesh_io_emscripten-1.2.1/itkwasm_mesh_io_emscripten/byu_write_mesh_async.py
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 itkwasm_mesh_io_emscripten-1.2.1/itkwasm_mesh_io_emscripten/extension_to_mesh_io.py
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 itkwasm_mesh_io_emscripten-1.2.1/itkwasm_mesh_io_emscripten/free_surfer_ascii_read_mesh_async.py
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 itkwasm_mesh_io_emscripten-1.2.1/itkwasm_mesh_io_emscripten/free_surfer_ascii_write_mesh_async.py
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 itkwasm_mesh_io_emscripten-1.2.1/itkwasm_mesh_io_emscripten/free_surfer_binary_read_mesh_async.py
+-rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 itkwasm_mesh_io_emscripten-1.2.1/itkwasm_mesh_io_emscripten/free_surfer_binary_write_mesh_async.py
+-rw-r--r--   0        0        0   204113 2020-02-02 00:00:00.000000 itkwasm_mesh_io_emscripten-1.2.1/itkwasm_mesh_io_emscripten/js_package.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 itkwasm_mesh_io_emscripten-1.2.1/itkwasm_mesh_io_emscripten/mesh_io_index.py
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 itkwasm_mesh_io_emscripten-1.2.1/itkwasm_mesh_io_emscripten/obj_read_mesh_async.py
+-rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 itkwasm_mesh_io_emscripten-1.2.1/itkwasm_mesh_io_emscripten/obj_write_mesh_async.py
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 itkwasm_mesh_io_emscripten-1.2.1/itkwasm_mesh_io_emscripten/off_read_mesh_async.py
+-rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 itkwasm_mesh_io_emscripten-1.2.1/itkwasm_mesh_io_emscripten/off_write_mesh_async.py
+-rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 itkwasm_mesh_io_emscripten-1.2.1/itkwasm_mesh_io_emscripten/read_mesh_async.py
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 itkwasm_mesh_io_emscripten-1.2.1/itkwasm_mesh_io_emscripten/stl_read_mesh_async.py
+-rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 itkwasm_mesh_io_emscripten-1.2.1/itkwasm_mesh_io_emscripten/stl_write_mesh_async.py
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 itkwasm_mesh_io_emscripten-1.2.1/itkwasm_mesh_io_emscripten/swc_read_mesh_async.py
+-rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 itkwasm_mesh_io_emscripten-1.2.1/itkwasm_mesh_io_emscripten/swc_write_mesh_async.py
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 itkwasm_mesh_io_emscripten-1.2.1/itkwasm_mesh_io_emscripten/vtk_poly_data_read_mesh_async.py
+-rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 itkwasm_mesh_io_emscripten-1.2.1/itkwasm_mesh_io_emscripten/vtk_poly_data_write_mesh_async.py
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 itkwasm_mesh_io_emscripten-1.2.1/itkwasm_mesh_io_emscripten/wasm_read_mesh_async.py
+-rw-r--r--   0        0        0     2135 2020-02-02 00:00:00.000000 itkwasm_mesh_io_emscripten-1.2.1/itkwasm_mesh_io_emscripten/wasm_write_mesh_async.py
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 itkwasm_mesh_io_emscripten-1.2.1/itkwasm_mesh_io_emscripten/wasm_zstd_read_mesh_async.py
+-rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 itkwasm_mesh_io_emscripten-1.2.1/itkwasm_mesh_io_emscripten/wasm_zstd_write_mesh_async.py
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 itkwasm_mesh_io_emscripten-1.2.1/itkwasm_mesh_io_emscripten/wasm_ztd_read_mesh_async.py
+-rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 itkwasm_mesh_io_emscripten-1.2.1/itkwasm_mesh_io_emscripten/wasm_ztd_write_mesh_async.py
+-rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 itkwasm_mesh_io_emscripten-1.2.1/itkwasm_mesh_io_emscripten/write_mesh_async.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 itkwasm_mesh_io_emscripten-1.2.1/.gitignore
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 itkwasm_mesh_io_emscripten-1.2.1/README.md
+-rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 itkwasm_mesh_io_emscripten-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 itkwasm_mesh_io_emscripten-1.2.1/PKG-INFO
```

### Comparing `itkwasm_mesh_io_emscripten-1.2.0/itkwasm_mesh_io_emscripten/__init__.py` & `itkwasm_mesh_io_emscripten-1.2.1/itkwasm_mesh_io_emscripten/__init__.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io_emscripten-1.2.0/itkwasm_mesh_io_emscripten/byu_read_mesh_async.py` & `itkwasm_mesh_io_emscripten-1.2.1/itkwasm_mesh_io_emscripten/byu_read_mesh_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io_emscripten-1.2.0/itkwasm_mesh_io_emscripten/byu_write_mesh_async.py` & `itkwasm_mesh_io_emscripten-1.2.1/itkwasm_mesh_io_emscripten/byu_write_mesh_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io_emscripten-1.2.0/itkwasm_mesh_io_emscripten/free_surfer_ascii_read_mesh_async.py` & `itkwasm_mesh_io_emscripten-1.2.1/itkwasm_mesh_io_emscripten/free_surfer_ascii_read_mesh_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io_emscripten-1.2.0/itkwasm_mesh_io_emscripten/free_surfer_ascii_write_mesh_async.py` & `itkwasm_mesh_io_emscripten-1.2.1/itkwasm_mesh_io_emscripten/free_surfer_ascii_write_mesh_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io_emscripten-1.2.0/itkwasm_mesh_io_emscripten/free_surfer_binary_read_mesh_async.py` & `itkwasm_mesh_io_emscripten-1.2.1/itkwasm_mesh_io_emscripten/free_surfer_binary_read_mesh_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io_emscripten-1.2.0/itkwasm_mesh_io_emscripten/free_surfer_binary_write_mesh_async.py` & `itkwasm_mesh_io_emscripten-1.2.1/itkwasm_mesh_io_emscripten/free_surfer_binary_write_mesh_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io_emscripten-1.2.0/itkwasm_mesh_io_emscripten/js_package.py` & `itkwasm_mesh_io_emscripten-1.2.1/itkwasm_mesh_io_emscripten/js_package.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io_emscripten-1.2.0/itkwasm_mesh_io_emscripten/obj_read_mesh_async.py` & `itkwasm_mesh_io_emscripten-1.2.1/itkwasm_mesh_io_emscripten/obj_read_mesh_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io_emscripten-1.2.0/itkwasm_mesh_io_emscripten/obj_write_mesh_async.py` & `itkwasm_mesh_io_emscripten-1.2.1/itkwasm_mesh_io_emscripten/obj_write_mesh_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io_emscripten-1.2.0/itkwasm_mesh_io_emscripten/off_read_mesh_async.py` & `itkwasm_mesh_io_emscripten-1.2.1/itkwasm_mesh_io_emscripten/off_read_mesh_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io_emscripten-1.2.0/itkwasm_mesh_io_emscripten/off_write_mesh_async.py` & `itkwasm_mesh_io_emscripten-1.2.1/itkwasm_mesh_io_emscripten/off_write_mesh_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io_emscripten-1.2.0/itkwasm_mesh_io_emscripten/read_mesh_async.py` & `itkwasm_mesh_io_emscripten-1.2.1/itkwasm_mesh_io_emscripten/read_mesh_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io_emscripten-1.2.0/itkwasm_mesh_io_emscripten/stl_read_mesh_async.py` & `itkwasm_mesh_io_emscripten-1.2.1/itkwasm_mesh_io_emscripten/stl_read_mesh_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io_emscripten-1.2.0/itkwasm_mesh_io_emscripten/stl_write_mesh_async.py` & `itkwasm_mesh_io_emscripten-1.2.1/itkwasm_mesh_io_emscripten/stl_write_mesh_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io_emscripten-1.2.0/itkwasm_mesh_io_emscripten/swc_read_mesh_async.py` & `itkwasm_mesh_io_emscripten-1.2.1/itkwasm_mesh_io_emscripten/swc_read_mesh_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io_emscripten-1.2.0/itkwasm_mesh_io_emscripten/swc_write_mesh_async.py` & `itkwasm_mesh_io_emscripten-1.2.1/itkwasm_mesh_io_emscripten/swc_write_mesh_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io_emscripten-1.2.0/itkwasm_mesh_io_emscripten/vtk_poly_data_read_mesh_async.py` & `itkwasm_mesh_io_emscripten-1.2.1/itkwasm_mesh_io_emscripten/vtk_poly_data_read_mesh_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io_emscripten-1.2.0/itkwasm_mesh_io_emscripten/vtk_poly_data_write_mesh_async.py` & `itkwasm_mesh_io_emscripten-1.2.1/itkwasm_mesh_io_emscripten/vtk_poly_data_write_mesh_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io_emscripten-1.2.0/itkwasm_mesh_io_emscripten/wasm_read_mesh_async.py` & `itkwasm_mesh_io_emscripten-1.2.1/itkwasm_mesh_io_emscripten/wasm_read_mesh_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io_emscripten-1.2.0/itkwasm_mesh_io_emscripten/wasm_write_mesh_async.py` & `itkwasm_mesh_io_emscripten-1.2.1/itkwasm_mesh_io_emscripten/wasm_write_mesh_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io_emscripten-1.2.0/itkwasm_mesh_io_emscripten/wasm_zstd_read_mesh_async.py` & `itkwasm_mesh_io_emscripten-1.2.1/itkwasm_mesh_io_emscripten/wasm_zstd_read_mesh_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io_emscripten-1.2.0/itkwasm_mesh_io_emscripten/wasm_zstd_write_mesh_async.py` & `itkwasm_mesh_io_emscripten-1.2.1/itkwasm_mesh_io_emscripten/wasm_zstd_write_mesh_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io_emscripten-1.2.0/itkwasm_mesh_io_emscripten/wasm_ztd_read_mesh_async.py` & `itkwasm_mesh_io_emscripten-1.2.1/itkwasm_mesh_io_emscripten/wasm_ztd_read_mesh_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io_emscripten-1.2.0/itkwasm_mesh_io_emscripten/wasm_ztd_write_mesh_async.py` & `itkwasm_mesh_io_emscripten-1.2.1/itkwasm_mesh_io_emscripten/wasm_ztd_write_mesh_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io_emscripten-1.2.0/itkwasm_mesh_io_emscripten/write_mesh_async.py` & `itkwasm_mesh_io_emscripten-1.2.1/itkwasm_mesh_io_emscripten/write_mesh_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io_emscripten-1.2.0/README.md` & `itkwasm_mesh_io_emscripten-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io_emscripten-1.2.0/pyproject.toml` & `itkwasm_mesh_io_emscripten-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
 [tool.hatch.envs.default.scripts]
 test = [
   "hatch build -t wheel ./dist/pyodide/",
   "pytest --dist-dir=./dist/pyodide --rt=chrome",
 ]
 download-pyodide = [
-  "curl -L https://github.com/pyodide/pyodide/releases/download/0.24.1/pyodide-0.24.1.tar.bz2 -o pyodide.tar.bz2",
+  "curl -L https://github.com/pyodide/pyodide/releases/download/0.25.1/pyodide-0.25.1.tar.bz2 -o pyodide.tar.bz2",
   "tar xjf pyodide.tar.bz2",
   "rm -rf dist/pyodide pyodide.tar.bz2",
   "mkdir -p dist",
   "mv pyodide dist",
 ]
 serve = [
   "hatch build -t wheel ./dist/pyodide/",
```

### Comparing `itkwasm_mesh_io_emscripten-1.2.0/PKG-INFO` & `itkwasm_mesh_io_emscripten-1.2.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itkwasm-mesh-io-emscripten
-Version: 1.2.0
+Version: 1.2.1
 Summary: Input and output for scientific and medical image file formats.
 Project-URL: Home, https://github.com/InsightSoftwareConsortium/itk-wasm
 Project-URL: Source, https://github.com/InsightSoftwareConsortium/itk-wasm
 License-Expression: Apache-2.0
 Keywords: emscripten,itkwasm,webassembly
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: WebAssembly
```

