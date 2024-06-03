# Comparing `tmp/python-automation-0.0.5.tar.gz` & `tmp/python-automation-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-automation-0.0.5.tar", last modified: Mon Jun  3 11:19:46 2024, max compression
+gzip compressed data, was "python-automation-0.0.6.tar", last modified: Mon Jun  3 11:24:27 2024, max compression
```

## Comparing `python-automation-0.0.5.tar` & `python-automation-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-06-03 11:19:46.820803 python-automation-0.0.5/
--rw-rw-rw-   0        0        0     1091 2024-06-03 07:02:26.000000 python-automation-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      491 2024-06-03 11:19:46.820803 python-automation-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      662 2024-06-03 05:07:06.000000 python-automation-0.0.5/README.md
--rw-rw-rw-   0        0        0        0 2024-06-03 05:29:42.000000 python-automation-0.0.5/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-06-03 11:19:46.816481 python-automation-0.0.5/python_automation.egg-info/
--rw-rw-rw-   0        0        0      491 2024-06-03 11:19:46.000000 python-automation-0.0.5/python_automation.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      336 2024-06-03 11:19:46.000000 python-automation-0.0.5/python_automation.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-03 11:19:46.000000 python-automation-0.0.5/python_automation.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-06-03 11:19:46.000000 python-automation-0.0.5/python_automation.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       35 2024-06-03 11:19:46.000000 python-automation-0.0.5/python_automation.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-06-03 11:19:46.000000 python-automation-0.0.5/python_automation.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-06-03 11:19:46.822801 python-automation-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      727 2024-06-03 11:19:39.000000 python-automation-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-06-03 11:19:46.819794 python-automation-0.0.5/tests/
--rw-rw-rw-   0        0        0        0 2024-06-03 05:18:13.000000 python-automation-0.0.5/tests/__init__.py
--rw-rw-rw-   0        0        0       46 2024-06-03 07:22:15.000000 python-automation-0.0.5/tests/test_executor.py
+drwxrwxrwx   0        0        0        0 2024-06-03 11:24:27.016375 python-automation-0.0.6/
+-rw-rw-rw-   0        0        0     1091 2024-06-03 07:02:26.000000 python-automation-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      491 2024-06-03 11:24:27.016375 python-automation-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      662 2024-06-03 05:07:06.000000 python-automation-0.0.6/README.md
+-rw-rw-rw-   0        0        0        0 2024-06-03 05:29:42.000000 python-automation-0.0.6/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-06-03 11:24:27.010370 python-automation-0.0.6/python_automation.egg-info/
+-rw-rw-rw-   0        0        0      491 2024-06-03 11:24:26.000000 python-automation-0.0.6/python_automation.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      336 2024-06-03 11:24:26.000000 python-automation-0.0.6/python_automation.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 11:24:26.000000 python-automation-0.0.6/python_automation.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-06-03 11:19:46.000000 python-automation-0.0.6/python_automation.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       35 2024-06-03 11:24:26.000000 python-automation-0.0.6/python_automation.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-06-03 11:24:26.000000 python-automation-0.0.6/python_automation.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-06-03 11:24:27.020371 python-automation-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      727 2024-06-03 11:24:21.000000 python-automation-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 11:24:27.015371 python-automation-0.0.6/tests/
+-rw-rw-rw-   0        0        0        0 2024-06-03 05:18:13.000000 python-automation-0.0.6/tests/__init__.py
+-rw-rw-rw-   0        0        0       46 2024-06-03 07:22:15.000000 python-automation-0.0.6/tests/test_executor.py
```

### Comparing `python-automation-0.0.5/LICENSE` & `python-automation-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `python-automation-0.0.5/README.md` & `python-automation-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `python-automation-0.0.5/setup.py` & `python-automation-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='python-automation',
-    version='0.0.5',
+    version='0.0.6',
     description='window automation package',
     author='changgwak',
     author_email='iamtony.ca@gmail.com',
     url='https://github.com/changgwak/',
     install_requires=['opencv-python', 'numpy', 'pillow', 'pywin32'],
     packages=find_packages(exclude=[]),
     keywords=['pyauto', 'rpa', 'python rpa', 'python automation', 'window selenium', 'pyautomation', 'autoclick'],
```

