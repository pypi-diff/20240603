# Comparing `tmp/dynamic_py_loader-1.0.0b2.tar.gz` & `tmp/dynamic_py_loader-1.0.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamic_py_loader-1.0.0b2.tar", last modified: Sat May 25 10:42:30 2024, max compression
+gzip compressed data, was "dynamic_py_loader-1.0.0b3.tar", last modified: Mon Jun  3 10:48:17 2024, max compression
```

## Comparing `dynamic_py_loader-1.0.0b2.tar` & `dynamic_py_loader-1.0.0b3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-05-25 10:42:30.091066 dynamic_py_loader-1.0.0b2/
--rw-rw-rw-   0        0        0     1088 2024-05-23 14:31:37.000000 dynamic_py_loader-1.0.0b2/LICENSE
--rw-rw-rw-   0        0        0     3175 2024-05-25 10:42:30.091066 dynamic_py_loader-1.0.0b2/PKG-INFO
--rw-rw-rw-   0        0        0     2717 2024-05-25 10:17:35.000000 dynamic_py_loader-1.0.0b2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-25 10:42:30.053274 dynamic_py_loader-1.0.0b2/dinamic_py_loader/
--rw-rw-rw-   0        0        0      235 2024-05-24 22:37:10.000000 dynamic_py_loader-1.0.0b2/dinamic_py_loader/__init__.py
--rw-rw-rw-   0        0        0     2002 2024-05-24 23:24:39.000000 dynamic_py_loader-1.0.0b2/dinamic_py_loader/dinamic_loader.py
--rw-rw-rw-   0        0        0     2005 2024-05-24 22:48:12.000000 dynamic_py_loader-1.0.0b2/dinamic_py_loader/module_controller.py
--rw-rw-rw-   0        0        0     3741 2024-05-24 22:48:12.000000 dynamic_py_loader-1.0.0b2/dinamic_py_loader/package_controller.py
-drwxrwxrwx   0        0        0        0 2024-05-25 10:42:30.053274 dynamic_py_loader-1.0.0b2/dinamic_py_loader/tests/
--rw-rw-rw-   0        0        0        0 2024-05-23 15:25:47.000000 dynamic_py_loader-1.0.0b2/dinamic_py_loader/tests/__init__.py
--rw-rw-rw-   0        0        0       51 2024-05-24 16:03:54.000000 dynamic_py_loader-1.0.0b2/dinamic_py_loader/tests/direct_module.py
-drwxrwxrwx   0        0        0        0 2024-05-25 10:42:30.068905 dynamic_py_loader-1.0.0b2/dinamic_py_loader/tests/pkg1/
--rw-rw-rw-   0        0        0       42 2024-05-24 20:09:30.000000 dynamic_py_loader-1.0.0b2/dinamic_py_loader/tests/pkg1/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-25 10:42:30.068905 dynamic_py_loader-1.0.0b2/dinamic_py_loader/tests/pkg1/pkg1_sub_pkg/
--rw-rw-rw-   0        0        0        0 2024-05-23 15:03:00.000000 dynamic_py_loader-1.0.0b2/dinamic_py_loader/tests/pkg1/pkg1_sub_pkg/__init__.py
--rw-rw-rw-   0        0        0       48 2024-05-23 15:07:53.000000 dynamic_py_loader-1.0.0b2/dinamic_py_loader/tests/pkg1/pkg1_sub_pkg/source_1_1.py
--rw-rw-rw-   0        0        0       46 2024-05-23 15:07:53.000000 dynamic_py_loader-1.0.0b2/dinamic_py_loader/tests/pkg1/source_1.py
--rw-rw-rw-   0        0        0     3772 2024-05-25 10:41:47.000000 dynamic_py_loader-1.0.0b2/dinamic_py_loader/tests/unittests.py
-drwxrwxrwx   0        0        0        0 2024-05-25 10:42:30.075418 dynamic_py_loader-1.0.0b2/dinamic_py_loader/tests/коська/
--rw-rw-rw-   0        0        0        0 2024-05-24 16:27:16.000000 dynamic_py_loader-1.0.0b2/dinamic_py_loader/tests/коська/__init__.py
--rw-rw-rw-   0        0        0       48 2024-05-24 16:30:19.000000 dynamic_py_loader-1.0.0b2/dinamic_py_loader/tests/коська/cat_module.py
-drwxrwxrwx   0        0        0        0 2024-05-25 10:42:30.075418 dynamic_py_loader-1.0.0b2/dinamic_py_loader/tests/коська/подкоська/
--rw-rw-rw-   0        0        0        0 2024-05-24 16:27:16.000000 dynamic_py_loader-1.0.0b2/dinamic_py_loader/tests/коська/подкоська/__init__.py
--rw-rw-rw-   0        0        0       52 2024-05-24 20:58:36.000000 dynamic_py_loader-1.0.0b2/dinamic_py_loader/tests/коська/подкоська/sub_cat_module.py
-drwxrwxrwx   0        0        0        0 2024-05-25 10:42:30.091066 dynamic_py_loader-1.0.0b2/dynamic_py_loader.egg-info/
--rw-rw-rw-   0        0        0     3175 2024-05-25 10:42:29.000000 dynamic_py_loader-1.0.0b2/dynamic_py_loader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      883 2024-05-25 10:42:29.000000 dynamic_py_loader-1.0.0b2/dynamic_py_loader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-25 10:42:29.000000 dynamic_py_loader-1.0.0b2/dynamic_py_loader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-05-25 10:42:29.000000 dynamic_py_loader-1.0.0b2/dynamic_py_loader.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-25 10:42:30.091066 dynamic_py_loader-1.0.0b2/setup.cfg
--rw-rw-rw-   0        0        0      703 2024-05-25 10:41:54.000000 dynamic_py_loader-1.0.0b2/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:48:17.959878 dynamic_py_loader-1.0.0b3/
+-rw-rw-rw-   0        0        0     1088 2024-05-23 14:31:37.000000 dynamic_py_loader-1.0.0b3/LICENSE
+-rw-rw-rw-   0        0        0     3175 2024-06-03 10:48:17.959878 dynamic_py_loader-1.0.0b3/PKG-INFO
+-rw-rw-rw-   0        0        0     2717 2024-05-28 08:11:22.000000 dynamic_py_loader-1.0.0b3/README.md
+drwxrwxrwx   0        0        0        0 2024-06-03 10:48:17.928615 dynamic_py_loader-1.0.0b3/dynamic_py_loader/
+-rw-rw-rw-   0        0        0      235 2024-05-24 22:37:10.000000 dynamic_py_loader-1.0.0b3/dynamic_py_loader/__init__.py
+-rw-rw-rw-   0        0        0     2002 2024-05-24 23:24:39.000000 dynamic_py_loader-1.0.0b3/dynamic_py_loader/dinamic_loader.py
+-rw-rw-rw-   0        0        0     2005 2024-05-24 22:48:12.000000 dynamic_py_loader-1.0.0b3/dynamic_py_loader/module_controller.py
+-rw-rw-rw-   0        0        0     3741 2024-05-24 22:48:12.000000 dynamic_py_loader-1.0.0b3/dynamic_py_loader/package_controller.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:48:17.944249 dynamic_py_loader-1.0.0b3/dynamic_py_loader/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-23 15:25:47.000000 dynamic_py_loader-1.0.0b3/dynamic_py_loader/tests/__init__.py
+-rw-rw-rw-   0        0        0       51 2024-05-24 16:03:54.000000 dynamic_py_loader-1.0.0b3/dynamic_py_loader/tests/direct_module.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:48:17.944249 dynamic_py_loader-1.0.0b3/dynamic_py_loader/tests/pkg1/
+-rw-rw-rw-   0        0        0       42 2024-05-24 20:09:30.000000 dynamic_py_loader-1.0.0b3/dynamic_py_loader/tests/pkg1/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:48:17.944249 dynamic_py_loader-1.0.0b3/dynamic_py_loader/tests/pkg1/pkg1_sub_pkg/
+-rw-rw-rw-   0        0        0        0 2024-05-23 15:03:00.000000 dynamic_py_loader-1.0.0b3/dynamic_py_loader/tests/pkg1/pkg1_sub_pkg/__init__.py
+-rw-rw-rw-   0        0        0       48 2024-05-23 15:07:53.000000 dynamic_py_loader-1.0.0b3/dynamic_py_loader/tests/pkg1/pkg1_sub_pkg/source_1_1.py
+-rw-rw-rw-   0        0        0       46 2024-05-23 15:07:53.000000 dynamic_py_loader-1.0.0b3/dynamic_py_loader/tests/pkg1/source_1.py
+-rw-rw-rw-   0        0        0     3772 2024-05-28 08:11:22.000000 dynamic_py_loader-1.0.0b3/dynamic_py_loader/tests/unittests.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:48:17.944249 dynamic_py_loader-1.0.0b3/dynamic_py_loader/tests/коська/
+-rw-rw-rw-   0        0        0        0 2024-05-24 16:27:16.000000 dynamic_py_loader-1.0.0b3/dynamic_py_loader/tests/коська/__init__.py
+-rw-rw-rw-   0        0        0       48 2024-05-24 16:30:19.000000 dynamic_py_loader-1.0.0b3/dynamic_py_loader/tests/коська/cat_module.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:48:17.959878 dynamic_py_loader-1.0.0b3/dynamic_py_loader/tests/коська/подкоська/
+-rw-rw-rw-   0        0        0        0 2024-05-24 16:27:16.000000 dynamic_py_loader-1.0.0b3/dynamic_py_loader/tests/коська/подкоська/__init__.py
+-rw-rw-rw-   0        0        0       52 2024-05-24 20:58:36.000000 dynamic_py_loader-1.0.0b3/dynamic_py_loader/tests/коська/подкоська/sub_cat_module.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:48:17.959878 dynamic_py_loader-1.0.0b3/dynamic_py_loader.egg-info/
+-rw-rw-rw-   0        0        0     3175 2024-06-03 10:48:17.000000 dynamic_py_loader-1.0.0b3/dynamic_py_loader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      883 2024-06-03 10:48:17.000000 dynamic_py_loader-1.0.0b3/dynamic_py_loader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 10:48:17.000000 dynamic_py_loader-1.0.0b3/dynamic_py_loader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-06-03 10:48:17.000000 dynamic_py_loader-1.0.0b3/dynamic_py_loader.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-03 10:48:17.959878 dynamic_py_loader-1.0.0b3/setup.cfg
+-rw-rw-rw-   0        0        0      703 2024-06-03 10:46:18.000000 dynamic_py_loader-1.0.0b3/setup.py
```

### Comparing `dynamic_py_loader-1.0.0b2/LICENSE` & `dynamic_py_loader-1.0.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `dynamic_py_loader-1.0.0b2/PKG-INFO` & `dynamic_py_loader-1.0.0b3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamic_py_loader
-Version: 1.0.0b2
+Version: 1.0.0b3
 Summary: A simple dynamic packages and modules loaders.
 Home-page: https://github.com/Waffe-Wafle/dynamic_py_loader
 Author: Waffe-Wafle
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -16,15 +16,15 @@
 
 ## 1. Module Controller
 ### The `ModuleController` class is designed to store and work with dynamically loaded module.
 
 ### Usage:
 
 ```python
