# Comparing `tmp/GameWorldNavigator-0.0.7.3.tar.gz` & `tmp/GameWorldNavigator-0.0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GameWorldNavigator-0.0.7.3.tar", last modified: Fri May 31 07:22:34 2024, max compression
+gzip compressed data, was "GameWorldNavigator-0.0.7.4.tar", last modified: Mon Jun  3 05:17:04 2024, max compression
```

## Comparing `GameWorldNavigator-0.0.7.3.tar` & `GameWorldNavigator-0.0.7.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 07:22:34.552883 GameWorldNavigator-0.0.7.3/
-drwxrwxrwx   0        0        0        0 2024-05-31 07:22:34.542657 GameWorldNavigator-0.0.7.3/GameWorldNavigator.egg-info/
--rw-rw-rw-   0        0        0      790 2024-05-31 07:22:34.000000 GameWorldNavigator-0.0.7.3/GameWorldNavigator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      718 2024-05-31 07:22:34.000000 GameWorldNavigator-0.0.7.3/GameWorldNavigator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 07:22:34.000000 GameWorldNavigator-0.0.7.3/GameWorldNavigator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      839 2024-05-31 07:22:34.000000 GameWorldNavigator-0.0.7.3/GameWorldNavigator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-31 07:22:34.000000 GameWorldNavigator-0.0.7.3/GameWorldNavigator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1084 2023-11-14 15:46:54.000000 GameWorldNavigator-0.0.7.3/LICENSE
--rw-rw-rw-   0        0        0      790 2024-05-31 07:22:34.551842 GameWorldNavigator-0.0.7.3/PKG-INFO
--rw-rw-rw-   0        0        0      352 2023-11-15 07:38:05.000000 GameWorldNavigator-0.0.7.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-31 07:22:34.548667 GameWorldNavigator-0.0.7.3/gamenavigator/
--rw-rw-rw-   0        0        0      575 2024-05-25 01:28:35.000000 GameWorldNavigator-0.0.7.3/gamenavigator/__init__.py
--rw-rw-rw-   0        0        0      253 2023-11-14 15:30:21.000000 GameWorldNavigator-0.0.7.3/gamenavigator/config.py
--rw-rw-rw-   0        0        0     4997 2024-05-30 14:20:09.000000 GameWorldNavigator-0.0.7.3/gamenavigator/controller.py
-drwxrwxrwx   0        0        0        0 2024-05-31 07:22:34.550837 GameWorldNavigator-0.0.7.3/gamenavigator/core/
--rw-rw-rw-   0        0        0      149 2024-05-30 14:04:45.000000 GameWorldNavigator-0.0.7.3/gamenavigator/core/__init__.py
--rw-rw-rw-   0        0        0      609 2024-05-26 04:19:24.000000 GameWorldNavigator-0.0.7.3/gamenavigator/core/image.py
--rw-rw-rw-   0        0        0     3766 2024-05-30 14:08:11.000000 GameWorldNavigator-0.0.7.3/gamenavigator/core/interface.py
--rw-rw-rw-   0        0        0     1811 2024-05-26 14:20:48.000000 GameWorldNavigator-0.0.7.3/gamenavigator/core/pos.py
--rw-rw-rw-   0        0        0      758 2023-11-19 02:27:01.000000 GameWorldNavigator-0.0.7.3/gamenavigator/core/rect.py
--rw-rw-rw-   0        0        0      372 2023-11-16 09:39:18.000000 GameWorldNavigator-0.0.7.3/gamenavigator/exception.py
--rw-rw-rw-   0        0        0    17077 2024-05-28 08:45:58.000000 GameWorldNavigator-0.0.7.3/gamenavigator/game_controller.py
--rw-rw-rw-   0        0        0     3237 2024-05-27 07:11:03.000000 GameWorldNavigator-0.0.7.3/gamenavigator/game_interface_controller.py
--rw-rw-rw-   0        0        0     4214 2024-05-31 07:02:49.000000 GameWorldNavigator-0.0.7.3/gamenavigator/image_recognition.py
--rw-rw-rw-   0        0        0     4325 2023-11-19 02:56:31.000000 GameWorldNavigator-0.0.7.3/gamenavigator/keyboard_mouse_simulation.py
--rw-rw-rw-   0        0        0      778 2023-11-15 07:05:17.000000 GameWorldNavigator-0.0.7.3/gamenavigator/listener.py
--rw-rw-rw-   0        0        0      703 2023-11-15 09:41:12.000000 GameWorldNavigator-0.0.7.3/gamenavigator/log.py
--rw-rw-rw-   0        0        0     1974 2024-05-26 09:59:22.000000 GameWorldNavigator-0.0.7.3/gamenavigator/ocr_recognition.py
--rw-rw-rw-   0        0        0       42 2024-05-31 07:22:34.552883 GameWorldNavigator-0.0.7.3/setup.cfg
--rw-rw-rw-   0        0        0      856 2024-05-31 07:22:12.000000 GameWorldNavigator-0.0.7.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 05:17:04.588358 GameWorldNavigator-0.0.7.4/
+drwxrwxrwx   0        0        0        0 2024-06-03 05:17:04.571216 GameWorldNavigator-0.0.7.4/GameWorldNavigator.egg-info/
+-rw-rw-rw-   0        0        0      790 2024-06-03 05:17:04.000000 GameWorldNavigator-0.0.7.4/GameWorldNavigator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      718 2024-06-03 05:17:04.000000 GameWorldNavigator-0.0.7.4/GameWorldNavigator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 05:17:04.000000 GameWorldNavigator-0.0.7.4/GameWorldNavigator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      839 2024-06-03 05:17:04.000000 GameWorldNavigator-0.0.7.4/GameWorldNavigator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-06-03 05:17:04.000000 GameWorldNavigator-0.0.7.4/GameWorldNavigator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1084 2023-11-14 15:46:54.000000 GameWorldNavigator-0.0.7.4/LICENSE
+-rw-rw-rw-   0        0        0      790 2024-06-03 05:17:04.587851 GameWorldNavigator-0.0.7.4/PKG-INFO
+-rw-rw-rw-   0        0        0      352 2023-11-15 07:38:05.000000 GameWorldNavigator-0.0.7.4/README.md
+drwxrwxrwx   0        0        0        0 2024-06-03 05:17:04.582329 GameWorldNavigator-0.0.7.4/gamenavigator/
+-rw-rw-rw-   0        0        0      575 2024-05-25 01:28:35.000000 GameWorldNavigator-0.0.7.4/gamenavigator/__init__.py
+-rw-rw-rw-   0        0        0      253 2023-11-14 15:30:21.000000 GameWorldNavigator-0.0.7.4/gamenavigator/config.py
+-rw-rw-rw-   0        0        0     4997 2024-05-30 14:20:09.000000 GameWorldNavigator-0.0.7.4/gamenavigator/controller.py
+drwxrwxrwx   0        0        0        0 2024-06-03 05:17:04.586842 GameWorldNavigator-0.0.7.4/gamenavigator/core/
+-rw-rw-rw-   0        0        0      149 2024-05-30 14:04:45.000000 GameWorldNavigator-0.0.7.4/gamenavigator/core/__init__.py
+-rw-rw-rw-   0        0        0      609 2024-05-26 04:19:24.000000 GameWorldNavigator-0.0.7.4/gamenavigator/core/image.py
+-rw-rw-rw-   0        0        0     3766 2024-05-30 14:08:11.000000 GameWorldNavigator-0.0.7.4/gamenavigator/core/interface.py
+-rw-rw-rw-   0        0        0     1811 2024-05-26 14:20:48.000000 GameWorldNavigator-0.0.7.4/gamenavigator/core/pos.py
+-rw-rw-rw-   0        0        0      758 2023-11-19 02:27:01.000000 GameWorldNavigator-0.0.7.4/gamenavigator/core/rect.py
+-rw-rw-rw-   0        0        0      372 2023-11-16 09:39:18.000000 GameWorldNavigator-0.0.7.4/gamenavigator/exception.py
+-rw-rw-rw-   0        0        0    17077 2024-05-28 08:45:58.000000 GameWorldNavigator-0.0.7.4/gamenavigator/game_controller.py
+-rw-rw-rw-   0        0        0     3237 2024-05-27 07:11:03.000000 GameWorldNavigator-0.0.7.4/gamenavigator/game_interface_controller.py
+-rw-rw-rw-   0        0        0     4214 2024-05-31 07:02:49.000000 GameWorldNavigator-0.0.7.4/gamenavigator/image_recognition.py
+-rw-rw-rw-   0        0        0     4325 2023-11-19 02:56:31.000000 GameWorldNavigator-0.0.7.4/gamenavigator/keyboard_mouse_simulation.py
+-rw-rw-rw-   0        0        0      778 2023-11-15 07:05:17.000000 GameWorldNavigator-0.0.7.4/gamenavigator/listener.py
+-rw-rw-rw-   0        0        0      703 2023-11-15 09:41:12.000000 GameWorldNavigator-0.0.7.4/gamenavigator/log.py
+-rw-rw-rw-   0        0        0     2061 2024-06-03 05:15:31.000000 GameWorldNavigator-0.0.7.4/gamenavigator/ocr_recognition.py
+-rw-rw-rw-   0        0        0       42 2024-06-03 05:17:04.588358 GameWorldNavigator-0.0.7.4/setup.cfg
+-rw-rw-rw-   0        0        0      856 2024-06-03 05:16:55.000000 GameWorldNavigator-0.0.7.4/setup.py
```

### Comparing `GameWorldNavigator-0.0.7.3/GameWorldNavigator.egg-info/PKG-INFO` & `GameWorldNavigator-0.0.7.4/GameWorldNavigator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GameWorldNavigator
-Version: 0.0.7.3
+Version: 0.0.7.4
 Summary: A framework for game automation
 Home-page: https://github.com/JunNanLYS/GameWorldNavigator
 Author: NanJunLYS
 Author-email: 18906571516@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `GameWorldNavigator-0.0.7.3/GameWorldNavigator.egg-info/SOURCES.txt` & `GameWorldNavigator-0.0.7.4/GameWorldNavigator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `GameWorldNavigator-0.0.7.3/GameWorldNavigator.egg-info/requires.txt` & `GameWorldNavigator-0.0.7.4/GameWorldNavigator.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `GameWorldNavigator-0.0.7.3/LICENSE` & `GameWorldNavigator-0.0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `GameWorldNavigator-0.0.7.3/PKG-INFO` & `GameWorldNavigator-0.0.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GameWorldNavigator
