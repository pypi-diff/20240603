# Comparing `tmp/propgrid-0.1.3.tar.gz` & `tmp/propgrid-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "propgrid-0.1.3.tar", last modified: Sun Mar 31 03:16:44 2024, max compression
+gzip compressed data, was "propgrid-0.1.4.tar", last modified: Mon Jun  3 04:00:00 2024, max compression
```

## Comparing `propgrid-0.1.3.tar` & `propgrid-0.1.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 tianzhuqiao   (501) staff       (20)        0 2024-03-31 03:16:44.964966 propgrid-0.1.3/
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)     1069 2023-02-14 21:59:49.000000 propgrid-0.1.3/LICENSE
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)     2090 2024-03-31 03:16:44.964277 propgrid-0.1.3/PKG-INFO
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)      455 2024-02-24 17:28:35.000000 propgrid-0.1.3/README.md
-drwxr-xr-x   0 tianzhuqiao   (501) staff       (20)        0 2024-03-31 03:16:44.960381 propgrid-0.1.3/propgrid/
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)      176 2024-02-06 06:36:19.000000 propgrid-0.1.3/propgrid/__init__.py
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)     2144 2023-02-17 17:53:11.000000 propgrid-0.1.3/propgrid/enumtype.py
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)    25985 2023-12-25 00:41:55.000000 propgrid-0.1.3/propgrid/formatters.py
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)    41983 2024-03-29 00:54:19.000000 propgrid-0.1.3/propgrid/prop.py
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)    11383 2024-03-29 21:51:36.000000 propgrid-0.1.3/propgrid/propart.py
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)    38898 2024-03-31 03:13:01.000000 propgrid-0.1.3/propgrid/propgrid.py
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)     2507 2023-02-17 17:53:11.000000 propgrid-0.1.3/propgrid/propxpm.py
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)    15265 2023-12-17 19:32:57.000000 propgrid-0.1.3/propgrid/validators.py
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)      184 2024-03-30 05:45:03.000000 propgrid-0.1.3/propgrid/version.py
-drwxr-xr-x   0 tianzhuqiao   (501) staff       (20)        0 2024-03-31 03:16:44.963516 propgrid-0.1.3/propgrid.egg-info/
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)     2090 2024-03-31 03:16:44.000000 propgrid-0.1.3/propgrid.egg-info/PKG-INFO
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)      377 2024-03-31 03:16:44.000000 propgrid-0.1.3/propgrid.egg-info/SOURCES.txt
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)        1 2024-03-31 03:16:44.000000 propgrid-0.1.3/propgrid.egg-info/dependency_links.txt
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)       16 2024-03-31 03:16:44.000000 propgrid-0.1.3/propgrid.egg-info/requires.txt
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)       18 2024-03-31 03:16:44.000000 propgrid-0.1.3/propgrid.egg-info/top_level.txt
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)      660 2024-02-06 06:35:24.000000 propgrid-0.1.3/pyproject.toml
--rw-r--r--   0 tianzhuqiao   (501) staff       (20)       38 2024-03-31 03:16:44.965113 propgrid-0.1.3/setup.cfg
+drwxr-xr-x   0 tianzhuqiao   (501) staff       (20)        0 2024-06-03 04:00:00.405349 propgrid-0.1.4/
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     1069 2023-02-14 21:59:49.000000 propgrid-0.1.4/LICENSE
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     2090 2024-06-03 04:00:00.404550 propgrid-0.1.4/PKG-INFO
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)      455 2024-02-24 17:28:35.000000 propgrid-0.1.4/README.md
+drwxr-xr-x   0 tianzhuqiao   (501) staff       (20)        0 2024-06-03 04:00:00.400625 propgrid-0.1.4/propgrid/
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)      176 2024-02-06 06:36:19.000000 propgrid-0.1.4/propgrid/__init__.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     2144 2023-02-17 17:53:11.000000 propgrid-0.1.4/propgrid/enumtype.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)    25985 2023-12-25 00:41:55.000000 propgrid-0.1.4/propgrid/formatters.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)    42422 2024-05-11 05:15:58.000000 propgrid-0.1.4/propgrid/prop.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)    11383 2024-03-29 21:51:36.000000 propgrid-0.1.4/propgrid/propart.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)    39247 2024-05-11 05:15:58.000000 propgrid-0.1.4/propgrid/propgrid.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     2507 2023-02-17 17:53:11.000000 propgrid-0.1.4/propgrid/propxpm.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)    15265 2023-12-17 19:32:57.000000 propgrid-0.1.4/propgrid/validators.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)      184 2024-05-31 04:59:48.000000 propgrid-0.1.4/propgrid/version.py
+drwxr-xr-x   0 tianzhuqiao   (501) staff       (20)        0 2024-06-03 04:00:00.403735 propgrid-0.1.4/propgrid.egg-info/
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     2090 2024-06-03 04:00:00.000000 propgrid-0.1.4/propgrid.egg-info/PKG-INFO
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)      377 2024-06-03 04:00:00.000000 propgrid-0.1.4/propgrid.egg-info/SOURCES.txt
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)        1 2024-06-03 04:00:00.000000 propgrid-0.1.4/propgrid.egg-info/dependency_links.txt
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)       16 2024-06-03 04:00:00.000000 propgrid-0.1.4/propgrid.egg-info/requires.txt
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)       18 2024-06-03 04:00:00.000000 propgrid-0.1.4/propgrid.egg-info/top_level.txt
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)      660 2024-02-06 06:35:24.000000 propgrid-0.1.4/pyproject.toml
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)       38 2024-06-03 04:00:00.405521 propgrid-0.1.4/setup.cfg
```

### Comparing `propgrid-0.1.3/LICENSE` & `propgrid-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `propgrid-0.1.3/PKG-INFO` & `propgrid-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propgrid
-Version: 0.1.3
+Version: 0.1.4
 Summary: A lightweight propgrid in wxpython to show/config data
 Author-email: Tianzhu Qiao <tq@feiyilin.com>
 License: MIT License
         
         Copyright (c) 2018 Tianzhu Qiao
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `propgrid-0.1.3/propgrid/enumtype.py` & `propgrid-0.1.4/propgrid/enumtype.py`

 * *Files identical despite different names*

### Comparing `propgrid-0.1.3/propgrid/formatters.py` & `propgrid-0.1.4/propgrid/formatters.py`

 * *Files identical despite different names*

### Comparing `propgrid-0.1.3/propgrid/prop.py` & `propgrid-0.1.4/propgrid/prop.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         self.font_label = None
         self.font_value = None
         self.has_children = False
         self.expanded = True
         self.visible = True
         self.readonly = False
         #self.window = None
