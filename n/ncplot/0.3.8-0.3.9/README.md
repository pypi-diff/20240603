# Comparing `tmp/ncplot-0.3.8.tar.gz` & `tmp/ncplot-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncplot-0.3.8.tar", last modified: Mon Dec  4 18:15:12 2023, max compression
+gzip compressed data, was "ncplot-0.3.9.tar", last modified: Wed Feb 28 14:05:08 2024, max compression
```

## Comparing `ncplot-0.3.8.tar` & `ncplot-0.3.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 18:15:12.982355 ncplot-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2023-12-04 18:14:59.000000 ncplot-0.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      564 2023-12-04 18:14:59.000000 ncplot-0.3.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2916 2023-12-04 18:15:12.982355 ncplot-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2023-12-04 18:14:59.000000 ncplot-0.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 18:15:12.982355 ncplot-0.3.8/ncplot/
--rwxr-xr-x   0 runner    (1001) docker     (127)       29 2023-12-04 18:15:00.000000 ncplot-0.3.8/ncplot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2023-12-04 18:15:00.000000 ncplot-0.3.8/ncplot/command_line.py
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 18:15:00.000000 ncplot-0.3.8/ncplot/deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)    35816 2023-12-04 18:15:00.000000 ncplot-0.3.8/ncplot/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     5149 2023-12-04 18:15:00.000000 ncplot-0.3.8/ncplot/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2023-12-04 18:15:00.000000 ncplot-0.3.8/ncplot/xarray.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 18:15:12.982355 ncplot-0.3.8/ncplot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2023-12-04 18:15:12.000000 ncplot-0.3.8/ncplot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)       78 2023-12-04 18:15:00.000000 ncplot-0.3.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-04 18:15:12.982355 ncplot-0.3.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     2053 2023-12-04 18:15:00.000000 ncplot-0.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 14:05:08.658947 ncplot-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-28 14:04:54.000000 ncplot-0.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-02-28 14:04:54.000000 ncplot-0.3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2916 2024-02-28 14:05:08.658947 ncplot-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-02-28 14:04:54.000000 ncplot-0.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 14:05:08.658947 ncplot-0.3.9/ncplot/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       29 2024-02-28 14:04:54.000000 ncplot-0.3.9/ncplot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-02-28 14:04:54.000000 ncplot-0.3.9/ncplot/command_line.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 14:04:54.000000 ncplot-0.3.9/ncplot/deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35034 2024-02-28 14:04:54.000000 ncplot-0.3.9/ncplot/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5149 2024-02-28 14:04:54.000000 ncplot-0.3.9/ncplot/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-02-28 14:04:54.000000 ncplot-0.3.9/ncplot/xarray.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 14:05:08.658947 ncplot-0.3.9/ncplot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-02-28 14:05:08.000000 ncplot-0.3.9/ncplot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-02-28 14:04:54.000000 ncplot-0.3.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-28 14:05:08.658947 ncplot-0.3.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2053 2024-02-28 14:04:54.000000 ncplot-0.3.9/setup.py
```

### Comparing `ncplot-0.3.8/LICENSE` & `ncplot-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ncplot-0.3.8/MANIFEST.in` & `ncplot-0.3.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `ncplot-0.3.8/PKG-INFO` & `ncplot-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncplot
-Version: 0.3.8
+Version: 0.3.9
 Summary: Interactive viewing of NetCDF data
 Home-page: https://github.com/pmlmodelling/ncplot
 Author: Robert Wilson
 Author-email: rwi@pml.ac.uk
 Maintainer: Robert Wilson
 Project-URL: Bug Tracker, https://github.com/pmlmodelling/ncplot/issues
 Project-URL: Documentation, https://ncplot.readthedocs.io/en/stable
```

### Comparing `ncplot-0.3.8/README.md` & `ncplot-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `ncplot-0.3.8/ncplot/command_line.py` & `ncplot-0.3.9/ncplot/command_line.py`

 * *Files identical despite different names*

### Comparing `ncplot-0.3.8/ncplot/plot.py` & `ncplot-0.3.9/ncplot/plot.py`

 * *Files 3% similar despite different names*

