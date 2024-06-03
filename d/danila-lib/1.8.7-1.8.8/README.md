# Comparing `tmp/danila-lib-1.8.7.tar.gz` & `tmp/danila-lib-1.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "danila-lib-1.8.7.tar", last modified: Sun Jun  2 10:32:23 2024, max compression
+gzip compressed data, was "danila-lib-1.8.8.tar", last modified: Mon Jun  3 10:16:57 2024, max compression
```

## Comparing `danila-lib-1.8.7.tar` & `danila-lib-1.8.8.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxrwxrwx   0        0        0        0 2024-06-02 10:32:23.305825 danila-lib-1.8.7/
--rw-rw-rw-   0        0        0     9615 2024-06-02 10:32:23.305825 danila-lib-1.8.7/PKG-INFO
--rw-rw-rw-   0        0        0     5060 2024-04-22 21:01:41.000000 danila-lib-1.8.7/README.md
-drwxrwxrwx   0        0        0        0 2024-06-02 10:32:22.877745 danila-lib-1.8.7/danila/
--rw-rw-rw-   0        0        0        0 2024-04-15 11:55:56.000000 danila-lib-1.8.7/danila/__init__.py
--rw-rw-rw-   0        0        0     2358 2024-06-02 09:51:55.000000 danila-lib-1.8.7/danila/danila.py
--rw-rw-rw-   0        0        0     9764 2024-05-22 08:43:39.000000 danila-lib-1.8.7/danila/danila_v1.py
--rw-rw-rw-   0        0        0    10182 2024-05-22 08:43:39.000000 danila-lib-1.8.7/danila/danila_v2.py
--rw-rw-rw-   0        0        0    10706 2024-05-22 08:43:39.000000 danila-lib-1.8.7/danila/danila_v3.py
--rw-rw-rw-   0        0        0    25557 2024-06-02 10:32:12.000000 danila-lib-1.8.7/danila/danila_v4.py
-drwxrwxrwx   0        0        0        0 2024-06-02 10:32:22.925535 danila-lib-1.8.7/danila_lib.egg-info/
--rw-rw-rw-   0        0        0     9615 2024-06-02 10:32:22.000000 danila-lib-1.8.7/danila_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      980 2024-06-02 10:32:22.000000 danila-lib-1.8.7/danila_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 10:32:22.000000 danila-lib-1.8.7/danila_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1879 2024-06-02 10:32:22.000000 danila-lib-1.8.7/danila_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-06-02 10:32:22.000000 danila-lib-1.8.7/danila_lib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-06-02 10:32:22.926526 danila-lib-1.8.7/data/
--rw-rw-rw-   0        0        0        0 2024-04-15 12:01:57.000000 danila-lib-1.8.7/data/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-02 10:32:23.153516 danila-lib-1.8.7/data/neuro/
--rw-rw-rw-   0        0        0     5722 2024-04-22 21:09:12.000000 danila-lib-1.8.7/data/neuro/Letters_recognize.py
--rw-rw-rw-   0        0        0     2754 2024-04-22 10:33:16.000000 danila-lib-1.8.7/data/neuro/Rama_classify_class.py
--rw-rw-rw-   0        0        0     2121 2024-05-22 08:48:35.000000 danila-lib-1.8.7/data/neuro/Rama_detect_class.py
--rw-rw-rw-   0        0        0     3000 2024-05-28 08:28:46.000000 danila-lib-1.8.7/data/neuro/Rama_prod_classify_class.py
--rw-rw-rw-   0        0        0     3153 2024-05-23 05:46:54.000000 danila-lib-1.8.7/data/neuro/Text_detect_class.py
--rw-rw-rw-   0        0        0     2643 2024-06-02 10:27:15.000000 danila-lib-1.8.7/data/neuro/Vagon_number_detect_class.py
--rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.8.7/data/neuro/__init__.py
--rw-rw-rw-   0        0        0     6695 2024-05-28 13:59:46.000000 danila-lib-1.8.7/data/neuro/letters_in_image.py
--rw-rw-rw-   0        0        0      959 2024-06-02 10:17:58.000000 danila-lib-1.8.7/data/neuro/models.py
--rw-rw-rw-   0        0        0     3222 2024-05-27 08:43:50.000000 danila-lib-1.8.7/data/neuro/objs_in_image.py
--rw-rw-rw-   0        0        0     4854 2024-05-28 13:59:46.000000 danila-lib-1.8.7/data/neuro/text_recognize_yolo.py
-drwxrwxrwx   0        0        0        0 2024-06-02 10:32:23.300848 danila-lib-1.8.7/data/result/
--rw-rw-rw-   0        0        0       89 2023-11-28 06:30:22.000000 danila-lib-1.8.7/data/result/Class_im.py
--rw-rw-rw-   0        0        0      108 2023-12-12 16:53:34.000000 danila-lib-1.8.7/data/result/Class_text.py
--rw-rw-rw-   0        0        0     2811 2024-04-22 19:35:07.000000 danila-lib-1.8.7/data/result/Image_text_areas.py
--rw-rw-rw-   0        0        0      332 2024-05-27 09:58:57.000000 danila-lib-1.8.7/data/result/Label_area.py
--rw-rw-rw-   0        0        0      236 2024-05-27 08:43:50.000000 danila-lib-1.8.7/data/result/Rama_prod.py
--rw-rw-rw-   0        0        0     3233 2024-04-22 18:17:45.000000 danila-lib-1.8.7/data/result/Rect.py
--rw-rw-rw-   0        0        0      539 2024-04-22 18:52:56.000000 danila-lib-1.8.7/data/result/Text_area.py
--rw-rw-rw-   0        0        0      716 2024-04-22 10:33:16.000000 danila-lib-1.8.7/data/result/Yolo_label_rect.py
--rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.8.7/data/result/__init__.py
--rw-rw-rw-   0        0        0      126 2024-05-14 11:04:15.000000 danila-lib-1.8.7/data/result/prod_classify_result.py
--rw-rw-rw-   0        0        0      122 2024-05-06 08:55:07.000000 danila-lib-1.8.7/data/result/word_compare_result.py
--rw-rw-rw-   0        0        0       42 2024-06-02 10:32:23.308812 danila-lib-1.8.7/setup.cfg
--rw-rw-rw-   0        0        0      983 2024-06-02 10:32:12.000000 danila-lib-1.8.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:16:57.683168 danila-lib-1.8.8/
+-rw-rw-rw-   0        0        0     9615 2024-06-03 10:16:57.682174 danila-lib-1.8.8/PKG-INFO
+-rw-rw-rw-   0        0        0     5060 2024-04-22 21:01:41.000000 danila-lib-1.8.8/README.md
+drwxrwxrwx   0        0        0        0 2024-06-03 10:16:56.896688 danila-lib-1.8.8/danila/
+-rw-rw-rw-   0        0        0        0 2024-04-15 11:55:56.000000 danila-lib-1.8.8/danila/__init__.py
+-rw-rw-rw-   0        0        0     2235 2024-06-03 10:16:44.000000 danila-lib-1.8.8/danila/danila.py
+-rw-rw-rw-   0        0        0     9764 2024-05-22 08:43:39.000000 danila-lib-1.8.8/danila/danila_v1.py
+-rw-rw-rw-   0        0        0    10182 2024-05-22 08:43:39.000000 danila-lib-1.8.8/danila/danila_v2.py
+-rw-rw-rw-   0        0        0    10706 2024-05-22 08:43:39.000000 danila-lib-1.8.8/danila/danila_v3.py
+-rw-rw-rw-   0        0        0    26797 2024-06-03 10:16:44.000000 danila-lib-1.8.8/danila/danila_v4.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:16:56.964387 danila-lib-1.8.8/danila_lib.egg-info/
+-rw-rw-rw-   0        0        0     9615 2024-06-03 10:16:56.000000 danila-lib-1.8.8/danila_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1023 2024-06-03 10:16:56.000000 danila-lib-1.8.8/danila_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 10:16:56.000000 danila-lib-1.8.8/danila_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1879 2024-06-03 10:16:56.000000 danila-lib-1.8.8/danila_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-06-03 10:16:56.000000 danila-lib-1.8.8/danila_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-03 10:16:56.965383 danila-lib-1.8.8/data/
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:01:57.000000 danila-lib-1.8.8/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:16:57.450211 danila-lib-1.8.8/data/neuro/
+-rw-rw-rw-   0        0        0     5722 2024-04-22 21:09:12.000000 danila-lib-1.8.8/data/neuro/Letters_recognize.py
+-rw-rw-rw-   0        0        0     2754 2024-04-22 10:33:16.000000 danila-lib-1.8.8/data/neuro/Rama_classify_class.py
+-rw-rw-rw-   0        0        0     2121 2024-05-22 08:48:35.000000 danila-lib-1.8.8/data/neuro/Rama_detect_class.py
+-rw-rw-rw-   0        0        0     3000 2024-05-28 08:28:46.000000 danila-lib-1.8.8/data/neuro/Rama_prod_classify_class.py
+-rw-rw-rw-   0        0        0     3153 2024-05-23 05:46:54.000000 danila-lib-1.8.8/data/neuro/Text_detect_class.py
+-rw-rw-rw-   0        0        0     2643 2024-06-02 10:27:15.000000 danila-lib-1.8.8/data/neuro/Vagon_number_detect_class.py
+-rw-rw-rw-   0        0        0     4279 2024-06-03 08:38:11.000000 danila-lib-1.8.8/data/neuro/Vagon_number_recognize_class.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.8.8/data/neuro/__init__.py
+-rw-rw-rw-   0        0        0     6695 2024-05-28 13:59:46.000000 danila-lib-1.8.8/data/neuro/letters_in_image.py
+-rw-rw-rw-   0        0        0      959 2024-06-02 10:17:58.000000 danila-lib-1.8.8/data/neuro/models.py
+-rw-rw-rw-   0        0        0     3222 2024-05-27 08:43:50.000000 danila-lib-1.8.8/data/neuro/objs_in_image.py
+-rw-rw-rw-   0        0        0     4854 2024-05-28 13:59:46.000000 danila-lib-1.8.8/data/neuro/text_recognize_yolo.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:16:57.677191 danila-lib-1.8.8/data/result/
+-rw-rw-rw-   0        0        0       89 2023-11-28 06:30:22.000000 danila-lib-1.8.8/data/result/Class_im.py
+-rw-rw-rw-   0        0        0      108 2023-12-12 16:53:34.000000 danila-lib-1.8.8/data/result/Class_text.py
+-rw-rw-rw-   0        0        0     2811 2024-04-22 19:35:07.000000 danila-lib-1.8.8/data/result/Image_text_areas.py
+-rw-rw-rw-   0        0        0      332 2024-05-27 09:58:57.000000 danila-lib-1.8.8/data/result/Label_area.py
+-rw-rw-rw-   0        0        0      236 2024-05-27 08:43:50.000000 danila-lib-1.8.8/data/result/Rama_prod.py
+-rw-rw-rw-   0        0        0     3233 2024-04-22 18:17:45.000000 danila-lib-1.8.8/data/result/Rect.py
+-rw-rw-rw-   0        0        0      539 2024-04-22 18:52:56.000000 danila-lib-1.8.8/data/result/Text_area.py
+-rw-rw-rw-   0        0        0      716 2024-04-22 10:33:16.000000 danila-lib-1.8.8/data/result/Yolo_label_rect.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.8.8/data/result/__init__.py
+-rw-rw-rw-   0        0        0      126 2024-05-14 11:04:15.000000 danila-lib-1.8.8/data/result/prod_classify_result.py
+-rw-rw-rw-   0        0        0      122 2024-05-06 08:55:07.000000 danila-lib-1.8.8/data/result/word_compare_result.py
+-rw-rw-rw-   0        0        0       42 2024-06-03 10:16:57.694115 danila-lib-1.8.8/setup.cfg
+-rw-rw-rw-   0        0        0      983 2024-06-03 10:16:44.000000 danila-lib-1.8.8/setup.py
```

### Comparing `danila-lib-1.8.7/PKG-INFO` & `danila-lib-1.8.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danila-lib
-Version: 1.8.7
+Version: 1.8.8
 Summary: This is the module for detecting and classifying text on rama pictures
 Home-page: https://github.com/Arseniy-Zhuck/danila_lib
 Author: arseniy_zhuck
 Author-email: arseniyzhuck@mail.ru
 Project-URL: GitHub, https://github.com/Arseniy-Zhuck/danila_lib
 Keywords: rama detect machine-learning computer-vision
 Classifier: Programming Language :: Python :: 3.11
