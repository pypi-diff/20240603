# Comparing `tmp/automation-fw-helper-0.0.2.tar.gz` & `tmp/automation-fw-helper-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automation-fw-helper-0.0.2.tar", last modified: Mon Jun  3 10:16:05 2024, max compression
+gzip compressed data, was "automation-fw-helper-0.0.3.tar", last modified: Mon Jun  3 10:39:21 2024, max compression
```

## Comparing `automation-fw-helper-0.0.2.tar` & `automation-fw-helper-0.0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-06-03 10:16:05.907202 automation-fw-helper-0.0.2/
--rw-rw-rw-   0        0        0    11558 2024-06-03 07:07:54.000000 automation-fw-helper-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      520 2024-06-03 10:16:05.905252 automation-fw-helper-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       50 2024-06-03 07:07:54.000000 automation-fw-helper-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-06-03 10:16:05.870118 automation-fw-helper-0.0.2/automation_fw_helper/
--rw-rw-rw-   0        0        0      478 2024-06-03 07:13:32.000000 automation-fw-helper-0.0.2/automation_fw_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-03 10:16:05.887690 automation-fw-helper-0.0.2/automation_fw_helper/common/
--rw-rw-rw-   0        0        0      478 2024-06-03 07:30:44.000000 automation-fw-helper-0.0.2/automation_fw_helper/common/__init__.py
--rw-rw-rw-   0        0        0     1399 2024-06-03 07:44:56.000000 automation-fw-helper-0.0.2/automation_fw_helper/common/dir.py
--rw-rw-rw-   0        0        0      527 2024-06-03 07:31:23.000000 automation-fw-helper-0.0.2/automation_fw_helper/common/log.py
-drwxrwxrwx   0        0        0        0 2024-06-03 10:16:05.894517 automation-fw-helper-0.0.2/automation_fw_helper/infrastructure/
--rw-rw-rw-   0        0        0      478 2024-06-03 07:20:17.000000 automation-fw-helper-0.0.2/automation_fw_helper/infrastructure/__init__.py
--rw-rw-rw-   0        0        0    22317 2024-06-03 10:15:44.000000 automation-fw-helper-0.0.2/automation_fw_helper/infrastructure/frame_api.py
--rw-rw-rw-   0        0        0      589 2024-06-03 07:53:10.000000 automation-fw-helper-0.0.2/automation_fw_helper/infrastructure/platform.py
-drwxrwxrwx   0        0        0        0 2024-06-03 10:16:05.901347 automation-fw-helper-0.0.2/automation_fw_helper/proxy/
--rw-rw-rw-   0        0        0      481 2024-06-03 07:29:23.000000 automation-fw-helper-0.0.2/automation_fw_helper/proxy/__init__.py
--rw-rw-rw-   0        0        0     1679 2024-06-03 10:06:17.000000 automation-fw-helper-0.0.2/automation_fw_helper/proxy/airtest_proxy.py
--rw-rw-rw-   0        0        0    10790 2024-06-03 07:40:25.000000 automation-fw-helper-0.0.2/automation_fw_helper/proxy/uiautomation_proxy.py
-drwxrwxrwx   0        0        0        0 2024-06-03 10:16:05.903299 automation-fw-helper-0.0.2/automation_fw_helper.egg-info/
--rw-rw-rw-   0        0        0      520 2024-06-03 10:16:05.000000 automation-fw-helper-0.0.2/automation_fw_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      665 2024-06-03 10:16:05.000000 automation-fw-helper-0.0.2/automation_fw_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-03 10:16:05.000000 automation-fw-helper-0.0.2/automation_fw_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-06-03 10:16:05.000000 automation-fw-helper-0.0.2/automation_fw_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2024-06-03 10:16:05.000000 automation-fw-helper-0.0.2/automation_fw_helper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-06-03 10:16:05.907202 automation-fw-helper-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1141 2024-06-03 10:16:01.000000 automation-fw-helper-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:39:21.247370 automation-fw-helper-0.0.3/
+-rw-rw-rw-   0        0        0    11558 2024-06-03 07:07:54.000000 automation-fw-helper-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      520 2024-06-03 10:39:21.245415 automation-fw-helper-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       50 2024-06-03 07:07:54.000000 automation-fw-helper-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-06-03 10:39:21.218089 automation-fw-helper-0.0.3/automation_fw_helper/
+-rw-rw-rw-   0        0        0      478 2024-06-03 07:13:32.000000 automation-fw-helper-0.0.3/automation_fw_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:39:21.231748 automation-fw-helper-0.0.3/automation_fw_helper/common/
+-rw-rw-rw-   0        0        0      478 2024-06-03 07:30:44.000000 automation-fw-helper-0.0.3/automation_fw_helper/common/__init__.py
+-rw-rw-rw-   0        0        0     1399 2024-06-03 07:44:56.000000 automation-fw-helper-0.0.3/automation_fw_helper/common/dir.py
+-rw-rw-rw-   0        0        0      834 2024-06-03 10:37:57.000000 automation-fw-helper-0.0.3/automation_fw_helper/common/log.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:39:21.236630 automation-fw-helper-0.0.3/automation_fw_helper/infrastructure/
+-rw-rw-rw-   0        0        0      478 2024-06-03 07:20:17.000000 automation-fw-helper-0.0.3/automation_fw_helper/infrastructure/__init__.py
+-rw-rw-rw-   0        0        0    22430 2024-06-03 10:39:04.000000 automation-fw-helper-0.0.3/automation_fw_helper/infrastructure/frame_api.py
+-rw-rw-rw-   0        0        0      589 2024-06-03 07:53:10.000000 automation-fw-helper-0.0.3/automation_fw_helper/infrastructure/platform.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:39:21.241508 automation-fw-helper-0.0.3/automation_fw_helper/proxy/
+-rw-rw-rw-   0        0        0      481 2024-06-03 07:29:23.000000 automation-fw-helper-0.0.3/automation_fw_helper/proxy/__init__.py
+-rw-rw-rw-   0        0        0     1679 2024-06-03 10:06:17.000000 automation-fw-helper-0.0.3/automation_fw_helper/proxy/airtest_proxy.py
+-rw-rw-rw-   0        0        0    10790 2024-06-03 07:40:25.000000 automation-fw-helper-0.0.3/automation_fw_helper/proxy/uiautomation_proxy.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:39:21.243461 automation-fw-helper-0.0.3/automation_fw_helper.egg-info/
+-rw-rw-rw-   0        0        0      520 2024-06-03 10:39:21.000000 automation-fw-helper-0.0.3/automation_fw_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      665 2024-06-03 10:39:21.000000 automation-fw-helper-0.0.3/automation_fw_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 10:39:21.000000 automation-fw-helper-0.0.3/automation_fw_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-06-03 10:39:21.000000 automation-fw-helper-0.0.3/automation_fw_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-06-03 10:39:21.000000 automation-fw-helper-0.0.3/automation_fw_helper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-03 10:39:21.247370 automation-fw-helper-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1141 2024-06-03 10:39:15.000000 automation-fw-helper-0.0.3/setup.py
```

### Comparing `automation-fw-helper-0.0.2/LICENSE` & `automation-fw-helper-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `automation-fw-helper-0.0.2/PKG-INFO` & `automation-fw-helper-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automation-fw-helper
-Version: 0.0.2
+Version: 0.0.3
 Summary: This is my automation framework helper package
 Home-page: https://github.com/ckf10000/automation-fw-helper
 Author: ckf10000
 Author-email: ckf10000@sina.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `automation-fw-helper-0.0.2/automation_fw_helper/common/dir.py` & `automation-fw-helper-0.0.3/automation_fw_helper/common/dir.py`

 * *Files identical despite different names*

### Comparing `automation-fw-helper-0.0.2/automation_fw_helper/infrastructure/frame_api.py` & `automation-fw-helper-0.0.3/automation_fw_helper/infrastructure/frame_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 import airtest
 import warnings
 import subprocess
 import typing as t
 from poco.proxy import UIObjectProxy
 from airtest.utils.transform import TargetPos
 
