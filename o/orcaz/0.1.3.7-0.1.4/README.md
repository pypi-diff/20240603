# Comparing `tmp/orcaz-0.1.3.7.tar.gz` & `tmp/orcaz-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orcaz-0.1.3.7.tar", last modified: Mon May 27 15:43:48 2024, max compression
+gzip compressed data, was "orcaz-0.1.4.tar", last modified: Mon Jun  3 11:14:46 2024, max compression
```

## Comparing `orcaz-0.1.3.7.tar` & `orcaz-0.1.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:43:48.367757 orcaz-0.1.3.7/
--rwxr-xr-x   0 runner    (1001) docker     (127)    35149 2024-05-27 15:43:43.000000 orcaz-0.1.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5687 2024-05-27 15:43:48.367757 orcaz-0.1.3.7/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     4789 2024-05-27 15:43:43.000000 orcaz-0.1.3.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:43:48.363757 orcaz-0.1.3.7/orcaz/
--rw-r--r--   0 runner    (1001) docker     (127)    47953 2024-05-27 15:43:43.000000 orcaz-0.1.3.7/orcaz/NiftiDataset.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       20 2024-05-27 15:43:43.000000 orcaz-0.1.3.7/orcaz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-27 15:43:43.000000 orcaz-0.1.3.7/orcaz/config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3431 2024-05-27 15:43:43.000000 orcaz-0.1.3.7/orcaz/constants.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5801 2024-05-27 15:43:43.000000 orcaz-0.1.3.7/orcaz/discriminators.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1702 2024-05-27 15:43:43.000000 orcaz-0.1.3.7/orcaz/display.py
--rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-05-27 15:43:43.000000 orcaz-0.1.3.7/orcaz/download.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4806 2024-05-27 15:43:43.000000 orcaz-0.1.3.7/orcaz/file_utilities.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16048 2024-05-27 15:43:43.000000 orcaz-0.1.3.7/orcaz/generators.py
--rw-r--r--   0 runner    (1001) docker     (127)     8565 2024-05-27 15:43:43.000000 orcaz-0.1.3.7/orcaz/image_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)    26207 2024-05-27 15:43:43.000000 orcaz-0.1.3.7/orcaz/image_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-05-27 15:43:43.000000 orcaz-0.1.3.7/orcaz/input_validation.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5672 2024-05-27 15:43:43.000000 orcaz-0.1.3.7/orcaz/options.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7285 2024-05-27 15:43:43.000000 orcaz-0.1.3.7/orcaz/orcaz.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3707 2024-05-27 15:43:43.000000 orcaz-0.1.3.7/orcaz/plot_generated_batch.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15581 2024-05-27 15:43:43.000000 orcaz-0.1.3.7/orcaz/predict_single_image.py
--rw-r--r--   0 runner    (1001) docker     (127)    10133 2024-05-27 15:43:43.000000 orcaz-0.1.3.7/orcaz/registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-05-27 15:43:43.000000 orcaz-0.1.3.7/orcaz/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-27 15:43:43.000000 orcaz-0.1.3.7/orcaz/settings.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13140 2024-05-27 15:43:43.000000 orcaz-0.1.3.7/orcaz/showcase.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10770 2024-05-27 15:43:43.000000 orcaz-0.1.3.7/orcaz/train.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2388 2024-05-27 15:43:43.000000 orcaz-0.1.3.7/orcaz/train_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:43:48.367757 orcaz-0.1.3.7/orcaz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5687 2024-05-27 15:43:48.000000 orcaz-0.1.3.7/orcaz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-27 15:43:48.000000 orcaz-0.1.3.7/orcaz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 15:43:48.000000 orcaz-0.1.3.7/orcaz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-27 15:43:48.000000 orcaz-0.1.3.7/orcaz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-27 15:43:48.000000 orcaz-0.1.3.7/orcaz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-27 15:43:48.000000 orcaz-0.1.3.7/orcaz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 15:43:48.367757 orcaz-0.1.3.7/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1312 2024-05-27 15:43:43.000000 orcaz-0.1.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:14:46.653741 orcaz-0.1.4/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    35149 2024-06-03 11:14:42.000000 orcaz-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-06-03 11:14:46.653741 orcaz-0.1.4/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4789 2024-06-03 11:14:42.000000 orcaz-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:14:46.649741 orcaz-0.1.4/orcaz/
+-rw-r--r--   0 runner    (1001) docker     (127)    47953 2024-06-03 11:14:42.000000 orcaz-0.1.4/orcaz/NiftiDataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       20 2024-06-03 11:14:42.000000 orcaz-0.1.4/orcaz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-06-03 11:14:42.000000 orcaz-0.1.4/orcaz/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3431 2024-06-03 11:14:42.000000 orcaz-0.1.4/orcaz/constants.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5801 2024-06-03 11:14:42.000000 orcaz-0.1.4/orcaz/discriminators.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1702 2024-06-03 11:14:42.000000 orcaz-0.1.4/orcaz/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-06-03 11:14:42.000000 orcaz-0.1.4/orcaz/download.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4806 2024-06-03 11:14:42.000000 orcaz-0.1.4/orcaz/file_utilities.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16048 2024-06-03 11:14:42.000000 orcaz-0.1.4/orcaz/generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8565 2024-06-03 11:14:42.000000 orcaz-0.1.4/orcaz/image_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26207 2024-06-03 11:14:42.000000 orcaz-0.1.4/orcaz/image_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-06-03 11:14:42.000000 orcaz-0.1.4/orcaz/input_validation.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5672 2024-06-03 11:14:42.000000 orcaz-0.1.4/orcaz/options.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7285 2024-06-03 11:14:42.000000 orcaz-0.1.4/orcaz/orcaz.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3707 2024-06-03 11:14:42.000000 orcaz-0.1.4/orcaz/plot_generated_batch.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15581 2024-06-03 11:14:42.000000 orcaz-0.1.4/orcaz/predict_single_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10133 2024-06-03 11:14:42.000000 orcaz-0.1.4/orcaz/registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-06-03 11:14:42.000000 orcaz-0.1.4/orcaz/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-06-03 11:14:42.000000 orcaz-0.1.4/orcaz/settings.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13140 2024-06-03 11:14:42.000000 orcaz-0.1.4/orcaz/showcase.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10770 2024-06-03 11:14:42.000000 orcaz-0.1.4/orcaz/train.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2388 2024-06-03 11:14:42.000000 orcaz-0.1.4/orcaz/train_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:14:46.653741 orcaz-0.1.4/orcaz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-06-03 11:14:46.000000 orcaz-0.1.4/orcaz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-06-03 11:14:46.000000 orcaz-0.1.4/orcaz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 11:14:46.000000 orcaz-0.1.4/orcaz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-06-03 11:14:46.000000 orcaz-0.1.4/orcaz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-06-03 11:14:46.000000 orcaz-0.1.4/orcaz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-06-03 11:14:46.000000 orcaz-0.1.4/orcaz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 11:14:46.653741 orcaz-0.1.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1310 2024-06-03 11:14:42.000000 orcaz-0.1.4/setup.py
```

### Comparing `orcaz-0.1.3.7/LICENSE` & `orcaz-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `orcaz-0.1.3.7/PKG-INFO` & `orcaz-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orcaz
-Version: 0.1.3.7
+Version: 0.1.4
 Summary: ORCA (Optimized Registration through Conditional Adversarial networks) 
 Home-page: 
 Author: Zacharias Chalampalakis, PhD, Lalith Kumar Shiyam Sundar, PhD
 Author-email: zacharias.chalampalakis@meduniwien.ac.at, lalith.shiyamsundar@meduniwien.ac.at
 License: GNU General Public License v3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `orcaz-0.1.3.7/README.md` & `orcaz-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `orcaz-0.1.3.7/orcaz/NiftiDataset.py` & `orcaz-0.1.4/orcaz/NiftiDataset.py`

 * *Files identical despite different names*

