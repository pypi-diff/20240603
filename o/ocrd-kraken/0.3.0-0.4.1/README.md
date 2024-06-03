# Comparing `tmp/ocrd_kraken-0.3.0.tar.gz` & `tmp/ocrd_kraken-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ocrd_kraken-0.3.0.tar", last modified: Sun Oct 23 12:43:09 2022, max compression
+gzip compressed data, was "ocrd_kraken-0.4.1.tar", last modified: Wed May 29 10:39:56 2024, max compression
```

## Comparing `ocrd_kraken-0.3.0.tar` & `ocrd_kraken-0.4.1.tar`

### file list

```diff
@@ -1,31 +1,37 @@
-drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2022-10-23 12:43:09.000000 ocrd_kraken-0.3.0/
--rw-rw-r--   0 kba       (1000) kba       (1000)    11357 2021-03-16 15:02:34.000000 ocrd_kraken-0.3.0/LICENSE
-drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2022-10-23 12:43:09.000000 ocrd_kraken-0.3.0/ocrd_kraken.egg-info/
--rw-rw-r--   0 kba       (1000) kba       (1000)       23 2022-10-23 12:43:09.000000 ocrd_kraken-0.3.0/ocrd_kraken.egg-info/requires.txt
--rw-rw-r--   0 kba       (1000) kba       (1000)       18 2022-10-23 12:43:09.000000 ocrd_kraken-0.3.0/ocrd_kraken.egg-info/top_level.txt
--rw-rw-r--   0 kba       (1000) kba       (1000)      613 2022-10-23 12:43:09.000000 ocrd_kraken-0.3.0/ocrd_kraken.egg-info/SOURCES.txt
--rw-rw-r--   0 kba       (1000) kba       (1000)        1 2022-10-23 12:43:09.000000 ocrd_kraken-0.3.0/ocrd_kraken.egg-info/dependency_links.txt
--rw-rw-r--   0 kba       (1000) kba       (1000)      175 2022-10-23 12:43:09.000000 ocrd_kraken-0.3.0/ocrd_kraken.egg-info/entry_points.txt
--rw-rw-r--   0 kba       (1000) kba       (1000)     4409 2022-10-23 12:43:09.000000 ocrd_kraken-0.3.0/ocrd_kraken.egg-info/PKG-INFO
--rw-rw-r--   0 kba       (1000) kba       (1000)     1217 2022-10-23 12:37:56.000000 ocrd_kraken-0.3.0/setup.py
-drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2022-10-23 12:43:09.000000 ocrd_kraken-0.3.0/tests/
-drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2022-10-23 12:43:09.000000 ocrd_kraken-0.3.0/tests/assets/
--rw-rw-r--   0 kba       (1000) kba       (1000)       35 2022-07-22 13:45:31.000000 ocrd_kraken-0.3.0/tests/assets/param-binarize.json
--rw-rw-r--   0 kba       (1000) kba       (1000)       37 2022-07-22 13:45:31.000000 ocrd_kraken-0.3.0/tests/assets/param-binarize-invalid.json
--rw-rw-r--   0 kba       (1000) kba       (1000)     1053 2022-07-22 13:45:30.000000 ocrd_kraken-0.3.0/tests/assets/__init__.py
-drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2022-10-23 12:43:09.000000 ocrd_kraken-0.3.0/ocrd_kraken/
--rw-rw-r--   0 kba       (1000) kba       (1000)      280 2022-10-23 12:37:56.000000 ocrd_kraken-0.3.0/ocrd_kraken/cli.py
--rw-rw-r--   0 kba       (1000) kba       (1000)      172 2022-10-23 12:37:56.000000 ocrd_kraken-0.3.0/ocrd_kraken/config.py
--rw-rw-r--   0 kba       (1000) kba       (1000)     8004 2022-10-23 12:41:53.000000 ocrd_kraken-0.3.0/ocrd_kraken/ocrd-tool.json
-drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2022-10-23 12:43:09.000000 ocrd_kraken-0.3.0/ocrd_kraken/cli/
--rw-rw-r--   0 kba       (1000) kba       (1000)      267 2022-10-23 12:37:56.000000 ocrd_kraken-0.3.0/ocrd_kraken/cli/recognize.py
--rw-rw-r--   0 kba       (1000) kba       (1000)      262 2022-10-23 12:37:56.000000 ocrd_kraken-0.3.0/ocrd_kraken/cli/binarize.py
--rw-rw-r--   0 kba       (1000) kba       (1000)      258 2022-10-23 12:37:56.000000 ocrd_kraken-0.3.0/ocrd_kraken/cli/segment.py
--rw-rw-r--   0 kba       (1000) kba       (1000)        0 2022-10-23 12:37:56.000000 ocrd_kraken-0.3.0/ocrd_kraken/cli/__init__.py
--rw-rw-r--   0 kba       (1000) kba       (1000)     5699 2022-10-23 12:37:56.000000 ocrd_kraken-0.3.0/ocrd_kraken/recognize.py
--rw-rw-r--   0 kba       (1000) kba       (1000)     3479 2021-03-16 15:02:34.000000 ocrd_kraken-0.3.0/ocrd_kraken/binarize.py
--rw-rw-r--   0 kba       (1000) kba       (1000)     8311 2022-10-23 12:37:56.000000 ocrd_kraken-0.3.0/ocrd_kraken/segment.py
--rw-rw-r--   0 kba       (1000) kba       (1000)        0 2022-10-23 12:37:56.000000 ocrd_kraken-0.3.0/ocrd_kraken/__init__.py
--rw-rw-r--   0 kba       (1000) kba       (1000)     4409 2022-10-23 12:43:09.000000 ocrd_kraken-0.3.0/PKG-INFO
--rw-rw-r--   0 kba       (1000) kba       (1000)     4068 2022-10-23 12:37:56.000000 ocrd_kraken-0.3.0/README.md
--rw-rw-r--   0 kba       (1000) kba       (1000)       38 2022-10-23 12:43:09.000000 ocrd_kraken-0.3.0/setup.cfg
+drwxrwxr-x   0 xbert     (1003) users      (100)        0 2024-05-29 10:39:56.749378 ocrd_kraken-0.4.1/
+-rw-rw-r--   0 xbert     (1003) users      (100)    11357 2021-01-07 16:57:19.000000 ocrd_kraken-0.4.1/LICENSE
+-rw-rw-r--   0 xbert     (1003) users      (100)       66 2024-05-29 10:39:51.000000 ocrd_kraken-0.4.1/MANIFEST.in
+-rw-r--r--   0 xbert     (1003) users      (100)     4844 2024-05-29 10:39:56.749378 ocrd_kraken-0.4.1/PKG-INFO
+-rw-rw-r--   0 xbert     (1003) users      (100)     4413 2024-05-29 10:29:27.000000 ocrd_kraken-0.4.1/README.md
+-rw-rw-r--   0 xbert     (1003) users      (100)     9117 2024-05-29 10:31:00.000000 ocrd_kraken-0.4.1/ocrd-tool.json
+drwxrwxr-x   0 xbert     (1003) users      (100)        0 2024-05-29 10:39:56.745378 ocrd_kraken-0.4.1/ocrd_kraken/
+-rw-rw-r--   0 xbert     (1003) users      (100)        0 2023-05-25 09:24:33.000000 ocrd_kraken-0.4.1/ocrd_kraken/__init__.py
+-rw-rw-r--   0 xbert     (1003) users      (100)     5215 2024-05-29 10:29:27.000000 ocrd_kraken-0.4.1/ocrd_kraken/binarize.py
+drwxrwxr-x   0 xbert     (1003) users      (100)        0 2024-05-29 10:39:56.745378 ocrd_kraken-0.4.1/ocrd_kraken/cli/
+-rw-rw-r--   0 xbert     (1003) users      (100)        0 2023-05-25 09:24:33.000000 ocrd_kraken-0.4.1/ocrd_kraken/cli/__init__.py
+-rw-rw-r--   0 xbert     (1003) users      (100)      262 2023-05-25 09:24:33.000000 ocrd_kraken-0.4.1/ocrd_kraken/cli/binarize.py
+-rw-rw-r--   0 xbert     (1003) users      (100)      267 2023-05-25 09:24:33.000000 ocrd_kraken-0.4.1/ocrd_kraken/cli/recognize.py
+-rw-rw-r--   0 xbert     (1003) users      (100)      258 2023-05-25 09:24:33.000000 ocrd_kraken-0.4.1/ocrd_kraken/cli/segment.py
+-rw-rw-r--   0 xbert     (1003) users      (100)      280 2023-05-25 09:24:33.000000 ocrd_kraken-0.4.1/ocrd_kraken/cli.py
+-rw-rw-r--   0 xbert     (1003) users      (100)      174 2024-05-29 10:29:27.000000 ocrd_kraken-0.4.1/ocrd_kraken/config.py
+-rw-rw-r--   0 xbert     (1003) users      (100)     9117 2024-05-29 10:31:00.000000 ocrd_kraken-0.4.1/ocrd_kraken/ocrd-tool.json
+-rw-rw-r--   0 xbert     (1003) users      (100)    23443 2024-05-29 10:29:27.000000 ocrd_kraken-0.4.1/ocrd_kraken/recognize.py
+-rw-rw-r--   0 xbert     (1003) users      (100)    16323 2024-05-29 10:29:27.000000 ocrd_kraken-0.4.1/ocrd_kraken/segment.py
+drwxrwxr-x   0 xbert     (1003) users      (100)        0 2024-05-29 10:39:56.749378 ocrd_kraken-0.4.1/ocrd_kraken.egg-info/
+-rw-r--r--   0 xbert     (1003) users      (100)     4844 2024-05-29 10:39:56.000000 ocrd_kraken-0.4.1/ocrd_kraken.egg-info/PKG-INFO
+-rw-rw-r--   0 xbert     (1003) users      (100)      726 2024-05-29 10:39:56.000000 ocrd_kraken-0.4.1/ocrd_kraken.egg-info/SOURCES.txt
+-rw-rw-r--   0 xbert     (1003) users      (100)        1 2024-05-29 10:39:56.000000 ocrd_kraken-0.4.1/ocrd_kraken.egg-info/dependency_links.txt
+-rw-rw-r--   0 xbert     (1003) users      (100)      174 2024-05-29 10:39:56.000000 ocrd_kraken-0.4.1/ocrd_kraken.egg-info/entry_points.txt
+-rw-rw-r--   0 xbert     (1003) users      (100)       37 2024-05-29 10:39:56.000000 ocrd_kraken-0.4.1/ocrd_kraken.egg-info/requires.txt
+-rw-rw-r--   0 xbert     (1003) users      (100)       18 2024-05-29 10:39:56.000000 ocrd_kraken-0.4.1/ocrd_kraken.egg-info/top_level.txt
+-rw-rw-r--   0 xbert     (1003) users      (100)       42 2024-05-29 10:29:27.000000 ocrd_kraken-0.4.1/requirements.txt
+-rw-rw-r--   0 xbert     (1003) users      (100)       38 2024-05-29 10:39:56.749378 ocrd_kraken-0.4.1/setup.cfg
+-rw-rw-r--   0 xbert     (1003) users      (100)     1199 2023-08-17 12:31:36.000000 ocrd_kraken-0.4.1/setup.py
+drwxrwxr-x   0 xbert     (1003) users      (100)        0 2024-05-29 10:39:56.749378 ocrd_kraken-0.4.1/tests/
+drwxrwxr-x   0 xbert     (1003) users      (100)        0 2024-05-29 10:39:56.749378 ocrd_kraken-0.4.1/tests/assets/
+-rw-rw-r--   0 xbert     (1003) users      (100)     1053 2024-05-29 06:51:34.000000 ocrd_kraken-0.4.1/tests/assets/__init__.py
+-rw-rw-r--   0 xbert     (1003) users      (100)       37 2024-05-29 06:51:35.000000 ocrd_kraken-0.4.1/tests/assets/param-binarize-invalid.json
+-rw-rw-r--   0 xbert     (1003) users      (100)       35 2024-05-29 06:51:35.000000 ocrd_kraken-0.4.1/tests/assets/param-binarize.json
+-rw-rw-r--   0 xbert     (1003) users      (100)     1510 2024-05-29 10:29:27.000000 ocrd_kraken-0.4.1/tests/test_binarize.py
+-rw-rw-r--   0 xbert     (1003) users      (100)      962 2024-05-29 10:29:27.000000 ocrd_kraken-0.4.1/tests/test_recognize.py
+-rw-rw-r--   0 xbert     (1003) users      (100)     2137 2024-05-29 10:29:27.000000 ocrd_kraken-0.4.1/tests/test_segment.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ocrd_kraken-0.3.0/LICENSE` & `ocrd_kraken-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ocrd_kraken-0.3.0/ocrd_kraken.egg-info/SOURCES.txt` & `ocrd_kraken-0.4.1/ocrd_kraken.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 LICENSE
+MANIFEST.in
 README.md