-from automation_fw_helper.common.log import logger
 from automation_fw_helper.common.dir import get_project_path
 # from airtest.cli.parser import cli_setup
 from automation_fw_helper.proxy.airtest_proxy import cli_setup
+from automation_fw_helper.common.log import logger, init_airtest_log
 from automation_fw_helper.proxy.airtest_proxy import get_javacap_url
 # from poco.drivers.android.uiautomation import AndroidUiautomationPoco
 from automation_fw_helper.proxy.uiautomation_proxy import AndroidUiautomationPoco
 from airtest.core.api import auto_setup, device, Template, touch, find_all, connect_device, exists
 from automation_fw_helper.infrastructure.platform import WINDOWS_PLATFORM, ANDROID_PLATFORM, iOS_PLATFORM
 
 warnings.filterwarnings(
@@ -105,17 +105,19 @@
 
 class AirtestProxy(object):
 
     def __init__(
             self,
             device_id: str,
             device_conn: str = None,
+            is_enabled_log: bool = False,
             platform: str = ANDROID_PLATFORM,
             enable_debug: bool = False
     ) -> None:
+        init_airtest_log(is_enable=is_enabled_log)
         self.platform = platform
         self.__device_id = device_id
         self.device_conn = device_conn or self.__init_conn()
         self.enable_debug = enable_debug
         self.__init_device()
         self.dev = device()
```

### Comparing `automation-fw-helper-0.0.2/automation_fw_helper/infrastructure/platform.py` & `automation-fw-helper-0.0.3/automation_fw_helper/infrastructure/platform.py`

 * *Files identical despite different names*

### Comparing `automation-fw-helper-0.0.2/automation_fw_helper/proxy/airtest_proxy.py` & `automation-fw-helper-0.0.3/automation_fw_helper/proxy/airtest_proxy.py`

 * *Files identical despite different names*

### Comparing `automation-fw-helper-0.0.2/automation_fw_helper/proxy/uiautomation_proxy.py` & `automation-fw-helper-0.0.3/automation_fw_helper/proxy/uiautomation_proxy.py`

 * *Files identical despite different names*

### Comparing `automation-fw-helper-0.0.2/automation_fw_helper.egg-info/PKG-INFO` & `automation-fw-helper-0.0.3/automation_fw_helper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automation-fw-helper
-Version: 0.0.2
+Version: 0.0.3
 Summary: This is my automation framework helper package
 Home-page: https://github.com/ckf10000/automation-fw-helper
 Author: ckf10000
 Author-email: ckf10000@sina.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `automation-fw-helper-0.0.2/automation_fw_helper.egg-info/SOURCES.txt` & `automation-fw-helper-0.0.3/automation_fw_helper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `automation-fw-helper-0.0.2/setup.py` & `automation-fw-helper-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='automation-fw-helper',
-    version='0.0.2',
+    version='0.0.3',
     description='This is my automation framework helper package',
     long_description='This is my automation framework helper package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/automation-fw-helper',
     packages=find_packages(),
     install_requires=[
```