@@ -57,16 +57,16 @@
 Requires-Dist: more-itertools==10.2.0
 Requires-Dist: mpmath==1.3.0
 Requires-Dist: networkx==3.2.1
 Requires-Dist: nh3==0.2.17
 Requires-Dist: ninja==1.11.1.1
 Requires-Dist: numpy==1.26.2
 Requires-Dist: oauthlib==3.2.2
-Requires-Dist: opencv-python==4.8.1.78
-Requires-Dist: opencv-python-headless==4.8.1.78
+Requires-Dist: opencv-python==4.9.0.80
+Requires-Dist: opencv-python-headless==4.9.0.80
 Requires-Dist: opt-einsum==3.3.0
 Requires-Dist: packaging==23.2
 Requires-Dist: pandas==2.1.4
 Requires-Dist: Pillow==10.3.0
 Requires-Dist: pkginfo==1.10.0
 Requires-Dist: protobuf==4.23.4
 Requires-Dist: psutil==5.9.6
```

### Comparing `danila-lib-1.8.7/README.md` & `danila-lib-1.8.8/README.md`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.7/danila/danila.py` & `danila-lib-1.8.8/danila/danila.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,52 +9,48 @@
 
 """main module for user"""
 
 
 class Danila:
     """main class for user"""
     def __init__(self, version, yolov5_dir):
-        if (version == 1):
-            self.danila = Danila_v1(yolov5_dir)
-        elif (version == 2):
-            self.danila = Danila_v2(yolov5_dir)
-        elif (version == 3):
-            self.danila = Danila_v3(yolov5_dir)
+        if (version == 4):
+            self.danila = Danila_v4(yolov5_dir)
         else:
             self.danila = Danila_v4(yolov5_dir)
     # returns string - class of rama using CNN network
     # img - openCV frame
 
     def rama_classify(self, img, size = 256):
         """rama_classify(Img : openCv frame): String - returns class of rama using CNN network"""
         """rama_classify uses Rama_classify_class method - classify(Img)"""
         return self.danila.rama_classify(img, size)
 
     # returns openCV frame with rama from openCV frame\
-    def rama_detect(self, img, size = 256):
-        """rama_detect(img : openCV img) -> openCV image with drawn rama rectangle"""
-        return self.danila.rama_detect(img, size)
-
-    # returns openCV image with cut_rama
-    def rama_cut(self, img, size = 256):
-        """rama_cut(img : openCV img) -> openCV image of rama rectangle"""
-        return self.danila.rama_cut(img, size)
+    # def rama_detect(self, img, size = 256):
+    #     """rama_detect(img : openCV img) -> openCV image with drawn rama rectangle"""
+    #     return self.danila.rama_detect(img, size)
+    #
+    # # returns openCV image with cut_rama
+    # def rama_cut(self, img, size = 256):
+    #     """rama_cut(img : openCV img) -> openCV image of rama rectangle"""
+    #     return self.danila.rama_cut(img, size)
 
     #
     # returns openCV cut rama with drawn text areas
     def rama_text_detect_cut(self, img, size = 256):
         """returns openCV cut rama with drawn text areas"""
-        return self.danila.text_detect_cut(img, size)
+        return self.danila.rama_text_detect_cut(img, size)
 
     # returns openCV img with drawn text areas
-    def rama_text_detect(self, img, size = 256):
-        """returns openCV img with drawn text areas"""
-        return self.danila.text_detect(img, size)
+    # def rama_text_detect(self, img, size = 256):
+    #     """returns openCV img with drawn text areas"""
+    #     return self.danila.text_detect(img, size)
     # returns dict {'number', 'prod', 'year'} for openCV rama img or 'no_rama'
     def rama_text_recognize(self, img, size = 256):
         """returns dict {'number', 'prod', 'year'} for openCV rama img or 'no_rama'"""
-        return self.danila.text_recognize(img, size)
+        return self.danila.rama_text_recognize(img, size)
 
     # returns openCV img with drawn number areas
     def vagon_number_detect(self, img, size = 256):
         """returns openCV img with drawn number areas"""
         return self.danila.vagon_number_detect(img, size)
```

