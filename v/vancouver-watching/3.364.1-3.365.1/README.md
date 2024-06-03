# Comparing `tmp/vancouver_watching-3.364.1.tar.gz` & `tmp/vancouver_watching-3.365.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vancouver_watching-3.364.1.tar", last modified: Fri May 31 02:52:26 2024, max compression
+gzip compressed data, was "vancouver_watching-3.365.1.tar", last modified: Mon Jun  3 06:05:24 2024, max compression
```

## Comparing `vancouver_watching-3.364.1.tar` & `vancouver_watching-3.365.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-31 02:52:26.804058 vancouver_watching-3.364.1/
--rw-r--r--   0 kamangir   (502) staff       (20)     7048 2024-05-26 04:17:22.000000 vancouver_watching-3.364.1/LICENSE
--rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-26 04:17:22.000000 vancouver_watching-3.364.1/MANIFEST.in
--rw-r--r--   0 kamangir   (502) staff       (20)     4633 2024-05-31 02:52:26.803389 vancouver_watching-3.364.1/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)     3611 2024-05-26 04:17:22.000000 vancouver_watching-3.364.1/README.md
--rw-r--r--   0 kamangir   (502) staff       (20)       81 2024-05-26 04:17:22.000000 vancouver_watching-3.364.1/pyproject.toml
--rw-r--r--   0 kamangir   (502) staff       (20)      156 2024-05-26 04:17:22.000000 vancouver_watching-3.364.1/requirements.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-31 02:52:26.804282 vancouver_watching-3.364.1/setup.cfg
--rw-r--r--   0 kamangir   (502) staff       (20)      385 2024-05-26 20:40:48.000000 vancouver_watching-3.364.1/setup.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-31 02:52:26.794736 vancouver_watching-3.364.1/vancouver_watching/
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-31 02:52:26.800224 vancouver_watching-3.364.1/vancouver_watching/.abcli/
--rw-r--r--   0 kamangir   (502) staff       (20)      166 2024-05-26 17:36:39.000000 vancouver_watching-3.364.1/vancouver_watching/.abcli/actions.sh
--rw-r--r--   0 kamangir   (502) staff       (20)       74 2024-05-26 17:36:39.000000 vancouver_watching-3.364.1/vancouver_watching/.abcli/aka.sh
--rw-r--r--   0 kamangir   (502) staff       (20)       65 2024-05-26 17:36:39.000000 vancouver_watching-3.364.1/vancouver_watching/.abcli/alias.sh
--rw-r--r--   0 kamangir   (502) staff       (20)     1109 2024-05-26 17:36:39.000000 vancouver_watching-3.364.1/vancouver_watching/.abcli/discover.sh
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-31 02:52:26.801228 vancouver_watching-3.364.1/vancouver_watching/.abcli/discovery/
--rw-r--r--   0 kamangir   (502) staff       (20)      225 2024-05-26 17:36:39.000000 vancouver_watching-3.364.1/vancouver_watching/.abcli/discovery/iran.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      458 2024-05-26 17:36:39.000000 vancouver_watching-3.364.1/vancouver_watching/.abcli/discovery/vancouver.sh
--rw-r--r--   0 kamangir   (502) staff       (20)     2258 2024-05-26 17:36:39.000000 vancouver_watching-3.364.1/vancouver_watching/.abcli/ingest.sh
--rw-r--r--   0 kamangir   (502) staff       (20)     1041 2024-05-26 17:36:39.000000 vancouver_watching-3.364.1/vancouver_watching/.abcli/list.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      982 2024-05-26 17:36:39.000000 vancouver_watching-3.364.1/vancouver_watching/.abcli/openai_vision.sh
--rw-r--r--   0 kamangir   (502) staff       (20)     1763 2024-05-26 17:36:39.000000 vancouver_watching-3.364.1/vancouver_watching/.abcli/process.sh
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-31 02:52:26.802105 vancouver_watching-3.364.1/vancouver_watching/.abcli/tests/
--rw-r--r--   0 kamangir   (502) staff       (20)      549 2024-05-26 17:36:39.000000 vancouver_watching-3.364.1/vancouver_watching/.abcli/tests/ingest.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      341 2024-05-26 17:36:39.000000 vancouver_watching-3.364.1/vancouver_watching/.abcli/tests/list.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      403 2024-05-26 17:36:39.000000 vancouver_watching-3.364.1/vancouver_watching/.abcli/tests/process.sh
--rw-r--r--   0 kamangir   (502) staff       (20)     2618 2024-05-26 17:36:39.000000 vancouver_watching-3.364.1/vancouver_watching/.abcli/update.sh
--rwxr-xr-x   0 kamangir   (502) staff       (20)      745 2024-05-26 17:36:39.000000 vancouver_watching-3.364.1/vancouver_watching/.abcli/vancouver_watching.sh
--rw-r--r--   0 kamangir   (502) staff       (20)     4758 2024-05-26 04:17:22.000000 vancouver_watching-3.364.1/vancouver_watching/QGIS.py
--rw-r--r--   0 kamangir   (502) staff       (20)      151 2024-05-31 02:52:20.000000 vancouver_watching-3.364.1/vancouver_watching/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     1302 2024-05-28 01:10:45.000000 vancouver_watching-3.364.1/vancouver_watching/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     6783 2024-05-26 04:17:22.000000 vancouver_watching-3.364.1/vancouver_watching/area.py
--rw-r--r--   0 kamangir   (502) staff       (20)      127 2024-05-26 04:17:22.000000 vancouver_watching-3.364.1/vancouver_watching/config.env
--rw-r--r--   0 kamangir   (502) staff       (20)      284 2024-05-26 04:17:22.000000 vancouver_watching-3.364.1/vancouver_watching/env.py
--rw-r--r--   0 kamangir   (502) staff       (20)       99 2024-05-26 04:17:22.000000 vancouver_watching-3.364.1/vancouver_watching/logger.py
--rw-r--r--   0 kamangir   (502) staff       (20)      355 2024-05-26 04:17:22.000000 vancouver_watching-3.364.1/vancouver_watching/notebook.py
--rw-r--r--   0 kamangir   (502) staff       (20)       17 2024-05-26 04:17:22.000000 vancouver_watching-3.364.1/vancouver_watching/urls.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-31 02:52:26.802513 vancouver_watching-3.364.1/vancouver_watching.egg-info/
--rw-r--r--   0 kamangir   (502) staff       (20)     4633 2024-05-31 02:52:26.000000 vancouver_watching-3.364.1/vancouver_watching.egg-info/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)     1133 2024-05-31 02:52:26.000000 vancouver_watching-3.364.1/vancouver_watching.egg-info/SOURCES.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-31 02:52:26.000000 vancouver_watching-3.364.1/vancouver_watching.egg-info/dependency_links.txt
--rw-r--r--   0 kamangir   (502) staff       (20)      156 2024-05-31 02:52:26.000000 vancouver_watching-3.364.1/vancouver_watching.egg-info/requires.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       19 2024-05-31 02:52:26.000000 vancouver_watching-3.364.1/vancouver_watching.egg-info/top_level.txt
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 06:05:24.301697 vancouver_watching-3.365.1/
+-rw-r--r--   0 kamangir   (502) staff       (20)     7048 2024-05-26 04:17:22.000000 vancouver_watching-3.365.1/LICENSE
+-rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-26 04:17:22.000000 vancouver_watching-3.365.1/MANIFEST.in
+-rw-r--r--   0 kamangir   (502) staff       (20)     4682 2024-06-03 06:05:24.301047 vancouver_watching-3.365.1/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)     3660 2024-06-03 06:05:07.000000 vancouver_watching-3.365.1/README.md
+-rw-r--r--   0 kamangir   (502) staff       (20)       81 2024-05-26 04:17:22.000000 vancouver_watching-3.365.1/pyproject.toml
+-rw-r--r--   0 kamangir   (502) staff       (20)      156 2024-05-26 04:17:22.000000 vancouver_watching-3.365.1/requirements.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-06-03 06:05:24.301831 vancouver_watching-3.365.1/setup.cfg
+-rw-r--r--   0 kamangir   (502) staff       (20)      385 2024-05-26 20:40:48.000000 vancouver_watching-3.365.1/setup.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 06:05:24.290336 vancouver_watching-3.365.1/vancouver_watching/
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 06:05:24.297536 vancouver_watching-3.365.1/vancouver_watching/.abcli/
+-rw-r--r--   0 kamangir   (502) staff       (20)      166 2024-05-26 17:36:39.000000 vancouver_watching-3.365.1/vancouver_watching/.abcli/actions.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)       74 2024-05-26 17:36:39.000000 vancouver_watching-3.365.1/vancouver_watching/.abcli/aka.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)       65 2024-05-26 17:36:39.000000 vancouver_watching-3.365.1/vancouver_watching/.abcli/alias.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     1109 2024-05-26 17:36:39.000000 vancouver_watching-3.365.1/vancouver_watching/.abcli/discover.sh
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 06:05:24.298412 vancouver_watching-3.365.1/vancouver_watching/.abcli/discovery/
+-rw-r--r--   0 kamangir   (502) staff       (20)      225 2024-05-26 17:36:39.000000 vancouver_watching-3.365.1/vancouver_watching/.abcli/discovery/iran.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      458 2024-05-26 17:36:39.000000 vancouver_watching-3.365.1/vancouver_watching/.abcli/discovery/vancouver.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     2258 2024-05-26 17:36:39.000000 vancouver_watching-3.365.1/vancouver_watching/.abcli/ingest.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     1041 2024-05-26 17:36:39.000000 vancouver_watching-3.365.1/vancouver_watching/.abcli/list.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      982 2024-05-26 17:36:39.000000 vancouver_watching-3.365.1/vancouver_watching/.abcli/openai_vision.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     1763 2024-05-26 17:36:39.000000 vancouver_watching-3.365.1/vancouver_watching/.abcli/process.sh
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 06:05:24.299720 vancouver_watching-3.365.1/vancouver_watching/.abcli/tests/
+-rw-r--r--   0 kamangir   (502) staff       (20)      549 2024-05-26 17:36:39.000000 vancouver_watching-3.365.1/vancouver_watching/.abcli/tests/ingest.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      341 2024-05-26 17:36:39.000000 vancouver_watching-3.365.1/vancouver_watching/.abcli/tests/list.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      403 2024-05-26 17:36:39.000000 vancouver_watching-3.365.1/vancouver_watching/.abcli/tests/process.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     2618 2024-05-26 17:36:39.000000 vancouver_watching-3.365.1/vancouver_watching/.abcli/update.sh
+-rwxr-xr-x   0 kamangir   (502) staff       (20)      745 2024-05-26 17:36:39.000000 vancouver_watching-3.365.1/vancouver_watching/.abcli/vancouver_watching.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     4758 2024-05-26 04:17:22.000000 vancouver_watching-3.365.1/vancouver_watching/QGIS.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      151 2024-06-03 06:05:19.000000 vancouver_watching-3.365.1/vancouver_watching/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     1302 2024-05-28 01:10:45.000000 vancouver_watching-3.365.1/vancouver_watching/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     6783 2024-05-26 04:17:22.000000 vancouver_watching-3.365.1/vancouver_watching/area.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      127 2024-05-26 04:17:22.000000 vancouver_watching-3.365.1/vancouver_watching/config.env
+-rw-r--r--   0 kamangir   (502) staff       (20)      284 2024-05-26 04:17:22.000000 vancouver_watching-3.365.1/vancouver_watching/env.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       99 2024-05-26 04:17:22.000000 vancouver_watching-3.365.1/vancouver_watching/logger.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      355 2024-05-26 04:17:22.000000 vancouver_watching-3.365.1/vancouver_watching/notebook.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       17 2024-05-26 04:17:22.000000 vancouver_watching-3.365.1/vancouver_watching/urls.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 06:05:24.300237 vancouver_watching-3.365.1/vancouver_watching.egg-info/
+-rw-r--r--   0 kamangir   (502) staff       (20)     4682 2024-06-03 06:05:24.000000 vancouver_watching-3.365.1/vancouver_watching.egg-info/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)     1133 2024-06-03 06:05:24.000000 vancouver_watching-3.365.1/vancouver_watching.egg-info/SOURCES.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-06-03 06:05:24.000000 vancouver_watching-3.365.1/vancouver_watching.egg-info/dependency_links.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)      156 2024-06-03 06:05:24.000000 vancouver_watching-3.365.1/vancouver_watching.egg-info/requires.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       19 2024-06-03 06:05:24.000000 vancouver_watching-3.365.1/vancouver_watching.egg-info/top_level.txt
```

### Comparing `vancouver_watching-3.364.1/LICENSE` & `vancouver_watching-3.365.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vancouver_watching-3.364.1/PKG-INFO` & `vancouver_watching-3.365.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vancouver_watching
-Version: 3.364.1
+Version: 3.365.1
 Summary: 🌈 Vancouver Watching with AI.
 Home-page: https://github.com/kamangir/vancouver-watching
 Author: Arash Abadpour (Kamangir)
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
@@ -25,17 +25,21 @@
 Requires-Dist: pyyaml
 Requires-Dist: pylint
 Requires-Dist: pytest
 Requires-Dist: python-dotenv[cli]
 Requires-Dist: requests
 Requires-Dist: tqdm
 
