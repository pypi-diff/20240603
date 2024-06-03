# Comparing `tmp/pywayne-1.0.0.7.5.tar.gz` & `tmp/pywayne-1.0.0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywayne-1.0.0.7.5.tar", last modified: Mon May 27 13:03:04 2024, max compression
+gzip compressed data, was "pywayne-1.0.0.7.6.tar", last modified: Mon Jun  3 09:01:41 2024, max compression
```

## Comparing `pywayne-1.0.0.7.5.tar` & `pywayne-1.0.0.7.6.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-05-27 13:03:04.756651 pywayne-1.0.0.7.5/
--rw-r--r--   0 wayne      (503) staff       (20)     1064 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.5/LICENSE
--rw-r--r--   0 wayne      (503) staff       (20)     1485 2024-05-27 13:03:04.756196 pywayne-1.0.0.7.5/PKG-INFO
--rw-r--r--   0 wayne      (503) staff       (20)      600 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.5/README.md
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-05-27 13:03:04.748179 pywayne-1.0.0.7.5/bin/
--rw-r--r--   0 wayne      (503) staff       (20)       63 2023-11-01 16:27:11.000000 pywayne-1.0.0.7.5/bin/gettool
--rw-r--r--   0 wayne      (503) staff       (20)     5024 2024-05-27 13:02:05.000000 pywayne-1.0.0.7.5/bin/gettool.py
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-05-27 13:03:04.750618 pywayne-1.0.0.7.5/pywayne/
--rw-r--r--   0 wayne      (503) staff       (20)      207 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.5/pywayne/__init__.py
--rw-r--r--   0 wayne      (503) staff       (20)      242 2024-05-27 13:02:19.000000 pywayne-1.0.0.7.5/pywayne/__version__.py
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-05-27 13:03:04.752631 pywayne-1.0.0.7.5/pywayne/adb/
--rw-r--r--   0 wayne      (503) staff       (20)      278 2023-11-07 03:21:11.000000 pywayne-1.0.0.7.5/pywayne/adb/__init__.py
--rw-r--r--   0 wayne      (503) staff       (20)     2168 2023-11-07 03:21:11.000000 pywayne-1.0.0.7.5/pywayne/adb/logcat_reader.py
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-05-27 13:03:04.753187 pywayne-1.0.0.7.5/pywayne/ahrs/
--rw-r--r--   0 wayne      (503) staff       (20)      211 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.5/pywayne/ahrs/__init__.py
--rw-r--r--   0 wayne      (503) staff       (20)     4038 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.5/pywayne/ahrs/tools.py
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-05-27 13:03:04.753978 pywayne-1.0.0.7.5/pywayne/calibration/
--rw-r--r--   0 wayne      (503) staff       (20)      211 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.5/pywayne/calibration/__init__.py
--rw-r--r--   0 wayne      (503) staff       (20)     4269 2023-12-05 12:13:27.000000 pywayne-1.0.0.7.5/pywayne/calibration/magnetometer_calibration.py
--rw-r--r--   0 wayne      (503) staff       (20)      223 2023-12-05 11:52:18.000000 pywayne-1.0.0.7.5/pywayne/calibration/temporal_calibration.py
--rw-r--r--   0 wayne      (503) staff       (20)     6948 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.5/pywayne/data_structure.py
--rw-r--r--   0 wayne      (503) staff       (20)    16705 2023-11-11 07:27:50.000000 pywayne-1.0.0.7.5/pywayne/dsp.py
--rw-r--r--   0 wayne      (503) staff       (20)     7535 2023-11-11 18:58:57.000000 pywayne-1.0.0.7.5/pywayne/gui.py
--rw-r--r--   0 wayne      (503) staff       (20)     2433 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.5/pywayne/math.py
--rw-r--r--   0 wayne      (503) staff       (20)    14981 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.5/pywayne/plot.py
--rw-r--r--   0 wayne      (503) staff       (20)    18000 2024-05-24 03:47:33.000000 pywayne-1.0.0.7.5/pywayne/tools.py
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-05-27 13:03:04.754612 pywayne-1.0.0.7.5/pywayne/vio/
--rw-r--r--   0 wayne      (503) staff       (20)      243 2024-01-13 09:21:45.000000 pywayne-1.0.0.7.5/pywayne/vio/__init__.py
--rw-r--r--   0 wayne      (503) staff       (20)     3281 2024-01-13 09:21:45.000000 pywayne-1.0.0.7.5/pywayne/vio/tools.py
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-05-27 13:03:04.755300 pywayne-1.0.0.7.5/pywayne/visualization/
--rw-r--r--   0 wayne      (503) staff       (20)      271 2023-11-06 04:42:24.000000 pywayne-1.0.0.7.5/pywayne/visualization/__init__.py
--rw-r--r--   0 wayne      (503) staff       (20)     3766 2023-11-11 18:56:53.000000 pywayne-1.0.0.7.5/pywayne/visualization/pangolin.py
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-05-27 13:03:04.755707 pywayne-1.0.0.7.5/pywayne.egg-info/
--rw-r--r--   0 wayne      (503) staff       (20)     1485 2024-05-27 13:03:04.000000 pywayne-1.0.0.7.5/pywayne.egg-info/PKG-INFO
--rw-r--r--   0 wayne      (503) staff       (20)      692 2024-05-27 13:03:04.000000 pywayne-1.0.0.7.5/pywayne.egg-info/SOURCES.txt
--rw-r--r--   0 wayne      (503) staff       (20)      184 2024-05-27 13:03:04.000000 pywayne-1.0.0.7.5/pywayne.egg-info/dependency_links.txt
--rw-r--r--   0 wayne      (503) staff       (20)      162 2024-05-27 13:03:04.000000 pywayne-1.0.0.7.5/pywayne.egg-info/requires.txt
--rw-r--r--   0 wayne      (503) staff       (20)        8 2024-05-27 13:03:04.000000 pywayne-1.0.0.7.5/pywayne.egg-info/top_level.txt
--rw-r--r--   0 wayne      (503) staff       (20)       38 2024-05-27 13:03:04.756729 pywayne-1.0.0.7.5/setup.cfg
--rw-r--r--   0 wayne      (503) staff       (20)     1555 2023-11-05 05:52:08.000000 pywayne-1.0.0.7.5/setup.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-06-03 09:01:41.716454 pywayne-1.0.0.7.6/
+-rw-r--r--   0 wayne      (503) staff       (20)     1064 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.6/LICENSE
+-rw-r--r--   0 wayne      (503) staff       (20)     1447 2024-06-03 09:01:41.716038 pywayne-1.0.0.7.6/PKG-INFO
+-rw-r--r--   0 wayne      (503) staff       (20)      600 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.6/README.md
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-06-03 09:01:41.708522 pywayne-1.0.0.7.6/bin/
+-rw-r--r--   0 wayne      (503) staff       (20)       63 2023-11-01 16:27:11.000000 pywayne-1.0.0.7.6/bin/gettool
+-rw-r--r--   0 wayne      (503) staff       (20)     5024 2024-05-27 13:02:05.000000 pywayne-1.0.0.7.6/bin/gettool.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-06-03 09:01:41.711131 pywayne-1.0.0.7.6/pywayne/
+-rw-r--r--   0 wayne      (503) staff       (20)      207 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.6/pywayne/__init__.py
+-rw-r--r--   0 wayne      (503) staff       (20)      242 2024-06-03 08:59:47.000000 pywayne-1.0.0.7.6/pywayne/__version__.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-06-03 09:01:41.712752 pywayne-1.0.0.7.6/pywayne/adb/
+-rw-r--r--   0 wayne      (503) staff       (20)      278 2023-11-07 03:21:11.000000 pywayne-1.0.0.7.6/pywayne/adb/__init__.py
+-rw-r--r--   0 wayne      (503) staff       (20)     2168 2023-11-07 03:21:11.000000 pywayne-1.0.0.7.6/pywayne/adb/logcat_reader.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-06-03 09:01:41.713335 pywayne-1.0.0.7.6/pywayne/ahrs/
+-rw-r--r--   0 wayne      (503) staff       (20)      211 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.6/pywayne/ahrs/__init__.py
+-rw-r--r--   0 wayne      (503) staff       (20)     4038 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.6/pywayne/ahrs/tools.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-06-03 09:01:41.714094 pywayne-1.0.0.7.6/pywayne/calibration/
+-rw-r--r--   0 wayne      (503) staff       (20)      211 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.6/pywayne/calibration/__init__.py
+-rw-r--r--   0 wayne      (503) staff       (20)     4269 2023-12-05 12:13:27.000000 pywayne-1.0.0.7.6/pywayne/calibration/magnetometer_calibration.py
+-rw-r--r--   0 wayne      (503) staff       (20)      223 2023-12-05 11:52:18.000000 pywayne-1.0.0.7.6/pywayne/calibration/temporal_calibration.py
+-rw-r--r--   0 wayne      (503) staff       (20)     6948 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.6/pywayne/data_structure.py
+-rw-r--r--   0 wayne      (503) staff       (20)    16705 2023-11-11 07:27:50.000000 pywayne-1.0.0.7.6/pywayne/dsp.py
+-rw-r--r--   0 wayne      (503) staff       (20)     7535 2023-11-11 18:58:57.000000 pywayne-1.0.0.7.6/pywayne/gui.py
+-rw-r--r--   0 wayne      (503) staff       (20)     2433 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.6/pywayne/math.py
+-rw-r--r--   0 wayne      (503) staff       (20)    14981 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.6/pywayne/plot.py
+-rw-r--r--   0 wayne      (503) staff       (20)    18000 2024-05-24 03:47:33.000000 pywayne-1.0.0.7.6/pywayne/tools.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-06-03 09:01:41.714690 pywayne-1.0.0.7.6/pywayne/vio/
+-rw-r--r--   0 wayne      (503) staff       (20)      243 2024-01-13 09:21:45.000000 pywayne-1.0.0.7.6/pywayne/vio/__init__.py
+-rw-r--r--   0 wayne      (503) staff       (20)     3281 2024-01-13 09:21:45.000000 pywayne-1.0.0.7.6/pywayne/vio/tools.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-06-03 09:01:41.715354 pywayne-1.0.0.7.6/pywayne/visualization/
+-rw-r--r--   0 wayne      (503) staff       (20)      271 2023-11-06 04:42:24.000000 pywayne-1.0.0.7.6/pywayne/visualization/__init__.py
+-rw-r--r--   0 wayne      (503) staff       (20)     3766 2023-11-11 18:56:53.000000 pywayne-1.0.0.7.6/pywayne/visualization/pangolin.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-06-03 09:01:41.715743 pywayne-1.0.0.7.6/pywayne.egg-info/
+-rw-r--r--   0 wayne      (503) staff       (20)     1447 2024-06-03 09:01:41.000000 pywayne-1.0.0.7.6/pywayne.egg-info/PKG-INFO
+-rw-r--r--   0 wayne      (503) staff       (20)      692 2024-06-03 09:01:41.000000 pywayne-1.0.0.7.6/pywayne.egg-info/SOURCES.txt
+-rw-r--r--   0 wayne      (503) staff       (20)      184 2024-06-03 09:01:41.000000 pywayne-1.0.0.7.6/pywayne.egg-info/dependency_links.txt
+-rw-r--r--   0 wayne      (503) staff       (20)      154 2024-06-03 09:01:41.000000 pywayne-1.0.0.7.6/pywayne.egg-info/requires.txt
+-rw-r--r--   0 wayne      (503) staff       (20)        8 2024-06-03 09:01:41.000000 pywayne-1.0.0.7.6/pywayne.egg-info/top_level.txt
+-rw-r--r--   0 wayne      (503) staff       (20)       38 2024-06-03 09:01:41.716521 pywayne-1.0.0.7.6/setup.cfg
+-rw-r--r--   0 wayne      (503) staff       (20)     1555 2023-11-05 05:52:08.000000 pywayne-1.0.0.7.6/setup.py
```

### Comparing `pywayne-1.0.0.7.5/LICENSE` & `pywayne-1.0.0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.7.5/PKG-INFO` & `pywayne-1.0.0.7.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywayne
-Version: 1.0.0.7.5
+Version: 1.0.0.7.6
 Summary: Some useful tools
 Home-page: https://github.com/wangyendt/wangye_algorithm_lib
 Author: Wayne
 Author-email: wang121ye@hotmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -25,16 +25,14 @@
 Requires-Dist: tqdm
 Requires-Dist: pillow
 Requires-Dist: pyyaml
 Requires-Dist: requests
 Requires-Dist: boto3
 Requires-Dist: botocore
 Requires-Dist: setuptools