-Version: 0.0.7.3
+Version: 0.0.7.4
 Summary: A framework for game automation
 Home-page: https://github.com/JunNanLYS/GameWorldNavigator
 Author: NanJunLYS
 Author-email: 18906571516@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `GameWorldNavigator-0.0.7.3/gamenavigator/__init__.py` & `GameWorldNavigator-0.0.7.4/gamenavigator/__init__.py`

 * *Files identical despite different names*

### Comparing `GameWorldNavigator-0.0.7.3/gamenavigator/controller.py` & `GameWorldNavigator-0.0.7.4/gamenavigator/controller.py`

 * *Files identical despite different names*

### Comparing `GameWorldNavigator-0.0.7.3/gamenavigator/core/image.py` & `GameWorldNavigator-0.0.7.4/gamenavigator/core/image.py`

 * *Files identical despite different names*

### Comparing `GameWorldNavigator-0.0.7.3/gamenavigator/core/interface.py` & `GameWorldNavigator-0.0.7.4/gamenavigator/core/interface.py`

 * *Files identical despite different names*

### Comparing `GameWorldNavigator-0.0.7.3/gamenavigator/core/pos.py` & `GameWorldNavigator-0.0.7.4/gamenavigator/core/pos.py`

 * *Files identical despite different names*

### Comparing `GameWorldNavigator-0.0.7.3/gamenavigator/core/rect.py` & `GameWorldNavigator-0.0.7.4/gamenavigator/core/rect.py`

 * *Files identical despite different names*

