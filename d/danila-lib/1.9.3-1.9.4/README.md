# Comparing `tmp/danila-lib-1.9.3.tar.gz` & `tmp/danila-lib-1.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "danila-lib-1.9.3.tar", last modified: Mon Jun  3 14:21:36 2024, max compression
+gzip compressed data, was "danila-lib-1.9.4.tar", last modified: Mon Jun  3 14:35:16 2024, max compression
```

## Comparing `danila-lib-1.9.3.tar` & `danila-lib-1.9.4.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2024-06-03 14:21:36.250494 danila-lib-1.9.3/
--rw-rw-rw-   0        0        0     9615 2024-06-03 14:21:36.249498 danila-lib-1.9.3/PKG-INFO
--rw-rw-rw-   0        0        0     5060 2024-04-22 21:01:41.000000 danila-lib-1.9.3/README.md
-drwxrwxrwx   0        0        0        0 2024-06-03 14:21:35.945865 danila-lib-1.9.3/danila/
--rw-rw-rw-   0        0        0        0 2024-04-15 11:55:56.000000 danila-lib-1.9.3/danila/__init__.py
--rw-rw-rw-   0        0        0     2366 2024-06-03 14:10:15.000000 danila-lib-1.9.3/danila/danila.py
--rw-rw-rw-   0        0        0     9764 2024-05-22 08:43:39.000000 danila-lib-1.9.3/danila/danila_v1.py
--rw-rw-rw-   0        0        0    10182 2024-05-22 08:43:39.000000 danila-lib-1.9.3/danila/danila_v2.py
--rw-rw-rw-   0        0        0    10706 2024-05-22 08:43:39.000000 danila-lib-1.9.3/danila/danila_v3.py
--rw-rw-rw-   0        0        0    19809 2024-06-03 14:21:20.000000 danila-lib-1.9.3/danila/danila_v4.py
-drwxrwxrwx   0        0        0        0 2024-06-03 14:21:35.987672 danila-lib-1.9.3/danila_lib.egg-info/
--rw-rw-rw-   0        0        0     9615 2024-06-03 14:21:35.000000 danila-lib-1.9.3/danila_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1025 2024-06-03 14:21:35.000000 danila-lib-1.9.3/danila_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-03 14:21:35.000000 danila-lib-1.9.3/danila_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1879 2024-06-03 14:21:35.000000 danila-lib-1.9.3/danila_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-06-03 14:21:35.000000 danila-lib-1.9.3/danila_lib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-06-03 14:21:35.988668 danila-lib-1.9.3/data/
--rw-rw-rw-   0        0        0        0 2024-04-15 12:01:57.000000 danila-lib-1.9.3/data/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-03 14:21:36.086236 danila-lib-1.9.3/data/neuro/
--rw-rw-rw-   0        0        0     2311 2024-06-03 14:02:44.000000 danila-lib-1.9.3/data/neuro/Detail_classify_class.py
--rw-rw-rw-   0        0        0     5722 2024-04-22 21:09:12.000000 danila-lib-1.9.3/data/neuro/Letters_recognize.py
--rw-rw-rw-   0        0        0     2121 2024-05-22 08:48:35.000000 danila-lib-1.9.3/data/neuro/Rama_detect_class.py
--rw-rw-rw-   0        0        0     3000 2024-05-28 08:28:46.000000 danila-lib-1.9.3/data/neuro/Rama_prod_classify_class.py
--rw-rw-rw-   0        0        0     3153 2024-05-23 05:46:54.000000 danila-lib-1.9.3/data/neuro/Text_detect_class.py
--rw-rw-rw-   0        0        0     2643 2024-06-02 10:27:15.000000 danila-lib-1.9.3/data/neuro/Vagon_number_detect_class.py
--rw-rw-rw-   0        0        0     4327 2024-06-03 10:52:22.000000 danila-lib-1.9.3/data/neuro/Vagon_number_recognize_class.py
--rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.9.3/data/neuro/__init__.py
--rw-rw-rw-   0        0        0     6695 2024-05-28 13:59:46.000000 danila-lib-1.9.3/data/neuro/letters_in_image.py
--rw-rw-rw-   0        0        0     1034 2024-06-03 13:03:03.000000 danila-lib-1.9.3/data/neuro/models.py
--rw-rw-rw-   0        0        0     3222 2024-05-27 08:43:50.000000 danila-lib-1.9.3/data/neuro/objs_in_image.py
--rw-rw-rw-   0        0        0     4854 2024-05-28 13:59:46.000000 danila-lib-1.9.3/data/neuro/text_recognize_yolo.py
-drwxrwxrwx   0        0        0        0 2024-06-03 14:21:36.217643 danila-lib-1.9.3/data/result/
--rw-rw-rw-   0        0        0      220 2024-06-03 14:02:44.000000 danila-lib-1.9.3/data/result/Class_im.py
--rw-rw-rw-   0        0        0      108 2023-12-12 16:53:34.000000 danila-lib-1.9.3/data/result/Class_text.py
--rw-rw-rw-   0        0        0     2811 2024-04-22 19:35:07.000000 danila-lib-1.9.3/data/result/Image_text_areas.py
--rw-rw-rw-   0        0        0      332 2024-05-27 09:58:57.000000 danila-lib-1.9.3/data/result/Label_area.py
--rw-rw-rw-   0        0        0      236 2024-05-27 08:43:50.000000 danila-lib-1.9.3/data/result/Rama_prod.py
--rw-rw-rw-   0        0        0     3233 2024-04-22 18:17:45.000000 danila-lib-1.9.3/data/result/Rect.py
--rw-rw-rw-   0        0        0      539 2024-04-22 18:52:56.000000 danila-lib-1.9.3/data/result/Text_area.py
--rw-rw-rw-   0        0        0      716 2024-04-22 10:33:16.000000 danila-lib-1.9.3/data/result/Yolo_label_rect.py
--rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.9.3/data/result/__init__.py
--rw-rw-rw-   0        0        0      126 2024-05-14 11:04:15.000000 danila-lib-1.9.3/data/result/prod_classify_result.py
--rw-rw-rw-   0        0        0      122 2024-05-06 08:55:07.000000 danila-lib-1.9.3/data/result/word_compare_result.py
--rw-rw-rw-   0        0        0       42 2024-06-03 14:21:36.272397 danila-lib-1.9.3/setup.cfg
--rw-rw-rw-   0        0        0      983 2024-06-03 14:21:32.000000 danila-lib-1.9.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 14:35:16.008038 danila-lib-1.9.4/
+-rw-rw-rw-   0        0        0     9615 2024-06-03 14:35:16.006046 danila-lib-1.9.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5060 2024-04-22 21:01:41.000000 danila-lib-1.9.4/README.md
+drwxrwxrwx   0        0        0        0 2024-06-03 14:35:15.651628 danila-lib-1.9.4/danila/
+-rw-rw-rw-   0        0        0        0 2024-04-15 11:55:56.000000 danila-lib-1.9.4/danila/__init__.py
+-rw-rw-rw-   0        0        0     2366 2024-06-03 14:10:15.000000 danila-lib-1.9.4/danila/danila.py
+-rw-rw-rw-   0        0        0     9764 2024-05-22 08:43:39.000000 danila-lib-1.9.4/danila/danila_v1.py
+-rw-rw-rw-   0        0        0    10182 2024-05-22 08:43:39.000000 danila-lib-1.9.4/danila/danila_v2.py
+-rw-rw-rw-   0        0        0    10706 2024-05-22 08:43:39.000000 danila-lib-1.9.4/danila/danila_v3.py
+-rw-rw-rw-   0        0        0    19809 2024-06-03 14:21:20.000000 danila-lib-1.9.4/danila/danila_v4.py
+drwxrwxrwx   0        0        0        0 2024-06-03 14:35:15.787028 danila-lib-1.9.4/danila_lib.egg-info/
+-rw-rw-rw-   0        0        0     9615 2024-06-03 14:35:15.000000 danila-lib-1.9.4/danila_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1025 2024-06-03 14:35:15.000000 danila-lib-1.9.4/danila_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 14:35:15.000000 danila-lib-1.9.4/danila_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1879 2024-06-03 14:35:15.000000 danila-lib-1.9.4/danila_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-06-03 14:35:15.000000 danila-lib-1.9.4/danila_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-03 14:35:15.819877 danila-lib-1.9.4/data/
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:01:57.000000 danila-lib-1.9.4/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 14:35:15.983143 danila-lib-1.9.4/data/neuro/
+-rw-rw-rw-   0        0        0     2327 2024-06-03 14:34:30.000000 danila-lib-1.9.4/data/neuro/Detail_classify_class.py
+-rw-rw-rw-   0        0        0     5722 2024-04-22 21:09:12.000000 danila-lib-1.9.4/data/neuro/Letters_recognize.py
+-rw-rw-rw-   0        0        0     2121 2024-05-22 08:48:35.000000 danila-lib-1.9.4/data/neuro/Rama_detect_class.py
+-rw-rw-rw-   0        0        0     3000 2024-05-28 08:28:46.000000 danila-lib-1.9.4/data/neuro/Rama_prod_classify_class.py
+-rw-rw-rw-   0        0        0     3153 2024-05-23 05:46:54.000000 danila-lib-1.9.4/data/neuro/Text_detect_class.py
+-rw-rw-rw-   0        0        0     2643 2024-06-02 10:27:15.000000 danila-lib-1.9.4/data/neuro/Vagon_number_detect_class.py
+-rw-rw-rw-   0        0        0     4327 2024-06-03 10:52:22.000000 danila-lib-1.9.4/data/neuro/Vagon_number_recognize_class.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.9.4/data/neuro/__init__.py
+-rw-rw-rw-   0        0        0     6695 2024-05-28 13:59:46.000000 danila-lib-1.9.4/data/neuro/letters_in_image.py
+-rw-rw-rw-   0        0        0     1034 2024-06-03 13:03:03.000000 danila-lib-1.9.4/data/neuro/models.py
+-rw-rw-rw-   0        0        0     3222 2024-05-27 08:43:50.000000 danila-lib-1.9.4/data/neuro/objs_in_image.py
+-rw-rw-rw-   0        0        0     4854 2024-05-28 13:59:46.000000 danila-lib-1.9.4/data/neuro/text_recognize_yolo.py
+drwxrwxrwx   0        0        0        0 2024-06-03 14:35:15.998075 danila-lib-1.9.4/data/result/
+-rw-rw-rw-   0        0        0      220 2024-06-03 14:02:44.000000 danila-lib-1.9.4/data/result/Class_im.py
+-rw-rw-rw-   0        0        0      108 2023-12-12 16:53:34.000000 danila-lib-1.9.4/data/result/Class_text.py
+-rw-rw-rw-   0        0        0     2811 2024-04-22 19:35:07.000000 danila-lib-1.9.4/data/result/Image_text_areas.py
+-rw-rw-rw-   0        0        0      332 2024-05-27 09:58:57.000000 danila-lib-1.9.4/data/result/Label_area.py
+-rw-rw-rw-   0        0        0      236 2024-05-27 08:43:50.000000 danila-lib-1.9.4/data/result/Rama_prod.py
+-rw-rw-rw-   0        0        0     3233 2024-04-22 18:17:45.000000 danila-lib-1.9.4/data/result/Rect.py
+-rw-rw-rw-   0        0        0      539 2024-04-22 18:52:56.000000 danila-lib-1.9.4/data/result/Text_area.py
+-rw-rw-rw-   0        0        0      716 2024-04-22 10:33:16.000000 danila-lib-1.9.4/data/result/Yolo_label_rect.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.9.4/data/result/__init__.py
+-rw-rw-rw-   0        0        0      126 2024-05-14 11:04:15.000000 danila-lib-1.9.4/data/result/prod_classify_result.py
+-rw-rw-rw-   0        0        0      122 2024-05-06 08:55:07.000000 danila-lib-1.9.4/data/result/word_compare_result.py
+-rw-rw-rw-   0        0        0       42 2024-06-03 14:35:16.026947 danila-lib-1.9.4/setup.cfg
+-rw-rw-rw-   0        0        0      983 2024-06-03 14:35:03.000000 danila-lib-1.9.4/setup.py
```

### Comparing `danila-lib-1.9.3/PKG-INFO` & `danila-lib-1.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danila-lib
-Version: 1.9.3
+Version: 1.9.4
 Summary: This is the module for detecting and classifying text on rama pictures
 Home-page: https://github.com/Arseniy-Zhuck/danila_lib
 Author: arseniy_zhuck
 Author-email: arseniyzhuck@mail.ru
 Project-URL: GitHub, https://github.com/Arseniy-Zhuck/danila_lib
 Keywords: rama detect machine-learning computer-vision
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `danila-lib-1.9.3/README.md` & `danila-lib-1.9.4/README.md`

 * *Files identical despite different names*

