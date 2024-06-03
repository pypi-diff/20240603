# Comparing `tmp/subdivision_hole_filler-1.0.3.tar.gz` & `tmp/subdivision_hole_filler-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subdivision_hole_filler-1.0.3.tar", last modified: Mon Jun  3 06:52:37 2024, max compression
+gzip compressed data, was "subdivision_hole_filler-1.0.4.tar", last modified: Mon Jun  3 06:55:21 2024, max compression
```

## Comparing `subdivision_hole_filler-1.0.3.tar` & `subdivision_hole_filler-1.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:52:37.511645 subdivision_hole_filler-1.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:52:37.503645 subdivision_hole_filler-1.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:52:37.507645 subdivision_hole_filler-1.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-06-03 06:52:29.000000 subdivision_hole_filler-1.0.3/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-06-03 06:52:29.000000 subdivision_hole_filler-1.0.3/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-06-03 06:52:29.000000 subdivision_hole_filler-1.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-06-03 06:52:29.000000 subdivision_hole_filler-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)   200849 2024-06-03 06:52:29.000000 subdivision_hole_filler-1.0.3/Levin_2000_Filling N-sided Holes Using Combined Subdivision Schemes.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-06-03 06:52:37.511645 subdivision_hole_filler-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-06-03 06:52:29.000000 subdivision_hole_filler-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   106308 2024-06-03 06:52:29.000000 subdivision_hole_filler-1.0.3/iso.png
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-06-03 06:52:29.000000 subdivision_hole_filler-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 06:52:37.511645 subdivision_hole_filler-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    52038 2024-06-03 06:52:29.000000 subdivision_hole_filler-1.0.3/side.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:52:37.507645 subdivision_hole_filler-1.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:52:37.507645 subdivision_hole_filler-1.0.3/src/subdivision_hole_filler/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-06-03 06:52:29.000000 subdivision_hole_filler-1.0.3/src/subdivision_hole_filler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-06-03 06:52:37.000000 subdivision_hole_filler-1.0.3/src/subdivision_hole_filler/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    12850 2024-06-03 06:52:29.000000 subdivision_hole_filler-1.0.3/src/subdivision_hole_filler/hole_filler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:52:37.511645 subdivision_hole_filler-1.0.3/src/subdivision_hole_filler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-06-03 06:52:37.000000 subdivision_hole_filler-1.0.3/src/subdivision_hole_filler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-06-03 06:52:37.000000 subdivision_hole_filler-1.0.3/src/subdivision_hole_filler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 06:52:37.000000 subdivision_hole_filler-1.0.3/src/subdivision_hole_filler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-06-03 06:52:37.000000 subdivision_hole_filler-1.0.3/src/subdivision_hole_filler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-06-03 06:52:37.000000 subdivision_hole_filler-1.0.3/src/subdivision_hole_filler.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:52:37.511645 subdivision_hole_filler-1.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-06-03 06:52:29.000000 subdivision_hole_filler-1.0.3/tests/test_6sided_hole.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:55:21.966808 subdivision_hole_filler-1.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:55:21.958808 subdivision_hole_filler-1.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:55:21.962808 subdivision_hole_filler-1.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-06-03 06:55:17.000000 subdivision_hole_filler-1.0.4/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-06-03 06:55:17.000000 subdivision_hole_filler-1.0.4/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-06-03 06:55:17.000000 subdivision_hole_filler-1.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-06-03 06:55:17.000000 subdivision_hole_filler-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)   200849 2024-06-03 06:55:17.000000 subdivision_hole_filler-1.0.4/Levin_2000_Filling N-sided Holes Using Combined Subdivision Schemes.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-06-03 06:55:21.966808 subdivision_hole_filler-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-06-03 06:55:17.000000 subdivision_hole_filler-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   106308 2024-06-03 06:55:17.000000 subdivision_hole_filler-1.0.4/iso.png
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-06-03 06:55:17.000000 subdivision_hole_filler-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 06:55:21.966808 subdivision_hole_filler-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    52038 2024-06-03 06:55:17.000000 subdivision_hole_filler-1.0.4/side.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:55:21.962808 subdivision_hole_filler-1.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:55:21.962808 subdivision_hole_filler-1.0.4/src/subdivision_hole_filler/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-06-03 06:55:17.000000 subdivision_hole_filler-1.0.4/src/subdivision_hole_filler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-06-03 06:55:21.000000 subdivision_hole_filler-1.0.4/src/subdivision_hole_filler/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12850 2024-06-03 06:55:17.000000 subdivision_hole_filler-1.0.4/src/subdivision_hole_filler/hole_filler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:55:21.962808 subdivision_hole_filler-1.0.4/src/subdivision_hole_filler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-06-03 06:55:21.000000 subdivision_hole_filler-1.0.4/src/subdivision_hole_filler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-06-03 06:55:21.000000 subdivision_hole_filler-1.0.4/src/subdivision_hole_filler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 06:55:21.000000 subdivision_hole_filler-1.0.4/src/subdivision_hole_filler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-06-03 06:55:21.000000 subdivision_hole_filler-1.0.4/src/subdivision_hole_filler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-06-03 06:55:21.000000 subdivision_hole_filler-1.0.4/src/subdivision_hole_filler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:55:21.962808 subdivision_hole_filler-1.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-06-03 06:55:17.000000 subdivision_hole_filler-1.0.4/tests/test_6sided_hole.py
```

### Comparing `subdivision_hole_filler-1.0.3/.github/workflows/python-package.yml` & `subdivision_hole_filler-1.0.4/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `subdivision_hole_filler-1.0.3/.github/workflows/python-publish.yml` & `subdivision_hole_filler-1.0.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `subdivision_hole_filler-1.0.3/.gitignore` & `subdivision_hole_filler-1.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `subdivision_hole_filler-1.0.3/LICENSE` & `subdivision_hole_filler-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `subdivision_hole_filler-1.0.3/Levin_2000_Filling N-sided Holes Using Combined Subdivision Schemes.pdf` & `subdivision_hole_filler-1.0.4/Levin_2000_Filling N-sided Holes Using Combined Subdivision Schemes.pdf`

 * *Files identical despite different names*

### Comparing `subdivision_hole_filler-1.0.3/PKG-INFO` & `subdivision_hole_filler-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: subdivision-hole-filler
-Version: 1.0.3
+Version: 1.0.4
 Summary: A python package to fill N-sided holes using combined subdivision schemes, based on Catmull-Clark subdivison.
 Author-email: HUANG Lihao <huang-lihao@outlook.com>
 Project-URL: Homepage, https://github.com/huang-lihao/subdivision-hole-filler
 Project-URL: Bug Tracker, https://github.com/huang-lihao/subdivision-hole-filler/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib
 Requires-Dist: numpy
