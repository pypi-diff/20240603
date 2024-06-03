# Comparing `tmp/automation-fw-helper-0.0.3.tar.gz` & `tmp/automation-fw-helper-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automation-fw-helper-0.0.3.tar", last modified: Mon Jun  3 10:39:21 2024, max compression
+gzip compressed data, was "automation-fw-helper-0.0.4.tar", last modified: Mon Jun  3 10:43:33 2024, max compression
```

## Comparing `automation-fw-helper-0.0.3.tar` & `automation-fw-helper-0.0.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-06-03 10:39:21.247370 automation-fw-helper-0.0.3/
--rw-rw-rw-   0        0        0    11558 2024-06-03 07:07:54.000000 automation-fw-helper-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      520 2024-06-03 10:39:21.245415 automation-fw-helper-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       50 2024-06-03 07:07:54.000000 automation-fw-helper-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-06-03 10:39:21.218089 automation-fw-helper-0.0.3/automation_fw_helper/
--rw-rw-rw-   0        0        0      478 2024-06-03 07:13:32.000000 automation-fw-helper-0.0.3/automation_fw_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-03 10:39:21.231748 automation-fw-helper-0.0.3/automation_fw_helper/common/
--rw-rw-rw-   0        0        0      478 2024-06-03 07:30:44.000000 automation-fw-helper-0.0.3/automation_fw_helper/common/__init__.py
--rw-rw-rw-   0        0        0     1399 2024-06-03 07:44:56.000000 automation-fw-helper-0.0.3/automation_fw_helper/common/dir.py
--rw-rw-rw-   0        0        0      834 2024-06-03 10:37:57.000000 automation-fw-helper-0.0.3/automation_fw_helper/common/log.py
-drwxrwxrwx   0        0        0        0 2024-06-03 10:39:21.236630 automation-fw-helper-0.0.3/automation_fw_helper/infrastructure/
--rw-rw-rw-   0        0        0      478 2024-06-03 07:20:17.000000 automation-fw-helper-0.0.3/automation_fw_helper/infrastructure/__init__.py
--rw-rw-rw-   0        0        0    22430 2024-06-03 10:39:04.000000 automation-fw-helper-0.0.3/automation_fw_helper/infrastructure/frame_api.py
--rw-rw-rw-   0        0        0      589 2024-06-03 07:53:10.000000 automation-fw-helper-0.0.3/automation_fw_helper/infrastructure/platform.py
-drwxrwxrwx   0        0        0        0 2024-06-03 10:39:21.241508 automation-fw-helper-0.0.3/automation_fw_helper/proxy/
--rw-rw-rw-   0        0        0      481 2024-06-03 07:29:23.000000 automation-fw-helper-0.0.3/automation_fw_helper/proxy/__init__.py
--rw-rw-rw-   0        0        0     1679 2024-06-03 10:06:17.000000 automation-fw-helper-0.0.3/automation_fw_helper/proxy/airtest_proxy.py
--rw-rw-rw-   0        0        0    10790 2024-06-03 07:40:25.000000 automation-fw-helper-0.0.3/automation_fw_helper/proxy/uiautomation_proxy.py
-drwxrwxrwx   0        0        0        0 2024-06-03 10:39:21.243461 automation-fw-helper-0.0.3/automation_fw_helper.egg-info/
--rw-rw-rw-   0        0        0      520 2024-06-03 10:39:21.000000 automation-fw-helper-0.0.3/automation_fw_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      665 2024-06-03 10:39:21.000000 automation-fw-helper-0.0.3/automation_fw_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-03 10:39:21.000000 automation-fw-helper-0.0.3/automation_fw_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-06-03 10:39:21.000000 automation-fw-helper-0.0.3/automation_fw_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2024-06-03 10:39:21.000000 automation-fw-helper-0.0.3/automation_fw_helper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-06-03 10:39:21.247370 automation-fw-helper-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1141 2024-06-03 10:39:15.000000 automation-fw-helper-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:43:33.351221 automation-fw-helper-0.0.4/
+-rw-rw-rw-   0        0        0    11558 2024-06-03 07:07:54.000000 automation-fw-helper-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      520 2024-06-03 10:43:33.349269 automation-fw-helper-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       50 2024-06-03 07:07:54.000000 automation-fw-helper-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-06-03 10:43:33.319014 automation-fw-helper-0.0.4/automation_fw_helper/
+-rw-rw-rw-   0        0        0      478 2024-06-03 07:13:32.000000 automation-fw-helper-0.0.4/automation_fw_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:43:33.335619 automation-fw-helper-0.0.4/automation_fw_helper/common/
+-rw-rw-rw-   0        0        0      478 2024-06-03 07:30:44.000000 automation-fw-helper-0.0.4/automation_fw_helper/common/__init__.py
+-rw-rw-rw-   0        0        0     1399 2024-06-03 07:44:56.000000 automation-fw-helper-0.0.4/automation_fw_helper/common/dir.py
+-rw-rw-rw-   0        0        0      834 2024-06-03 10:37:57.000000 automation-fw-helper-0.0.4/automation_fw_helper/common/log.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:43:33.342469 automation-fw-helper-0.0.4/automation_fw_helper/infrastructure/
+-rw-rw-rw-   0        0        0      478 2024-06-03 07:20:17.000000 automation-fw-helper-0.0.4/automation_fw_helper/infrastructure/__init__.py
+-rw-rw-rw-   0        0        0    22510 2024-06-03 10:42:47.000000 automation-fw-helper-0.0.4/automation_fw_helper/infrastructure/frame_api.py
+-rw-rw-rw-   0        0        0      589 2024-06-03 07:53:10.000000 automation-fw-helper-0.0.4/automation_fw_helper/infrastructure/platform.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:43:33.346341 automation-fw-helper-0.0.4/automation_fw_helper/proxy/
+-rw-rw-rw-   0        0        0      481 2024-06-03 07:29:23.000000 automation-fw-helper-0.0.4/automation_fw_helper/proxy/__init__.py
+-rw-rw-rw-   0        0        0     1679 2024-06-03 10:06:17.000000 automation-fw-helper-0.0.4/automation_fw_helper/proxy/airtest_proxy.py
+-rw-rw-rw-   0        0        0    10790 2024-06-03 07:40:25.000000 automation-fw-helper-0.0.4/automation_fw_helper/proxy/uiautomation_proxy.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:43:33.348293 automation-fw-helper-0.0.4/automation_fw_helper.egg-info/
+-rw-rw-rw-   0        0        0      520 2024-06-03 10:43:33.000000 automation-fw-helper-0.0.4/automation_fw_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      665 2024-06-03 10:43:33.000000 automation-fw-helper-0.0.4/automation_fw_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 10:43:33.000000 automation-fw-helper-0.0.4/automation_fw_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-06-03 10:43:33.000000 automation-fw-helper-0.0.4/automation_fw_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-06-03 10:43:33.000000 automation-fw-helper-0.0.4/automation_fw_helper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-03 10:43:33.351221 automation-fw-helper-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1141 2024-06-03 10:42:58.000000 automation-fw-helper-0.0.4/setup.py
```

### Comparing `automation-fw-helper-0.0.3/LICENSE` & `automation-fw-helper-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `automation-fw-helper-0.0.3/PKG-INFO` & `automation-fw-helper-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automation-fw-helper
-Version: 0.0.3
+Version: 0.0.4
 Summary: This is my automation framework helper package
 Home-page: https://github.com/ckf10000/automation-fw-helper
 Author: ckf10000
 Author-email: ckf10000@sina.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `automation-fw-helper-0.0.3/automation_fw_helper/common/dir.py` & `automation-fw-helper-0.0.4/automation_fw_helper/common/dir.py`

 * *Files identical despite different names*

### Comparing `automation-fw-helper-0.0.3/automation_fw_helper/common/log.py` & `automation-fw-helper-0.0.4/automation_fw_helper/common/log.py`

 * *Files identical despite different names*

### Comparing `automation-fw-helper-0.0.3/automation_fw_helper/infrastructure/frame_api.py` & `automation-fw-helper-0.0.4/automation_fw_helper/infrastructure/frame_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 # CreateDate:   2024/06/03
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 import re
 import shlex
 import airtest
