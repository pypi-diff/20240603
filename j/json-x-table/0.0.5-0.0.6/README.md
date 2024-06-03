# Comparing `tmp/json_x_table-0.0.5.tar.gz` & `tmp/json_x_table-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json_x_table-0.0.5.tar", last modified: Mon Jun  3 03:56:06 2024, max compression
+gzip compressed data, was "json_x_table-0.0.6.tar", last modified: Mon Jun  3 03:59:59 2024, max compression
```

## Comparing `json_x_table-0.0.5.tar` & `json_x_table-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 sagardhande   (501) staff       (20)        0 2024-06-03 03:56:06.830399 json_x_table-0.0.5/
--rw-r--r--   0 sagardhande   (501) staff       (20)     1069 2024-06-01 03:27:44.000000 json_x_table-0.0.5/LICENSE
--rw-r--r--   0 sagardhande   (501) staff       (20)      779 2024-06-03 03:56:06.830090 json_x_table-0.0.5/PKG-INFO
--rw-r--r--   0 sagardhande   (501) staff       (20)       79 2024-06-01 03:27:44.000000 json_x_table-0.0.5/README.md
-drwxr-xr-x   0 sagardhande   (501) staff       (20)        0 2024-06-03 03:56:06.828104 json_x_table-0.0.5/json_x_table/
--rw-r--r--   0 sagardhande   (501) staff       (20)       97 2024-06-02 06:18:13.000000 json_x_table-0.0.5/json_x_table/__init__.py
--rw-r--r--   0 sagardhande   (501) staff       (20)     2858 2024-06-03 03:53:18.000000 json_x_table-0.0.5/json_x_table/table.py
--rw-r--r--   0 sagardhande   (501) staff       (20)      652 2024-06-03 03:21:50.000000 json_x_table-0.0.5/json_x_table/table_parser.py
--rw-r--r--   0 sagardhande   (501) staff       (20)     2062 2024-06-03 03:40:04.000000 json_x_table-0.0.5/json_x_table/text_field.py
-drwxr-xr-x   0 sagardhande   (501) staff       (20)        0 2024-06-03 03:56:06.829681 json_x_table-0.0.5/json_x_table.egg-info/
--rw-r--r--   0 sagardhande   (501) staff       (20)      779 2024-06-03 03:56:06.000000 json_x_table-0.0.5/json_x_table.egg-info/PKG-INFO
--rw-r--r--   0 sagardhande   (501) staff       (20)      308 2024-06-03 03:56:06.000000 json_x_table-0.0.5/json_x_table.egg-info/SOURCES.txt
--rw-r--r--   0 sagardhande   (501) staff       (20)        1 2024-06-03 03:56:06.000000 json_x_table-0.0.5/json_x_table.egg-info/dependency_links.txt
--rw-r--r--   0 sagardhande   (501) staff       (20)       20 2024-06-03 03:56:06.000000 json_x_table-0.0.5/json_x_table.egg-info/requires.txt
--rw-r--r--   0 sagardhande   (501) staff       (20)       13 2024-06-03 03:56:06.000000 json_x_table-0.0.5/json_x_table.egg-info/top_level.txt
--rw-r--r--   0 sagardhande   (501) staff       (20)       38 2024-06-03 03:56:06.830517 json_x_table-0.0.5/setup.cfg
--rw-r--r--   0 sagardhande   (501) staff       (20)      994 2024-06-03 03:55:09.000000 json_x_table-0.0.5/setup.py
+drwxr-xr-x   0 sagardhande   (501) staff       (20)        0 2024-06-03 03:59:59.790238 json_x_table-0.0.6/
+-rw-r--r--   0 sagardhande   (501) staff       (20)     1069 2024-06-01 03:27:44.000000 json_x_table-0.0.6/LICENSE
+-rw-r--r--   0 sagardhande   (501) staff       (20)      779 2024-06-03 03:59:59.789842 json_x_table-0.0.6/PKG-INFO
+-rw-r--r--   0 sagardhande   (501) staff       (20)       79 2024-06-01 03:27:44.000000 json_x_table-0.0.6/README.md
+drwxr-xr-x   0 sagardhande   (501) staff       (20)        0 2024-06-03 03:59:59.787610 json_x_table-0.0.6/json_x_table/
+-rw-r--r--   0 sagardhande   (501) staff       (20)       97 2024-06-02 06:18:13.000000 json_x_table-0.0.6/json_x_table/__init__.py
+-rw-r--r--   0 sagardhande   (501) staff       (20)     2858 2024-06-03 03:53:18.000000 json_x_table-0.0.6/json_x_table/table.py
+-rw-r--r--   0 sagardhande   (501) staff       (20)      652 2024-06-03 03:21:50.000000 json_x_table-0.0.6/json_x_table/table_parser.py
+-rw-r--r--   0 sagardhande   (501) staff       (20)     2063 2024-06-03 03:57:52.000000 json_x_table-0.0.6/json_x_table/text_field.py
+drwxr-xr-x   0 sagardhande   (501) staff       (20)        0 2024-06-03 03:59:59.789374 json_x_table-0.0.6/json_x_table.egg-info/
+-rw-r--r--   0 sagardhande   (501) staff       (20)      779 2024-06-03 03:59:59.000000 json_x_table-0.0.6/json_x_table.egg-info/PKG-INFO
+-rw-r--r--   0 sagardhande   (501) staff       (20)      308 2024-06-03 03:59:59.000000 json_x_table-0.0.6/json_x_table.egg-info/SOURCES.txt
+-rw-r--r--   0 sagardhande   (501) staff       (20)        1 2024-06-03 03:59:59.000000 json_x_table-0.0.6/json_x_table.egg-info/dependency_links.txt
+-rw-r--r--   0 sagardhande   (501) staff       (20)       20 2024-06-03 03:59:59.000000 json_x_table-0.0.6/json_x_table.egg-info/requires.txt
+-rw-r--r--   0 sagardhande   (501) staff       (20)       13 2024-06-03 03:59:59.000000 json_x_table-0.0.6/json_x_table.egg-info/top_level.txt
+-rw-r--r--   0 sagardhande   (501) staff       (20)       38 2024-06-03 03:59:59.790370 json_x_table-0.0.6/setup.cfg
+-rw-r--r--   0 sagardhande   (501) staff       (20)      994 2024-06-03 03:58:42.000000 json_x_table-0.0.6/setup.py
```

### Comparing `json_x_table-0.0.5/LICENSE` & `json_x_table-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `json_x_table-0.0.5/PKG-INFO` & `json_x_table-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json_x_table
-Version: 0.0.5
+Version: 0.0.6
 Summary: Convert your json dump files with a certain format to HTML tables in a fast and efficient way
 Author: Sagar Dhande
 Author-email: dhandesagar78@gmail.com
 Keywords: python3,Json_to_HTML
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
```