-from dinamic_py_loader import ModuleController
+from dynamic_py_loader import ModuleController
 from pathlib import Path
 
 # Load, there is no need to call resolve(),
 # also object can be inited empty to be loaded later:
 absolute_path = Path(__file__).parent / 'module.py'
 module = ModuleController(absolute_path)
 
@@ -44,15 +44,15 @@
 ## 2. Package Controller
 ### The `PackageController` class is designed to store and work with dynamically loaded package.
 ### It can contain modules and subpackages, also imports all from `__init__.py`.
 
 ### Usage:
 
 ```python
-from dinamic_py_loader import PackageLoader
+from dynamic_py_loader import PackageLoader
 from pathlib import Path
 
 # Load will work even for modern package without __init__.py,
 # also object can be inited empty:
 absolute_path = Path(__file__).parent / 'package'
 package = PackageLoader(absolute_path)
 
@@ -84,15 +84,15 @@
 
 ## 3. Dynamic loader wrapper (PackageController)
 ### Just wrapper to push arguments more comfortable and with ability to load modules and packages in the same level.
 
 ### Usage:
 
 ```python
-from dinamic_py_loader import PackageLoader
+from dynamic_py_loader import PackageLoader
 from pathlib import Path
 
 absolute_path = Path(__file__).parent / 'package'
 package = PackageLoader(absolute_path)
 
 package4 = PackageLoader('./pkg4')
 packages = PackageLoader('./pkg1', ['./pkg2', './pkg3'], package4)
