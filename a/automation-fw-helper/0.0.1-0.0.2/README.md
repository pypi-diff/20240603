# Comparing `tmp/automation-fw-helper-0.0.1.tar.gz` & `tmp/automation-fw-helper-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automation-fw-helper-0.0.1.tar", last modified: Mon Jun  3 08:33:16 2024, max compression
+gzip compressed data, was "automation-fw-helper-0.0.2.tar", last modified: Mon Jun  3 10:16:05 2024, max compression
```

## Comparing `automation-fw-helper-0.0.1.tar` & `automation-fw-helper-0.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-06-03 08:33:16.409616 automation-fw-helper-0.0.1/
--rw-rw-rw-   0        0        0    11558 2024-06-03 07:07:54.000000 automation-fw-helper-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      520 2024-06-03 08:33:16.407622 automation-fw-helper-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       50 2024-06-03 07:07:54.000000 automation-fw-helper-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-06-03 08:33:16.388073 automation-fw-helper-0.0.1/automation_fw_helper/
--rw-rw-rw-   0        0        0      478 2024-06-03 07:13:32.000000 automation-fw-helper-0.0.1/automation_fw_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:33:16.397648 automation-fw-helper-0.0.1/automation_fw_helper/common/
--rw-rw-rw-   0        0        0      478 2024-06-03 07:30:44.000000 automation-fw-helper-0.0.1/automation_fw_helper/common/__init__.py
--rw-rw-rw-   0        0        0     1399 2024-06-03 07:44:56.000000 automation-fw-helper-0.0.1/automation_fw_helper/common/dir.py
--rw-rw-rw-   0        0        0      527 2024-06-03 07:31:23.000000 automation-fw-helper-0.0.1/automation_fw_helper/common/log.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:33:16.401638 automation-fw-helper-0.0.1/automation_fw_helper/infrastructure/
--rw-rw-rw-   0        0        0      478 2024-06-03 07:20:17.000000 automation-fw-helper-0.0.1/automation_fw_helper/infrastructure/__init__.py
--rw-rw-rw-   0        0        0    22157 2024-06-03 08:19:35.000000 automation-fw-helper-0.0.1/automation_fw_helper/infrastructure/frame_api.py
--rw-rw-rw-   0        0        0      589 2024-06-03 07:53:10.000000 automation-fw-helper-0.0.1/automation_fw_helper/infrastructure/platform.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:33:16.405626 automation-fw-helper-0.0.1/automation_fw_helper/proxy/
--rw-rw-rw-   0        0        0      481 2024-06-03 07:29:23.000000 automation-fw-helper-0.0.1/automation_fw_helper/proxy/__init__.py
--rw-rw-rw-   0        0        0     1679 2024-06-03 08:24:49.000000 automation-fw-helper-0.0.1/automation_fw_helper/proxy/airtest_proxy.py
--rw-rw-rw-   0        0        0    10790 2024-06-03 07:40:25.000000 automation-fw-helper-0.0.1/automation_fw_helper/proxy/uiautomation_proxy.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:33:16.406624 automation-fw-helper-0.0.1/automation_fw_helper.egg-info/
--rw-rw-rw-   0        0        0      520 2024-06-03 08:33:16.000000 automation-fw-helper-0.0.1/automation_fw_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      665 2024-06-03 08:33:16.000000 automation-fw-helper-0.0.1/automation_fw_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-03 08:33:16.000000 automation-fw-helper-0.0.1/automation_fw_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-06-03 08:33:16.000000 automation-fw-helper-0.0.1/automation_fw_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2024-06-03 08:33:16.000000 automation-fw-helper-0.0.1/automation_fw_helper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-06-03 08:33:16.409616 automation-fw-helper-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1141 2024-06-03 07:28:18.000000 automation-fw-helper-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:16:05.907202 automation-fw-helper-0.0.2/
+-rw-rw-rw-   0        0        0    11558 2024-06-03 07:07:54.000000 automation-fw-helper-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      520 2024-06-03 10:16:05.905252 automation-fw-helper-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       50 2024-06-03 07:07:54.000000 automation-fw-helper-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-06-03 10:16:05.870118 automation-fw-helper-0.0.2/automation_fw_helper/
+-rw-rw-rw-   0        0        0      478 2024-06-03 07:13:32.000000 automation-fw-helper-0.0.2/automation_fw_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:16:05.887690 automation-fw-helper-0.0.2/automation_fw_helper/common/
+-rw-rw-rw-   0        0        0      478 2024-06-03 07:30:44.000000 automation-fw-helper-0.0.2/automation_fw_helper/common/__init__.py
+-rw-rw-rw-   0        0        0     1399 2024-06-03 07:44:56.000000 automation-fw-helper-0.0.2/automation_fw_helper/common/dir.py
+-rw-rw-rw-   0        0        0      527 2024-06-03 07:31:23.000000 automation-fw-helper-0.0.2/automation_fw_helper/common/log.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:16:05.894517 automation-fw-helper-0.0.2/automation_fw_helper/infrastructure/
+-rw-rw-rw-   0        0        0      478 2024-06-03 07:20:17.000000 automation-fw-helper-0.0.2/automation_fw_helper/infrastructure/__init__.py
+-rw-rw-rw-   0        0        0    22317 2024-06-03 10:15:44.000000 automation-fw-helper-0.0.2/automation_fw_helper/infrastructure/frame_api.py
+-rw-rw-rw-   0        0        0      589 2024-06-03 07:53:10.000000 automation-fw-helper-0.0.2/automation_fw_helper/infrastructure/platform.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:16:05.901347 automation-fw-helper-0.0.2/automation_fw_helper/proxy/
+-rw-rw-rw-   0        0        0      481 2024-06-03 07:29:23.000000 automation-fw-helper-0.0.2/automation_fw_helper/proxy/__init__.py
+-rw-rw-rw-   0        0        0     1679 2024-06-03 10:06:17.000000 automation-fw-helper-0.0.2/automation_fw_helper/proxy/airtest_proxy.py
+-rw-rw-rw-   0        0        0    10790 2024-06-03 07:40:25.000000 automation-fw-helper-0.0.2/automation_fw_helper/proxy/uiautomation_proxy.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:16:05.903299 automation-fw-helper-0.0.2/automation_fw_helper.egg-info/
+-rw-rw-rw-   0        0        0      520 2024-06-03 10:16:05.000000 automation-fw-helper-0.0.2/automation_fw_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      665 2024-06-03 10:16:05.000000 automation-fw-helper-0.0.2/automation_fw_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 10:16:05.000000 automation-fw-helper-0.0.2/automation_fw_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-06-03 10:16:05.000000 automation-fw-helper-0.0.2/automation_fw_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-06-03 10:16:05.000000 automation-fw-helper-0.0.2/automation_fw_helper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-03 10:16:05.907202 automation-fw-helper-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1141 2024-06-03 10:16:01.000000 automation-fw-helper-0.0.2/setup.py
```

### Comparing `automation-fw-helper-0.0.1/LICENSE` & `automation-fw-helper-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `automation-fw-helper-0.0.1/PKG-INFO` & `automation-fw-helper-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automation-fw-helper
-Version: 0.0.1
+Version: 0.0.2
 Summary: This is my automation framework helper package
 Home-page: https://github.com/ckf10000/automation-fw-helper
 Author: ckf10000
 Author-email: ckf10000@sina.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `automation-fw-helper-0.0.1/automation_fw_helper/common/dir.py` & `automation-fw-helper-0.0.2/automation_fw_helper/common/dir.py`

 * *Files identical despite different names*

### Comparing `automation-fw-helper-0.0.1/automation_fw_helper/common/log.py` & `automation-fw-helper-0.0.2/automation_fw_helper/common/log.py`

 * *Files identical despite different names*

### Comparing `automation-fw-helper-0.0.1/automation_fw_helper/infrastructure/frame_api.py` & `automation-fw-helper-0.0.2/automation_fw_helper/infrastructure/frame_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from poco.proxy import UIObjectProxy
 from airtest.utils.transform import TargetPos
 
 from automation_fw_helper.common.log import logger
 from automation_fw_helper.common.dir import get_project_path
 # from airtest.cli.parser import cli_setup
 from automation_fw_helper.proxy.airtest_proxy import cli_setup