### Comparing `GameWorldNavigator-0.0.7.3/gamenavigator/game_controller.py` & `GameWorldNavigator-0.0.7.4/gamenavigator/game_controller.py`

 * *Files identical despite different names*

### Comparing `GameWorldNavigator-0.0.7.3/gamenavigator/game_interface_controller.py` & `GameWorldNavigator-0.0.7.4/gamenavigator/game_interface_controller.py`

 * *Files identical despite different names*

### Comparing `GameWorldNavigator-0.0.7.3/gamenavigator/image_recognition.py` & `GameWorldNavigator-0.0.7.4/gamenavigator/image_recognition.py`

 * *Files identical despite different names*

### Comparing `GameWorldNavigator-0.0.7.3/gamenavigator/keyboard_mouse_simulation.py` & `GameWorldNavigator-0.0.7.4/gamenavigator/keyboard_mouse_simulation.py`

 * *Files identical despite different names*

### Comparing `GameWorldNavigator-0.0.7.3/gamenavigator/listener.py` & `GameWorldNavigator-0.0.7.4/gamenavigator/listener.py`

 * *Files identical despite different names*

### Comparing `GameWorldNavigator-0.0.7.3/gamenavigator/log.py` & `GameWorldNavigator-0.0.7.4/gamenavigator/log.py`

 * *Files identical despite different names*

