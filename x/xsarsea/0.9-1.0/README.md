# Comparing `tmp/xsarsea-0.9.tar.gz` & `tmp/xsarsea-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xsarsea-0.9.tar", last modified: Tue Oct 17 14:27:58 2023, max compression
+gzip compressed data, was "xsarsea-1.0.tar", last modified: Mon Jun  3 07:42:44 2024, max compression
```

## Comparing `xsarsea-0.9.tar` & `xsarsea-1.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 14:27:58.585702 xsarsea-0.9/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2023-10-17 14:27:42.000000 xsarsea-0.9/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (127)      553 2023-10-17 14:27:42.000000 xsarsea-0.9/.gitconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 14:27:58.569702 xsarsea-0.9/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-10-17 14:27:42.000000 xsarsea-0.9/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 14:27:58.569702 xsarsea-0.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      936 2023-10-17 14:27:42.000000 xsarsea-0.9/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      829 2023-10-17 14:27:42.000000 xsarsea-0.9/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2023-10-17 14:27:42.000000 xsarsea-0.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      957 2023-10-17 14:27:42.000000 xsarsea-0.9/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2023-10-17 14:27:42.000000 xsarsea-0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      710 2023-10-17 14:27:58.585702 xsarsea-0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2023-10-17 14:27:42.000000 xsarsea-0.9/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 14:27:58.573702 xsarsea-0.9/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2023-10-17 14:27:42.000000 xsarsea-0.9/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 14:27:58.565702 xsarsea-0.9/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 14:27:58.573702 xsarsea-0.9/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2023-10-17 14:27:42.000000 xsarsea-0.9/docs/_static/css/xsarsea.css
--rw-r--r--   0 runner    (1001) docker     (127)      565 2023-10-17 14:27:42.000000 xsarsea-0.9/docs/basic_api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3270 2023-10-17 14:27:42.000000 xsarsea-0.9/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 14:27:58.577702 xsarsea-0.9/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)    10800 2023-10-17 14:27:42.000000 xsarsea-0.9/docs/examples/gmfs_and_luts.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    12273 2023-10-17 14:27:42.000000 xsarsea-0.9/docs/examples/streaks.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    12008 2023-10-17 14:27:42.000000 xsarsea-0.9/docs/examples/windspeed_inversion.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)  3931394 2023-10-17 14:27:42.000000 xsarsea-0.9/docs/examples/windspeed_retrieval_L1.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3466 2023-10-17 14:27:42.000000 xsarsea-0.9/docs/examples/xsarsea.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2023-10-17 14:27:42.000000 xsarsea-0.9/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      960 2023-10-17 14:27:42.000000 xsarsea-0.9/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      381 2023-10-17 14:27:42.000000 xsarsea-0.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-17 14:27:58.585702 xsarsea-0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      994 2023-10-17 14:27:42.000000 xsarsea-0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 14:27:58.565702 xsarsea-0.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 14:27:58.581702 xsarsea-0.9/src/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      551 2023-10-17 14:27:42.000000 xsarsea-0.9/src/scripts/configuration_L1B_xspectra_IW_SLC_IFR_v1.yml
--rw-r--r--   0 runner    (1001) docker     (127)     8684 2023-10-17 14:27:42.000000 xsarsea-0.9/src/scripts/wind_speed_retrieval.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1163 2023-10-17 14:27:42.000000 xsarsea-0.9/src/scripts/xsarsea_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 14:27:58.581702 xsarsea-0.9/src/xsarsea/
--rw-r--r--   0 runner    (1001) docker     (127)      377 2023-10-17 14:27:42.000000 xsarsea-0.9/src/xsarsea/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2023-10-17 14:27:42.000000 xsarsea-0.9/src/xsarsea/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)    26004 2023-10-17 14:27:42.000000 xsarsea-0.9/src/xsarsea/gradients.py
--rw-r--r--   0 runner    (1001) docker     (127)     3455 2023-10-17 14:27:42.000000 xsarsea-0.9/src/xsarsea/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 14:27:58.585702 xsarsea-0.9/src/xsarsea/windspeed/
--rw-r--r--   0 runner    (1001) docker     (127)      466 2023-10-17 14:27:42.000000 xsarsea-0.9/src/xsarsea/windspeed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12311 2023-10-17 14:27:42.000000 xsarsea-0.9/src/xsarsea/windspeed/gmfs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9776 2023-10-17 14:27:42.000000 xsarsea-0.9/src/xsarsea/windspeed/gmfs_impl.py
--rw-r--r--   0 runner    (1001) docker     (127)    13902 2023-10-17 14:27:42.000000 xsarsea-0.9/src/xsarsea/windspeed/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4108 2023-10-17 14:27:42.000000 xsarsea-0.9/src/xsarsea/windspeed/sarwing_luts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3208 2023-10-17 14:27:42.000000 xsarsea-0.9/src/xsarsea/windspeed/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16219 2023-10-17 14:27:42.000000 xsarsea-0.9/src/xsarsea/windspeed/windspeed.py
--rw-r--r--   0 runner    (1001) docker     (127)     3216 2023-10-17 14:27:42.000000 xsarsea-0.9/src/xsarsea/xsarsea.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 14:27:58.581702 xsarsea-0.9/src/xsarsea.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      710 2023-10-17 14:27:58.000000 xsarsea-0.9/src/xsarsea.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2023-10-17 14:27:58.000000 xsarsea-0.9/src/xsarsea.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-17 14:27:58.000000 xsarsea-0.9/src/xsarsea.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2023-10-17 14:27:58.000000 xsarsea-0.9/src/xsarsea.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-10-17 14:27:58.000000 xsarsea-0.9/src/xsarsea.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 14:27:58.585702 xsarsea-0.9/test/
--rw-r--r--   0 runner    (1001) docker     (127)     5008 2023-10-17 14:27:42.000000 xsarsea-0.9/test/test_xsarsea.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:42:44.338263 xsarsea-1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-06-03 07:42:27.000000 xsarsea-1.0/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-06-03 07:42:27.000000 xsarsea-1.0/.gitconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:42:44.334263 xsarsea-1.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-06-03 07:42:27.000000 xsarsea-1.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:42:44.334263 xsarsea-1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-06-03 07:42:27.000000 xsarsea-1.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-06-03 07:42:27.000000 xsarsea-1.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-06-03 07:42:27.000000 xsarsea-1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-06-03 07:42:27.000000 xsarsea-1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-06-03 07:42:27.000000 xsarsea-1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-06-03 07:42:44.338263 xsarsea-1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-06-03 07:42:27.000000 xsarsea-1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:42:44.334263 xsarsea-1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-06-03 07:42:27.000000 xsarsea-1.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:42:44.330263 xsarsea-1.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:42:44.334263 xsarsea-1.0/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-06-03 07:42:27.000000 xsarsea-1.0/docs/_static/css/xsarsea.css
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-06-03 07:42:27.000000 xsarsea-1.0/docs/basic_api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-06-03 07:42:27.000000 xsarsea-1.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:42:44.334263 xsarsea-1.0/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    11102 2024-06-03 07:42:27.000000 xsarsea-1.0/docs/examples/gmfs_and_luts.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    12274 2024-06-03 07:42:27.000000 xsarsea-1.0/docs/examples/streaks.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    15869 2024-06-03 07:42:27.000000 xsarsea-1.0/docs/examples/windspeed_inversion.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    15728 2024-06-03 07:42:27.000000 xsarsea-1.0/docs/examples/windspeed_retrieval_L1.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-06-03 07:42:27.000000 xsarsea-1.0/docs/examples/xsarsea.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-06-03 07:42:27.000000 xsarsea-1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-06-03 07:42:27.000000 xsarsea-1.0/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-06-03 07:42:27.000000 xsarsea-1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 07:42:44.338263 xsarsea-1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-06-03 07:42:27.000000 xsarsea-1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:42:44.330263 xsarsea-1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:42:44.334263 xsarsea-1.0/src/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-06-03 07:42:27.000000 xsarsea-1.0/src/scripts/configuration_L1B_xspectra_IW_SLC_IFR_v1.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1163 2024-06-03 07:42:27.000000 xsarsea-1.0/src/scripts/xsarsea_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:42:44.334263 xsarsea-1.0/src/xsarsea/
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-06-03 07:42:27.000000 xsarsea-1.0/src/xsarsea/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-06-03 07:42:27.000000 xsarsea-1.0/src/xsarsea/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    29364 2024-06-03 07:42:27.000000 xsarsea-1.0/src/xsarsea/gradients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-06-03 07:42:27.000000 xsarsea-1.0/src/xsarsea/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:42:44.338263 xsarsea-1.0/src/xsarsea/windspeed/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-06-03 07:42:27.000000 xsarsea-1.0/src/xsarsea/windspeed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-06-03 07:42:27.000000 xsarsea-1.0/src/xsarsea/windspeed/cmod7.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12311 2024-06-03 07:42:27.000000 xsarsea-1.0/src/xsarsea/windspeed/gmfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9776 2024-06-03 07:42:27.000000 xsarsea-1.0/src/xsarsea/windspeed/gmfs_impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14244 2024-06-03 07:42:27.000000 xsarsea-1.0/src/xsarsea/windspeed/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5304 2024-06-03 07:42:27.000000 xsarsea-1.0/src/xsarsea/windspeed/sarwing_luts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-06-03 07:42:27.000000 xsarsea-1.0/src/xsarsea/windspeed/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16594 2024-06-03 07:42:27.000000 xsarsea-1.0/src/xsarsea/windspeed/windspeed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-06-03 07:42:27.000000 xsarsea-1.0/src/xsarsea/xsarsea.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:42:44.338263 xsarsea-1.0/src/xsarsea.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-06-03 07:42:44.000000 xsarsea-1.0/src/xsarsea.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-06-03 07:42:44.000000 xsarsea-1.0/src/xsarsea.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 07:42:44.000000 xsarsea-1.0/src/xsarsea.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-06-03 07:42:44.000000 xsarsea-1.0/src/xsarsea.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-06-03 07:42:44.000000 xsarsea-1.0/src/xsarsea.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:42:44.338263 xsarsea-1.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     5008 2024-06-03 07:42:27.000000 xsarsea-1.0/test/test_xsarsea.py
```

### Comparing `xsarsea-0.9/.gitconfig` & `xsarsea-1.0/.gitconfig`

 * *Files identical despite different names*

### Comparing `xsarsea-0.9/.github/workflows/main.yml` & `xsarsea-1.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `xsarsea-0.9/.github/workflows/publish.yml` & `xsarsea-1.0/.github/workflows/publish.yml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 jobs:
   publish:
     name: Publish to PyPI
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
       - name: Set up Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: '3.x'
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip build twine
       - name: Build
         run: |
```