-        self.parent = -1
+        self.parent = None
         self.SetTextColor(silent=True)
         self.SetBgColor(silent=True)
         if wx.Platform == '__WXMSW__':
             self.min_size = wx.Size(200, 35)
         else:
             self.min_size = wx.Size(200, 25)
         self.rect = wx.Rect(0, 0, 0, 0)
@@ -290,14 +290,26 @@
         if not silent:
             self.Refresh(True)
 
     def IsVisible(self):
         """return true if the property is visible"""
         return self.visible
 
+    def IsShown(self):
+        parent = self.GetParent()
+        if parent is not None:
+            return self.IsVisible() and parent.IsExpanded() and parent.IsShown()
+        return self.IsVisible()
+
+    def Show(self):
+        self.Visible(True)
+        if self.GetParent():
+            self.GetParent().Expand(True).Show()
+        return self
+
     def Parent(self, prop):
         """set the parent property"""
         self.SetParent(prop)
         return self
 
     def SetParent(self, prop):
         """set the parent property"""
@@ -825,30 +837,32 @@
 
     def doCreateControl(self):
         return None
 
     def CreateControl(self):
         """create the control"""
         if self.window is not None:
-            return
+            return False
         if not self.allow_editing:
-            return
+            return False
         win = self.doCreateControl()
 
         if win is not None:
             if win.GetValidator():
                 win.GetValidator().TransferToWindow()
             self.window = win
             # the window size may be larger than the value rect, notify parent
             # grid to update it
             self.Resize()
             self.LayoutControl()
             self.window.SetFocus()
             #self.window.Bind(wx.EVT_KILL_FOCUS, self.OnKillFocus)
             self.draws['value'] = False
+            return True
+        return False
 
     def OnMouseDown(self, pt):
         ht = super().OnMouseDown(pt)
 
         if self.IsEnabled() and ht == 'value':
             if not self.IsReadonly() and self.IsActivated():
                 self.CreateControl()
@@ -879,20 +893,21 @@
             if ht is None:
                 self.UpdatePropValue()
                 self.DestroyControl()
 
         return super().OnMouseRightClick(pt)
 
     def OnKeyDown(self, evt):
+        if self.window:
+            return False
         if super().OnKeyDown(evt):
             return True
         keycode = evt.GetKeyCode()
         if keycode == wx.WXK_SPACE:
-            self.CreateControl()
-            return True
+            return self.CreateControl()
         if keycode == wx.WXK_ESCAPE:
             self.OnTextEnter()
             return True
         return False
 
     def OnTextEnter(self):
         self.UpdatePropValue()
