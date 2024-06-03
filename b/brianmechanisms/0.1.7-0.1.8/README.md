# Comparing `tmp/brianmechanisms-0.1.7.tar.gz` & `tmp/brianmechanisms-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brianmechanisms-0.1.7.tar", last modified: Fri May 31 10:21:03 2024, max compression
+gzip compressed data, was "brianmechanisms-0.1.8.tar", last modified: Mon Jun  3 04:46:33 2024, max compression
```

## Comparing `brianmechanisms-0.1.7.tar` & `brianmechanisms-0.1.8.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:21:03.759320 brianmechanisms-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)    10761 2024-05-31 10:20:53.000000 brianmechanisms-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6631 2024-05-31 10:21:03.759320 brianmechanisms-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5925 2024-05-31 10:20:53.000000 brianmechanisms-0.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-31 10:20:53.000000 brianmechanisms-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 10:21:03.759320 brianmechanisms-0.1.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:21:03.755320 brianmechanisms-0.1.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:21:03.755320 brianmechanisms-0.1.7/src/brianmechanisms/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-31 10:20:53.000000 brianmechanisms-0.1.7/src/brianmechanisms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23980 2024-05-31 10:20:53.000000 brianmechanisms-0.1.7/src/brianmechanisms/appproximateStraightLineMechanisms.py
--rw-r--r--   0 runner    (1001) docker     (127)    14454 2024-05-31 10:20:53.000000 brianmechanisms-0.1.7/src/brianmechanisms/locii.py
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-31 10:20:53.000000 brianmechanisms-0.1.7/src/brianmechanisms/mirror.py
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-31 10:20:53.000000 brianmechanisms-0.1.7/src/brianmechanisms/straightLineMechanisms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:21:03.759320 brianmechanisms-0.1.7/src/brianmechanisms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6631 2024-05-31 10:21:03.000000 brianmechanisms-0.1.7/src/brianmechanisms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-31 10:21:03.000000 brianmechanisms-0.1.7/src/brianmechanisms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 10:21:03.000000 brianmechanisms-0.1.7/src/brianmechanisms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-31 10:21:03.000000 brianmechanisms-0.1.7/src/brianmechanisms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-31 10:21:03.000000 brianmechanisms-0.1.7/src/brianmechanisms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 04:46:33.666528 brianmechanisms-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    10761 2024-06-03 04:46:19.000000 brianmechanisms-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6631 2024-06-03 04:46:33.662528 brianmechanisms-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5925 2024-06-03 04:46:19.000000 brianmechanisms-0.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-06-03 04:46:19.000000 brianmechanisms-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 04:46:33.666528 brianmechanisms-0.1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 04:46:33.662528 brianmechanisms-0.1.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 04:46:33.662528 brianmechanisms-0.1.8/src/brianmechanisms/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-06-03 04:46:19.000000 brianmechanisms-0.1.8/src/brianmechanisms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23980 2024-06-03 04:46:19.000000 brianmechanisms-0.1.8/src/brianmechanisms/appproximateStraightLineMechanisms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-06-03 04:46:19.000000 brianmechanisms-0.1.8/src/brianmechanisms/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14486 2024-06-03 04:46:19.000000 brianmechanisms-0.1.8/src/brianmechanisms/locii.py
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-06-03 04:46:19.000000 brianmechanisms-0.1.8/src/brianmechanisms/mirror.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-06-03 04:46:19.000000 brianmechanisms-0.1.8/src/brianmechanisms/straightLineMechanisms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 04:46:33.662528 brianmechanisms-0.1.8/src/brianmechanisms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6631 2024-06-03 04:46:33.000000 brianmechanisms-0.1.8/src/brianmechanisms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-06-03 04:46:33.000000 brianmechanisms-0.1.8/src/brianmechanisms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 04:46:33.000000 brianmechanisms-0.1.8/src/brianmechanisms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-06-03 04:46:33.000000 brianmechanisms-0.1.8/src/brianmechanisms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-06-03 04:46:33.000000 brianmechanisms-0.1.8/src/brianmechanisms.egg-info/top_level.txt
```

### Comparing `brianmechanisms-0.1.7/LICENSE` & `brianmechanisms-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `brianmechanisms-0.1.7/PKG-INFO` & `brianmechanisms-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brianmechanisms
-Version: 0.1.7
+Version: 0.1.8
 Summary: Python module for designing mechanisms and robots
 Home-page: https://brianmechanisms.github.io
 Author: Brian Onang'o
 Author-email: surgbc@gmail.com
 Project-URL: Homepage, https://github.com/brianmechanisms/brianmechanisms-designer
 Project-URL: Issues, https://github.com/brianmechanisms/brianmechanisms-designer/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `brianmechanisms-0.1.7/README.md` & `brianmechanisms-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `brianmechanisms-0.1.7/src/brianmechanisms/appproximateStraightLineMechanisms.py` & `brianmechanisms-0.1.8/src/brianmechanisms/appproximateStraightLineMechanisms.py`

 * *Files identical despite different names*

### Comparing `brianmechanisms-0.1.7/src/brianmechanisms/locii.py` & `brianmechanisms-0.1.8/src/brianmechanisms/locii.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,15 +193,15 @@
                 point = self.rotate_point(point, thetaRotation) # Rotate the point
             positions[pointName] =  point#(x_position, y_position) #
         link["positions"] = positions
         return link
 
     def outputPath(self, thetaRange=None):
         if thetaRange is None:
-            thetaRange = np.arange(0, 361, 1)
+            thetaRange = np.arange(0, self.configs.get("thetaMax", 360)+1, 1)
         paths = []
         for theta in thetaRange:
             thetaPoints = {}
             for key, link in self.links.items():
                 link = self.calculatePositions(link, theta, self.configs[key] if key in self.configs else {})
                 thetaPoints[key] = link["positions"]
             paths.append(thetaPoints)
```

### Comparing `brianmechanisms-0.1.7/src/brianmechanisms.egg-info/PKG-INFO` & `brianmechanisms-0.1.8/src/brianmechanisms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brianmechanisms
-Version: 0.1.7
+Version: 0.1.8
 Summary: Python module for designing mechanisms and robots
 Home-page: https://brianmechanisms.github.io
 Author: Brian Onang'o
 Author-email: surgbc@gmail.com
 Project-URL: Homepage, https://github.com/brianmechanisms/brianmechanisms-designer
 Project-URL: Issues, https://github.com/brianmechanisms/brianmechanisms-designer/issues
 Classifier: Programming Language :: Python :: 3
```

