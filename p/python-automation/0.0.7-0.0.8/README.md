# Comparing `tmp/python-automation-0.0.7.tar.gz` & `tmp/python-automation-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-automation-0.0.7.tar", last modified: Mon Jun  3 11:34:23 2024, max compression
+gzip compressed data, was "python-automation-0.0.8.tar", last modified: Mon Jun  3 11:37:10 2024, max compression
```

## Comparing `python-automation-0.0.7.tar` & `python-automation-0.0.8.tar`

### file list

```diff
@@ -1,47 +1,45 @@
-drwxrwxrwx   0        0        0        0 2024-06-03 11:34:23.692834 python-automation-0.0.7/
--rw-rw-rw-   0        0        0     1091 2024-06-03 07:02:26.000000 python-automation-0.0.7/LICENSE
--rw-rw-rw-   0        0        0      491 2024-06-03 11:34:23.693835 python-automation-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      662 2024-06-03 05:07:06.000000 python-automation-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-06-03 11:34:23.640825 python-automation-0.0.7/pyautomation/
--rw-rw-rw-   0        0        0        0 2024-06-03 11:34:03.000000 python-automation-0.0.7/pyautomation/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-03 11:34:23.652823 python-automation-0.0.7/pyautomation/src/
--rw-rw-rw-   0        0        0       22 2024-06-03 11:24:06.000000 python-automation-0.0.7/pyautomation/src/__init__.py
--rw-rw-rw-   0        0        0       72 2024-06-03 06:41:33.000000 python-automation-0.0.7/pyautomation/src/app.py
--rw-rw-rw-   0        0        0       90 2024-06-03 11:26:34.000000 python-automation-0.0.7/pyautomation/src/autogui.py
--rw-rw-rw-   0        0        0      265 2024-06-03 11:26:41.000000 python-automation-0.0.7/pyautomation/src/displayinfo.py
-drwxrwxrwx   0        0        0        0 2024-06-03 11:34:23.654827 python-automation-0.0.7/pyautomation/src/modules/
--rw-rw-rw-   0        0        0        0 2024-06-03 09:11:37.000000 python-automation-0.0.7/pyautomation/src/modules/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-03 11:34:23.663826 python-automation-0.0.7/pyautomation/src/modules/screeninfo/
--rw-rw-rw-   0        0        0      186 2024-06-03 09:08:10.000000 python-automation-0.0.7/pyautomation/src/modules/screeninfo/__init__.py
--rw-rw-rw-   0        0        0      468 2024-06-03 09:00:49.000000 python-automation-0.0.7/pyautomation/src/modules/screeninfo/__main__.py
--rw-rw-rw-   0        0        0      904 2024-06-03 08:12:04.000000 python-automation-0.0.7/pyautomation/src/modules/screeninfo/common.py
-drwxrwxrwx   0        0        0        0 2024-06-03 11:34:23.674825 python-automation-0.0.7/pyautomation/src/modules/screeninfo/enumerators/
--rw-rw-rw-   0        0        0      217 2024-06-03 09:07:47.000000 python-automation-0.0.7/pyautomation/src/modules/screeninfo/enumerators/__init__.py
--rw-rw-rw-   0        0        0     1645 2024-06-03 09:08:54.000000 python-automation-0.0.7/pyautomation/src/modules/screeninfo/enumerators/cygwin.py
--rw-rw-rw-   0        0        0    10315 2024-06-03 09:08:59.000000 python-automation-0.0.7/pyautomation/src/modules/screeninfo/enumerators/drm.py
--rw-rw-rw-   0        0        0      707 2024-06-03 09:09:07.000000 python-automation-0.0.7/pyautomation/src/modules/screeninfo/enumerators/osx.py
--rw-rw-rw-   0        0        0     3122 2024-06-03 09:09:10.000000 python-automation-0.0.7/pyautomation/src/modules/screeninfo/enumerators/windows.py
--rw-rw-rw-   0        0        0     1572 2024-06-03 09:09:13.000000 python-automation-0.0.7/pyautomation/src/modules/screeninfo/enumerators/xinerama.py
--rw-rw-rw-   0        0        0     4344 2024-06-03 09:09:17.000000 python-automation-0.0.7/pyautomation/src/modules/screeninfo/enumerators/xrandr.py
--rw-rw-rw-   0        0        0      218 2024-06-03 09:00:33.000000 python-automation-0.0.7/pyautomation/src/modules/screeninfo/mytest.py
--rw-rw-rw-   0        0        0      966 2024-06-03 09:08:35.000000 python-automation-0.0.7/pyautomation/src/modules/screeninfo/screeninfo.py
--rw-rw-rw-   0        0        0      270 2024-06-03 09:11:56.000000 python-automation-0.0.7/pyautomation/src/modules/screeninfo/util.py
--rw-rw-rw-   0        0        0   398934 2024-06-03 07:01:41.000000 python-automation-0.0.7/pyautomation/src/msuiauto.py
--rw-rw-rw-   0        0        0       37 2024-06-03 11:26:48.000000 python-automation-0.0.7/pyautomation/src/pyauto.py
--rw-rw-rw-   0        0        0       30 2024-06-03 11:26:53.000000 python-automation-0.0.7/pyautomation/src/pyautovision.py
-drwxrwxrwx   0        0        0        0 2024-06-03 11:34:23.678825 python-automation-0.0.7/pyautomation/tools/
--rw-rw-rw-   0        0        0        0 2024-06-03 05:18:13.000000 python-automation-0.0.7/pyautomation/tools/__init__.py
--rw-rw-rw-   0        0        0      916 2024-06-03 10:37:14.000000 python-automation-0.0.7/pyautomation/tools/project_structure.py
--rw-rw-rw-   0        0        0    14031 2024-06-03 04:58:33.000000 python-automation-0.0.7/pyautomation/tools/utils.py
--rw-rw-rw-   0        0        0        0 2024-06-03 05:29:42.000000 python-automation-0.0.7/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-06-03 11:34:23.689834 python-automation-0.0.7/python_automation.egg-info/
--rw-rw-rw-   0        0        0      491 2024-06-03 11:34:23.000000 python-automation-0.0.7/python_automation.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1368 2024-06-03 11:34:23.000000 python-automation-0.0.7/python_automation.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-03 11:34:23.000000 python-automation-0.0.7/python_automation.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-06-03 11:19:46.000000 python-automation-0.0.7/python_automation.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       35 2024-06-03 11:34:23.000000 python-automation-0.0.7/python_automation.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-06-03 11:34:23.000000 python-automation-0.0.7/python_automation.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-06-03 11:34:23.694836 python-automation-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      727 2024-06-03 11:27:01.000000 python-automation-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-06-03 11:34:23.691833 python-automation-0.0.7/tests/
--rw-rw-rw-   0        0        0       46 2024-06-03 07:22:15.000000 python-automation-0.0.7/tests/test_executor.py
+drwxrwxrwx   0        0        0        0 2024-06-03 11:37:10.774207 python-automation-0.0.8/
+-rw-rw-rw-   0        0        0     1091 2024-06-03 07:02:26.000000 python-automation-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0      491 2024-06-03 11:37:10.774207 python-automation-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      662 2024-06-03 05:07:06.000000 python-automation-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-06-03 11:37:10.708207 python-automation-0.0.8/pyautomation/
+-rw-rw-rw-   0        0        0       22 2024-06-03 11:37:00.000000 python-automation-0.0.8/pyautomation/__init__.py
+-rw-rw-rw-   0        0        0       72 2024-06-03 06:41:33.000000 python-automation-0.0.8/pyautomation/app.py
+-rw-rw-rw-   0        0        0       90 2024-06-03 11:26:34.000000 python-automation-0.0.8/pyautomation/autogui.py
+-rw-rw-rw-   0        0        0      265 2024-06-03 11:26:41.000000 python-automation-0.0.8/pyautomation/displayinfo.py
+drwxrwxrwx   0        0        0        0 2024-06-03 11:37:10.710205 python-automation-0.0.8/pyautomation/modules/
+-rw-rw-rw-   0        0        0        0 2024-06-03 09:11:37.000000 python-automation-0.0.8/pyautomation/modules/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 11:37:10.724210 python-automation-0.0.8/pyautomation/modules/screeninfo/
+-rw-rw-rw-   0        0        0      186 2024-06-03 09:08:10.000000 python-automation-0.0.8/pyautomation/modules/screeninfo/__init__.py
+-rw-rw-rw-   0        0        0      468 2024-06-03 09:00:49.000000 python-automation-0.0.8/pyautomation/modules/screeninfo/__main__.py
+-rw-rw-rw-   0        0        0      904 2024-06-03 08:12:04.000000 python-automation-0.0.8/pyautomation/modules/screeninfo/common.py
+drwxrwxrwx   0        0        0        0 2024-06-03 11:37:10.747209 python-automation-0.0.8/pyautomation/modules/screeninfo/enumerators/
+-rw-rw-rw-   0        0        0      217 2024-06-03 09:07:47.000000 python-automation-0.0.8/pyautomation/modules/screeninfo/enumerators/__init__.py
+-rw-rw-rw-   0        0        0     1645 2024-06-03 09:08:54.000000 python-automation-0.0.8/pyautomation/modules/screeninfo/enumerators/cygwin.py
+-rw-rw-rw-   0        0        0    10315 2024-06-03 09:08:59.000000 python-automation-0.0.8/pyautomation/modules/screeninfo/enumerators/drm.py
+-rw-rw-rw-   0        0        0      707 2024-06-03 09:09:07.000000 python-automation-0.0.8/pyautomation/modules/screeninfo/enumerators/osx.py
+-rw-rw-rw-   0        0        0     3122 2024-06-03 09:09:10.000000 python-automation-0.0.8/pyautomation/modules/screeninfo/enumerators/windows.py
+-rw-rw-rw-   0        0        0     1572 2024-06-03 09:09:13.000000 python-automation-0.0.8/pyautomation/modules/screeninfo/enumerators/xinerama.py
+-rw-rw-rw-   0        0        0     4344 2024-06-03 09:09:17.000000 python-automation-0.0.8/pyautomation/modules/screeninfo/enumerators/xrandr.py
+-rw-rw-rw-   0        0        0      218 2024-06-03 09:00:33.000000 python-automation-0.0.8/pyautomation/modules/screeninfo/mytest.py
+-rw-rw-rw-   0        0        0      966 2024-06-03 09:08:35.000000 python-automation-0.0.8/pyautomation/modules/screeninfo/screeninfo.py
+-rw-rw-rw-   0        0        0      270 2024-06-03 09:11:56.000000 python-automation-0.0.8/pyautomation/modules/screeninfo/util.py
+-rw-rw-rw-   0        0        0   398934 2024-06-03 07:01:41.000000 python-automation-0.0.8/pyautomation/msuiauto.py
+-rw-rw-rw-   0        0        0       37 2024-06-03 11:26:48.000000 python-automation-0.0.8/pyautomation/pyauto.py
+-rw-rw-rw-   0        0        0       30 2024-06-03 11:26:53.000000 python-automation-0.0.8/pyautomation/pyautovision.py
+drwxrwxrwx   0        0        0        0 2024-06-03 11:37:10.751206 python-automation-0.0.8/pyautomation/tools/
+-rw-rw-rw-   0        0        0        0 2024-06-03 05:18:13.000000 python-automation-0.0.8/pyautomation/tools/__init__.py
+-rw-rw-rw-   0        0        0      916 2024-06-03 10:37:14.000000 python-automation-0.0.8/pyautomation/tools/project_structure.py
+-rw-rw-rw-   0        0        0    14031 2024-06-03 04:58:33.000000 python-automation-0.0.8/pyautomation/tools/utils.py
+-rw-rw-rw-   0        0        0        0 2024-06-03 05:29:42.000000 python-automation-0.0.8/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-06-03 11:37:10.771207 python-automation-0.0.8/python_automation.egg-info/
+-rw-rw-rw-   0        0        0      491 2024-06-03 11:37:10.000000 python-automation-0.0.8/python_automation.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1259 2024-06-03 11:37:10.000000 python-automation-0.0.8/python_automation.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 11:37:10.000000 python-automation-0.0.8/python_automation.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-06-03 11:19:46.000000 python-automation-0.0.8/python_automation.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       35 2024-06-03 11:37:10.000000 python-automation-0.0.8/python_automation.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-06-03 11:37:10.000000 python-automation-0.0.8/python_automation.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-06-03 11:37:10.777207 python-automation-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      727 2024-06-03 11:37:05.000000 python-automation-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 11:37:10.773254 python-automation-0.0.8/tests/
+-rw-rw-rw-   0        0        0       46 2024-06-03 07:22:15.000000 python-automation-0.0.8/tests/test_executor.py
```

### Comparing `python-automation-0.0.7/LICENSE` & `python-automation-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `python-automation-0.0.7/README.md` & `python-automation-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `python-automation-0.0.7/pyautomation/src/modules/screeninfo/common.py` & `python-automation-0.0.8/pyautomation/modules/screeninfo/common.py`

 * *Files identical despite different names*

### Comparing `python-automation-0.0.7/pyautomation/src/modules/screeninfo/enumerators/cygwin.py` & `python-automation-0.0.8/pyautomation/modules/screeninfo/enumerators/cygwin.py`

 * *Files identical despite different names*

### Comparing `python-automation-0.0.7/pyautomation/src/modules/screeninfo/enumerators/drm.py` & `python-automation-0.0.8/pyautomation/modules/screeninfo/enumerators/drm.py`

 * *Files identical despite different names*

### Comparing `python-automation-0.0.7/pyautomation/src/modules/screeninfo/enumerators/osx.py` & `python-automation-0.0.8/pyautomation/modules/screeninfo/enumerators/osx.py`

 * *Files identical despite different names*

### Comparing `python-automation-0.0.7/pyautomation/src/modules/screeninfo/enumerators/windows.py` & `python-automation-0.0.8/pyautomation/modules/screeninfo/enumerators/windows.py`

 * *Files identical despite different names*

### Comparing `python-automation-0.0.7/pyautomation/src/modules/screeninfo/enumerators/xinerama.py` & `python-automation-0.0.8/pyautomation/modules/screeninfo/enumerators/xinerama.py`

 * *Files identical despite different names*

### Comparing `python-automation-0.0.7/pyautomation/src/modules/screeninfo/enumerators/xrandr.py` & `python-automation-0.0.8/pyautomation/modules/screeninfo/enumerators/xrandr.py`

 * *Files identical despite different names*

### Comparing `python-automation-0.0.7/pyautomation/src/modules/screeninfo/screeninfo.py` & `python-automation-0.0.8/pyautomation/modules/screeninfo/screeninfo.py`

 * *Files identical despite different names*

### Comparing `python-automation-0.0.7/pyautomation/src/msuiauto.py` & `python-automation-0.0.8/pyautomation/msuiauto.py`

 * *Files identical despite different names*

### Comparing `python-automation-0.0.7/pyautomation/tools/project_structure.py` & `python-automation-0.0.8/pyautomation/tools/project_structure.py`

 * *Files identical despite different names*

### Comparing `python-automation-0.0.7/pyautomation/tools/utils.py` & `python-automation-0.0.8/pyautomation/tools/utils.py`

 * *Files identical despite different names*

### Comparing `python-automation-0.0.7/python_automation.egg-info/SOURCES.txt` & `python-automation-0.0.8/python_automation.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 pyautomation/__init__.py
-pyautomation/src/__init__.py
-pyautomation/src/app.py
-pyautomation/src/autogui.py
-pyautomation/src/displayinfo.py
-pyautomation/src/msuiauto.py
-pyautomation/src/pyauto.py
-pyautomation/src/pyautovision.py
-pyautomation/src/modules/__init__.py
-pyautomation/src/modules/screeninfo/__init__.py
-pyautomation/src/modules/screeninfo/__main__.py
-pyautomation/src/modules/screeninfo/common.py
-pyautomation/src/modules/screeninfo/mytest.py
-pyautomation/src/modules/screeninfo/screeninfo.py
-pyautomation/src/modules/screeninfo/util.py
-pyautomation/src/modules/screeninfo/enumerators/__init__.py
-pyautomation/src/modules/screeninfo/enumerators/cygwin.py
-pyautomation/src/modules/screeninfo/enumerators/drm.py
-pyautomation/src/modules/screeninfo/enumerators/osx.py
-pyautomation/src/modules/screeninfo/enumerators/windows.py
-pyautomation/src/modules/screeninfo/enumerators/xinerama.py
-pyautomation/src/modules/screeninfo/enumerators/xrandr.py
+pyautomation/app.py
+pyautomation/autogui.py
+pyautomation/displayinfo.py
+pyautomation/msuiauto.py
+pyautomation/pyauto.py
+pyautomation/pyautovision.py
+pyautomation/modules/__init__.py
+pyautomation/modules/screeninfo/__init__.py
+pyautomation/modules/screeninfo/__main__.py
+pyautomation/modules/screeninfo/common.py
+pyautomation/modules/screeninfo/mytest.py
+pyautomation/modules/screeninfo/screeninfo.py
+pyautomation/modules/screeninfo/util.py
+pyautomation/modules/screeninfo/enumerators/__init__.py
+pyautomation/modules/screeninfo/enumerators/cygwin.py
+pyautomation/modules/screeninfo/enumerators/drm.py
+pyautomation/modules/screeninfo/enumerators/osx.py
+pyautomation/modules/screeninfo/enumerators/windows.py
+pyautomation/modules/screeninfo/enumerators/xinerama.py
+pyautomation/modules/screeninfo/enumerators/xrandr.py
 pyautomation/tools/__init__.py
 pyautomation/tools/project_structure.py
 pyautomation/tools/utils.py
 python_automation.egg-info/PKG-INFO
 python_automation.egg-info/SOURCES.txt
 python_automation.egg-info/dependency_links.txt
 python_automation.egg-info/not-zip-safe
```

### Comparing `python-automation-0.0.7/setup.py` & `python-automation-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='python-automation',
-    version='0.0.7',
+    version='0.0.8',
     description='window automation package',
     author='changgwak',
     author_email='iamtony.ca@gmail.com',
     url='https://github.com/changgwak/',
     install_requires=['opencv-python', 'numpy', 'pillow', 'pywin32'],
     packages=find_packages(exclude=[]),
     keywords=['pyauto', 'rpa', 'python rpa', 'python automation', 'window selenium', 'pyautomation', 'autoclick'],
```