```

### Comparing `dynamic_py_loader-1.0.0b2/README.md` & `dynamic_py_loader-1.0.0b3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 ## 1. Module Controller
 ### The `ModuleController` class is designed to store and work with dynamically loaded module.
 
 ### Usage:
 
 ```python
-from dinamic_py_loader import ModuleController
+from dynamic_py_loader import ModuleController
 from pathlib import Path
 
 # Load, there is no need to call resolve(),
 # also object can be inited empty to be loaded later:
 absolute_path = Path(__file__).parent / 'module.py'
 module = ModuleController(absolute_path)
 
@@ -30,15 +30,15 @@
 ## 2. Package Controller
 ### The `PackageController` class is designed to store and work with dynamically loaded package.
 ### It can contain modules and subpackages, also imports all from `__init__.py`.
 
 ### Usage:
 
 ```python
-from dinamic_py_loader import PackageLoader
+from dynamic_py_loader import PackageLoader
 from pathlib import Path
 
 # Load will work even for modern package without __init__.py,
 # also object can be inited empty:
 absolute_path = Path(__file__).parent / 'package'
 package = PackageLoader(absolute_path)
 
@@ -70,15 +70,15 @@
 
 ## 3. Dynamic loader wrapper (PackageController)
 ### Just wrapper to push arguments more comfortable and with ability to load modules and packages in the same level.
 
 ### Usage:
 
 ```python
-from dinamic_py_loader import PackageLoader
+from dynamic_py_loader import PackageLoader
 from pathlib import Path
 
 absolute_path = Path(__file__).parent / 'package'
 package = PackageLoader(absolute_path)
 
 package4 = PackageLoader('./pkg4')
 packages = PackageLoader('./pkg1', ['./pkg2', './pkg3'], package4)
```

