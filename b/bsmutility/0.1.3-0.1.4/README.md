# Comparing `tmp/bsmutility-0.1.3.tar.gz` & `tmp/bsmutility-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bsmutility-0.1.3.tar", last modified: Sun Mar 31 04:02:11 2024, max compression
+gzip compressed data, was "bsmutility-0.1.4.tar", last modified: Mon Jun  3 04:09:33 2024, max compression
```

## Comparing `bsmutility-0.1.3.tar` & `bsmutility-0.1.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 tianzhuqiao   (501) staff       (20)        0 2024-03-31 04:02:11.117545 bsmutility-0.1.3/
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)     1069 2024-02-11 23:35:49.000000 bsmutility-0.1.3/LICENSE
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)     1801 2024-03-31 04:02:11.116504 bsmutility-0.1.3/PKG-INFO
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)       12 2024-02-11 23:35:49.000000 bsmutility-0.1.3/README.md
-drwxr-xr-x   0 tianzhuqiao   (501) staff       (20)        0 2024-03-31 04:02:11.111878 bsmutility-0.1.3/bsmutility/
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)       33 2024-02-14 00:29:44.000000 bsmutility-0.1.3/bsmutility/__init__.py
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)     8808 2024-03-09 19:09:18.000000 bsmutility-0.1.3/bsmutility/autocomplete.py
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)      963 2024-02-14 04:41:45.000000 bsmutility-0.1.3/bsmutility/bsminterface.py
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)    22305 2024-02-11 23:35:49.000000 bsmutility-0.1.3/bsmutility/bsmxpm.py
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)     2572 2024-03-28 05:12:33.000000 bsmutility-0.1.3/bsmutility/configfile.py
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)    47673 2024-02-11 23:35:49.000000 bsmutility-0.1.3/bsmutility/debugger.py
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)     8543 2024-02-14 04:42:49.000000 bsmutility-0.1.3/bsmutility/debugtool.py
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)    11788 2024-02-11 23:35:49.000000 bsmutility-0.1.3/bsmutility/dirtreectrl.py
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)    42746 2024-02-24 04:10:08.000000 bsmutility-0.1.3/bsmutility/editor.py
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)    35414 2024-02-11 23:35:49.000000 bsmutility-0.1.3/bsmutility/editor_base.py
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)    61701 2024-03-29 04:29:17.000000 bsmutility-0.1.3/bsmutility/fileviewbase.py
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)    18717 2024-03-30 05:06:17.000000 bsmutility-0.1.3/bsmutility/frameplus.py
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)    36586 2024-02-14 04:29:28.000000 bsmutility-0.1.3/bsmutility/misctools.py
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)     3159 2024-02-11 23:35:49.000000 bsmutility-0.1.3/bsmutility/pymgr_helpers.py
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)     6010 2024-03-28 05:12:33.000000 bsmutility-0.1.3/bsmutility/quaternion.py
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)    35946 2024-03-09 19:09:18.000000 bsmutility-0.1.3/bsmutility/shell.py
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)     5225 2024-02-11 23:35:49.000000 bsmutility-0.1.3/bsmutility/shell_base.py
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)     9673 2024-03-29 00:56:14.000000 bsmutility-0.1.3/bsmutility/signalselsettingdlg.py
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)    10195 2024-03-24 05:40:57.000000 bsmutility-0.1.3/bsmutility/utility.py
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)      186 2024-03-30 05:19:10.000000 bsmutility-0.1.3/bsmutility/version.py
-drwxr-xr-x   0 tianzhuqiao   (501) staff       (20)        0 2024-03-31 04:02:11.115544 bsmutility-0.1.3/bsmutility.egg-info/
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)     1801 2024-03-31 04:02:11.000000 bsmutility-0.1.3/bsmutility.egg-info/PKG-INFO
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)      695 2024-03-31 04:02:11.000000 bsmutility-0.1.3/bsmutility.egg-info/SOURCES.txt
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)        1 2024-03-31 04:02:11.000000 bsmutility-0.1.3/bsmutility.egg-info/dependency_links.txt
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)       97 2024-03-31 04:02:11.000000 bsmutility-0.1.3/bsmutility.egg-info/requires.txt
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)       16 2024-03-31 04:02:11.000000 bsmutility-0.1.3/bsmutility.egg-info/top_level.txt
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)      772 2024-03-31 04:01:58.000000 bsmutility-0.1.3/pyproject.toml
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)       38 2024-03-31 04:02:11.117855 bsmutility-0.1.3/setup.cfg
+drwxr-xr-x   0 tianzhuqiao   (501) staff       (20)        0 2024-06-03 04:09:33.415730 bsmutility-0.1.4/
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     1069 2024-02-11 23:35:49.000000 bsmutility-0.1.4/LICENSE
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     1801 2024-06-03 04:09:33.415027 bsmutility-0.1.4/PKG-INFO
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)       12 2024-02-11 23:35:49.000000 bsmutility-0.1.4/README.md
+drwxr-xr-x   0 tianzhuqiao   (501) staff       (20)        0 2024-06-03 04:09:33.408096 bsmutility-0.1.4/bsmutility/
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)       33 2024-02-14 00:29:44.000000 bsmutility-0.1.4/bsmutility/__init__.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     8808 2024-03-09 19:09:18.000000 bsmutility-0.1.4/bsmutility/autocomplete.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)      963 2024-02-14 04:41:45.000000 bsmutility-0.1.4/bsmutility/bsminterface.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)    22305 2024-02-11 23:35:49.000000 bsmutility-0.1.4/bsmutility/bsmxpm.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     2572 2024-05-11 05:15:43.000000 bsmutility-0.1.4/bsmutility/configfile.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)    47673 2024-02-11 23:35:49.000000 bsmutility-0.1.4/bsmutility/debugger.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     8543 2024-02-14 04:42:49.000000 bsmutility-0.1.4/bsmutility/debugtool.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)    11788 2024-02-11 23:35:49.000000 bsmutility-0.1.4/bsmutility/dirtreectrl.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)    42746 2024-02-24 04:10:08.000000 bsmutility-0.1.4/bsmutility/editor.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)    35414 2024-02-11 23:35:49.000000 bsmutility-0.1.4/bsmutility/editor_base.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)    63511 2024-05-11 05:15:46.000000 bsmutility-0.1.4/bsmutility/fileviewbase.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)    18717 2024-03-30 05:06:17.000000 bsmutility-0.1.4/bsmutility/frameplus.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)    36586 2024-02-14 04:29:28.000000 bsmutility-0.1.4/bsmutility/misctools.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     3159 2024-02-11 23:35:49.000000 bsmutility-0.1.4/bsmutility/pymgr_helpers.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     6010 2024-03-28 05:12:33.000000 bsmutility-0.1.4/bsmutility/quaternion.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)    35946 2024-03-09 19:09:18.000000 bsmutility-0.1.4/bsmutility/shell.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     5225 2024-02-11 23:35:49.000000 bsmutility-0.1.4/bsmutility/shell_base.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)    15625 2024-05-11 05:15:46.000000 bsmutility-0.1.4/bsmutility/signalselsettingdlg.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)    10195 2024-03-24 05:40:57.000000 bsmutility-0.1.4/bsmutility/utility.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)      186 2024-06-03 04:08:27.000000 bsmutility-0.1.4/bsmutility/version.py
+drwxr-xr-x   0 tianzhuqiao   (501) staff       (20)        0 2024-06-03 04:09:33.414159 bsmutility-0.1.4/bsmutility.egg-info/
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     1801 2024-06-03 04:09:33.000000 bsmutility-0.1.4/bsmutility.egg-info/PKG-INFO
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)      695 2024-06-03 04:09:33.000000 bsmutility-0.1.4/bsmutility.egg-info/SOURCES.txt
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)        1 2024-06-03 04:09:33.000000 bsmutility-0.1.4/bsmutility.egg-info/dependency_links.txt
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)       97 2024-06-03 04:09:33.000000 bsmutility-0.1.4/bsmutility.egg-info/requires.txt
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)       16 2024-06-03 04:09:33.000000 bsmutility-0.1.4/bsmutility.egg-info/top_level.txt
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)      772 2024-03-31 04:01:58.000000 bsmutility-0.1.4/pyproject.toml
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)       38 2024-06-03 04:09:33.415877 bsmutility-0.1.4/setup.cfg
```

### Comparing `bsmutility-0.1.3/LICENSE` & `bsmutility-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bsmutility-0.1.3/PKG-INFO` & `bsmutility-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bsmutility
-Version: 0.1.3
+Version: 0.1.4
 Summary: Some helper class
 Author-email: Tianzhu Qiao <tq@feiyilin.com>
 License: MIT License
         
         Copyright (c) 2024 Tianzhu Qiao
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `bsmutility-0.1.3/bsmutility/autocomplete.py` & `bsmutility-0.1.4/bsmutility/autocomplete.py`

 * *Files identical despite different names*

