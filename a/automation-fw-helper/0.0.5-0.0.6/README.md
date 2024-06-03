# Comparing `tmp/automation-fw-helper-0.0.5.tar.gz` & `tmp/automation-fw-helper-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automation-fw-helper-0.0.5.tar", last modified: Mon Jun  3 10:47:36 2024, max compression
+gzip compressed data, was "automation-fw-helper-0.0.6.tar", last modified: Mon Jun  3 12:37:15 2024, max compression
```

## Comparing `automation-fw-helper-0.0.5.tar` & `automation-fw-helper-0.0.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-06-03 10:47:36.095742 automation-fw-helper-0.0.5/
--rw-rw-rw-   0        0        0    11558 2024-06-03 07:07:54.000000 automation-fw-helper-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      520 2024-06-03 10:47:36.094766 automation-fw-helper-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       50 2024-06-03 07:07:54.000000 automation-fw-helper-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-06-03 10:47:36.071344 automation-fw-helper-0.0.5/automation_fw_helper/
--rw-rw-rw-   0        0        0      478 2024-06-03 07:13:32.000000 automation-fw-helper-0.0.5/automation_fw_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-03 10:47:36.083076 automation-fw-helper-0.0.5/automation_fw_helper/common/
--rw-rw-rw-   0        0        0      478 2024-06-03 07:30:44.000000 automation-fw-helper-0.0.5/automation_fw_helper/common/__init__.py
--rw-rw-rw-   0        0        0     1399 2024-06-03 07:44:56.000000 automation-fw-helper-0.0.5/automation_fw_helper/common/dir.py
--rw-rw-rw-   0        0        0      830 2024-06-03 10:47:18.000000 automation-fw-helper-0.0.5/automation_fw_helper/common/log.py
-drwxrwxrwx   0        0        0        0 2024-06-03 10:47:36.086960 automation-fw-helper-0.0.5/automation_fw_helper/infrastructure/
--rw-rw-rw-   0        0        0      478 2024-06-03 07:20:17.000000 automation-fw-helper-0.0.5/automation_fw_helper/infrastructure/__init__.py
--rw-rw-rw-   0        0        0    22510 2024-06-03 10:42:47.000000 automation-fw-helper-0.0.5/automation_fw_helper/infrastructure/frame_api.py
--rw-rw-rw-   0        0        0      589 2024-06-03 07:53:10.000000 automation-fw-helper-0.0.5/automation_fw_helper/infrastructure/platform.py
-drwxrwxrwx   0        0        0        0 2024-06-03 10:47:36.091837 automation-fw-helper-0.0.5/automation_fw_helper/proxy/
--rw-rw-rw-   0        0        0      481 2024-06-03 07:29:23.000000 automation-fw-helper-0.0.5/automation_fw_helper/proxy/__init__.py
--rw-rw-rw-   0        0        0     1679 2024-06-03 10:06:17.000000 automation-fw-helper-0.0.5/automation_fw_helper/proxy/airtest_proxy.py
--rw-rw-rw-   0        0        0    10790 2024-06-03 07:40:25.000000 automation-fw-helper-0.0.5/automation_fw_helper/proxy/uiautomation_proxy.py
-drwxrwxrwx   0        0        0        0 2024-06-03 10:47:36.093789 automation-fw-helper-0.0.5/automation_fw_helper.egg-info/
--rw-rw-rw-   0        0        0      520 2024-06-03 10:47:35.000000 automation-fw-helper-0.0.5/automation_fw_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      665 2024-06-03 10:47:36.000000 automation-fw-helper-0.0.5/automation_fw_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-03 10:47:35.000000 automation-fw-helper-0.0.5/automation_fw_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-06-03 10:47:35.000000 automation-fw-helper-0.0.5/automation_fw_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2024-06-03 10:47:35.000000 automation-fw-helper-0.0.5/automation_fw_helper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-06-03 10:47:36.096717 automation-fw-helper-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1141 2024-06-03 10:47:32.000000 automation-fw-helper-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 12:37:15.259752 automation-fw-helper-0.0.6/
+-rw-rw-rw-   0        0        0    11558 2024-06-03 07:07:54.000000 automation-fw-helper-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      520 2024-06-03 12:37:15.252732 automation-fw-helper-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       50 2024-06-03 07:07:54.000000 automation-fw-helper-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-06-03 12:37:15.179006 automation-fw-helper-0.0.6/automation_fw_helper/
+-rw-rw-rw-   0        0        0      478 2024-06-03 07:13:32.000000 automation-fw-helper-0.0.6/automation_fw_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 12:37:15.208444 automation-fw-helper-0.0.6/automation_fw_helper/common/
+-rw-rw-rw-   0        0        0      478 2024-06-03 07:30:44.000000 automation-fw-helper-0.0.6/automation_fw_helper/common/__init__.py
+-rw-rw-rw-   0        0        0     1399 2024-06-03 07:44:56.000000 automation-fw-helper-0.0.6/automation_fw_helper/common/dir.py
+-rw-rw-rw-   0        0        0      830 2024-06-03 10:47:18.000000 automation-fw-helper-0.0.6/automation_fw_helper/common/log.py
+drwxrwxrwx   0        0        0        0 2024-06-03 12:37:15.227205 automation-fw-helper-0.0.6/automation_fw_helper/infrastructure/
+-rw-rw-rw-   0        0        0      478 2024-06-03 07:20:17.000000 automation-fw-helper-0.0.6/automation_fw_helper/infrastructure/__init__.py
+-rw-rw-rw-   0        0        0    22686 2024-06-03 12:36:52.000000 automation-fw-helper-0.0.6/automation_fw_helper/infrastructure/frame_api.py
+-rw-rw-rw-   0        0        0      589 2024-06-03 07:53:10.000000 automation-fw-helper-0.0.6/automation_fw_helper/infrastructure/platform.py
+drwxrwxrwx   0        0        0        0 2024-06-03 12:37:15.240888 automation-fw-helper-0.0.6/automation_fw_helper/proxy/
+-rw-rw-rw-   0        0        0      481 2024-06-03 07:29:23.000000 automation-fw-helper-0.0.6/automation_fw_helper/proxy/__init__.py
+-rw-rw-rw-   0        0        0     1679 2024-06-03 10:06:17.000000 automation-fw-helper-0.0.6/automation_fw_helper/proxy/airtest_proxy.py
+-rw-rw-rw-   0        0        0    10790 2024-06-03 07:40:25.000000 automation-fw-helper-0.0.6/automation_fw_helper/proxy/uiautomation_proxy.py
+drwxrwxrwx   0        0        0        0 2024-06-03 12:37:15.251756 automation-fw-helper-0.0.6/automation_fw_helper.egg-info/
+-rw-rw-rw-   0        0        0      520 2024-06-03 12:37:14.000000 automation-fw-helper-0.0.6/automation_fw_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      665 2024-06-03 12:37:14.000000 automation-fw-helper-0.0.6/automation_fw_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 12:37:14.000000 automation-fw-helper-0.0.6/automation_fw_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-06-03 12:37:14.000000 automation-fw-helper-0.0.6/automation_fw_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-06-03 12:37:14.000000 automation-fw-helper-0.0.6/automation_fw_helper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-03 12:37:15.259752 automation-fw-helper-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1141 2024-06-03 12:37:05.000000 automation-fw-helper-0.0.6/setup.py
```

### Comparing `automation-fw-helper-0.0.5/LICENSE` & `automation-fw-helper-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `automation-fw-helper-0.0.5/PKG-INFO` & `automation-fw-helper-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automation-fw-helper
-Version: 0.0.5
+Version: 0.0.6
 Summary: This is my automation framework helper package
 Home-page: https://github.com/ckf10000/automation-fw-helper
 Author: ckf10000
 Author-email: ckf10000@sina.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `automation-fw-helper-0.0.5/automation_fw_helper/common/dir.py` & `automation-fw-helper-0.0.6/automation_fw_helper/common/dir.py`

 * *Files identical despite different names*

### Comparing `automation-fw-helper-0.0.5/automation_fw_helper/common/log.py` & `automation-fw-helper-0.0.6/automation_fw_helper/common/log.py`

 * *Files identical despite different names*

### Comparing `automation-fw-helper-0.0.5/automation_fw_helper/infrastructure/frame_api.py` & `automation-fw-helper-0.0.6/automation_fw_helper/infrastructure/frame_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     adb_cmd = "adb.exe -s {} shell am force-stop {}".format(device_id, app_name)
     # 将命令字符串分割成列表
     cmd_list = shlex.split(adb_cmd)
     try:
         # 执行ADB命令并设置超时时间
         subprocess.run(cmd_list, timeout=timeout, check=True)
         logger.info("execute cmd: {}".format(adb_cmd))