### Comparing `danila-lib-1.8.7/danila/danila_v1.py` & `danila-lib-1.8.8/danila/danila_v1.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.7/danila/danila_v2.py` & `danila-lib-1.8.8/danila/danila_v2.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.7/danila/danila_v3.py` & `danila-lib-1.8.8/danila/danila_v3.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.7/danila/danila_v4.py` & `danila-lib-1.8.8/danila/danila_v4.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import cv2
 
 from data.neuro.Letters_recognize import Letters_recognize
 from data.neuro.Rama_detect_class import Rama_detect_class
 from data.neuro.Rama_prod_classify_class import Rama_prod_classify_class
 from data.neuro.Text_detect_class import Text_detect_class
 from data.neuro.Vagon_number_detect_class import Vagon_number_detect_class
+from data.neuro.Vagon_number_recognize_class import Vagon_number_recognize_class
 from data.neuro.models import *
 from data.result.Class_im import Class_im
 from data.result.Class_text import Class_text
 from data.result.Rama_prod import Rama_Prod
 from data.result.Rect import Rect
 
 """main module for user"""
@@ -60,15 +61,16 @@
         self.text_recognize_ruzhimmash_model = Text_Recognize_yolo(text_recognize_yolo_ruzhimmash_model_path, yolo_path)
         text_recognize_yolo_begickaya_model_path = TEXT_RECOGNIZE_BEGICKAYA_MODEL_ADDRESS
         print('reading and loading - TEXT_RECOGNIZE_BEGICKAYA_MODEL')
         self.text_recognize_begickaya_model = Text_Recognize_yolo(text_recognize_yolo_begickaya_model_path, yolo_path)
         vagon_number_detect_model_path = VAGON_NUMBER_DETECT_MODEL_ADDRESS
         print('reading and loading - VAGON_NUMBER_DETECT_MODEL')
         self.vagon_number_detect_model = Vagon_number_detect_class(vagon_number_detect_model_path, yolo_path)
