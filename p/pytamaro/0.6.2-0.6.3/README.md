# Comparing `tmp/pytamaro-0.6.2.tar.gz` & `tmp/pytamaro-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytamaro-0.6.2.tar", max compression
+gzip compressed data, was "pytamaro-0.6.3.tar", max compression
```

## Comparing `pytamaro-0.6.2.tar` & `pytamaro-0.6.3.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     1103 2022-03-04 16:39:39.043278 pytamaro-0.6.2/LICENSE
--rw-r--r--   0        0        0     1870 2024-02-15 10:00:37.997986 pytamaro-0.6.2/README.md
--rw-r--r--   0        0        0      960 2024-02-15 10:15:51.666702 pytamaro-0.6.2/pyproject.toml
--rw-r--r--   0        0        0      472 2024-02-15 10:15:51.676503 pytamaro-0.6.2/pytamaro/__init__.py
--rw-r--r--   0        0        0     3850 2023-12-05 16:10:05.448171 pytamaro-0.6.2/pytamaro/checks.py
--rw-r--r--   0        0        0     1297 2023-11-20 08:55:51.374330 pytamaro-0.6.2/pytamaro/color.py
--rw-r--r--   0        0        0     4641 2023-02-27 12:54:43.438488 pytamaro-0.6.2/pytamaro/color_functions.py
--rw-r--r--   0        0        0     1010 2023-11-20 08:55:51.374788 pytamaro-0.6.2/pytamaro/color_names.py
--rw-r--r--   0        0        0      456 2023-02-27 12:54:43.439015 pytamaro-0.6.2/pytamaro/de/__init__.py
--rw-r--r--   0        0        0     3948 2023-02-27 12:54:43.439329 pytamaro-0.6.2/pytamaro/de/color.py
--rw-r--r--   0        0        0     1093 2023-11-06 13:08:00.795889 pytamaro-0.6.2/pytamaro/de/color_names.py
--rw-r--r--   0        0        0      445 2023-02-27 12:54:43.439701 pytamaro-0.6.2/pytamaro/de/graphic.py
--rw-r--r--   0        0        0     3211 2023-05-29 08:23:29.417046 pytamaro-0.6.2/pytamaro/de/io.py
--rw-r--r--   0        0        0     4206 2023-02-27 12:54:43.440314 pytamaro-0.6.2/pytamaro/de/operations.py
--rw-r--r--   0        0        0      119 2023-02-27 12:54:43.440547 pytamaro-0.6.2/pytamaro/de/point.py
--rw-r--r--   0        0        0     1364 2023-02-27 12:54:43.440806 pytamaro-0.6.2/pytamaro/de/point_names.py
--rw-r--r--   0        0        0     4626 2023-02-27 12:54:43.441003 pytamaro-0.6.2/pytamaro/de/primitives.py
--rw-r--r--   0        0        0     2643 2023-11-20 08:55:51.375234 pytamaro-0.6.2/pytamaro/debug.py
--rw-r--r--   0        0        0      456 2023-11-20 08:55:51.375364 pytamaro-0.6.2/pytamaro/fr/__init__.py
--rw-r--r--   0        0        0     3601 2023-11-20 08:55:51.375483 pytamaro-0.6.2/pytamaro/fr/color.py
--rw-r--r--   0        0        0      987 2023-11-20 08:55:51.375571 pytamaro-0.6.2/pytamaro/fr/color_names.py
--rw-r--r--   0        0        0      439 2023-11-20 08:55:51.375645 pytamaro-0.6.2/pytamaro/fr/graphic.py
--rw-r--r--   0        0        0     3378 2023-11-20 08:55:51.375738 pytamaro-0.6.2/pytamaro/fr/io.py
--rw-r--r--   0        0        0     4804 2023-11-20 08:55:51.375943 pytamaro-0.6.2/pytamaro/fr/operations.py
--rw-r--r--   0        0        0      113 2023-11-20 08:55:51.376011 pytamaro-0.6.2/pytamaro/fr/point.py
--rw-r--r--   0        0        0     1548 2023-11-20 08:55:51.376080 pytamaro-0.6.2/pytamaro/fr/point_names.py
--rw-r--r--   0        0        0     5014 2023-11-20 08:55:51.376201 pytamaro-0.6.2/pytamaro/fr/primitives.py
--rw-r--r--   0        0        0    14151 2024-02-15 09:42:31.139645 pytamaro-0.6.2/pytamaro/graphic.py
--rw-r--r--   0        0        0     9382 2023-12-05 16:10:05.448563 pytamaro-0.6.2/pytamaro/io.py
--rw-r--r--   0        0        0      457 2023-02-27 12:54:43.441979 pytamaro-0.6.2/pytamaro/it/__init__.py
--rw-r--r--   0        0        0     3370 2023-02-27 12:54:43.442282 pytamaro-0.6.2/pytamaro/it/color.py
--rw-r--r--   0        0        0      923 2022-11-30 08:45:09.899740 pytamaro-0.6.2/pytamaro/it/color_names.py
--rw-r--r--   0        0        0      459 2023-02-27 12:54:43.442558 pytamaro-0.6.2/pytamaro/it/graphic.py
--rw-r--r--   0        0        0     2949 2023-05-29 08:23:29.417817 pytamaro-0.6.2/pytamaro/it/io.py
--rw-r--r--   0        0        0     4512 2023-02-27 12:54:43.442887 pytamaro-0.6.2/pytamaro/it/operations.py
--rw-r--r--   0        0        0      111 2023-02-27 12:54:43.443014 pytamaro-0.6.2/pytamaro/it/point.py
--rw-r--r--   0        0        0     1626 2023-02-27 12:54:43.443240 pytamaro-0.6.2/pytamaro/it/point_names.py
--rw-r--r--   0        0        0     4636 2023-11-20 08:55:51.377302 pytamaro-0.6.2/pytamaro/it/primitives.py
--rw-r--r--   0        0        0    11360 2023-12-05 16:10:05.448746 pytamaro-0.6.2/pytamaro/localization.py
--rw-r--r--   0        0        0     4985 2023-11-20 08:55:51.377946 pytamaro-0.6.2/pytamaro/operations.py
--rw-r--r--   0        0        0     2298 2023-11-20 08:55:51.378301 pytamaro-0.6.2/pytamaro/point.py
--rw-r--r--   0        0        0     1527 2023-11-20 08:55:51.378550 pytamaro-0.6.2/pytamaro/point_names.py
--rw-r--r--   0        0        0     4997 2023-02-27 12:54:43.444392 pytamaro-0.6.2/pytamaro/primitives.py
--rw-r--r--   0        0        0        0 2022-10-31 08:45:16.764275 pytamaro-0.6.2/pytamaro/py.typed
--rw-r--r--   0        0        0     1032 2023-05-29 08:23:29.418250 pytamaro-0.6.2/pytamaro/utils.py
--rw-r--r--   0        0        0     2460 1970-01-01 00:00:00.000000 pytamaro-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1103 2022-03-04 16:39:39.043278 pytamaro-0.6.3/LICENSE
+-rw-r--r--   0        0        0     1870 2024-02-15 10:00:37.997986 pytamaro-0.6.3/README.md
+-rw-r--r--   0        0        0      960 2024-02-18 10:57:51.232981 pytamaro-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0      472 2024-02-18 10:57:51.244174 pytamaro-0.6.3/pytamaro/__init__.py
+-rw-r--r--   0        0        0     3850 2023-12-05 16:10:05.448171 pytamaro-0.6.3/pytamaro/checks.py
+-rw-r--r--   0        0        0     1297 2023-11-20 08:55:51.374330 pytamaro-0.6.3/pytamaro/color.py
+-rw-r--r--   0        0        0     4641 2023-02-27 12:54:43.438488 pytamaro-0.6.3/pytamaro/color_functions.py
+-rw-r--r--   0        0        0     1010 2023-11-20 08:55:51.374788 pytamaro-0.6.3/pytamaro/color_names.py
+-rw-r--r--   0        0        0      456 2023-02-27 12:54:43.439015 pytamaro-0.6.3/pytamaro/de/__init__.py
+-rw-r--r--   0        0        0     3948 2023-02-27 12:54:43.439329 pytamaro-0.6.3/pytamaro/de/color.py
+-rw-r--r--   0        0        0     1093 2023-11-06 13:08:00.795889 pytamaro-0.6.3/pytamaro/de/color_names.py
+-rw-r--r--   0        0        0      445 2023-02-27 12:54:43.439701 pytamaro-0.6.3/pytamaro/de/graphic.py
+-rw-r--r--   0        0        0     3211 2023-05-29 08:23:29.417046 pytamaro-0.6.3/pytamaro/de/io.py
+-rw-r--r--   0        0        0     4206 2023-02-27 12:54:43.440314 pytamaro-0.6.3/pytamaro/de/operations.py
+-rw-r--r--   0        0        0      119 2023-02-27 12:54:43.440547 pytamaro-0.6.3/pytamaro/de/point.py
+-rw-r--r--   0        0        0     1364 2023-02-27 12:54:43.440806 pytamaro-0.6.3/pytamaro/de/point_names.py
+-rw-r--r--   0        0        0     4626 2023-02-27 12:54:43.441003 pytamaro-0.6.3/pytamaro/de/primitives.py
+-rw-r--r--   0        0        0     2643 2023-11-20 08:55:51.375234 pytamaro-0.6.3/pytamaro/debug.py
+-rw-r--r--   0        0        0      456 2023-11-20 08:55:51.375364 pytamaro-0.6.3/pytamaro/fr/__init__.py
+-rw-r--r--   0        0        0     3601 2023-11-20 08:55:51.375483 pytamaro-0.6.3/pytamaro/fr/color.py
+-rw-r--r--   0        0        0      987 2023-11-20 08:55:51.375571 pytamaro-0.6.3/pytamaro/fr/color_names.py
+-rw-r--r--   0        0        0      439 2023-11-20 08:55:51.375645 pytamaro-0.6.3/pytamaro/fr/graphic.py
+-rw-r--r--   0        0        0     3378 2023-11-20 08:55:51.375738 pytamaro-0.6.3/pytamaro/fr/io.py
+-rw-r--r--   0        0        0     4804 2023-11-20 08:55:51.375943 pytamaro-0.6.3/pytamaro/fr/operations.py
+-rw-r--r--   0        0        0      113 2023-11-20 08:55:51.376011 pytamaro-0.6.3/pytamaro/fr/point.py
+-rw-r--r--   0        0        0     1548 2023-11-20 08:55:51.376080 pytamaro-0.6.3/pytamaro/fr/point_names.py
+-rw-r--r--   0        0        0     5014 2023-11-20 08:55:51.376201 pytamaro-0.6.3/pytamaro/fr/primitives.py
+-rw-r--r--   0        0        0    14151 2024-02-15 09:42:31.139645 pytamaro-0.6.3/pytamaro/graphic.py
+-rw-r--r--   0        0        0     9496 2024-02-18 10:23:36.614365 pytamaro-0.6.3/pytamaro/io.py
+-rw-r--r--   0        0        0      457 2023-02-27 12:54:43.441979 pytamaro-0.6.3/pytamaro/it/__init__.py
+-rw-r--r--   0        0        0     3370 2023-02-27 12:54:43.442282 pytamaro-0.6.3/pytamaro/it/color.py
+-rw-r--r--   0        0        0      923 2022-11-30 08:45:09.899740 pytamaro-0.6.3/pytamaro/it/color_names.py
+-rw-r--r--   0        0        0      459 2023-02-27 12:54:43.442558 pytamaro-0.6.3/pytamaro/it/graphic.py
+-rw-r--r--   0        0        0     2949 2023-05-29 08:23:29.417817 pytamaro-0.6.3/pytamaro/it/io.py
+-rw-r--r--   0        0        0     4512 2023-02-27 12:54:43.442887 pytamaro-0.6.3/pytamaro/it/operations.py
+-rw-r--r--   0        0        0      111 2023-02-27 12:54:43.443014 pytamaro-0.6.3/pytamaro/it/point.py
+-rw-r--r--   0        0        0     1626 2023-02-27 12:54:43.443240 pytamaro-0.6.3/pytamaro/it/point_names.py
+-rw-r--r--   0        0        0     4636 2023-11-20 08:55:51.377302 pytamaro-0.6.3/pytamaro/it/primitives.py
+-rw-r--r--   0        0        0    11698 2024-02-18 10:12:43.410558 pytamaro-0.6.3/pytamaro/localization.py
+-rw-r--r--   0        0        0     4985 2023-11-20 08:55:51.377946 pytamaro-0.6.3/pytamaro/operations.py
+-rw-r--r--   0        0        0     2303 2024-02-18 10:40:57.734102 pytamaro-0.6.3/pytamaro/point.py
+-rw-r--r--   0        0        0     1527 2023-11-20 08:55:51.378550 pytamaro-0.6.3/pytamaro/point_names.py
+-rw-r--r--   0        0        0     4997 2023-02-27 12:54:43.444392 pytamaro-0.6.3/pytamaro/primitives.py
+-rw-r--r--   0        0        0        0 2022-10-31 08:45:16.764275 pytamaro-0.6.3/pytamaro/py.typed
+-rw-r--r--   0        0        0     1032 2023-05-29 08:23:29.418250 pytamaro-0.6.3/pytamaro/utils.py
+-rw-r--r--   0        0        0     2460 1970-01-01 00:00:00.000000 pytamaro-0.6.3/PKG-INFO
```

### Comparing `pytamaro-0.6.2/LICENSE` & `pytamaro-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pytamaro-0.6.2/README.md` & `pytamaro-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `pytamaro-0.6.2/pyproject.toml` & `pytamaro-0.6.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytamaro"
-version = "0.6.2"
+version = "0.6.3"
 description = "Educational library for Python to teach programming using graphics"
 authors = ["Luca Chiodini <luca@chiodini.org>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 Pillow = "^10.2.0"
```

