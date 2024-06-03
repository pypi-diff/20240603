# Comparing `tmp/json_x_table-0.0.6.tar.gz` & `tmp/json_x_table-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json_x_table-0.0.6.tar", last modified: Mon Jun  3 03:59:59 2024, max compression
+gzip compressed data, was "json_x_table-0.0.7.tar", last modified: Mon Jun  3 04:21:39 2024, max compression
```

## Comparing `json_x_table-0.0.6.tar` & `json_x_table-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 sagardhande   (501) staff       (20)        0 2024-06-03 03:59:59.790238 json_x_table-0.0.6/
--rw-r--r--   0 sagardhande   (501) staff       (20)     1069 2024-06-01 03:27:44.000000 json_x_table-0.0.6/LICENSE
--rw-r--r--   0 sagardhande   (501) staff       (20)      779 2024-06-03 03:59:59.789842 json_x_table-0.0.6/PKG-INFO
--rw-r--r--   0 sagardhande   (501) staff       (20)       79 2024-06-01 03:27:44.000000 json_x_table-0.0.6/README.md
-drwxr-xr-x   0 sagardhande   (501) staff       (20)        0 2024-06-03 03:59:59.787610 json_x_table-0.0.6/json_x_table/
--rw-r--r--   0 sagardhande   (501) staff       (20)       97 2024-06-02 06:18:13.000000 json_x_table-0.0.6/json_x_table/__init__.py
--rw-r--r--   0 sagardhande   (501) staff       (20)     2858 2024-06-03 03:53:18.000000 json_x_table-0.0.6/json_x_table/table.py
--rw-r--r--   0 sagardhande   (501) staff       (20)      652 2024-06-03 03:21:50.000000 json_x_table-0.0.6/json_x_table/table_parser.py
--rw-r--r--   0 sagardhande   (501) staff       (20)     2063 2024-06-03 03:57:52.000000 json_x_table-0.0.6/json_x_table/text_field.py
-drwxr-xr-x   0 sagardhande   (501) staff       (20)        0 2024-06-03 03:59:59.789374 json_x_table-0.0.6/json_x_table.egg-info/
--rw-r--r--   0 sagardhande   (501) staff       (20)      779 2024-06-03 03:59:59.000000 json_x_table-0.0.6/json_x_table.egg-info/PKG-INFO
--rw-r--r--   0 sagardhande   (501) staff       (20)      308 2024-06-03 03:59:59.000000 json_x_table-0.0.6/json_x_table.egg-info/SOURCES.txt
--rw-r--r--   0 sagardhande   (501) staff       (20)        1 2024-06-03 03:59:59.000000 json_x_table-0.0.6/json_x_table.egg-info/dependency_links.txt
--rw-r--r--   0 sagardhande   (501) staff       (20)       20 2024-06-03 03:59:59.000000 json_x_table-0.0.6/json_x_table.egg-info/requires.txt
--rw-r--r--   0 sagardhande   (501) staff       (20)       13 2024-06-03 03:59:59.000000 json_x_table-0.0.6/json_x_table.egg-info/top_level.txt
--rw-r--r--   0 sagardhande   (501) staff       (20)       38 2024-06-03 03:59:59.790370 json_x_table-0.0.6/setup.cfg
--rw-r--r--   0 sagardhande   (501) staff       (20)      994 2024-06-03 03:58:42.000000 json_x_table-0.0.6/setup.py
+drwxr-xr-x   0 sagardhande   (501) staff       (20)        0 2024-06-03 04:21:39.966852 json_x_table-0.0.7/
+-rw-r--r--   0 sagardhande   (501) staff       (20)     1069 2024-06-01 03:27:44.000000 json_x_table-0.0.7/LICENSE
+-rw-r--r--   0 sagardhande   (501) staff       (20)      779 2024-06-03 04:21:39.966396 json_x_table-0.0.7/PKG-INFO
+-rw-r--r--   0 sagardhande   (501) staff       (20)       79 2024-06-01 03:27:44.000000 json_x_table-0.0.7/README.md
+drwxr-xr-x   0 sagardhande   (501) staff       (20)        0 2024-06-03 04:21:39.964103 json_x_table-0.0.7/json_x_table/
+-rw-r--r--   0 sagardhande   (501) staff       (20)       97 2024-06-02 06:18:13.000000 json_x_table-0.0.7/json_x_table/__init__.py
+-rw-r--r--   0 sagardhande   (501) staff       (20)     2922 2024-06-03 04:17:52.000000 json_x_table-0.0.7/json_x_table/table.py
+-rw-r--r--   0 sagardhande   (501) staff       (20)      652 2024-06-03 03:21:50.000000 json_x_table-0.0.7/json_x_table/table_parser.py
+-rw-r--r--   0 sagardhande   (501) staff       (20)     2063 2024-06-03 03:57:52.000000 json_x_table-0.0.7/json_x_table/text_field.py
+drwxr-xr-x   0 sagardhande   (501) staff       (20)        0 2024-06-03 04:21:39.965935 json_x_table-0.0.7/json_x_table.egg-info/
+-rw-r--r--   0 sagardhande   (501) staff       (20)      779 2024-06-03 04:21:39.000000 json_x_table-0.0.7/json_x_table.egg-info/PKG-INFO
+-rw-r--r--   0 sagardhande   (501) staff       (20)      308 2024-06-03 04:21:39.000000 json_x_table-0.0.7/json_x_table.egg-info/SOURCES.txt
+-rw-r--r--   0 sagardhande   (501) staff       (20)        1 2024-06-03 04:21:39.000000 json_x_table-0.0.7/json_x_table.egg-info/dependency_links.txt
+-rw-r--r--   0 sagardhande   (501) staff       (20)       20 2024-06-03 04:21:39.000000 json_x_table-0.0.7/json_x_table.egg-info/requires.txt
+-rw-r--r--   0 sagardhande   (501) staff       (20)       13 2024-06-03 04:21:39.000000 json_x_table-0.0.7/json_x_table.egg-info/top_level.txt
+-rw-r--r--   0 sagardhande   (501) staff       (20)       38 2024-06-03 04:21:39.967005 json_x_table-0.0.7/setup.cfg
+-rw-r--r--   0 sagardhande   (501) staff       (20)      994 2024-06-03 04:20:53.000000 json_x_table-0.0.7/setup.py
```

### Comparing `json_x_table-0.0.6/LICENSE` & `json_x_table-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `json_x_table-0.0.6/PKG-INFO` & `json_x_table-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json_x_table
-Version: 0.0.6
+Version: 0.0.7
 Summary: Convert your json dump files with a certain format to HTML tables in a fast and efficient way
 Author: Sagar Dhande
 Author-email: dhandesagar78@gmail.com
 Keywords: python3,Json_to_HTML
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
```