-
+        print('loading - VAGON_NUMBER_RECOGNIZE_MODEL')
+        self.vagon_number_recognize_model = Vagon_number_recognize_class()
 
     # returns Rama_Prod_Conf - class of rama and confidence using CNN network
     # img - openCV frame
     def rama_classify(self, img, size = 256):
         """rama_classify(Img : openCv frame): String - returns class of rama using CNN network"""
         """rama_classify uses Rama_classify_class method - classify(Img)"""
         # img = cv2.imread(img_path)
@@ -85,87 +87,87 @@
                     detail1 = Text_recognize_result(detail_prod1)
                     if (detail1.detail.text != 'no_rama'):
                         detail = detail1
                         flag = False
         return detail
 
     # returns openCV frame with rama from openCV frame\
-    def rama_detect(self, img, size = 256):
-        """rama_detect(img : openCV img) -> openCV image with drawn rama rectangle"""
-        hash_object = hashlib.md5(bytes(str(datetime.now()), 'utf-8'))
-        hash_str = hash_object.hexdigest()
-        initial_image_path = 'initial_image' + hash_str + '.jpg'
-        cv2.imwrite(initial_image_path, img)
-        rama_prod_conf = self.rama_prod_classify_model.classify(img, size)
-        rama_prod = rama_prod_conf.rama_prod
-        if rama_prod == Rama_Prod.no_rama:
-            sizes = [256, 384, 512, 640]
-            flag = True
-            for s in sizes:
-                if flag:
-                    rama_prod_conf1 = self.rama_prod_classify_model.classify(img, s)
-                    rama_prod1 = rama_prod_conf1.rama_prod
-                    if (rama_prod1 != Rama_Prod.no_rama):
-                        rama_prod_conf = rama_prod_conf1
-                        rama_prod = rama_prod_conf.rama_prod
-                        flag = False
-            if flag:
-                os.remove(initial_image_path)
-                return img
-        rect = Rect()
-        if (rama_prod == Rama_Prod.ruzhimmash):
-            rect = self.rama_spring_detect_model.rama_detect(initial_image_path)
-        else:
-            rect = self.rama_no_spring_detect_model.rama_detect(initial_image_path)
-        new_img = img.copy()
-        os.remove(initial_image_path)
-        if rect is None:
-            os.remove(initial_image_path)
-            return img
-        cv2.rectangle(new_img, (rect.xmin, rect.ymin), (rect.xmax, rect.ymax), (0, 0, 255), 2)
-        cv2.putText(new_img, rama_prod.name, (rect.xmin, rect.ymin), cv2.FONT_HERSHEY_SIMPLEX, 0.5, (0,0,255), 2)
-        return new_img
+    # def rama_detect(self, img, size = 256):
+    #     """rama_detect(img : openCV img) -> openCV image with drawn rama rectangle"""
+    #     hash_object = hashlib.md5(bytes(str(datetime.now()), 'utf-8'))
+    #     hash_str = hash_object.hexdigest()
+    #     initial_image_path = 'initial_image' + hash_str + '.jpg'
+    #     cv2.imwrite(initial_image_path, img)
+    #     rama_prod_conf = self.rama_prod_classify_model.classify(img, size)
+    #     rama_prod = rama_prod_conf.rama_prod
+    #     if rama_prod == Rama_Prod.no_rama:
+    #         sizes = [256, 384, 512, 640]
+    #         flag = True
+    #         for s in sizes:
+    #             if flag:
+    #                 rama_prod_conf1 = self.rama_prod_classify_model.classify(img, s)
+    #                 rama_prod1 = rama_prod_conf1.rama_prod
+    #                 if (rama_prod1 != Rama_Prod.no_rama):
+    #                     rama_prod_conf = rama_prod_conf1
+    #                     rama_prod = rama_prod_conf.rama_prod
+    #                     flag = False
+    #         if flag:
+    #             os.remove(initial_image_path)
+    #             return img
+    #     rect = Rect()
+    #     if (rama_prod == Rama_Prod.ruzhimmash):
+    #         rect = self.rama_spring_detect_model.rama_detect(initial_image_path)
+    #     else:
+    #         rect = self.rama_no_spring_detect_model.rama_detect(initial_image_path)
+    #     new_img = img.copy()
+    #     os.remove(initial_image_path)
+    #     if rect is None:
+    #         os.remove(initial_image_path)
+    #         return img
+    #     cv2.rectangle(new_img, (rect.xmin, rect.ymin), (rect.xmax, rect.ymax), (0, 0, 255), 2)
+    #     cv2.putText(new_img, rama_prod.name, (rect.xmin, rect.ymin), cv2.FONT_HERSHEY_SIMPLEX, 0.5, (0,0,255), 2)
+    #     return new_img
 
     # returns openCV image with cut_rama
