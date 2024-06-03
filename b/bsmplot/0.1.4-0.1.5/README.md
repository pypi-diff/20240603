# Comparing `tmp/bsmplot-0.1.4.tar.gz` & `tmp/bsmplot-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bsmplot-0.1.4.tar", last modified: Sun Mar 31 04:05:28 2024, max compression
+gzip compressed data, was "bsmplot-0.1.5.tar", last modified: Mon Jun  3 04:17:06 2024, max compression
```

## Comparing `bsmplot-0.1.4.tar` & `bsmplot-0.1.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 tianzhuqiao   (501) staff       (20)        0 2024-03-31 04:05:28.411136 bsmplot-0.1.4/
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)     1069 2024-02-11 17:37:54.000000 bsmplot-0.1.4/LICENSE
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)     2480 2024-03-31 04:05:28.410447 bsmplot-0.1.4/PKG-INFO
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)      499 2024-02-24 18:36:47.000000 bsmplot-0.1.4/README.md
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)       91 2024-02-10 16:17:02.000000 bsmplot-0.1.4/README_pip.md
-drwxr-xr-x   0 tianzhuqiao   (501) staff       (20)        0 2024-03-31 04:05:28.396270 bsmplot-0.1.4/bsmplot/
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)       96 2024-02-11 17:37:54.000000 bsmplot-0.1.4/bsmplot/__init__.py
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)     1791 2024-02-11 17:37:54.000000 bsmplot-0.1.4/bsmplot/__main__.py
-drwxr-xr-x   0 tianzhuqiao   (501) staff       (20)        0 2024-03-31 04:05:28.406244 bsmplot-0.1.4/bsmplot/bsm/
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)      123 2024-02-13 22:01:59.000000 bsmplot-0.1.4/bsmplot/bsm/__init__.py
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)     1849 2024-02-14 05:11:17.000000 bsmplot-0.1.4/bsmplot/bsm/bsmbackend.py
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)     2685 2024-03-28 05:12:02.000000 bsmplot-0.1.4/bsmplot/bsm/csvs.py
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)      156 2024-02-14 04:46:03.000000 bsmplot-0.1.4/bsmplot/bsm/debugtool.py
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)      482 2024-02-14 01:04:10.000000 bsmplot-0.1.4/bsmplot/bsm/editor.py
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)     9558 2024-03-11 02:45:44.000000 bsmplot-0.1.4/bsmplot/bsm/graph.py
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)     4508 2024-03-29 00:56:02.000000 bsmplot-0.1.4/bsmplot/bsm/mat.py
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)      156 2024-02-14 04:33:23.000000 bsmplot-0.1.4/bsmplot/bsm/misctools.py
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)     9383 2024-02-11 17:37:54.000000 bsmplot-0.1.4/bsmplot/bsm/parsetab.py
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)     1827 2024-02-17 20:28:00.000000 bsmplot-0.1.4/bsmplot/bsm/shell.py
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)     9310 2024-03-28 05:12:02.000000 bsmplot-0.1.4/bsmplot/bsm/ulog.py
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)     9382 2024-02-11 17:37:54.000000 bsmplot-0.1.4/bsmplot/bsm/utility.py
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)    20293 2024-03-30 03:33:04.000000 bsmplot-0.1.4/bsmplot/bsm/vcds.py
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)    19009 2024-03-28 05:12:02.000000 bsmplot-0.1.4/bsmplot/bsm/zmqs.py
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)    17218 2024-03-11 03:11:24.000000 bsmplot-0.1.4/bsmplot/mainframe.py
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)      671 2024-02-11 17:37:54.000000 bsmplot-0.1.4/bsmplot/mainframexpm.py
-drwxr-xr-x   0 tianzhuqiao   (501) staff       (20)        0 2024-03-31 04:05:28.409099 bsmplot-0.1.4/bsmplot/pvcd/
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)     1098 2024-02-11 17:37:54.000000 bsmplot-0.1.4/bsmplot/pvcd/lextab.py
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)     8488 2024-02-11 17:37:54.000000 bsmplot-0.1.4/bsmplot/pvcd/parsetab.py
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)    11561 2024-03-30 03:34:08.000000 bsmplot-0.1.4/bsmplot/pvcd/pvcd.py
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)    13258 2024-02-11 17:37:54.000000 bsmplot-0.1.4/bsmplot/pvcd/pvcd2.py
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)      183 2024-03-30 05:41:43.000000 bsmplot-0.1.4/bsmplot/version.py
-drwxr-xr-x   0 tianzhuqiao   (501) staff       (20)        0 2024-03-31 04:05:28.409746 bsmplot-0.1.4/bsmplot.egg-info/
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)     2480 2024-03-31 04:05:28.000000 bsmplot-0.1.4/bsmplot.egg-info/PKG-INFO
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)      739 2024-03-31 04:05:28.000000 bsmplot-0.1.4/bsmplot.egg-info/SOURCES.txt
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)        1 2024-03-31 04:05:28.000000 bsmplot-0.1.4/bsmplot.egg-info/dependency_links.txt
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)       46 2024-03-31 04:05:28.000000 bsmplot-0.1.4/bsmplot.egg-info/entry_points.txt
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)      166 2024-03-31 04:05:28.000000 bsmplot-0.1.4/bsmplot.egg-info/requires.txt
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)       18 2024-03-31 04:05:28.000000 bsmplot-0.1.4/bsmplot.egg-info/top_level.txt
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)      943 2024-03-31 04:04:57.000000 bsmplot-0.1.4/pyproject.toml
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)       38 2024-03-31 04:05:28.411290 bsmplot-0.1.4/setup.cfg
+drwxr-xr-x   0 tianzhuqiao   (501) staff       (20)        0 2024-06-03 04:17:06.379962 bsmplot-0.1.5/
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     1069 2024-02-11 17:37:54.000000 bsmplot-0.1.5/LICENSE
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     2500 2024-06-03 04:17:06.378968 bsmplot-0.1.5/PKG-INFO
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)      499 2024-02-24 18:36:47.000000 bsmplot-0.1.5/README.md
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)       91 2024-02-10 16:17:02.000000 bsmplot-0.1.5/README_pip.md
+drwxr-xr-x   0 tianzhuqiao   (501) staff       (20)        0 2024-06-03 04:17:06.349926 bsmplot-0.1.5/bsmplot/
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)       96 2024-02-11 17:37:54.000000 bsmplot-0.1.5/bsmplot/__init__.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     1791 2024-02-11 17:37:54.000000 bsmplot-0.1.5/bsmplot/__main__.py
+drwxr-xr-x   0 tianzhuqiao   (501) staff       (20)        0 2024-06-03 04:17:06.370504 bsmplot-0.1.5/bsmplot/bsm/
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)      123 2024-02-13 22:01:59.000000 bsmplot-0.1.5/bsmplot/bsm/__init__.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     1849 2024-02-14 05:11:17.000000 bsmplot-0.1.5/bsmplot/bsm/bsmbackend.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     2685 2024-03-28 05:12:02.000000 bsmplot-0.1.5/bsmplot/bsm/csvs.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)      156 2024-02-14 04:46:03.000000 bsmplot-0.1.5/bsmplot/bsm/debugtool.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)      482 2024-02-14 01:04:10.000000 bsmplot-0.1.5/bsmplot/bsm/editor.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     9623 2024-06-03 04:04:26.000000 bsmplot-0.1.5/bsmplot/bsm/graph.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     4873 2024-05-31 05:00:28.000000 bsmplot-0.1.5/bsmplot/bsm/mat.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)      156 2024-02-14 04:33:23.000000 bsmplot-0.1.5/bsmplot/bsm/misctools.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     9383 2024-02-11 17:37:54.000000 bsmplot-0.1.5/bsmplot/bsm/parsetab.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     1827 2024-02-17 20:28:00.000000 bsmplot-0.1.5/bsmplot/bsm/shell.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     9310 2024-03-28 05:12:02.000000 bsmplot-0.1.5/bsmplot/bsm/ulog.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     9382 2024-02-11 17:37:54.000000 bsmplot-0.1.5/bsmplot/bsm/utility.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)    20293 2024-03-30 03:33:04.000000 bsmplot-0.1.5/bsmplot/bsm/vcds.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)    19009 2024-03-28 05:12:02.000000 bsmplot-0.1.5/bsmplot/bsm/zmqs.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)    17218 2024-03-11 03:11:24.000000 bsmplot-0.1.5/bsmplot/mainframe.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)      671 2024-02-11 17:37:54.000000 bsmplot-0.1.5/bsmplot/mainframexpm.py
+drwxr-xr-x   0 tianzhuqiao   (501) staff       (20)        0 2024-06-03 04:17:06.376577 bsmplot-0.1.5/bsmplot/pvcd/
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     1098 2024-02-11 17:37:54.000000 bsmplot-0.1.5/bsmplot/pvcd/lextab.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     8488 2024-02-11 17:37:54.000000 bsmplot-0.1.5/bsmplot/pvcd/parsetab.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)    11561 2024-03-30 03:34:08.000000 bsmplot-0.1.5/bsmplot/pvcd/pvcd.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)    13258 2024-02-11 17:37:54.000000 bsmplot-0.1.5/bsmplot/pvcd/pvcd2.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)      183 2024-06-03 04:16:25.000000 bsmplot-0.1.5/bsmplot/version.py
+drwxr-xr-x   0 tianzhuqiao   (501) staff       (20)        0 2024-06-03 04:17:06.377935 bsmplot-0.1.5/bsmplot.egg-info/
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     2500 2024-06-03 04:17:06.000000 bsmplot-0.1.5/bsmplot.egg-info/PKG-INFO
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)      739 2024-06-03 04:17:06.000000 bsmplot-0.1.5/bsmplot.egg-info/SOURCES.txt
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)        1 2024-06-03 04:17:06.000000 bsmplot-0.1.5/bsmplot.egg-info/dependency_links.txt
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)       46 2024-06-03 04:17:06.000000 bsmplot-0.1.5/bsmplot.egg-info/entry_points.txt
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)      171 2024-06-03 04:17:06.000000 bsmplot-0.1.5/bsmplot.egg-info/requires.txt
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)       18 2024-06-03 04:17:06.000000 bsmplot-0.1.5/bsmplot.egg-info/top_level.txt
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)      951 2024-06-03 04:13:38.000000 bsmplot-0.1.5/pyproject.toml
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)       38 2024-06-03 04:17:06.380123 bsmplot-0.1.5/setup.cfg
```

### Comparing `bsmplot-0.1.4/LICENSE` & `bsmplot-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bsmplot-0.1.4/PKG-INFO` & `bsmplot-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bsmplot
-Version: 0.1.4
+Version: 0.1.5
 Summary: bsmplot is a tool to visualize time series
 Author-email: Tianzhu Qiao <tq@feiyilin.com>
 License: MIT License
         
         Copyright (c) 2024 Tianzhu Qiao
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -34,21 +34,22 @@
 Requires-Dist: matplotlib>=3.8.1
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: click>=8.1
 Requires-Dist: pandas
 Requires-Dist: pyulog
 Requires-Dist: pyvcd
