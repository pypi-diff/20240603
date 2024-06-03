# Comparing `tmp/agridable-0.0.3.tar.gz` & `tmp/agridable-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agridable-0.0.3.tar", last modified: Wed May 29 21:48:19 2024, max compression
+gzip compressed data, was "agridable-0.0.4.tar", last modified: Mon Jun  3 13:55:07 2024, max compression
```

## Comparing `agridable-0.0.3.tar` & `agridable-0.0.4.tar`

### file list

```diff
@@ -1,49 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:48:19.236820 agridable-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-29 21:48:14.000000 agridable-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-29 21:48:19.232820 agridable-0.0.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:48:19.228820 agridable-0.0.3/agridable/
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-29 21:48:14.000000 agridable-0.0.3/agridable/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:48:19.228820 agridable-0.0.3/agridable/agridable/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-29 21:48:14.000000 agridable-0.0.3/agridable/agridable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-05-29 21:48:14.000000 agridable-0.0.3/agridable/agridable/agridable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:48:19.228820 agridable-0.0.3/agridable/formats/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:48:14.000000 agridable-0.0.3/agridable/formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-29 21:48:14.000000 agridable-0.0.3/agridable/formats/_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:48:19.232820 agridable-0.0.3/agridable/formats/cell/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-29 21:48:14.000000 agridable-0.0.3/agridable/formats/cell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-29 21:48:14.000000 agridable-0.0.3/agridable/formats/cell/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-05-29 21:48:14.000000 agridable-0.0.3/agridable/formats/cell/align.py
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-29 21:48:14.000000 agridable-0.0.3/agridable/formats/cell/border.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:48:19.232820 agridable-0.0.3/agridable/formats/conditional/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-29 21:48:14.000000 agridable-0.0.3/agridable/formats/conditional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-29 21:48:14.000000 agridable-0.0.3/agridable/formats/conditional/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-05-29 21:48:14.000000 agridable-0.0.3/agridable/formats/conditional/continuous_colour.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-29 21:48:14.000000 agridable-0.0.3/agridable/formats/conditional/discrete_colour.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:48:19.232820 agridable-0.0.3/agridable/formats/grid/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-29 21:48:14.000000 agridable-0.0.3/agridable/formats/grid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-29 21:48:14.000000 agridable-0.0.3/agridable/formats/grid/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-29 21:48:14.000000 agridable-0.0.3/agridable/formats/grid/pin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-29 21:48:14.000000 agridable-0.0.3/agridable/formats/grid/width.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:48:19.232820 agridable-0.0.3/agridable/formats/value/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-29 21:48:14.000000 agridable-0.0.3/agridable/formats/value/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-29 21:48:14.000000 agridable-0.0.3/agridable/formats/value/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-05-29 21:48:14.000000 agridable-0.0.3/agridable/formats/value/currency.py
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-29 21:48:14.000000 agridable-0.0.3/agridable/formats/value/duration.py
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-29 21:48:14.000000 agridable-0.0.3/agridable/formats/value/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-29 21:48:14.000000 agridable-0.0.3/agridable/formats/value/number.py
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-29 21:48:14.000000 agridable-0.0.3/agridable/formats/value/percentage.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-29 21:48:14.000000 agridable-0.0.3/agridable/formats/value/url.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:48:19.232820 agridable-0.0.3/agridable/formatters/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-29 21:48:14.000000 agridable-0.0.3/agridable/formatters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-29 21:48:14.000000 agridable-0.0.3/agridable/formatters/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-05-29 21:48:14.000000 agridable-0.0.3/agridable/formatters/column_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-05-29 21:48:14.000000 agridable-0.0.3/agridable/formatters/conditional_column_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-29 21:48:14.000000 agridable-0.0.3/agridable/formatters/row_formatter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:48:19.232820 agridable-0.0.3/agridable.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-29 21:48:19.000000 agridable-0.0.3/agridable.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-29 21:48:19.000000 agridable-0.0.3/agridable.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 21:48:19.000000 agridable-0.0.3/agridable.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-29 21:48:19.000000 agridable-0.0.3/agridable.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-29 21:48:19.000000 agridable-0.0.3/agridable.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 21:48:19.236820 agridable-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-05-29 21:48:14.000000 agridable-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:55:07.256769 agridable-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-06-03 13:54:55.000000 agridable-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-06-03 13:54:55.000000 agridable-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-06-03 13:55:07.256769 agridable-0.0.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:55:07.248768 agridable-0.0.4/agridable/
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-06-03 13:54:55.000000 agridable-0.0.4/agridable/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:55:07.248768 agridable-0.0.4/agridable/agridable/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-06-03 13:54:55.000000 agridable-0.0.4/agridable/agridable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-06-03 13:54:55.000000 agridable-0.0.4/agridable/agridable/agridable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:55:07.248768 agridable-0.0.4/agridable/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:54:55.000000 agridable-0.0.4/agridable/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-06-03 13:54:55.000000 agridable-0.0.4/agridable/assets/dashAgGridComponentFunctions.js
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-06-03 13:54:55.000000 agridable-0.0.4/agridable/assets/dashAgGridCss.css
+-rw-r--r--   0 runner    (1001) docker     (127)     5574 2024-06-03 13:54:55.000000 agridable-0.0.4/agridable/assets/dashAgGridFunctions.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:55:07.252768 agridable-0.0.4/agridable/formats/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:54:55.000000 agridable-0.0.4/agridable/formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-06-03 13:54:55.000000 agridable-0.0.4/agridable/formats/_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:55:07.252768 agridable-0.0.4/agridable/formats/cell/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-06-03 13:54:55.000000 agridable-0.0.4/agridable/formats/cell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-06-03 13:54:55.000000 agridable-0.0.4/agridable/formats/cell/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-06-03 13:54:55.000000 agridable-0.0.4/agridable/formats/cell/align.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-06-03 13:54:55.000000 agridable-0.0.4/agridable/formats/cell/border.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:55:07.252768 agridable-0.0.4/agridable/formats/conditional/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-06-03 13:54:55.000000 agridable-0.0.4/agridable/formats/conditional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-06-03 13:54:55.000000 agridable-0.0.4/agridable/formats/conditional/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-06-03 13:54:55.000000 agridable-0.0.4/agridable/formats/conditional/continuous_colour.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-06-03 13:54:55.000000 agridable-0.0.4/agridable/formats/conditional/discrete_colour.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:55:07.252768 agridable-0.0.4/agridable/formats/grid/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-06-03 13:54:55.000000 agridable-0.0.4/agridable/formats/grid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-06-03 13:54:55.000000 agridable-0.0.4/agridable/formats/grid/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-06-03 13:54:55.000000 agridable-0.0.4/agridable/formats/grid/pin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-06-03 13:54:55.000000 agridable-0.0.4/agridable/formats/grid/width.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:55:07.252768 agridable-0.0.4/agridable/formats/value/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-06-03 13:54:55.000000 agridable-0.0.4/agridable/formats/value/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-06-03 13:54:55.000000 agridable-0.0.4/agridable/formats/value/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-06-03 13:54:55.000000 agridable-0.0.4/agridable/formats/value/currency.py
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-06-03 13:54:55.000000 agridable-0.0.4/agridable/formats/value/duration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-06-03 13:54:55.000000 agridable-0.0.4/agridable/formats/value/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-06-03 13:54:55.000000 agridable-0.0.4/agridable/formats/value/number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-06-03 13:54:55.000000 agridable-0.0.4/agridable/formats/value/percentage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-06-03 13:54:55.000000 agridable-0.0.4/agridable/formats/value/url.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:55:07.256769 agridable-0.0.4/agridable/formatters/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-06-03 13:54:55.000000 agridable-0.0.4/agridable/formatters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-06-03 13:54:55.000000 agridable-0.0.4/agridable/formatters/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-06-03 13:54:55.000000 agridable-0.0.4/agridable/formatters/column_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-06-03 13:54:55.000000 agridable-0.0.4/agridable/formatters/conditional_column_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-06-03 13:54:55.000000 agridable-0.0.4/agridable/formatters/row_formatter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:55:07.256769 agridable-0.0.4/agridable.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-06-03 13:55:07.000000 agridable-0.0.4/agridable.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-06-03 13:55:07.000000 agridable-0.0.4/agridable.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 13:55:07.000000 agridable-0.0.4/agridable.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-06-03 13:55:07.000000 agridable-0.0.4/agridable.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-03 13:55:07.000000 agridable-0.0.4/agridable.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 13:55:07.256769 agridable-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-06-03 13:54:55.000000 agridable-0.0.4/setup.py
```

### Comparing `agridable-0.0.3/LICENSE` & `agridable-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `agridable-0.0.3/PKG-INFO` & `agridable-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agridable
-Version: 0.0.3
+Version: 0.0.4
 Summary: AGridable is a Python library which makes formatting tables in your Dash app a breeze.
 Home-page: https://github.com/Electrify-Video-Partners/AGridable
 Author: James Laidler
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.12
```