### Comparing `danila-lib-1.9.3/danila/danila.py` & `danila-lib-1.9.4/danila/danila.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.9.3/danila/danila_v1.py` & `danila-lib-1.9.4/danila/danila_v1.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.9.3/danila/danila_v2.py` & `danila-lib-1.9.4/danila/danila_v2.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.9.3/danila/danila_v3.py` & `danila-lib-1.9.4/danila/danila_v3.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.9.3/danila/danila_v4.py` & `danila-lib-1.9.4/danila/danila_v4.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.9.3/danila_lib.egg-info/PKG-INFO` & `danila-lib-1.9.4/danila_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danila-lib
-Version: 1.9.3
+Version: 1.9.4
 Summary: This is the module for detecting and classifying text on rama pictures
 Home-page: https://github.com/Arseniy-Zhuck/danila_lib
 Author: arseniy_zhuck
 Author-email: arseniyzhuck@mail.ru
 Project-URL: GitHub, https://github.com/Arseniy-Zhuck/danila_lib
 Keywords: rama detect machine-learning computer-vision
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `danila-lib-1.9.3/danila_lib.egg-info/SOURCES.txt` & `danila-lib-1.9.4/danila_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `danila-lib-1.9.3/danila_lib.egg-info/requires.txt` & `danila-lib-1.9.4/danila_lib.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `danila-lib-1.9.3/data/neuro/Detail_classify_class.py` & `danila-lib-1.9.4/data/neuro/Detail_classify_class.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import cv2
-import keras
+from tensorflow import keras
 import numpy as np
 
 from data.neuro.models import *
 from data.result.Class_im import *
 import zipfile
 import requests
 from urllib.parse import urlencode
```

