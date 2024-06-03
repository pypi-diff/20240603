# Comparing `tmp/mplpanel-0.1.2.tar.gz` & `tmp/mplpanel-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mplpanel-0.1.2.tar", last modified: Mon Mar 11 03:57:33 2024, max compression
+gzip compressed data, was "mplpanel-0.1.3.tar", last modified: Mon Jun  3 04:07:08 2024, max compression
```

## Comparing `mplpanel-0.1.2.tar` & `mplpanel-0.1.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 tianzhuqiao   (501) staff       (20)        0 2024-03-11 03:57:33.997265 mplpanel-0.1.2/
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)     1313 2024-03-11 03:57:33.996394 mplpanel-0.1.2/PKG-INFO
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)      956 2024-02-24 17:35:17.000000 mplpanel-0.1.2/README.md
-drwxr-xr-x   0 tianzhuqiao   (501) staff       (20)        0 2024-03-11 03:57:33.975616 mplpanel-0.1.2/demo/
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)        0 2024-02-06 01:36:28.000000 mplpanel-0.1.2/demo/__init__.py
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)      631 2024-02-06 01:36:28.000000 mplpanel-0.1.2/demo/demo.py
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)     1899 2024-02-11 17:01:10.000000 mplpanel-0.1.2/demo/demo_backend.py
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)     1326 2024-02-06 01:36:28.000000 mplpanel-0.1.2/demo/demo_panel.py
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)    13656 2024-02-06 01:36:28.000000 mplpanel-0.1.2/demo/frameplus.py
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)     4625 2024-02-06 01:36:28.000000 mplpanel-0.1.2/demo/mainframe.py
-drwxr-xr-x   0 tianzhuqiao   (501) staff       (20)        0 2024-03-11 03:57:33.989412 mplpanel-0.1.2/mplpanel/
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)      279 2024-02-09 06:03:28.000000 mplpanel-0.1.2/mplpanel/__init__.py
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)    33186 2024-03-09 19:09:44.000000 mplpanel-0.1.2/mplpanel/graph.py
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)     1931 2024-02-06 01:36:28.000000 mplpanel-0.1.2/mplpanel/graph_backend.py
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)     3840 2024-02-06 01:36:28.000000 mplpanel-0.1.2/mplpanel/graph_canvas.py
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)     5855 2024-03-09 19:09:44.000000 mplpanel-0.1.2/mplpanel/graph_common.py
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)    21567 2024-03-09 19:09:44.000000 mplpanel-0.1.2/mplpanel/graph_datatip.py
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)    12989 2024-02-10 04:44:13.000000 mplpanel-0.1.2/mplpanel/graph_dock.py
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)     9558 2024-03-09 19:09:44.000000 mplpanel-0.1.2/mplpanel/graph_edit.py
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)    11019 2024-03-09 19:09:44.000000 mplpanel-0.1.2/mplpanel/graph_subplot.py
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)     6102 2024-02-06 01:36:28.000000 mplpanel-0.1.2/mplpanel/graph_svg.py
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)    24612 2024-03-09 19:09:44.000000 mplpanel-0.1.2/mplpanel/graph_timeline.py
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)     5928 2024-02-06 01:36:28.000000 mplpanel-0.1.2/mplpanel/graph_toolbar.py
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)     3970 2024-02-06 01:36:28.000000 mplpanel-0.1.2/mplpanel/utility.py
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)      184 2024-03-11 03:56:27.000000 mplpanel-0.1.2/mplpanel/version.py
-drwxr-xr-x   0 tianzhuqiao   (501) staff       (20)        0 2024-03-11 03:57:33.994659 mplpanel-0.1.2/mplpanel.egg-info/
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)     1313 2024-03-11 03:57:33.000000 mplpanel-0.1.2/mplpanel.egg-info/PKG-INFO
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)      617 2024-03-11 03:57:33.000000 mplpanel-0.1.2/mplpanel.egg-info/SOURCES.txt
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)        1 2024-03-11 03:57:33.000000 mplpanel-0.1.2/mplpanel.egg-info/dependency_links.txt
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)       16 2024-03-11 03:57:33.000000 mplpanel-0.1.2/mplpanel.egg-info/requires.txt
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)        9 2024-03-11 03:57:33.000000 mplpanel-0.1.2/mplpanel.egg-info/top_level.txt
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)      657 2024-02-09 06:02:26.000000 mplpanel-0.1.2/pyproject.toml
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)       38 2024-03-11 03:57:33.997433 mplpanel-0.1.2/setup.cfg
+drwxr-xr-x   0 tianzhuqiao   (501) staff       (20)        0 2024-06-03 04:07:08.864356 mplpanel-0.1.3/
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     1313 2024-06-03 04:07:08.863585 mplpanel-0.1.3/PKG-INFO
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)      956 2024-02-24 17:35:17.000000 mplpanel-0.1.3/README.md
+drwxr-xr-x   0 tianzhuqiao   (501) staff       (20)        0 2024-06-03 04:07:08.844548 mplpanel-0.1.3/demo/
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)        0 2024-02-06 01:36:28.000000 mplpanel-0.1.3/demo/__init__.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)      631 2024-02-06 01:36:28.000000 mplpanel-0.1.3/demo/demo.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     1899 2024-02-11 17:01:10.000000 mplpanel-0.1.3/demo/demo_backend.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     1326 2024-02-06 01:36:28.000000 mplpanel-0.1.3/demo/demo_panel.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)    13656 2024-02-06 01:36:28.000000 mplpanel-0.1.3/demo/frameplus.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     4625 2024-02-06 01:36:28.000000 mplpanel-0.1.3/demo/mainframe.py
+drwxr-xr-x   0 tianzhuqiao   (501) staff       (20)        0 2024-06-03 04:07:08.858608 mplpanel-0.1.3/mplpanel/
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)      279 2024-02-09 06:03:28.000000 mplpanel-0.1.3/mplpanel/__init__.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)    33356 2024-04-10 15:55:44.000000 mplpanel-0.1.3/mplpanel/graph.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     1931 2024-02-06 01:36:28.000000 mplpanel-0.1.3/mplpanel/graph_backend.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     3840 2024-02-06 01:36:28.000000 mplpanel-0.1.3/mplpanel/graph_canvas.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     5855 2024-03-09 19:09:44.000000 mplpanel-0.1.3/mplpanel/graph_common.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)    21567 2024-03-09 19:09:44.000000 mplpanel-0.1.3/mplpanel/graph_datatip.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)    12989 2024-02-10 04:44:13.000000 mplpanel-0.1.3/mplpanel/graph_dock.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     9558 2024-03-09 19:09:44.000000 mplpanel-0.1.3/mplpanel/graph_edit.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)    11019 2024-03-09 19:09:44.000000 mplpanel-0.1.3/mplpanel/graph_subplot.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     6102 2024-02-06 01:36:28.000000 mplpanel-0.1.3/mplpanel/graph_svg.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)    25182 2024-06-03 04:02:22.000000 mplpanel-0.1.3/mplpanel/graph_timeline.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     5928 2024-02-06 01:36:28.000000 mplpanel-0.1.3/mplpanel/graph_toolbar.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     3970 2024-02-06 01:36:28.000000 mplpanel-0.1.3/mplpanel/utility.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)      184 2024-06-03 04:02:44.000000 mplpanel-0.1.3/mplpanel/version.py
+drwxr-xr-x   0 tianzhuqiao   (501) staff       (20)        0 2024-06-03 04:07:08.862778 mplpanel-0.1.3/mplpanel.egg-info/
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     1313 2024-06-03 04:07:08.000000 mplpanel-0.1.3/mplpanel.egg-info/PKG-INFO
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)      617 2024-06-03 04:07:08.000000 mplpanel-0.1.3/mplpanel.egg-info/SOURCES.txt
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)        1 2024-06-03 04:07:08.000000 mplpanel-0.1.3/mplpanel.egg-info/dependency_links.txt
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)       16 2024-06-03 04:07:08.000000 mplpanel-0.1.3/mplpanel.egg-info/requires.txt
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)        9 2024-06-03 04:07:08.000000 mplpanel-0.1.3/mplpanel.egg-info/top_level.txt
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)      657 2024-02-09 06:02:26.000000 mplpanel-0.1.3/pyproject.toml
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)       38 2024-06-03 04:07:08.864574 mplpanel-0.1.3/setup.cfg
```

### Comparing `mplpanel-0.1.2/PKG-INFO` & `mplpanel-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mplpanel
-Version: 0.1.2
+Version: 0.1.3
 Summary: A wx.Panel to use matplotlib plot in wxPython
 Author-email: Tianzhu Qiao <tq@feiyilin.com>
 Project-URL: Homepage, https://github.com/tianzhuqiao/mplpanel
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 Requires-Dist: wxpython>=4.2.1
```

### Comparing `mplpanel-0.1.2/README.md` & `mplpanel-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `mplpanel-0.1.2/demo/demo.py` & `mplpanel-0.1.3/demo/demo.py`

 * *Files identical despite different names*

