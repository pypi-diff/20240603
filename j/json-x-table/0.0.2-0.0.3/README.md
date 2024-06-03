# Comparing `tmp/json_x_table-0.0.2.tar.gz` & `tmp/json_x_table-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json_x_table-0.0.2.tar", last modified: Sun Jun  2 06:19:52 2024, max compression
+gzip compressed data, was "json_x_table-0.0.3.tar", last modified: Mon Jun  3 03:25:39 2024, max compression
```

## Comparing `json_x_table-0.0.2.tar` & `json_x_table-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 sagardhande   (501) staff       (20)        0 2024-06-02 06:19:52.768345 json_x_table-0.0.2/
--rw-r--r--   0 sagardhande   (501) staff       (20)     1069 2024-06-01 03:27:44.000000 json_x_table-0.0.2/LICENSE
--rw-r--r--   0 sagardhande   (501) staff       (20)      784 2024-06-02 06:19:52.768134 json_x_table-0.0.2/PKG-INFO
--rw-r--r--   0 sagardhande   (501) staff       (20)       79 2024-06-01 03:27:44.000000 json_x_table-0.0.2/README.md
-drwxr-xr-x   0 sagardhande   (501) staff       (20)        0 2024-06-02 06:19:52.766862 json_x_table-0.0.2/json_x_table/
--rw-r--r--   0 sagardhande   (501) staff       (20)       97 2024-06-02 06:18:13.000000 json_x_table-0.0.2/json_x_table/__init__.py
--rw-r--r--   0 sagardhande   (501) staff       (20)     2858 2024-06-02 06:18:13.000000 json_x_table-0.0.2/json_x_table/table.py
--rw-r--r--   0 sagardhande   (501) staff       (20)      644 2024-06-02 06:18:13.000000 json_x_table-0.0.2/json_x_table/table_parser.py
--rw-r--r--   0 sagardhande   (501) staff       (20)     2063 2024-06-02 06:18:13.000000 json_x_table-0.0.2/json_x_table/text_field.py
-drwxr-xr-x   0 sagardhande   (501) staff       (20)        0 2024-06-02 06:19:52.767857 json_x_table-0.0.2/json_x_table.egg-info/
--rw-r--r--   0 sagardhande   (501) staff       (20)      784 2024-06-02 06:19:52.000000 json_x_table-0.0.2/json_x_table.egg-info/PKG-INFO
--rw-r--r--   0 sagardhande   (501) staff       (20)      308 2024-06-02 06:19:52.000000 json_x_table-0.0.2/json_x_table.egg-info/SOURCES.txt
--rw-r--r--   0 sagardhande   (501) staff       (20)        1 2024-06-02 06:19:52.000000 json_x_table-0.0.2/json_x_table.egg-info/dependency_links.txt
--rw-r--r--   0 sagardhande   (501) staff       (20)       20 2024-06-02 06:19:52.000000 json_x_table-0.0.2/json_x_table.egg-info/requires.txt
--rw-r--r--   0 sagardhande   (501) staff       (20)       13 2024-06-02 06:19:52.000000 json_x_table-0.0.2/json_x_table.egg-info/top_level.txt
--rw-r--r--   0 sagardhande   (501) staff       (20)       38 2024-06-02 06:19:52.768471 json_x_table-0.0.2/setup.cfg
--rw-r--r--   0 sagardhande   (501) staff       (20)      994 2024-06-02 06:19:37.000000 json_x_table-0.0.2/setup.py
+drwxr-xr-x   0 sagardhande   (501) staff       (20)        0 2024-06-03 03:25:39.580759 json_x_table-0.0.3/
+-rw-r--r--   0 sagardhande   (501) staff       (20)     1069 2024-06-01 03:27:44.000000 json_x_table-0.0.3/LICENSE
+-rw-r--r--   0 sagardhande   (501) staff       (20)      779 2024-06-03 03:25:39.580377 json_x_table-0.0.3/PKG-INFO
+-rw-r--r--   0 sagardhande   (501) staff       (20)       79 2024-06-01 03:27:44.000000 json_x_table-0.0.3/README.md
+drwxr-xr-x   0 sagardhande   (501) staff       (20)        0 2024-06-03 03:25:39.578022 json_x_table-0.0.3/json_x_table/
+-rw-r--r--   0 sagardhande   (501) staff       (20)       97 2024-06-02 06:18:13.000000 json_x_table-0.0.3/json_x_table/__init__.py
+-rw-r--r--   0 sagardhande   (501) staff       (20)     2858 2024-06-02 06:18:13.000000 json_x_table-0.0.3/json_x_table/table.py
+-rw-r--r--   0 sagardhande   (501) staff       (20)      652 2024-06-03 03:21:50.000000 json_x_table-0.0.3/json_x_table/table_parser.py
+-rw-r--r--   0 sagardhande   (501) staff       (20)     2063 2024-06-02 06:18:13.000000 json_x_table-0.0.3/json_x_table/text_field.py
+drwxr-xr-x   0 sagardhande   (501) staff       (20)        0 2024-06-03 03:25:39.579916 json_x_table-0.0.3/json_x_table.egg-info/
+-rw-r--r--   0 sagardhande   (501) staff       (20)      779 2024-06-03 03:25:39.000000 json_x_table-0.0.3/json_x_table.egg-info/PKG-INFO
+-rw-r--r--   0 sagardhande   (501) staff       (20)      308 2024-06-03 03:25:39.000000 json_x_table-0.0.3/json_x_table.egg-info/SOURCES.txt
+-rw-r--r--   0 sagardhande   (501) staff       (20)        1 2024-06-03 03:25:39.000000 json_x_table-0.0.3/json_x_table.egg-info/dependency_links.txt
+-rw-r--r--   0 sagardhande   (501) staff       (20)       20 2024-06-03 03:25:39.000000 json_x_table-0.0.3/json_x_table.egg-info/requires.txt
+-rw-r--r--   0 sagardhande   (501) staff       (20)       13 2024-06-03 03:25:39.000000 json_x_table-0.0.3/json_x_table.egg-info/top_level.txt
+-rw-r--r--   0 sagardhande   (501) staff       (20)       38 2024-06-03 03:25:39.580882 json_x_table-0.0.3/setup.cfg
+-rw-r--r--   0 sagardhande   (501) staff       (20)      994 2024-06-03 03:23:12.000000 json_x_table-0.0.3/setup.py
```

### Comparing `json_x_table-0.0.2/LICENSE` & `json_x_table-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `json_x_table-0.0.2/PKG-INFO` & `json_x_table-0.0.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: json_x_table
-Version: 0.0.2
+Version: 0.0.3
 Summary: Convert your json dump files with a certain format to HTML tables in a fast and efficient way
-Home-page: UNKNOWN
 Author: Sagar Dhande
 Author-email: dhandesagar78@gmail.com
-License: UNKNOWN
 Keywords: python3,Json_to_HTML
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 License-File: LICENSE
+Requires-Dist: jsoncomment
+Requires-Dist: pathlib
 
 Convert your json dump files with a certain format to HTML tables in a fast and efficient way.
 You may want to override the functions in order to match any format that you want, with specific customizable column values.
-
```

