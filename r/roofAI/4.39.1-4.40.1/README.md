# Comparing `tmp/roofai-4.39.1.tar.gz` & `tmp/roofai-4.40.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roofai-4.39.1.tar", last modified: Mon Jun  3 04:34:14 2024, max compression
+gzip compressed data, was "roofai-4.40.1.tar", last modified: Mon Jun  3 04:36:33 2024, max compression
```

## Comparing `roofai-4.39.1.tar` & `roofai-4.40.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:34:14.223003 roofai-4.39.1/
--rw-r--r--   0 kamangir   (502) staff       (20)     7048 2023-10-03 04:10:45.000000 roofai-4.39.1/LICENSE
--rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-20 04:50:37.000000 roofai-4.39.1/MANIFEST.in
--rw-r--r--   0 kamangir   (502) staff       (20)     4715 2024-06-03 04:34:14.222515 roofai-4.39.1/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)     3177 2024-06-03 04:34:06.000000 roofai-4.39.1/README.md
--rw-r--r--   0 kamangir   (502) staff       (20)       81 2024-05-23 04:22:10.000000 roofai-4.39.1/pyproject.toml
--rw-r--r--   0 kamangir   (502) staff       (20)      318 2024-05-20 22:40:00.000000 roofai-4.39.1/requirements.txt
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:34:14.214897 roofai-4.39.1/roofAI/
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:34:14.220128 roofai-4.39.1/roofAI/.abcli/
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:34:14.220780 roofai-4.39.1/roofAI/.abcli/QGIS/
--rw-r--r--   0 kamangir   (502) staff       (20)     1264 2024-05-26 18:51:36.000000 roofai-4.39.1/roofAI/.abcli/QGIS/expressions.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      803 2024-05-26 18:51:36.000000 roofai-4.39.1/roofAI/.abcli/QGIS/server.sh
--rw-r--r--   0 kamangir   (502) staff       (20)     1316 2024-06-03 01:49:48.000000 roofai-4.39.1/roofAI/.abcli/QGIS.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      142 2024-05-26 18:51:36.000000 roofai-4.39.1/roofAI/.abcli/actions.sh
--rw-r--r--   0 kamangir   (502) staff       (20)       58 2024-05-26 18:51:36.000000 roofai-4.39.1/roofAI/.abcli/aka.sh
--rw-r--r--   0 kamangir   (502) staff       (20)     1307 2024-05-26 18:51:36.000000 roofai-4.39.1/roofAI/.abcli/cloudwatch.sh
--rw-r--r--   0 kamangir   (502) staff       (20)     3052 2024-05-26 18:51:36.000000 roofai-4.39.1/roofAI/.abcli/conda.sh
--rw-r--r--   0 kamangir   (502) staff       (20)     4275 2024-05-26 18:51:36.000000 roofai-4.39.1/roofAI/.abcli/dataset_ingest.sh
--rw-r--r--   0 kamangir   (502) staff       (20)     1028 2024-05-26 18:51:36.000000 roofai-4.39.1/roofAI/.abcli/dataset_review.sh
--rw-r--r--   0 kamangir   (502) staff       (20)     5921 2024-05-26 18:51:36.000000 roofai-4.39.1/roofAI/.abcli/inference.sh
--rwxr-xr-x   0 kamangir   (502) staff       (20)     1682 2024-05-26 18:51:36.000000 roofai-4.39.1/roofAI/.abcli/roofAI.sh
--rw-r--r--   0 kamangir   (502) staff       (20)     4940 2024-05-26 18:51:36.000000 roofai-4.39.1/roofAI/.abcli/semseg.sh
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:34:14.221682 roofai-4.39.1/roofAI/.abcli/tests/
--rw-r--r--   0 kamangir   (502) staff       (20)      964 2024-05-26 18:51:36.000000 roofai-4.39.1/roofAI/.abcli/tests/dataset_ingest.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      863 2024-05-26 18:51:36.000000 roofai-4.39.1/roofAI/.abcli/tests/sagemaker_train.sh
--rw-r--r--   0 kamangir   (502) staff       (20)     1255 2024-05-26 18:51:36.000000 roofai-4.39.1/roofAI/.abcli/tests/semseg_train.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      106 2024-06-03 04:34:08.000000 roofai-4.39.1/roofAI/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      751 2024-03-04 07:11:52.000000 roofai-4.39.1/roofAI/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)       87 2024-03-24 00:16:41.000000 roofai-4.39.1/roofAI/logger.py
--rw-r--r--   0 kamangir   (502) staff       (20)       17 2023-10-03 04:10:45.000000 roofai-4.39.1/roofAI/urls.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:34:14.222009 roofai-4.39.1/roofAI.egg-info/
--rw-r--r--   0 kamangir   (502) staff       (20)     4715 2024-06-03 04:34:14.000000 roofai-4.39.1/roofAI.egg-info/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)      723 2024-06-03 04:34:14.000000 roofai-4.39.1/roofAI.egg-info/SOURCES.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-06-03 04:34:14.000000 roofai-4.39.1/roofAI.egg-info/dependency_links.txt
--rw-r--r--   0 kamangir   (502) staff       (20)      319 2024-06-03 04:34:14.000000 roofai-4.39.1/roofAI.egg-info/requires.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        7 2024-06-03 04:34:14.000000 roofai-4.39.1/roofAI.egg-info/top_level.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-06-03 04:34:14.223085 roofai-4.39.1/setup.cfg
--rw-r--r--   0 kamangir   (502) staff       (20)      336 2024-05-26 20:40:34.000000 roofai-4.39.1/setup.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:36:33.053660 roofai-4.40.1/
+-rw-r--r--   0 kamangir   (502) staff       (20)     7048 2023-10-03 04:10:45.000000 roofai-4.40.1/LICENSE
+-rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-20 04:50:37.000000 roofai-4.40.1/MANIFEST.in
+-rw-r--r--   0 kamangir   (502) staff       (20)     4715 2024-06-03 04:36:33.053068 roofai-4.40.1/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)     3177 2024-06-03 04:36:23.000000 roofai-4.40.1/README.md
+-rw-r--r--   0 kamangir   (502) staff       (20)       81 2024-05-23 04:22:10.000000 roofai-4.40.1/pyproject.toml
+-rw-r--r--   0 kamangir   (502) staff       (20)      318 2024-05-20 22:40:00.000000 roofai-4.40.1/requirements.txt
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:36:33.044762 roofai-4.40.1/roofAI/
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:36:33.050320 roofai-4.40.1/roofAI/.abcli/
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:36:33.051019 roofai-4.40.1/roofAI/.abcli/QGIS/
+-rw-r--r--   0 kamangir   (502) staff       (20)     1264 2024-05-26 18:51:36.000000 roofai-4.40.1/roofAI/.abcli/QGIS/expressions.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      803 2024-05-26 18:51:36.000000 roofai-4.40.1/roofAI/.abcli/QGIS/server.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     1316 2024-06-03 01:49:48.000000 roofai-4.40.1/roofAI/.abcli/QGIS.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      142 2024-05-26 18:51:36.000000 roofai-4.40.1/roofAI/.abcli/actions.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)       58 2024-05-26 18:51:36.000000 roofai-4.40.1/roofAI/.abcli/aka.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     1307 2024-05-26 18:51:36.000000 roofai-4.40.1/roofAI/.abcli/cloudwatch.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     3052 2024-05-26 18:51:36.000000 roofai-4.40.1/roofAI/.abcli/conda.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     4275 2024-05-26 18:51:36.000000 roofai-4.40.1/roofAI/.abcli/dataset_ingest.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     1028 2024-05-26 18:51:36.000000 roofai-4.40.1/roofAI/.abcli/dataset_review.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     5921 2024-05-26 18:51:36.000000 roofai-4.40.1/roofAI/.abcli/inference.sh
+-rwxr-xr-x   0 kamangir   (502) staff       (20)     1682 2024-05-26 18:51:36.000000 roofai-4.40.1/roofAI/.abcli/roofAI.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     4940 2024-05-26 18:51:36.000000 roofai-4.40.1/roofAI/.abcli/semseg.sh
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:36:33.052055 roofai-4.40.1/roofAI/.abcli/tests/
+-rw-r--r--   0 kamangir   (502) staff       (20)      964 2024-05-26 18:51:36.000000 roofai-4.40.1/roofAI/.abcli/tests/dataset_ingest.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      863 2024-05-26 18:51:36.000000 roofai-4.40.1/roofAI/.abcli/tests/sagemaker_train.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     1255 2024-05-26 18:51:36.000000 roofai-4.40.1/roofAI/.abcli/tests/semseg_train.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      106 2024-06-03 04:36:27.000000 roofai-4.40.1/roofAI/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      751 2024-03-04 07:11:52.000000 roofai-4.40.1/roofAI/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       87 2024-03-24 00:16:41.000000 roofai-4.40.1/roofAI/logger.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       17 2023-10-03 04:10:45.000000 roofai-4.40.1/roofAI/urls.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:36:33.052389 roofai-4.40.1/roofAI.egg-info/
+-rw-r--r--   0 kamangir   (502) staff       (20)     4715 2024-06-03 04:36:33.000000 roofai-4.40.1/roofAI.egg-info/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)      723 2024-06-03 04:36:33.000000 roofai-4.40.1/roofAI.egg-info/SOURCES.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-06-03 04:36:33.000000 roofai-4.40.1/roofAI.egg-info/dependency_links.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)      319 2024-06-03 04:36:33.000000 roofai-4.40.1/roofAI.egg-info/requires.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        7 2024-06-03 04:36:33.000000 roofai-4.40.1/roofAI.egg-info/top_level.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-06-03 04:36:33.053794 roofai-4.40.1/setup.cfg
+-rw-r--r--   0 kamangir   (502) staff       (20)      336 2024-05-26 20:40:34.000000 roofai-4.40.1/setup.py
```

### Comparing `roofai-4.39.1/LICENSE` & `roofai-4.40.1/LICENSE`

 * *Files identical despite different names*

### Comparing `roofai-4.39.1/PKG-INFO` & `roofai-4.40.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roofAI
-Version: 4.39.1
+Version: 4.40.1
 Summary: 🏛️ everything AI about roofs.
 Home-page: https://github.com/kamangir/roofAI
 Author: Arash Abadpour (Kamangir)
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
@@ -34,15 +34,15 @@
 Requires-Dist: scipy
 Requires-Dist: segmentation-models-pytorch
 Requires-Dist: shapely
 Requires-Dist: timm
 Requires-Dist: torch
 Requires-Dist: tqdm
 
