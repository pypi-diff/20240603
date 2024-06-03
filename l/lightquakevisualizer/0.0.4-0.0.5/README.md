# Comparing `tmp/lightquakevisualizer-0.0.4.tar.gz` & `tmp/lightquakevisualizer-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightquakevisualizer-0.0.4.tar", last modified: Tue May 28 13:23:47 2024, max compression
+gzip compressed data, was "lightquakevisualizer-0.0.5.tar", last modified: Mon Jun  3 07:54:34 2024, max compression
```

## Comparing `lightquakevisualizer-0.0.4.tar` & `lightquakevisualizer-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 ulrich    (1000) ulrich    (1000)        0 2024-05-28 13:23:47.670257 lightquakevisualizer-0.0.4/
--rw-rw-r--   0 ulrich    (1000) ulrich    (1000)     1074 2024-05-14 14:46:16.000000 lightquakevisualizer-0.0.4/LICENSE
--rw-r--r--   0 ulrich    (1000) ulrich    (1000)     2507 2024-05-28 13:23:47.670257 lightquakevisualizer-0.0.4/PKG-INFO
--rw-rw-r--   0 ulrich    (1000) ulrich    (1000)     1847 2024-05-16 17:17:10.000000 lightquakevisualizer-0.0.4/README.md
-drwxrwxr-x   0 ulrich    (1000) ulrich    (1000)        0 2024-05-28 13:23:47.670257 lightquakevisualizer-0.0.4/lightquakevisualizer/
--rw-rw-r--   0 ulrich    (1000) ulrich    (1000)        0 2024-05-16 12:02:30.000000 lightquakevisualizer-0.0.4/lightquakevisualizer/__init__.py
--rwxrwxr-x   0 ulrich    (1000) ulrich    (1000)     6047 2024-05-16 12:47:50.000000 lightquakevisualizer-0.0.4/lightquakevisualizer/generateColorBar.py
--rwxrwxr-x   0 ulrich    (1000) ulrich    (1000)     2600 2024-05-16 12:47:50.000000 lightquakevisualizer-0.0.4/lightquakevisualizer/imageCombiner.py
--rw-rw-r--   0 ulrich    (1000) ulrich    (1000)     2787 2024-05-16 12:47:50.000000 lightquakevisualizer-0.0.4/lightquakevisualizer/imageCombinernew.py
--rwxrwxr-x   0 ulrich    (1000) ulrich    (1000)    23507 2024-05-28 13:22:12.000000 lightquakevisualizer-0.0.4/lightquakevisualizer/lightQuakeVisualizer.py
-drwxrwxr-x   0 ulrich    (1000) ulrich    (1000)        0 2024-05-28 13:23:47.670257 lightquakevisualizer-0.0.4/lightquakevisualizer.egg-info/
--rw-r--r--   0 ulrich    (1000) ulrich    (1000)     2507 2024-05-28 13:23:47.000000 lightquakevisualizer-0.0.4/lightquakevisualizer.egg-info/PKG-INFO
--rw-rw-r--   0 ulrich    (1000) ulrich    (1000)      496 2024-05-28 13:23:47.000000 lightquakevisualizer-0.0.4/lightquakevisualizer.egg-info/SOURCES.txt
--rw-rw-r--   0 ulrich    (1000) ulrich    (1000)        1 2024-05-28 13:23:47.000000 lightquakevisualizer-0.0.4/lightquakevisualizer.egg-info/dependency_links.txt
--rw-rw-r--   0 ulrich    (1000) ulrich    (1000)      211 2024-05-28 13:23:47.000000 lightquakevisualizer-0.0.4/lightquakevisualizer.egg-info/entry_points.txt
--rw-rw-r--   0 ulrich    (1000) ulrich    (1000)       73 2024-05-28 13:23:47.000000 lightquakevisualizer-0.0.4/lightquakevisualizer.egg-info/requires.txt
--rw-rw-r--   0 ulrich    (1000) ulrich    (1000)       21 2024-05-28 13:23:47.000000 lightquakevisualizer-0.0.4/lightquakevisualizer.egg-info/top_level.txt
--rw-rw-r--   0 ulrich    (1000) ulrich    (1000)      921 2024-05-28 13:23:18.000000 lightquakevisualizer-0.0.4/pyproject.toml
--rw-rw-r--   0 ulrich    (1000) ulrich    (1000)       38 2024-05-28 13:23:47.670257 lightquakevisualizer-0.0.4/setup.cfg
+drwxrwxr-x   0 ulrich    (1000) ulrich    (1000)        0 2024-06-03 07:54:34.963529 lightquakevisualizer-0.0.5/
+-rw-rw-r--   0 ulrich    (1000) ulrich    (1000)     1074 2024-05-14 14:46:16.000000 lightquakevisualizer-0.0.5/LICENSE
+-rw-r--r--   0 ulrich    (1000) ulrich    (1000)     2507 2024-06-03 07:54:34.963529 lightquakevisualizer-0.0.5/PKG-INFO
+-rw-rw-r--   0 ulrich    (1000) ulrich    (1000)     1847 2024-05-16 17:17:10.000000 lightquakevisualizer-0.0.5/README.md
+drwxrwxr-x   0 ulrich    (1000) ulrich    (1000)        0 2024-06-03 07:54:34.959529 lightquakevisualizer-0.0.5/lightquakevisualizer/
+-rw-rw-r--   0 ulrich    (1000) ulrich    (1000)        0 2024-05-16 12:02:30.000000 lightquakevisualizer-0.0.5/lightquakevisualizer/__init__.py
+-rwxrwxr-x   0 ulrich    (1000) ulrich    (1000)     6047 2024-05-16 12:47:50.000000 lightquakevisualizer-0.0.5/lightquakevisualizer/generateColorBar.py
+-rwxrwxr-x   0 ulrich    (1000) ulrich    (1000)     2600 2024-05-16 12:47:50.000000 lightquakevisualizer-0.0.5/lightquakevisualizer/imageCombiner.py
+-rw-rw-r--   0 ulrich    (1000) ulrich    (1000)     2787 2024-05-16 12:47:50.000000 lightquakevisualizer-0.0.5/lightquakevisualizer/imageCombinernew.py
+-rwxrwxr-x   0 ulrich    (1000) ulrich    (1000)    23925 2024-06-03 07:52:20.000000 lightquakevisualizer-0.0.5/lightquakevisualizer/lightQuakeVisualizer.py
+drwxrwxr-x   0 ulrich    (1000) ulrich    (1000)        0 2024-06-03 07:54:34.963529 lightquakevisualizer-0.0.5/lightquakevisualizer.egg-info/
+-rw-r--r--   0 ulrich    (1000) ulrich    (1000)     2507 2024-06-03 07:54:34.000000 lightquakevisualizer-0.0.5/lightquakevisualizer.egg-info/PKG-INFO
+-rw-rw-r--   0 ulrich    (1000) ulrich    (1000)      496 2024-06-03 07:54:34.000000 lightquakevisualizer-0.0.5/lightquakevisualizer.egg-info/SOURCES.txt
+-rw-rw-r--   0 ulrich    (1000) ulrich    (1000)        1 2024-06-03 07:54:34.000000 lightquakevisualizer-0.0.5/lightquakevisualizer.egg-info/dependency_links.txt
+-rw-rw-r--   0 ulrich    (1000) ulrich    (1000)      211 2024-06-03 07:54:34.000000 lightquakevisualizer-0.0.5/lightquakevisualizer.egg-info/entry_points.txt
+-rw-rw-r--   0 ulrich    (1000) ulrich    (1000)       73 2024-06-03 07:54:34.000000 lightquakevisualizer-0.0.5/lightquakevisualizer.egg-info/requires.txt
+-rw-rw-r--   0 ulrich    (1000) ulrich    (1000)       21 2024-06-03 07:54:34.000000 lightquakevisualizer-0.0.5/lightquakevisualizer.egg-info/top_level.txt
+-rw-rw-r--   0 ulrich    (1000) ulrich    (1000)      921 2024-06-03 07:53:03.000000 lightquakevisualizer-0.0.5/pyproject.toml
+-rw-rw-r--   0 ulrich    (1000) ulrich    (1000)       38 2024-06-03 07:54:34.963529 lightquakevisualizer-0.0.5/setup.cfg
```

### Comparing `lightquakevisualizer-0.0.4/LICENSE` & `lightquakevisualizer-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lightquakevisualizer-0.0.4/PKG-INFO` & `lightquakevisualizer-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightquakevisualizer
-Version: 0.0.4
+Version: 0.0.5
 Summary: A collection of scripts to visualize SeisSol output using pyvista
 Author: Thomas Ulrich
 License: MIT
 Project-URL: Repository, https://github.com/Thomas-Ulrich/light-quake-visualizer.git
 Keywords: pyvista,SeisSol
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `lightquakevisualizer-0.0.4/README.md` & `lightquakevisualizer-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `lightquakevisualizer-0.0.4/lightquakevisualizer/generateColorBar.py` & `lightquakevisualizer-0.0.5/lightquakevisualizer/generateColorBar.py`

 * *Files identical despite different names*

### Comparing `lightquakevisualizer-0.0.4/lightquakevisualizer/imageCombiner.py` & `lightquakevisualizer-0.0.5/lightquakevisualizer/imageCombiner.py`

 * *Files identical despite different names*

### Comparing `lightquakevisualizer-0.0.4/lightquakevisualizer/imageCombinernew.py` & `lightquakevisualizer-0.0.5/lightquakevisualizer/imageCombinernew.py`

 * *Files identical despite different names*

### Comparing `lightquakevisualizer-0.0.4/lightquakevisualizer/lightQuakeVisualizer.py` & `lightquakevisualizer-0.0.5/lightquakevisualizer/lightQuakeVisualizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -401,14 +401,20 @@
         metavar=("specular", "diffuse", "ambient"),
         help="Lighting parameters",
         type=float,
         default=([0.1, 0.8, 0.5]),
     )
 
     parser.add_argument(
+        "--log_scale",
+        nargs=1,
+        help="Log color scale. 1: log scale, 0: linear scale. n values separated by ';'",
+    )
+
+    parser.add_argument(
         "--opacity",
         nargs=1,
         help="Opacity values, separated by ';'",
     )
 
     parser.add_argument(
         "--output_prefix", nargs=1, help="Specify output prefix of the snapshot"
@@ -486,14 +492,22 @@
     if not os.path.exists("output") and not args.interactive:
         os.makedirs("output")
 
     fnames = args.input_files.split(";")
     variables = args.variables[0].split(";")
     cmap_names = args.cmap[0].split(";")
     nfiles = len(fnames)
+
+    use_log_scale = (
+        [True if int(v) else False for v in args.log_scale[0].split(";")]
+        if args.log_scale
+        else np.zeros(nfiles, dtype=bool)
+    )
+    assert len(use_log_scale) == nfiles
+
     opacity = (
         [float(v) for v in args.opacity[0].split(";")]
         if args.opacity
         else np.ones(nfiles)
     )
     assert len(opacity) == nfiles
 
@@ -620,14 +634,15 @@
                 scalar_bar_dic = {}
 
             plotter.add_mesh(
                 mesh,
                 cmap=cmaps[i],
                 scalars=var,
                 **lighting,
+                log_scale=use_log_scale[i],
                 opacity=opacity[i],
                 **clim_dic,
                 **scalar_bar_dic,
             )
 
             if args.contours:
                 add_contours(plotter, grid, sx, i, idx[0], args.contours[0])
```

### Comparing `lightquakevisualizer-0.0.4/lightquakevisualizer.egg-info/PKG-INFO` & `lightquakevisualizer-0.0.5/lightquakevisualizer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightquakevisualizer
-Version: 0.0.4
+Version: 0.0.5
 Summary: A collection of scripts to visualize SeisSol output using pyvista
 Author: Thomas Ulrich
 License: MIT
 Project-URL: Repository, https://github.com/Thomas-Ulrich/light-quake-visualizer.git
 Keywords: pyvista,SeisSol
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `lightquakevisualizer-0.0.4/pyproject.toml` & `lightquakevisualizer-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lightquakevisualizer"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
     {name = "Thomas Ulrich"},
 ]
 description = "A collection of scripts to visualize SeisSol output using pyvista"
 readme = "README.md"
 requires-python = ">=3.10"
 keywords = ["pyvista", "SeisSol"]
```

