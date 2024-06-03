# Comparing `tmp/osvg-1.1.1.tar.gz` & `tmp/osvg-1.1.2.tar.gz`

## Comparing `osvg-1.1.1.tar` & `osvg-1.1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 osvg-1.1.1/osvg/__init__.py
--rw-r--r--   0        0        0     7043 2020-02-02 00:00:00.000000 osvg-1.1.1/osvg/float.py
--rw-r--r--   0        0        0     5929 2020-02-02 00:00:00.000000 osvg-1.1.1/osvg/float_math.py
--rw-r--r--   0        0        0     5622 2020-02-02 00:00:00.000000 osvg-1.1.1/osvg/helper.py
--rw-r--r--   0        0        0    10569 2020-02-02 00:00:00.000000 osvg-1.1.1/osvg/positions.py
--rw-r--r--   0        0        0    11969 2020-02-02 00:00:00.000000 osvg-1.1.1/osvg/style.py
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 osvg-1.1.1/osvg/elements/circle.py
--rw-r--r--   0        0        0     2650 2020-02-02 00:00:00.000000 osvg-1.1.1/osvg/elements/circlebase.py
--rw-r--r--   0        0        0     8828 2020-02-02 00:00:00.000000 osvg-1.1.1/osvg/elements/elementbase.py
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 osvg-1.1.1/osvg/elements/ellipse.py
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 osvg-1.1.1/osvg/elements/group.py
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 osvg-1.1.1/osvg/elements/line.py
--rw-r--r--   0        0        0    10476 2020-02-02 00:00:00.000000 osvg-1.1.1/osvg/elements/line_marker.py
--rw-r--r--   0        0        0    11539 2020-02-02 00:00:00.000000 osvg-1.1.1/osvg/elements/path.py
--rw-r--r--   0        0        0     3945 2020-02-02 00:00:00.000000 osvg-1.1.1/osvg/elements/polyline.py
--rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 osvg-1.1.1/osvg/elements/rectangle.py
--rw-r--r--   0        0        0     7633 2020-02-02 00:00:00.000000 osvg-1.1.1/osvg/elements/rectanglebase.py
--rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 osvg-1.1.1/osvg/elements/svg.py
--rw-r--r--   0        0        0     8312 2020-02-02 00:00:00.000000 osvg-1.1.1/osvg/elements/text.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 osvg-1.1.1/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 osvg-1.1.1/LICENSE
--rw-r--r--   0        0        0     5052 2020-02-02 00:00:00.000000 osvg-1.1.1/README.md
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 osvg-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     5842 2020-02-02 00:00:00.000000 osvg-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 osvg-1.1.2/osvg/__init__.py
+-rw-r--r--   0        0        0     7043 2020-02-02 00:00:00.000000 osvg-1.1.2/osvg/float.py
+-rw-r--r--   0        0        0     5929 2020-02-02 00:00:00.000000 osvg-1.1.2/osvg/float_math.py
+-rw-r--r--   0        0        0     5622 2020-02-02 00:00:00.000000 osvg-1.1.2/osvg/helper.py
+-rw-r--r--   0        0        0    10569 2020-02-02 00:00:00.000000 osvg-1.1.2/osvg/positions.py
+-rw-r--r--   0        0        0    11969 2020-02-02 00:00:00.000000 osvg-1.1.2/osvg/style.py
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 osvg-1.1.2/osvg/elements/circle.py
+-rw-r--r--   0        0        0     2650 2020-02-02 00:00:00.000000 osvg-1.1.2/osvg/elements/circlebase.py
+-rw-r--r--   0        0        0     8828 2020-02-02 00:00:00.000000 osvg-1.1.2/osvg/elements/elementbase.py
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 osvg-1.1.2/osvg/elements/ellipse.py
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 osvg-1.1.2/osvg/elements/group.py
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 osvg-1.1.2/osvg/elements/line.py
+-rw-r--r--   0        0        0    10476 2020-02-02 00:00:00.000000 osvg-1.1.2/osvg/elements/line_marker.py
+-rw-r--r--   0        0        0    12107 2020-02-02 00:00:00.000000 osvg-1.1.2/osvg/elements/path.py
+-rw-r--r--   0        0        0     3945 2020-02-02 00:00:00.000000 osvg-1.1.2/osvg/elements/polyline.py
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 osvg-1.1.2/osvg/elements/rectangle.py
+-rw-r--r--   0        0        0     7633 2020-02-02 00:00:00.000000 osvg-1.1.2/osvg/elements/rectanglebase.py
+-rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 osvg-1.1.2/osvg/elements/svg.py
+-rw-r--r--   0        0        0     8312 2020-02-02 00:00:00.000000 osvg-1.1.2/osvg/elements/text.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 osvg-1.1.2/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 osvg-1.1.2/LICENSE
+-rw-r--r--   0        0        0     5052 2020-02-02 00:00:00.000000 osvg-1.1.2/README.md
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 osvg-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     5842 2020-02-02 00:00:00.000000 osvg-1.1.2/PKG-INFO
```

### Comparing `osvg-1.1.1/osvg/float.py` & `osvg-1.1.2/osvg/float.py`

 * *Files identical despite different names*

### Comparing `osvg-1.1.1/osvg/float_math.py` & `osvg-1.1.2/osvg/float_math.py`

 * *Files identical despite different names*

### Comparing `osvg-1.1.1/osvg/helper.py` & `osvg-1.1.2/osvg/helper.py`

 * *Files identical despite different names*

### Comparing `osvg-1.1.1/osvg/positions.py` & `osvg-1.1.2/osvg/positions.py`

 * *Files identical despite different names*

### Comparing `osvg-1.1.1/osvg/style.py` & `osvg-1.1.2/osvg/style.py`

 * *Files identical despite different names*

### Comparing `osvg-1.1.1/osvg/elements/circle.py` & `osvg-1.1.2/osvg/elements/circle.py`

 * *Files identical despite different names*

### Comparing `osvg-1.1.1/osvg/elements/circlebase.py` & `osvg-1.1.2/osvg/elements/circlebase.py`

 * *Files identical despite different names*

### Comparing `osvg-1.1.1/osvg/elements/elementbase.py` & `osvg-1.1.2/osvg/elements/elementbase.py`

 * *Files identical despite different names*

### Comparing `osvg-1.1.1/osvg/elements/ellipse.py` & `osvg-1.1.2/osvg/elements/ellipse.py`

 * *Files identical despite different names*

### Comparing `osvg-1.1.1/osvg/elements/group.py` & `osvg-1.1.2/osvg/elements/group.py`

 * *Files identical despite different names*

### Comparing `osvg-1.1.1/osvg/elements/line.py` & `osvg-1.1.2/osvg/elements/line.py`

 * *Files identical despite different names*

### Comparing `osvg-1.1.1/osvg/elements/line_marker.py` & `osvg-1.1.2/osvg/elements/line_marker.py`

 * *Files identical despite different names*

### Comparing `osvg-1.1.1/osvg/elements/path.py` & `osvg-1.1.2/osvg/elements/path.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,26 +16,27 @@
 class _PathElement:
     """
     Base class for all Path elements
     """
 
     tag = ""
     needs_previous_path_element = False
