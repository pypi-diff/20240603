# Comparing `tmp/danila-lib-1.8.6.tar.gz` & `tmp/danila-lib-1.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "danila-lib-1.8.6.tar", last modified: Sun Jun  2 10:27:20 2024, max compression
+gzip compressed data, was "danila-lib-1.8.7.tar", last modified: Sun Jun  2 10:32:23 2024, max compression
```

## Comparing `danila-lib-1.8.6.tar` & `danila-lib-1.8.7.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-06-02 10:27:20.303128 danila-lib-1.8.6/
--rw-rw-rw-   0        0        0     9615 2024-06-02 10:27:20.303128 danila-lib-1.8.6/PKG-INFO
--rw-rw-rw-   0        0        0     5060 2024-04-22 21:01:41.000000 danila-lib-1.8.6/README.md
-drwxrwxrwx   0        0        0        0 2024-06-02 10:27:20.164750 danila-lib-1.8.6/danila/
--rw-rw-rw-   0        0        0        0 2024-04-15 11:55:56.000000 danila-lib-1.8.6/danila/__init__.py
--rw-rw-rw-   0        0        0     2358 2024-06-02 09:51:55.000000 danila-lib-1.8.6/danila/danila.py
--rw-rw-rw-   0        0        0     9764 2024-05-22 08:43:39.000000 danila-lib-1.8.6/danila/danila_v1.py
--rw-rw-rw-   0        0        0    10182 2024-05-22 08:43:39.000000 danila-lib-1.8.6/danila/danila_v2.py
--rw-rw-rw-   0        0        0    10706 2024-05-22 08:43:39.000000 danila-lib-1.8.6/danila/danila_v3.py
--rw-rw-rw-   0        0        0    25555 2024-06-02 10:17:58.000000 danila-lib-1.8.6/danila/danila_v4.py
-drwxrwxrwx   0        0        0        0 2024-06-02 10:27:20.247384 danila-lib-1.8.6/danila_lib.egg-info/
--rw-rw-rw-   0        0        0     9615 2024-06-02 10:27:19.000000 danila-lib-1.8.6/danila_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      980 2024-06-02 10:27:19.000000 danila-lib-1.8.6/danila_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 10:27:19.000000 danila-lib-1.8.6/danila_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1879 2024-06-02 10:27:19.000000 danila-lib-1.8.6/danila_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-06-02 10:27:19.000000 danila-lib-1.8.6/danila_lib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-06-02 10:27:20.249367 danila-lib-1.8.6/data/
--rw-rw-rw-   0        0        0        0 2024-04-15 12:01:57.000000 danila-lib-1.8.6/data/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-02 10:27:20.293173 danila-lib-1.8.6/data/neuro/
--rw-rw-rw-   0        0        0     5722 2024-04-22 21:09:12.000000 danila-lib-1.8.6/data/neuro/Letters_recognize.py
--rw-rw-rw-   0        0        0     2754 2024-04-22 10:33:16.000000 danila-lib-1.8.6/data/neuro/Rama_classify_class.py
--rw-rw-rw-   0        0        0     2121 2024-05-22 08:48:35.000000 danila-lib-1.8.6/data/neuro/Rama_detect_class.py
--rw-rw-rw-   0        0        0     3000 2024-05-28 08:28:46.000000 danila-lib-1.8.6/data/neuro/Rama_prod_classify_class.py
--rw-rw-rw-   0        0        0     3153 2024-05-23 05:46:54.000000 danila-lib-1.8.6/data/neuro/Text_detect_class.py
--rw-rw-rw-   0        0        0     2643 2024-06-02 10:27:15.000000 danila-lib-1.8.6/data/neuro/Vagon_number_detect_class.py
--rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.8.6/data/neuro/__init__.py
--rw-rw-rw-   0        0        0     6695 2024-05-28 13:59:46.000000 danila-lib-1.8.6/data/neuro/letters_in_image.py
--rw-rw-rw-   0        0        0      959 2024-06-02 10:17:58.000000 danila-lib-1.8.6/data/neuro/models.py
--rw-rw-rw-   0        0        0     3222 2024-05-27 08:43:50.000000 danila-lib-1.8.6/data/neuro/objs_in_image.py
--rw-rw-rw-   0        0        0     4854 2024-05-28 13:59:46.000000 danila-lib-1.8.6/data/neuro/text_recognize_yolo.py
-drwxrwxrwx   0        0        0        0 2024-06-02 10:27:20.302132 danila-lib-1.8.6/data/result/
--rw-rw-rw-   0        0        0       89 2023-11-28 06:30:22.000000 danila-lib-1.8.6/data/result/Class_im.py
--rw-rw-rw-   0        0        0      108 2023-12-12 16:53:34.000000 danila-lib-1.8.6/data/result/Class_text.py
--rw-rw-rw-   0        0        0     2811 2024-04-22 19:35:07.000000 danila-lib-1.8.6/data/result/Image_text_areas.py
--rw-rw-rw-   0        0        0      332 2024-05-27 09:58:57.000000 danila-lib-1.8.6/data/result/Label_area.py
--rw-rw-rw-   0        0        0      236 2024-05-27 08:43:50.000000 danila-lib-1.8.6/data/result/Rama_prod.py
--rw-rw-rw-   0        0        0     3233 2024-04-22 18:17:45.000000 danila-lib-1.8.6/data/result/Rect.py
--rw-rw-rw-   0        0        0      539 2024-04-22 18:52:56.000000 danila-lib-1.8.6/data/result/Text_area.py
--rw-rw-rw-   0        0        0      716 2024-04-22 10:33:16.000000 danila-lib-1.8.6/data/result/Yolo_label_rect.py
--rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.8.6/data/result/__init__.py
--rw-rw-rw-   0        0        0      126 2024-05-14 11:04:15.000000 danila-lib-1.8.6/data/result/prod_classify_result.py
--rw-rw-rw-   0        0        0      122 2024-05-06 08:55:07.000000 danila-lib-1.8.6/data/result/word_compare_result.py
--rw-rw-rw-   0        0        0       42 2024-06-02 10:27:20.305120 danila-lib-1.8.6/setup.cfg
--rw-rw-rw-   0        0        0      983 2024-06-02 10:27:15.000000 danila-lib-1.8.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 10:32:23.305825 danila-lib-1.8.7/
+-rw-rw-rw-   0        0        0     9615 2024-06-02 10:32:23.305825 danila-lib-1.8.7/PKG-INFO
+-rw-rw-rw-   0        0        0     5060 2024-04-22 21:01:41.000000 danila-lib-1.8.7/README.md
+drwxrwxrwx   0        0        0        0 2024-06-02 10:32:22.877745 danila-lib-1.8.7/danila/
+-rw-rw-rw-   0        0        0        0 2024-04-15 11:55:56.000000 danila-lib-1.8.7/danila/__init__.py
+-rw-rw-rw-   0        0        0     2358 2024-06-02 09:51:55.000000 danila-lib-1.8.7/danila/danila.py
+-rw-rw-rw-   0        0        0     9764 2024-05-22 08:43:39.000000 danila-lib-1.8.7/danila/danila_v1.py
+-rw-rw-rw-   0        0        0    10182 2024-05-22 08:43:39.000000 danila-lib-1.8.7/danila/danila_v2.py
+-rw-rw-rw-   0        0        0    10706 2024-05-22 08:43:39.000000 danila-lib-1.8.7/danila/danila_v3.py
+-rw-rw-rw-   0        0        0    25557 2024-06-02 10:32:12.000000 danila-lib-1.8.7/danila/danila_v4.py
+drwxrwxrwx   0        0        0        0 2024-06-02 10:32:22.925535 danila-lib-1.8.7/danila_lib.egg-info/
+-rw-rw-rw-   0        0        0     9615 2024-06-02 10:32:22.000000 danila-lib-1.8.7/danila_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      980 2024-06-02 10:32:22.000000 danila-lib-1.8.7/danila_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 10:32:22.000000 danila-lib-1.8.7/danila_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1879 2024-06-02 10:32:22.000000 danila-lib-1.8.7/danila_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-06-02 10:32:22.000000 danila-lib-1.8.7/danila_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-02 10:32:22.926526 danila-lib-1.8.7/data/
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:01:57.000000 danila-lib-1.8.7/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-02 10:32:23.153516 danila-lib-1.8.7/data/neuro/
+-rw-rw-rw-   0        0        0     5722 2024-04-22 21:09:12.000000 danila-lib-1.8.7/data/neuro/Letters_recognize.py
+-rw-rw-rw-   0        0        0     2754 2024-04-22 10:33:16.000000 danila-lib-1.8.7/data/neuro/Rama_classify_class.py
+-rw-rw-rw-   0        0        0     2121 2024-05-22 08:48:35.000000 danila-lib-1.8.7/data/neuro/Rama_detect_class.py
+-rw-rw-rw-   0        0        0     3000 2024-05-28 08:28:46.000000 danila-lib-1.8.7/data/neuro/Rama_prod_classify_class.py
+-rw-rw-rw-   0        0        0     3153 2024-05-23 05:46:54.000000 danila-lib-1.8.7/data/neuro/Text_detect_class.py
+-rw-rw-rw-   0        0        0     2643 2024-06-02 10:27:15.000000 danila-lib-1.8.7/data/neuro/Vagon_number_detect_class.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.8.7/data/neuro/__init__.py
+-rw-rw-rw-   0        0        0     6695 2024-05-28 13:59:46.000000 danila-lib-1.8.7/data/neuro/letters_in_image.py
+-rw-rw-rw-   0        0        0      959 2024-06-02 10:17:58.000000 danila-lib-1.8.7/data/neuro/models.py
+-rw-rw-rw-   0        0        0     3222 2024-05-27 08:43:50.000000 danila-lib-1.8.7/data/neuro/objs_in_image.py
+-rw-rw-rw-   0        0        0     4854 2024-05-28 13:59:46.000000 danila-lib-1.8.7/data/neuro/text_recognize_yolo.py
+drwxrwxrwx   0        0        0        0 2024-06-02 10:32:23.300848 danila-lib-1.8.7/data/result/
+-rw-rw-rw-   0        0        0       89 2023-11-28 06:30:22.000000 danila-lib-1.8.7/data/result/Class_im.py
+-rw-rw-rw-   0        0        0      108 2023-12-12 16:53:34.000000 danila-lib-1.8.7/data/result/Class_text.py
+-rw-rw-rw-   0        0        0     2811 2024-04-22 19:35:07.000000 danila-lib-1.8.7/data/result/Image_text_areas.py
+-rw-rw-rw-   0        0        0      332 2024-05-27 09:58:57.000000 danila-lib-1.8.7/data/result/Label_area.py
+-rw-rw-rw-   0        0        0      236 2024-05-27 08:43:50.000000 danila-lib-1.8.7/data/result/Rama_prod.py
+-rw-rw-rw-   0        0        0     3233 2024-04-22 18:17:45.000000 danila-lib-1.8.7/data/result/Rect.py
+-rw-rw-rw-   0        0        0      539 2024-04-22 18:52:56.000000 danila-lib-1.8.7/data/result/Text_area.py
+-rw-rw-rw-   0        0        0      716 2024-04-22 10:33:16.000000 danila-lib-1.8.7/data/result/Yolo_label_rect.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.8.7/data/result/__init__.py
+-rw-rw-rw-   0        0        0      126 2024-05-14 11:04:15.000000 danila-lib-1.8.7/data/result/prod_classify_result.py
+-rw-rw-rw-   0        0        0      122 2024-05-06 08:55:07.000000 danila-lib-1.8.7/data/result/word_compare_result.py
+-rw-rw-rw-   0        0        0       42 2024-06-02 10:32:23.308812 danila-lib-1.8.7/setup.cfg
+-rw-rw-rw-   0        0        0      983 2024-06-02 10:32:12.000000 danila-lib-1.8.7/setup.py
```

### Comparing `danila-lib-1.8.6/PKG-INFO` & `danila-lib-1.8.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danila-lib
-Version: 1.8.6
+Version: 1.8.7
 Summary: This is the module for detecting and classifying text on rama pictures
 Home-page: https://github.com/Arseniy-Zhuck/danila_lib
 Author: arseniy_zhuck
 Author-email: arseniyzhuck@mail.ru
 Project-URL: GitHub, https://github.com/Arseniy-Zhuck/danila_lib
 Keywords: rama detect machine-learning computer-vision
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `danila-lib-1.8.6/README.md` & `danila-lib-1.8.7/README.md`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.6/danila/danila.py` & `danila-lib-1.8.7/danila/danila.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.6/danila/danila_v1.py` & `danila-lib-1.8.7/danila/danila_v1.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.6/danila/danila_v2.py` & `danila-lib-1.8.7/danila/danila_v2.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.6/danila/danila_v3.py` & `danila-lib-1.8.7/danila/danila_v3.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.6/danila/danila_v4.py` & `danila-lib-1.8.7/danila/danila_v4.py`

 * *Files 0% similar despite different names*

```diff
@@ -438,12 +438,12 @@
         hash_str = hash_object.hexdigest()
         initial_image_path = 'initial_image' + hash_str + '.jpg'
         cv2.imwrite(initial_image_path, img)
         number_rects = self.vagon_number_detect_model.vagon_rama_detect(initial_image_path, size)
         if len(number_rects) == 0:
             os.remove(initial_image_path)
             return img