+        logger.info("启动APP：{}".format(app_name))
     except subprocess.TimeoutExpired:
         logger.error("Timeout occurred. Failed to stop the app.")
     except subprocess.CalledProcessError:
         logger.error("Failed to stop the app.")
     except Exception as e:
         logger.error("An error occurred: {}".format(e))
 
@@ -150,24 +151,26 @@
     def start_app(self, app_name: str) -> bool:
         """
         在设备上启动目标应用
         platform: Android, iOS
         """
         if self.platform in (ANDROID_PLATFORM, WINDOWS_PLATFORM):
             self.dev.start_app(app_name)
+            logger.info("启动APP：{}".format(app_name))
             return True
         return False
 
     def stop_app(self, app_name: str) -> bool:
         """
         终止目标应用在设备上的运行
         platform: Android, iOS
         """
         if self.platform in (ANDROID_PLATFORM, WINDOWS_PLATFORM):
             self.dev.stop_app(app_name)
+            logger.info("停止APP：{}".format(app_name))
             return True
         return False
 
     @classmethod
     def get_cv_template(cls,
                         file_name: t.LiteralString | str | bytes,
                         threshold: float = None,
```

### Comparing `automation-fw-helper-0.0.5/automation_fw_helper/infrastructure/platform.py` & `automation-fw-helper-0.0.6/automation_fw_helper/infrastructure/platform.py`

 * *Files identical despite different names*

### Comparing `automation-fw-helper-0.0.5/automation_fw_helper/proxy/airtest_proxy.py` & `automation-fw-helper-0.0.6/automation_fw_helper/proxy/airtest_proxy.py`

 * *Files identical despite different names*

### Comparing `automation-fw-helper-0.0.5/automation_fw_helper/proxy/uiautomation_proxy.py` & `automation-fw-helper-0.0.6/automation_fw_helper/proxy/uiautomation_proxy.py`

 * *Files identical despite different names*

### Comparing `automation-fw-helper-0.0.5/automation_fw_helper.egg-info/PKG-INFO` & `automation-fw-helper-0.0.6/automation_fw_helper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automation-fw-helper
-Version: 0.0.5
+Version: 0.0.6
 Summary: This is my automation framework helper package
 Home-page: https://github.com/ckf10000/automation-fw-helper
 Author: ckf10000
 Author-email: ckf10000@sina.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `automation-fw-helper-0.0.5/automation_fw_helper.egg-info/SOURCES.txt` & `automation-fw-helper-0.0.6/automation_fw_helper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `automation-fw-helper-0.0.5/setup.py` & `automation-fw-helper-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='automation-fw-helper',
-    version='0.0.5',
+    version='0.0.6',
     description='This is my automation framework helper package',
     long_description='This is my automation framework helper package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/automation-fw-helper',
     packages=find_packages(),
     install_requires=[
```

