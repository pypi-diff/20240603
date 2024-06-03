# Comparing `tmp/python-automation-0.1.1.tar.gz` & `tmp/python-automation-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-automation-0.1.1.tar", last modified: Mon Jun  3 11:53:27 2024, max compression
+gzip compressed data, was "python-automation-0.1.2.tar", last modified: Mon Jun  3 11:56:32 2024, max compression
```

## Comparing `python-automation-0.1.1.tar` & `python-automation-0.1.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxrwx   0        0        0        0 2024-06-03 11:53:27.989965 python-automation-0.1.1/
--rw-rw-rw-   0        0        0     1091 2024-06-03 07:02:26.000000 python-automation-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      491 2024-06-03 11:53:27.990964 python-automation-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      662 2024-06-03 05:07:06.000000 python-automation-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-06-03 11:53:27.932963 python-automation-0.1.1/pyautomation/
--rw-rw-rw-   0        0        0       22 2024-06-03 11:53:15.000000 python-automation-0.1.1/pyautomation/__init__.py
--rw-rw-rw-   0        0        0       72 2024-06-03 06:41:33.000000 python-automation-0.1.1/pyautomation/app.py
--rw-rw-rw-   0        0        0       90 2024-06-03 11:26:34.000000 python-automation-0.1.1/pyautomation/autogui.py
--rw-rw-rw-   0        0        0      265 2024-06-03 11:26:41.000000 python-automation-0.1.1/pyautomation/displayinfo.py
-drwxrwxrwx   0        0        0        0 2024-06-03 11:53:27.933965 python-automation-0.1.1/pyautomation/modules/
--rw-rw-rw-   0        0        0        0 2024-06-03 11:50:47.000000 python-automation-0.1.1/pyautomation/modules/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-03 11:53:27.934963 python-automation-0.1.1/pyautomation/modules/pyautogui/
--rw-rw-rw-   0        0        0        0 2024-06-03 11:50:28.000000 python-automation-0.1.1/pyautomation/modules/pyautogui/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-03 11:53:27.944963 python-automation-0.1.1/pyautomation/modules/pyautogui/pyautogui/
--rw-rw-rw-   0        0        0    79299 2024-06-03 06:25:08.000000 python-automation-0.1.1/pyautomation/modules/pyautogui/pyautogui/__init__.py
--rw-rw-rw-   0        0        0       57 2024-06-03 06:25:08.000000 python-automation-0.1.1/pyautomation/modules/pyautogui/pyautogui/__main__.py
--rw-rw-rw-   0        0        0        0 2024-06-03 06:25:08.000000 python-automation-0.1.1/pyautomation/modules/pyautogui/pyautogui/_pyautogui_java.py
--rw-rw-rw-   0        0        0    15294 2024-06-03 09:19:14.000000 python-automation-0.1.1/pyautomation/modules/pyautogui/pyautogui/_pyautogui_osx.py
--rw-rw-rw-   0        0        0    20417 2024-06-03 09:19:30.000000 python-automation-0.1.1/pyautomation/modules/pyautogui/pyautogui/_pyautogui_win.py
--rw-rw-rw-   0        0        0    16472 2024-06-03 09:19:43.000000 python-automation-0.1.1/pyautomation/modules/pyautogui/pyautogui/_pyautogui_x11.py
-drwxrwxrwx   0        0        0        0 2024-06-03 11:53:27.953962 python-automation-0.1.1/pyautomation/modules/screeninfo/
--rw-rw-rw-   0        0        0      186 2024-06-03 09:08:10.000000 python-automation-0.1.1/pyautomation/modules/screeninfo/__init__.py
--rw-rw-rw-   0        0        0      468 2024-06-03 09:00:49.000000 python-automation-0.1.1/pyautomation/modules/screeninfo/__main__.py
--rw-rw-rw-   0        0        0      904 2024-06-03 08:12:04.000000 python-automation-0.1.1/pyautomation/modules/screeninfo/common.py
-drwxrwxrwx   0        0        0        0 2024-06-03 11:53:27.964963 python-automation-0.1.1/pyautomation/modules/screeninfo/enumerators/
--rw-rw-rw-   0        0        0      217 2024-06-03 09:07:47.000000 python-automation-0.1.1/pyautomation/modules/screeninfo/enumerators/__init__.py
--rw-rw-rw-   0        0        0     1645 2024-06-03 09:08:54.000000 python-automation-0.1.1/pyautomation/modules/screeninfo/enumerators/cygwin.py
--rw-rw-rw-   0        0        0    10315 2024-06-03 09:08:59.000000 python-automation-0.1.1/pyautomation/modules/screeninfo/enumerators/drm.py
--rw-rw-rw-   0        0        0      707 2024-06-03 09:09:07.000000 python-automation-0.1.1/pyautomation/modules/screeninfo/enumerators/osx.py
--rw-rw-rw-   0        0        0     3122 2024-06-03 09:09:10.000000 python-automation-0.1.1/pyautomation/modules/screeninfo/enumerators/windows.py
--rw-rw-rw-   0        0        0     1572 2024-06-03 09:09:13.000000 python-automation-0.1.1/pyautomation/modules/screeninfo/enumerators/xinerama.py
--rw-rw-rw-   0        0        0     4344 2024-06-03 09:09:17.000000 python-automation-0.1.1/pyautomation/modules/screeninfo/enumerators/xrandr.py
--rw-rw-rw-   0        0        0      218 2024-06-03 09:00:33.000000 python-automation-0.1.1/pyautomation/modules/screeninfo/mytest.py
--rw-rw-rw-   0        0        0      966 2024-06-03 09:08:35.000000 python-automation-0.1.1/pyautomation/modules/screeninfo/screeninfo.py
--rw-rw-rw-   0        0        0      270 2024-06-03 09:11:56.000000 python-automation-0.1.1/pyautomation/modules/screeninfo/util.py
--rw-rw-rw-   0        0        0   398934 2024-06-03 07:01:41.000000 python-automation-0.1.1/pyautomation/msuiauto.py
--rw-rw-rw-   0        0        0       37 2024-06-03 11:26:48.000000 python-automation-0.1.1/pyautomation/pyauto.py
--rw-rw-rw-   0        0        0       30 2024-06-03 11:26:53.000000 python-automation-0.1.1/pyautomation/pyautovision.py
-drwxrwxrwx   0        0        0        0 2024-06-03 11:53:27.969962 python-automation-0.1.1/pyautomation/tools/
--rw-rw-rw-   0        0        0        0 2024-06-03 05:18:13.000000 python-automation-0.1.1/pyautomation/tools/__init__.py
--rw-rw-rw-   0        0        0      916 2024-06-03 10:37:14.000000 python-automation-0.1.1/pyautomation/tools/project_structure.py
--rw-rw-rw-   0        0        0    14031 2024-06-03 04:58:33.000000 python-automation-0.1.1/pyautomation/tools/utils.py
--rw-rw-rw-   0        0        0        0 2024-06-03 05:29:42.000000 python-automation-0.1.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-06-03 11:53:27.988962 python-automation-0.1.1/python_automation.egg-info/
--rw-rw-rw-   0        0        0      491 2024-06-03 11:53:27.000000 python-automation-0.1.1/python_automation.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1622 2024-06-03 11:53:27.000000 python-automation-0.1.1/python_automation.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-03 11:53:27.000000 python-automation-0.1.1/python_automation.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-06-03 11:53:27.000000 python-automation-0.1.1/python_automation.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       35 2024-06-03 11:53:27.000000 python-automation-0.1.1/python_automation.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-06-03 11:53:27.000000 python-automation-0.1.1/python_automation.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-06-03 11:53:27.991962 python-automation-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      727 2024-06-03 11:53:08.000000 python-automation-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 11:56:32.251213 python-automation-0.1.2/
+-rw-rw-rw-   0        0        0     1091 2024-06-03 07:02:26.000000 python-automation-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      491 2024-06-03 11:56:32.252213 python-automation-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      662 2024-06-03 05:07:06.000000 python-automation-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-06-03 11:56:32.200216 python-automation-0.1.2/pyautomation/
+-rw-rw-rw-   0        0        0       22 2024-06-03 11:56:30.000000 python-automation-0.1.2/pyautomation/__init__.py
+-rw-rw-rw-   0        0        0       72 2024-06-03 06:41:33.000000 python-automation-0.1.2/pyautomation/app.py
+-rw-rw-rw-   0        0        0       91 2024-06-03 11:56:08.000000 python-automation-0.1.2/pyautomation/autogui.py
+-rw-rw-rw-   0        0        0      265 2024-06-03 11:26:41.000000 python-automation-0.1.2/pyautomation/displayinfo.py
+drwxrwxrwx   0        0        0        0 2024-06-03 11:56:32.201213 python-automation-0.1.2/pyautomation/modules/
+-rw-rw-rw-   0        0        0        0 2024-06-03 11:50:47.000000 python-automation-0.1.2/pyautomation/modules/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 11:56:32.202217 python-automation-0.1.2/pyautomation/modules/pyautogui/
+-rw-rw-rw-   0        0        0        0 2024-06-03 11:50:28.000000 python-automation-0.1.2/pyautomation/modules/pyautogui/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 11:56:32.211212 python-automation-0.1.2/pyautomation/modules/pyautogui/pyautogui/
+-rw-rw-rw-   0        0        0    79299 2024-06-03 06:25:08.000000 python-automation-0.1.2/pyautomation/modules/pyautogui/pyautogui/__init__.py
+-rw-rw-rw-   0        0        0       57 2024-06-03 06:25:08.000000 python-automation-0.1.2/pyautomation/modules/pyautogui/pyautogui/__main__.py
+-rw-rw-rw-   0        0        0        0 2024-06-03 06:25:08.000000 python-automation-0.1.2/pyautomation/modules/pyautogui/pyautogui/_pyautogui_java.py
+-rw-rw-rw-   0        0        0    15294 2024-06-03 09:19:14.000000 python-automation-0.1.2/pyautomation/modules/pyautogui/pyautogui/_pyautogui_osx.py
+-rw-rw-rw-   0        0        0    20417 2024-06-03 09:19:30.000000 python-automation-0.1.2/pyautomation/modules/pyautogui/pyautogui/_pyautogui_win.py
+-rw-rw-rw-   0        0        0    16472 2024-06-03 09:19:43.000000 python-automation-0.1.2/pyautomation/modules/pyautogui/pyautogui/_pyautogui_x11.py
+drwxrwxrwx   0        0        0        0 2024-06-03 11:56:32.220212 python-automation-0.1.2/pyautomation/modules/screeninfo/
+-rw-rw-rw-   0        0        0      186 2024-06-03 09:08:10.000000 python-automation-0.1.2/pyautomation/modules/screeninfo/__init__.py
+-rw-rw-rw-   0        0        0      468 2024-06-03 09:00:49.000000 python-automation-0.1.2/pyautomation/modules/screeninfo/__main__.py
+-rw-rw-rw-   0        0        0      904 2024-06-03 08:12:04.000000 python-automation-0.1.2/pyautomation/modules/screeninfo/common.py
+drwxrwxrwx   0        0        0        0 2024-06-03 11:56:32.231214 python-automation-0.1.2/pyautomation/modules/screeninfo/enumerators/
+-rw-rw-rw-   0        0        0      217 2024-06-03 09:07:47.000000 python-automation-0.1.2/pyautomation/modules/screeninfo/enumerators/__init__.py
+-rw-rw-rw-   0        0        0     1645 2024-06-03 09:08:54.000000 python-automation-0.1.2/pyautomation/modules/screeninfo/enumerators/cygwin.py
+-rw-rw-rw-   0        0        0    10315 2024-06-03 09:08:59.000000 python-automation-0.1.2/pyautomation/modules/screeninfo/enumerators/drm.py
+-rw-rw-rw-   0        0        0      707 2024-06-03 09:09:07.000000 python-automation-0.1.2/pyautomation/modules/screeninfo/enumerators/osx.py
+-rw-rw-rw-   0        0        0     3122 2024-06-03 09:09:10.000000 python-automation-0.1.2/pyautomation/modules/screeninfo/enumerators/windows.py
+-rw-rw-rw-   0        0        0     1572 2024-06-03 09:09:13.000000 python-automation-0.1.2/pyautomation/modules/screeninfo/enumerators/xinerama.py
+-rw-rw-rw-   0        0        0     4344 2024-06-03 09:09:17.000000 python-automation-0.1.2/pyautomation/modules/screeninfo/enumerators/xrandr.py
+-rw-rw-rw-   0        0        0      218 2024-06-03 09:00:33.000000 python-automation-0.1.2/pyautomation/modules/screeninfo/mytest.py
+-rw-rw-rw-   0        0        0      966 2024-06-03 09:08:35.000000 python-automation-0.1.2/pyautomation/modules/screeninfo/screeninfo.py
+-rw-rw-rw-   0        0        0      270 2024-06-03 09:11:56.000000 python-automation-0.1.2/pyautomation/modules/screeninfo/util.py
+-rw-rw-rw-   0        0        0   398934 2024-06-03 07:01:41.000000 python-automation-0.1.2/pyautomation/msuiauto.py
+-rw-rw-rw-   0        0        0       37 2024-06-03 11:26:48.000000 python-automation-0.1.2/pyautomation/pyauto.py
+-rw-rw-rw-   0        0        0       30 2024-06-03 11:26:53.000000 python-automation-0.1.2/pyautomation/pyautovision.py
+drwxrwxrwx   0        0        0        0 2024-06-03 11:56:32.235214 python-automation-0.1.2/pyautomation/tools/
+-rw-rw-rw-   0        0        0        0 2024-06-03 05:18:13.000000 python-automation-0.1.2/pyautomation/tools/__init__.py
+-rw-rw-rw-   0        0        0      916 2024-06-03 10:37:14.000000 python-automation-0.1.2/pyautomation/tools/project_structure.py
+-rw-rw-rw-   0        0        0    14031 2024-06-03 04:58:33.000000 python-automation-0.1.2/pyautomation/tools/utils.py
+-rw-rw-rw-   0        0        0        0 2024-06-03 05:29:42.000000 python-automation-0.1.2/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-06-03 11:56:32.250213 python-automation-0.1.2/python_automation.egg-info/
+-rw-rw-rw-   0        0        0      491 2024-06-03 11:56:32.000000 python-automation-0.1.2/python_automation.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1622 2024-06-03 11:56:32.000000 python-automation-0.1.2/python_automation.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 11:56:32.000000 python-automation-0.1.2/python_automation.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-06-03 11:53:27.000000 python-automation-0.1.2/python_automation.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       35 2024-06-03 11:56:32.000000 python-automation-0.1.2/python_automation.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-06-03 11:56:32.000000 python-automation-0.1.2/python_automation.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-06-03 11:56:32.253213 python-automation-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      727 2024-06-03 11:56:24.000000 python-automation-0.1.2/setup.py
```

### Comparing `python-automation-0.1.1/LICENSE` & `python-automation-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python-automation-0.1.1/README.md` & `python-automation-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `python-automation-0.1.1/pyautomation/modules/pyautogui/pyautogui/__init__.py` & `python-automation-0.1.2/pyautomation/modules/pyautogui/pyautogui/__init__.py`

 * *Files identical despite different names*