+Requires-Dist: scipy
 
 # Filler for N-sided holes
 [![GitHub release (with filter)](https://img.shields.io/github/v/release/huang-lihao/subdivision-hole-filler?logo=github)
 ](https://github.com/huang-lihao/subdivision-hole-filler)
 [![Upload Python Package](https://github.com/huang-lihao/subdivision-hole-filler/actions/workflows/python-publish.yml/badge.svg)](https://github.com/huang-lihao/subdivision-hole-filler/actions/workflows/python-publish.yml)
 [![PyPI - Version](https://img.shields.io/pypi/v/subdivision-hole-filler?logo=pypi)](https://pypi.org/project/subdivision-hole-filler/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/subdivision-hole-filler?logo=PyPI)](https://pypi.org/project/subdivision-hole-filler/)
```

### Comparing `subdivision_hole_filler-1.0.3/README.md` & `subdivision_hole_filler-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `subdivision_hole_filler-1.0.3/iso.png` & `subdivision_hole_filler-1.0.4/iso.png`

 * *Files identical despite different names*

### Comparing `subdivision_hole_filler-1.0.3/pyproject.toml` & `subdivision_hole_filler-1.0.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [ # Optional
     "matplotlib",
     "numpy",
+    "scipy",
 ]
 dynamic = ["version"]
 
 [project.urls]
 "Homepage" = "https://github.com/huang-lihao/subdivision-hole-filler"
 "Bug Tracker" = "https://github.com/huang-lihao/subdivision-hole-filler/issues"
```

### Comparing `subdivision_hole_filler-1.0.3/side.png` & `subdivision_hole_filler-1.0.4/side.png`

 * *Files identical despite different names*

### Comparing `subdivision_hole_filler-1.0.3/src/subdivision_hole_filler/hole_filler.py` & `subdivision_hole_filler-1.0.4/src/subdivision_hole_filler/hole_filler.py`

 * *Files identical despite different names*

### Comparing `subdivision_hole_filler-1.0.3/src/subdivision_hole_filler.egg-info/PKG-INFO` & `subdivision_hole_filler-1.0.4/src/subdivision_hole_filler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: subdivision-hole-filler
-Version: 1.0.3
+Version: 1.0.4
 Summary: A python package to fill N-sided holes using combined subdivision schemes, based on Catmull-Clark subdivison.
 Author-email: HUANG Lihao <huang-lihao@outlook.com>
 Project-URL: Homepage, https://github.com/huang-lihao/subdivision-hole-filler
 Project-URL: Bug Tracker, https://github.com/huang-lihao/subdivision-hole-filler/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib
 Requires-Dist: numpy
+Requires-Dist: scipy
 
 # Filler for N-sided holes
 [![GitHub release (with filter)](https://img.shields.io/github/v/release/huang-lihao/subdivision-hole-filler?logo=github)
 ](https://github.com/huang-lihao/subdivision-hole-filler)
 [![Upload Python Package](https://github.com/huang-lihao/subdivision-hole-filler/actions/workflows/python-publish.yml/badge.svg)](https://github.com/huang-lihao/subdivision-hole-filler/actions/workflows/python-publish.yml)
 [![PyPI - Version](https://img.shields.io/pypi/v/subdivision-hole-filler?logo=pypi)](https://pypi.org/project/subdivision-hole-filler/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/subdivision-hole-filler?logo=PyPI)](https://pypi.org/project/subdivision-hole-filler/)
```

### Comparing `subdivision_hole_filler-1.0.3/src/subdivision_hole_filler.egg-info/SOURCES.txt` & `subdivision_hole_filler-1.0.4/src/subdivision_hole_filler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `subdivision_hole_filler-1.0.3/tests/test_6sided_hole.py` & `subdivision_hole_filler-1.0.4/tests/test_6sided_hole.py`

 * *Files identical despite different names*

