# Comparing `tmp/pyacad-0.0.1.tar.gz` & `tmp/pyacad-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyacad-0.0.1.tar", last modified: Mon Mar 25 18:09:19 2024, max compression
+gzip compressed data, was "pyacad-0.0.2.tar", last modified: Mon Jun  3 11:39:09 2024, max compression
```

## Comparing `pyacad-0.0.1.tar` & `pyacad-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-03-25 18:09:19.472697 pyacad-0.0.1/
--rw-rw-rw-   0        0        0     1091 2024-03-25 17:08:22.000000 pyacad-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      317 2024-03-25 18:09:19.472697 pyacad-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      527 2022-02-22 23:15:02.000000 pyacad-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-03-25 18:09:19.457074 pyacad-0.0.1/pyacad/
--rw-rw-rw-   0        0        0     3820 2022-09-26 01:22:32.000000 pyacad-0.0.1/pyacad/APoint.py
--rw-rw-rw-   0        0        0     4801 2022-09-26 14:16:58.000000 pyacad-0.0.1/pyacad/Autocad.py
--rw-rw-rw-   0        0        0      169 2022-09-26 00:27:51.000000 pyacad-0.0.1/pyacad/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-25 18:09:19.472697 pyacad-0.0.1/pyacad.egg-info/
--rw-rw-rw-   0        0        0      317 2024-03-25 18:09:19.000000 pyacad-0.0.1/pyacad.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2024-03-25 18:09:19.000000 pyacad-0.0.1/pyacad.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-25 18:09:19.000000 pyacad-0.0.1/pyacad.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-03-25 18:09:19.000000 pyacad-0.0.1/pyacad.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-03-25 18:09:19.000000 pyacad-0.0.1/pyacad.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-25 18:09:19.472697 pyacad-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      429 2024-03-25 18:09:13.000000 pyacad-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 11:39:09.056628 pyacad-0.0.2/
+-rw-rw-rw-   0        0        0     1091 2024-03-25 17:08:22.000000 pyacad-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      893 2024-06-03 11:39:09.055552 pyacad-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      531 2024-05-30 15:17:47.000000 pyacad-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-06-03 11:39:09.027868 pyacad-0.0.2/pyacad/
+-rw-rw-rw-   0        0        0     3511 2024-03-26 14:42:26.000000 pyacad-0.0.2/pyacad/APoint.py
+-rw-rw-rw-   0        0        0     5090 2024-06-03 10:57:21.000000 pyacad-0.0.2/pyacad/Autocad.py
+-rw-rw-rw-   0        0        0      715 2024-06-03 11:23:23.000000 pyacad-0.0.2/pyacad/Types.py
+-rw-rw-rw-   0        0        0      169 2022-09-26 00:27:51.000000 pyacad-0.0.2/pyacad/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 11:39:09.053522 pyacad-0.0.2/pyacad.egg-info/
+-rw-rw-rw-   0        0        0      893 2024-06-03 11:39:06.000000 pyacad-0.0.2/pyacad.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2024-06-03 11:39:07.000000 pyacad-0.0.2/pyacad.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 11:39:06.000000 pyacad-0.0.2/pyacad.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-06-03 11:39:06.000000 pyacad-0.0.2/pyacad.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-06-03 11:39:06.000000 pyacad-0.0.2/pyacad.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-03 11:39:09.056628 pyacad-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      561 2024-06-03 11:28:00.000000 pyacad-0.0.2/setup.py
```

### Comparing `pyacad-0.0.1/LICENSE` & `pyacad-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyacad-0.0.1/README.md` & `pyacad-0.0.2/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -13,12 +13,12 @@
 ```
 from pyacad import Autocad, APoint
 
 # Create a line in the active document model space.
 acad = Autocad()
 p0 = APoint(1, 1)
 p1 = APoint(2, 3)
-acad.model.AddLine(p0, p1)
+acad.model.AddLine(p0(), p1())
 
 # Zoom the line by extents.
 acad.app.ZoomExtents()
 ```
```

### Comparing `pyacad-0.0.1/pyacad/APoint.py` & `pyacad-0.0.2/pyacad/APoint.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,65 +30,32 @@
     @property
     def x(self):
         """ """
         return self._x
 
     @x.setter
     def x(self, value):
-        """
-
-        Parameters
-        ----------
-        value :
-            
-
-        Returns
-        -------
-
-        """
         self._x = value
 
     @property
     def y(self):
         """ """
         return self._y
 
     @y.setter
     def y(self, value):
-        """
-
-        Parameters
-        ----------
-        value :
-            
-
-        Returns
-        -------
-
-        """
         self._y = value
 
     @property
     def z(self):
         """ """
         return self._z
 
     @z.setter
     def z(self, value):
-        """
-
-        Parameters
-        ----------
-        value :
-            
-
-        Returns
-        -------
-
-        """
         self._z = value
 
     def __call__(self):
         return win32com.client.VARIANT(pythoncom.VT_ARRAY | pythoncom.VT_R8, (self.x, self.y, self.z))
 
     def __getitem__(self, item):
         return list(self)[item]
@@ -143,36 +110,35 @@
 
     def __left_op(self, p1, p2, op):
         if isinstance(p2, (float, int)):
             return APoint(op(p1[0], p2), op(p1[1], p2), op(p1[2], p2))
         return APoint(op(p1[0], p2[0]), op(p1[1], p2[1]), op(p1[2], p2[2]))
 
     def distance_to(self, other):
-        """
+        """Returns distance betwen two points 'p1' and 'p2'
 
         Parameters
         ----------
-        other :
-            
+        other : APoint, the point at which the distance is calculated
 
         Returns
         -------
 
         """
         return distance(self, other)
 
 
 def distance(p1, p2):
     """Returns distance between two points `p1` and `p2`
 
     Parameters
     ----------
-    p1 :
+    p1 : APoint
         
-    p2 :
+    p2 : APoint
         
 
     Returns
     -------
 
     """
     return ((p1.x - p2.x) ** 2 + (p1.y - p2.y) ** 2 + (p1.z - p2.z) ** 2) ** 0.5
```

### Comparing `pyacad-0.0.1/pyacad/Autocad.py` & `pyacad-0.0.2/pyacad/Autocad.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 import win32com.client
 # from pywintypes import com_error # Not in use.
 
 
 class Autocad:
     """Main class of AutoCAD app."""
 
-    def __init__(self):
+    def __init__(self, create_if_not_exist: bool = True, visible: bool = True):
         self._app = None
+        self._create_if_not_exist = create_if_not_exist
+        self._visible = True
 
     @property
     def app(self):
         """Creates/gets and returns AutoCAD Application."""
         try:
             self._app = win32com.client.GetActiveObject("AutoCAD.Application")
         except:
-            self._app = win32com.client.Dispatch("AutoCAD.Application")
+            if self._create_if_not_exist:
+                self._app = win32com.client.Dispatch("AutoCAD.Application")
+                self._app.Visible = self._visible
+            else:
+                return None
         return self._app
 
     @property
     def doc(self):
         """Returns active document."""
         return self.app.ActiveDocument
```