### Comparing `bsmutility-0.1.3/bsmutility/bsminterface.py` & `bsmutility-0.1.4/bsmutility/bsminterface.py`

 * *Files identical despite different names*

### Comparing `bsmutility-0.1.3/bsmutility/bsmxpm.py` & `bsmutility-0.1.4/bsmutility/bsmxpm.py`

 * *Files identical despite different names*

### Comparing `bsmutility-0.1.3/bsmutility/configfile.py` & `bsmutility-0.1.4/bsmutility/configfile.py`

 * *Files identical despite different names*

### Comparing `bsmutility-0.1.3/bsmutility/debugger.py` & `bsmutility-0.1.4/bsmutility/debugger.py`

 * *Files identical despite different names*

### Comparing `bsmutility-0.1.3/bsmutility/debugtool.py` & `bsmutility-0.1.4/bsmutility/debugtool.py`

 * *Files identical despite different names*

### Comparing `bsmutility-0.1.3/bsmutility/dirtreectrl.py` & `bsmutility-0.1.4/bsmutility/dirtreectrl.py`

 * *Files identical despite different names*

### Comparing `bsmutility-0.1.3/bsmutility/editor.py` & `bsmutility-0.1.4/bsmutility/editor.py`

 * *Files identical despite different names*

### Comparing `bsmutility-0.1.3/bsmutility/editor_base.py` & `bsmutility-0.1.4/bsmutility/editor_base.py`

 * *Files identical despite different names*

### Comparing `bsmutility-0.1.3/bsmutility/fileviewbase.py` & `bsmutility-0.1.4/bsmutility/fileviewbase.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,67 +7,85 @@
 import wx.py.dispatcher as dp
 from wx.lib.mixins.listctrl import ListCtrlAutoWidthMixin
 import numpy as np
 import pandas as pd
 from pandas.api.types import is_numeric_dtype
 import matplotlib.pyplot as plt
 import aui2 as aui
-from propgrid import PropText, PropSeparator, PropCheckBox
+from propgrid import PropText, PropCheckBox
 from .bsmxpm import open_svg, refresh_svg, more_svg
 from .utility import FastLoadTreeCtrl, _dict, send_data_to_shell, get_variable_name
 from .utility import svg_to_bitmap, build_tree, flatten_tree
 from .utility import get_file_finder_name, show_file_in_finder, \
                      get_tree_item_path, get_tree_item_name
 from .autocomplete import AutocompleteTextCtrl
 from .bsminterface import Interface
-from .signalselsettingdlg import SignalSelSettingDlg, PropSettingDlg, ConvertSettingDlg
+from .signalselsettingdlg import SignalSelSettingDlg, ConvertManagingDlg
 from .quaternion import Quaternion
 from .configfile import ConfigFile
 
 class FindListCtrl(wx.ListCtrl):
     ID_FIND_REPLACE = wx.NewIdRef()
     ID_FIND_NEXT = wx.NewIdRef()
     ID_FIND_PREV = wx.NewIdRef()
     ID_COPY_NO_INDEX = wx.NewIdRef()