-    def rama_cut(self, img, size = 256):
-        """rama_cut(img : openCV img) -> openCV image of rama rectangle"""
-        hash_object = hashlib.md5(bytes(str(datetime.now()), 'utf-8'))
-        hash_str = hash_object.hexdigest()
-        initial_image_path = 'initial_image' + hash_str + '.jpg'
-        cv2.imwrite(initial_image_path, img)
-        rama_prod_conf = self.rama_prod_classify_model.classify(img, size)
-        rama_prod = rama_prod_conf.rama_prod
-        if rama_prod == Rama_Prod.no_rama:
-            sizes = [256, 384, 512, 640]
-            flag = True
-            for s in sizes:
-                if flag:
-                    rama_prod_conf1 = self.rama_prod_classify_model.classify(img, s)
-                    rama_prod1 = rama_prod_conf1.rama_prod
-                    if (rama_prod1 != Rama_Prod.no_rama):
-                        rama_prod_conf = rama_prod_conf1
-                        rama_prod = rama_prod_conf.rama_prod
-                        flag = False
-            if flag:
-                os.remove(initial_image_path)
-                return img
-        rect = Rect()
-        if (rama_prod == Rama_Prod.ruzhimmash):
-            rect = self.rama_spring_detect_model.rama_detect(initial_image_path)
-        else:
-            rect = self.rama_no_spring_detect_model.rama_detect(initial_image_path)
-        if rect is None:
-            os.remove(initial_image_path)
-            return img
-        img_res = img[rect.ymin:rect.ymax, rect.xmin:rect.xmax]
-        os.remove(initial_image_path)
-        return img_res
-    #
+    # def rama_cut(self, img, size = 256):
+    #     """rama_cut(img : openCV img) -> openCV image of rama rectangle"""
+    #     hash_object = hashlib.md5(bytes(str(datetime.now()), 'utf-8'))
+    #     hash_str = hash_object.hexdigest()
+    #     initial_image_path = 'initial_image' + hash_str + '.jpg'
+    #     cv2.imwrite(initial_image_path, img)
+    #     rama_prod_conf = self.rama_prod_classify_model.classify(img, size)
+    #     rama_prod = rama_prod_conf.rama_prod
+    #     if rama_prod == Rama_Prod.no_rama:
+    #         sizes = [256, 384, 512, 640]
+    #         flag = True
+    #         for s in sizes:
+    #             if flag:
+    #                 rama_prod_conf1 = self.rama_prod_classify_model.classify(img, s)
+    #                 rama_prod1 = rama_prod_conf1.rama_prod
+    #                 if (rama_prod1 != Rama_Prod.no_rama):
+    #                     rama_prod_conf = rama_prod_conf1
+    #                     rama_prod = rama_prod_conf.rama_prod
+    #                     flag = False
+    #         if flag:
+    #             os.remove(initial_image_path)
+    #             return img
+    #     rect = Rect()
+    #     if (rama_prod == Rama_Prod.ruzhimmash):
+    #         rect = self.rama_spring_detect_model.rama_detect(initial_image_path)
+    #     else:
+    #         rect = self.rama_no_spring_detect_model.rama_detect(initial_image_path)
+    #     if rect is None:
+    #         os.remove(initial_image_path)
+    #         return img
+    #     img_res = img[rect.ymin:rect.ymax, rect.xmin:rect.xmax]
+    #     os.remove(initial_image_path)
+    #     return img_res
+    # #
     # returns openCV cut rama with drawn text areas
