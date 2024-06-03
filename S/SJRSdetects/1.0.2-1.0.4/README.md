# Comparing `tmp/sjrsdetects-1.0.2.tar.gz` & `tmp/sjrsdetects-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sjrsdetects-1.0.2.tar", last modified: Sat Jun  1 15:32:50 2024, max compression
+gzip compressed data, was "sjrsdetects-1.0.4.tar", last modified: Mon Jun  3 03:48:20 2024, max compression
```

## Comparing `sjrsdetects-1.0.2.tar` & `sjrsdetects-1.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 15:32:50.168100 sjrsdetects-1.0.2/
--rw-rw-rw-   0        0        0      588 2024-06-01 15:32:50.165984 sjrsdetects-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       58 2024-05-27 08:29:42.000000 sjrsdetects-1.0.2/README.md
--rw-rw-rw-   0        0        0       42 2024-06-01 15:32:50.168100 sjrsdetects-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      860 2024-06-01 15:32:35.000000 sjrsdetects-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-06-01 15:32:50.078877 sjrsdetects-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2024-06-01 15:32:50.105556 sjrsdetects-1.0.2/src/SJRSdetects/
--rw-rw-rw-   0        0        0     1602 2024-05-27 09:36:31.000000 sjrsdetects-1.0.2/src/SJRSdetects/DetectaFormas.py
--rw-rw-rw-   0        0        0     2206 2024-06-01 14:30:15.000000 sjrsdetects-1.0.2/src/SJRSdetects/DetectaMovCamara.py
--rw-rw-rw-   0        0        0     2568 2024-05-27 09:28:51.000000 sjrsdetects-1.0.2/src/SJRSdetects/DetectaMovFotos.py
--rw-rw-rw-   0        0        0     3010 2024-05-27 09:31:31.000000 sjrsdetects-1.0.2/src/SJRSdetects/DetectaMovVideo.py
--rw-rw-rw-   0        0        0      180 2024-05-27 07:55:51.000000 sjrsdetects-1.0.2/src/SJRSdetects/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-01 15:32:50.163291 sjrsdetects-1.0.2/src/SJRSdetects.egg-info/
--rw-rw-rw-   0        0        0      588 2024-06-01 15:32:49.000000 sjrsdetects-1.0.2/src/SJRSdetects.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      341 2024-06-01 15:32:50.000000 sjrsdetects-1.0.2/src/SJRSdetects.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 15:32:49.000000 sjrsdetects-1.0.2/src/SJRSdetects.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-06-01 15:32:49.000000 sjrsdetects-1.0.2/src/SJRSdetects.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-03 03:48:20.329742 sjrsdetects-1.0.4/
+-rw-rw-rw-   0        0        0      588 2024-06-03 03:48:20.327234 sjrsdetects-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       58 2024-06-01 15:51:37.000000 sjrsdetects-1.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-06-03 03:48:20.329742 sjrsdetects-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      860 2024-06-01 15:52:31.000000 sjrsdetects-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 03:48:20.280024 sjrsdetects-1.0.4/src/
+drwxrwxrwx   0        0        0        0 2024-06-03 03:48:20.296455 sjrsdetects-1.0.4/src/SJRSdetects/
+-rw-rw-rw-   0        0        0     1602 2024-05-27 09:36:31.000000 sjrsdetects-1.0.4/src/SJRSdetects/DetectaFormas.py
+-rw-rw-rw-   0        0        0     2239 2024-06-01 15:48:21.000000 sjrsdetects-1.0.4/src/SJRSdetects/DetectaMovCamara.py
+-rw-rw-rw-   0        0        0     2568 2024-05-27 09:28:51.000000 sjrsdetects-1.0.4/src/SJRSdetects/DetectaMovFotos.py
+-rw-rw-rw-   0        0        0     3010 2024-05-27 09:31:31.000000 sjrsdetects-1.0.4/src/SJRSdetects/DetectaMovVideo.py
+-rw-rw-rw-   0        0        0      180 2024-05-27 07:55:51.000000 sjrsdetects-1.0.4/src/SJRSdetects/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 03:48:20.325459 sjrsdetects-1.0.4/src/SJRSdetects.egg-info/
+-rw-rw-rw-   0        0        0      588 2024-06-03 03:48:20.000000 sjrsdetects-1.0.4/src/SJRSdetects.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      341 2024-06-03 03:48:20.000000 sjrsdetects-1.0.4/src/SJRSdetects.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 03:48:20.000000 sjrsdetects-1.0.4/src/SJRSdetects.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-06-03 03:48:20.000000 sjrsdetects-1.0.4/src/SJRSdetects.egg-info/top_level.txt
```

### Comparing `sjrsdetects-1.0.2/PKG-INFO` & `sjrsdetects-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SJRSdetects
-Version: 1.0.2
+Version: 1.0.4
 Summary: Detecta movimiento en fotos, video y camara
 Home-page: https://github.com/Stevenjoelrs/SJRSdetects
 Author: Stevenjoelrs
 Author-email: Stevenjramossalazar@gmail.com
 Project-URL: Bug Tracker, https://github.com/Stevenjoelrs/SJRSdetect/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sjrsdetects-1.0.2/setup.py` & `sjrsdetects-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="SJRSdetects",