### Comparing `mplpanel-0.1.2/demo/demo_backend.py` & `mplpanel-0.1.3/demo/demo_backend.py`

 * *Files identical despite different names*

### Comparing `mplpanel-0.1.2/demo/demo_panel.py` & `mplpanel-0.1.3/demo/demo_panel.py`

 * *Files identical despite different names*

### Comparing `mplpanel-0.1.2/demo/frameplus.py` & `mplpanel-0.1.3/demo/frameplus.py`

 * *Files identical despite different names*

### Comparing `mplpanel-0.1.2/demo/mainframe.py` & `mplpanel-0.1.3/demo/mainframe.py`

 * *Files identical despite different names*

### Comparing `mplpanel-0.1.2/mplpanel/graph.py` & `mplpanel-0.1.3/mplpanel/graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -447,14 +447,15 @@
         action = self.actions.get(self.mode, None)
         if action is None or not hasattr(action, 'mouse_move'):
             if not self.mode:
                 self.dock.mouse_move(event)
             return
         if action.mouse_move(event):
             self.canvas.draw()
+
     def OnScroll(self, event):
         self.do_zoom(event)
 
     def OnZoomFun(self, event):
         # get the current x and y limits
         if not self.GetToolToggled(self.wx_ids['Zoom']):
             return
