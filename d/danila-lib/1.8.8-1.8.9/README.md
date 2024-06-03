# Comparing `tmp/danila-lib-1.8.8.tar.gz` & `tmp/danila-lib-1.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "danila-lib-1.8.8.tar", last modified: Mon Jun  3 10:16:57 2024, max compression
+gzip compressed data, was "danila-lib-1.8.9.tar", last modified: Mon Jun  3 10:26:38 2024, max compression
```

## Comparing `danila-lib-1.8.8.tar` & `danila-lib-1.8.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2024-06-03 10:16:57.683168 danila-lib-1.8.8/
--rw-rw-rw-   0        0        0     9615 2024-06-03 10:16:57.682174 danila-lib-1.8.8/PKG-INFO
--rw-rw-rw-   0        0        0     5060 2024-04-22 21:01:41.000000 danila-lib-1.8.8/README.md
-drwxrwxrwx   0        0        0        0 2024-06-03 10:16:56.896688 danila-lib-1.8.8/danila/
--rw-rw-rw-   0        0        0        0 2024-04-15 11:55:56.000000 danila-lib-1.8.8/danila/__init__.py
--rw-rw-rw-   0        0        0     2235 2024-06-03 10:16:44.000000 danila-lib-1.8.8/danila/danila.py
--rw-rw-rw-   0        0        0     9764 2024-05-22 08:43:39.000000 danila-lib-1.8.8/danila/danila_v1.py
--rw-rw-rw-   0        0        0    10182 2024-05-22 08:43:39.000000 danila-lib-1.8.8/danila/danila_v2.py
--rw-rw-rw-   0        0        0    10706 2024-05-22 08:43:39.000000 danila-lib-1.8.8/danila/danila_v3.py
--rw-rw-rw-   0        0        0    26797 2024-06-03 10:16:44.000000 danila-lib-1.8.8/danila/danila_v4.py
-drwxrwxrwx   0        0        0        0 2024-06-03 10:16:56.964387 danila-lib-1.8.8/danila_lib.egg-info/
--rw-rw-rw-   0        0        0     9615 2024-06-03 10:16:56.000000 danila-lib-1.8.8/danila_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1023 2024-06-03 10:16:56.000000 danila-lib-1.8.8/danila_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-03 10:16:56.000000 danila-lib-1.8.8/danila_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1879 2024-06-03 10:16:56.000000 danila-lib-1.8.8/danila_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-06-03 10:16:56.000000 danila-lib-1.8.8/danila_lib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-06-03 10:16:56.965383 danila-lib-1.8.8/data/
--rw-rw-rw-   0        0        0        0 2024-04-15 12:01:57.000000 danila-lib-1.8.8/data/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-03 10:16:57.450211 danila-lib-1.8.8/data/neuro/
--rw-rw-rw-   0        0        0     5722 2024-04-22 21:09:12.000000 danila-lib-1.8.8/data/neuro/Letters_recognize.py
--rw-rw-rw-   0        0        0     2754 2024-04-22 10:33:16.000000 danila-lib-1.8.8/data/neuro/Rama_classify_class.py
--rw-rw-rw-   0        0        0     2121 2024-05-22 08:48:35.000000 danila-lib-1.8.8/data/neuro/Rama_detect_class.py
--rw-rw-rw-   0        0        0     3000 2024-05-28 08:28:46.000000 danila-lib-1.8.8/data/neuro/Rama_prod_classify_class.py
--rw-rw-rw-   0        0        0     3153 2024-05-23 05:46:54.000000 danila-lib-1.8.8/data/neuro/Text_detect_class.py
--rw-rw-rw-   0        0        0     2643 2024-06-02 10:27:15.000000 danila-lib-1.8.8/data/neuro/Vagon_number_detect_class.py
--rw-rw-rw-   0        0        0     4279 2024-06-03 08:38:11.000000 danila-lib-1.8.8/data/neuro/Vagon_number_recognize_class.py
--rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.8.8/data/neuro/__init__.py
--rw-rw-rw-   0        0        0     6695 2024-05-28 13:59:46.000000 danila-lib-1.8.8/data/neuro/letters_in_image.py
--rw-rw-rw-   0        0        0      959 2024-06-02 10:17:58.000000 danila-lib-1.8.8/data/neuro/models.py
--rw-rw-rw-   0        0        0     3222 2024-05-27 08:43:50.000000 danila-lib-1.8.8/data/neuro/objs_in_image.py
--rw-rw-rw-   0        0        0     4854 2024-05-28 13:59:46.000000 danila-lib-1.8.8/data/neuro/text_recognize_yolo.py
-drwxrwxrwx   0        0        0        0 2024-06-03 10:16:57.677191 danila-lib-1.8.8/data/result/
--rw-rw-rw-   0        0        0       89 2023-11-28 06:30:22.000000 danila-lib-1.8.8/data/result/Class_im.py
--rw-rw-rw-   0        0        0      108 2023-12-12 16:53:34.000000 danila-lib-1.8.8/data/result/Class_text.py
--rw-rw-rw-   0        0        0     2811 2024-04-22 19:35:07.000000 danila-lib-1.8.8/data/result/Image_text_areas.py
--rw-rw-rw-   0        0        0      332 2024-05-27 09:58:57.000000 danila-lib-1.8.8/data/result/Label_area.py
--rw-rw-rw-   0        0        0      236 2024-05-27 08:43:50.000000 danila-lib-1.8.8/data/result/Rama_prod.py
--rw-rw-rw-   0        0        0     3233 2024-04-22 18:17:45.000000 danila-lib-1.8.8/data/result/Rect.py
--rw-rw-rw-   0        0        0      539 2024-04-22 18:52:56.000000 danila-lib-1.8.8/data/result/Text_area.py
--rw-rw-rw-   0        0        0      716 2024-04-22 10:33:16.000000 danila-lib-1.8.8/data/result/Yolo_label_rect.py
--rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.8.8/data/result/__init__.py
--rw-rw-rw-   0        0        0      126 2024-05-14 11:04:15.000000 danila-lib-1.8.8/data/result/prod_classify_result.py
--rw-rw-rw-   0        0        0      122 2024-05-06 08:55:07.000000 danila-lib-1.8.8/data/result/word_compare_result.py
--rw-rw-rw-   0        0        0       42 2024-06-03 10:16:57.694115 danila-lib-1.8.8/setup.cfg
--rw-rw-rw-   0        0        0      983 2024-06-03 10:16:44.000000 danila-lib-1.8.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:26:38.845033 danila-lib-1.8.9/
+-rw-rw-rw-   0        0        0     9615 2024-06-03 10:26:38.845033 danila-lib-1.8.9/PKG-INFO
+-rw-rw-rw-   0        0        0     5060 2024-04-22 21:01:41.000000 danila-lib-1.8.9/README.md
+drwxrwxrwx   0        0        0        0 2024-06-03 10:26:38.440845 danila-lib-1.8.9/danila/
+-rw-rw-rw-   0        0        0        0 2024-04-15 11:55:56.000000 danila-lib-1.8.9/danila/__init__.py
+-rw-rw-rw-   0        0        0     2354 2024-06-03 10:26:25.000000 danila-lib-1.8.9/danila/danila.py
+-rw-rw-rw-   0        0        0     9764 2024-05-22 08:43:39.000000 danila-lib-1.8.9/danila/danila_v1.py
+-rw-rw-rw-   0        0        0    10182 2024-05-22 08:43:39.000000 danila-lib-1.8.9/danila/danila_v2.py
+-rw-rw-rw-   0        0        0    10706 2024-05-22 08:43:39.000000 danila-lib-1.8.9/danila/danila_v3.py
+-rw-rw-rw-   0        0        0    26888 2024-06-03 10:26:25.000000 danila-lib-1.8.9/danila/danila_v4.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:26:38.638962 danila-lib-1.8.9/danila_lib.egg-info/
+-rw-rw-rw-   0        0        0     9615 2024-06-03 10:26:38.000000 danila-lib-1.8.9/danila_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1023 2024-06-03 10:26:38.000000 danila-lib-1.8.9/danila_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 10:26:38.000000 danila-lib-1.8.9/danila_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1879 2024-06-03 10:26:38.000000 danila-lib-1.8.9/danila_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-06-03 10:26:38.000000 danila-lib-1.8.9/danila_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-03 10:26:38.682763 danila-lib-1.8.9/data/
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:01:57.000000 danila-lib-1.8.9/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:26:38.778334 danila-lib-1.8.9/data/neuro/
+-rw-rw-rw-   0        0        0     5722 2024-04-22 21:09:12.000000 danila-lib-1.8.9/data/neuro/Letters_recognize.py
+-rw-rw-rw-   0        0        0     2754 2024-04-22 10:33:16.000000 danila-lib-1.8.9/data/neuro/Rama_classify_class.py
+-rw-rw-rw-   0        0        0     2121 2024-05-22 08:48:35.000000 danila-lib-1.8.9/data/neuro/Rama_detect_class.py
+-rw-rw-rw-   0        0        0     3000 2024-05-28 08:28:46.000000 danila-lib-1.8.9/data/neuro/Rama_prod_classify_class.py
+-rw-rw-rw-   0        0        0     3153 2024-05-23 05:46:54.000000 danila-lib-1.8.9/data/neuro/Text_detect_class.py
+-rw-rw-rw-   0        0        0     2643 2024-06-02 10:27:15.000000 danila-lib-1.8.9/data/neuro/Vagon_number_detect_class.py
+-rw-rw-rw-   0        0        0     4279 2024-06-03 08:38:11.000000 danila-lib-1.8.9/data/neuro/Vagon_number_recognize_class.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.8.9/data/neuro/__init__.py
+-rw-rw-rw-   0        0        0     6695 2024-05-28 13:59:46.000000 danila-lib-1.8.9/data/neuro/letters_in_image.py
+-rw-rw-rw-   0        0        0      959 2024-06-02 10:17:58.000000 danila-lib-1.8.9/data/neuro/models.py
+-rw-rw-rw-   0        0        0     3222 2024-05-27 08:43:50.000000 danila-lib-1.8.9/data/neuro/objs_in_image.py
+-rw-rw-rw-   0        0        0     4854 2024-05-28 13:59:46.000000 danila-lib-1.8.9/data/neuro/text_recognize_yolo.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:26:38.842047 danila-lib-1.8.9/data/result/
+-rw-rw-rw-   0        0        0       89 2023-11-28 06:30:22.000000 danila-lib-1.8.9/data/result/Class_im.py
+-rw-rw-rw-   0        0        0      108 2023-12-12 16:53:34.000000 danila-lib-1.8.9/data/result/Class_text.py
+-rw-rw-rw-   0        0        0     2811 2024-04-22 19:35:07.000000 danila-lib-1.8.9/data/result/Image_text_areas.py
+-rw-rw-rw-   0        0        0      332 2024-05-27 09:58:57.000000 danila-lib-1.8.9/data/result/Label_area.py
+-rw-rw-rw-   0        0        0      236 2024-05-27 08:43:50.000000 danila-lib-1.8.9/data/result/Rama_prod.py
+-rw-rw-rw-   0        0        0     3233 2024-04-22 18:17:45.000000 danila-lib-1.8.9/data/result/Rect.py
+-rw-rw-rw-   0        0        0      539 2024-04-22 18:52:56.000000 danila-lib-1.8.9/data/result/Text_area.py
+-rw-rw-rw-   0        0        0      716 2024-04-22 10:33:16.000000 danila-lib-1.8.9/data/result/Yolo_label_rect.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.8.9/data/result/__init__.py
+-rw-rw-rw-   0        0        0      126 2024-05-14 11:04:15.000000 danila-lib-1.8.9/data/result/prod_classify_result.py
+-rw-rw-rw-   0        0        0      122 2024-05-06 08:55:07.000000 danila-lib-1.8.9/data/result/word_compare_result.py
+-rw-rw-rw-   0        0        0       42 2024-06-03 10:26:38.858972 danila-lib-1.8.9/setup.cfg
+-rw-rw-rw-   0        0        0      983 2024-06-03 10:26:25.000000 danila-lib-1.8.9/setup.py
```

### Comparing `danila-lib-1.8.8/PKG-INFO` & `danila-lib-1.8.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danila-lib
-Version: 1.8.8
+Version: 1.8.9
 Summary: This is the module for detecting and classifying text on rama pictures
 Home-page: https://github.com/Arseniy-Zhuck/danila_lib
 Author: arseniy_zhuck
 Author-email: arseniyzhuck@mail.ru
 Project-URL: GitHub, https://github.com/Arseniy-Zhuck/danila_lib
 Keywords: rama detect machine-learning computer-vision
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `danila-lib-1.8.8/README.md` & `danila-lib-1.8.9/README.md`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.8/danila/danila.py` & `danila-lib-1.8.9/danila/danila.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,8 +49,11 @@
     def rama_text_recognize(self, img, size = 256):
         """returns dict {'number', 'prod', 'year'} for openCV rama img or 'no_rama'"""
         return self.danila.rama_text_recognize(img, size)
 
     # returns openCV img with drawn number areas
     def vagon_number_detect(self, img, size = 256):
         """returns openCV img with drawn number areas"""
