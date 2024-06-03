# Comparing `tmp/ferfereh-1.139.1.tar.gz` & `tmp/ferfereh-1.140.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ferfereh-1.139.1.tar", last modified: Mon Jun  3 01:55:31 2024, max compression
+gzip compressed data, was "ferfereh-1.140.1.tar", last modified: Mon Jun  3 05:42:15 2024, max compression
```

## Comparing `ferfereh-1.139.1.tar` & `ferfereh-1.140.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 01:55:31.790668 ferfereh-1.139.1/
--rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-21 05:59:00.000000 ferfereh-1.139.1/MANIFEST.in
--rw-r--r--   0 kamangir   (502) staff       (20)     6182 2024-06-03 01:55:31.789917 ferfereh-1.139.1/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)     4095 2024-05-21 06:02:29.000000 ferfereh-1.139.1/README.md
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 01:55:31.783446 ferfereh-1.139.1/ferfereh/
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 01:55:31.788085 ferfereh-1.139.1/ferfereh/.abcli/
--rw-r--r--   0 kamangir   (502) staff       (20)      146 2024-05-26 17:55:07.000000 ferfereh-1.139.1/ferfereh/.abcli/actions.sh
--rw-r--r--   0 kamangir   (502) staff       (20)     2354 2024-05-26 17:55:07.000000 ferfereh-1.139.1/ferfereh/.abcli/exif.sh
--rwxr-xr-x   0 kamangir   (502) staff       (20)      564 2024-05-26 17:55:07.000000 ferfereh-1.139.1/ferfereh/.abcli/ferfereh.sh
--rw-r--r--   0 kamangir   (502) staff       (20)     1832 2024-06-03 01:49:53.000000 ferfereh-1.139.1/ferfereh/.abcli/publish.sh
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 01:55:31.788489 ferfereh-1.139.1/ferfereh/.abcli/tests/
--rw-r--r--   0 kamangir   (502) staff       (20)      224 2024-05-28 01:33:21.000000 ferfereh-1.139.1/ferfereh/.abcli/tests/version.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      100 2024-06-03 01:55:26.000000 ferfereh-1.139.1/ferfereh/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      959 2024-02-25 23:42:23.000000 ferfereh-1.139.1/ferfereh/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     2768 2024-02-25 23:44:02.000000 ferfereh-1.139.1/ferfereh/coords.py
--rw-r--r--   0 kamangir   (502) staff       (20)       89 2024-03-24 00:16:12.000000 ferfereh-1.139.1/ferfereh/logger.py
--rw-r--r--   0 kamangir   (502) staff       (20)       17 2023-02-27 00:15:30.000000 ferfereh-1.139.1/ferfereh/urls.py
--rw-r--r--   0 kamangir   (502) staff       (20)      642 2024-03-04 07:37:30.000000 ferfereh-1.139.1/ferfereh/utils.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 01:55:31.789030 ferfereh-1.139.1/ferfereh.egg-info/
--rw-r--r--   0 kamangir   (502) staff       (20)     6182 2024-06-03 01:55:31.000000 ferfereh-1.139.1/ferfereh.egg-info/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)      475 2024-06-03 01:55:31.000000 ferfereh-1.139.1/ferfereh.egg-info/SOURCES.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-06-03 01:55:31.000000 ferfereh-1.139.1/ferfereh.egg-info/dependency_links.txt
--rw-r--r--   0 kamangir   (502) staff       (20)      125 2024-06-03 01:55:31.000000 ferfereh-1.139.1/ferfereh.egg-info/requires.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        9 2024-06-03 01:55:31.000000 ferfereh-1.139.1/ferfereh.egg-info/top_level.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       81 2024-05-21 05:52:18.000000 ferfereh-1.139.1/pyproject.toml
--rw-r--r--   0 kamangir   (502) staff       (20)      125 2024-05-21 05:56:20.000000 ferfereh-1.139.1/requirements.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-06-03 01:55:31.790816 ferfereh-1.139.1/setup.cfg
--rw-r--r--   0 kamangir   (502) staff       (20)      340 2024-05-26 20:37:51.000000 ferfereh-1.139.1/setup.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 05:42:15.370041 ferfereh-1.140.1/
+-rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-21 05:59:00.000000 ferfereh-1.140.1/MANIFEST.in
+-rw-r--r--   0 kamangir   (502) staff       (20)     6335 2024-06-03 05:42:15.369684 ferfereh-1.140.1/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)     4248 2024-06-03 05:41:47.000000 ferfereh-1.140.1/README.md
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 05:42:15.366314 ferfereh-1.140.1/ferfereh/
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 05:42:15.368716 ferfereh-1.140.1/ferfereh/.abcli/
+-rw-r--r--   0 kamangir   (502) staff       (20)      146 2024-05-26 17:55:07.000000 ferfereh-1.140.1/ferfereh/.abcli/actions.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     2354 2024-05-26 17:55:07.000000 ferfereh-1.140.1/ferfereh/.abcli/exif.sh
+-rwxr-xr-x   0 kamangir   (502) staff       (20)      564 2024-05-26 17:55:07.000000 ferfereh-1.140.1/ferfereh/.abcli/ferfereh.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     1832 2024-06-03 01:49:53.000000 ferfereh-1.140.1/ferfereh/.abcli/publish.sh
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 05:42:15.368953 ferfereh-1.140.1/ferfereh/.abcli/tests/
+-rw-r--r--   0 kamangir   (502) staff       (20)      224 2024-05-28 01:33:21.000000 ferfereh-1.140.1/ferfereh/.abcli/tests/version.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      100 2024-06-03 05:42:10.000000 ferfereh-1.140.1/ferfereh/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      959 2024-02-25 23:42:23.000000 ferfereh-1.140.1/ferfereh/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     2768 2024-02-25 23:44:02.000000 ferfereh-1.140.1/ferfereh/coords.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       89 2024-03-24 00:16:12.000000 ferfereh-1.140.1/ferfereh/logger.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       17 2023-02-27 00:15:30.000000 ferfereh-1.140.1/ferfereh/urls.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      642 2024-03-04 07:37:30.000000 ferfereh-1.140.1/ferfereh/utils.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 05:42:15.369261 ferfereh-1.140.1/ferfereh.egg-info/
+-rw-r--r--   0 kamangir   (502) staff       (20)     6335 2024-06-03 05:42:15.000000 ferfereh-1.140.1/ferfereh.egg-info/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)      475 2024-06-03 05:42:15.000000 ferfereh-1.140.1/ferfereh.egg-info/SOURCES.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-06-03 05:42:15.000000 ferfereh-1.140.1/ferfereh.egg-info/dependency_links.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)      125 2024-06-03 05:42:15.000000 ferfereh-1.140.1/ferfereh.egg-info/requires.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        9 2024-06-03 05:42:15.000000 ferfereh-1.140.1/ferfereh.egg-info/top_level.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       81 2024-05-21 05:52:18.000000 ferfereh-1.140.1/pyproject.toml
+-rw-r--r--   0 kamangir   (502) staff       (20)      125 2024-05-21 05:56:20.000000 ferfereh-1.140.1/requirements.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-06-03 05:42:15.370116 ferfereh-1.140.1/setup.cfg
+-rw-r--r--   0 kamangir   (502) staff       (20)      340 2024-05-26 20:37:51.000000 ferfereh-1.140.1/setup.py
```

### Comparing `ferfereh-1.139.1/PKG-INFO` & `ferfereh-1.140.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ferfereh
-Version: 1.139.1
+Version: 1.140.1
 Summary: 🌀 3d-printed graffiti.
 Home-page: https://github.com/kamangir/ferfereh
 Author: Arash Abadpour (Kamangir)
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
@@ -21,17 +21,21 @@
 Requires-Dist: pymysql==0.10.1
 Requires-Dist: pyyaml
 Requires-Dist: pylint
 Requires-Dist: pytest
 Requires-Dist: python-dotenv[cli]
 Requires-Dist: tqdm
 