### Comparing `xsarsea-0.9/.gitignore` & `xsarsea-1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `xsarsea-0.9/.pre-commit-config.yaml` & `xsarsea-1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `xsarsea-0.9/LICENSE` & `xsarsea-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xsarsea-0.9/PKG-INFO` & `xsarsea-1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xsarsea
-Version: 0.9
+Version: 1.0
 Summary: cmod, detrend, and others sar processing tools over ocean
 Home-page: https://github.com/umr-lops/xsarsea
 Author: Olivier Archer
 Author-email: Olivier.Archer@ifremer.fr
 License: MIT
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `xsarsea-0.9/README.rst` & `xsarsea-1.0/README.rst`

 * *Files identical despite different names*

### Comparing `xsarsea-0.9/docs/Makefile` & `xsarsea-1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `xsarsea-0.9/docs/basic_api.rst` & `xsarsea-1.0/docs/basic_api.rst`

 * *Files identical despite different names*

### Comparing `xsarsea-0.9/docs/conf.py` & `xsarsea-1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `xsarsea-0.9/docs/examples/gmfs_and_luts.ipynb` & `xsarsea-1.0/docs/examples/gmfs_and_luts.ipynb`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9151785714285714%*

 * *Differences: {"'metadata'": "{'language_info': {'codemirror_mode': OrderedDict([('name', 'ipython'), "*

 * *               "('version', 3)]), 'file_extension': '.py', 'mimetype': 'text/x-python', "*

 * *               "'nbconvert_exporter': 'python', 'version': '3.10.12'}, 'kernelspec': "*

 * *               "OrderedDict([('display_name', 'Python 3 (ipykernel)'), ('language', 'python'), "*

 * *               "('name', 'python3')])}"}*

```diff
@@ -350,15 +350,28 @@
             "id": "78f4b231-1815-446e-8f0b-afc589e28988",
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
+        "kernelspec": {
+            "display_name": "Python 3 (ipykernel)",
+            "language": "python",
+            "name": "python3"
+        },
         "language_info": {
+            "codemirror_mode": {
+                "name": "ipython",
+                "version": 3
+            },
+            "file_extension": ".py",
+            "mimetype": "text/x-python",
             "name": "python",
-            "pygments_lexer": "ipython3"
+            "nbconvert_exporter": "python",
+            "pygments_lexer": "ipython3",
+            "version": "3.10.12"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `xsarsea-0.9/docs/examples/streaks.ipynb` & `xsarsea-1.0/docs/examples/streaks.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9977678571428572%*

 * *Differences: {"'metadata'": "{'language_info': {'version': '3.10.12'}}"}*