```

### Comparing `propgrid-0.1.3/propgrid/propart.py` & `propgrid-0.1.4/propgrid/propart.py`

 * *Files identical despite different names*

### Comparing `propgrid-0.1.3/propgrid/propgrid.py` & `propgrid-0.1.4/propgrid/propgrid.py`

 * *Files 6% similar despite different names*

```diff
@@ -90,14 +90,15 @@
 
         self.SetDropTarget(PropDropTarget(self))
         self.draggable = True
         self.configurable = True
 
         self.drag_image = None
         self.drag_bitmap = None
+        self.edit_mode = True
 
         self.Bind(wx.EVT_PAINT, self.OnPaint)
         self.Bind(wx.EVT_SIZE, self.OnSize)
         self.Bind(wx.EVT_ERASE_BACKGROUND, self.OnEraseBackground)
         self.Bind(wx.EVT_LEFT_DOWN, self.OnMouseDown)
         self.Bind(wx.EVT_LEFT_UP, self.OnMouseUp)
         self.Bind(wx.EVT_RIGHT_DOWN, self.OnMouseRightClick)
@@ -119,15 +120,15 @@
         self.Bind(EVT_PROP_DOUBLE_CLICK, self.OnPropEventsHandler)
         self.Bind(EVT_PROP_INDENT, self.OnPropEventsHandler)
         self.Bind(EVT_PROP_KEYDOWN, self.OnPropEventsHandler)
         self.Bind(EVT_PROP_RESIZE, self.OnPropEventsHandler)
         self.Bind(EVT_PROP_REFRESH, self.OnPropRefresh)
         self.Bind(EVT_PROP_DROP, self.OnPropEventsHandler)
         self.Bind(EVT_PROP_BEGIN_DRAG, self.OnPropEventsHandler)
-        self.Bind(wx.EVT_MENU, self.OnProcessCommand)
+        #self.Bind(wx.EVT_MENU, self.OnProcessCommand)
         self.SetBackgroundStyle(wx.BG_STYLE_PAINT)
 
     def CreateDragImage(self, prop):
         memory = wx.MemoryDC(wx.Bitmap(1, 1))
 
         w, h = prop.GetSize()
         w = min(500, w-100)
@@ -153,39 +154,52 @@
     def SetArtProvider(self, art):
         self._art = art
         self.Refresh()
 
     def GetArtProvider(self):
         return self._art
 
+    def EditMode(self, enable):
+        """set if it is allow to edit the propgrid"""
+        self.SetEditMode(enable)
+        return self
+
+    def SetEditMode(self, enable):
+        """set if it is allow to edit the propgrid"""
+        self.edit_mode = enable
+
+    def GetEditMode(self):
+        """get if it is allow to edit the propgrid"""
+        return self.edit_mode
+
     def Draggable(self, draggable):
         """set if it is allow to drag/drop any prop"""
         self.SetDraggable(draggable)
         return self
 
     def SetDraggable(self, draggable):
         """set if it is allow to drag/drop any prop"""
         self.draggable = draggable
 
     def IsDraggable(self):
         """get if it is allow to drag/drop any prop"""
-        return self.draggable
+        return self.draggable and self.GetEditMode()
 
     def Configurable(self, configurable):
         """set if it is allow to drag/drop any prop"""
         self.SetConfigurable(configurable)
         return self
 
     def SetConfigurable(self, configurable):
         """set if it is allow to drag/drop any prop"""
         self.configurable = configurable
 
     def IsConfigurable(self):
         """get if it is allow to drag/drop any prop"""
-        return self.configurable
+        return self.configurable and self.GetEditMode()
 
     def Append(self, prop, update=True):
         return self.Insert(prop, -1, update)
 
     def Insert(self, prop, index=-1, update=True):
         # add the prop window to the grid
         if not isinstance(prop, PropBase):
@@ -354,24 +368,24 @@
             # move zero step is no move at all
             return
 
         # calculate the new position
         index2 = index
         # move up
         while step < 0 and index2 >= 1:
-           index2 -= 1
-           p = self.Get(index2)
-           if p.IsVisible():
-               step += 1
+            index2 -= 1
+            p = self.Get(index2)
+            if p.IsShown():
+                step += 1
 
         # move down
         while step > 0 and index2 < self.GetCount()-1:
             index2 += 1
             p = self.Get(index2)
-            if p.IsVisible():
+            if p.IsShown():
                 step -= 1
 
         index2 += step
 
         if index2 < 0:
             index2 = 0
         # move the prop, prop will be placed on top of index2
