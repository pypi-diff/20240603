# Comparing `tmp/subdivision_hole_filler-1.0.2.tar.gz` & `tmp/subdivision_hole_filler-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subdivision_hole_filler-1.0.2.tar", last modified: Sun May 12 11:37:28 2024, max compression
+gzip compressed data, was "subdivision_hole_filler-1.0.3.tar", last modified: Mon Jun  3 06:52:37 2024, max compression
```

## Comparing `subdivision_hole_filler-1.0.2.tar` & `subdivision_hole_filler-1.0.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:37:28.427783 subdivision_hole_filler-1.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:37:28.419783 subdivision_hole_filler-1.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:37:28.423783 subdivision_hole_filler-1.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-12 11:37:23.000000 subdivision_hole_filler-1.0.2/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-12 11:37:23.000000 subdivision_hole_filler-1.0.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-05-12 11:37:23.000000 subdivision_hole_filler-1.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-12 11:37:23.000000 subdivision_hole_filler-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)   200849 2024-05-12 11:37:23.000000 subdivision_hole_filler-1.0.2/Levin_2000_Filling N-sided Holes Using Combined Subdivision Schemes.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-05-12 11:37:28.427783 subdivision_hole_filler-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-05-12 11:37:23.000000 subdivision_hole_filler-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   106308 2024-05-12 11:37:23.000000 subdivision_hole_filler-1.0.2/iso.png
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-12 11:37:23.000000 subdivision_hole_filler-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 11:37:28.427783 subdivision_hole_filler-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    52038 2024-05-12 11:37:23.000000 subdivision_hole_filler-1.0.2/side.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:37:28.419783 subdivision_hole_filler-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:37:28.423783 subdivision_hole_filler-1.0.2/src/subdivision_hole_filler/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-12 11:37:23.000000 subdivision_hole_filler-1.0.2/src/subdivision_hole_filler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-12 11:37:28.000000 subdivision_hole_filler-1.0.2/src/subdivision_hole_filler/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    12292 2024-05-12 11:37:23.000000 subdivision_hole_filler-1.0.2/src/subdivision_hole_filler/hole_filler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:37:28.423783 subdivision_hole_filler-1.0.2/src/subdivision_hole_filler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-05-12 11:37:28.000000 subdivision_hole_filler-1.0.2/src/subdivision_hole_filler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-12 11:37:28.000000 subdivision_hole_filler-1.0.2/src/subdivision_hole_filler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 11:37:28.000000 subdivision_hole_filler-1.0.2/src/subdivision_hole_filler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-12 11:37:28.000000 subdivision_hole_filler-1.0.2/src/subdivision_hole_filler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-12 11:37:28.000000 subdivision_hole_filler-1.0.2/src/subdivision_hole_filler.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:37:28.423783 subdivision_hole_filler-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-12 11:37:23.000000 subdivision_hole_filler-1.0.2/tests/test_6sided_hole.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:52:37.511645 subdivision_hole_filler-1.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:52:37.503645 subdivision_hole_filler-1.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:52:37.507645 subdivision_hole_filler-1.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-06-03 06:52:29.000000 subdivision_hole_filler-1.0.3/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-06-03 06:52:29.000000 subdivision_hole_filler-1.0.3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-06-03 06:52:29.000000 subdivision_hole_filler-1.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-06-03 06:52:29.000000 subdivision_hole_filler-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)   200849 2024-06-03 06:52:29.000000 subdivision_hole_filler-1.0.3/Levin_2000_Filling N-sided Holes Using Combined Subdivision Schemes.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-06-03 06:52:37.511645 subdivision_hole_filler-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-06-03 06:52:29.000000 subdivision_hole_filler-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   106308 2024-06-03 06:52:29.000000 subdivision_hole_filler-1.0.3/iso.png
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-06-03 06:52:29.000000 subdivision_hole_filler-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 06:52:37.511645 subdivision_hole_filler-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    52038 2024-06-03 06:52:29.000000 subdivision_hole_filler-1.0.3/side.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:52:37.507645 subdivision_hole_filler-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:52:37.507645 subdivision_hole_filler-1.0.3/src/subdivision_hole_filler/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-06-03 06:52:29.000000 subdivision_hole_filler-1.0.3/src/subdivision_hole_filler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-06-03 06:52:37.000000 subdivision_hole_filler-1.0.3/src/subdivision_hole_filler/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12850 2024-06-03 06:52:29.000000 subdivision_hole_filler-1.0.3/src/subdivision_hole_filler/hole_filler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:52:37.511645 subdivision_hole_filler-1.0.3/src/subdivision_hole_filler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-06-03 06:52:37.000000 subdivision_hole_filler-1.0.3/src/subdivision_hole_filler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-06-03 06:52:37.000000 subdivision_hole_filler-1.0.3/src/subdivision_hole_filler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 06:52:37.000000 subdivision_hole_filler-1.0.3/src/subdivision_hole_filler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-06-03 06:52:37.000000 subdivision_hole_filler-1.0.3/src/subdivision_hole_filler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-06-03 06:52:37.000000 subdivision_hole_filler-1.0.3/src/subdivision_hole_filler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:52:37.511645 subdivision_hole_filler-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-06-03 06:52:29.000000 subdivision_hole_filler-1.0.3/tests/test_6sided_hole.py
```

### Comparing `subdivision_hole_filler-1.0.2/.github/workflows/python-package.yml` & `subdivision_hole_filler-1.0.3/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `subdivision_hole_filler-1.0.2/.github/workflows/python-publish.yml` & `subdivision_hole_filler-1.0.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `subdivision_hole_filler-1.0.2/.gitignore` & `subdivision_hole_filler-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `subdivision_hole_filler-1.0.2/LICENSE` & `subdivision_hole_filler-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `subdivision_hole_filler-1.0.2/Levin_2000_Filling N-sided Holes Using Combined Subdivision Schemes.pdf` & `subdivision_hole_filler-1.0.3/Levin_2000_Filling N-sided Holes Using Combined Subdivision Schemes.pdf`

 * *Files identical despite different names*

### Comparing `subdivision_hole_filler-1.0.2/PKG-INFO` & `subdivision_hole_filler-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: subdivision-hole-filler
-Version: 1.0.2
+Version: 1.0.3
 Summary: A python package to fill N-sided holes using combined subdivision schemes, based on Catmull-Clark subdivison.
 Author-email: HUANG Lihao <huang-lihao@outlook.com>
 Project-URL: Homepage, https://github.com/huang-lihao/subdivision-hole-filler
 Project-URL: Bug Tracker, https://github.com/huang-lihao/subdivision-hole-filler/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `subdivision_hole_filler-1.0.2/README.md` & `subdivision_hole_filler-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `subdivision_hole_filler-1.0.2/iso.png` & `subdivision_hole_filler-1.0.3/iso.png`

 * *Files identical despite different names*