### Comparing `GameWorldNavigator-0.0.7.3/gamenavigator/ocr_recognition.py` & `GameWorldNavigator-0.0.7.4/gamenavigator/ocr_recognition.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from . import log
 from .core import Pos
 
 system = TextSystem(use_angle_cls=False)
 
 
-def get_text_position(img: ndarray, text: str) -> ndarray:
+def get_text_position(img: ndarray, texts: tuple[str, ...]) -> ndarray:
     """获取输入的文本坐标
 
     优先返回与text完全相同的文本的坐标,其次返回相似度最高的文本的坐标,最后返回空坐标
 
     Args:
         img (ndarray): 图像
         text (str): 文本
@@ -24,22 +24,23 @@
     res = system.detect_and_ocr(img)
     equal = None
     equal_val = 0
     similarity = None
     similarity_val = 0
     for i in range(len(res)):
         box = res[i]
-        if box.ocr_text == text:
-            if box.score > equal_val:
-                equal_val = box.score
-                equal = box.box
-        if text in box.ocr_text:
-            if box.score > similarity_val:
-                similarity_val = box.score
-                similarity = box.box
+        for text in texts:
+            if box.ocr_text == text:
+                if box.score > equal_val:
+                    equal_val = box.score
+                    equal = box.box
+            if text in box.ocr_text:
+                if box.score > similarity_val:
+                    similarity_val = box.score
+                    similarity = box.box
     if equal is not None:
         return equal
     elif similarity is not None:
         return similarity
     log.debug("There are no equal or similar texts")
     return array([])
 
@@ -61,11 +62,11 @@
     elif direction == "right":
         index = -1
     positions = positions[index]
     x, y = positions
     pos = Pos(int(x), int(y))
     return pos
 
-def text_in_img(img: ndarray, text: str) -> bool:
+def text_in_img(img: ndarray, texts: tuple[str, ...]) -> bool:
     """ 判断图片中是否包含该文本 """
-    res = get_text_position(img, text)
+    res = get_text_position(img, texts)
     return res.size != 0
```

### Comparing `GameWorldNavigator-0.0.7.3/setup.py` & `GameWorldNavigator-0.0.7.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="GameWorldNavigator",
-    version="0.0.7.3",
+    version="0.0.7.4",
     author="NanJunLYS",
     author_email="18906571516@163.com",
     description="A framework for game automation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/JunNanLYS/GameWorldNavigator",
     packages=setuptools.find_packages(),
```

