# Comparing `tmp/cam_manager-0.2.3.tar.gz` & `tmp/cam_manager-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cam_manager-0.2.3.tar", last modified: Mon Jun  3 09:58:26 2024, max compression
+gzip compressed data, was "cam_manager-0.3.0.tar", last modified: Mon Jun  3 11:54:45 2024, max compression
```

## Comparing `cam_manager-0.2.3.tar` & `cam_manager-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:58:26.557878 cam_manager-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-06-03 09:58:26.557878 cam_manager-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-06-03 09:58:18.000000 cam_manager-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:58:26.557878 cam_manager-0.2.3/cam_manager/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-06-03 09:58:18.000000 cam_manager-0.2.3/cam_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-06-03 09:58:18.000000 cam_manager-0.2.3/cam_manager/cam_ai.py
--rw-r--r--   0 runner    (1001) docker     (127)     6573 2024-06-03 09:58:18.000000 cam_manager-0.2.3/cam_manager/cam_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-06-03 09:58:18.000000 cam_manager-0.2.3/cam_manager/cam_effects.py
--rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-06-03 09:58:18.000000 cam_manager-0.2.3/cam_manager/cam_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-06-03 09:58:18.000000 cam_manager-0.2.3/cam_manager/cam_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:58:26.557878 cam_manager-0.2.3/cam_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-06-03 09:58:26.000000 cam_manager-0.2.3/cam_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-06-03 09:58:26.000000 cam_manager-0.2.3/cam_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 09:58:26.000000 cam_manager-0.2.3/cam_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-06-03 09:58:26.000000 cam_manager-0.2.3/cam_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-06-03 09:58:26.000000 cam_manager-0.2.3/cam_manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 09:58:26.557878 cam_manager-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-06-03 09:58:18.000000 cam_manager-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:54:45.427923 cam_manager-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-06-03 11:54:45.427923 cam_manager-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-06-03 11:54:39.000000 cam_manager-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:54:45.423923 cam_manager-0.3.0/cam_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-06-03 11:54:39.000000 cam_manager-0.3.0/cam_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-06-03 11:54:39.000000 cam_manager-0.3.0/cam_manager/cam_ai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6768 2024-06-03 11:54:39.000000 cam_manager-0.3.0/cam_manager/cam_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-06-03 11:54:39.000000 cam_manager-0.3.0/cam_manager/cam_effects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-06-03 11:54:39.000000 cam_manager-0.3.0/cam_manager/cam_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-06-03 11:54:39.000000 cam_manager-0.3.0/cam_manager/cam_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-06-03 11:54:39.000000 cam_manager-0.3.0/cam_manager/cam_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:54:45.423923 cam_manager-0.3.0/cam_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-06-03 11:54:45.000000 cam_manager-0.3.0/cam_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-06-03 11:54:45.000000 cam_manager-0.3.0/cam_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 11:54:45.000000 cam_manager-0.3.0/cam_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-06-03 11:54:45.000000 cam_manager-0.3.0/cam_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-06-03 11:54:45.000000 cam_manager-0.3.0/cam_manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 11:54:45.427923 cam_manager-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-06-03 11:54:39.000000 cam_manager-0.3.0/setup.py
```

### Comparing `cam_manager-0.2.3/PKG-INFO` & `cam_manager-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cam_manager
-Version: 0.2.3
+Version: 0.3.0
 Summary: A camera management library to easily handle cameras with OpenCV.
 Home-page: https://github.com/snatev/cam-manager
 Author: snatev
 Author-email: snatev@proton.me
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cam_manager-0.2.3/README.md` & `cam_manager-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `cam_manager-0.2.3/cam_manager/cam_ai.py` & `cam_manager-0.3.0/cam_manager/cam_ai.py`

 * *Files identical despite different names*

### Comparing `cam_manager-0.2.3/cam_manager/cam_control.py` & `cam_manager-0.3.0/cam_manager/cam_control.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import cv2
 import mss
 import numpy as np
+from cam_manager.cam_settings import CamSettingsMixin as Settings
 
 class CamControlMixin:
     def add_cam(self, cam_id: int, capture_method = cv2.CAP_DSHOW, tricky_window_title: str = None) -> None:
         """
         Add a cam by its ID or a "tricky cam" by a window title.
         Parameters:
             cam_id (int): The ID of the cam to be added.
@@ -23,14 +24,18 @@
             else: print(f"Tricky cam [{tricky_window_title}] is already added.")
         else:
             if cam_id not in self.cams:
                 cap = cv2.VideoCapture(cam_id, capture_method)
                 if not cap.isOpened(): print(f"Failed to open cam [{cam_id}].")
                 else:
                     self.cams[cam_id] = cap
+
+                    cam_settings = Settings(f"cam_settings_{cam_id}.json")
+                    cam_settings.load_settings(cap)
+
                     if self.active_cam_id is None: self.active_cam_id = cam_id
                     print(f"Cam [{cam_id}] added successfully.")
             else: print(f"Cam [{cam_id}] is already added.")
 
     def release_cam(self, cam_id: int = None, tricky_window_title: str = None) -> None:
         """
         Release a specific cam by its ID or a tricky cam by its window title.
```

### Comparing `cam_manager-0.2.3/cam_manager/cam_effects.py` & `cam_manager-0.3.0/cam_manager/cam_effects.py`

 * *Files identical despite different names*

### Comparing `cam_manager-0.2.3/cam_manager/cam_info.py` & `cam_manager-0.3.0/cam_manager/cam_info.py`

 * *Files identical despite different names*

### Comparing `cam_manager-0.2.3/cam_manager/cam_manager.py` & `cam_manager-0.3.0/cam_manager/cam_manager.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from cam_manager.cam_info import CamInfoMixin
 from cam_manager.cam_control import CamControlMixin
 from cam_manager.cam_effects import CamEffectsMixin
+from cam_manager.cam_settings import CamSettingsMixin
 
-class CamManager(CamInfoMixin, CamControlMixin, CamEffectsMixin):
-    def __init__(self, is_ai = False, ai_mode = "detection"):
+class CamManager(CamInfoMixin, CamControlMixin, CamEffectsMixin, CamSettingsMixin):
+    def __init__(self, is_ai = False, ai_mode = "detection", load_settings = False):
         possible_ai_modes = ["detection", "segmentation", "classify", "pose"]
         if ai_mode not in possible_ai_modes:
             ai_mode = "detection"
             print(f"Invalid AI mode. Possible values are {possible_ai_modes}")
 
         super().__init__()
 
         self.cams = {}
         self.tricky_cams = {}
         self.active_cam_id = None
+        self.load_settings = load_settings
 
         if is_ai:
             from cam_manager.cam_ai import CamAIMixin
             self.ai = CamAIMixin(ai_mode)
         else: self.ai = None
```

### Comparing `cam_manager-0.2.3/cam_manager.egg-info/PKG-INFO` & `cam_manager-0.3.0/cam_manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cam_manager
-Version: 0.2.3
+Version: 0.3.0
 Summary: A camera management library to easily handle cameras with OpenCV.
 Home-page: https://github.com/snatev/cam-manager
 Author: snatev
 Author-email: snatev@proton.me
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cam_manager-0.2.3/setup.py` & `cam_manager-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
-    version = "0.2.3",
+    version = "0.3.0",
     name = "cam_manager",
     description = "A camera management library to easily handle cameras with OpenCV.",
 
     long_description = open("README.md").read(),
     long_description_content_type = "text/markdown",
 
     author = "snatev",
```