-    previous_path_element_classes = ()
+    previous_path_element_sub_classes = []
 
     def verify_previous_path_element(self, element: "_PathElement") -> None:
         """
         Checks if given (previous) path element if the one which is needed
         """
-        if not isinstance(element, self.previous_path_element_classes):
+        if not issubclass(type(element), tuple(self.previous_path_element_sub_classes)):
             class_names = " or ".join(
-                [x.__name__ for x in self.previous_path_element_classes]
+                [x.__name__ for x in self.previous_path_element_sub_classes]
             )
             raise RuntimeError(
-                f"{self.__class__.__name__} need class {class_names} as previous path element"
+                f"{self.__class__.__name__} need sub-class of "
+                + f"{class_names} as previous path element"
             )
 
 
 class _SingleFloatElement(_PathElement):
     """
     Base class for Path elements which uses a position
     """
@@ -242,139 +243,151 @@
 
     tag = "v"
 
     def __init__(self, y: int | float | osvg.float.Float) -> None:
         super().__init__(ref=y)
 
 
-class PathZ:
+class PathZ(_PathElement):
     """
     Class for the final 'Z' element which closes the path to
     the starting position
     """
 
     def __str__(self):
         return "Z"
 
 
-class PathC(_ThreeAbsolutePositionElement):
+class CubicBezierCurveElement:
+    """
+    Meta class to to verify previous path element
+    """
+
+
+class PathC(_ThreeAbsolutePositionElement, CubicBezierCurveElement):
     """
     Class to draw a cubic Bézier curve by using three position objects:
     - postion1: Bézier Point 1
     - postion2: Bézier Point 2
     - postion3: Final Point
     """
 
     tag = "C"
 
 