### Comparing `python-automation-0.1.1/pyautomation/modules/pyautogui/pyautogui/_pyautogui_osx.py` & `python-automation-0.1.2/pyautomation/modules/pyautogui/pyautogui/_pyautogui_osx.py`

 * *Files identical despite different names*

### Comparing `python-automation-0.1.1/pyautomation/modules/pyautogui/pyautogui/_pyautogui_win.py` & `python-automation-0.1.2/pyautomation/modules/pyautogui/pyautogui/_pyautogui_win.py`

 * *Files identical despite different names*

### Comparing `python-automation-0.1.1/pyautomation/modules/pyautogui/pyautogui/_pyautogui_x11.py` & `python-automation-0.1.2/pyautomation/modules/pyautogui/pyautogui/_pyautogui_x11.py`

 * *Files identical despite different names*

### Comparing `python-automation-0.1.1/pyautomation/modules/screeninfo/common.py` & `python-automation-0.1.2/pyautomation/modules/screeninfo/common.py`

 * *Files identical despite different names*

### Comparing `python-automation-0.1.1/pyautomation/modules/screeninfo/enumerators/cygwin.py` & `python-automation-0.1.2/pyautomation/modules/screeninfo/enumerators/cygwin.py`

 * *Files identical despite different names*

### Comparing `python-automation-0.1.1/pyautomation/modules/screeninfo/enumerators/drm.py` & `python-automation-0.1.2/pyautomation/modules/screeninfo/enumerators/drm.py`

 * *Files identical despite different names*