-# ferfereh
+# 🌀 ferfereh
 
-Ferfereh is a 3d-printed piece of graffiti with a cloud-generated [map](https://raw.githubusercontent.com/kamangir/ferfereh/main/coords.geojson).
+🌀 `ferfereh` is a 3d-printed piece of graffiti with a cloud-generated [map](https://raw.githubusercontent.com/kamangir/ferfereh/main/coords.geojson).
+
+```bash
+pip install blue-plugin
+```
 
 ```bash
  > ferfereh help
 ferfereh cleanup
  . cleanup ferfereh.
 ferfereh exif get \
 	[-] \
@@ -86,7 +90,11 @@
 | mini pliers                                                               | ![image](https://raw.githubusercontent.com/kamangir/ferfereh/main/images/tools/mini-pliers.jpeg)                       |                                                                                    |
 | propeller fan                                                             | ![image](https://raw.githubusercontent.com/kamangir/ferfereh/main/images/tools/propellers.jpeg)                        | https://www.adafruit.com/product/3896, https://www.amazon.ca/gp/product/B091TBQ7CK |
 | double-sided, outdoor, water-resistant, mounting tape                     | ![image](https://raw.githubusercontent.com/kamangir/ferfereh/main/images/tools/mounting-tape.jpeg)                     |                                                                                    |
 | multi bit electronics screwdriver                                         | ![image](https://raw.githubusercontent.com/kamangir/ferfereh/main/images/tools/multi-bit-electronics-screwdriver.jpeg) |                                                                                    |
 | precision craft knife w/ spare blade                                      | ![image](https://raw.githubusercontent.com/kamangir/ferfereh/main/images/tools/precision-craft-knife.jpeg)             |                                                                                    |
 | small hammer                                                              | ![image](https://raw.githubusercontent.com/kamangir/ferfereh/main/images/tools/small-hammer.jpeg)                      |                                                                                    |
 | M3 Nylon Machine Screws                                                   | ![image](https://raw.githubusercontent.com/kamangir/ferfereh/main/images/tools/screws.jpg)                             | https://www.amazon.ca/gp/product/B012TACIBC                                        |
+
+---
+
+[![PyPI version](https://img.shields.io/pypi/v/ferfereh.svg)](https://pypi.org/project/ferfereh/)
```

### Comparing `ferfereh-1.139.1/README.md` & `ferfereh-1.140.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,14 @@
-# ferfereh
+# 🌀 ferfereh
 
-Ferfereh is a 3d-printed piece of graffiti with a cloud-generated [map](./coords.geojson).
+🌀 `ferfereh` is a 3d-printed piece of graffiti with a cloud-generated [map](./coords.geojson).
+
+```bash
+pip install blue-plugin
+```
 
 ```bash
  > ferfereh help
 ferfereh cleanup
  . cleanup ferfereh.
 ferfereh exif get \
 	[-] \
@@ -59,7 +63,11 @@
 | mini pliers                                                               | ![image](./images/tools/mini-pliers.jpeg)                       |                                                                                    |
 | propeller fan                                                             | ![image](./images/tools/propellers.jpeg)                        | https://www.adafruit.com/product/3896, https://www.amazon.ca/gp/product/B091TBQ7CK |
 | double-sided, outdoor, water-resistant, mounting tape                     | ![image](./images/tools/mounting-tape.jpeg)                     |                                                                                    |
 | multi bit electronics screwdriver                                         | ![image](./images/tools/multi-bit-electronics-screwdriver.jpeg) |                                                                                    |
 | precision craft knife w/ spare blade                                      | ![image](./images/tools/precision-craft-knife.jpeg)             |                                                                                    |
 | small hammer                                                              | ![image](./images/tools/small-hammer.jpeg)                      |                                                                                    |
 | M3 Nylon Machine Screws                                                   | ![image](./images/tools/screws.jpg)                             | https://www.amazon.ca/gp/product/B012TACIBC                                        |
+
+---
+
+[![PyPI version](https://img.shields.io/pypi/v/ferfereh.svg)](https://pypi.org/project/ferfereh/)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ferfereh-1.139.1/ferfereh/.abcli/exif.sh` & `ferfereh-1.140.1/ferfereh/.abcli/exif.sh`

 * *Files identical despite different names*

### Comparing `ferfereh-1.139.1/ferfereh/.abcli/ferfereh.sh` & `ferfereh-1.140.1/ferfereh/.abcli/ferfereh.sh`

 * *Files identical despite different names*

### Comparing `ferfereh-1.139.1/ferfereh/.abcli/publish.sh` & `ferfereh-1.140.1/ferfereh/.abcli/publish.sh`

 * *Files identical despite different names*

### Comparing `ferfereh-1.139.1/ferfereh/__main__.py` & `ferfereh-1.140.1/ferfereh/__main__.py`

 * *Files identical despite different names*

### Comparing `ferfereh-1.139.1/ferfereh/coords.py` & `ferfereh-1.140.1/ferfereh/coords.py`

 * *Files identical despite different names*

### Comparing `ferfereh-1.139.1/ferfereh/utils.py` & `ferfereh-1.140.1/ferfereh/utils.py`

 * *Files identical despite different names*

### Comparing `ferfereh-1.139.1/ferfereh.egg-info/PKG-INFO` & `ferfereh-1.140.1/ferfereh.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ferfereh
-Version: 1.139.1
+Version: 1.140.1
 Summary: 🌀 3d-printed graffiti.
 Home-page: https://github.com/kamangir/ferfereh
 Author: Arash Abadpour (Kamangir)
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
@@ -21,17 +21,21 @@
 Requires-Dist: pymysql==0.10.1
 Requires-Dist: pyyaml
 Requires-Dist: pylint
 Requires-Dist: pytest
 Requires-Dist: python-dotenv[cli]
 Requires-Dist: tqdm
 
-# ferfereh
+# 🌀 ferfereh
 
-Ferfereh is a 3d-printed piece of graffiti with a cloud-generated [map](https://raw.githubusercontent.com/kamangir/ferfereh/main/coords.geojson).
+🌀 `ferfereh` is a 3d-printed piece of graffiti with a cloud-generated [map](https://raw.githubusercontent.com/kamangir/ferfereh/main/coords.geojson).
+
+```bash
+pip install blue-plugin
+```
 
 ```bash
  > ferfereh help
 ferfereh cleanup
  . cleanup ferfereh.
 ferfereh exif get \
 	[-] \
@@ -86,7 +90,11 @@
 | mini pliers                                                               | ![image](https://raw.githubusercontent.com/kamangir/ferfereh/main/images/tools/mini-pliers.jpeg)                       |                                                                                    |
 | propeller fan                                                             | ![image](https://raw.githubusercontent.com/kamangir/ferfereh/main/images/tools/propellers.jpeg)                        | https://www.adafruit.com/product/3896, https://www.amazon.ca/gp/product/B091TBQ7CK |
 | double-sided, outdoor, water-resistant, mounting tape                     | ![image](https://raw.githubusercontent.com/kamangir/ferfereh/main/images/tools/mounting-tape.jpeg)                     |                                                                                    |
 | multi bit electronics screwdriver                                         | ![image](https://raw.githubusercontent.com/kamangir/ferfereh/main/images/tools/multi-bit-electronics-screwdriver.jpeg) |                                                                                    |
 | precision craft knife w/ spare blade                                      | ![image](https://raw.githubusercontent.com/kamangir/ferfereh/main/images/tools/precision-craft-knife.jpeg)             |                                                                                    |
 | small hammer                                                              | ![image](https://raw.githubusercontent.com/kamangir/ferfereh/main/images/tools/small-hammer.jpeg)                      |                                                                                    |
 | M3 Nylon Machine Screws                                                   | ![image](https://raw.githubusercontent.com/kamangir/ferfereh/main/images/tools/screws.jpg)                             | https://www.amazon.ca/gp/product/B012TACIBC                                        |
+
+---
+
+[![PyPI version](https://img.shields.io/pypi/v/ferfereh.svg)](https://pypi.org/project/ferfereh/)
```