### Comparing `agridable-0.0.3/agridable/agridable/agridable.py` & `agridable-0.0.4/agridable/agridable/agridable.py`

 * *Files identical despite different names*

### Comparing `agridable-0.0.3/agridable/formats/cell/align.py` & `agridable-0.0.4/agridable/formats/cell/align.py`

 * *Files identical despite different names*

### Comparing `agridable-0.0.3/agridable/formats/cell/border.py` & `agridable-0.0.4/agridable/formats/cell/border.py`

 * *Files identical despite different names*

### Comparing `agridable-0.0.3/agridable/formats/conditional/continuous_colour.py` & `agridable-0.0.4/agridable/formats/conditional/continuous_colour.py`

 * *Files identical despite different names*

### Comparing `agridable-0.0.3/agridable/formats/conditional/discrete_colour.py` & `agridable-0.0.4/agridable/formats/conditional/discrete_colour.py`

 * *Files identical despite different names*

### Comparing `agridable-0.0.3/agridable/formats/grid/pin.py` & `agridable-0.0.4/agridable/formats/grid/pin.py`

 * *Files identical despite different names*

### Comparing `agridable-0.0.3/agridable/formats/grid/width.py` & `agridable-0.0.4/agridable/formats/grid/width.py`

 * *Files identical despite different names*