-    def text_detect_cut(self, img, size = 256):
+    def rama_text_detect_cut(self, img, size = 256):
         """returns openCV cut rama with drawn text areas"""
         hash_object = hashlib.md5(bytes(str(datetime.now()), 'utf-8'))
         hash_str = hash_object.hexdigest()
         initial_image_path = 'initial_image' + hash_str + '.jpg'
         cv2.imwrite(initial_image_path, img)
         rama_prod_conf = self.rama_prod_classify_model.classify(img, size)
         rama_prod = rama_prod_conf.rama_prod
@@ -212,72 +214,72 @@
             image_text_areas = self.rama_no_spring_bejickaya_text_detect_model.text_detect(img_cut_path)
             image_drawn_text_areas = self.rama_no_spring_bejickaya_text_detect_model.draw_text_areas_in_opencv(image_text_areas, img_cut)
             os.remove(initial_image_path)
             os.remove(img_cut_path)
             return image_drawn_text_areas
 
     # returns openCV img with drawn text areas
-    def text_detect(self, img, size = 256):
-        """returns openCV img with drawn text areas"""
-        hash_object = hashlib.md5(bytes(str(datetime.now()), 'utf-8'))
-        hash_str = hash_object.hexdigest()
-        initial_image_path = 'initial_image' + hash_str + '.jpg'
-        cv2.imwrite(initial_image_path, img)
-        rama_prod_conf = self.rama_prod_classify_model.classify(img, size)
-        rama_prod = rama_prod_conf.rama_prod
-        if rama_prod == Rama_Prod.no_rama:
-            sizes = [256, 384, 512, 640]
-            flag = True
-            for s in sizes:
-                if flag:
-                    rama_prod_conf1 = self.rama_prod_classify_model.classify(img, s)
-                    rama_prod1 = rama_prod_conf1.rama_prod
-                    if (rama_prod1 != Rama_Prod.no_rama):
-                        rama_prod_conf = rama_prod_conf1
-                        rama_prod = rama_prod_conf.rama_prod
-                        flag = False
-            if flag:
-                os.remove(initial_image_path)
-                return img
-        rect = Rect()
-        if (rama_prod == Rama_Prod.ruzhimmash):
-            rect = self.rama_spring_detect_model.rama_detect(initial_image_path)
-            if rect is None:
-                os.remove(initial_image_path)
-                return img
-            img_cut = img[rect.ymin:rect.ymax, rect.xmin:rect.xmax]
-            hash_object = hashlib.md5(bytes(str(datetime.now()), 'utf-8'))
-            hash_str = hash_object.hexdigest()
-            img_cut_path = 'cut_img' + hash_str + '.jpg'
-            cv2.imwrite(img_cut_path, img_cut)
-            image_text_areas = self.rama_spring_ruzhimmash_text_detect_model.text_detect(img_cut_path)
-            image_text_areas.explore_to_whole_image(rect)
-            image_drawn_text_areas = self.rama_spring_ruzhimmash_text_detect_model.draw_text_areas_in_opencv(image_text_areas, img)
-            os.remove(initial_image_path)
-            os.remove(img_cut_path)
-            return image_drawn_text_areas
-        else:
-            rect = self.rama_no_spring_detect_model.rama_detect(initial_image_path)
-            if rect is None:
-                os.remove(initial_image_path)
-                return img
-            img_cut = img[rect.ymin:rect.ymax, rect.xmin:rect.xmax]
-            hash_object = hashlib.md5(bytes(str(datetime.now()), 'utf-8'))
-            hash_str = hash_object.hexdigest()
-            img_cut_path = 'cut_img' + hash_str + '.jpg'
-            cv2.imwrite(img_cut_path, img_cut)
-            image_text_areas = self.rama_no_spring_bejickaya_text_detect_model.text_detect(img_cut_path)
-            image_text_areas.explore_to_whole_image(rect)
-            image_drawn_text_areas = self.rama_no_spring_bejickaya_text_detect_model.draw_text_areas_in_opencv(image_text_areas, img)
-            os.remove(initial_image_path)
-            os.remove(img_cut_path)
-            return image_drawn_text_areas
+    # def text_detect(self, img, size = 256):
+    #     """returns openCV img with drawn text areas"""
+    #     hash_object = hashlib.md5(bytes(str(datetime.now()), 'utf-8'))
+    #     hash_str = hash_object.hexdigest()
+    #     initial_image_path = 'initial_image' + hash_str + '.jpg'
+    #     cv2.imwrite(initial_image_path, img)
+    #     rama_prod_conf = self.rama_prod_classify_model.classify(img, size)
+    #     rama_prod = rama_prod_conf.rama_prod
+    #     if rama_prod == Rama_Prod.no_rama:
+    #         sizes = [256, 384, 512, 640]
+    #         flag = True
+    #         for s in sizes:
+    #             if flag:
+    #                 rama_prod_conf1 = self.rama_prod_classify_model.classify(img, s)
+    #                 rama_prod1 = rama_prod_conf1.rama_prod
+    #                 if (rama_prod1 != Rama_Prod.no_rama):
+    #                     rama_prod_conf = rama_prod_conf1
+    #                     rama_prod = rama_prod_conf.rama_prod
+    #                     flag = False
+    #         if flag:
+    #             os.remove(initial_image_path)
+    #             return img
+    #     rect = Rect()
+    #     if (rama_prod == Rama_Prod.ruzhimmash):
+    #         rect = self.rama_spring_detect_model.rama_detect(initial_image_path)
+    #         if rect is None:
+    #             os.remove(initial_image_path)
+    #             return img
+    #         img_cut = img[rect.ymin:rect.ymax, rect.xmin:rect.xmax]
+    #         hash_object = hashlib.md5(bytes(str(datetime.now()), 'utf-8'))
+    #         hash_str = hash_object.hexdigest()
+    #         img_cut_path = 'cut_img' + hash_str + '.jpg'
+    #         cv2.imwrite(img_cut_path, img_cut)
+    #         image_text_areas = self.rama_spring_ruzhimmash_text_detect_model.text_detect(img_cut_path)
+    #         image_text_areas.explore_to_whole_image(rect)
+    #         image_drawn_text_areas = self.rama_spring_ruzhimmash_text_detect_model.draw_text_areas_in_opencv(image_text_areas, img)
+    #         os.remove(initial_image_path)
+    #         os.remove(img_cut_path)
+    #         return image_drawn_text_areas
+    #     else:
+    #         rect = self.rama_no_spring_detect_model.rama_detect(initial_image_path)
+    #         if rect is None:
+    #             os.remove(initial_image_path)
+    #             return img
+    #         img_cut = img[rect.ymin:rect.ymax, rect.xmin:rect.xmax]
+    #         hash_object = hashlib.md5(bytes(str(datetime.now()), 'utf-8'))
+    #         hash_str = hash_object.hexdigest()
+    #         img_cut_path = 'cut_img' + hash_str + '.jpg'
+    #         cv2.imwrite(img_cut_path, img_cut)
+    #         image_text_areas = self.rama_no_spring_bejickaya_text_detect_model.text_detect(img_cut_path)
+    #         image_text_areas.explore_to_whole_image(rect)
+    #         image_drawn_text_areas = self.rama_no_spring_bejickaya_text_detect_model.draw_text_areas_in_opencv(image_text_areas, img)
+    #         os.remove(initial_image_path)
+    #         os.remove(img_cut_path)
+    #         return image_drawn_text_areas
 
     # returns dict {'number', 'prod', 'year'} for openCV rama img or 'no_rama'