+    ID_COPY_SEL_COLS = wx.NewIdRef()
     def __init__(self, *args, **kwargs):
         wx.ListCtrl.__init__(self, *args, **kwargs)
         self.SetupFind()
 
         self.index_column = 0
         self.Bind(wx.EVT_LIST_ITEM_RIGHT_CLICK, self.OnRightClick)
         self.Bind(wx.EVT_TOOL, self.OnBtnCopy, id=wx.ID_COPY)
         self.Bind(wx.EVT_TOOL, self.OnBtnCopy, id=self.ID_COPY_NO_INDEX)
+        self.Bind(wx.EVT_TOOL, self.OnBtnCopy, id=self.ID_COPY_SEL_COLS)
 
         accel = [
             (wx.ACCEL_CTRL, ord('F'), self.ID_FIND_REPLACE),
             (wx.ACCEL_SHIFT, wx.WXK_F3, self.ID_FIND_PREV),
             (wx.ACCEL_CTRL, ord('H'), self.ID_FIND_REPLACE),
             (wx.ACCEL_RAW_CTRL, ord('H'), self.ID_FIND_REPLACE),
             (wx.ACCEL_CTRL, ord('C'), wx.ID_COPY),
             (wx.ACCEL_CTRL | wx.ACCEL_SHIFT, ord('C'), self.ID_COPY_NO_INDEX),
         ]
         self.accel = wx.AcceleratorTable(accel)
         self.SetAcceleratorTable(self.accel)
 
+        self._copy_columns = None
+
     def OnRightClick(self, event):
 
         if self.GetSelectedItemCount() <= 0:
             return
 
         menu = wx.Menu()
         menu.Append(wx.ID_COPY, "&Copy \tCtrl+C")
         if 0 <= self.index_column < self.GetColumnCount():
             menu.Append(self.ID_COPY_NO_INDEX, "C&opy without index \tCtrl+Shift+C")
+        if self.GetColumnCount() > 1:
+            menu.Append(self.ID_COPY_SEL_COLS, "Copy &selected columns")
+
         self.PopupMenu(menu)
 
     def OnBtnCopy(self, event):
         cmd = event.GetId()
         columns = list(range(self.GetColumnCount()))
         if cmd == self.ID_COPY_NO_INDEX:
             columns.remove(self.index_column)
+        elif cmd == self.ID_COPY_SEL_COLS:
+            lst = [self.GetColumn(c).GetText() for c in range(self.GetColumnCount())]
+            dlg = wx.MultiChoiceDialog(self, "Select column(s):","Copy ...", lst)
+            if self._copy_columns is None:
+                # default all columns
+                self._copy_columns = range(len(lst))
+            dlg.SetSelections(self._copy_columns)
+            if dlg.ShowModal() == wx.ID_OK:
+                columns = dlg.GetSelections()
+                self._copy_columns = columns
+
         if wx.TheClipboard.Open():
             item = self.GetFirstSelected()
             text = []
             while item != -1:
                 tmp = []
                 for c in columns:
                     tmp.append(self.GetItemText(item, c))
@@ -300,14 +318,16 @@
 
     ID_EXPORT = wx.NewIdRef()
     ID_PLOT = wx.NewIdRef()
     ID_CONVERT = wx.NewIdRef()
     ID_CONVERT_CUSTOM = wx.NewIdRef()
     ID_CONVERT_MANAGE = wx.NewIdRef()
     ID_DELETE = wx.NewIdRef()
+    ID_COPY_PATH = wx.NewIdRef()
+    ID_COPY_NAME = wx.NewIdRef()
     IDS_CONVERT = {}
 
     def __init__(self, parent, style=wx.TR_DEFAULT_STYLE):
         style = style | wx.TR_HAS_VARIABLE_ROW_HEIGHT | wx.TR_HIDE_ROOT |\
                 wx.TR_MULTIPLE | wx.TR_LINES_AT_ROOT
         super().__init__(parent, self.get_children, style=style)
 
@@ -325,19 +345,27 @@
                                     'outputs': '#_deg',
                                     'equation': 'np.rad2deg(#1)',
                                     'force_select_signal': False},
                                 {'label': 'Degree to radian',
                                     'inputs': ['#1'],
                                     'outputs': '#_rad',
                                     'equation': 'np.deg2rad(#1)',
-                                    'force_select_signal': False}]
+                                    'force_select_signal': False},
+                                {'label': 'Moving average',
+                                    'inputs': ['#1'],
+                                    'args': [['Window size', '$w', 30]],
+                                    'outputs': '#_avg',
+                                    'equation': 'np.convolve(#1, np.ones($w), "same")/$w',
+                                    'force_select_signal': True}
+                                ]
         self.customized_convert = []
         self._converted_item = {}
         self._convert_labels = {'label': 'Label',
                                 'inputs': 'Input(s), separated by ","',
+                                'args': 'Argument(s)',
                                 'equation': 'Equation',
                                 'outputs': 'Output(s), separated by ","',
                                 'force_select_signal': 'Always show the signal selecting dialog'}
         self.config_file = None
         self.filename = None
 
         self.graph_drop = False
@@ -403,14 +431,23 @@
                     if self.config_file:
                         self.config_file.SetConfig('conversion',
                                                    converted_item=self._converted_item)
 
                 self.RefreshChildren(parent)
         elif cmd == self.ID_PLOT:
             self.PlotItem(item)