### Comparing `pytamaro-0.6.2/pytamaro/checks.py` & `pytamaro-0.6.3/pytamaro/checks.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.6.2/pytamaro/color.py` & `pytamaro-0.6.3/pytamaro/color.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.6.2/pytamaro/color_functions.py` & `pytamaro-0.6.3/pytamaro/color_functions.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.6.2/pytamaro/color_names.py` & `pytamaro-0.6.3/pytamaro/color_names.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.6.2/pytamaro/de/color.py` & `pytamaro-0.6.3/pytamaro/de/color.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.6.2/pytamaro/de/color_names.py` & `pytamaro-0.6.3/pytamaro/de/color_names.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.6.2/pytamaro/de/io.py` & `pytamaro-0.6.3/pytamaro/de/io.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.6.2/pytamaro/de/operations.py` & `pytamaro-0.6.3/pytamaro/de/operations.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.6.2/pytamaro/de/point_names.py` & `pytamaro-0.6.3/pytamaro/de/point_names.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.6.2/pytamaro/de/primitives.py` & `pytamaro-0.6.3/pytamaro/de/primitives.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.6.2/pytamaro/debug.py` & `pytamaro-0.6.3/pytamaro/debug.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.6.2/pytamaro/fr/color.py` & `pytamaro-0.6.3/pytamaro/fr/color.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.6.2/pytamaro/fr/color_names.py` & `pytamaro-0.6.3/pytamaro/fr/color_names.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.6.2/pytamaro/fr/io.py` & `pytamaro-0.6.3/pytamaro/fr/io.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.6.2/pytamaro/fr/operations.py` & `pytamaro-0.6.3/pytamaro/fr/operations.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.6.2/pytamaro/fr/point_names.py` & `pytamaro-0.6.3/pytamaro/fr/point_names.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.6.2/pytamaro/fr/primitives.py` & `pytamaro-0.6.3/pytamaro/fr/primitives.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.6.2/pytamaro/graphic.py` & `pytamaro-0.6.3/pytamaro/graphic.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.6.2/pytamaro/io.py` & `pytamaro-0.6.3/pytamaro/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 def graphic_to_image(graphic: Graphic) -> Image:
     """
     Renders a graphic into a Skia image.
 
     :param graphic: graphic to be rendered
     :returns: rendered graphic as a Skia image
     """