```diff
@@ -161,24 +161,27 @@
 
     if "spyder" in sys.modules:
         return False
 
     return "ipykernel" in sys.modules
 
 
-def view(x, vars=None, autoscale=True, out=None, server = None, **kwargs):
+def view(x, vars=None, autoscale=True, out=None, **kwargs):
     """
     Plot the contents of a NetCDF out
 
     Parameters
     -------------
     x : object or str
         xarray object or file  path
     vars : list or str
         Variables you want to plot. Everything will be plotted if this is not supplied
+    autoscale : bool
+        Set to False if you do not want the colour scales to vary. Defaults to True, which sets
+        scales based on minimum and maximum values.
 
     out : str
         Name of file if you want to store output
 
     """
 
     if "clim" in kwargs:
@@ -543,19 +546,14 @@
             else:
                 hvplot.save(intplot, out)
                 return None
 
         t = Thread(target=ctrc)
         t.start()
 
-        # create a panel server if server specified
-
-        bokeh_server = pn.panel(intplot, sizing_mode="stretch_both", websocket_origin = server).show(
-            threaded=False
-        )
         return None
 
     # heat map where 2 coords have more than 1 value, not a spatial map
     if len([x for x in coord_df.length if x > 1]) == 2 and spatial_map is False:
 
         df = ds.to_dataframe().reset_index()
         x_var = coord_df.query("length > 1").reset_index().coord[0]
@@ -688,17 +686,14 @@
                     return None
             if out is not None:
                 hvplot.save(intplot, out)
                 return None
 
             t = Thread(target=ctrc)
             t.start()
-            bokeh_server = pn.panel(intplot, sizing_mode="stretch_both").show(
-                threaded=False
-            )
             return None
 
     # heat map where 3 coords have more than 1 value, and one of them is time. Not a spatial map though
     if len([x for x in coord_df.length if x > 1]) == 3:
 
         non_map = True
 
@@ -804,17 +799,14 @@
                             return intplot
                         else:
                             hvplot.save(intplot, out)
                             return None
 
                     t = Thread(target=ctrc)
                     t.start()
-                    bokeh_server = pn.panel(intplot, sizing_mode="stretch_both").show(
-                        threaded=False
-                    )
                     return None
 
     if (n_times > 1) and (n_points < 2) and (n_levels <= 1):
 
         if type(vars) is str:
             vars = [vars]
 
@@ -856,17 +848,14 @@
             else:
                 hvplot.save(intplot, out)
                 return None
 
         t = Thread(target=ctrc)
         t.start()
 
-        bokeh_server = pn.panel(intplot, sizing_mode="stretch_both").show(
-            threaded=False
-        )
         return None
 
     if (n_points > 1) and (n_levels >= 1) and (type(vars) is list):
 
         if quadmesh:
 
             if coastline:
@@ -925,17 +914,14 @@
                 return intplot
             else:
                 hvplot.save(intplot, out)
                 return None
 
         t = Thread(target=ctrc)
         t.start()
-        bokeh_server = pn.panel(intplot, sizing_mode="stretch_both").show(
-            threaded=False
-        )
         return None
 
     if n_points > 1:
 
         if type(vars) is list:
             warnings.warn(message="Warning: Only the first variable is mapped")
             vars = vars[0]
@@ -1035,17 +1021,14 @@
                     return intplot
                 else:
                     hvplot.save(intplot, out)
                     return None
 
             t = Thread(target=ctrc)
             t.start()
-            bokeh_server = pn.panel(intplot, sizing_mode="stretch_both").show(
-                threaded=False
-            )
             return None
 
         else:
             if quadmesh:
                 if coastline:
                     coastline = get_coastline(ds, lon_name, lat_name)
                     try:
@@ -1131,17 +1114,14 @@
                     return intplot
                 else:
                     hvplot.save(intplot, out)
                     return None
 
             t = Thread(target=ctrc)
             t.start()
-            bokeh_server = pn.panel(intplot, sizing_mode="stretch_both").show(
-                threaded=False
-            )
 
             return None
 
     # it's possible that the data has not spatial or temporal coordinates. Do something about it....
 
     # Throw an error if case has not plotting method available yet
     # right now this only seems to be when you have lon/lat/time/levels and multiple variables
```

### Comparing `ncplot-0.3.8/ncplot/utils.py` & `ncplot-0.3.9/ncplot/utils.py`

 * *Files identical despite different names*

### Comparing `ncplot-0.3.8/ncplot/xarray.py` & `ncplot-0.3.9/ncplot/xarray.py`

 * *Files identical despite different names*

### Comparing `ncplot-0.3.8/setup.py` & `ncplot-0.3.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         ],
 }
 
 
 extras_require["complete"] = ["geoviews"]
 
 setup(name='ncplot',
-      version='0.3.8',
+      version='0.3.9',
       description=DESCRIPTION,
       long_description=long_description,
       long_description_content_type='text/markdown',
 
       python_requires='>=3.6.1',
 
       entry_points={
```