### Comparing `json_x_table-0.0.2/json_x_table/table.py` & `json_x_table-0.0.3/json_x_table/table.py`

 * *Files identical despite different names*

### Comparing `json_x_table-0.0.2/json_x_table/table_parser.py` & `json_x_table-0.0.3/json_x_table/table_parser.py`

 * *Files 27% similar despite different names*

```diff
@@ -14,15 +14,15 @@
   "float": float
 }
 
 def parse_table(file_path: pathlib.Path) -> Table:
   json_parser = JsonComment(json)
   data = json_parser.loads(file_path.read_text())
   table = Table()
-  for row, data in data.items():
+  for row, row_data in data.items():
     rows = []
-    for column, value in data.items():
+    for column, value in row_data.items():
       if column not in table: 
         table.add_column(column, types_mapping[value["type"]])
       rows.append(value["value"])
     table.add_rows(rows)
   return table
```

### Comparing `json_x_table-0.0.2/json_x_table/text_field.py` & `json_x_table-0.0.3/json_x_table/text_field.py`

 * *Files identical despite different names*

### Comparing `json_x_table-0.0.2/json_x_table.egg-info/PKG-INFO` & `json_x_table-0.0.3/json_x_table.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
-Name: json-x-table
-Version: 0.0.2
+Name: json_x_table
+Version: 0.0.3
 Summary: Convert your json dump files with a certain format to HTML tables in a fast and efficient way
-Home-page: UNKNOWN
 Author: Sagar Dhande
 Author-email: dhandesagar78@gmail.com
-License: UNKNOWN
 Keywords: python3,Json_to_HTML
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 License-File: LICENSE
+Requires-Dist: jsoncomment
+Requires-Dist: pathlib
 
 Convert your json dump files with a certain format to HTML tables in a fast and efficient way.
 You may want to override the functions in order to match any format that you want, with specific customizable column values.
-
```

### Comparing `json_x_table-0.0.2/setup.py` & `json_x_table-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-VERSION = '0.0.2' 
+VERSION = '0.0.3' 
 DESCRIPTION = 'Convert your json dump files with a certain format to HTML tables in a fast and efficient way'
 LONG_DESCRIPTION = '''Convert your json dump files with a certain format to HTML tables in a fast and efficient way.\nYou may want to override the functions in order to match any format that you want, with specific customizable column values.'''
 
 setup(
     name="json_x_table", 
     version=VERSION,
     author="Sagar Dhande",
```