### Comparing `agridable-0.0.3/agridable/formats/value/_base.py` & `agridable-0.0.4/agridable/formats/value/_base.py`

 * *Files identical despite different names*

### Comparing `agridable-0.0.3/agridable/formats/value/currency.py` & `agridable-0.0.4/agridable/formats/value/currency.py`

 * *Files identical despite different names*

### Comparing `agridable-0.0.3/agridable/formats/value/duration.py` & `agridable-0.0.4/agridable/formats/value/duration.py`

 * *Files identical despite different names*

### Comparing `agridable-0.0.3/agridable/formats/value/number.py` & `agridable-0.0.4/agridable/formats/value/number.py`

 * *Files identical despite different names*

### Comparing `agridable-0.0.3/agridable/formats/value/percentage.py` & `agridable-0.0.4/agridable/formats/value/percentage.py`

 * *Files identical despite different names*

### Comparing `agridable-0.0.3/agridable/formatters/_base.py` & `agridable-0.0.4/agridable/formatters/_base.py`

 * *Files identical despite different names*

### Comparing `agridable-0.0.3/agridable/formatters/column_formatter.py` & `agridable-0.0.4/agridable/formatters/column_formatter.py`

 * *Files identical despite different names*

### Comparing `agridable-0.0.3/agridable/formatters/conditional_column_formatter.py` & `agridable-0.0.4/agridable/formatters/conditional_column_formatter.py`

 * *Files identical despite different names*

### Comparing `agridable-0.0.3/agridable/formatters/row_formatter.py` & `agridable-0.0.4/agridable/formatters/row_formatter.py`

 * *Files identical despite different names*

### Comparing `agridable-0.0.3/agridable.egg-info/PKG-INFO` & `agridable-0.0.4/agridable.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agridable
-Version: 0.0.3
+Version: 0.0.4
 Summary: AGridable is a Python library which makes formatting tables in your Dash app a breeze.
 Home-page: https://github.com/Electrify-Video-Partners/AGridable
 Author: James Laidler
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.12
```

### Comparing `agridable-0.0.3/agridable.egg-info/SOURCES.txt` & `agridable-0.0.4/agridable.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 LICENSE
+MANIFEST.in
 setup.py
 agridable/__init__.py
 agridable.egg-info/PKG-INFO
 agridable.egg-info/SOURCES.txt
 agridable.egg-info/dependency_links.txt
 agridable.egg-info/requires.txt
 agridable.egg-info/top_level.txt
 agridable/agridable/__init__.py
 agridable/agridable/agridable.py
+agridable/assets/__init__.py
+agridable/assets/dashAgGridComponentFunctions.js
+agridable/assets/dashAgGridCss.css
+agridable/assets/dashAgGridFunctions.js
 agridable/formats/__init__.py
 agridable/formats/_base.py
 agridable/formats/cell/__init__.py
 agridable/formats/cell/_base.py
 agridable/formats/cell/align.py
 agridable/formats/cell/border.py
 agridable/formats/conditional/__init__.py
```

### Comparing `agridable-0.0.3/setup.py` & `agridable-0.0.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,23 +22,24 @@
     'dev': [
         'twine>=5.0.0,<6.0.0',
         'pytest>=8.2.1,<9.0.0'
     ]
 }
 setuptools.setup(
     name="agridable",
-    version="0.0.3",
+    version="0.0.4",
     author="James Laidler",
     url="https://github.com/Electrify-Video-Partners/AGridable",
     description="AGridable is a Python library which makes formatting tables in your Dash app a breeze.",
     packages=setuptools.find_packages(exclude=['examples']),
     install_requires=INSTALL_REQUIRES,
     extras_require=EXTRAS_REQUIRE,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.12',
     long_description=long_description,
-    long_description_content_type='text/markdown'
+    long_description_content_type='text/markdown',
+    include_package_data=True
 )
```