-class Pathc(_ThreeRelativePositionElement):
+class Pathc(_ThreeRelativePositionElement, CubicBezierCurveElement):
     """
     Class to draw a cubic Bézier curve by using three relative positions:
     - x1: x Float value of Bézier Point 1
     - y1: y Float value of Bézier Point 1
     - x2: x Float value of Bézier Point 2
     - y2: y Float value of Bézier Point 2
     - x3: x Float value of Final Point
     - y3: y Float value of Final Point
     """
 
     tag = "c"
 
 
-class PathS(_TwoAbsolutePositionElement):
+class PathS(_TwoAbsolutePositionElement, CubicBezierCurveElement):
     """
     Class to draw a follow-up cubic Bézier curve by using two position objects:
     - postion1: Bézier Point 2
     - postion2: Final Point
     Note: Bézier Point 1 is a reflection of Bézier Point 2 of previous
     cubic Bézier Curve.
     """
 
     tag = "S"
     needs_previous_path_element = True
-    previous_path_element_classes = (PathC, Pathc)
+    previous_path_element_sub_classes = [CubicBezierCurveElement]
 
 
-class Paths(_TwoRelativePositionElement):
+class Paths(_TwoRelativePositionElement, CubicBezierCurveElement):
     """
     Class to draw a follow-up cubic Bézier curve by using two relative positions:
     - x1: x Float value of Bézier Point 2
     - y1: y Float value of Bézier Point 2
     - x2: x Float value of Final Point
     - y2: y Float value of Final Point
     Note: Bézier Point 1 is a reflection of Bézier Point 2 of previous
     cubic Bézier Curve.
     """
 
     tag = "s"
     needs_previous_path_element = True
-    previous_path_element_classes = (PathC, Pathc)
+    previous_path_element_sub_classes = [CubicBezierCurveElement]
+
+
+class QuadraticBezierCurveElement:
+    """
+    Meta class to to verify previous path element
+    """
 
 
-class PathQ(_TwoAbsolutePositionElement):
+class PathQ(_TwoAbsolutePositionElement, QuadraticBezierCurveElement):
     """
     Class to draw a quadratic Bézier curve by using two position objects:
     - postion1: Bézier Point
     - postion2: Final Point
     """
 
     tag = "Q"
 
 
-class Pathq(_TwoRelativePositionElement):
+class Pathq(_TwoRelativePositionElement, QuadraticBezierCurveElement):
     """
     Class to draw a quadratic Bézier curve by using two relative positions:
     - x1: x Float value of Bézier Point
     - y1: y Float value of Bézier Point
     - x2: x Float value of Final Point
     - y2: y Float value of Final Point
     """
 
     tag = "q"
 
 