-    def text_recognize(self, img, size = 256):
+    def rama_text_recognize(self, img, size = 256):
         """returns dict {'number', 'prod', 'year'} for openCV rama img or 'no_rama'"""
         hash_object = hashlib.md5(bytes(str(datetime.now()), 'utf-8'))
         hash_str = hash_object.hexdigest()
         initial_image_path = 'initial_image' + hash_str + '.jpg'
         cv2.imwrite(initial_image_path, img)
         rama_prod_conf = self.rama_prod_classify_model.classify(img, size)
         rama_prod = rama_prod_conf.rama_prod
@@ -295,17 +297,16 @@
                     if (rama_prod1 != Rama_Prod.no_rama):
                         rama_prod_conf = rama_prod_conf1
                         rama_prod = rama_prod_conf.rama_prod
                         detail = detail1
                         detail_prod = detail_prod1
                         flag = False
             if flag:
-
                 os.remove(initial_image_path)
-                return img
+                return detail
         rect = Rect()
         detail.prod = Text_cut_recognize_result(rama_prod.name, rama_prod_conf.conf)
         if (rama_prod == Rama_Prod.ruzhimmash):
             rect = self.rama_spring_detect_model.rama_detect(initial_image_path)
             if rect is None:
                 os.remove(initial_image_path)
                 return detail
@@ -442,8 +443,22 @@
         if len(number_rects) == 0:
             os.remove(initial_image_path)
             return img
         img_with_number = img.copy()
         for number_rect in number_rects:
             cv2.rectangle(img_with_number, (number_rect.xmin, number_rect.ymin), (number_rect.xmax, number_rect.ymax), (0, 0, 255), 2)
             cv2.putText(img_with_number, 'number', (number_rect.xmin, number_rect.ymin), cv2.FONT_HERSHEY_SIMPLEX, 0.5, (0, 0, 255), 2)
-        return img_with_number
+        return img_with_number
+
+    def vagon_number_recognize(self, img, size = 256):
+        hash_object = hashlib.md5(bytes(str(datetime.now()), 'utf-8'))
+        hash_str = hash_object.hexdigest()
+        initial_image_path = 'initial_image' + hash_str + '.jpg'
+        cv2.imwrite(initial_image_path, img)
+        vagon_number_rects = self.vagon_number_detect_model.vagon_rama_detect(initial_image_path, size)
+        detail = Text_recognize_result(Text_cut_recognize_result('vagon',0.0))
+        if len(vagon_number_rects)==0:
+            detail.detail.text = 'no-vagon'
+            os.remove(initial_image_path)
+            return detail
+        detail.number.text, detail.number.conf = self.vagon_number_recognize_model.work_image(img,vagon_number_rects)
+        return detail
```

### Comparing `danila-lib-1.8.7/danila_lib.egg-info/PKG-INFO` & `danila-lib-1.8.8/danila_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danila-lib
-Version: 1.8.7
+Version: 1.8.8
 Summary: This is the module for detecting and classifying text on rama pictures
 Home-page: https://github.com/Arseniy-Zhuck/danila_lib
 Author: arseniy_zhuck
 Author-email: arseniyzhuck@mail.ru
 Project-URL: GitHub, https://github.com/Arseniy-Zhuck/danila_lib
 Keywords: rama detect machine-learning computer-vision
 Classifier: Programming Language :: Python :: 3.11