### Comparing `dynamic_py_loader-1.0.0b2/dinamic_py_loader/dinamic_loader.py` & `dynamic_py_loader-1.0.0b3/dynamic_py_loader/dinamic_loader.py`

 * *Files identical despite different names*

### Comparing `dynamic_py_loader-1.0.0b2/dinamic_py_loader/module_controller.py` & `dynamic_py_loader-1.0.0b3/dynamic_py_loader/module_controller.py`

 * *Files identical despite different names*

### Comparing `dynamic_py_loader-1.0.0b2/dinamic_py_loader/package_controller.py` & `dynamic_py_loader-1.0.0b3/dynamic_py_loader/package_controller.py`

 * *Files identical despite different names*

### Comparing `dynamic_py_loader-1.0.0b2/dinamic_py_loader/tests/unittests.py` & `dynamic_py_loader-1.0.0b3/dynamic_py_loader/tests/unittests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import unittest
-from dinamic_py_loader.dinamic_py_loader import PackageController, ModuleController, DinamicLoader
+from dynamic_py_loader.dinamic_py_loader import PackageController, ModuleController, DinamicLoader
 from pathlib import Path
 
 
 TEST_ROOT = Path(__file__).parent
 
 
 class LoadingTests(unittest.TestCase):
```

### Comparing `dynamic_py_loader-1.0.0b2/dynamic_py_loader.egg-info/PKG-INFO` & `dynamic_py_loader-1.0.0b3/dynamic_py_loader.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamic_py_loader
-Version: 1.0.0b2
+Version: 1.0.0b3
 Summary: A simple dynamic packages and modules loaders.
 Home-page: https://github.com/Waffe-Wafle/dynamic_py_loader
 Author: Waffe-Wafle
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -16,15 +16,15 @@
 
 ## 1. Module Controller
 ### The `ModuleController` class is designed to store and work with dynamically loaded module.
 
 ### Usage:
 
 ```python
-from dinamic_py_loader import ModuleController
+from dynamic_py_loader import ModuleController
 from pathlib import Path
 
 # Load, there is no need to call resolve(),
 # also object can be inited empty to be loaded later:
 absolute_path = Path(__file__).parent / 'module.py'
 module = ModuleController(absolute_path)
 
@@ -44,15 +44,15 @@
 ## 2. Package Controller
 ### The `PackageController` class is designed to store and work with dynamically loaded package.
 ### It can contain modules and subpackages, also imports all from `__init__.py`.
 
 ### Usage:
 
 ```python