### Comparing `orcaz-0.1.3.7/orcaz/config.py` & `orcaz-0.1.4/orcaz/config.py`

 * *Files identical despite different names*

### Comparing `orcaz-0.1.3.7/orcaz/constants.py` & `orcaz-0.1.4/orcaz/constants.py`

 * *Files identical despite different names*

### Comparing `orcaz-0.1.3.7/orcaz/discriminators.py` & `orcaz-0.1.4/orcaz/discriminators.py`

 * *Files identical despite different names*

### Comparing `orcaz-0.1.3.7/orcaz/display.py` & `orcaz-0.1.4/orcaz/display.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     """
     Display WOLFZ logo
     :return:
     """
     print(' ')
     logo_color_code = constants.ANSI_BLUE
     slogan_color_code = constants.ANSI_BLUE
-    result = logo_color_code + pyfiglet.figlet_format("ORCA 0.1.2", font="slant").rstrip() + "\033[0m"
+    result = logo_color_code + pyfiglet.figlet_format("ORCA 0.1.4", font="slant").rstrip() + "\033[0m"
     text = slogan_color_code + " A part of the ENHANCE-PET framework." + "\033[0m"
     print(result)
     print(text)
     print(' ')
 
 
 def expectations():
```

### Comparing `orcaz-0.1.3.7/orcaz/download.py` & `orcaz-0.1.4/orcaz/download.py`

 * *Files identical despite different names*

### Comparing `orcaz-0.1.3.7/orcaz/file_utilities.py` & `orcaz-0.1.4/orcaz/file_utilities.py`

 * *Files identical despite different names*

### Comparing `orcaz-0.1.3.7/orcaz/generators.py` & `orcaz-0.1.4/orcaz/generators.py`

 * *Files identical despite different names*

### Comparing `orcaz-0.1.3.7/orcaz/image_conversion.py` & `orcaz-0.1.4/orcaz/image_conversion.py`

 * *Files identical despite different names*

### Comparing `orcaz-0.1.3.7/orcaz/image_processing.py` & `orcaz-0.1.4/orcaz/image_processing.py`

 * *Files identical despite different names*

### Comparing `orcaz-0.1.3.7/orcaz/input_validation.py` & `orcaz-0.1.4/orcaz/input_validation.py`

 * *Files identical despite different names*

### Comparing `orcaz-0.1.3.7/orcaz/options.py` & `orcaz-0.1.4/orcaz/options.py`

 * *Files identical despite different names*

### Comparing `orcaz-0.1.3.7/orcaz/orcaz.py` & `orcaz-0.1.4/orcaz/orcaz.py`

 * *Files identical despite different names*

### Comparing `orcaz-0.1.3.7/orcaz/plot_generated_batch.py` & `orcaz-0.1.4/orcaz/plot_generated_batch.py`

 * *Files identical despite different names*

### Comparing `orcaz-0.1.3.7/orcaz/predict_single_image.py` & `orcaz-0.1.4/orcaz/predict_single_image.py`

 * *Files identical despite different names*

### Comparing `orcaz-0.1.3.7/orcaz/registration.py` & `orcaz-0.1.4/orcaz/registration.py`

 * *Files identical despite different names*

### Comparing `orcaz-0.1.3.7/orcaz/resources.py` & `orcaz-0.1.4/orcaz/resources.py`

 * *Files 19% similar despite different names*

```diff
@@ -26,36 +26,36 @@
         "url": "https://enhance-pet.s3.eu-central-1.amazonaws.com/orca/fdg_nac_g_epoch_2000.zip",
         "filename": "fdg_nac_g_epoch_2000.zip",
         "model": "fdg_nac_g_epoch_2000.pth",
         "directory": "fdg_nac_g_epoch_2000",
         "voxel_spacing": [2.80374, 2.80374, 2.00086]
     },
     "nac_psma": {
-        "url": "http://0.0.0.0:2781/psma_nac_g_epoch_2000.zip",
+        "url": "https://enhance-pet.s3.eu-central-1.amazonaws.com/orca/psma_nac_g_epoch_2000.zip",
         "filename": "psma_nac_g_epoch_2000.zip",
         "model": "psma_nac_g_epoch_2000.pth",
         "directory": "psma_nac_g_epoch_2000",
         "voxel_spacing": [3.3, 3.3, 2]
     },
     "nac_fluciclovine": {
-        "url": "http://0.0.0.0:2781/fluciclovine_nac_g_epoch_2000.zip",
+        "url": "https://enhance-pet.s3.eu-central-1.amazonaws.com/orca/fluciclovine_nac_g_epoch_2000.zip",
         "filename": "fluciclovine_nac_g_epoch_2000.zip",
         "model": "fluciclovine_nac_g_epoch_2000.pth",
         "directory": "fluciclovine_nac_g_epoch_2000",
         "voxel_spacing": [2.34375, 2.34375, 2.344]
     },
     "nac_dotatate": {
-        "url": "http://0.0.0.0:2781/dotatate_nac_g_epoch_2000.zip",
+        "url": "https://enhance-pet.s3.eu-central-1.amazonaws.com/orca/dotatate_nac_g_epoch_2000.zip",
         "filename": "dotatate_nac_g_epoch_2000.zip",
         "model": "dotatate_nac_g_epoch_2000.pth",
         "directory": "dotatate_nac_g_epoch_2000",
         "voxel_spacing": [2.34375, 2.34375, 2.344]
     },
     "nac_agnostic": {
-        "url": "http://0.0.0.0:2781/agnostic_nac_g_epoch_2000.zip",
+        "url": "https://enhance-pet.s3.eu-central-1.amazonaws.com/orca/agnostic_nac_g_epoch_2000.zip",
         "filename": "agnostic_nac_g_epoch_2000.zip",
         "model": "agnostic_nac_g_epoch_2000.pth",
         "directory": "agnostic_nac_g_epoch_2000",
         "voxel_spacing": [2.80374, 2.80374, 2.00086]
     },
 }
```

### Comparing `orcaz-0.1.3.7/orcaz/showcase.py` & `orcaz-0.1.4/orcaz/showcase.py`

 * *Files identical despite different names*

### Comparing `orcaz-0.1.3.7/orcaz/train.py` & `orcaz-0.1.4/orcaz/train.py`

 * *Files identical despite different names*

### Comparing `orcaz-0.1.3.7/orcaz/train_utils.py` & `orcaz-0.1.4/orcaz/train_utils.py`

 * *Files identical despite different names*

### Comparing `orcaz-0.1.3.7/orcaz.egg-info/PKG-INFO` & `orcaz-0.1.4/orcaz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orcaz
-Version: 0.1.3.7
+Version: 0.1.4
 Summary: ORCA (Optimized Registration through Conditional Adversarial networks) 
 Home-page: 
 Author: Zacharias Chalampalakis, PhD, Lalith Kumar Shiyam Sundar, PhD
 Author-email: zacharias.chalampalakis@meduniwien.ac.at, lalith.shiyamsundar@meduniwien.ac.at
 License: GNU General Public License v3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `orcaz-0.1.3.7/orcaz.egg-info/SOURCES.txt` & `orcaz-0.1.4/orcaz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `orcaz-0.1.3.7/setup.py` & `orcaz-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='orcaz',
-    version='0.1.3.7',
+    version='0.1.4',
     packages=['orcaz'],
     url='',
     license='GNU General Public License v3.0',
     author='Zacharias Chalampalakis, PhD, Lalith Kumar Shiyam Sundar, PhD',
     author_email='zacharias.chalampalakis@meduniwien.ac.at, lalith.shiyamsundar@meduniwien.ac.at',
     description='ORCA (Optimized Registration through Conditional Adversarial networks) ',
     long_description_content_type="text/markdown",
```