+from automation_fw_helper.proxy.airtest_proxy import get_javacap_url
 # from poco.drivers.android.uiautomation import AndroidUiautomationPoco
 from automation_fw_helper.proxy.uiautomation_proxy import AndroidUiautomationPoco
 from airtest.core.api import auto_setup, device, Template, touch, find_all, connect_device, exists
 from automation_fw_helper.infrastructure.platform import WINDOWS_PLATFORM, ANDROID_PLATFORM, iOS_PLATFORM
 
 warnings.filterwarnings(
     "ignore", category=UserWarning, message="Currently using ADB touch, the efficiency may be very low."
@@ -103,34 +104,35 @@
 
 
 class AirtestProxy(object):
 
     def __init__(
             self,
             device_id: str,
-            port: int = 0,
             device_conn: str = None,
             platform: str = ANDROID_PLATFORM,
             enable_debug: bool = False
     ) -> None:
         self.platform = platform
-        self.device_id = device_id
-        self.port = port
-        self.device_conn = device_conn
+        self.__device_id = device_id
+        self.device_conn = device_conn or self.__init_conn()
         self.enable_debug = enable_debug
         self.__init_device()
         self.dev = device()
 
+    def __init_conn(self) -> str:
+        return get_javacap_url(device_id=self.__device_id)
+
     def __init_device(self) -> None:
         if not cli_setup():
             project_root = get_project_path()
             airtest.utils.compat.DEFAULT_LOG_DIR = "logs"
             airtest.core.settings.Settings.DEBUG = self.enable_debug
-            airtest.core.settings.Settings.LOG_FILE = "{}.log".format(self.device_id)
-            if self.port > 0:
+            airtest.core.settings.Settings.LOG_FILE = "{}.log".format(self.__device_id)
+            if self.__device_id.find(":") != -1:
                 if self.platform == ANDROID_PLATFORM:
                     connect_device(self.device_conn)
                 else:
                     raise ValueError("暂时还不支持非android平台的手机初始化...")
             else:
                 auto_setup(
                     project_root,
@@ -430,15 +432,15 @@
             self.dev.paste(*args, **kwargs)
             return True
         return False
 
     # 快捷滑屏
     def quick_slide_screen(self, duration: float = 0.5):
         # 获取屏幕尺寸
-        screen_width, screen_height = get_screen_size_via_adb(device_id=self.device_id)
+        screen_width, screen_height = get_screen_size_via_adb(device_id=self.__device_id)
         # 定义起始点和终止点坐标
         start_x = screen_width // 2  # 屏幕中心点的横坐标
         start_y = screen_height // 2  # 屏幕中心点的纵坐标
         end_x = start_x  # 横坐标保持不变
         end_y = screen_height // 4  # 终止点纵坐标为屏幕顶部 1/4 处
         # 执行滑动操作
         self.swipe((start_x, start_y), (end_x, end_y), duration=duration)
```

### Comparing `automation-fw-helper-0.0.1/automation_fw_helper/infrastructure/platform.py` & `automation-fw-helper-0.0.2/automation_fw_helper/infrastructure/platform.py`

 * *Files identical despite different names*

### Comparing `automation-fw-helper-0.0.1/automation_fw_helper/proxy/airtest_proxy.py` & `automation-fw-helper-0.0.2/automation_fw_helper/proxy/airtest_proxy.py`

 * *Files identical despite different names*

### Comparing `automation-fw-helper-0.0.1/automation_fw_helper/proxy/uiautomation_proxy.py` & `automation-fw-helper-0.0.2/automation_fw_helper/proxy/uiautomation_proxy.py`

 * *Files identical despite different names*

### Comparing `automation-fw-helper-0.0.1/automation_fw_helper.egg-info/PKG-INFO` & `automation-fw-helper-0.0.2/automation_fw_helper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automation-fw-helper
-Version: 0.0.1
+Version: 0.0.2
 Summary: This is my automation framework helper package
 Home-page: https://github.com/ckf10000/automation-fw-helper
 Author: ckf10000
 Author-email: ckf10000@sina.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `automation-fw-helper-0.0.1/automation_fw_helper.egg-info/SOURCES.txt` & `automation-fw-helper-0.0.2/automation_fw_helper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `automation-fw-helper-0.0.1/setup.py` & `automation-fw-helper-0.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='automation-fw-helper',
-    version='0.0.1',
+    version='0.0.2',
     description='This is my automation framework helper package',
     long_description='This is my automation framework helper package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/automation-fw-helper',
     packages=find_packages(),
     install_requires=[
```