-from dinamic_py_loader import PackageLoader
+from dynamic_py_loader import PackageLoader
 from pathlib import Path
 
 # Load will work even for modern package without __init__.py,
 # also object can be inited empty:
 absolute_path = Path(__file__).parent / 'package'
 package = PackageLoader(absolute_path)
 
@@ -84,15 +84,15 @@
 
 ## 3. Dynamic loader wrapper (PackageController)
 ### Just wrapper to push arguments more comfortable and with ability to load modules and packages in the same level.
 
 ### Usage:
 
 ```python
-from dinamic_py_loader import PackageLoader
+from dynamic_py_loader import PackageLoader
 from pathlib import Path
 
 absolute_path = Path(__file__).parent / 'package'
 package = PackageLoader(absolute_path)
 
 package4 = PackageLoader('./pkg4')
 packages = PackageLoader('./pkg1', ['./pkg2', './pkg3'], package4)
```

### Comparing `dynamic_py_loader-1.0.0b2/dynamic_py_loader.egg-info/SOURCES.txt` & `dynamic_py_loader-1.0.0b3/dynamic_py_loader.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 LICENSE
 README.md
 setup.py
-dinamic_py_loader/__init__.py
-dinamic_py_loader/dinamic_loader.py
-dinamic_py_loader/module_controller.py
-dinamic_py_loader/package_controller.py
-dinamic_py_loader/tests/__init__.py
-dinamic_py_loader/tests/direct_module.py
-dinamic_py_loader/tests/unittests.py
-dinamic_py_loader/tests/pkg1/__init__.py
-dinamic_py_loader/tests/pkg1/source_1.py
-dinamic_py_loader/tests/pkg1/pkg1_sub_pkg/__init__.py
-dinamic_py_loader/tests/pkg1/pkg1_sub_pkg/source_1_1.py
-dinamic_py_loader/tests/коська/__init__.py
-dinamic_py_loader/tests/коська/cat_module.py
-dinamic_py_loader/tests/коська/подкоська/__init__.py
-dinamic_py_loader/tests/коська/подкоська/sub_cat_module.py
+dynamic_py_loader/__init__.py
+dynamic_py_loader/dinamic_loader.py
+dynamic_py_loader/module_controller.py
+dynamic_py_loader/package_controller.py
 dynamic_py_loader.egg-info/PKG-INFO
 dynamic_py_loader.egg-info/SOURCES.txt
 dynamic_py_loader.egg-info/dependency_links.txt
-dynamic_py_loader.egg-info/top_level.txt
+dynamic_py_loader.egg-info/top_level.txt
+dynamic_py_loader/tests/__init__.py
+dynamic_py_loader/tests/direct_module.py
+dynamic_py_loader/tests/unittests.py
+dynamic_py_loader/tests/pkg1/__init__.py
+dynamic_py_loader/tests/pkg1/source_1.py
+dynamic_py_loader/tests/pkg1/pkg1_sub_pkg/__init__.py
+dynamic_py_loader/tests/pkg1/pkg1_sub_pkg/source_1_1.py
+dynamic_py_loader/tests/коська/__init__.py
+dynamic_py_loader/tests/коська/cat_module.py
+dynamic_py_loader/tests/коська/подкоська/__init__.py
+dynamic_py_loader/tests/коська/подкоська/sub_cat_module.py
```

### Comparing `dynamic_py_loader-1.0.0b2/setup.py` & `dynamic_py_loader-1.0.0b3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open('README.md') as f:
         return f.read()
 
 
 setup(
     name='dynamic_py_loader',
-    version='1.0.0b2',
+    version='1.0.0b3',
     packages=find_packages(exclude=('tests')),
     author='Waffe-Wafle',
     description='A simple dynamic packages and modules loaders.',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://github.com/Waffe-Wafle/dynamic_py_loader',
     license='MIT',
```