@@ -446,81 +460,89 @@
         eventObject = self.GetParent()
         evt.SetEventObject(eventObject)
         evtHandler = eventObject.GetEventHandler()
 
         evtHandler.ProcessEvent(evt)
         return not evt.GetVeto()
 
-    def NavigateProp(self, down):
+    def NavigateProp(self, down, loop=False):
         """change the selected property"""
+        if self.GetCount() == 0:
+            return
         sel = self.GetSelection()
+        looped = False
         # find the next visible property and activate it
         while True:
             if down:
                 sel += 1
             else:
                 sel -= 1
 
             if sel < 0 or sel >= self.GetCount():
-                break
+                if loop and not looped:
+                    sel %= self.GetCount()
+                    # to avoid loop forever
+                    looped = True
+                else:
+                    break
 
             prop = self._props[sel]
-            if prop.IsVisible():
+            if prop.IsShown():
                 self.SetSelection(sel)
                 self.EnsureVisible(sel)
                 break
 
     def PropHitTest(self, pt):
         """find the property under the mouse"""
         for i, prop in enumerate(self._props):
             prop = self._props[i]
-            if not prop.IsVisible():
+            if not prop.IsShown():
                 continue
             if prop.GetRect().Contains(pt):
                 return i
         return -1
 
     def LayoutAll(self, update=True):
         """layout the properties"""
         rc = self.GetClientRect()
         (w, h) = (rc.width, 1)
 
         self.CheckProp()
         # calculate the width and height
         for p in self._props:
-            if p.IsVisible():
+            if p.IsShown():
                 sz = p.GetMinSize()
                 w = max(w, sz.x)
                 h = h + sz.y
         if update:
             # update the virtual size
             self.SetVirtualSize(wx.Size(w, h))
 
         # set the property rect
         rc = self.GetClientRect()
         w, y = max(w, rc.width), 1
         for p in self._props:
-            if p.IsVisible():
+            if p.IsShown():
                 h = p.GetMinSize().y
                 p.SetRect(wx.Rect(0, y, w, h))
                 # let art provider update drawing regions (e.g., value rect)
                 self._art.PrepareDrawRect(p)
                 y += h
         prev_prop = None
         for p in self._props:
-            if not  p.IsVisible():
+            if not p.IsShown():
                 continue
             p.top_value_border = False
             if prev_prop is None or prev_prop.IsSeparator() or p.IsSeparator():
                 p.top_value_border = True
             prev_prop = p
 
         next_prop = None
         for p in reversed(self._props):
-            if not  p.IsVisible():
+            if not p.IsShown():
                 continue
             p.bottom_value_border = False
             if next_prop is None or next_prop.IsSeparator() or p.IsSeparator():
                 p.bottom_value_border = True
             next_prop = p
 
     def GetDrawRect(self):
@@ -548,25 +570,14 @@
             if parent:
                 # the parent has children now
                 parent.SetHasChildren(True, True)
             # the current one does not have children yet; will be set by its
             # children
             prop.SetHasChildren(False, True)
 
-        # show/hide the properties
-        for prop in self._props:
-            parent = prop.GetParent()
-            if not parent:
-                # always show prop without parent
-                show = True
-            else:
-                # prop with parent depends on parent's status
-                show = parent.IsExpanded() and parent.IsVisible()
-            prop.SetVisible(show)
-
     def OnPropRefresh(self, evt):
         """refresh the property, for example, due to value changed"""
         self.SendPropEvent(evt.GetEventType(), evt.GetProp())
         prop = evt.GetProp()
         if prop is None:
             return
         rc = prop.GetRect()
@@ -646,38 +657,48 @@
         """key down event"""
         prop = self.prop_selected
         skip = True
         keycode = evt.GetKeyCode()
         if prop and self.SendPropEvent(wxEVT_PROP_KEYDOWN, prop, keycode=keycode):
             index = self.GetSelection()
             indent = prop.GetIndent()