+ocrd-tool.json
+requirements.txt
 setup.py
 ocrd_kraken/__init__.py
 ocrd_kraken/binarize.py
 ocrd_kraken/cli.py
 ocrd_kraken/config.py
 ocrd_kraken/ocrd-tool.json
 ocrd_kraken/recognize.py
@@ -14,10 +17,13 @@
 ocrd_kraken.egg-info/entry_points.txt
 ocrd_kraken.egg-info/requires.txt
 ocrd_kraken.egg-info/top_level.txt
 ocrd_kraken/cli/__init__.py
 ocrd_kraken/cli/binarize.py
 ocrd_kraken/cli/recognize.py
 ocrd_kraken/cli/segment.py
+tests/test_binarize.py
+tests/test_recognize.py
+tests/test_segment.py
 tests/assets/__init__.py
 tests/assets/param-binarize-invalid.json
 tests/assets/param-binarize.json
```

### Comparing `ocrd_kraken-0.3.0/ocrd_kraken.egg-info/PKG-INFO` & `ocrd_kraken-0.4.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
-Name: ocrd-kraken
-Version: 0.3.0
-Summary: kraken bindings
+Name: ocrd_kraken
+Version: 0.4.1
+Summary: Kraken bindings
 Home-page: https://github.com/OCR-D/ocrd_kraken