### Comparing `json_x_table-0.0.5/json_x_table/table.py` & `json_x_table-0.0.6/json_x_table/table.py`

 * *Files identical despite different names*

### Comparing `json_x_table-0.0.5/json_x_table/table_parser.py` & `json_x_table-0.0.6/json_x_table/table_parser.py`

 * *Files identical despite different names*

### Comparing `json_x_table-0.0.5/json_x_table/text_field.py` & `json_x_table-0.0.6/json_x_table/text_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
   def __iter__(self):
     """Method to iterate over the text field"""
     self.index = 0
     return self
 
   def __next__(self) -> Any:
     """Method to get the next value of the text field"""
-    if self.index > len(self.rows):
+    if self.index >= len(self.rows):
       self.index = 0
       raise StopIteration
     self.index += 1
     return self.rows[self.index - 1]
 
   def __str__(self):
     return f"<input type='text' value='{self.name}'>"
```

### Comparing `json_x_table-0.0.5/json_x_table.egg-info/PKG-INFO` & `json_x_table-0.0.6/json_x_table.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json_x_table
-Version: 0.0.5
+Version: 0.0.6
 Summary: Convert your json dump files with a certain format to HTML tables in a fast and efficient way
 Author: Sagar Dhande
 Author-email: dhandesagar78@gmail.com
 Keywords: python3,Json_to_HTML
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
```

### Comparing `json_x_table-0.0.5/setup.py` & `json_x_table-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-VERSION = '0.0.5' 
+VERSION = '0.0.6' 
 DESCRIPTION = 'Convert your json dump files with a certain format to HTML tables in a fast and efficient way'
 LONG_DESCRIPTION = '''Convert your json dump files with a certain format to HTML tables in a fast and efficient way.\nYou may want to override the functions in order to match any format that you want, with specific customizable column values.'''
 
 setup(
     name="json_x_table", 
     version=VERSION,
     author="Sagar Dhande",
```