-        return self.danila.vagon_number_detect(img, size)
+        return self.danila.vagon_number_detect(img, size)
+
+    def vagon_number_recognize(self, img, size = 256):
+        return self.danila.vagon_number_recognize(img,size)
```

### Comparing `danila-lib-1.8.8/danila/danila_v1.py` & `danila-lib-1.8.9/danila/danila_v1.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.8/danila/danila_v2.py` & `danila-lib-1.8.9/danila/danila_v2.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.8/danila/danila_v3.py` & `danila-lib-1.8.9/danila/danila_v3.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.8/danila/danila_v4.py` & `danila-lib-1.8.9/danila/danila_v4.py`

 * *Files 0% similar despite different names*

```diff
@@ -456,9 +456,10 @@
         cv2.imwrite(initial_image_path, img)
         vagon_number_rects = self.vagon_number_detect_model.vagon_rama_detect(initial_image_path, size)
         detail = Text_recognize_result(Text_cut_recognize_result('vagon',0.0))
         if len(vagon_number_rects)==0:
             detail.detail.text = 'no-vagon'
             os.remove(initial_image_path)
             return detail
-        detail.number.text, detail.number.conf = self.vagon_number_recognize_model.work_image(img,vagon_number_rects)
+        detail_number_text, detail_number_conf = self.vagon_number_recognize_model.work_image(img,vagon_number_rects)
+        detail.number = Text_cut_recognize_result(detail_number_text, detail_number_conf)
         return detail