```diff
@@ -356,13 +356,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.9"
+            "version": "3.10.12"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `xsarsea-0.9/docs/examples/windspeed_inversion.ipynb` & `xsarsea-1.0/docs/examples/windspeed_inversion.ipynb`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8813462885154062%*

 * *Differences: {"'cells'": "{4: {'source': {insert: [(2, 'sarwing_ds')], delete: [3, 2]}}, 12: {'source': "*

 * *            "{insert: [(0, 'wind_co = windspeed.invert_from_model(\\n'), (5, 'windspeed_co = "*

 * *            "np.abs(wind_co)')], delete: [0]}}, 21: {'source': {insert: [(3, 'wind_co, wind_dual = "*

 * *            "windspeed.invert_from_model(\\n'), (10, 'windspeed_co = np.abs(wind_co)\\n'), (11, "*

 * *            "'windspeed_dual =  np.abs(wind_dual)')], delete: [11, 10, 3]}}, 33: {'id': "*

 * *            "'f408e45f-b188-4937-97 […]*

```diff
@@ -53,16 +53,15 @@
             "execution_count": null,
             "id": "77630d90-573a-428a-9029-1c3272289879",
             "metadata": {},
             "outputs": [],
             "source": [
                 "sarwing_owi_file = xsarsea.get_test_file('s1a-iw-owi-xx-20210909t130650-20210909t130715-039605-04AE83.nc')\n",
                 "sarwing_ds = xsarsea.read_sarwing_owi(sarwing_owi_file)\n",
-                "sarwing_ds\n",
-                "\n"
+                "sarwing_ds"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "4ced9944-f9ba-4fa8-aa95-4e14c49fe0f8",
             "metadata": {},
             "source": [
@@ -170,19 +169,20 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "499ad90a-2d90-4a16-a016-cb3d55c7d23d",
             "metadata": {},
             "outputs": [],
             "source": [
-                "windspeed_co = windspeed.invert_from_model(\n",
+                "wind_co = windspeed.invert_from_model(\n",
                 "        sarwing_ds.owiIncidenceAngle,\n",
                 "        sarwing_ds.owiNrcs,\n",
                 "        ancillary_wind = -np.conj(sarwing_ds.owi_ancillary_wind),\n",
-                "        model='cmod5n')\n"
+                "        model='cmod5n')\n",
+                "windspeed_co = np.abs(wind_co)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "089780fa-aeab-4b28-b39c-55f5c221e205",
             "metadata": {},
             "source": [
@@ -288,23 +288,23 @@
             "id": "af0841b0-b5a4-42d8-994d-360cecd32797",
             "metadata": {},
             "outputs": [],
             "source": [
                 "sarwing_luts_subset_path = xsarsea.get_test_file('sarwing_luts_subset')\n",
                 "windspeed.register_all_sarwing_luts(sarwing_luts_subset_path)\n",
                 "\n",
-                "windspeed_co, windspeed_dual = windspeed.invert_from_model(\n",
+                "wind_co, wind_dual = windspeed.invert_from_model(\n",
                 "        sarwing_ds.owiIncidenceAngle,\n",
                 "        sarwing_ds.owiNrcs,\n",
                 "        sarwing_ds.owiNrcs_cross,\n",
                 "        ancillary_wind=-np.conj(sarwing_ds.owi_ancillary_wind),\n",
                 "        dsig_cr = dsig_cr,\n",
                 "        model=('cmod5n','cmodms1ahw'))\n",
-                "windspeed_co = np.abs(windspeed_co)\n",
-                "windspeed_dual =  np.abs(windspeed_dual)"
+                "windspeed_co = np.abs(wind_co)\n",
+                "windspeed_dual =  np.abs(wind_dual)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "29379eaa-c340-4f52-9586-dafecb0cfa19",
             "metadata": {},
             "source": [
@@ -323,24 +323,153 @@
                 "    (hv.Image(windspeed_dual).opts(title='xsarsea') + \n",
                 "     hv.Image(sarwing_ds.owiWindSpeed_Tab_dualpol_2steps).opts(title='sarwing' )).opts(hv.opts.Image(cmap='jet', clim=(0,50))) +  \n",
                 "    hv.Image(windspeed_diff).opts(cmap='jet', clim=(-0.5,0.5), title='xsarsea-sarwing\\nmean=%.4f std=%.4f' % (np.mean(windspeed_diff), np.std(windspeed_diff)))\n",
                 ").opts(hv.opts.Image(colorbar=True, tools=['hover']))"
             ]
         },
         {
+            "cell_type": "markdown",
+            "id": "d79a3983-5c50-4ba4-a4df-61cb6b9ef955",
+            "metadata": {},
+            "source": [
+                "## direction output"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "id": "d21b329b-0218-4b81-8994-0e9317fe11a7",
             "metadata": {},
             "outputs": [],
+            "source": [
+                "sarwing_ds[\"winddir_dual\"] = (90 - (np.angle(-np.conj(wind_dual),deg=True)) + sarwing_ds.owiHeading)%360\n",
+                "sub_sarwing_ds = sarwing_ds.isel(line=slice(None, None, 10), sample=slice(None, None, 10))\n",
+                "\n",
+                "vectorfield = hv.VectorField(\n",
+                "    (\n",
+                "        sub_sarwing_ds.sample, sub_sarwing_ds.line,\n",
+                "        xsarsea.dir_geo_to_sample(sarwing_ds[\"winddir_dual\"] ,sub_sarwing_ds.owiHeading),\n",
+                "        np.abs(wind_dual).isel(line=slice(None, None, 10), sample=slice(None, None, 10))\n",
+                "    )\n",
+                ")\n",
+                "\n",
+                "hv.Image(windspeed_dual, kdims=['sample','line']).opts(title='speed and dir', clim=(0,50), cmap='jet') * vectorfield\n"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "974eaccb-619a-4316-b8d0-3e751d4e964d",
+            "metadata": {},
+            "source": [
+                "###\u00a0sarwing direction output"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "6dc527c2-1f19-447e-9bd3-7e43acaf1a66",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "sub_sarwing_ds = sarwing_ds.isel(line=slice(None, None, 10), sample=slice(None, None, 10))\n",
+                "\n",
+                "vectorfield = hv.VectorField(\n",
+                "    (\n",
+                "        sub_sarwing_ds.sample, sub_sarwing_ds.line,\n",
+                "        xsarsea.dir_geo_to_sample(sub_sarwing_ds.owiWindDirection ,sub_sarwing_ds.owiHeading),\n",
+                "        sub_sarwing_ds.owiWindSpeed\n",
+                "    )\n",
+                ")\n",
+                "\n",
+                "hv.Image(sarwing_ds.owiWindSpeed, kdims=['sample','line']).opts(title='speed and dir', clim=(0,50), cmap='jet') * vectorfield\n"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "e4016131-62f2-4557-a57f-795741f9cad0",
+            "metadata": {},
+            "source": [
+                "## direction difference"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "0a48cad7-f888-4d13-8df7-a9191690d7bb",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "def normalize_angle(diff):\n",
+                "    return (diff + 180) % 360 - 180\n",
+                "    \n",
+                "angle_diff = normalize_angle(sarwing_ds[\"winddir_dual\"] - sarwing_ds.owiWindDirection_Tab_dualpol_2steps)\n",
+                "\n",
+                "(\n",
+                "    (hv.Image(sarwing_ds[\"winddir_dual\"]).opts(title='xsarsea') + \n",
+                "     hv.Image(sarwing_ds.owiWindDirection_Tab_dualpol_2steps).opts(title='sarwing' )).opts(hv.opts.Image(cmap='jet', clim=(0,360))) +  \n",
+                "    hv.Image(normalize_angle(angle_diff)).opts(cmap='jet', clim=(-5,5), title='xsarsea-sarwing\\nmean=%.4f std=%.4f' % (np.mean(angle_diff), np.std(angle_diff)))\n",
+                ").opts(hv.opts.Image(colorbar=True, tools=['hover']))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "aa425555-299c-4ce2-8987-5e27fd8d0af8",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "np.angle(wind_co)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "e4c10815-be94-4470-9fe6-1760c82bacc8",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "wphi_co = 15.0\n",
+                "wspd_co = 30\n",
+                "sol = wspd_co * np.exp(1j * np.deg2rad(wphi_co))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "c321f8c9-fd00-4d1c-a7e4-058ccb81df52",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "np.rad2deg(np.angle(sol))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "f408e45f-b188-4937-9725-8daacb6629b2",
+            "metadata": {},
+            "outputs": [],
             "source": []
         }
     ],
     "metadata": {
+        "kernelspec": {
+            "display_name": "Python 3 (ipykernel)",
+            "language": "python",
+            "name": "python3"
+        },
         "language_info": {
+            "codemirror_mode": {
+                "name": "ipython",
+                "version": 3
+            },
+            "file_extension": ".py",
+            "mimetype": "text/x-python",
             "name": "python",
-            "pygments_lexer": "ipython3"
+            "nbconvert_exporter": "python",
+            "pygments_lexer": "ipython3",
+            "version": "3.10.12"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `xsarsea-0.9/docs/examples/xsarsea.ipynb` & `xsarsea-1.0/docs/examples/xsarsea.ipynb`

 * *Files identical despite different names*

### Comparing `xsarsea-0.9/docs/index.rst` & `xsarsea-1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `xsarsea-0.9/docs/installing.rst` & `xsarsea-1.0/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `xsarsea-0.9/setup.py` & `xsarsea-1.0/setup.py`

 * *Files identical despite different names*

### Comparing `xsarsea-0.9/src/scripts/configuration_L1B_xspectra_IW_SLC_IFR_v1.yml` & `xsarsea-1.0/src/scripts/configuration_L1B_xspectra_IW_SLC_IFR_v1.yml`

 * *Files identical despite different names*

### Comparing `xsarsea-0.9/src/scripts/xsarsea_cli.py` & `xsarsea-1.0/src/scripts/xsarsea_cli.py`

 * *Files identical despite different names*

### Comparing `xsarsea-0.9/src/xsarsea/gradients.py` & `xsarsea-1.0/src/xsarsea/gradients.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,18 +5,19 @@
 
 https://ieeexplore.ieee.org/document/1288365
 
 https://www.climate-service-center.de/imperia/md/content/gkss/institut_fuer_kuestenforschung/ksd/paper/kochw_ieee_2004.pdf
 
 """
 
-__all__ = ['Gradients', 'Gradients2D', 'circ_smooth', 'PlotGradients', 'circ_hist']
+__all__ = ['Gradients', 'Gradients2D',
+           'circ_smooth', 'PlotGradients', 'circ_hist']
 
 import numpy as np
-from scipy import signal
+from scipy import signal, ndimage
 import xarray as xr
 import warnings
 import cv2
 from functools import reduce, partial
 from operator import mul
 from itertools import product
 import pandas as pd
@@ -56,15 +57,16 @@
         window_step: float
 
             stepping of windows sliding. (0.5 is half of the windows, 1 is for non overlapping windows)
 
         windows_at: dict
         """
         if window_step is not None and windows_at is not None:
-            raise ValueError('window_step and window_at are mutually exclusive')
+            raise ValueError(
+                'window_step and window_at are mutually exclusive')
         if window_step is None and windows_at is None:
             window_step = 1
         self.sigma0 = sigma0
 
         self._spatial_dims = ['line', 'sample']
 
         # window size, in asample coordinate
@@ -80,33 +82,38 @@
     @property
     @timing(logger=logger.debug)
     def histogram(self):
         """
         direction histogram as a xarray.Dataset, for all windows from `self.stepping_gradients`.
         This is the main attribute needed by user.
         """
-        angles_bins = np.linspace(-np.pi / 2, np.pi / 2, self.n_angles + 1)  # one extra bin
-        angles_bins = (angles_bins[1:] + angles_bins[:-1]) / 2  # suppress extra bin (middle)
+        angles_bins = np.linspace(-np.pi / 2, np.pi / 2,
+                                  self.n_angles + 1)  # one extra bin
+        # suppress extra bin (middle)
+        angles_bins = (angles_bins[1:] + angles_bins[:-1]) / 2
         with warnings.catch_warnings():
             warnings.simplefilter("ignore", RuntimeWarning)
             stepping_gradients = self.stepping_gradients
             grad_hist, ratio = xr.apply_ufunc(
                 gradient_histogram,
                 stepping_gradients['G2'], stepping_gradients['c'], angles_bins,
-                input_core_dims=[self._window_dims.values(), self._window_dims.values(), ["angles"]],
+                input_core_dims=[self._window_dims.values(
+                ), self._window_dims.values(), ["angles"]],
                 exclude_dims=set(self._window_dims.values()),
                 output_core_dims=[['angles'], []],
                 vectorize=True,
                 output_dtypes=[np.float, np.float]
             )
-            grad_hist = grad_hist.rename('weight').assign_coords(angles=angles_bins)
+            grad_hist = grad_hist.rename(
+                'weight').assign_coords(angles=angles_bins)
             ratio = ratio.rename('used_ratio').fillna(0)
         _histogram = xr.merge((grad_hist, ratio))
         # normalize histogram so values are independents from window size
-        window_pixels = mul(*(stepping_gradients[k].size for k in self._window_dims.values()))
+        window_pixels = mul(
+            *(stepping_gradients[k].size for k in self._window_dims.values()))
         _histogram['weight'] = _histogram['weight'] / window_pixels
         return _histogram
 
     @property
     def window_pixels(self):
         # pixel count per window
         return reduce(mul, self.window.values())
@@ -131,15 +138,16 @@
 
     @property
     def rolling_gradients(self):
         """rolling window over `self.local_gradient` (all, with step 1)"""
         lg = self.local_gradients
         # self.window_size is in asample coordinate, and we want it in pixels of lg
         window_size = np.mean(
-            tuple(self.window_size / np.unique(np.diff(ax))[0] for ax in [lg.line, lg.sample])
+            tuple(self.window_size / np.unique(np.diff(ax))
+                  [0] for ax in [lg.line, lg.sample])
         )
         window = {k: int(window_size) for k in self._spatial_dims}
         return lg.rolling(window, center=True).construct(self._window_dims)
 
     @property
     def windows_at(self):
         """
@@ -153,18 +161,26 @@
             This property can be set by user.
         """
         if self._windows_at is None and self.window_step is not None:
             # windows_at computed from window_step
             # self.window_size is in asample coordinate, and we want it in pixels of self.sigma0
             window_size = int(
                 np.mean(
-                    tuple(self.window_size / np.unique(np.diff(ax))[0] for ax in [self.sigma0.line, self.sigma0.sample])
+                    tuple(self.window_size / np.unique(np.diff(ax))
+                          [0] for ax in [self.sigma0.line, self.sigma0.sample])
                 )
             )
-            ds = self.sigma0.isel(line=slice(0, None, int(window_size)), sample=slice(0, None, int(window_size)))
+
+            step_size = int(window_size * self.window_step)
+
+            ds = self.sigma0.isel(
+                line=slice(0, None, step_size),
+                sample=slice(0, None, step_size)
+            )
+
             self._windows_at = {
                 'line': ds.line,
                 'sample': ds.sample
             }
         return self._windows_at
 
     @windows_at.setter
@@ -270,21 +286,20 @@
             for df in downscales_factors:
                 sigma0_resampled = Gradients._sigma0_resample(sigma0.sel(pol=p), df) \
                     .assign_coords(downscale_factor=df)
                 for ws in windows_sizes:
                     self.gradients_list.append(
                         Gradients2D(
                             sigma0_resampled.assign_coords(window_size=ws),
-                            window_size=ws,
+                            window_size=ws
                         )
                     )
 
         # 1st gradient define windows_at from window_step for all others gradients
         self.gradients_list[0].window_step = window_step
-
         self.stacked_gradients = StackedGradients(self.gradients_list)
 
     @property
     @timing(logger=logger.info)
     def histogram(self):
         """
         xarray.Dataset
@@ -313,16 +328,18 @@
 
         return hist
 
     @staticmethod
     def _sigma0_resample(sigma0, factor):
         if factor == 1:
             return sigma0
-        __sigma0 = sigma0.isel(line=slice(0, None, factor), sample=slice(0, None, factor)).copy(True)
-        __sigma0.values[::] = cv2.resize(sigma0.values, __sigma0.shape[::-1], cv2.INTER_AREA)
+        __sigma0 = sigma0.isel(line=slice(0, None, factor),
+                               sample=slice(0, None, factor)).copy(True)
+        __sigma0.values[::] = cv2.resize(
+            sigma0.values, __sigma0.shape[::-1], cv2.INTER_AREA)
         return __sigma0
 
 
 class PlotGradients:
     """Plotting class"""
 
     def __init__(self, gradients_hist):
@@ -334,21 +351,23 @@
 
             from `Gradients2D.histogram` or mean from `Gradients.histogram`.
 
         """
         self.gradients_hist = gradients_hist
         self._spatial_dims = ['sample', 'line']
         # non spatial dims, probably like  ['pol' 'window_dims' 'downscale_factor']
-        self._non_spatial_dims = list(set(gradients_hist.dims) - set(self._spatial_dims) - set(['angles']))
+        self._non_spatial_dims = list(
+            set(gradients_hist.dims) - set(self._spatial_dims) - set(['angles']))
 
         # list of dicts, where keys are from self._non_spatial_dims, and values are all possible values for key
         # so by looping this list, all gradients for all non-spatial dims can be accessed
         self.combine_all = [
             dict(zip(self._non_spatial_dims, comb)) for comb in list(
-                product(*[self.gradients_hist[k].values for k in self._non_spatial_dims])
+                product(
+                    *[self.gradients_hist[k].values for k in self._non_spatial_dims])
             )
         ]
 
         # styles: only one style allowed per dim
         self.dim_styles = {
             'pol': {'line_dash': ['solid', 'dotted']},
             'downscale_factor': {'line_width': [1, 2, 3, 4]},
@@ -358,35 +377,34 @@
         self.styles_names = []
 
         # add variables named like style, ie self.gradients_hist['line_color']
         # the values are the style values, and the dim name is the dim the style belong to
         for dim, style_dict in self.dim_styles.items():
             for style_name, style_values in style_dict.items():
                 try:
-                    self.gradients_hist[style_name] = (dim, style_values[:self.gradients_hist[dim].size])
+                    self.gradients_hist[style_name] = (
+                        dim, style_values[:self.gradients_hist[dim].size])
                     self.styles_names.append(style_name)
                 except (KeyError, ValueError):
                     # dim is not in self.gradients_hist: ignore
                     pass
 
-
         # get maximum histogram
         hist = self.gradients_hist
         iangle = np.abs(hist['weight']).fillna(0).argmax(dim='angles')
         self.peak = hist.angles.isel(angles=iangle).to_dataset(name='angle')
         self.peak['used_ratio'] = hist['used_ratio']
         self.peak['weight'] = hist['weight'].isel(angles=iangle)
 
         # add styles to self.peak
         for style_name in self.styles_names:
             self.peak[style_name] = self.gradients_hist[style_name]
 
         self._vectorfield = None
 
-
     def _get_style(self, ds):
         # return style for ds, using variables from self.styles_names
         # style is only returned if dim len is 1
         return {st: ds[st].values.item() for st in self.styles_names if (st in ds) and (ds[st].size == 1)}
 
     def vectorfield(self, tap=True):
         """Show gradients as a `hv.VectorField` object"""
@@ -405,28 +423,31 @@
 
             # manual legend, to have a style per dimension
             legends = []
             dummy_line = [(0, 0), (0.01, 0)]
             for st in self.styles_names:
                 label = self.peak[st].dims[0]
                 for item in self.peak[st]:
-                    style = {'line_dash': 'solid', 'line_width': 1, 'line_color': 'k'}
+                    style = {'line_dash': 'solid',
+                             'line_width': 1, 'line_color': 'k'}
                     style.update({st: item.item()})
                     legends.append(
                         hv.Curve(
                             dummy_line,
                             label="%s %s" % (label, item[label].item())
                         ).redim.label(x='sample', y='line').opts(**style)
                     )
-            self._vectorfield = hv.Overlay(vf_list + legends).opts(active_tools=['wheel_zoom', 'pan'])
+            self._vectorfield = hv.Overlay(
+                vf_list + legends).opts(active_tools=['wheel_zoom', 'pan'])
 
         if tap:
             line = self.peak.line.values[self.peak.line.size // 2]
             sample = self.peak.sample.values[self.peak.sample.size // 2]
-            self._mouse_stream = hv.streams.Tap(x=sample, y=line, source=self._vectorfield)
+            self._mouse_stream = hv.streams.Tap(
+                x=sample, y=line, source=self._vectorfield)
             return self._vectorfield * hv.DynamicMap(self._get_windows, streams=[self._mouse_stream])
 
         return self._vectorfield
 
     def mouse_histogram(self, source=None):
         assert self._mouse_stream is not None
         if source is None:
@@ -435,15 +456,16 @@
 
     def _get_xline(self, sample=None, line=None, data=None):
         # called by histogram_plot to normalize coords
         if data is not None:
             # called by hv streams (like a mouse tap)
             sample = data[0]
             line = data[1]
-        nearest_center = self.peak.sel(line=line, sample=sample, method='nearest', tolerance=1e6)
+        nearest_center = self.peak.sel(
+            line=line, sample=sample, method='nearest', tolerance=1e6)
         line = nearest_center.line.values.item()
         sample = nearest_center.sample.values.item()
         return sample, line
 
     def _get_windows(self, sample=None, line=None, x=None, y=None):
 
         if x is not None:
@@ -452,54 +474,57 @@
             line = y
 
         # line and sample are from mouse or user. get the nearest where histogram is defined
         sample, line = self._get_xline(sample=sample, line=line)
 
         windows_list = []
         try:
-            ws_list = self.gradients_hist['window_size' ]
+            ws_list = self.gradients_hist['window_size']
         except KeyError:
             # no 'window_size'. compute it from asample neighbors
             ws_list = [
                 np.diff(
                     np.array(
-                        [[self.gradients_hist[ax].isel({ax: i}).item() for i in [0, 1]] for ax in ['line', 'sample']]
+                        [[self.gradients_hist[ax].isel({ax: i}).item() for i in [0, 1]] for ax in [
+                            'line', 'sample']]
                     )
                 ).mean()
             ]
 
         for ws in ws_list:
             # window as a hv.Path object corresponding to window_size
             amin, amax, xmin, xmax = (
                 line - ws / 2, line + ws / 2, sample - ws / 2, sample + ws / 2
             )
             try:
-                style = self._get_style(self.gradients_hist.sel(window_size=ws))
+                style = self._get_style(
+                    self.gradients_hist.sel(window_size=ws))
             except (IndexError, KeyError):
                 style = {}
             windows_list.append(
-                hv.Path([[(xmin, amin), (xmin, amax), (xmax, amax), (xmax, amin), (xmin, amin)]]).opts(**style)
+                hv.Path([[(xmin, amin), (xmin, amax), (xmax, amax),
+                        (xmax, amin), (xmin, amin)]]).opts(**style)
             )
 
         return hv.Overlay(windows_list)
 
-
     def histogram_plot(self, sample=None, line=None, x=None, y=None):
         """plot histogram at sample, line"""
 
         if x is not None:
             sample = x
         if y is not None:
             line = y
 
         # line and sample are from mouse or user. get the nearest where histogram is defined
         sample, line = self._get_xline(sample=sample, line=line)
 
         # get histogram
-        hist_at = self.gradients_hist.sel(line=line, sample=sample, method='nearest', tolerance=500)
+        hist_at = self.gradients_hist.sel(
+            line=line, sample=sample, method='nearest', tolerance=500)
 
         hp_list = []
         for sel_one2D in self.combine_all:
             hist2D_at = hist_at.sel(sel_one2D)
             hist2D360 = circ_hist(hist2D_at['weight'])
             style = self._get_style(hist2D_at)
             hp_list.append(
@@ -548,20 +573,21 @@
 
     # 2 factor resize
     grad2 = R2(grad12)
     grad2.name = 'G2'
 
     # grad quality
     grad3 = R2(abs(grad12))
+    grad3.name = 'G3'
     c = abs(grad2) / (grad3 + 0.00001)
     c = c.where(c <= 1).fillna(0)
     c.name = 'c'
 
     # return np.sqrt(grad2) ( so angles are in range [-pi/2, pi/2]
-    return xr.merge([np.sqrt(grad2), c])
+    return xr.merge([np.sqrt(grad2), grad3, c])
 
 
 def convolve2d(in1, in2, boundary='symm', fillvalue=0, dask=True):
     """
     wrapper around scipy.signal.convolve2d for in1 as xarray.DataArray
     mode is forced to 'same', so axes are not changed.
     """
@@ -587,21 +613,36 @@
 
         # make sure the smallest in1 chunk size is >= in2.shape.
         min_in1_chunk = tuple([min(c) for c in in1.chunks])
         if np.min(np.array(min_in1_chunk) - np.array(in2.shape)) < 0:
             raise IndexError("""Some chunks are too small (%s).
             all chunks must be >= %s.
             """ % (str(in1.chunks), str(in2.shape)))
-        res.data = in1.data.map_overlap(_conv2d, depth=in2.shape, boundary=boundary_map[boundary])
+        res.data = in1.data.map_overlap(
+            _conv2d, depth=in2.shape, boundary=boundary_map[boundary])
     else:
-        res.data = signal.convolve2d(in1.data, in2, mode='same', boundary=boundary)
+        res.data = signal.convolve2d(
+            in1.data, in2, mode='same', boundary=boundary)
 
     return res
 
 
+def smoothing(image):
+    # filtre gaussien
+
+    B2 = np.mat('[1,2,1; 2,4,2; 1,2,1]', float) * 1 / 16
+    B2 = np.array(B2)
+
+    _image = convolve2d(image, B2, boundary='symm')
+    num = convolve2d(xr.ones_like(_image), B2, boundary='symm')
+    image = _image / num
+
+    return image
+
+
 def R2(image):
     """
     reduce image by factor 2, with no moire effect
 
     Parameters
     ----------
     image: xarray.DataArray with dims ['line', 'sample']
@@ -628,14 +669,113 @@
     _image = convolve2d(image, B2, boundary='symm')
     num = convolve2d(xr.ones_like(_image), B2, boundary='symm')
     image = _image / num
 
     return image
 
 
+def Mean(image):
+    """
+    Local Mean Operator
+
+    Parameters
+    ----------
+    image: xarray.DataArray with dims ['line', 'sample']
+
+    Returns
+    -------
+    xarray.DataArray
+        smoothed
+    """
+    B2 = np.mat('[1,2,1; 2,4,2; 1,2,1]', float) * 1 / 16
+    B2 = np.array(B2)
+    B4 = signal.convolve(B2, B2)
+
+    B22 = np.mat(
+        '[1,0,2,0,1;0,0,0,0,0;2,0,4,0,2;0,0,0,0,0;1,0,2,0,1]', float) * 1/16
+    B42 = signal.convolve(B22, B22)
+
+    _image = convolve2d(image, B4, boundary='symm')
+    num = convolve2d(np.ones_like(_image), B4, boundary='symm')
+    image = _image/num
+
+    _image = convolve2d(image, B42, boundary='symm')
+    num = convolve2d(np.ones_like(_image), B4, boundary='symm')
+    image = _image/num
+
+    return image
+
+
+def filtering_parameters(image_ori):
+    """
+    Mask filter parameters definition
+    Zhao, Y.; Longépé, N.; Mouche, A.; Husson, R. Automated Rain Detection by Dual-Polarization Sentinel-1 Data.
+    Remote Sens. 2021, 13, 3155. https://doi.org/10.3390/rs13163155
+
+    Parameters
+    ----------
+    image_ori: xarray.DataArray with dims ['line', 'sample']
+
+    Returns
+    -------
+    list of xarray.DataArray
+        f1, f2, f3, f4, F (all between 0 and 1)
+    """
+    image = np.sqrt(image_ori)  # sqrt de NRCS=amplitude
+
+    # useful parameters
+    r2 = R2(image)
+    lg = local_gradients(image)
+    G3 = lg.G3
+    c = lg.c
+    J = Mean(r2)
+
+    # P1
+    J1 = Mean(r2**2)
+    J2 = np.sqrt(J1 - J**2)
+    # standart deviation / mean
+    P1 = J2/(J+0.00001)
+    a1 = -50
+    b1 = 2.75
+
+    # P2
+    resampl = r2.coarsen({'line': 2, 'sample': 2}, boundary='trim').mean()
+    # we compute the exact factor so that the two terms match dimensions in case of odd original dimensions
+    K = r2 - ndimage.zoom(smoothing(resampl),
+                          (r2.shape[0] / resampl.shape[0], r2.shape[1] / resampl.shape[1]), order=1)
+    P2 = K**2 / ((J**2)+0.00001)
+    a2 = -5000
+    b2 = 3
+
+    # P3
+    G4 = Mean(G3)
+    P3 = G3/(G4+0.00001)
+    a3 = -2.5
+    b3 = 4
+
+    # P4
+    P4 = np.sqrt(c)
+    a4 = -10
+    b4 = 6.3
+
+    # set values between 0 & 1
+    f1 = np.clip(a1*P1+b1, 0, 1)
+    f2 = np.clip(a2*P2+b2, 0, 1)
+    f3 = np.clip(a3*P3+b3, 0, 1)
+    f4 = np.clip(a4*P4+b4, 0, 1)
+
+    F = np.sqrt(1/4. * (f1**2 + f2**2 + f3**2 + f4**2))
+
+    #  TO CHECK
+    if F.shape == image_ori.shape:
+        F[F < 0.0015] = 0  # suppress black band # to check
+
+    return f1, f2, f3, f4, F
+
+
 def gradient_histogram(g2, c, angles_bins):
     """
         internal function that compute histogram from local_gradients for only on small box.
 
         Parameters
         ----------
         g2: numpy.ndarray
@@ -700,15 +840,16 @@
     xarray.DataArray
       same as hist, but smoothed.
 
     """
     Bx = np.array([1, 2, 1], float) * 1 / 4
     Bx2 = np.array([1, 0, 2, 0, 1], float) * 1 / 4
     Bx4 = np.array([1, 0, 0, 0, 2, 0, 0, 0, 1], float) * 1 / 4
-    Bx8 = np.array([1, 0, 0, 0, 0, 0, 0, 0, 2, 0, 0, 0, 0, 0, 0, 0, 1], float) * 1 / 4
+    Bx8 = np.array([1, 0, 0, 0, 0, 0, 0, 0, 2, 0, 0,
+                   0, 0, 0, 0, 0, 1], float) * 1 / 4
     Bs = [Bx, Bx2, Bx4, Bx8]
 
     # circular wrap
     maxsize_B = max([len(B) for B in Bs])
     smooth_hist = hist.pad({'angles': maxsize_B}, mode='wrap')
 
     for B in Bs:
@@ -741,19 +882,21 @@
     """
 
     # convert histogram to circular histogram
     # convert to complex
     hist_at = hist_at * np.exp(1j * hist_at.angles)
 
     # central symmetry, to get 360°
-    hist_at = xr.concat([hist_at, -hist_at], 'angles').drop_vars(['line', 'sample'])
+    hist_at = xr.concat([hist_at, -hist_at],
+                        'angles').drop_vars(['line', 'sample'])
     hist_at['angles'] = np.angle(hist_at)
     hist_at['sample_g'] = np.real(hist_at)
     hist_at['line_g'] = np.imag(hist_at)
 
     # convert to dataframe (weight no longer needed)
     circ_hist_pts = hist_at.to_dataframe('tmp')[['line_g', 'sample_g']]
 
     # close path
-    circ_hist_pts = pd.concat([circ_hist_pts, pd.DataFrame(circ_hist_pts.iloc[0]).T])
+    circ_hist_pts = pd.concat(
+        [circ_hist_pts, pd.DataFrame(circ_hist_pts.iloc[0]).T])
 
     return circ_hist_pts
```

### Comparing `xsarsea-0.9/src/xsarsea/utils.py` & `xsarsea-1.0/src/xsarsea/utils.py`

 * *Files identical despite different names*

### Comparing `xsarsea-0.9/src/xsarsea/windspeed/gmfs.py` & `xsarsea-1.0/src/xsarsea/windspeed/gmfs.py`

 * *Files identical despite different names*

### Comparing `xsarsea-0.9/src/xsarsea/windspeed/gmfs_impl.py` & `xsarsea-1.0/src/xsarsea/windspeed/gmfs_impl.py`

 * *Files identical despite different names*

### Comparing `xsarsea-0.9/src/xsarsea/windspeed/models.py` & `xsarsea-1.0/src/xsarsea/windspeed/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 import netCDF4
 import logging
 import pandas as pd
 
 logger = logging.getLogger('xsarsea.windspeed')
 
 
-
-
 class Model:
     """
     Model class is an abstact class, for handling GMF or LUT.
     It should not be instanciated by the user.
 
     All registered models can be retreived with :func:`~xsarsea.windspeed.available_models`
     """
@@ -66,58 +64,62 @@
         try:
             units = lut.attrs['units']
         except KeyError:
             raise KeyError("lut has no lut.attrs['units']")
 
         allowed_units = ['linear', 'dB']
         if units not in allowed_units:
-            raise ValueError("Unknown lut units '%s'. Allowed are '%s'" % (units, allowed_units))
+            raise ValueError(
+                "Unknown lut units '%s'. Allowed are '%s'" % (units, allowed_units))
 
         if lut.ndim == 2:
             good_dims = ('incidence', 'wspd')
             if not (lut.dims == good_dims):
-                raise IndexError("Bad dims '%s'. Should be '%s'" % (lut.dims, good_dims))
+                raise IndexError("Bad dims '%s'. Should be '%s'" %
+                                 (lut.dims, good_dims))
         elif lut.ndim == 3:
             good_dims = ('incidence', 'wspd', 'phi')
             if not (lut.dims == good_dims):
-                raise IndexError("Bad dims '%s'. Should be '%s'" % (lut.dims, good_dims))
+                raise IndexError("Bad dims '%s'. Should be '%s'" %
+                                 (lut.dims, good_dims))
         else:
             raise IndexError("Bad dims '%s'" % lut.dims)
 
         assert 'resolution' in lut.attrs
 
         # we check if the lut needs interpolation
         resolution = kwargs.pop('resolution', 'high')
         if resolution is None:
             # high res by default
             resolution = 'high'
 
         lut_resolution = lut.attrs['resolution']
-
         if resolution is not None and resolution != lut_resolution:
             if resolution == 'high':
                 # high resolution steps
                 inc_step = kwargs.pop('inc_step', self.inc_step)
                 wspd_step = kwargs.pop('wspd_step', self.wspd_step)
                 phi_step = kwargs.pop('phi_step', self.phi_step)
             elif resolution == 'low':
                 # low resolution steps
                 inc_step = kwargs.pop('inc_step_lr', self.inc_step_lr)
                 wspd_step = kwargs.pop('wspd_step_lr', self.wspd_step_lr)
                 phi_step = kwargs.pop('phi_step_lr', self.phi_step_lr)
 
             inc, wspd, phi = [
-                r and np.linspace(r[0], r[1], num=int(np.round((r[1] - r[0]) / step) + 1))
+                r and np.linspace(r[0], r[1], num=int(
+                    np.round((r[1] - r[0]) / step) + 1))
                 for r, step in zip(
                     [self.inc_range, self.wspd_range, self.phi_range],
                     [inc_step, wspd_step, phi_step]
                 )
             ]
             logger.debug('interp lut %s to high res' % self.name)
-            interp_kwargs = {k: v for k, v in zip(['incidence', 'wspd', 'phi'], [inc, wspd, phi]) if v is not None}
+            interp_kwargs = {k: v for k, v in zip(['incidence', 'wspd', 'phi'], [
+                                                  inc, wspd, phi]) if v is not None}
             lut = lut.interp(**interp_kwargs, kwargs=dict(bounds_error=True))
             lut.attrs['resolution'] = resolution
 
         return lut
 
     @property
     def iscopol(self):
@@ -153,24 +155,26 @@
         if units is None:
             return final_lut
 
         if units == 'dB':
             if lut.attrs['units'] == 'dB':
                 final_lut = lut
             elif lut.attrs['units'] == 'linear':
-                final_lut = 10 * np.log10(lut + 1e-15)  # clip with epsilon to avoid nans
+                # clip with epsilon to avoid nans
+                final_lut = 10 * np.log10(lut + 1e-15)
                 final_lut.attrs['units'] = 'dB'
         elif units == 'linear':
             if lut.attrs['units'] == 'linear':
                 final_lut = lut
             elif lut.attrs['units'] == 'dB':
                 final_lut = 10. ** (lut / 10.)
                 final_lut.attrs['units'] = 'linear'
         else:
-            raise ValueError("Unit not known: %s. Known are 'dB' or 'linear' " % units)
+            raise ValueError(
+                "Unit not known: %s. Known are 'dB' or 'linear' " % units)
 
         final_lut.attrs['model'] = self.name
         final_lut.attrs['pol'] = self.pol
         final_lut.name = 'sigma0_model'
 
         return final_lut
 
@@ -194,22 +198,24 @@
         ds_lut.attrs['inc_range'] = self.inc_range
         ds_lut.attrs['wspd_range'] = self.wspd_range
         ds_lut.attrs['resolution'] = resolution
         ds_lut.attrs['model'] = self.short_name
         if 'phi' in lut.dims:
             ds_lut.attrs['phi_range'] = self.phi_range
 
-        ds_lut.attrs['wspd_step'] = np.round(np.unique(np.diff(lut.wspd)), decimals=2)[0]
-        ds_lut.attrs['inc_step'] = np.round(np.unique(np.diff(lut.incidence)), decimals=2)[0]
+        ds_lut.attrs['wspd_step'] = np.round(
+            np.unique(np.diff(lut.wspd)), decimals=2)[0]
+        ds_lut.attrs['inc_step'] = np.round(
+            np.unique(np.diff(lut.incidence)), decimals=2)[0]
         if 'phi' in lut.dims:
-            ds_lut.attrs['phi_step'] = np.round(np.unique(np.diff(lut.phi)), decimals=2)[0]
+            ds_lut.attrs['phi_step'] = np.round(
+                np.unique(np.diff(lut.phi)), decimals=2)[0]
 
         ds_lut.to_netcdf(file)
 
-
     @abstractmethod
     def __call__(self, inc, wspd, phi=None, broadcast=False):
         """
 
         Parameters
         ----------
         inc: array-like
@@ -258,24 +264,27 @@
     """
 
     _name_prefix = 'nc_lut_'
     _priority = None
 
     def __call__(self, inc, wspd, phi=None, units=None, **kwargs):
 
-        all_scalar = all(np.isscalar(v) for v in [inc, wspd, phi] if v is not None)
+        all_scalar = all(np.isscalar(v)
+                         for v in [inc, wspd, phi] if v is not None)
 
         all_1d = False
         try:
-            all_1d = all(v.ndim == 1 for v in [inc, wspd, phi] if v is not None)
+            all_1d = all(v.ndim == 1 for v in [
+                         inc, wspd, phi] if v is not None)
         except AttributeError:
             all_1d = False
 
         if not (all_scalar or all_1d):
-            raise NotImplementedError('Only scalar or 1D array are implemented for LutModel')
+            raise NotImplementedError(
+                'Only scalar or 1D array are implemented for LutModel')
 
         lut = self.to_lut(units=units, **kwargs)
         if 'phi' in lut.dims:
             sigma0 = lut.interp(incidence=inc, wspd=wspd, phi=phi)
         else:
             sigma0 = lut.interp(incidence=inc, wspd=wspd)
 
@@ -305,20 +314,21 @@
 
     def __init__(self, path, **kwargs):
         name = os.path.splitext(os.path.basename(path))[0]
         # we do not want to read full dataset at this step, we just want global attributes
         with netCDF4.Dataset(path) as ncfile:
             for attr in ['units', 'pol', 'model', 'resolution', 'inc_range', 'wspd_range', 'phi_range', 'inc_step', 'wspd_step', 'phi_step']:
                 try:
-                    kwargs[attr]=ncfile.getncattr(attr)
+                    kwargs[attr] = ncfile.getncattr(attr)
                     if isinstance(kwargs[attr], np.ndarray):
                         kwargs[attr] = list(kwargs[attr])
                 except AttributeError as e:
                     if 'phi' not in attr:
-                        raise AttributeError('Attr %s not found in %s' % (attr, path))
+                        raise AttributeError(
+                            'Attr %s not found in %s' % (attr, path))
         self._short_name = kwargs.pop('model')
         if kwargs['resolution'] == 'low':
             kwargs['inc_step_lr'] = kwargs.pop('inc_step')
             kwargs['wspd_step_lr'] = kwargs.pop('wspd_step')
             kwargs['phi_step_lr'] = kwargs.pop('phi_step', None)
 
         super().__init__(name, **kwargs)
@@ -330,17 +340,17 @@
         ds_lut = xr.open_dataset(self.path)
 
         lut = ds_lut.sigma0_model
         lut.attrs['units'] = ds_lut.attrs['units']
         lut.attrs['model'] = ds_lut.attrs['model']
         lut.attrs['resolution'] = ds_lut.attrs['resolution']
 
-
         return lut
 
+
 def register_all_nc_luts(topdir):
     """
     Register all netcdf luts found under `topdir`.
 
     This function return nothing. See `xsarsea.windspeed.available_models` to see registered models.
 
     Parameters
@@ -386,39 +396,40 @@
 
     Returns
     -------
     pandas.DataFrame
 
     """
 
-    avail_models = pd.DataFrame(columns=['short_name', 'priority', 'pol', 'model'], index=[])
+    avail_models = pd.DataFrame(
+        columns=['short_name', 'priority', 'pol', 'model'], index=[])
 
     for name, model in Model._available_models.items():
         # print('%s: %s' % (name, model))
         avail_models.loc[name, 'model'] = model
         avail_models.loc[name, 'pol'] = model.pol
         avail_models.loc[name, 'priority'] = model._priority
         avail_models.loc[name, 'short_name'] = model.short_name
 
     aliased = avail_models.sort_values('priority', ascending=False).drop_duplicates('short_name').rename(
         columns=dict(short_name='alias')).drop(columns='priority')
 
-    non_aliased = avail_models.drop(aliased.index).drop(columns='priority').rename(columns=dict(short_name='alias'))
+    non_aliased = avail_models.drop(aliased.index).drop(
+        columns='priority').rename(columns=dict(short_name='alias'))
     non_aliased['alias'] = None
     # aliased.merge(non_aliased)
     # aliased
     avail_models = pd.concat([aliased, non_aliased])
 
     # filter
     if pol is not None:
         avail_models = avail_models[avail_models.pol == pol]
 
     return avail_models
 
-
     if pol is None:
         return Model._available_models
     else:
         models_found = {}
         for name, model in Model._available_models.items():
             if pol == model.pol:
                 models_found[name] = model
```

### Comparing `xsarsea-0.9/src/xsarsea/windspeed/sarwing_luts.py` & `xsarsea-1.0/src/xsarsea/windspeed/sarwing_luts.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,38 +19,42 @@
         if not os.path.isdir(self.path):
             raise FileNotFoundError(self.path)
 
         logger.info('load sarwing lut from %s' % self.path)
 
         sigma0_db_path = os.path.join(self.path, 'sigma.npy')
         sigma0_db = np.ascontiguousarray(np.transpose(np.load(sigma0_db_path)))
-        inc = pkl.load(open(os.path.join(self.path, 'incidence_angle.pkl'), 'rb'), encoding='iso-8859-1')
+        inc = pkl.load(open(os.path.join(
+            self.path, 'incidence_angle.pkl'), 'rb'), encoding='iso-8859-1')
         try:
             phi, wspd = pkl.load(open(os.path.join(self.path, 'wind_speed_and_direction.pkl'), 'rb'),
                                  encoding='iso-8859-1')
         except FileNotFoundError:
             phi = None
-            wspd = pkl.load(open(os.path.join(self.path, 'wind_speed.pkl'), 'rb'), encoding='iso-8859-1')
+            wspd = pkl.load(
+                open(os.path.join(self.path, 'wind_speed.pkl'), 'rb'), encoding='iso-8859-1')
 
         self.wspd_step = np.round(np.unique(np.diff(wspd)), decimals=2)[0]
         self.inc_step = np.round(np.unique(np.diff(inc)), decimals=2)[0]
-        self.inc_range = [ np.round(np.min(inc), decimals=2), np.round(np.max(inc), decimals=2) ]
-        self.wspd_range = [np.round(np.min(wspd), decimals=2), np.round(np.max(wspd), decimals=2)]
-
+        self.inc_range = [np.round(np.min(inc), decimals=2), np.round(
+            np.max(inc), decimals=2)]
+        self.wspd_range = [np.round(np.min(wspd), decimals=2), np.round(
+            np.max(wspd), decimals=2)]
 
         if phi is not None:
             dims = ['wspd', 'phi', 'incidence']
             final_dims = ['incidence', 'wspd', 'phi']
             coords = {'incidence': inc, 'phi': phi, 'wspd': wspd}
             self.phi_step = np.round(np.unique(np.diff(phi)), decimals=2)[0]
             # low res parameters, for downsampling
             self.inc_step_lr = 1.
             self.wspd_step_lr = 0.4
             self.phi_step_lr = 2.5
-            self.phi_range = [np.round(np.min(phi), decimals=2), np.round(np.max(phi), decimals=2)]
+            self.phi_range = [np.round(np.min(phi), decimals=2), np.round(
+                np.max(phi), decimals=2)]
         else:
             dims = ['wspd', 'incidence']
             final_dims = ['incidence', 'wspd']
             coords = {'incidence': inc, 'wspd': wspd}
             # low res parameters, for downsampling. those a close to high res, as crosspol lut has quite small
             self.inc_step_lr = 1.
             self.wspd_step_lr = 0.1
@@ -111,7 +115,48 @@
         elif os.path.exists(os.path.join(path, 'wind_speed.pkl')):
             pol = 'VH'
         else:
             pol = None
 
         sarwing_model = SarwingLutModel(name, path, pol=pol)
 
+
+def register_one_sarwing_lut(path):
+    """
+    Register a single sarwing lut.
+
+    This function return nothing. See `xsarsea.windspeed.available_models` to see registered models.
+
+    Parameters
+    ----------
+    path: str
+        path to sarwing lut.
+
+    Examples
+    --------
+    register a single sarwing lut
+
+    >>> xsarsea.windspeed.register_one_sarwing_lut(xsarsea.get_test_file('sarwing_luts_subset/GMF_cmodms1ahw'))
+
+    Notes
+    _____
+    Sarwing lut can be downloaded from https://cyclobs.ifremer.fr/static/sarwing_datarmor/xsardata/sarwing_luts
+
+    See Also
+    --------
+    xsarsea.windspeed.available_models
+    xsarsea.windspeed.gmfs.GmfModel.register
+
+    """
+    sarwing_name = os.path.basename(path)
+    name = sarwing_name.replace('GMF_', SarwingLutModel._name_prefix)
+
+    # guess available pols from filenames
+    if os.path.exists(os.path.join(path, 'wind_speed_and_direction.pkl')):
+        pol = 'VV'
+    elif os.path.exists(os.path.join(path, 'wind_speed.pkl')):
+        pol = 'VH'
+    else:
+        pol = None
+
+    sarwing_model = SarwingLutModel(name, path, pol=pol)
+    return sarwing_model
```

### Comparing `xsarsea-0.9/src/xsarsea/windspeed/utils.py` & `xsarsea-1.0/src/xsarsea/windspeed/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import numpy as np
 
 import logging
 logger = logging.getLogger('xsarsea.windspeed')
 logger.addHandler(logging.NullHandler())
 
 
-def get_dsig(name,inc,sigma0_cr,nesz_cr):
+def get_dsig(name, inc, sigma0_cr, nesz_cr):
     """
     get dsig_cr value(s) by name
 
     Parameters
     ----------
     name: str
         dsig_cr name
@@ -22,29 +22,36 @@
     nesz_cr: xarray.DataArray
         nesz in cross pol
 
     Returns
     -------
     float | xarray.DataArray
     """
-    if name == "gmf_s1_v2":                     
-        b=1
-        def sigmoid(x,c0,c1,d0,d1):
+    if name == "gmf_s1_v2":
+        b = 1
+
+        def sigmoid(x, c0, c1, d0, d1):
             sig = d0 + d1 / (1 + np.exp(-c0*(x-c1)))
             return sig
-        poptsig = np.array([ 1.57952257, 25.61843791,  1.46852088,  1.4058646 ])
-        c=sigmoid(inc,*poptsig)
+        poptsig = np.array([1.57952257, 25.61843791,  1.46852088,  1.4058646])
+        c = sigmoid(inc, *poptsig)
         return (1 / np.sqrt(b*(sigma0_cr / nesz_cr)**c))
 
     elif name == "gmf_rs2_v2":
         b = 1
         c = 8
         return (1 / np.sqrt(b*(sigma0_cr / nesz_cr)**c))
-    else : 
-        raise ValueError("dsig names different than 'gmf_s1_v2' or 'gmf_rs2_v2' are not handled. You can compute your own dsig_cr.")
+
+    elif name == "sarwing_lut_cmodms1ahw":
+        return 1.25 / (sigma0_cr / nesz_cr) ** 4.
+
+    else:
+        raise ValueError(
+            "dsig names different than 'gmf_s1_v2' or 'gmf_rs2_v2' or 'gmf_cmodms1ahw' are not handled. You can compute your own dsig_cr.")
+
 
 def nesz_flattening(noise, inc):
     """
     Noise flatten by polynomial fit (order 1)
 
     Parameters
     ----------
@@ -71,15 +78,16 @@
 
     """
 
     if noise.ndim != 2:
         raise IndexError('Only 2D noise allowed')
 
     with warnings.catch_warnings():
-        warnings.filterwarnings('ignore', message='.*empty.*', category=RuntimeWarning)
+        warnings.filterwarnings(
+            'ignore', message='.*empty.*', category=RuntimeWarning)
         noise_mean = np.nanmean(noise, axis=0)
 
     try:
         # unlike np.mean, np.nanmean return a numpy array, even if noise is an xarray
         # if this behaviour change in the future, we want to be sure to have a numpy array
         noise_mean = noise_mean.values
     except AttributeError:
```

### Comparing `xsarsea-0.9/src/xsarsea/windspeed/windspeed.py` & `xsarsea-1.0/src/xsarsea/windspeed/windspeed.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,19 @@
     See Also
     --------
     xsarsea.windspeed.available_models
     """
     # default array values if no dualpol
     nan = sigma0 * np.nan
 
+    #  put nan values where sigma0 is nan or 0
+    #  sigma0 = np.where(sigma0 == 0, np.nan, sigma0)
+    #  if sigma0_dual is not None:
+    #    sigma0_dual = np.where(sigma0_dual == 0, np.nan, sigma0_dual)
+
     if not isinstance(model, tuple):
         models = (model, None)
     else:
         models = model
 
     models = tuple(get_model(m) if m is not None else None for m in models)
 
@@ -200,38 +205,44 @@
                                one_sigma0_co_db) / dsig_co) ** 2
                     J_co = Jwind_co + Jsig_co
                     # cost function
                     iJ_co = np.argmin(J_co)
                     lut_idx = (iJ_co // J_co.shape[-1], iJ_co % J_co.shape[-1])
                     wspd_co = np_wspd_lut[lut_idx]
                     wphi_co = np_phi_lut[lut_idx]
-
                     if phi_180:
-                        # two phi solution. choose closest from ancillary wind
-                        diff_angle = np.angle(
-                            one_ancillary_wind / (wspd_co + np.exp(1j * np.deg2rad(wphi_co))))
-                        wphi_co_rad = np.arctan2(
-                            np.sin(diff_angle), np.cos(diff_angle))
+                        # two phi solution (phi & -phi). choose closest from ancillary wind
+
+                        sol = wspd_co * np.exp(1j * np.deg2rad(wphi_co))
+                        sol_2 = wspd_co * \
+                            np.exp(1j * (np.deg2rad(-wphi_co)))
+
+                        diff_angle = np.angle(one_ancillary_wind / sol)
+                        diff_angle_2 = np.angle(one_ancillary_wind / sol_2)
+
+                        wind_co = sol if np.abs(
+                            diff_angle) <= np.abs(diff_angle_2) else sol_2
+
+                        # xr.where(np.abs(diff_angle) > np.pi/2, -sol, sol)
+
                     else:
-                        wphi_co_rad = np.deg2rad(wphi_co)
-                    wind_co = wspd_co * np.exp(1j * wphi_co_rad)
+                        wind_co = wspd_co * np.exp(1j * np.deg2rad(wphi_co))
 
                 else:
-                    # no copol. use ancillary wind as wspd_co (if available)
-                    wind_co = one_ancillary_wind
+                    wind_co = np.nan * 1j
 
                 if not np.isnan(one_sigma0_cr_db) and not np.isnan(one_dsig_cr):
                     # crosspol available, do dualpol inversion
                     i_inc = np.argmin(np.abs(np_inc_cr_dim - one_inc))
                     np_sigma0_cr_lut_db_inc = np_sigma0_cr_lut_db[:, i_inc]
 
                     Jwind_cr = (
                         (np_wspd_lut_cr - np.abs(wind_co)) / dwspd_fg) ** 2.
                     Jsig_cr = ((np_sigma0_cr_lut_db_inc -
-                               one_sigma0_cr_db) / one_dsig_cr) ** 2.
+                                one_sigma0_cr_db) / one_dsig_cr) ** 2.
                     if not np.isnan(np.abs(wind_co)):
                         # dualpol inversion, or crosspol with ancillary wind
                         J_cr = Jsig_cr + Jwind_cr
                     else:
                         # crosspol only inversion
                         J_cr = Jsig_cr
                     # numba doesn't support nanargmin
@@ -257,15 +268,15 @@
         debug = sys.gettrace()
         #  debug = True  # force pure python
         # debug = False # force numba.guvectorize
         if debug:
             logger.debug(
                 'using __invert_from_model_1d in pure python mode (debug)')
 
-            @timing(logger=logger.debug)
+            @ timing(logger=logger.debug)
             def __invert_from_model_vect(*args):
                 ori_shape = args[0].shape
                 args_flat = tuple((arg.flatten() for arg in args))
 
                 out_co = np.empty_like(args_flat[0])
                 out_cr = np.empty_like(args_flat[1])
                 __invert_from_model_1d(*args_flat, out_co, out_cr)
@@ -346,15 +357,15 @@
         inc, sigma0_co_db, sigma0_cr_db, dsig_cr, ancillary_wind)
 
     if models[0] and models[0].iscopol:
         try:
             ws_co.attrs['comment'] = "wind speed and direction inverted from model %s (%s)" % (
                 models[0].name, models[0].pol)
             ws_co.attrs['model'] = models[0].name
-            ws_co.attrs['units'] = 'm/s'
+            #  ws_co.attrs['units'] = 'm/s'
         except AttributeError:
             # numpy only
             pass
 
     if models[1]:
         if sigma0_dual is None and models[1].iscrosspol:
             # crosspol only
@@ -382,12 +393,12 @@
             np.abs(ws_cr_or_dual) < 5), ws_co, ws_cr_or_dual)
         # wspd_dual = ws_cr_or_dual
         try:
             wspd_dual.attrs['comment'] = "wind speed and direction inverted from model %s (%s) and %s (%s)" % (
                 models[0].name, models[0].pol, models[1].name, models[1].pol)
             wspd_dual.attrs['model'] = "%s %s" % (
                 models[0].name, models[1].name)
-            wspd_dual.attrs['units'] = 'm/s'
+            # wspd_dual.attrs['units'] = 'm/s'
         except AttributeError:
             # numpy only
             pass
         return ws_co, wspd_dual
```

### Comparing `xsarsea-0.9/src/xsarsea/xsarsea.py` & `xsarsea-1.0/src/xsarsea/xsarsea.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,15 +33,16 @@
             model, (wind_speed_gmf, wind_dir_gmf),
             template=inc_angle.isel(line=0),
             kwargs={'broadcast': True}
         )
     except AttributeError:
         # this should be the standard way
         # see https://github.com/dask/distributed/issues/3450#issuecomment-585255484
-        sigma0_gmf_sample = model(inc_angle.isel(line=0), wind_speed_gmf, wind_dir_gmf, broadcast=True)
+        sigma0_gmf_sample = model(inc_angle.isel(
+            line=0), wind_speed_gmf, wind_dir_gmf, broadcast=True)
 
     gmf_ratio_sample = sigma0_gmf_sample / np.nanmean(sigma0_gmf_sample)
     detrended = sigma0 / gmf_ratio_sample.broadcast_like(sigma0)
 
     detrended.attrs['comment'] = 'detrended with model %s' % model.name
 
     return detrended
@@ -58,16 +59,18 @@
     Returns
     -------
     xarray.Dataset
         in xsar like format
     """
 
     sarwing_ds = xr.open_dataset(owi_file)
-    sarwing_ds = xr.merge([sarwing_ds, xr.open_dataset(owi_file, group='owiInversionTables_UV')])
-    sarwing_ds = sarwing_ds.rename_dims({'owiAzSize': 'line', 'owiRaSize': 'sample'})
+    sarwing_ds = xr.merge([sarwing_ds, xr.open_dataset(
+        owi_file, group='owiInversionTables_UV')])
+    sarwing_ds = sarwing_ds.rename_dims(
+        {'owiAzSize': 'line', 'owiRaSize': 'sample'})
     sarwing_ds = sarwing_ds.drop_vars(['owiCalConstObsi', 'owiCalConstInci'])
     sarwing_ds = sarwing_ds.assign_coords(
         {'line': np.arange(len(sarwing_ds.line)), 'sample': np.arange(len(sarwing_ds.sample))})
 
     return sarwing_ds
 
 
@@ -97,11 +100,11 @@
     ----------
     sample_dir: geographical direction in degrees north
     ground_heading: azimuth at position, in degrees north
 
     Returns
     -------
     np.float64
-        same shape as input. angle in radian, relative to sample, anticlockwise
+        same shape as input. angle in degrees, relative to sample, anticlockwise
     """
 
-    return 90 - np.rad2deg(sample_dir) + ground_heading
+    return 90 - sample_dir + ground_heading
```

### Comparing `xsarsea-0.9/src/xsarsea.egg-info/PKG-INFO` & `xsarsea-1.0/src/xsarsea.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xsarsea
-Version: 0.9
+Version: 1.0
 Summary: cmod, detrend, and others sar processing tools over ocean
 Home-page: https://github.com/umr-lops/xsarsea
 Author: Olivier Archer
 Author-email: Olivier.Archer@ifremer.fr
 License: MIT
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `xsarsea-0.9/src/xsarsea.egg-info/SOURCES.txt` & `xsarsea-1.0/src/xsarsea.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -17,27 +17,27 @@
 docs/_static/css/xsarsea.css
 docs/examples/gmfs_and_luts.ipynb
 docs/examples/streaks.ipynb
 docs/examples/windspeed_inversion.ipynb
 docs/examples/windspeed_retrieval_L1.ipynb
 docs/examples/xsarsea.ipynb
 src/scripts/configuration_L1B_xspectra_IW_SLC_IFR_v1.yml
-src/scripts/wind_speed_retrieval.py
 src/scripts/xsarsea_cli.py
 src/xsarsea/__init__.py
 src/xsarsea/config.yml
 src/xsarsea/gradients.py
 src/xsarsea/utils.py
 src/xsarsea/xsarsea.py
 src/xsarsea.egg-info/PKG-INFO
 src/xsarsea.egg-info/SOURCES.txt
 src/xsarsea.egg-info/dependency_links.txt
 src/xsarsea.egg-info/requires.txt
 src/xsarsea.egg-info/top_level.txt
 src/xsarsea/windspeed/__init__.py
+src/xsarsea/windspeed/cmod7.py
 src/xsarsea/windspeed/gmfs.py
 src/xsarsea/windspeed/gmfs_impl.py
 src/xsarsea/windspeed/models.py
 src/xsarsea/windspeed/sarwing_luts.py
 src/xsarsea/windspeed/utils.py
 src/xsarsea/windspeed/windspeed.py
 test/test_xsarsea.py
```

### Comparing `xsarsea-0.9/test/test_xsarsea.py` & `xsarsea-1.0/test/test_xsarsea.py`

 * *Files identical despite different names*