-    version="1.0.2",
+    version="1.0.4",
     author="Stevenjoelrs",
     author_email="Stevenjramossalazar@gmail.com",
     description="Detecta movimiento en fotos, video y camara",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Stevenjoelrs/SJRSdetects",
     project_urls={
```

### Comparing `sjrsdetects-1.0.2/src/SJRSdetects/DetectaFormas.py` & `sjrsdetects-1.0.4/src/SJRSdetects/DetectaFormas.py`

 * *Files identical despite different names*

### Comparing `sjrsdetects-1.0.2/src/SJRSdetects/DetectaMovCamara.py` & `sjrsdetects-1.0.4/src/SJRSdetects/DetectaMovCamara.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import numpy as np
 
 class DetectaMovCamara:
     def __init__(self):
         self.prevFrame = None
         self.prevCenter = None
 
-    def detectarMovimiento(self):
+    def detectarMovimiento(self, resultados):
         # Abrir la cámara
         capture = cv2.VideoCapture(0)
         if not capture.isOpened():
             print("No se pudo abrir la cámara")
             return
 
         while True:
@@ -45,18 +45,19 @@
                 if abs(dx) > 2 and abs(dy) > 2:
                     direction = "movimiento en diagonal hacia " + ("abajo y a la derecha" if dx > 0 and dy > 0 else "arriba y a la derecha" if dx > 0 else "abajo y a la izquierda" if dy > 0 else "arriba y a la izquierda")
                 elif abs(dx) > 2:
                     direction = "movimiento hacia la " + ("derecha" if dx > 0 else "izquierda")
                 elif abs(dy) > 2:
                     direction = "movimiento hacia " + ("abajo" if dy > 0 else "arriba")
 
-                print(direction)
+                resultados.set(direction)
+
                 self.prevCenter = center
 
             self.prevFrame = gray
         capture.release()
         return direction
     
     
     def mostrarCamara(self):
-        print ("Mostrando camara")
+        print ("Se esta mostrado la camara")
         #cv2.destroyAllWindows()
```

### Comparing `sjrsdetects-1.0.2/src/SJRSdetects/DetectaMovFotos.py` & `sjrsdetects-1.0.4/src/SJRSdetects/DetectaMovFotos.py`

 * *Files identical despite different names*

### Comparing `sjrsdetects-1.0.2/src/SJRSdetects/DetectaMovVideo.py` & `sjrsdetects-1.0.4/src/SJRSdetects/DetectaMovVideo.py`

 * *Files identical despite different names*

### Comparing `sjrsdetects-1.0.2/src/SJRSdetects.egg-info/PKG-INFO` & `sjrsdetects-1.0.4/src/SJRSdetects.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SJRSdetects
-Version: 1.0.2
+Version: 1.0.4
 Summary: Detecta movimiento en fotos, video y camara
 Home-page: https://github.com/Stevenjoelrs/SJRSdetects
 Author: Stevenjoelrs
 Author-email: Stevenjramossalazar@gmail.com
 Project-URL: Bug Tracker, https://github.com/Stevenjoelrs/SJRSdetect/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