-Requires-Dist: propgrid>=0.1.3
-Requires-Dist: mplpanel>=0.1.2
+Requires-Dist: propgrid>=0.1.4
+Requires-Dist: mplpanel>=0.1.3
 Requires-Dist: aui2>=0.1.4
 Requires-Dist: zmq
-Requires-Dist: bsmutility>=0.1.3
+Requires-Dist: bsmutility>=0.1.4
 Requires-Dist: ply
 Requires-Dist: charset_normalizer
+Requires-Dist: h5py
 
 # bsmplot
 **bsmplot** is a cross-platform tool to visualize time series based on [Matplotlib](https://matplotlib.org/) and [wxPython](https://wxpython.org/). Supported data source
 - VCD (value change dump)
 - PX4 [ulog](https://docs.px4.io/main/en/dev_log/ulog_file_format.html)
 - CSV
 - Matlab .mat
```

### Comparing `bsmplot-0.1.4/bsmplot/__main__.py` & `bsmplot-0.1.5/bsmplot/__main__.py`

 * *Files identical despite different names*

### Comparing `bsmplot-0.1.4/bsmplot/bsm/bsmbackend.py` & `bsmplot-0.1.5/bsmplot/bsm/bsmbackend.py`

 * *Files identical despite different names*

### Comparing `bsmplot-0.1.4/bsmplot/bsm/csvs.py` & `bsmplot-0.1.5/bsmplot/bsm/csvs.py`

 * *Files identical despite different names*

### Comparing `bsmplot-0.1.4/bsmplot/bsm/graph.py` & `bsmplot-0.1.5/bsmplot/bsm/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,20 +49,23 @@
         return d
 
 class MatplotPanel(MPLPanel):
 
     def __init__(self, parent, title=None, num=-1, thisFig=None):
         MPLPanel.__init__(self, parent, title, num, thisFig)
 
-        dp.connect(self.simLoad, 'sim.loaded')
         dp.connect(self.DataUpdated, 'graph.data_updated')
 
         dt = DataDropTarget(self.canvas)
         self.canvas.SetDropTarget(dt)
 
+    def Destroy(self):
+        dp.disconnect(self.DataUpdated, 'graph.data_updated')
+        super().Destroy()
+
     def DataUpdated(self):
         updated_ax = []
         for ax in self.figure.get_axes():
             autorelim = False
             updated = False
             for l in ax.lines:
                 if not hasattr(l, 'trace_signal'):
```

### Comparing `bsmplot-0.1.4/bsmplot/bsm/mat.py` & `bsmplot-0.1.5/bsmplot/bsm/mat.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,49 +1,64 @@
 import os
 import sys
 import traceback
 import wx
 import wx.py.dispatcher as dp
 from scipy import io
+import numpy as np
+import h5py
 from bsmutility.pymgr_helpers import Gcm
 from bsmutility.fileviewbase import TreeCtrlNoTimeStamp, ListCtrlBase, PanelNotebookBase, FileViewBase
 
 def process_record(d):
+    if hasattr(d, 'keys'):
+        keys = [k for k in d.keys() if not k.startswith('__')]
+        data = {}
+        for k in keys:
+            data[k] = process_record(d[k])
+        return data
+
     if d.dtype.names is None:
         if len(d) == 1 and d.dtype.name == 'object':
             return process_record(d[0])
         if hasattr(d, 'shape'):
             if len(d.shape) <= 1 or sorted(d.shape)[-2] == 1:
-                d = d.flatten()
+                d = np.array(d).flatten()
         return d
     data = {}
     for name in d.dtype.names:
         data[name] = process_record(d[name])
     return data
 
 def load_mat(filename):
     data = {'info': {}, 'data': {}}
     try:
-        raw = io.loadmat(filename)
+        try:
+            raw = io.loadmat(filename)
+        except:
+            raw = h5py.File(filename,'r')
+
         data['info']['version'] = raw.get('__version__', '')
         data['info']['header'] = raw.get('__header__', '')
         data['info']['globals'] = raw.get('__globals__', '')
 
-        # data
-        keys = [k for k in raw if not k.startswith('__')]
-        for k in keys:
-            data['data'][k] = process_record(raw[k])
+        data['data'] = process_record(raw)
     except:
         traceback.print_exc(file=sys.stdout)
 
     return data
 
 
 class MatTree(TreeCtrlNoTimeStamp):
-    pass
+
+    def GetItemDataFromPath(self, path):
+        d = super().GetItemDataFromPath(path)
+        if not self._is_folder(d):
+            d = np.array(d)
+        return d
 
 
 class InfoListCtrl(ListCtrlBase):
 
     def BuildColumns(self):
         super().BuildColumns()
         start = self.data_start_column
```

### Comparing `bsmplot-0.1.4/bsmplot/bsm/parsetab.py` & `bsmplot-0.1.5/bsmplot/bsm/parsetab.py`

 * *Files identical despite different names*

### Comparing `bsmplot-0.1.4/bsmplot/bsm/shell.py` & `bsmplot-0.1.5/bsmplot/bsm/shell.py`

 * *Files identical despite different names*

### Comparing `bsmplot-0.1.4/bsmplot/bsm/ulog.py` & `bsmplot-0.1.5/bsmplot/bsm/ulog.py`

 * *Files identical despite different names*

### Comparing `bsmplot-0.1.4/bsmplot/bsm/utility.py` & `bsmplot-0.1.5/bsmplot/bsm/utility.py`

 * *Files identical despite different names*

### Comparing `bsmplot-0.1.4/bsmplot/bsm/vcds.py` & `bsmplot-0.1.5/bsmplot/bsm/vcds.py`

 * *Files identical despite different names*

### Comparing `bsmplot-0.1.4/bsmplot/bsm/zmqs.py` & `bsmplot-0.1.5/bsmplot/bsm/zmqs.py`

 * *Files identical despite different names*

### Comparing `bsmplot-0.1.4/bsmplot/mainframe.py` & `bsmplot-0.1.5/bsmplot/mainframe.py`

 * *Files identical despite different names*

### Comparing `bsmplot-0.1.4/bsmplot/mainframexpm.py` & `bsmplot-0.1.5/bsmplot/mainframexpm.py`

 * *Files identical despite different names*

### Comparing `bsmplot-0.1.4/bsmplot/pvcd/lextab.py` & `bsmplot-0.1.5/bsmplot/pvcd/lextab.py`

 * *Files identical despite different names*

### Comparing `bsmplot-0.1.4/bsmplot/pvcd/parsetab.py` & `bsmplot-0.1.5/bsmplot/pvcd/parsetab.py`

 * *Files identical despite different names*

### Comparing `bsmplot-0.1.4/bsmplot/pvcd/pvcd.py` & `bsmplot-0.1.5/bsmplot/pvcd/pvcd.py`

 * *Files identical despite different names*

### Comparing `bsmplot-0.1.4/bsmplot/pvcd/pvcd2.py` & `bsmplot-0.1.5/bsmplot/pvcd/pvcd2.py`

 * *Files identical despite different names*

### Comparing `bsmplot-0.1.4/bsmplot.egg-info/PKG-INFO` & `bsmplot-0.1.5/bsmplot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bsmplot
-Version: 0.1.4
+Version: 0.1.5
 Summary: bsmplot is a tool to visualize time series
 Author-email: Tianzhu Qiao <tq@feiyilin.com>
 License: MIT License
         
         Copyright (c) 2024 Tianzhu Qiao
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -34,21 +34,22 @@
 Requires-Dist: matplotlib>=3.8.1
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: click>=8.1
 Requires-Dist: pandas
 Requires-Dist: pyulog
 Requires-Dist: pyvcd
-Requires-Dist: propgrid>=0.1.3
-Requires-Dist: mplpanel>=0.1.2
+Requires-Dist: propgrid>=0.1.4
+Requires-Dist: mplpanel>=0.1.3
 Requires-Dist: aui2>=0.1.4
 Requires-Dist: zmq
-Requires-Dist: bsmutility>=0.1.3
+Requires-Dist: bsmutility>=0.1.4
 Requires-Dist: ply
 Requires-Dist: charset_normalizer
+Requires-Dist: h5py
 
 # bsmplot
 **bsmplot** is a cross-platform tool to visualize time series based on [Matplotlib](https://matplotlib.org/) and [wxPython](https://wxpython.org/). Supported data source
 - VCD (value change dump)
 - PX4 [ulog](https://docs.px4.io/main/en/dev_log/ulog_file_format.html)
 - CSV
 - Matlab .mat
```

### Comparing `bsmplot-0.1.4/bsmplot.egg-info/SOURCES.txt` & `bsmplot-0.1.5/bsmplot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bsmplot-0.1.4/pyproject.toml` & `bsmplot-0.1.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 readme = "README.md"
 requires-python = ">=3.0"
 classifiers = [
     "Operating System :: OS Independent",
 ]
 dependencies = [
           'wxpython>=4.2.1', 'matplotlib>=3.8.1', 'numpy', 'scipy', 'click>=8.1', 'pandas',
-          'pyulog', 'pyvcd', 'propgrid>=0.1.3', 'mplpanel>=0.1.2', 'aui2>=0.1.4', 'zmq',
-          'bsmutility>=0.1.3','ply', 'charset_normalizer'
+          'pyulog', 'pyvcd', 'propgrid>=0.1.4', 'mplpanel>=0.1.3', 'aui2>=0.1.4', 'zmq',
+          'bsmutility>=0.1.4','ply', 'charset_normalizer', 'h5py'
       ]
 dynamic = ["version"]
 
 [tool.setuptools.dynamic]
 version = {attr = "bsmplot.__version__"}
 
 [project.urls]
```