+        elif cmd in [self.ID_COPY_NAME, self.ID_COPY_PATH]:
+            if wx.TheClipboard.Open():
+                if cmd == self.ID_COPY_NAME:
+                    p = self.GetItemText(item)
+                else:
+                    p = self.GetItemName(item)
+                wx.TheClipboard.SetData(wx.TextDataObject(p))
+                wx.TheClipboard.Close()
+
         elif cmd == self.ID_CONVERT:
             self.ConvertItems(item, self.GetSelections())
         elif cmd == self.ID_CONVERT_CUSTOM:
             self.AddCustomizedConvert()
         elif cmd == self.ID_CONVERT_MANAGE:
             self.ManageCustomizedConvert()
         elif cmd in self.IDS_CONVERT.values():
@@ -481,14 +518,17 @@
         menu = wx.Menu()
         menu.Append(self.ID_EXPORT, "Export to shell")
         menu.AppendSeparator()
         menu.Append(self.ID_PLOT, "Plot")
         menu.AppendSeparator()
         menu.Append(self.ID_DELETE, "Delete")
         menu.AppendSeparator()
+        menu.Append(self.ID_COPY_NAME, "Copy name")
+        menu.Append(self.ID_COPY_PATH, "Copy path")
+        menu.AppendSeparator()
         menu.Append(self.ID_CONVERT, "Convert to ...")
         for c in self.common_convert:
             if c['label'] not in self.IDS_CONVERT:
                 self.IDS_CONVERT[c['label']] = wx.NewIdRef()
             menu.Append(self.IDS_CONVERT[c['label']], c['label'])
 
         menu_customize = wx.Menu()
@@ -525,14 +565,15 @@
 
     def ConvertItems(self, item, items, equation=None, config=None,
                      force_select_signal=False, **kwargs):
         settings = kwargs
         settings['equation'] = equation
         outputs = kwargs.get('outputs', '~#')
         inputs = kwargs.get('inputs', None)
+        args = kwargs.get('args', None)
         N_IN = len(inputs) if inputs is not None else len(items)
         if inputs is None:
             inputs = [f'#{i+1}' for i in range(N_IN)]
         for i in range(min(N_IN, len(items))):
             if items[i] is not None:
                 settings[f'{inputs[i]}'] = self.GetItemName(items[i])
 
@@ -550,24 +591,30 @@
                 start = self.GetItemName(parent)
             values = {f'{inputs[i]}': settings.get(f'{inputs[i]}', '') for i in range(N_IN)}
             values['equation'] = equation
             values['outputs'] = outputs
             additional = self.GetConvertItemProp(item, inputs, outputs.split(','))
             df_in, settings = self.SelectSignal(items=inputs,
                                             values=values,
+                                            args=args,
                                             config=config,
                                             additional=additional,
                                             start=start)
             if settings is None or df_in is None:
                 return None, settings
             settings['inputs'] = inputs
             equation = settings.get('equation', None)
             outputs = settings.get('outputs', outputs)
         if not equation:
             return None, settings
+
+        if outputs:
+            for i in settings['inputs']:
+                outputs = outputs.replace(i, get_tree_item_path(settings[i])[-1])
+
         if item is not None:
             text = self.GetItemText(item)
             outputs = outputs or f'~{text}'
             outputs = outputs.replace('#', text)
 
         d = self.doConvertFromSetting(settings)
 
@@ -616,50 +663,56 @@
             d = d[idx[1]]
         self.SetData(p, d)
         self._converted_item[p] = [idx, settings]
         return True
 
     def doConvertFromSetting(self, settings):
         inputs = settings.get('inputs', ['x'])
+        args = settings.get('args', None)
         equation = settings.get('equation', None)
         if inputs is None or equation is None:
             return None
         N_IN = len(inputs)
         paths = []
         for i in range(N_IN):
             signal = settings.get(inputs[i], None)
             if N_IN == 1 and not signal:
                 signal = settings.get('#', None)
             if signal is None:
                 return None
             paths.append(get_tree_item_path(f'{signal}'))
             # replace input name (e.g., #w) with input index (e.g., #1)
             equation = equation.replace(f'#{inputs[i].lstrip("#")}', f'#{i+1}')
-        return self.doConvert(paths, equation)
+        return self.doConvert(paths, args, equation)
 
-    def doConvert(self, paths, equation):
+    def doConvert(self, paths, args, equation):
         # calculate equation(paths)
         # paths are path of input items
         # and equation may look like foo(#1, #2, #3, ...), e.g., where #1 will
         # be replaced with data from paths[0], etc.
-
         data = []
         for path in paths:
             d = self.GetItemDataFromPath(path)
             if d is None:
                 print(f'Invalid inputs {get_tree_item_name(path)}')
                 return None
             data.append(d)
 
         for i in range(len(paths)):
             equation = equation.replace(f'#{i+1}', f'data[{i}]')
 
         # or '#' for first input
         equation = equation.replace('#', 'data[0]')
 
+        # arguments
+        if args is None:
+            args = []
+        for _, arg, value in args:
+            equation = equation.replace(arg, str(value))
+
         try:
             # get the locals from shell, to reuse the functions/modules
             resp = dp.send('shell.get_locals')
             if resp:
                 local = resp[0][1]
                 local.update(locals())
             else:
@@ -667,55 +720,42 @@
             d = eval(equation, globals(), local)
             return d
         except:
             traceback.print_exc(file=sys.stdout)
 
         return None
 
-    def GetCustomizedConvertProp(self):
+    def CreateEmptyConvert(self):
         # the configuration props used to convert an item
         label = 'my conversion'
         labels = [c['label'] for c in self.common_convert + self.GetCustomizedConvert()]
         i = 1
         while f'{label} {i}' in labels:
             i += 1
         label = f'{label} {i}'