```

### Comparing `danila-lib-1.8.8/danila_lib.egg-info/PKG-INFO` & `danila-lib-1.8.9/danila_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danila-lib
-Version: 1.8.8
+Version: 1.8.9
 Summary: This is the module for detecting and classifying text on rama pictures
 Home-page: https://github.com/Arseniy-Zhuck/danila_lib
 Author: arseniy_zhuck
 Author-email: arseniyzhuck@mail.ru
 Project-URL: GitHub, https://github.com/Arseniy-Zhuck/danila_lib
 Keywords: rama detect machine-learning computer-vision
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `danila-lib-1.8.8/danila_lib.egg-info/SOURCES.txt` & `danila-lib-1.8.9/danila_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.8/danila_lib.egg-info/requires.txt` & `danila-lib-1.8.9/danila_lib.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.8/data/neuro/Letters_recognize.py` & `danila-lib-1.8.9/data/neuro/Letters_recognize.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.8/data/neuro/Rama_classify_class.py` & `danila-lib-1.8.9/data/neuro/Rama_classify_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.8/data/neuro/Rama_detect_class.py` & `danila-lib-1.8.9/data/neuro/Rama_detect_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.8/data/neuro/Rama_prod_classify_class.py` & `danila-lib-1.8.9/data/neuro/Rama_prod_classify_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.8/data/neuro/Text_detect_class.py` & `danila-lib-1.8.9/data/neuro/Text_detect_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.8/data/neuro/Vagon_number_detect_class.py` & `danila-lib-1.8.9/data/neuro/Vagon_number_detect_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.8/data/neuro/Vagon_number_recognize_class.py` & `danila-lib-1.8.9/data/neuro/Vagon_number_recognize_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.8/data/neuro/letters_in_image.py` & `danila-lib-1.8.9/data/neuro/letters_in_image.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.8/data/neuro/models.py` & `danila-lib-1.8.9/data/neuro/models.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.8/data/neuro/objs_in_image.py` & `danila-lib-1.8.9/data/neuro/objs_in_image.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.8/data/neuro/text_recognize_yolo.py` & `danila-lib-1.8.9/data/neuro/text_recognize_yolo.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.8/data/result/Image_text_areas.py` & `danila-lib-1.8.9/data/result/Image_text_areas.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.8/data/result/Rect.py` & `danila-lib-1.8.9/data/result/Rect.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.8/data/result/Text_area.py` & `danila-lib-1.8.9/data/result/Text_area.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.8/data/result/Yolo_label_rect.py` & `danila-lib-1.8.9/data/result/Yolo_label_rect.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.8/setup.py` & `danila-lib-1.8.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   with open('requirements.txt', 'r') as f:
     a = f.read()
   b = a.split()
   return b
 
 setup(
   name='danila-lib',
-  version='1.8.8',
+  version='1.8.9',
   author='arseniy_zhuck',
   author_email='arseniyzhuck@mail.ru',
   description='This is the module for detecting and classifying text on rama pictures',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://github.com/Arseniy-Zhuck/danila_lib',
   packages=find_packages(),
```