-# Vancouver Watching (`vanwatch`) 🌈
+# 🌈 Vancouver Watching (`vanwatch`)
 
-`vanwatch` 🌈 discovers and ingests images from traffic cameras in an area and then runs [YOLO 🚀](https://github.com/ultralytics/ultralytics), [OpenAI Vision](https://github.com/kamangir/openai_commands#vision), and other vision algo to extract information about urban activity at scale. Also see [`@vanwatch`](https://github.com/kamangir/notebooks-and-scripts/tree/main/scripts#vanwatch).
+`vanwatch` 🌈 discovers and ingests images from traffic cameras in an area and then runs [YOLO 🚀](https://github.com/ultralytics/ultralytics), [OpenAI Vision](https://github.com/kamangir/openai_commands#vision), and other vision algo to extract information about urban activity at scale.
+
+```bash
+pip install vancouver-watching
+```
 
 ```bash
  > vanwatch help
 vanwatch conda create [validate,~recreate]
  . create conda environment.
 vanwatch conda validate
  . validate conda environment.
@@ -78,39 +82,33 @@
 	[--verbose 1]
  . update QGIS cache.
 vancouver_watching test \
 	[dryrun,~ingest,~list,~process,upload]
  . test vancouver_watching.
 ```
 
----
-
-last build [🔗](https://kamangir-public.s3.ca-central-1.amazonaws.com/test_vancouver_watching_ingest/animation.gif):
+last build [🔗](https://kamangir-public.s3.ca-central-1.amazonaws.com/test_vancouver_watching_ingest/animation.gif) ![image](https://kamangir-public.s3.ca-central-1.amazonaws.com/test_vancouver_watching_ingest/animation.gif?raw=true)
 
-![image](https://kamangir-public.s3.ca-central-1.amazonaws.com/test_vancouver_watching_ingest/animation.gif?raw=true)
-
----
-
-## Discover and Ingest an Area
+## discover and Ingest an Area
 
 ![image](https://user-images.githubusercontent.com/1007567/196573547-b1c71b3b-7fac-4d2c-bba0-a87b063830da.png)
 
-To see the list of areas supported by `vanwatch` type in,
+to see the list of areas supported by `vanwatch` type in,
 
 ```bash
 vanwatch list areas
 ```
 
-To discover the available cameras in an area type in,
+to discover the available cameras in an area type in,
 
 ```bash
 vanwatch discover area=vancouver
 ```
 
-You have generated a `geojson` of [traffic images in the City of Vancouver](https://raw.githubusercontent.com/kamangir/vancouver-watching/main/data/vancouver.geojson). Now, you can ingest the traffic images from this area and detect people and cars in them,
+you have generated a `geojson` of [traffic images in the City of Vancouver](https://raw.githubusercontent.com/kamangir/vancouver-watching/main/data/vancouver.geojson). Now, you can ingest the traffic images from this area and detect people and cars in them,
 
 ```bash
 vanwatch ingest area=vancouver,count=2,publish
 ```
 
 ![image](https://github.com/kamangir/assets/blob/main/vanwatch/2023-11-25-openai-vision/DavieWestBute-inference.jpg?raw=true)
 
@@ -122,8 +120,10 @@
 
 ![image](https://github.com/kamangir/assets/blob/main/vanwatch/2024-01-06-20-39-46-73614-QGIS.gif?raw=true?raw=1)
 
 dataset: [vanwatch-cache-2024-02-28-21-04-19-26236.tar.gz](https://kamangir-public.s3.ca-central-1.amazonaws.com/vanwatch-cache-2024-02-28-21-04-19-26236.tar.gz) ([details](https://medium.com/@arash-kamangir/vancouver-watching-with-ai-37-72b6a032b7fa)).
 
 ---
 
-To use on [AWS SageMaker](https://aws.amazon.com/sagemaker/) replace `<plugin-name>` with `vanwatch` and follow [these instructions](https://github.com/kamangir/blue-plugin/blob/main/SageMaker.md).
+[![PyPI version](https://img.shields.io/pypi/v/vancouver-watching.svg)](https://pypi.org/project/vancouver-watching/)
+
+to use on [AWS SageMaker](https://aws.amazon.com/sagemaker/) replace `<plugin-name>` with `vanwatch` and follow [these instructions](https://github.com/kamangir/blue-plugin/blob/main/SageMaker.md).
```

### Comparing `vancouver_watching-3.364.1/README.md` & `vancouver_watching-3.365.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,14 @@
-# Vancouver Watching (`vanwatch`) 🌈
+# 🌈 Vancouver Watching (`vanwatch`)
 
-`vanwatch` 🌈 discovers and ingests images from traffic cameras in an area and then runs [YOLO 🚀](https://github.com/ultralytics/ultralytics), [OpenAI Vision](https://github.com/kamangir/openai_commands#vision), and other vision algo to extract information about urban activity at scale. Also see [`@vanwatch`](https://github.com/kamangir/notebooks-and-scripts/tree/main/scripts#vanwatch).
+`vanwatch` 🌈 discovers and ingests images from traffic cameras in an area and then runs [YOLO 🚀](https://github.com/ultralytics/ultralytics), [OpenAI Vision](https://github.com/kamangir/openai_commands#vision), and other vision algo to extract information about urban activity at scale.
+
+```bash
+pip install vancouver-watching
+```
 
 ```bash
  > vanwatch help
 vanwatch conda create [validate,~recreate]
  . create conda environment.
 vanwatch conda validate
  . validate conda environment.
@@ -47,39 +51,33 @@
 	[--verbose 1]
  . update QGIS cache.
 vancouver_watching test \
 	[dryrun,~ingest,~list,~process,upload]
  . test vancouver_watching.
 ```
 
----
-
-last build [🔗](https://kamangir-public.s3.ca-central-1.amazonaws.com/test_vancouver_watching_ingest/animation.gif):
+last build [🔗](https://kamangir-public.s3.ca-central-1.amazonaws.com/test_vancouver_watching_ingest/animation.gif) ![image](https://kamangir-public.s3.ca-central-1.amazonaws.com/test_vancouver_watching_ingest/animation.gif?raw=true)
 
-![image](https://kamangir-public.s3.ca-central-1.amazonaws.com/test_vancouver_watching_ingest/animation.gif?raw=true)
-
----
-
-## Discover and Ingest an Area
+## discover and Ingest an Area
 
 ![image](https://user-images.githubusercontent.com/1007567/196573547-b1c71b3b-7fac-4d2c-bba0-a87b063830da.png)
 
-To see the list of areas supported by `vanwatch` type in,
+to see the list of areas supported by `vanwatch` type in,
 
 ```bash
 vanwatch list areas
 ```
 
-To discover the available cameras in an area type in,
+to discover the available cameras in an area type in,
 
 ```bash
 vanwatch discover area=vancouver
 ```
 
-You have generated a `geojson` of [traffic images in the City of Vancouver](./data/vancouver.geojson). Now, you can ingest the traffic images from this area and detect people and cars in them,
+you have generated a `geojson` of [traffic images in the City of Vancouver](./data/vancouver.geojson). Now, you can ingest the traffic images from this area and detect people and cars in them,
 
 ```bash
 vanwatch ingest area=vancouver,count=2,publish
 ```
 
 ![image](https://github.com/kamangir/assets/blob/main/vanwatch/2023-11-25-openai-vision/DavieWestBute-inference.jpg?raw=true)
 
@@ -91,8 +89,10 @@
 
 ![image](https://github.com/kamangir/assets/blob/main/vanwatch/2024-01-06-20-39-46-73614-QGIS.gif?raw=true?raw=1)
 
 dataset: [vanwatch-cache-2024-02-28-21-04-19-26236.tar.gz](https://kamangir-public.s3.ca-central-1.amazonaws.com/vanwatch-cache-2024-02-28-21-04-19-26236.tar.gz) ([details](https://medium.com/@arash-kamangir/vancouver-watching-with-ai-37-72b6a032b7fa)).
 
 ---
 
-To use on [AWS SageMaker](https://aws.amazon.com/sagemaker/) replace `<plugin-name>` with `vanwatch` and follow [these instructions](https://github.com/kamangir/blue-plugin/blob/main/SageMaker.md).
+[![PyPI version](https://img.shields.io/pypi/v/vancouver-watching.svg)](https://pypi.org/project/vancouver-watching/)
+
+to use on [AWS SageMaker](https://aws.amazon.com/sagemaker/) replace `<plugin-name>` with `vanwatch` and follow [these instructions](https://github.com/kamangir/blue-plugin/blob/main/SageMaker.md).
```

### Comparing `vancouver_watching-3.364.1/vancouver_watching/.abcli/discover.sh` & `vancouver_watching-3.365.1/vancouver_watching/.abcli/discover.sh`

 * *Files identical despite different names*

### Comparing `vancouver_watching-3.364.1/vancouver_watching/.abcli/ingest.sh` & `vancouver_watching-3.365.1/vancouver_watching/.abcli/ingest.sh`

 * *Files identical despite different names*

### Comparing `vancouver_watching-3.364.1/vancouver_watching/.abcli/list.sh` & `vancouver_watching-3.365.1/vancouver_watching/.abcli/list.sh`

 * *Files identical despite different names*

### Comparing `vancouver_watching-3.364.1/vancouver_watching/.abcli/openai_vision.sh` & `vancouver_watching-3.365.1/vancouver_watching/.abcli/openai_vision.sh`

 * *Files identical despite different names*

### Comparing `vancouver_watching-3.364.1/vancouver_watching/.abcli/process.sh` & `vancouver_watching-3.365.1/vancouver_watching/.abcli/process.sh`

 * *Files identical despite different names*

### Comparing `vancouver_watching-3.364.1/vancouver_watching/.abcli/tests/ingest.sh` & `vancouver_watching-3.365.1/vancouver_watching/.abcli/tests/ingest.sh`

 * *Files identical despite different names*

### Comparing `vancouver_watching-3.364.1/vancouver_watching/.abcli/update.sh` & `vancouver_watching-3.365.1/vancouver_watching/.abcli/update.sh`

 * *Files identical despite different names*

### Comparing `vancouver_watching-3.364.1/vancouver_watching/.abcli/vancouver_watching.sh` & `vancouver_watching-3.365.1/vancouver_watching/.abcli/vancouver_watching.sh`

 * *Files identical despite different names*

### Comparing `vancouver_watching-3.364.1/vancouver_watching/QGIS.py` & `vancouver_watching-3.365.1/vancouver_watching/QGIS.py`

 * *Files identical despite different names*

### Comparing `vancouver_watching-3.364.1/vancouver_watching/__main__.py` & `vancouver_watching-3.365.1/vancouver_watching/__main__.py`

 * *Files identical despite different names*

### Comparing `vancouver_watching-3.364.1/vancouver_watching/area.py` & `vancouver_watching-3.365.1/vancouver_watching/area.py`

 * *Files identical despite different names*

### Comparing `vancouver_watching-3.364.1/vancouver_watching.egg-info/PKG-INFO` & `vancouver_watching-3.365.1/vancouver_watching.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vancouver_watching
-Version: 3.364.1
+Version: 3.365.1
 Summary: 🌈 Vancouver Watching with AI.
 Home-page: https://github.com/kamangir/vancouver-watching
 Author: Arash Abadpour (Kamangir)
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
@@ -25,17 +25,21 @@
 Requires-Dist: pyyaml
 Requires-Dist: pylint
 Requires-Dist: pytest
 Requires-Dist: python-dotenv[cli]
 Requires-Dist: requests
 Requires-Dist: tqdm
 
-# Vancouver Watching (`vanwatch`) 🌈
+# 🌈 Vancouver Watching (`vanwatch`)
 
-`vanwatch` 🌈 discovers and ingests images from traffic cameras in an area and then runs [YOLO 🚀](https://github.com/ultralytics/ultralytics), [OpenAI Vision](https://github.com/kamangir/openai_commands#vision), and other vision algo to extract information about urban activity at scale. Also see [`@vanwatch`](https://github.com/kamangir/notebooks-and-scripts/tree/main/scripts#vanwatch).
+`vanwatch` 🌈 discovers and ingests images from traffic cameras in an area and then runs [YOLO 🚀](https://github.com/ultralytics/ultralytics), [OpenAI Vision](https://github.com/kamangir/openai_commands#vision), and other vision algo to extract information about urban activity at scale.
+
+```bash
+pip install vancouver-watching
+```
 
 ```bash
  > vanwatch help
 vanwatch conda create [validate,~recreate]
  . create conda environment.
 vanwatch conda validate
  . validate conda environment.
@@ -78,39 +82,33 @@
 	[--verbose 1]
  . update QGIS cache.
 vancouver_watching test \
 	[dryrun,~ingest,~list,~process,upload]
  . test vancouver_watching.
 ```
 
----
-
-last build [🔗](https://kamangir-public.s3.ca-central-1.amazonaws.com/test_vancouver_watching_ingest/animation.gif):
+last build [🔗](https://kamangir-public.s3.ca-central-1.amazonaws.com/test_vancouver_watching_ingest/animation.gif) ![image](https://kamangir-public.s3.ca-central-1.amazonaws.com/test_vancouver_watching_ingest/animation.gif?raw=true)
 
-![image](https://kamangir-public.s3.ca-central-1.amazonaws.com/test_vancouver_watching_ingest/animation.gif?raw=true)
-
----
-
-## Discover and Ingest an Area
+## discover and Ingest an Area
 
 ![image](https://user-images.githubusercontent.com/1007567/196573547-b1c71b3b-7fac-4d2c-bba0-a87b063830da.png)
 
-To see the list of areas supported by `vanwatch` type in,
+to see the list of areas supported by `vanwatch` type in,
 
 ```bash
 vanwatch list areas
 ```
 
-To discover the available cameras in an area type in,
+to discover the available cameras in an area type in,
 
 ```bash
 vanwatch discover area=vancouver
 ```
 
-You have generated a `geojson` of [traffic images in the City of Vancouver](https://raw.githubusercontent.com/kamangir/vancouver-watching/main/data/vancouver.geojson). Now, you can ingest the traffic images from this area and detect people and cars in them,
+you have generated a `geojson` of [traffic images in the City of Vancouver](https://raw.githubusercontent.com/kamangir/vancouver-watching/main/data/vancouver.geojson). Now, you can ingest the traffic images from this area and detect people and cars in them,
 
 ```bash
 vanwatch ingest area=vancouver,count=2,publish
 ```
 
 ![image](https://github.com/kamangir/assets/blob/main/vanwatch/2023-11-25-openai-vision/DavieWestBute-inference.jpg?raw=true)
 
@@ -122,8 +120,10 @@
 
 ![image](https://github.com/kamangir/assets/blob/main/vanwatch/2024-01-06-20-39-46-73614-QGIS.gif?raw=true?raw=1)
 
 dataset: [vanwatch-cache-2024-02-28-21-04-19-26236.tar.gz](https://kamangir-public.s3.ca-central-1.amazonaws.com/vanwatch-cache-2024-02-28-21-04-19-26236.tar.gz) ([details](https://medium.com/@arash-kamangir/vancouver-watching-with-ai-37-72b6a032b7fa)).
 
 ---
 
-To use on [AWS SageMaker](https://aws.amazon.com/sagemaker/) replace `<plugin-name>` with `vanwatch` and follow [these instructions](https://github.com/kamangir/blue-plugin/blob/main/SageMaker.md).
+[![PyPI version](https://img.shields.io/pypi/v/vancouver-watching.svg)](https://pypi.org/project/vancouver-watching/)
+
+to use on [AWS SageMaker](https://aws.amazon.com/sagemaker/) replace `<plugin-name>` with `vanwatch` and follow [these instructions](https://github.com/kamangir/blue-plugin/blob/main/SageMaker.md).
```

### Comparing `vancouver_watching-3.364.1/vancouver_watching.egg-info/SOURCES.txt` & `vancouver_watching-3.365.1/vancouver_watching.egg-info/SOURCES.txt`

 * *Files identical despite different names*