-        img_with_number = img.copy
+        img_with_number = img.copy()
         for number_rect in number_rects:
             cv2.rectangle(img_with_number, (number_rect.xmin, number_rect.ymin), (number_rect.xmax, number_rect.ymax), (0, 0, 255), 2)
             cv2.putText(img_with_number, 'number', (number_rect.xmin, number_rect.ymin), cv2.FONT_HERSHEY_SIMPLEX, 0.5, (0, 0, 255), 2)
         return img_with_number
```

### Comparing `danila-lib-1.8.6/danila_lib.egg-info/PKG-INFO` & `danila-lib-1.8.7/danila_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danila-lib
-Version: 1.8.6
+Version: 1.8.7
 Summary: This is the module for detecting and classifying text on rama pictures
 Home-page: https://github.com/Arseniy-Zhuck/danila_lib
 Author: arseniy_zhuck
 Author-email: arseniyzhuck@mail.ru
 Project-URL: GitHub, https://github.com/Arseniy-Zhuck/danila_lib
 Keywords: rama detect machine-learning computer-vision
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `danila-lib-1.8.6/danila_lib.egg-info/SOURCES.txt` & `danila-lib-1.8.7/danila_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.6/danila_lib.egg-info/requires.txt` & `danila-lib-1.8.7/danila_lib.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.6/data/neuro/Letters_recognize.py` & `danila-lib-1.8.7/data/neuro/Letters_recognize.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.6/data/neuro/Rama_classify_class.py` & `danila-lib-1.8.7/data/neuro/Rama_classify_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.6/data/neuro/Rama_detect_class.py` & `danila-lib-1.8.7/data/neuro/Rama_detect_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.6/data/neuro/Rama_prod_classify_class.py` & `danila-lib-1.8.7/data/neuro/Rama_prod_classify_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.6/data/neuro/Text_detect_class.py` & `danila-lib-1.8.7/data/neuro/Text_detect_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.6/data/neuro/Vagon_number_detect_class.py` & `danila-lib-1.8.7/data/neuro/Vagon_number_detect_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.6/data/neuro/letters_in_image.py` & `danila-lib-1.8.7/data/neuro/letters_in_image.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.6/data/neuro/models.py` & `danila-lib-1.8.7/data/neuro/models.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.6/data/neuro/objs_in_image.py` & `danila-lib-1.8.7/data/neuro/objs_in_image.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.6/data/neuro/text_recognize_yolo.py` & `danila-lib-1.8.7/data/neuro/text_recognize_yolo.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.6/data/result/Image_text_areas.py` & `danila-lib-1.8.7/data/result/Image_text_areas.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.6/data/result/Rect.py` & `danila-lib-1.8.7/data/result/Rect.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.6/data/result/Text_area.py` & `danila-lib-1.8.7/data/result/Text_area.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.6/data/result/Yolo_label_rect.py` & `danila-lib-1.8.7/data/result/Yolo_label_rect.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.6/setup.py` & `danila-lib-1.8.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   with open('requirements.txt', 'r') as f:
     a = f.read()
   b = a.split()
   return b
 
 setup(
   name='danila-lib',
-  version='1.8.6',
+  version='1.8.7',
   author='arseniy_zhuck',
   author_email='arseniyzhuck@mail.ru',
   description='This is the module for detecting and classifying text on rama pictures',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://github.com/Arseniy-Zhuck/danila_lib',
   packages=find_packages(),
```