-        in_size =  max(1, len(self.GetSelections()))
-        inputs = ', '.join([f'#{i+1}' for i in range(in_size)])
-        props = [PropText().Name('label').Value(label),
-                 PropText().Name('inputs').Value(inputs),
-                 PropText().Name('equation').Value('#1'),
-                 PropCheckBox().Name('force_select_signal').Value(in_size>1),
-                 PropText().Name('outputs').Value('~#')]
-        for p in props:
-            name = p.GetName()
-            label = self._convert_labels.get(name, name.capitalize())
-            p.Label(label)
-        return props
+        setting = {'label': label, 'equation': '#1', 'inputs': ['#1'], 'outputs': '~#1',
+                   'args':[], 'force_select_signal': False}
+        return setting
 
     def AddCustomizedConvert(self):
         settings = None
-        # settings is none, get it from user
-        props = self.GetCustomizedConvertProp()
-        dlg = PropSettingDlg(self, props=props, config='')
-        dlg.propgrid.GetArtProvider().SetTitleWidth(200)
+        convert = self.CreateEmptyConvert()
+        dlg = ConvertManagingDlg(self, [convert], labels=self._convert_labels, size=(800, 600))
         if dlg.ShowModal() == wx.ID_OK:
             settings = dlg.GetSettings()
-            settings['inputs'] = [x.strip() for x in settings.get('inputs', '#1').split(',')]
+            settings = settings[0]
             self.customized_convert.append(settings)
             self.SetConfig(convert=self.customized_convert)
         return settings
 
     def ManageCustomizedConvert(self):
         converts = self.GetCustomizedConvert()
-        dlg = ConvertSettingDlg(self, converts, labels=self._convert_labels)
+        dlg = ConvertManagingDlg(self, converts, labels=self._convert_labels, size=(800, 600))
         if dlg.ShowModal() == wx.ID_OK:
             settings = dlg.GetSettings()
-            for s in settings:
-                s['inputs'] = [x.strip() for x in s.get('inputs', '#1').split(',')]
             self.customized_convert = settings
             self.SetConfig(convert=self.customized_convert)
 
     def GetCustomizedConvert(self):
         self.customized_convert = self.LoadConfig(key='convert') or []
         return self.customized_convert
 
@@ -781,14 +821,16 @@
             ax.grid(True)
             xlabel = self.GetPlotXLabel()
             if xlabel:
                 ax.set_xlabel(xlabel)
             if step:
                 # hide the y-axis tick label
                 ax.get_yaxis().set_ticklabels([])
+        # notify the graph to update (e.g., timeline)
+        dp.send('graph.axes_updated', figure=fig, axes=[ax])
         return line[0]
 
     def GetItemPath(self, item):
         path = []
         while item.IsOk() and item != self.GetRootItem():
             path.insert(0, self.GetItemText(item))
             item = self.GetItemParent(item)
@@ -976,29 +1018,29 @@
                     item = child
                     break
                 child, cookie = self.GetNextChild(item, cookie)
             else:
                 return None
         return item
 
-    def SelectSignal(self, items, values, config, additional=None, start=''):
+    def SelectSignal(self, items, values, args, config, additional=None, start=''):
         data = self.data
         if start:
             data = self.GetData(start)
         # remove the "start" from values
         if start:
             for k, v in values.items():
                 if not v or not v.startswith(start):
                     continue
                 # remove '{start}.'
                 values[k] = v[len(start):].lstrip('.')
 
         dlg = SignalSelSettingDlg(self.GetTopLevelParent(), data=data,
-                                  items=items, values=values, config=config,
-                                  additional=additional)
+                                  items=items, values=values, args=args,
+                                  config=config, additional=additional)
         if dlg.ShowModal() == wx.ID_OK:
             settings = dlg.GetSettings()
             df = pd.DataFrame()
             for item in items:
                 signal = settings.get(item, '')
                 if not signal:
                     print(f'Input "{item}" is missing!')
@@ -1014,14 +1056,19 @@
                     return None, settings
                 if hasattr(d, 'shape') and len(d.shape) > 1:
                     print(f'Input "{item}({signal})" is not 1-d!')
                     return None, settings
                 df[item] = d
                 # the full path with "start"
                 settings[item] = signal
+            # args
+            if args is not None:
+                for i in range(len(args)):
+                    args[i][2] = settings.get(args[i][1], args[i][2])
+                settings['args'] = args
             return df, settings
         return None, None
 
 
 class TreeCtrlWithTimeStamp(TreeCtrlBase):
     # the leaf node is a DataFrame
 
@@ -1195,20 +1242,18 @@
         props = super().GetConvertItemProp(item, inputs, outputs)
         if len(outputs) == 1:
             # for single output
             xaxis_label = self._convert_labels.get(self.XAXIS, 'Set as x-axis')
             props.append(PropCheckBox().Label(xaxis_label).Name(self.XAXIS).Value(False))
         return props
 
-    def GetCustomizedConvertProp(self):
-        # the configuration props used to convert an item
-        props = super().GetCustomizedConvertProp()
-        xaxis_label = self._convert_labels.get(self.XAXIS, 'Set as x-axis')
-        props.append(PropCheckBox().Label(xaxis_label).Name(self.XAXIS).Value(False))
-        return props
+    def CreateEmptyConvert(self):
+        convert = super().CreateEmptyConvert()
+        convert[self.XAXIS] = False
+        return convert
 
     def ConvertItems(self, item, items, equation=None, config=None,
                      force_select_signal=False, **kwargs):
         new_item, settings = super().ConvertItems(item, items, equation, config,
                                                   force_select_signal, **kwargs)
         if new_item and len(new_item) == 1 and new_item[0].IsOk():
             if settings is not None and settings.get(self.XAXIS, False):
@@ -1275,29 +1320,31 @@
     def GetItemExportData(self, item):
         y = self.GetItemData(item)
         path = self.GetItemPath(item)
         name = self.GetItemText(item)
         data = [[name, y]]
         selections = self.GetSelections()
         for sel in selections:
-            if self.ItemHasChildren(sel) and sel != item:
+            if self.ItemHasChildren(sel) or sel == item:
                 continue
             y = self.GetItemData(sel)
             name = self.GetItemText(sel)
             data.append([name, y])
         data_size = [len(d[1]) for d in data]
         data_1d = [len(d[1].shape) <= 1 or sorted(d[1].shape)[-2] == 1  for d in data]
         if all(data_1d) and all(d == data_size[0] for d in data_size):
             # if all data has same size, convert it to DataFrame
             df = pd.DataFrame()
             for name, val in data:
                 if isinstance(val, np.ndarray):
                     val = val.flatten()
                 df[name] = val
             data = df
+        elif len(data) == 1:
+            data = data[0][1]
 
         if len(selections) <= 1:
             output_name = get_variable_name(path)
         else:
             output_name = "_data"
         return output_name, data
```

### Comparing `bsmutility-0.1.3/bsmutility/frameplus.py` & `bsmutility-0.1.4/bsmutility/frameplus.py`

 * *Files identical despite different names*

### Comparing `bsmutility-0.1.3/bsmutility/misctools.py` & `bsmutility-0.1.4/bsmutility/misctools.py`

 * *Files identical despite different names*

### Comparing `bsmutility-0.1.3/bsmutility/pymgr_helpers.py` & `bsmutility-0.1.4/bsmutility/pymgr_helpers.py`

 * *Files identical despite different names*

### Comparing `bsmutility-0.1.3/bsmutility/quaternion.py` & `bsmutility-0.1.4/bsmutility/quaternion.py`

 * *Files identical despite different names*

### Comparing `bsmutility-0.1.3/bsmutility/shell.py` & `bsmutility-0.1.4/bsmutility/shell.py`

 * *Files identical despite different names*

### Comparing `bsmutility-0.1.3/bsmutility/shell_base.py` & `bsmutility-0.1.4/bsmutility/shell_base.py`

 * *Files identical despite different names*

### Comparing `bsmutility-0.1.3/bsmutility/signalselsettingdlg.py` & `bsmutility-0.1.4/bsmutility/signalselsettingdlg.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import wx
 import wx.py.dispatcher as dp
 import propgrid
 from propgrid import PropControl, PropGrid, TextValidator, PropCheckBox, \
-                     PropText
+                     PropText, PropSeparator
 from .autocomplete import AutocompleteTextCtrl
 from .utility import get_tree_item_path
 
 class PropAutoCompleteEditBox(PropControl):
     def __init__(self, completer, *args, **kwargs):
         super().__init__(self, *args, **kwargs)
         self.completer = completer
@@ -51,14 +51,15 @@
     def __init__(self, parent, config=None, title='Settings ...',
                  size=wx.DefaultSize, pos=wx.DefaultPosition,
                  style=wx.DEFAULT_DIALOG_STYLE|wx.RESIZE_BORDER):
         wx.Dialog.__init__(self)
         self.SetExtraStyle(wx.DIALOG_EX_CONTEXTHELP)
         self.Create(parent, title=title, pos=pos, size=size, style=style)
 
+        self.SetEscapeId(wx.ID_CANCEL)
         self.config = config
         if self.config and '.' in self.config:
             self.config = self.config.split('.')
         assert not self.config or len(self.config) == 2
 
         self.propgrid = PropGrid(self)
         g = self.propgrid
@@ -67,40 +68,44 @@
         g.SetFocus()
 
         sizer = wx.BoxSizer(wx.VERTICAL)
 
         sizer.Add(g, 1, wx.EXPAND|wx.ALL, 1)
 
         # ok/cancel button
-        btnsizer = wx.StdDialogButtonSizer()
+        btnsizer = wx.BoxSizer(wx.HORIZONTAL)
         btnsizer.AddStretchSpacer(1)
-
-        btn = wx.Button(self, wx.ID_OK)
-        btn.SetDefault()
-        btnsizer.AddButton(btn)
-
-        btn = wx.Button(self, wx.ID_CANCEL)
-        btnsizer.AddButton(btn)
-        btnsizer.Realize()
-
+        for btn in self.CreateButtons():
+            btnsizer.Add(btn, 0, wx.ALL, 5)
         sizer.Add(btnsizer, 0, wx.ALL|wx.EXPAND, 15)
 
         self.SetSizer(sizer)
 
         self.Bind(wx.EVT_CONTEXT_MENU, self.OnContextMenu)
         self.Bind(propgrid.EVT_PROP_KEYDOWN, self.OnPropKeyDown)
+        g.Bind(propgrid.EVT_PROP_RIGHT_CLICK, self.OnRightClick)
+
+    def CreateButtons(self):
+        btn_ok = wx.Button(self, wx.ID_OK)
+        btn_ok.SetDefault()
+        btn_cancel = wx.Button(self, wx.ID_CANCEL)
+        return [btn_ok, btn_cancel]
 
     def OnPropKeyDown(self, event):
         data = event.GetData()
         keycode = data.get('keycode', '')
-        if keycode in [wx.WXK_UP, wx.WXK_DOWN] and not wx.GetKeyState(wx.WXK_COMMAND):
-            # only allow up/down
+        if keycode in [wx.WXK_UP, wx.WXK_DOWN, wx.WXK_SPACE, wx.WXK_ESCAPE, wx.WXK_TAB] and \
+           not wx.GetKeyState(wx.WXK_COMMAND):
+            # only allow up/down/space/escape
             return
         event.Veto()
 
+    def OnRightClick(self, event):
+        pass
+
     def OnContextMenu(self, event):
         # it is necessary, otherwise when right click on the dialog, the context
         # menu of the MatplotPanel will show; it may be due to some 'bug' in
         # CaptureMouse/ReleaseMouse (canvas is a panel that capture mouse)
         # and we also need to release the mouse before show the MatplotPanel
         # context menu (wchich will eventually show this dialog)
         pass
@@ -133,15 +138,15 @@
                     settings[name] = bool(settings[name])
 
         self.SetConfig(settings)
         return settings
 
 
 class SignalSelSettingDlg(SettingDlgBase):
