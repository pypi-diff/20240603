# Comparing `tmp/cam_manager-0.2.2.tar.gz` & `tmp/cam_manager-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cam_manager-0.2.2.tar", last modified: Thu May 30 12:49:24 2024, max compression
+gzip compressed data, was "cam_manager-0.2.3.tar", last modified: Mon Jun  3 09:58:26 2024, max compression
```

## Comparing `cam_manager-0.2.2.tar` & `cam_manager-0.2.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:49:24.182844 cam_manager-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-05-30 12:49:24.182844 cam_manager-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-05-30 12:49:12.000000 cam_manager-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:49:24.178845 cam_manager-0.2.2/cam_manager/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-30 12:49:12.000000 cam_manager-0.2.2/cam_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-05-30 12:49:12.000000 cam_manager-0.2.2/cam_manager/cam_ai.py
--rw-r--r--   0 runner    (1001) docker     (127)     6699 2024-05-30 12:49:12.000000 cam_manager-0.2.2/cam_manager/cam_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-30 12:49:12.000000 cam_manager-0.2.2/cam_manager/cam_effects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-30 12:49:12.000000 cam_manager-0.2.2/cam_manager/cam_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-30 12:49:12.000000 cam_manager-0.2.2/cam_manager/cam_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:49:24.182844 cam_manager-0.2.2/cam_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-05-30 12:49:24.000000 cam_manager-0.2.2/cam_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-30 12:49:24.000000 cam_manager-0.2.2/cam_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 12:49:24.000000 cam_manager-0.2.2/cam_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-30 12:49:24.000000 cam_manager-0.2.2/cam_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-30 12:49:24.000000 cam_manager-0.2.2/cam_manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 12:49:24.182844 cam_manager-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-30 12:49:12.000000 cam_manager-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:58:26.557878 cam_manager-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-06-03 09:58:26.557878 cam_manager-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-06-03 09:58:18.000000 cam_manager-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:58:26.557878 cam_manager-0.2.3/cam_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-06-03 09:58:18.000000 cam_manager-0.2.3/cam_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-06-03 09:58:18.000000 cam_manager-0.2.3/cam_manager/cam_ai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6573 2024-06-03 09:58:18.000000 cam_manager-0.2.3/cam_manager/cam_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-06-03 09:58:18.000000 cam_manager-0.2.3/cam_manager/cam_effects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-06-03 09:58:18.000000 cam_manager-0.2.3/cam_manager/cam_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-06-03 09:58:18.000000 cam_manager-0.2.3/cam_manager/cam_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:58:26.557878 cam_manager-0.2.3/cam_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-06-03 09:58:26.000000 cam_manager-0.2.3/cam_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-06-03 09:58:26.000000 cam_manager-0.2.3/cam_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 09:58:26.000000 cam_manager-0.2.3/cam_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-06-03 09:58:26.000000 cam_manager-0.2.3/cam_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-06-03 09:58:26.000000 cam_manager-0.2.3/cam_manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 09:58:26.557878 cam_manager-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-06-03 09:58:18.000000 cam_manager-0.2.3/setup.py
```

### Comparing `cam_manager-0.2.2/PKG-INFO` & `cam_manager-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: cam_manager
-Version: 0.2.2
+Version: 0.2.3
 Summary: A camera management library to easily handle cameras with OpenCV.
 Home-page: https://github.com/snatev/cam-manager
 Author: snatev
 Author-email: snatev@proton.me
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: mss==9.0.1
 Requires-Dist: torch==2.2.2
 Requires-Dist: torchaudio==2.2.2
-Requires-Dist: torchvision==0.17.2
+Requires-Dist: python-xlib==0.33
 Requires-Dist: PyGetWindow==0.0.9
 Requires-Dist: setuptools==69.5.1
+Requires-Dist: torchvision==0.17.2
 Requires-Dist: ultralytics==8.2.22
 Requires-Dist: opencv-python==4.9.0.80
 
 #MANAGER
 --------------------
 In the CamManager init, switch "is_ai" parameter to use the default AI process.
 You can also change the AI mode on the CamManager init with the "ai_mode" parameter. Possible options are: "detection", "segmentation"