### Comparing `json_x_table-0.0.6/json_x_table/table.py` & `json_x_table-0.0.7/json_x_table/table.py`

 * *Files 8% similar despite different names*

```diff
@@ -56,14 +56,15 @@
     """Method to get the string representation of the table"""
     table = f"<table>\n"
     table += f"<caption>{self.name}</caption>\n"
     table += "<thead>\n"
 
   def to_html(self) -> str:
     """Method to get the HTML representation of the table"""
+    no_of_rows = len(self.columns[0]) if self.columns else 0
     html = """<style>
         table {
             border: 2px solid black;
             width: 100%;
             border-collapse: collapse;
         }
 
@@ -79,16 +80,16 @@
     table += "<thead>\n"
     table += "<tr>\n"
     for column in self.columns:
       table += f"<th>{column.name}</th>\n"
     table += "</tr>\n"
     table += "</thead>\n"
     table += "<tbody>\n"
-    for index in range(len(self.columns)):
+    for index in range(len(self.columns[0])):
       table += "<tr>\n"
-      for column in self.columns[index]:
-        table += f"<td>{column}</td>\n"
+      for column in self.columns:
+        table += f"<td>{column[index]}</td>\n"
       table += "</tr>\n"
     table += "</tbody>\n"
     table += "</table>\n"
     return table
```

### Comparing `json_x_table-0.0.6/json_x_table/table_parser.py` & `json_x_table-0.0.7/json_x_table/table_parser.py`

 * *Files identical despite different names*

### Comparing `json_x_table-0.0.6/json_x_table/text_field.py` & `json_x_table-0.0.7/json_x_table/text_field.py`

 * *Files identical despite different names*

### Comparing `json_x_table-0.0.6/json_x_table.egg-info/PKG-INFO` & `json_x_table-0.0.7/json_x_table.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json_x_table
-Version: 0.0.6
+Version: 0.0.7
 Summary: Convert your json dump files with a certain format to HTML tables in a fast and efficient way
 Author: Sagar Dhande
 Author-email: dhandesagar78@gmail.com
 Keywords: python3,Json_to_HTML
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
```

### Comparing `json_x_table-0.0.6/setup.py` & `json_x_table-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-VERSION = '0.0.6' 
+VERSION = '0.0.7' 
 DESCRIPTION = 'Convert your json dump files with a certain format to HTML tables in a fast and efficient way'
 LONG_DESCRIPTION = '''Convert your json dump files with a certain format to HTML tables in a fast and efficient way.\nYou may want to override the functions in order to match any format that you want, with specific customizable column values.'''
 
 setup(
     name="json_x_table", 
     version=VERSION,
     author="Sagar Dhande",
```