### Comparing `subdivision_hole_filler-1.0.2/pyproject.toml` & `subdivision_hole_filler-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `subdivision_hole_filler-1.0.2/side.png` & `subdivision_hole_filler-1.0.3/side.png`

 * *Files identical despite different names*

### Comparing `subdivision_hole_filler-1.0.2/src/subdivision_hole_filler/hole_filler.py` & `subdivision_hole_filler-1.0.3/src/subdivision_hole_filler/hole_filler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,31 @@
 """
 
 See Levin 1999 paper: "Filling an N-sided hole using combined subdivision schemes
 """
 
 import matplotlib.pyplot as plt
 import numpy as np
+from scipy.interpolate import PPoly
+
+
+catmull_clark_coefs = {}
+
+def get_catmull_clark_coef(m):
+    if m in catmull_clark_coefs:
+        return catmull_clark_coefs[m]
+    k = np.cos(np.pi / m)
+    pp = PPoly(np.array([[1, 0, 4 * k ** 2 - 3, - 2 * k]]).T, [0, 10])
+    x = pp.roots()[0]
+    W = x ** 2 + 2 * k * x - 3
+    alpha = 1
+    gamma = (k * x + 2 * k ** 2 - 1)/(x**2*(k*x + 1))
+    beta = - gamma
+    catmull_clark_coefs[m] = (W, alpha, beta, gamma)
+    return catmull_clark_coefs[m]
 
 
 class Boundary:
     def __init__(self):
         pass
 
     def coord(self, u: float):