@@ -468,31 +469,33 @@
                 if a.in_axes(event)]
 
         yzoom_key = xzoom_key = True
         if wx.GetKeyState(wx.WXK_CONTROL_X):
             yzoom_key = False
         elif wx.GetKeyState(wx.WXK_CONTROL_Y):
             xzoom_key = False
-        xzoom = yzoom = xzoom_key, yzoom_key
+        xzoom, yzoom = xzoom_key, yzoom_key
         xdata, ydata = event.xdata, event.ydata
         axes = [[a, xzoom, yzoom, xdata, ydata] for a in self.figure.get_axes()
                 if a.in_axes(event)]
         if not axes:
             axes = []
             for ax in self.figure.get_axes():
                 x,y = event.x, event.y
                 xAxes, yAxes = ax.transAxes.inverted().transform([x, y])
-                if -0.1 < xAxes < 0:
-                    xzoom = False
-                if -0.1 < yAxes < 0:
-                    yzoom = False
+                xzoom, yzoom = False, False
+                if -0.1 < xAxes < 0 and 0 < yAxes < 1:
+                    # the mouse is near the right edge of the axes
+                    yzoom = yzoom_key
+                if -0.1 < yAxes < 0 and 0 < xAxes < 1:
+                    # the mouse is near the bottom edge of the axes
+                    xzoom = xzoom_key
                 xdata, ydata = ax.transData.inverted().transform([x, y])
                 if not yzoom or (not xzoom and -0.05 < yAxes < 1):
                     axes.append([ax, xzoom, yzoom, xdata, ydata])
-                xzoom = yzoom = xzoom_key, yzoom_key
             if not axes:
                 return
 
         base_scale = 2.0
         if event.button == 'up':
             # deal with zoom in
             scale_factor = 1.0 / base_scale
```

### Comparing `mplpanel-0.1.2/mplpanel/graph_backend.py` & `mplpanel-0.1.3/mplpanel/graph_backend.py`

 * *Files identical despite different names*

### Comparing `mplpanel-0.1.2/mplpanel/graph_canvas.py` & `mplpanel-0.1.3/mplpanel/graph_canvas.py`

 * *Files identical despite different names*

### Comparing `mplpanel-0.1.2/mplpanel/graph_common.py` & `mplpanel-0.1.3/mplpanel/graph_common.py`

 * *Files identical despite different names*

### Comparing `mplpanel-0.1.2/mplpanel/graph_datatip.py` & `mplpanel-0.1.3/mplpanel/graph_datatip.py`

 * *Files identical despite different names*

### Comparing `mplpanel-0.1.2/mplpanel/graph_dock.py` & `mplpanel-0.1.3/mplpanel/graph_dock.py`

 * *Files identical despite different names*

### Comparing `mplpanel-0.1.2/mplpanel/graph_edit.py` & `mplpanel-0.1.3/mplpanel/graph_edit.py`

 * *Files identical despite different names*

### Comparing `mplpanel-0.1.2/mplpanel/graph_subplot.py` & `mplpanel-0.1.3/mplpanel/graph_subplot.py`

 * *Files identical despite different names*

### Comparing `mplpanel-0.1.2/mplpanel/graph_svg.py` & `mplpanel-0.1.3/mplpanel/graph_svg.py`

 * *Files identical despite different names*

### Comparing `mplpanel-0.1.2/mplpanel/graph_timeline.py` & `mplpanel-0.1.3/mplpanel/graph_timeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,26 +154,28 @@
            self.line3() is None or self.text() is None:
             return
 
         if not (self.active in [self.line(), self.line2()]):
             return
         xdata = data
         x, idx = None, None