### Comparing `danila-lib-1.9.3/data/neuro/Letters_recognize.py` & `danila-lib-1.9.4/data/neuro/Letters_recognize.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.9.3/data/neuro/Rama_detect_class.py` & `danila-lib-1.9.4/data/neuro/Rama_detect_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.9.3/data/neuro/Rama_prod_classify_class.py` & `danila-lib-1.9.4/data/neuro/Rama_prod_classify_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.9.3/data/neuro/Text_detect_class.py` & `danila-lib-1.9.4/data/neuro/Text_detect_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.9.3/data/neuro/Vagon_number_detect_class.py` & `danila-lib-1.9.4/data/neuro/Vagon_number_detect_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.9.3/data/neuro/Vagon_number_recognize_class.py` & `danila-lib-1.9.4/data/neuro/Vagon_number_recognize_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.9.3/data/neuro/letters_in_image.py` & `danila-lib-1.9.4/data/neuro/letters_in_image.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.9.3/data/neuro/models.py` & `danila-lib-1.9.4/data/neuro/models.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.9.3/data/neuro/objs_in_image.py` & `danila-lib-1.9.4/data/neuro/objs_in_image.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.9.3/data/neuro/text_recognize_yolo.py` & `danila-lib-1.9.4/data/neuro/text_recognize_yolo.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.9.3/data/result/Image_text_areas.py` & `danila-lib-1.9.4/data/result/Image_text_areas.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.9.3/data/result/Rect.py` & `danila-lib-1.9.4/data/result/Rect.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.9.3/data/result/Text_area.py` & `danila-lib-1.9.4/data/result/Text_area.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.9.3/data/result/Yolo_label_rect.py` & `danila-lib-1.9.4/data/result/Yolo_label_rect.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.9.3/setup.py` & `danila-lib-1.9.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   with open('requirements.txt', 'r') as f:
     a = f.read()
   b = a.split()
   return b
 
 setup(
   name='danila-lib',
-  version='1.9.3',
+  version='1.9.4',
   author='arseniy_zhuck',
   author_email='arseniyzhuck@mail.ru',
   description='This is the module for detecting and classifying text on rama pictures',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://github.com/Arseniy-Zhuck/danila_lib',
   packages=find_packages(),
```