```

### Comparing `cam_manager-0.2.2/README.md` & `cam_manager-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `cam_manager-0.2.2/cam_manager/cam_control.py` & `cam_manager-0.2.3/cam_manager/cam_control.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,65 +1,60 @@
 import cv2
 import mss
 import numpy as np
-import pygetwindow as gw
 
 class CamControlMixin:
-    def add_cam(self, cam_id: int, capture_method=cv2.CAP_DSHOW, tricky_window_title: str = None) -> None:
+    def add_cam(self, cam_id: int, capture_method = cv2.CAP_DSHOW, tricky_window_title: str = None) -> None:
         """
         Add a cam by its ID or a "tricky cam" by a window title.
         Parameters:
             cam_id (int): The ID of the cam to be added.
             capture_method: The method used to capture the video stream.
             tricky_window_title (str, optional): The title of the window to be used as a tricky cam.
         """
 
         if tricky_window_title:
             if tricky_window_title not in self.tricky_cams:
-                window = gw.getWindowsWithTitle(tricky_window_title)
+                window = self.get_window_by_title(tricky_window_title)
                 if window:
                     self.tricky_cams[tricky_window_title] = window[0]
-                    if self.active_cam_id is None:
-                        self.active_cam_id = tricky_window_title
+                    if self.active_cam_id is None: self.active_cam_id = tricky_window_title
                     print(f"Tricky cam [{tricky_window_title}] added successfully.")
                 else: print(f"Window with title [{tricky_window_title}] not found.")
             else: print(f"Tricky cam [{tricky_window_title}] is already added.")
         else:
             if cam_id not in self.cams:
                 cap = cv2.VideoCapture(cam_id, capture_method)
                 if not cap.isOpened(): print(f"Failed to open cam [{cam_id}].")
                 else:
                     self.cams[cam_id] = cap
-                    if self.active_cam_id is None:
-                        self.active_cam_id = cam_id
+                    if self.active_cam_id is None: self.active_cam_id = cam_id
                     print(f"Cam [{cam_id}] added successfully.")
             else: print(f"Cam [{cam_id}] is already added.")
 
     def release_cam(self, cam_id: int = None, tricky_window_title: str = None) -> None:
         """
         Release a specific cam by its ID or a tricky cam by its window title.
         Parameters:
             cam_id (int, optional): The ID of the cam to be released.
             tricky_window_title (str, optional): The title of the tricky cam window to be released.
         """
 
         if tricky_window_title:
             if tricky_window_title in self.tricky_cams:
                 del self.tricky_cams[tricky_window_title]
-                if self.active_cam_id == tricky_window_title:
-                    self.active_cam_id = None
+                if self.active_cam_id == tricky_window_title: self.active_cam_id = None
                 print(f"Tricky cam [{tricky_window_title}] released successfully.")
-            else: print(f"Tricky cam [{tricky_window_title}] does not exist.")
+            else:print(f"Tricky cam [{tricky_window_title}] does not exist.")
         else:
             if cam_id in self.cams:
                 self.cams[cam_id].release()
                 del self.cams[cam_id]
 
-                if self.active_cam_id == cam_id:
-                    self.active_cam_id = None
+                if self.active_cam_id == cam_id: self.active_cam_id = None
                 print(f"Cam [{cam_id}] released successfully.")
             else: print(f"Cam [{cam_id}] does not exist.")
 
     def release_all_cams(self) -> None:
         """Release all cams and tricky cams."""
 
         for cam_id in list(self.cams.keys()):
@@ -96,16 +91,15 @@
         Returns: frame (any): The captured frame from the specified or active cam/tricky cam, or None if failed.
         """
 
         if cam_id is None and tricky_window_title is None:
             if self.active_cam_id is None:
                 print("No active cam.")
                 return None
-            if isinstance(self.active_cam_id, int):
-                cam_id = self.active_cam_id
+            if isinstance(self.active_cam_id, int): cam_id = self.active_cam_id
             else: tricky_window_title = self.active_cam_id
 
         if tricky_window_title:
             if tricky_window_title in self.tricky_cams:
                 window = self.tricky_cams[tricky_window_title]
                 with mss.mss() as sct:
                     monitor = {"top": window.top, "left": window.left, "width": window.width, "height": window.height}
```

### Comparing `cam_manager-0.2.2/cam_manager/cam_effects.py` & `cam_manager-0.2.3/cam_manager/cam_effects.py`

 * *Files identical despite different names*

### Comparing `cam_manager-0.2.2/cam_manager/cam_manager.py` & `cam_manager-0.2.3/cam_manager/cam_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from cam_manager.cam_info import CamInfoMixin
 from cam_manager.cam_control import CamControlMixin
 from cam_manager.cam_effects import CamEffectsMixin
 
 class CamManager(CamInfoMixin, CamControlMixin, CamEffectsMixin):
     def __init__(self, is_ai = False, ai_mode = "detection"):
-        possible_ai_modes = ["detection", "segmentation"]
+        possible_ai_modes = ["detection", "segmentation", "classify", "pose"]
         if ai_mode not in possible_ai_modes:
             ai_mode = "detection"
             print(f"Invalid AI mode. Possible values are {possible_ai_modes}")
 
         super().__init__()
 
         self.cams = {}
```

### Comparing `cam_manager-0.2.2/cam_manager.egg-info/PKG-INFO` & `cam_manager-0.2.3/cam_manager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: cam_manager
-Version: 0.2.2
+Version: 0.2.3
 Summary: A camera management library to easily handle cameras with OpenCV.
 Home-page: https://github.com/snatev/cam-manager
 Author: snatev
 Author-email: snatev@proton.me
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: mss==9.0.1
 Requires-Dist: torch==2.2.2
 Requires-Dist: torchaudio==2.2.2
-Requires-Dist: torchvision==0.17.2
+Requires-Dist: python-xlib==0.33
 Requires-Dist: PyGetWindow==0.0.9
 Requires-Dist: setuptools==69.5.1
+Requires-Dist: torchvision==0.17.2
 Requires-Dist: ultralytics==8.2.22
 Requires-Dist: opencv-python==4.9.0.80
 
 #MANAGER
 --------------------
 In the CamManager init, switch "is_ai" parameter to use the default AI process.
 You can also change the AI mode on the CamManager init with the "ai_mode" parameter. Possible options are: "detection", "segmentation"
```

### Comparing `cam_manager-0.2.2/setup.py` & `cam_manager-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
-    version = "0.2.2",
+    version = "0.2.3",
     name = "cam_manager",
     description = "A camera management library to easily handle cameras with OpenCV.",
 
     long_description = open("README.md").read(),
     long_description_content_type = "text/markdown",
 
     author = "snatev",
```