+        x_min = np.inf
         if xdata is None:
             xdata = self.active.get_xdata()[0]
-
         for l in self.active.axes.lines:
             label = l.get_label()
             if label.startswith('_bsm'):
                 # legend is not visible
                 continue
-            x = l.get_xdata()
-            idx = np.argmin(np.abs(x - xdata))
-            break
-
+            lx = l.get_xdata()
+            lidx = np.argmin(np.abs(lx - xdata))
+            if np.abs(lx[lidx] - xdata) < x_min:
+                x_min = np.abs(lx[lidx] - xdata)
+                x = lx
+                idx = lidx
         if x is not None and idx is not None:
             self.active.set_xdata([x[idx], x[idx]])
             if self.active == self.line():
                 self.line_idx = idx
             else:
                 self.line2_idx = idx
             start = self.line().get_xdata()[0]
@@ -296,34 +298,41 @@
         self.y_aux_line.create_if_needed()
 
     def update_legend(self, xdata = None):
         # update x-axis axvline and legend
         if xdata is None:
             xdata = self.axvline().get_xdata()[0]
         x, y, idx = None, None, None
+        x_min = np.inf
         for l in self.ax().lines:
             label = l.get_label()
+            if label.startswith('_bsm'):
+                # ignore _bsm line
+                continue
+            lx = l.get_xdata()
+            lidx = np.argmin(np.abs(lx - xdata))
+            if np.abs(lx[lidx] - xdata) < x_min:
+                x_min = np.abs(lx[lidx] - xdata)
+                x = lx
+                idx = lidx
             if label.startswith('_'):
                 # legend is not visible
                 continue
 
             label = label.split(' ')
             if len(label) > 1:
                 label = label[:-1]
             label = ' '.join(label)
-            x = l.get_xdata()
             y = l.get_ydata()
             idx = np.argmin(np.abs(x - xdata))
             label = f'{label} {y[idx]:g}'
             l.set_label(label)
-
         if x is not None and idx is not None:
             self.axvline().set_xdata([x[idx], x[idx]])
             self.axvline_idx = idx
-            #self.update_x_axvline2()
 
     def hit_test(self, x, y):
         # check if (x, y) is close to the axvline in ax
         for line in (self.axvline,):
             if line is None:
                 continue
             line = line()
@@ -582,20 +591,22 @@
         for ax in axes:
             axline = self.get(ax, create=False)
             if axline is None:
                 continue
             idx = axline.axvline_idx
             for l in ax.lines:
                 label = l.get_label()
-                if label.startswith('_'):
+                if label.startswith('_bsm'):
                     continue
-                label = label.split(' ')
-                if len(label) > 1:
-                    label = label[:-1]
-                label = ' '.join(label)
+                if not label.startswith('_'):
+                    # visible legend, remove value first
+                    label = label.split(' ')
+                    if len(label) > 1:
+                        label = label[:-1]
+                    label = ' '.join(label)
                 x = l.get_xdata()
                 y = l.get_ydata()
                 sharex = self.get_sharex(ax)
                 if sharex not in data:
                     data[sharex] = pd.DataFrame()
                     data[sharex]['x'] = [x[idx]]
                 data[sharex][label] = [y[idx]]
```

### Comparing `mplpanel-0.1.2/mplpanel/graph_toolbar.py` & `mplpanel-0.1.3/mplpanel/graph_toolbar.py`

 * *Files identical despite different names*

### Comparing `mplpanel-0.1.2/mplpanel/utility.py` & `mplpanel-0.1.3/mplpanel/utility.py`

 * *Files identical despite different names*

### Comparing `mplpanel-0.1.2/mplpanel.egg-info/PKG-INFO` & `mplpanel-0.1.3/mplpanel.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mplpanel
-Version: 0.1.2
+Version: 0.1.3
 Summary: A wx.Panel to use matplotlib plot in wxPython
 Author-email: Tianzhu Qiao <tq@feiyilin.com>
 Project-URL: Homepage, https://github.com/tianzhuqiao/mplpanel
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 Requires-Dist: wxpython>=4.2.1
```

### Comparing `mplpanel-0.1.2/mplpanel.egg-info/SOURCES.txt` & `mplpanel-0.1.3/mplpanel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mplpanel-0.1.2/pyproject.toml` & `mplpanel-0.1.3/pyproject.toml`

 * *Files identical despite different names*