-Requires-Dist: qmt
-Requires-Dist: vqf
 
 # This is a useful tool for python and c++ (pybind)
 
 ## Currently includes:
 - data-structure
 - dsp
 - gui
```

### Comparing `pywayne-1.0.0.7.5/README.md` & `pywayne-1.0.0.7.6/README.md`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.7.5/bin/gettool.py` & `pywayne-1.0.0.7.6/bin/gettool.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.7.5/pywayne/adb/logcat_reader.py` & `pywayne-1.0.0.7.6/pywayne/adb/logcat_reader.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.7.5/pywayne/ahrs/tools.py` & `pywayne-1.0.0.7.6/pywayne/ahrs/tools.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.7.5/pywayne/calibration/magnetometer_calibration.py` & `pywayne-1.0.0.7.6/pywayne/calibration/magnetometer_calibration.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.7.5/pywayne/data_structure.py` & `pywayne-1.0.0.7.6/pywayne/data_structure.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.7.5/pywayne/dsp.py` & `pywayne-1.0.0.7.6/pywayne/dsp.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.7.5/pywayne/gui.py` & `pywayne-1.0.0.7.6/pywayne/gui.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.7.5/pywayne/math.py` & `pywayne-1.0.0.7.6/pywayne/math.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.7.5/pywayne/plot.py` & `pywayne-1.0.0.7.6/pywayne/plot.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.7.5/pywayne/tools.py` & `pywayne-1.0.0.7.6/pywayne/tools.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.7.5/pywayne/vio/tools.py` & `pywayne-1.0.0.7.6/pywayne/vio/tools.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.7.5/pywayne/visualization/pangolin.py` & `pywayne-1.0.0.7.6/pywayne/visualization/pangolin.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.7.5/pywayne.egg-info/PKG-INFO` & `pywayne-1.0.0.7.6/pywayne.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywayne
-Version: 1.0.0.7.5
+Version: 1.0.0.7.6
 Summary: Some useful tools
 Home-page: https://github.com/wangyendt/wangye_algorithm_lib
 Author: Wayne
 Author-email: wang121ye@hotmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -25,16 +25,14 @@
 Requires-Dist: tqdm
 Requires-Dist: pillow
 Requires-Dist: pyyaml
 Requires-Dist: requests
 Requires-Dist: boto3
 Requires-Dist: botocore
 Requires-Dist: setuptools
-Requires-Dist: qmt
-Requires-Dist: vqf
 
 # This is a useful tool for python and c++ (pybind)
 
 ## Currently includes:
 - data-structure
 - dsp
 - gui
```

### Comparing `pywayne-1.0.0.7.5/pywayne.egg-info/SOURCES.txt` & `pywayne-1.0.0.7.6/pywayne.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.7.5/setup.py` & `pywayne-1.0.0.7.6/setup.py`

 * *Files identical despite different names*

