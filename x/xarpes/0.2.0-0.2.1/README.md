# Comparing `tmp/xarpes-0.2.0.tar.gz` & `tmp/xarpes-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xarpes-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "xarpes-0.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `xarpes-0.2.0.tar` & `xarpes-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rwxr-xr-x   0        0        0    35149 2024-06-02 15:16:58.370851 xarpes-0.2.0/LICENSE
--rwxr-xr-x   0        0        0     3324 2024-06-02 15:16:29.101945 xarpes-0.2.0/README.md
--rwxr-xr-x   0        0        0      625 2024-06-02 11:12:10.476982 xarpes-0.2.0/pyproject.toml
--rwxr-xr-x   0        0        0      291 2024-05-29 10:56:48.000000 xarpes-0.2.0/xarpes/.ipynb_checkpoints/__init__-checkpoint.py
--rwxr-xr-x   0        0        0     7423 2024-06-02 15:33:12.000000 xarpes-0.2.0/xarpes/.ipynb_checkpoints/band_map-checkpoint.py
--rwxr-xr-x   0        0        0    13410 2024-06-02 15:32:56.000000 xarpes-0.2.0/xarpes/.ipynb_checkpoints/distributions-checkpoint.py
--rwxr-xr-x   0        0        0     4600 2024-06-02 15:33:22.000000 xarpes-0.2.0/xarpes/.ipynb_checkpoints/functions-checkpoint.py
--rwxr-xr-x   0        0        0     5343 2024-06-02 15:33:09.000000 xarpes-0.2.0/xarpes/.ipynb_checkpoints/plotting-checkpoint.py
--rwxr-xr-x   0        0        0      149 2024-06-03 09:02:42.838874 xarpes-0.2.0/xarpes/__init__.py
--rwxr-xr-x   0        0        0     7423 2024-06-02 15:33:12.136538 xarpes-0.2.0/xarpes/band_map.py
--rwxr-xr-x   0        0        0    13410 2024-06-02 15:32:56.826971 xarpes-0.2.0/xarpes/distributions.py
--rwxr-xr-x   0        0        0     4600 2024-06-02 15:33:22.242443 xarpes-0.2.0/xarpes/functions.py
--rwxr-xr-x   0        0        0     5343 2024-06-02 15:33:09.246452 xarpes-0.2.0/xarpes/plotting.py
--rw-r--r--   0        0        0     3865 1970-01-01 00:00:00.000000 xarpes-0.2.0/PKG-INFO
+-rwxr-xr-x   0        0        0    35149 2024-06-02 15:16:58.370851 xarpes-0.2.1/LICENSE
+-rwxr-xr-x   0        0        0     3324 2024-06-02 15:16:29.101945 xarpes-0.2.1/README.md
+-rwxr-xr-x   0        0        0      625 2024-06-02 11:12:10.476982 xarpes-0.2.1/pyproject.toml
+-rwxr-xr-x   0        0        0      291 2024-05-29 10:56:48.000000 xarpes-0.2.1/xarpes/.ipynb_checkpoints/__init__-checkpoint.py
+-rwxr-xr-x   0        0        0     7423 2024-06-02 15:33:12.000000 xarpes-0.2.1/xarpes/.ipynb_checkpoints/band_map-checkpoint.py
+-rwxr-xr-x   0        0        0    13410 2024-06-02 15:32:56.000000 xarpes-0.2.1/xarpes/.ipynb_checkpoints/distributions-checkpoint.py
+-rwxr-xr-x   0        0        0     4600 2024-06-02 15:33:22.000000 xarpes-0.2.1/xarpes/.ipynb_checkpoints/functions-checkpoint.py
+-rwxr-xr-x   0        0        0     5343 2024-06-02 15:33:09.000000 xarpes-0.2.1/xarpes/.ipynb_checkpoints/plotting-checkpoint.py
+-rwxr-xr-x   0        0        0      149 2024-06-03 11:32:10.396629 xarpes-0.2.1/xarpes/__init__.py
+-rwxr-xr-x   0        0        0     7423 2024-06-02 15:33:12.136538 xarpes-0.2.1/xarpes/band_map.py
+-rwxr-xr-x   0        0        0    13410 2024-06-02 15:32:56.826971 xarpes-0.2.1/xarpes/distributions.py
+-rwxr-xr-x   0        0        0     4600 2024-06-02 15:33:22.242443 xarpes-0.2.1/xarpes/functions.py
+-rwxr-xr-x   0        0        0     5343 2024-06-02 15:33:09.246452 xarpes-0.2.1/xarpes/plotting.py
+-rw-r--r--   0        0        0     3865 1970-01-01 00:00:00.000000 xarpes-0.2.1/PKG-INFO
```

### Comparing `xarpes-0.2.0/LICENSE` & `xarpes-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xarpes-0.2.0/README.md` & `xarpes-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `xarpes-0.2.0/pyproject.toml` & `xarpes-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xarpes-0.2.0/xarpes/.ipynb_checkpoints/band_map-checkpoint.py` & `xarpes-0.2.1/xarpes/.ipynb_checkpoints/band_map-checkpoint.py`

 * *Files identical despite different names*

### Comparing `xarpes-0.2.0/xarpes/.ipynb_checkpoints/distributions-checkpoint.py` & `xarpes-0.2.1/xarpes/.ipynb_checkpoints/distributions-checkpoint.py`

 * *Files identical despite different names*

### Comparing `xarpes-0.2.0/xarpes/.ipynb_checkpoints/functions-checkpoint.py` & `xarpes-0.2.1/xarpes/.ipynb_checkpoints/functions-checkpoint.py`

 * *Files identical despite different names*

### Comparing `xarpes-0.2.0/xarpes/.ipynb_checkpoints/plotting-checkpoint.py` & `xarpes-0.2.1/xarpes/.ipynb_checkpoints/plotting-checkpoint.py`

 * *Files identical despite different names*

### Comparing `xarpes-0.2.0/xarpes/band_map.py` & `xarpes-0.2.1/xarpes/band_map.py`

 * *Files identical despite different names*

### Comparing `xarpes-0.2.0/xarpes/distributions.py` & `xarpes-0.2.1/xarpes/distributions.py`

 * *Files identical despite different names*

### Comparing `xarpes-0.2.0/xarpes/functions.py` & `xarpes-0.2.1/xarpes/functions.py`

 * *Files identical despite different names*

### Comparing `xarpes-0.2.0/xarpes/plotting.py` & `xarpes-0.2.1/xarpes/plotting.py`

 * *Files identical despite different names*

### Comparing `xarpes-0.2.0/PKG-INFO` & `xarpes-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xarpes
-Version: 0.2.0
+Version: 0.2.1
 Summary: Extraction from angle resolved photoemission spectra
 Author: xARPES Developers
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: igor2
```