### Comparing `python-automation-0.1.1/pyautomation/modules/screeninfo/enumerators/osx.py` & `python-automation-0.1.2/pyautomation/modules/screeninfo/enumerators/osx.py`

 * *Files identical despite different names*

### Comparing `python-automation-0.1.1/pyautomation/modules/screeninfo/enumerators/windows.py` & `python-automation-0.1.2/pyautomation/modules/screeninfo/enumerators/windows.py`

 * *Files identical despite different names*

### Comparing `python-automation-0.1.1/pyautomation/modules/screeninfo/enumerators/xinerama.py` & `python-automation-0.1.2/pyautomation/modules/screeninfo/enumerators/xinerama.py`

 * *Files identical despite different names*

### Comparing `python-automation-0.1.1/pyautomation/modules/screeninfo/enumerators/xrandr.py` & `python-automation-0.1.2/pyautomation/modules/screeninfo/enumerators/xrandr.py`

 * *Files identical despite different names*

### Comparing `python-automation-0.1.1/pyautomation/modules/screeninfo/screeninfo.py` & `python-automation-0.1.2/pyautomation/modules/screeninfo/screeninfo.py`

 * *Files identical despite different names*

### Comparing `python-automation-0.1.1/pyautomation/msuiauto.py` & `python-automation-0.1.2/pyautomation/msuiauto.py`

 * *Files identical despite different names*

### Comparing `python-automation-0.1.1/pyautomation/tools/project_structure.py` & `python-automation-0.1.2/pyautomation/tools/project_structure.py`

 * *Files identical despite different names*

### Comparing `python-automation-0.1.1/pyautomation/tools/utils.py` & `python-automation-0.1.2/pyautomation/tools/utils.py`

 * *Files identical despite different names*

### Comparing `python-automation-0.1.1/python_automation.egg-info/SOURCES.txt` & `python-automation-0.1.2/python_automation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-automation-0.1.1/setup.py` & `python-automation-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='python-automation',
-    version='0.1.1',
+    version='0.1.2',
     description='window automation package',
     author='changgwak',
     author_email='iamtony.ca@gmail.com',
     url='https://github.com/changgwak/',
     install_requires=['opencv-python', 'numpy', 'pillow', 'pywin32'],
     packages=find_packages(exclude=[]),
     keywords=['pyauto', 'rpa', 'python rpa', 'python automation', 'window selenium', 'pyautomation', 'autoclick'],
```