-class PathT(_AbsolutePositionElement):
+class PathT(_AbsolutePositionElement, QuadraticBezierCurveElement):
     """
     Class to draw a follow-up quadratic Bézier curve by using a position object:
     - postion: Final Point
     Note: Bézier Point is a reflection of Bezier Point of previous
     quadratic Bézier Curve.
     """
 
     tag = "T"
     needs_previous_path_element = True
-    previous_path_element_classes = (PathQ, Pathq)
+    previous_path_element_sub_classes = [QuadraticBezierCurveElement]
 
 
-class Patht(_RelativePositionElement):
+class Patht(_RelativePositionElement, QuadraticBezierCurveElement):
     """
     Class to draw a follow-up quadratic Bézier curve by using a relative position:
     - x: x Float value of Final Point
     - y: y Float value of Final Point
     Note: Bézier Point is a reflection of Bezier Point of previous
     quadratic Bézier Curve.
     """
 
     tag = "t"
     needs_previous_path_element = True
-    previous_path_element_classes = (PathQ, Pathq)
+    previous_path_element_sub_classes = [QuadraticBezierCurveElement]
 
 
 class PathAParams(TypedDict):
     """
     Optional parameter definition for class PathA
     """
 
     angle: int | float | osvg.float.Float = (0,)
     long_bow: bool = (True,)
     right_bend: bool = (True,)
 
 
-class PathA:
+class PathA(_PathElement):
     """
     Class to draw a elliptic arc bow:
     - position: Final position of the arc curve
     - width: Width of the ellipse
     - height: Height of the ellipse
     - angle: Angled orientation of the ellipse
     - long_bow: Indicator if long bow should be drawn
```

### Comparing `osvg-1.1.1/osvg/elements/polyline.py` & `osvg-1.1.2/osvg/elements/polyline.py`

 * *Files identical despite different names*

### Comparing `osvg-1.1.1/osvg/elements/rectangle.py` & `osvg-1.1.2/osvg/elements/rectangle.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,13 +66,13 @@
 
     Parameter:
       percentage: Percent of the lower value of width or height.
     """
 
     percentage = osvg.float.FloatProperty()
 
-    def __init__(self, **kwargs: Unpack[RectangleParams]) -> None:
+    def __init__(self, **kwargs: Unpack[SCRectangleParams]) -> None:
         super().__init__(**kwargs)
         self.percentage = kwargs.get("percentage", 5)
         self.rx = osvg.float_math.PercentOf(
             osvg.float_math.Min(self.width, self.height), self.percentage
         )
```

### Comparing `osvg-1.1.1/osvg/elements/rectanglebase.py` & `osvg-1.1.2/osvg/elements/rectanglebase.py`

 * *Files identical despite different names*

### Comparing `osvg-1.1.1/osvg/elements/svg.py` & `osvg-1.1.2/osvg/elements/svg.py`

 * *Files identical despite different names*

### Comparing `osvg-1.1.1/osvg/elements/text.py` & `osvg-1.1.2/osvg/elements/text.py`

 * *Files identical despite different names*

### Comparing `osvg-1.1.1/LICENSE` & `osvg-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `osvg-1.1.1/README.md` & `osvg-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `osvg-1.1.1/pyproject.toml` & `osvg-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.hatch.build]
 include = [
   "/osvg",
 ]
 
 [project]
 name = "osvg"
-version = "1.1.1"
+version = "1.1.2"
 authors = [
   { name="Korte Noack", email="korte@8lacht.de" },
 ]
 description = "osvg is a python API to create SVG XML code with object-oriented elements"
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
```

### Comparing `osvg-1.1.1/PKG-INFO` & `osvg-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: osvg
-Version: 1.1.1
+Version: 1.1.2
 Summary: osvg is a python API to create SVG XML code with object-oriented elements
 Project-URL: Homepage, https://gitlab.com/ko.no/osvg
 Project-URL: Bug Tracker, https://gitlab.com/ko.no/osvg/-/issues
 Author-email: Korte Noack <korte@8lacht.de>
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