-    def __init__(self, parent, data=None, items=None, values=None,
+    def __init__(self, parent, data=None, items=None, values=None, args=None,
                  config=None, additional=None, title='Settings ...',
                  size=wx.DefaultSize, pos=wx.DefaultPosition,
                  style=wx.DEFAULT_DIALOG_STYLE|wx.RESIZE_BORDER):
         SettingDlgBase.__init__(self, parent, config, title, size, pos, style)
 
         self.data = data
         self.items = items or []
@@ -149,15 +154,20 @@
         g = self.propgrid
         cfg = self.LoadConfig() or {}
         if values:
             cfg.update(values)
         for item in items:
             g.Insert(PropAutoCompleteEditBox(self.completer).Label(f'Input ({item})')
                      .Name(item).Value(cfg.get(item, '')))
-        for p in additional:
+        if args is not None:
+            for name, signal, default in args:
+                g.Insert(PropText().Label(f'{name.capitalize()}({signal})')
+                     .Name(signal).Value(default))
+
+        for p in self.additional:
             value = cfg.get(p.GetName(), None)
             if value is not None:
                 p.Value(value)
             g.Insert(p)
 
     def completer(self, query):
         path = get_tree_item_path(query)
@@ -178,90 +188,236 @@
         cfg = self.LoadConfig() or {}
         for p in props:
             value = cfg.get(p.GetName(), None)
             if value is not None:
                 p.Value(value)
             g.Insert(p)
 
-class ConvertSettingDlg(SettingDlgBase):
+class ConvertManagingDlg(SettingDlgBase):
     ID_DELETE = wx.NewIdRef()
+    ID_ADD_ARGUMENT = wx.NewIdRef()
 
     def __init__(self, parent, converts, labels=None, title='Settings ...',
                  size=wx.DefaultSize, pos=wx.DefaultPosition,
                  style=wx.DEFAULT_DIALOG_STYLE|wx.RESIZE_BORDER):
         SettingDlgBase.__init__(self, parent, None, title, size, pos, style)
 
+        self.labels = labels or {}
         g = self.propgrid
         g.Draggable(True)
-        if labels is None:
-            labels = {}
         for c in converts:
-            indent = 0
-            for k, v in c.items():
-                if isinstance(v, (tuple, list)):
-                    v = ','.join(v)
-                label = labels.get(k, k)
-                label = label.replace('_', ' ').capitalize()
-                if isinstance(v, bool):
-                    g.Insert(PropCheckBox().Label(label).Name(k).Value(v).Indent(indent)
-                             .Draggable(indent==0))
-                else:
-                    g.Insert(PropText().Label(label).Name(k).Value(v).Indent(indent)
-                             .Draggable(indent==0))
-                indent = 1
+            self.add_convert(c)
+
+        # expand the 1st convert
+        if g.GetCount() > 0:
+            g.Get(0).Expand(True)
 
-        g.Bind(propgrid.EVT_PROP_RIGHT_CLICK, self.OnRightClick)
         self.Bind(propgrid.EVT_PROP_DROP, self.OnDrop)
         self.Bind(propgrid.EVT_PROP_BEGIN_DRAG, self.OnDrag)
+        self.Bind(wx.EVT_BUTTON, self.OnAddArgument, id=self.ID_ADD_ARGUMENT)
+        self.Bind(wx.EVT_UPDATE_UI, self.OnUpdateCmdUI)
+
+    def OnUpdateCmdUI(self, event):
+        eid = event.GetId()
+        if eid == self.ID_ADD_ARGUMENT:
+            event.Enable(self.propgrid.GetSelected() is not None)
+
+    def _T(self, name):
+        label = self.labels.get(name, name)
+        label = label.replace('_', ' ').capitalize()
+        return label
+
+    def add_argument(self, arg, index=-1, indent=1):
+
+        p = self.propgrid.Insert(PropText().Label(self._T('name'))
+                                           .Value(arg[0]).Indent(indent),
+                                           index=index)
+        if index != -1:
+            index += 1
+        self.propgrid.Insert(PropText().Label(self._T('argument'))
+                                       .Value(arg[1]).Indent(indent+1),
+                                        index=index)
+
+        if index != -1:
+            index += 1
+        if isinstance(arg[2], bool):
+            self.propgrid.Insert(PropCheckBox().Label(self._T('default'))
+                                               .Value(arg[2]).Indent(indent+1),
+                                               index=index)
+        else:
+            self.propgrid.Insert(PropText().Label(self._T('default'))
+                                           .Value(arg[2]).Indent(indent+1),
+                                           index=index)
+
+        self.propgrid.SetSelection(p)
+        self.propgrid.EnsureVisible(p)
+
+    def add_convert(self, setting):
+
+        label = setting['label']
+        inputs = setting['inputs']
+        args = setting.get('args', None) or []
+        equation = setting.get('equation', '#1')
+        outputs = setting.get('outputs', '~#')
+        g = self.propgrid
+
+        p = g.Insert(PropText().Name('label').Label(self._T('label'))
+                               .Value(label).Indent(0).Expand(False))
+        if inputs is None:
+            inputs = ["#1"]
+        g.Insert(PropText().Name('inputs').Label(self._T('inputs'))
+                           .Value(','.join(inputs)).Indent(1))
+
+        g.Insert(PropSeparator().Name('args').Label(self._T('args'))
+                                .Indent(1).Expand(False).Visible(len(args) > 0))
+        for arg in args:
+            self.add_argument(arg, indent=2)
+
+        g.Insert(PropText().Name('equation').Label(self._T('equation'))
+                           .Value(equation).Indent(1))
+        g.Insert(PropText().Name('outputs').Label(self._T('outputs'))
+                           .Value(outputs).Indent(1))
+        # other settings
+        for k, v in setting.items():
+            if k in ['label', 'inputs', 'args', 'equation', 'outputs']:
+                continue
+            label = self._T(k)
+            if isinstance(v, bool):
+                g.Insert(PropCheckBox().Label(label).Name(k).Value(v).Indent(1)
+                         .Draggable(False))
+            else:
+                g.Insert(PropText().Label(label).Name(k).Value(v).Indent(1)
+                         .Draggable(False))
+        return p
+
+
+    def get_next_index(self, prop):
+        idx = self.propgrid.Index(prop)
+        indent = self.propgrid.Get(idx).GetIndent()
+        idx += 1
+        while idx < self.propgrid.GetCount():
+            p = self.propgrid.Get(idx)
+            if p.GetIndent() == indent:
+                break
+            idx += 1
+        return idx
+
+    def GetCurrentConvert(self):
+        prop = self.propgrid.GetSelected()
+        # find the current convert
+        while prop and prop.GetIndent() != 0:
+            prop = prop.GetParent()
+
+        return prop
+
+    def GetCurrentArgs(self):
+        prop = self.GetCurrentConvert()
+        if prop is None:
+            return None
+        idx = self.propgrid.Index(prop)
+        # find the args in current convert
+        while prop:
+            prop = self.propgrid.Get(idx)
+            if prop.GetName() == 'args':
+                return prop
+            idx += 1
+        return None
+
+    def OnAddArgument(self, event):
+        # find the args in current convert
+        prop = self.GetCurrentArgs()
+        if prop is None:
+            return
+
+        # show the arguments section
+        prop.Visible(True).Expand(True).Show()
+        idx = self.get_next_index(prop)
+        self.add_argument(["", "", "0"], index=idx, indent=prop.GetIndent()+1)
+
+    def CreateButtons(self):
+        btns = [wx.Button(self, self.ID_ADD_ARGUMENT, label="Add argument")]
+        return btns + super().CreateButtons()
 
     def OnDrag(self, event):
         prop = event.GetProp()
         if prop.IsExpanded():
             # not allow to move if in expanded mode
             event.Veto()
 
     def OnDrop(self, event):
         prop = event.GetProp()
         if (prop is not None) and prop.GetIndent() != 0:
             event.Veto()
 
     def OnRightClick(self, event):
         prop = event.GetProp()
-        if prop.GetIndent() == 0:
+        if prop.GetIndent() in [0, 2]:
             menu = wx.Menu()
             menu.Append(self.ID_DELETE, 'Delete')
             cmd = self.GetPopupMenuSelectionFromUser(menu)
             if cmd == wx.ID_NONE:
                 return
             if cmd == self.ID_DELETE:
                 idx = self.propgrid.Index(prop)
                 # delete the group
                 self.propgrid.Delete(idx)
                 while idx < self.propgrid.GetCount():
                     p = self.propgrid.Get(idx)
-                    if p.GetIndent() == 0:
+                    if p.GetIndent() <= prop.GetIndent():
                         break
                     self.propgrid.Delete(idx)
-
-    def GetSettings(self):
-        settings = []
+            if prop.GetIndent() == 2:
+                p = self.GetCurrentArgs()
+                if p and not p.HasChildren():
+                    p.Visible(False)
+            self.propgrid.UpdateGrid()
+
+    def GetConvert(self, index = 0):
+        p = self.propgrid.Get(index)
+        if p.GetIndent() != 0:
+            return None
         convert = {}
-        for i in range(self.propgrid.GetCount()):
-            p = self.propgrid.Get(i)
-            # apply the change from editing
-            p.Activated(False)
-            if p.IsSeparator():
-                continue
-            # start of a group
+        convert[p.GetName()] = p.GetValue()
+        index += 1
+        while index < self.propgrid.GetCount():
+            p = self.propgrid.Get(index)
             if p.GetIndent() == 0:
-                if convert:
-                    settings.append(convert)
-                convert = {}
+                break
+            if p.GetName() == 'args':
+                index += 1
+                args = []
+                while index < self.propgrid.GetCount():
+                    p = self.propgrid.Get(index)
+                    if p is None or p.GetIndent() <= 1:
+                        break
+                    name = p.GetValue()
+                    p = self.propgrid.Get(index+1)
+                    signal = p.GetValue()
+                    p = self.propgrid.Get(index+2)
+                    default = p.GetValue()
+                    args.append([name, signal, default])
+                    index += 3
+                convert['args'] = args
+                continue
             name = p.GetName()
             value = p.GetValue()
             if isinstance(p, PropCheckBox):
                 value = bool(value)
+            if name == 'inputs':
+                value = [v.strip() for v in value.split(',')]
             convert[name] = value
-        # add the last group
-        if convert:
-            settings.append(convert)
+            index += 1
+        return convert, index
+
+    def GetSettings(self):
+        for i in range(self.propgrid.GetCount()):
+            p = self.propgrid.Get(i)
+            # apply the change from editing
+            p.Activated(False)
+
+        settings = []
+        index = 0
+        while index < self.propgrid.GetCount():
+            convert, index = self.GetConvert(index)
+            if convert:
+                settings.append(convert)
         return settings
```

### Comparing `bsmutility-0.1.3/bsmutility/utility.py` & `bsmutility-0.1.4/bsmutility/utility.py`

 * *Files identical despite different names*

### Comparing `bsmutility-0.1.3/bsmutility.egg-info/PKG-INFO` & `bsmutility-0.1.4/bsmutility.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bsmutility
-Version: 0.1.3
+Version: 0.1.4
 Summary: Some helper class
 Author-email: Tianzhu Qiao <tq@feiyilin.com>
 License: MIT License
         
         Copyright (c) 2024 Tianzhu Qiao
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `bsmutility-0.1.3/bsmutility.egg-info/SOURCES.txt` & `bsmutility-0.1.4/bsmutility.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bsmutility-0.1.3/pyproject.toml` & `bsmutility-0.1.4/pyproject.toml`

 * *Files identical despite different names*