-    int_size = graphic.size().toCeil()
+    int_size = graphic.size().toRound()
     surface = Surface(int_size.width(), int_size.height())
     _draw_to_canvas(surface.getCanvas(), graphic)
     return surface.makeImageSnapshot()
 
 
 def graphic_to_pillow_image(graphic: Graphic) -> PILImage:
     """
@@ -212,14 +212,16 @@
     check_type(filename, str, "filename")
     if Path(filename).suffix != ".gif":
         raise ValueError(translate("INVALID_FILENAME_GIF"))
     check_type(graphics, list, "graphics")
     if len(graphics) == 0:
         raise ValueError(translate("EMPTY_GRAPHICS_LIST"))
     pil_images = list(map(graphic_to_pillow_image, graphics))
+    if len(set(image.size for image in pil_images)) != 1:
+        raise ValueError(translate("DIFFERENT_SIZES"))
     pil_images[0].save(
         filename,
         save_all=True,
         append_images=pil_images[1:],
         duration=duration,
         loop=0 if loop else 1,  # loop 0 means "indefinitely", 1 means "once"
     )
```

### Comparing `pytamaro-0.6.2/pytamaro/it/color.py` & `pytamaro-0.6.3/pytamaro/it/color.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.6.2/pytamaro/it/color_names.py` & `pytamaro-0.6.3/pytamaro/it/color_names.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.6.2/pytamaro/it/io.py` & `pytamaro-0.6.3/pytamaro/it/io.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.6.2/pytamaro/it/operations.py` & `pytamaro-0.6.3/pytamaro/it/operations.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.6.2/pytamaro/it/point_names.py` & `pytamaro-0.6.3/pytamaro/it/point_names.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.6.2/pytamaro/it/primitives.py` & `pytamaro-0.6.3/pytamaro/it/primitives.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.6.2/pytamaro/localization.py` & `pytamaro-0.6.3/pytamaro/localization.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,20 @@
     },
     "FONT_NOT_FOUND": {
         "en": "Cannot find font '{}', another font used as fallback",
         "it": "Impossibile trovare il font '{}', un altro font è stato usato come alternativa",
         "de": "Schriftart '{}' nicht gefunden, eine andere Schriftart wird als Fallback verwendet",
         "fr": "Impossible de trouver la police '{}', une autre police est utilisée comme alternative",
     },
+    "DIFFERENT_SIZES": {
+        "en": "All graphics in the list must have the same size",
+        "it": "Tutte le grafiche nella lista devono avere le stesse dimensioni",
+        "de": "Alle Grafiken in der Liste müssen die gleiche Größe haben",
+        "fr": "Tous les graphiques dans la liste doivent avoir la même taille",
+    },
     # Function names
     "compose": {
         "en": "compose",
         "it": "componi",
         "de": "kombiniere",
         "fr": "compose",
     },
```

### Comparing `pytamaro-0.6.2/pytamaro/operations.py` & `pytamaro-0.6.3/pytamaro/operations.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.6.2/pytamaro/point.py` & `pytamaro-0.6.3/pytamaro/point.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
     def __repr__(self) -> str:
         from pytamaro.point_names import \
             _known_points  # pylint: disable=cyclic-import,import-outside-toplevel
         maybe_known_point = _known_points.get(self)
         if maybe_known_point:
             return translate(maybe_known_point)
-        return f"({self.x}, {self.y})"
+        return f"Point({self.x}, {self.y})"
 
 
 # Center of the 2-dimensional space
 zero = Point(0.0, 0.0)
 
 
 @dataclass(frozen=True)
```

### Comparing `pytamaro-0.6.2/pytamaro/point_names.py` & `pytamaro-0.6.3/pytamaro/point_names.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.6.2/pytamaro/primitives.py` & `pytamaro-0.6.3/pytamaro/primitives.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.6.2/pytamaro/utils.py` & `pytamaro-0.6.3/pytamaro/utils.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.6.2/PKG-INFO` & `pytamaro-0.6.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytamaro
-Version: 0.6.2
+Version: 0.6.3
 Summary: Educational library for Python to teach programming using graphics
 Author: Luca Chiodini
 Author-email: luca@chiodini.org
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytamaro Version: 0.6.2 Summary: Educational
+Metadata-Version: 2.1 Name: pytamaro Version: 0.6.3 Summary: Educational
 library for Python to teach programming using graphics Author: Luca Chiodini
 Author-email: luca@chiodini.org Requires-Python: >=3.9,<4.0 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Requires-Dist: Pillow (>=10.2.0,<11.0.0) Requires-Dist: skia-
 python (>=121.0b6,<122.0) Description-Content-Type: text/markdown ![PyTamaro
```