-            if self.HasFocus():
-                if prop.OnKeyDown(evt):
-                    # the prop has process the event
-                    skip = False
-                elif keycode == wx.WXK_UP:
-                    if evt.CmdDown():
-                        # Ctrl + Up move up
-                        self.MovePropertyUp(index)
-                    else:
-                        # Up select the above property
-                        self.NavigateProp(False)
-                    skip = False
-                elif keycode == wx.WXK_DOWN:
-                    if evt.CmdDown():
-                        # Ctrl + Down move the property down
-                        self.MovePropertyDown(index)
-                    else:
-                        # Down select the property below
-                        self.NavigateProp(True)
-                    skip = False
-                elif keycode == wx.WXK_DELETE:
-                    # delete the property
-                    self.Delete(self.GetSelected())
-                    skip = False
+            if prop.OnKeyDown(evt):
+                # the prop has process the event
+                skip = False
+            elif keycode == wx.WXK_TAB:
+                prop.Activated(False)
+                if evt.ShiftDown():
+                    # move up
+                    self.NavigateProp(False, loop=True)
+                else:
+                    # move down
+                    self.NavigateProp(True, loop=True)
+                skip = False
+            elif keycode == wx.WXK_UP:
+                prop.Activated(False)
+                if evt.CmdDown() and self.GetEditMode():
+                    # Ctrl + Up move up
+                    self.MovePropertyUp(index)
+                else:
+                    # Up select the above property
+                    self.NavigateProp(False)
+                skip = False
+            elif keycode == wx.WXK_DOWN:
+                prop.Activated(False)
+                if evt.CmdDown() and self.GetEditMode():
+                    # Ctrl + Down move the property down
+                    self.MovePropertyDown(index)
+                else:
+                    # Down select the property below
+                    self.NavigateProp(True)
+                skip = False
+            elif keycode == wx.WXK_DELETE and self.GetEditMode():
+                # delete the property
+                self.Delete(self.GetSelected())
+                skip = False
         if skip:
             evt.Skip()
 
     def OnPaint(self, event):
         """draw the property"""
         dc = wx.AutoBufferedPaintDC(self)
         self.DoPrepareDC(dc)
@@ -695,15 +716,15 @@
 
         # draw the top edge
         dc.SetPen(wx.Pen(wx.SystemSettings.GetColour(wx.SYS_COLOUR_3DSHADOW)))
         dc.DrawLine(rc.left, rc.top, rc.right, rc.top)
 
         # draw the properties
         for p in self._props:
-            if not p.IsVisible():
+            if not p.IsShown():
                 continue
             rc_prop = p.GetRect()
             if rc.Intersects(rc_prop):
                 self._art.DrawItem(dc, p)
                 p.PostRefresh()
 
     def OnSize(self, evt):
@@ -1007,15 +1028,15 @@
         wx.Dialog.__init__(self,
                            parent,
                            title="Settings...",
                            size=wx.Size(600, 460),
                            style=wx.DEFAULT_DIALOG_STYLE | wx.RESIZE_BORDER)
 
         self.propgrid = PropGrid(self).Configurable(False)
-        self.propgrid.Draggable(False)
+        self.propgrid.EditMode(False)
         self.propgrid.GetArtProvider().SetTitleWidth(200)
         self.prop = prop
         if prop.IsSeparator():
             self.items = (('name', PropText().Label('Name'), ''),
                           ('label', PropText().Label('Label'), ''),
                           ('indent',PropSpin(0, 100).Label('Indent level'), ''),
                           ('font_label', PropFont().Label('Label font'), '_font_label'),
@@ -1067,23 +1088,14 @@
         sz.Add(btnsizer, 0, wx.ALIGN_RIGHT | wx.RIGHT, 5)
 
         self.SetSizer(sz)
         self.Layout()
 
         # Connect Events
         self.Bind(wx.EVT_BUTTON, self.OnBtnOk, id=wx.ID_OK)
-        self.Bind(EVT_PROP_KEYDOWN, self.OnPropKeyDown)
-
-    def OnPropKeyDown(self, event):
-        data = event.GetData()
-        keycode = data.get('keycode', '')
-        if keycode in [wx.WXK_UP, wx.WXK_DOWN] and not wx.GetKeyState(wx.WXK_COMMAND):
-            # only allow up/down
-            return
-        event.Veto()
 
     def OnBtnOk(self, event):
         if self.propgrid.prop_selected:
             # update the value if necessary
             self.propgrid.prop_selected.OnTextEnter()
 
         for (name, pp, _ ) in self.items:
```

### Comparing `propgrid-0.1.3/propgrid/propxpm.py` & `propgrid-0.1.4/propgrid/propxpm.py`

 * *Files identical despite different names*

### Comparing `propgrid-0.1.3/propgrid/validators.py` & `propgrid-0.1.4/propgrid/validators.py`

 * *Files identical despite different names*

### Comparing `propgrid-0.1.3/propgrid.egg-info/PKG-INFO` & `propgrid-0.1.4/propgrid.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propgrid
-Version: 0.1.3
+Version: 0.1.4
 Summary: A lightweight propgrid in wxpython to show/config data
 Author-email: Tianzhu Qiao <tq@feiyilin.com>
 License: MIT License
         
         Copyright (c) 2018 Tianzhu Qiao
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `propgrid-0.1.3/pyproject.toml` & `propgrid-0.1.4/pyproject.toml`

 * *Files identical despite different names*

