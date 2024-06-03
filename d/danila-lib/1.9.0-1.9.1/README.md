# Comparing `tmp/danila-lib-1.9.0.tar.gz` & `tmp/danila-lib-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "danila-lib-1.9.0.tar", last modified: Mon Jun  3 14:02:50 2024, max compression
+gzip compressed data, was "danila-lib-1.9.1.tar", last modified: Mon Jun  3 14:10:31 2024, max compression
```

## Comparing `danila-lib-1.9.0.tar` & `danila-lib-1.9.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2024-06-03 14:02:50.263303 danila-lib-1.9.0/
--rw-rw-rw-   0        0        0     9615 2024-06-03 14:02:50.263303 danila-lib-1.9.0/PKG-INFO
--rw-rw-rw-   0        0        0     5060 2024-04-22 21:01:41.000000 danila-lib-1.9.0/README.md
-drwxrwxrwx   0        0        0        0 2024-06-03 14:02:50.146827 danila-lib-1.9.0/danila/
--rw-rw-rw-   0        0        0        0 2024-04-15 11:55:56.000000 danila-lib-1.9.0/danila/__init__.py
--rw-rw-rw-   0        0        0     2354 2024-06-03 10:26:25.000000 danila-lib-1.9.0/danila/danila.py
--rw-rw-rw-   0        0        0     9764 2024-05-22 08:43:39.000000 danila-lib-1.9.0/danila/danila_v1.py
--rw-rw-rw-   0        0        0    10182 2024-05-22 08:43:39.000000 danila-lib-1.9.0/danila/danila_v2.py
--rw-rw-rw-   0        0        0    10706 2024-05-22 08:43:39.000000 danila-lib-1.9.0/danila/danila_v3.py
--rw-rw-rw-   0        0        0    19873 2024-06-03 14:02:44.000000 danila-lib-1.9.0/danila/danila_v4.py
-drwxrwxrwx   0        0        0        0 2024-06-03 14:02:50.244387 danila-lib-1.9.0/danila_lib.egg-info/
--rw-rw-rw-   0        0        0     9615 2024-06-03 14:02:49.000000 danila-lib-1.9.0/danila_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1059 2024-06-03 14:02:49.000000 danila-lib-1.9.0/danila_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-03 14:02:49.000000 danila-lib-1.9.0/danila_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1879 2024-06-03 14:02:49.000000 danila-lib-1.9.0/danila_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-06-03 14:02:49.000000 danila-lib-1.9.0/danila_lib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-06-03 14:02:50.245383 danila-lib-1.9.0/data/
--rw-rw-rw-   0        0        0        0 2024-04-15 12:01:57.000000 danila-lib-1.9.0/data/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-03 14:02:50.255339 danila-lib-1.9.0/data/neuro/
--rw-rw-rw-   0        0        0     2311 2024-06-03 14:02:44.000000 danila-lib-1.9.0/data/neuro/Detail_classify_class.py
--rw-rw-rw-   0        0        0     5722 2024-04-22 21:09:12.000000 danila-lib-1.9.0/data/neuro/Letters_recognize.py
--rw-rw-rw-   0        0        0     2754 2024-04-22 10:33:16.000000 danila-lib-1.9.0/data/neuro/Rama_classify_class.py
--rw-rw-rw-   0        0        0     2121 2024-05-22 08:48:35.000000 danila-lib-1.9.0/data/neuro/Rama_detect_class.py
--rw-rw-rw-   0        0        0     3000 2024-05-28 08:28:46.000000 danila-lib-1.9.0/data/neuro/Rama_prod_classify_class.py
--rw-rw-rw-   0        0        0     3153 2024-05-23 05:46:54.000000 danila-lib-1.9.0/data/neuro/Text_detect_class.py
--rw-rw-rw-   0        0        0     2643 2024-06-02 10:27:15.000000 danila-lib-1.9.0/data/neuro/Vagon_number_detect_class.py
--rw-rw-rw-   0        0        0     4327 2024-06-03 10:52:22.000000 danila-lib-1.9.0/data/neuro/Vagon_number_recognize_class.py
--rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.9.0/data/neuro/__init__.py
--rw-rw-rw-   0        0        0     6695 2024-05-28 13:59:46.000000 danila-lib-1.9.0/data/neuro/letters_in_image.py
--rw-rw-rw-   0        0        0     1034 2024-06-03 13:03:03.000000 danila-lib-1.9.0/data/neuro/models.py
--rw-rw-rw-   0        0        0     3222 2024-05-27 08:43:50.000000 danila-lib-1.9.0/data/neuro/objs_in_image.py
--rw-rw-rw-   0        0        0     4854 2024-05-28 13:59:46.000000 danila-lib-1.9.0/data/neuro/text_recognize_yolo.py
-drwxrwxrwx   0        0        0        0 2024-06-03 14:02:50.262307 danila-lib-1.9.0/data/result/
--rw-rw-rw-   0        0        0      220 2024-06-03 14:02:44.000000 danila-lib-1.9.0/data/result/Class_im.py
--rw-rw-rw-   0        0        0      108 2023-12-12 16:53:34.000000 danila-lib-1.9.0/data/result/Class_text.py
--rw-rw-rw-   0        0        0     2811 2024-04-22 19:35:07.000000 danila-lib-1.9.0/data/result/Image_text_areas.py
--rw-rw-rw-   0        0        0      332 2024-05-27 09:58:57.000000 danila-lib-1.9.0/data/result/Label_area.py
--rw-rw-rw-   0        0        0      236 2024-05-27 08:43:50.000000 danila-lib-1.9.0/data/result/Rama_prod.py
--rw-rw-rw-   0        0        0     3233 2024-04-22 18:17:45.000000 danila-lib-1.9.0/data/result/Rect.py
--rw-rw-rw-   0        0        0      539 2024-04-22 18:52:56.000000 danila-lib-1.9.0/data/result/Text_area.py
--rw-rw-rw-   0        0        0      716 2024-04-22 10:33:16.000000 danila-lib-1.9.0/data/result/Yolo_label_rect.py
--rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.9.0/data/result/__init__.py
--rw-rw-rw-   0        0        0      126 2024-05-14 11:04:15.000000 danila-lib-1.9.0/data/result/prod_classify_result.py
--rw-rw-rw-   0        0        0      122 2024-05-06 08:55:07.000000 danila-lib-1.9.0/data/result/word_compare_result.py
--rw-rw-rw-   0        0        0       42 2024-06-03 14:02:50.279232 danila-lib-1.9.0/setup.cfg
--rw-rw-rw-   0        0        0      983 2024-06-03 14:02:44.000000 danila-lib-1.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 14:10:31.470478 danila-lib-1.9.1/
+-rw-rw-rw-   0        0        0     9615 2024-06-03 14:10:31.469483 danila-lib-1.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5060 2024-04-22 21:01:41.000000 danila-lib-1.9.1/README.md
+drwxrwxrwx   0        0        0        0 2024-06-03 14:10:31.333090 danila-lib-1.9.1/danila/
+-rw-rw-rw-   0        0        0        0 2024-04-15 11:55:56.000000 danila-lib-1.9.1/danila/__init__.py
+-rw-rw-rw-   0        0        0     2366 2024-06-03 14:10:15.000000 danila-lib-1.9.1/danila/danila.py
+-rw-rw-rw-   0        0        0     9764 2024-05-22 08:43:39.000000 danila-lib-1.9.1/danila/danila_v1.py
+-rw-rw-rw-   0        0        0    10182 2024-05-22 08:43:39.000000 danila-lib-1.9.1/danila/danila_v2.py
+-rw-rw-rw-   0        0        0    10706 2024-05-22 08:43:39.000000 danila-lib-1.9.1/danila/danila_v3.py
+-rw-rw-rw-   0        0        0    19873 2024-06-03 14:02:44.000000 danila-lib-1.9.1/danila/danila_v4.py
+drwxrwxrwx   0        0        0        0 2024-06-03 14:10:31.414727 danila-lib-1.9.1/danila_lib.egg-info/
+-rw-rw-rw-   0        0        0     9615 2024-06-03 14:10:30.000000 danila-lib-1.9.1/danila_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1059 2024-06-03 14:10:30.000000 danila-lib-1.9.1/danila_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 14:10:30.000000 danila-lib-1.9.1/danila_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1879 2024-06-03 14:10:30.000000 danila-lib-1.9.1/danila_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-06-03 14:10:30.000000 danila-lib-1.9.1/danila_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-03 14:10:31.415722 danila-lib-1.9.1/data/
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:01:57.000000 danila-lib-1.9.1/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 14:10:31.454552 danila-lib-1.9.1/data/neuro/
+-rw-rw-rw-   0        0        0     2311 2024-06-03 14:02:44.000000 danila-lib-1.9.1/data/neuro/Detail_classify_class.py
+-rw-rw-rw-   0        0        0     5722 2024-04-22 21:09:12.000000 danila-lib-1.9.1/data/neuro/Letters_recognize.py
+-rw-rw-rw-   0        0        0     2754 2024-04-22 10:33:16.000000 danila-lib-1.9.1/data/neuro/Rama_classify_class.py
+-rw-rw-rw-   0        0        0     2121 2024-05-22 08:48:35.000000 danila-lib-1.9.1/data/neuro/Rama_detect_class.py
+-rw-rw-rw-   0        0        0     3000 2024-05-28 08:28:46.000000 danila-lib-1.9.1/data/neuro/Rama_prod_classify_class.py
+-rw-rw-rw-   0        0        0     3153 2024-05-23 05:46:54.000000 danila-lib-1.9.1/data/neuro/Text_detect_class.py
+-rw-rw-rw-   0        0        0     2643 2024-06-02 10:27:15.000000 danila-lib-1.9.1/data/neuro/Vagon_number_detect_class.py
+-rw-rw-rw-   0        0        0     4327 2024-06-03 10:52:22.000000 danila-lib-1.9.1/data/neuro/Vagon_number_recognize_class.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.9.1/data/neuro/__init__.py
+-rw-rw-rw-   0        0        0     6695 2024-05-28 13:59:46.000000 danila-lib-1.9.1/data/neuro/letters_in_image.py
+-rw-rw-rw-   0        0        0     1034 2024-06-03 13:03:03.000000 danila-lib-1.9.1/data/neuro/models.py
+-rw-rw-rw-   0        0        0     3222 2024-05-27 08:43:50.000000 danila-lib-1.9.1/data/neuro/objs_in_image.py
+-rw-rw-rw-   0        0        0     4854 2024-05-28 13:59:46.000000 danila-lib-1.9.1/data/neuro/text_recognize_yolo.py
+drwxrwxrwx   0        0        0        0 2024-06-03 14:10:31.468487 danila-lib-1.9.1/data/result/
+-rw-rw-rw-   0        0        0      220 2024-06-03 14:02:44.000000 danila-lib-1.9.1/data/result/Class_im.py
+-rw-rw-rw-   0        0        0      108 2023-12-12 16:53:34.000000 danila-lib-1.9.1/data/result/Class_text.py
+-rw-rw-rw-   0        0        0     2811 2024-04-22 19:35:07.000000 danila-lib-1.9.1/data/result/Image_text_areas.py
+-rw-rw-rw-   0        0        0      332 2024-05-27 09:58:57.000000 danila-lib-1.9.1/data/result/Label_area.py
+-rw-rw-rw-   0        0        0      236 2024-05-27 08:43:50.000000 danila-lib-1.9.1/data/result/Rama_prod.py
+-rw-rw-rw-   0        0        0     3233 2024-04-22 18:17:45.000000 danila-lib-1.9.1/data/result/Rect.py
+-rw-rw-rw-   0        0        0      539 2024-04-22 18:52:56.000000 danila-lib-1.9.1/data/result/Text_area.py
+-rw-rw-rw-   0        0        0      716 2024-04-22 10:33:16.000000 danila-lib-1.9.1/data/result/Yolo_label_rect.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.9.1/data/result/__init__.py
+-rw-rw-rw-   0        0        0      126 2024-05-14 11:04:15.000000 danila-lib-1.9.1/data/result/prod_classify_result.py
+-rw-rw-rw-   0        0        0      122 2024-05-06 08:55:07.000000 danila-lib-1.9.1/data/result/word_compare_result.py
+-rw-rw-rw-   0        0        0       42 2024-06-03 14:10:31.472469 danila-lib-1.9.1/setup.cfg
+-rw-rw-rw-   0        0        0      983 2024-06-03 14:10:27.000000 danila-lib-1.9.1/setup.py
```

### Comparing `danila-lib-1.9.0/PKG-INFO` & `danila-lib-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danila-lib
-Version: 1.9.0
+Version: 1.9.1
 Summary: This is the module for detecting and classifying text on rama pictures
 Home-page: https://github.com/Arseniy-Zhuck/danila_lib
 Author: arseniy_zhuck
 Author-email: arseniyzhuck@mail.ru
 Project-URL: GitHub, https://github.com/Arseniy-Zhuck/danila_lib
 Keywords: rama detect machine-learning computer-vision
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `danila-lib-1.9.0/README.md` & `danila-lib-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `danila-lib-1.9.0/danila/danila.py` & `danila-lib-1.9.1/danila/danila.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-import os
-
-import cv2
-
-from danila.danila_v1 import Danila_v1
-from danila.danila_v2 import Danila_v2
-from danila.danila_v3 import Danila_v3
+# import os
+#
+# import cv2
+#
+# from danila.danila_v1 import Danila_v1
+# from danila.danila_v2 import Danila_v2
+# from danila.danila_v3 import Danila_v3
 from danila.danila_v4 import Danila_v4
 
 """main module for user"""
 
 
 class Danila:
     """main class for user"""