-# roofAI 🏛️
+# 🏛️ roofAI
 
 everything AI about roofs. 🏛️
 
 🔷 [datasets](https://raw.githubusercontent.com/kamangir/roofAI/main/roofAI/dataset) 🔷 [notebooks](https://raw.githubusercontent.com/kamangir/roofAI/main/notebooks/) 🔷 [semseg](https://raw.githubusercontent.com/kamangir/roofAI/main/roofAI/semseg) 🔷 [inference](https://raw.githubusercontent.com/kamangir/roofAI/main/roofAI/inference) 🔷 [QGIS](https://raw.githubusercontent.com/kamangir/roofAI/main/roofAI/QGIS/console/) 🔷 [sagemaker](https://raw.githubusercontent.com/kamangir/roofAI/main/roofAI/semseg/sagemaker/) 🔷
 
 ![image](https://raw.githubusercontent.com/kamangir/roofAI/main/assets/predict-00247.png)
```

### Comparing `roofai-4.39.1/README.md` & `roofai-4.40.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# roofAI 🏛️
+# 🏛️ roofAI
 
 everything AI about roofs. 🏛️
 
 🔷 [datasets](./roofAI/dataset) 🔷 [notebooks](./notebooks/) 🔷 [semseg](./roofAI/semseg) 🔷 [inference](./roofAI/inference) 🔷 [QGIS](./roofAI/QGIS/console/) 🔷 [sagemaker](./roofAI/semseg/sagemaker/) 🔷
 
 ![image](./assets/predict-00247.png)
```

### Comparing `roofai-4.39.1/roofAI/.abcli/QGIS/expressions.sh` & `roofai-4.40.1/roofAI/.abcli/QGIS/expressions.sh`

 * *Files identical despite different names*

### Comparing `roofai-4.39.1/roofAI/.abcli/QGIS/server.sh` & `roofai-4.40.1/roofAI/.abcli/QGIS/server.sh`

 * *Files identical despite different names*

### Comparing `roofai-4.39.1/roofAI/.abcli/QGIS.sh` & `roofai-4.40.1/roofAI/.abcli/QGIS.sh`

 * *Files identical despite different names*

### Comparing `roofai-4.39.1/roofAI/.abcli/cloudwatch.sh` & `roofai-4.40.1/roofAI/.abcli/cloudwatch.sh`

 * *Files identical despite different names*

### Comparing `roofai-4.39.1/roofAI/.abcli/conda.sh` & `roofai-4.40.1/roofAI/.abcli/conda.sh`

 * *Files identical despite different names*

### Comparing `roofai-4.39.1/roofAI/.abcli/dataset_ingest.sh` & `roofai-4.40.1/roofAI/.abcli/dataset_ingest.sh`

 * *Files identical despite different names*

### Comparing `roofai-4.39.1/roofAI/.abcli/dataset_review.sh` & `roofai-4.40.1/roofAI/.abcli/dataset_review.sh`

 * *Files identical despite different names*

### Comparing `roofai-4.39.1/roofAI/.abcli/inference.sh` & `roofai-4.40.1/roofAI/.abcli/inference.sh`

 * *Files identical despite different names*

### Comparing `roofai-4.39.1/roofAI/.abcli/roofAI.sh` & `roofai-4.40.1/roofAI/.abcli/roofAI.sh`

 * *Files identical despite different names*

### Comparing `roofai-4.39.1/roofAI/.abcli/semseg.sh` & `roofai-4.40.1/roofAI/.abcli/semseg.sh`

 * *Files identical despite different names*

### Comparing `roofai-4.39.1/roofAI/.abcli/tests/dataset_ingest.sh` & `roofai-4.40.1/roofAI/.abcli/tests/dataset_ingest.sh`

 * *Files identical despite different names*

### Comparing `roofai-4.39.1/roofAI/.abcli/tests/sagemaker_train.sh` & `roofai-4.40.1/roofAI/.abcli/tests/sagemaker_train.sh`

 * *Files identical despite different names*

### Comparing `roofai-4.39.1/roofAI/.abcli/tests/semseg_train.sh` & `roofai-4.40.1/roofAI/.abcli/tests/semseg_train.sh`

 * *Files identical despite different names*

### Comparing `roofai-4.39.1/roofAI/__main__.py` & `roofai-4.40.1/roofAI/__main__.py`

 * *Files identical despite different names*

### Comparing `roofai-4.39.1/roofAI.egg-info/PKG-INFO` & `roofai-4.40.1/roofAI.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roofAI
-Version: 4.39.1
+Version: 4.40.1
 Summary: 🏛️ everything AI about roofs.
 Home-page: https://github.com/kamangir/roofAI
 Author: Arash Abadpour (Kamangir)
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
@@ -34,15 +34,15 @@
 Requires-Dist: scipy
 Requires-Dist: segmentation-models-pytorch
 Requires-Dist: shapely
 Requires-Dist: timm
 Requires-Dist: torch
 Requires-Dist: tqdm
 
-# roofAI 🏛️
+# 🏛️ roofAI
 
 everything AI about roofs. 🏛️
 
 🔷 [datasets](https://raw.githubusercontent.com/kamangir/roofAI/main/roofAI/dataset) 🔷 [notebooks](https://raw.githubusercontent.com/kamangir/roofAI/main/notebooks/) 🔷 [semseg](https://raw.githubusercontent.com/kamangir/roofAI/main/roofAI/semseg) 🔷 [inference](https://raw.githubusercontent.com/kamangir/roofAI/main/roofAI/inference) 🔷 [QGIS](https://raw.githubusercontent.com/kamangir/roofAI/main/roofAI/QGIS/console/) 🔷 [sagemaker](https://raw.githubusercontent.com/kamangir/roofAI/main/roofAI/semseg/sagemaker/) 🔷
 
 ![image](https://raw.githubusercontent.com/kamangir/roofAI/main/assets/predict-00247.png)
```

### Comparing `roofai-4.39.1/roofAI.egg-info/SOURCES.txt` & `roofai-4.40.1/roofAI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