-Author: Konstantin Baierer, Kay-Michael Würzner
-Author-email: unixprog@gmail.com, wuerzner@gmail.com
+Author: Konstantin Baierer, Robert Sachunsky
+Author-email: unixprog@gmail.com, sachunsky@informatik.uni-leipzig.de
 License: Apache License 2.0
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: ocrd>=2.65
+Requires-Dist: kraken>=5.0
+Requires-Dist: scipy
+Requires-Dist: shapely
 
 # ocrd_kraken
 
 > OCR-D wrapper for the Kraken OCR engine
 
-[![image](https://travis-ci.org/OCR-D/ocrd_kraken.svg?branch=master)](https://travis-ci.org/OCR-D/ocrd_kraken)
+[![CI](https://github.com/OCR-D/ocrd_kraken/actions/workflows/ci.yml/badge.svg)](https://github.com/OCR-D/ocrd_kraken/actions/workflows/ci.yml)
 [![Docker Automated build](https://img.shields.io/docker/automated/ocrd/kraken.svg)](https://hub.docker.com/r/ocrd/kraken/tags/)
 [![image](https://circleci.com/gh/OCR-D/ocrd_kraken.svg?style=svg)](https://circleci.com/gh/OCR-D/ocrd_kraken)
 
 ## Introduction
 
 This package offers [OCR-D](https://ocr-d.de/en/spec) compliant [workspace processors](https://ocr-d.de/en/spec/cli)
 for (some of) the functionality of [Kraken](https://kraken.re).
@@ -41,15 +44,20 @@
 
     docker pull ocrd/kraken
 
 
 To run with Docker:
 
 
-    docker run -v path/to/workspaces:/data ocrd/kraken ocrd-kraken-recognize ...
+    docker run --rm \
+    -v path/to/workspaces:/data \
+    -v path/to/models:/usr/local/share/ocrd-resources \
+    ocrd/kraken ocrd-kraken-recognize ...
+    # or ocrd-kraken-segment or ocrd-kraken-binarize
+
 
 ### Native, from PyPI
 
 This is the best option if you want to use the stable, released version.
 
     pip install ocrd_kraken
 
@@ -86,25 +94,24 @@
 For details, see docstrings in the individual processors and [ocrd-tool.json](ocrd_tesserocr/ocrd-tool.json) descriptions,
 or simply `--help`.
 
 Available [OCR-D processors](https://ocr-d.de/en/spec/cli) are:
 
 - [ocrd-kraken-binarize](ocrd_kraken/binarize.py) (nlbin – not recommended)  
   - adds `AlternativeImage` files (per page, region or line) to the output fileGrp
-- [ocrd-kraken-segment](ocrd_kraken/segment.py) (all-in-one segmentation – recommended for handwriting and simply layouted prints)  
-  - adds `TextRegion`s, `TableRegion`s, `ImageRegion`s, `MathsRegion`s, `NoiseRegion`s, `ReadingOrder` and `AlternativeImage` to `Page` (depending on model training)
-  - adds `TextLine`s to `TextRegion`s, including their `Baseline`
-- [ocrd-kraken-recognize](ocrd_kraken/recognize.py)
+- [ocrd-kraken-segment](ocrd_kraken/segment.py) (all-in-one segmentation – recommended for handwriting and simply layouted prints, or as pure line segmentation)  
+  - adds `TextRegion`s to `Page` (if `level-of-operation=page`) or `TableRegion`s (if `table`)
+  - adds `TextLine`s (with `Baseline`) to `TextRegion`s (for all `level-of-operation`)
+  - masks existing segments during detection (unless `overwrite_segments`)
+- [ocrd-kraken-recognize](ocrd_kraken/recognize.py) (benefits from annotated `Baseline`s, falls back to center-normalized bboxes)
   - adds `Word`s to `TextLine`s
   - adds `Glyph`s to `Word`s
-  - adds `TextEquiv`
+  - adds `TextEquiv` (removing existing `TextEquiv` if `overwrite_text`)
 
 ## Testing
 
     make test
 
 
 This downloads test data from https://github.com/OCR-D/assets under `repo/assets`, and runs some basic tests of the Python API.
 
 Set `PYTEST_ARGS="-s --verbose"` to see log output (`-s`) and individual test results (`--verbose`).
-
-
```

### Comparing `ocrd_kraken-0.3.0/tests/assets/__init__.py` & `ocrd_kraken-0.4.1/tests/assets/__init__.py`

 * *Files identical despite different names*

### Comparing `ocrd_kraken-0.3.0/PKG-INFO` & `ocrd_kraken-0.4.1/ocrd_kraken.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: ocrd_kraken
-Version: 0.3.0
-Summary: kraken bindings
+Version: 0.4.1
+Summary: Kraken bindings
 Home-page: https://github.com/OCR-D/ocrd_kraken
-Author: Konstantin Baierer, Kay-Michael Würzner
-Author-email: unixprog@gmail.com, wuerzner@gmail.com
+Author: Konstantin Baierer, Robert Sachunsky
+Author-email: unixprog@gmail.com, sachunsky@informatik.uni-leipzig.de
 License: Apache License 2.0
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: ocrd>=2.65
+Requires-Dist: kraken>=5.0
+Requires-Dist: scipy
+Requires-Dist: shapely
 
 # ocrd_kraken
 
 > OCR-D wrapper for the Kraken OCR engine
 
-[![image](https://travis-ci.org/OCR-D/ocrd_kraken.svg?branch=master)](https://travis-ci.org/OCR-D/ocrd_kraken)
+[![CI](https://github.com/OCR-D/ocrd_kraken/actions/workflows/ci.yml/badge.svg)](https://github.com/OCR-D/ocrd_kraken/actions/workflows/ci.yml)
 [![Docker Automated build](https://img.shields.io/docker/automated/ocrd/kraken.svg)](https://hub.docker.com/r/ocrd/kraken/tags/)
 [![image](https://circleci.com/gh/OCR-D/ocrd_kraken.svg?style=svg)](https://circleci.com/gh/OCR-D/ocrd_kraken)
 
 ## Introduction
 
 This package offers [OCR-D](https://ocr-d.de/en/spec) compliant [workspace processors](https://ocr-d.de/en/spec/cli)
 for (some of) the functionality of [Kraken](https://kraken.re).
@@ -41,15 +44,20 @@
 
     docker pull ocrd/kraken
 
 
 To run with Docker:
 
 
-    docker run -v path/to/workspaces:/data ocrd/kraken ocrd-kraken-recognize ...
+    docker run --rm \
+    -v path/to/workspaces:/data \
+    -v path/to/models:/usr/local/share/ocrd-resources \
+    ocrd/kraken ocrd-kraken-recognize ...
+    # or ocrd-kraken-segment or ocrd-kraken-binarize
+
 
 ### Native, from PyPI
 
 This is the best option if you want to use the stable, released version.
 
     pip install ocrd_kraken
 
@@ -86,25 +94,24 @@
 For details, see docstrings in the individual processors and [ocrd-tool.json](ocrd_tesserocr/ocrd-tool.json) descriptions,
 or simply `--help`.
 
 Available [OCR-D processors](https://ocr-d.de/en/spec/cli) are:
 
 - [ocrd-kraken-binarize](ocrd_kraken/binarize.py) (nlbin – not recommended)  
   - adds `AlternativeImage` files (per page, region or line) to the output fileGrp
-- [ocrd-kraken-segment](ocrd_kraken/segment.py) (all-in-one segmentation – recommended for handwriting and simply layouted prints)  
-  - adds `TextRegion`s, `TableRegion`s, `ImageRegion`s, `MathsRegion`s, `NoiseRegion`s, `ReadingOrder` and `AlternativeImage` to `Page` (depending on model training)
-  - adds `TextLine`s to `TextRegion`s, including their `Baseline`
-- [ocrd-kraken-recognize](ocrd_kraken/recognize.py)
+- [ocrd-kraken-segment](ocrd_kraken/segment.py) (all-in-one segmentation – recommended for handwriting and simply layouted prints, or as pure line segmentation)  
+  - adds `TextRegion`s to `Page` (if `level-of-operation=page`) or `TableRegion`s (if `table`)
+  - adds `TextLine`s (with `Baseline`) to `TextRegion`s (for all `level-of-operation`)
+  - masks existing segments during detection (unless `overwrite_segments`)
+- [ocrd-kraken-recognize](ocrd_kraken/recognize.py) (benefits from annotated `Baseline`s, falls back to center-normalized bboxes)
   - adds `Word`s to `TextLine`s
   - adds `Glyph`s to `Word`s
-  - adds `TextEquiv`
+  - adds `TextEquiv` (removing existing `TextEquiv` if `overwrite_text`)
 
 ## Testing
 
     make test
 
 
 This downloads test data from https://github.com/OCR-D/assets under `repo/assets`, and runs some basic tests of the Python API.
 
 Set `PYTEST_ARGS="-s --verbose"` to see log output (`-s`) and individual test results (`--verbose`).
-
-
```

### Comparing `ocrd_kraken-0.3.0/README.md` & `ocrd_kraken-0.4.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # ocrd_kraken
 
 > OCR-D wrapper for the Kraken OCR engine
 
-[![image](https://travis-ci.org/OCR-D/ocrd_kraken.svg?branch=master)](https://travis-ci.org/OCR-D/ocrd_kraken)
+[![CI](https://github.com/OCR-D/ocrd_kraken/actions/workflows/ci.yml/badge.svg)](https://github.com/OCR-D/ocrd_kraken/actions/workflows/ci.yml)
 [![Docker Automated build](https://img.shields.io/docker/automated/ocrd/kraken.svg)](https://hub.docker.com/r/ocrd/kraken/tags/)
 [![image](https://circleci.com/gh/OCR-D/ocrd_kraken.svg?style=svg)](https://circleci.com/gh/OCR-D/ocrd_kraken)
 
 ## Introduction
 
 This package offers [OCR-D](https://ocr-d.de/en/spec) compliant [workspace processors](https://ocr-d.de/en/spec/cli)
 for (some of) the functionality of [Kraken](https://kraken.re).
@@ -29,15 +29,20 @@
 
     docker pull ocrd/kraken
 
 
 To run with Docker:
 
 
-    docker run -v path/to/workspaces:/data ocrd/kraken ocrd-kraken-recognize ...
+    docker run --rm \
+    -v path/to/workspaces:/data \
+    -v path/to/models:/usr/local/share/ocrd-resources \
+    ocrd/kraken ocrd-kraken-recognize ...
+    # or ocrd-kraken-segment or ocrd-kraken-binarize
+
 
 ### Native, from PyPI
 
 This is the best option if you want to use the stable, released version.
 
     pip install ocrd_kraken
 
@@ -74,21 +79,22 @@
 For details, see docstrings in the individual processors and [ocrd-tool.json](ocrd_tesserocr/ocrd-tool.json) descriptions,
 or simply `--help`.
 
 Available [OCR-D processors](https://ocr-d.de/en/spec/cli) are:
 
 - [ocrd-kraken-binarize](ocrd_kraken/binarize.py) (nlbin – not recommended)  
   - adds `AlternativeImage` files (per page, region or line) to the output fileGrp
-- [ocrd-kraken-segment](ocrd_kraken/segment.py) (all-in-one segmentation – recommended for handwriting and simply layouted prints)  
-  - adds `TextRegion`s, `TableRegion`s, `ImageRegion`s, `MathsRegion`s, `NoiseRegion`s, `ReadingOrder` and `AlternativeImage` to `Page` (depending on model training)
-  - adds `TextLine`s to `TextRegion`s, including their `Baseline`
-- [ocrd-kraken-recognize](ocrd_kraken/recognize.py)
+- [ocrd-kraken-segment](ocrd_kraken/segment.py) (all-in-one segmentation – recommended for handwriting and simply layouted prints, or as pure line segmentation)  
+  - adds `TextRegion`s to `Page` (if `level-of-operation=page`) or `TableRegion`s (if `table`)
+  - adds `TextLine`s (with `Baseline`) to `TextRegion`s (for all `level-of-operation`)
+  - masks existing segments during detection (unless `overwrite_segments`)
+- [ocrd-kraken-recognize](ocrd_kraken/recognize.py) (benefits from annotated `Baseline`s, falls back to center-normalized bboxes)
   - adds `Word`s to `TextLine`s
   - adds `Glyph`s to `Word`s
-  - adds `TextEquiv`
+  - adds `TextEquiv` (removing existing `TextEquiv` if `overwrite_text`)
 
 ## Testing
 
     make test
 
 
 This downloads test data from https://github.com/OCR-D/assets under `repo/assets`, and runs some basic tests of the Python API.
```