```

### Comparing `danila-lib-1.9.0/danila/danila_v1.py` & `danila-lib-1.9.1/danila/danila_v1.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.9.0/danila/danila_v2.py` & `danila-lib-1.9.1/danila/danila_v2.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.9.0/danila/danila_v3.py` & `danila-lib-1.9.1/danila/danila_v3.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.9.0/danila/danila_v4.py` & `danila-lib-1.9.1/danila/danila_v4.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.9.0/danila_lib.egg-info/PKG-INFO` & `danila-lib-1.9.1/danila_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danila-lib
-Version: 1.9.0
+Version: 1.9.1
 Summary: This is the module for detecting and classifying text on rama pictures
 Home-page: https://github.com/Arseniy-Zhuck/danila_lib
 Author: arseniy_zhuck
 Author-email: arseniyzhuck@mail.ru
 Project-URL: GitHub, https://github.com/Arseniy-Zhuck/danila_lib
 Keywords: rama detect machine-learning computer-vision
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `danila-lib-1.9.0/danila_lib.egg-info/SOURCES.txt` & `danila-lib-1.9.1/danila_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `danila-lib-1.9.0/danila_lib.egg-info/requires.txt` & `danila-lib-1.9.1/danila_lib.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `danila-lib-1.9.0/data/neuro/Detail_classify_class.py` & `danila-lib-1.9.1/data/neuro/Detail_classify_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.9.0/data/neuro/Letters_recognize.py` & `danila-lib-1.9.1/data/neuro/Letters_recognize.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.9.0/data/neuro/Rama_classify_class.py` & `danila-lib-1.9.1/data/neuro/Rama_classify_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.9.0/data/neuro/Rama_detect_class.py` & `danila-lib-1.9.1/data/neuro/Rama_detect_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.9.0/data/neuro/Rama_prod_classify_class.py` & `danila-lib-1.9.1/data/neuro/Rama_prod_classify_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.9.0/data/neuro/Text_detect_class.py` & `danila-lib-1.9.1/data/neuro/Text_detect_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.9.0/data/neuro/Vagon_number_detect_class.py` & `danila-lib-1.9.1/data/neuro/Vagon_number_detect_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.9.0/data/neuro/Vagon_number_recognize_class.py` & `danila-lib-1.9.1/data/neuro/Vagon_number_recognize_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.9.0/data/neuro/letters_in_image.py` & `danila-lib-1.9.1/data/neuro/letters_in_image.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.9.0/data/neuro/models.py` & `danila-lib-1.9.1/data/neuro/models.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.9.0/data/neuro/objs_in_image.py` & `danila-lib-1.9.1/data/neuro/objs_in_image.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.9.0/data/neuro/text_recognize_yolo.py` & `danila-lib-1.9.1/data/neuro/text_recognize_yolo.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.9.0/data/result/Image_text_areas.py` & `danila-lib-1.9.1/data/result/Image_text_areas.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.9.0/data/result/Rect.py` & `danila-lib-1.9.1/data/result/Rect.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.9.0/data/result/Text_area.py` & `danila-lib-1.9.1/data/result/Text_area.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.9.0/data/result/Yolo_label_rect.py` & `danila-lib-1.9.1/data/result/Yolo_label_rect.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.9.0/setup.py` & `danila-lib-1.9.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   with open('requirements.txt', 'r') as f:
     a = f.read()
   b = a.split()
   return b
 
 setup(
   name='danila-lib',
-  version='1.9.0',
+  version='1.9.1',
   author='arseniy_zhuck',
   author_email='arseniyzhuck@mail.ru',
   description='This is the module for detecting and classifying text on rama pictures',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://github.com/Arseniy-Zhuck/danila_lib',
   packages=find_packages(),
```