+import logging
 import warnings
 import subprocess
 import typing as t
 from poco.proxy import UIObjectProxy
 from airtest.utils.transform import TargetPos
 
 from automation_fw_helper.common.dir import get_project_path
@@ -106,18 +107,19 @@
 class AirtestProxy(object):
 
     def __init__(
             self,
             device_id: str,
             device_conn: str = None,
             is_enabled_log: bool = False,
+            log_level: int = logging.WARNING,
             platform: str = ANDROID_PLATFORM,
             enable_debug: bool = False
     ) -> None:
-        init_airtest_log(is_enable=is_enabled_log)
+        init_airtest_log(is_enable=is_enabled_log, level=log_level)
         self.platform = platform
         self.__device_id = device_id
         self.device_conn = device_conn or self.__init_conn()
         self.enable_debug = enable_debug
         self.__init_device()
         self.dev = device()
```

### Comparing `automation-fw-helper-0.0.3/automation_fw_helper/infrastructure/platform.py` & `automation-fw-helper-0.0.4/automation_fw_helper/infrastructure/platform.py`

 * *Files identical despite different names*

### Comparing `automation-fw-helper-0.0.3/automation_fw_helper/proxy/airtest_proxy.py` & `automation-fw-helper-0.0.4/automation_fw_helper/proxy/airtest_proxy.py`

 * *Files identical despite different names*

### Comparing `automation-fw-helper-0.0.3/automation_fw_helper/proxy/uiautomation_proxy.py` & `automation-fw-helper-0.0.4/automation_fw_helper/proxy/uiautomation_proxy.py`

 * *Files identical despite different names*

### Comparing `automation-fw-helper-0.0.3/automation_fw_helper.egg-info/PKG-INFO` & `automation-fw-helper-0.0.4/automation_fw_helper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automation-fw-helper
-Version: 0.0.3
+Version: 0.0.4
 Summary: This is my automation framework helper package
 Home-page: https://github.com/ckf10000/automation-fw-helper
 Author: ckf10000
 Author-email: ckf10000@sina.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `automation-fw-helper-0.0.3/automation_fw_helper.egg-info/SOURCES.txt` & `automation-fw-helper-0.0.4/automation_fw_helper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `automation-fw-helper-0.0.3/setup.py` & `automation-fw-helper-0.0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='automation-fw-helper',
-    version='0.0.3',
+    version='0.0.4',
     description='This is my automation framework helper package',
     long_description='This is my automation framework helper package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/automation-fw-helper',
     packages=find_packages(),
     install_requires=[
```