@@ -57,16 +57,16 @@
 Requires-Dist: more-itertools==10.2.0
 Requires-Dist: mpmath==1.3.0
 Requires-Dist: networkx==3.2.1
 Requires-Dist: nh3==0.2.17
 Requires-Dist: ninja==1.11.1.1
 Requires-Dist: numpy==1.26.2
 Requires-Dist: oauthlib==3.2.2
-Requires-Dist: opencv-python==4.8.1.78
-Requires-Dist: opencv-python-headless==4.8.1.78
+Requires-Dist: opencv-python==4.9.0.80
+Requires-Dist: opencv-python-headless==4.9.0.80
 Requires-Dist: opt-einsum==3.3.0
 Requires-Dist: packaging==23.2
 Requires-Dist: pandas==2.1.4
 Requires-Dist: Pillow==10.3.0
 Requires-Dist: pkginfo==1.10.0
 Requires-Dist: protobuf==4.23.4
 Requires-Dist: psutil==5.9.6
```

### Comparing `danila-lib-1.8.7/danila_lib.egg-info/SOURCES.txt` & `danila-lib-1.8.8/danila_lib.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 data/__init__.py
 data/neuro/Letters_recognize.py
 data/neuro/Rama_classify_class.py
 data/neuro/Rama_detect_class.py
 data/neuro/Rama_prod_classify_class.py
 data/neuro/Text_detect_class.py
 data/neuro/Vagon_number_detect_class.py
+data/neuro/Vagon_number_recognize_class.py
 data/neuro/__init__.py
 data/neuro/letters_in_image.py
 data/neuro/models.py
 data/neuro/objs_in_image.py
 data/neuro/text_recognize_yolo.py
 data/result/Class_im.py
 data/result/Class_text.py
```

### Comparing `danila-lib-1.8.7/danila_lib.egg-info/requires.txt` & `danila-lib-1.8.8/danila_lib.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -43,16 +43,16 @@
 more-itertools==10.2.0
 mpmath==1.3.0
 networkx==3.2.1
 nh3==0.2.17
 ninja==1.11.1.1
 numpy==1.26.2
 oauthlib==3.2.2
-opencv-python==4.8.1.78
-opencv-python-headless==4.8.1.78
+opencv-python==4.9.0.80
+opencv-python-headless==4.9.0.80
 opt-einsum==3.3.0
 packaging==23.2
 pandas==2.1.4
 Pillow==10.3.0
 pkginfo==1.10.0
 protobuf==4.23.4
 psutil==5.9.6
```

### Comparing `danila-lib-1.8.7/data/neuro/Letters_recognize.py` & `danila-lib-1.8.8/data/neuro/Letters_recognize.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.7/data/neuro/Rama_classify_class.py` & `danila-lib-1.8.8/data/neuro/Rama_classify_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.7/data/neuro/Rama_detect_class.py` & `danila-lib-1.8.8/data/neuro/Rama_detect_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.7/data/neuro/Rama_prod_classify_class.py` & `danila-lib-1.8.8/data/neuro/Rama_prod_classify_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.7/data/neuro/Text_detect_class.py` & `danila-lib-1.8.8/data/neuro/Text_detect_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.7/data/neuro/Vagon_number_detect_class.py` & `danila-lib-1.8.8/data/neuro/Vagon_number_detect_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.7/data/neuro/letters_in_image.py` & `danila-lib-1.8.8/data/neuro/letters_in_image.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.7/data/neuro/models.py` & `danila-lib-1.8.8/data/neuro/models.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.7/data/neuro/objs_in_image.py` & `danila-lib-1.8.8/data/neuro/objs_in_image.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.7/data/neuro/text_recognize_yolo.py` & `danila-lib-1.8.8/data/neuro/text_recognize_yolo.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.7/data/result/Image_text_areas.py` & `danila-lib-1.8.8/data/result/Image_text_areas.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.7/data/result/Rect.py` & `danila-lib-1.8.8/data/result/Rect.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.7/data/result/Text_area.py` & `danila-lib-1.8.8/data/result/Text_area.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.7/data/result/Yolo_label_rect.py` & `danila-lib-1.8.8/data/result/Yolo_label_rect.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.7/setup.py` & `danila-lib-1.8.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   with open('requirements.txt', 'r') as f:
     a = f.read()
   b = a.split()
   return b
 
 setup(
   name='danila-lib',
-  version='1.8.7',
+  version='1.8.8',
   author='arseniy_zhuck',
   author_email='arseniyzhuck@mail.ru',
   description='This is the module for detecting and classifying text on rama pictures',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://github.com/Arseniy-Zhuck/danila_lib',
   packages=find_packages(),
```