@@ -34,15 +51,15 @@
     def __init__(self, points: list[Point], sub_face: int) -> None:
         assert len(points) == 4
         self.points = points
         for i in range(4):
             points[i].faces.append(self)
             for d in [-1, +1]:
                 j = (i + d) % 4
-                if points[i] not in points[i].neighbours:
+                if points[j] not in points[i].neighbours:
                     points[i].neighbours.append(points[j])
         self.sub_face = sub_face
         
     
     def center_point(self) -> Point:
         point = Point(*np.mean([p.coord for p in self.points], axis=0))
         point.parametric_coord_in_sub_face[self.sub_face] = 0.25 * (
@@ -75,15 +92,15 @@
         for face in faces:
             coord = [pt.coord for pt in face.points]
             coord = np.array([[coord[0], coord[1]], [coord[3], coord[2]]])
             X = coord[:, :, 0]
             Y = coord[:, :, 1]
             Z = coord[:, :, 2]
             ax.plot_surface(X,Y,Z,color="none", edgecolor="black")
-        ax.scatter([self.center_point[0]], [self.center_point[1]], [self.center_point[2]])
+        ax.scatter([self.center_point.coord[0]], [self.center_point.coord[1]], [self.center_point.coord[2]])
         plt.axis('equal')
         ax.set_proj_type('ortho')
         ax.view_init(elev=np.arctan(np.sqrt(0.5))/np.pi*180, azim=45)
         ax.view_init(elev=0, azim=0)
         if output_path is not None:
             plt.tight_layout()
             plt.savefig(output_path)
@@ -261,17 +278,17 @@
                 [face_points[face].coord for face in point.faces],
                 axis=0
             )
             R = np.mean(
                 [1/2*(point.coord + q.coord) for q in point.neighbours],
                 axis=0
             )
-            n = max(len(point.neighbours), 4)
-            point.coord = (F + 2*R + (n - 3) * point.coord) / n
-                
+            m = max(len(point.neighbours), 4)
+            W, alpha, beta, gamma = get_catmull_clark_coef(m)
+            point.coord = alpha * R + beta * F + gamma * point.coord
 
         # Form faces in the new mesh
         self.clear_points(points)
         for face in faces:
             for i in range(4):
                 mid = []
                 for d in [-1, +1]:
```

### Comparing `subdivision_hole_filler-1.0.2/src/subdivision_hole_filler.egg-info/PKG-INFO` & `subdivision_hole_filler-1.0.3/src/subdivision_hole_filler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: subdivision-hole-filler
-Version: 1.0.2
+Version: 1.0.3
 Summary: A python package to fill N-sided holes using combined subdivision schemes, based on Catmull-Clark subdivison.
 Author-email: HUANG Lihao <huang-lihao@outlook.com>
 Project-URL: Homepage, https://github.com/huang-lihao/subdivision-hole-filler
 Project-URL: Bug Tracker, https://github.com/huang-lihao/subdivision-hole-filler/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `subdivision_hole_filler-1.0.2/src/subdivision_hole_filler.egg-info/SOURCES.txt` & `subdivision_hole_filler-1.0.3/src/subdivision_hole_filler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `subdivision_hole_filler-1.0.2/tests/test_6sided_hole.py` & `subdivision_hole_filler-1.0.3/tests/test_6sided_hole.py`

 * *Files identical despite different names*

