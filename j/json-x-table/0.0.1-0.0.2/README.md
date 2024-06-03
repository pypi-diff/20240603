# Comparing `tmp/json_x_table-0.0.1.tar.gz` & `tmp/json_x_table-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json_x_table-0.0.1.tar", last modified: Sun Jun  2 03:57:27 2024, max compression
+gzip compressed data, was "json_x_table-0.0.2.tar", last modified: Sun Jun  2 06:19:52 2024, max compression
```

## Comparing `json_x_table-0.0.1.tar` & `json_x_table-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,17 @@
-drwxr-xr-x   0 sagardhande   (501) staff       (20)        0 2024-06-02 03:57:27.701622 json_x_table-0.0.1/
--rw-r--r--   0 sagardhande   (501) staff       (20)     1069 2024-06-01 03:27:44.000000 json_x_table-0.0.1/LICENSE
--rw-r--r--   0 sagardhande   (501) staff       (20)      729 2024-06-02 03:57:27.701279 json_x_table-0.0.1/PKG-INFO
--rw-r--r--   0 sagardhande   (501) staff       (20)       79 2024-06-01 03:27:44.000000 json_x_table-0.0.1/README.md
-drwxr-xr-x   0 sagardhande   (501) staff       (20)        0 2024-06-02 03:57:27.700898 json_x_table-0.0.1/json_x_table.egg-info/
--rw-r--r--   0 sagardhande   (501) staff       (20)      729 2024-06-02 03:57:27.000000 json_x_table-0.0.1/json_x_table.egg-info/PKG-INFO
--rw-r--r--   0 sagardhande   (501) staff       (20)      170 2024-06-02 03:57:27.000000 json_x_table-0.0.1/json_x_table.egg-info/SOURCES.txt
--rw-r--r--   0 sagardhande   (501) staff       (20)        1 2024-06-02 03:57:27.000000 json_x_table-0.0.1/json_x_table.egg-info/dependency_links.txt
--rw-r--r--   0 sagardhande   (501) staff       (20)        1 2024-06-02 03:57:27.000000 json_x_table-0.0.1/json_x_table.egg-info/top_level.txt
--rw-r--r--   0 sagardhande   (501) staff       (20)       38 2024-06-02 03:57:27.701716 json_x_table-0.0.1/setup.cfg
--rw-r--r--   0 sagardhande   (501) staff       (20)      983 2024-06-02 03:53:24.000000 json_x_table-0.0.1/setup.py
+drwxr-xr-x   0 sagardhande   (501) staff       (20)        0 2024-06-02 06:19:52.768345 json_x_table-0.0.2/
+-rw-r--r--   0 sagardhande   (501) staff       (20)     1069 2024-06-01 03:27:44.000000 json_x_table-0.0.2/LICENSE
+-rw-r--r--   0 sagardhande   (501) staff       (20)      784 2024-06-02 06:19:52.768134 json_x_table-0.0.2/PKG-INFO
+-rw-r--r--   0 sagardhande   (501) staff       (20)       79 2024-06-01 03:27:44.000000 json_x_table-0.0.2/README.md
+drwxr-xr-x   0 sagardhande   (501) staff       (20)        0 2024-06-02 06:19:52.766862 json_x_table-0.0.2/json_x_table/
+-rw-r--r--   0 sagardhande   (501) staff       (20)       97 2024-06-02 06:18:13.000000 json_x_table-0.0.2/json_x_table/__init__.py
+-rw-r--r--   0 sagardhande   (501) staff       (20)     2858 2024-06-02 06:18:13.000000 json_x_table-0.0.2/json_x_table/table.py
+-rw-r--r--   0 sagardhande   (501) staff       (20)      644 2024-06-02 06:18:13.000000 json_x_table-0.0.2/json_x_table/table_parser.py
+-rw-r--r--   0 sagardhande   (501) staff       (20)     2063 2024-06-02 06:18:13.000000 json_x_table-0.0.2/json_x_table/text_field.py
+drwxr-xr-x   0 sagardhande   (501) staff       (20)        0 2024-06-02 06:19:52.767857 json_x_table-0.0.2/json_x_table.egg-info/
+-rw-r--r--   0 sagardhande   (501) staff       (20)      784 2024-06-02 06:19:52.000000 json_x_table-0.0.2/json_x_table.egg-info/PKG-INFO
+-rw-r--r--   0 sagardhande   (501) staff       (20)      308 2024-06-02 06:19:52.000000 json_x_table-0.0.2/json_x_table.egg-info/SOURCES.txt
+-rw-r--r--   0 sagardhande   (501) staff       (20)        1 2024-06-02 06:19:52.000000 json_x_table-0.0.2/json_x_table.egg-info/dependency_links.txt
+-rw-r--r--   0 sagardhande   (501) staff       (20)       20 2024-06-02 06:19:52.000000 json_x_table-0.0.2/json_x_table.egg-info/requires.txt
+-rw-r--r--   0 sagardhande   (501) staff       (20)       13 2024-06-02 06:19:52.000000 json_x_table-0.0.2/json_x_table.egg-info/top_level.txt
+-rw-r--r--   0 sagardhande   (501) staff       (20)       38 2024-06-02 06:19:52.768471 json_x_table-0.0.2/setup.cfg
+-rw-r--r--   0 sagardhande   (501) staff       (20)      994 2024-06-02 06:19:37.000000 json_x_table-0.0.2/setup.py
```

### Comparing `json_x_table-0.0.1/LICENSE` & `json_x_table-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `json_x_table-0.0.1/PKG-INFO` & `json_x_table-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 Metadata-Version: 2.1
 Name: json_x_table
-Version: 0.0.1
+Version: 0.0.2
 Summary: Convert your json dump files with a certain format to HTML tables in a fast and efficient way
+Home-page: UNKNOWN
 Author: Sagar Dhande
 Author-email: dhandesagar78@gmail.com
+License: UNKNOWN
 Keywords: python3,Json_to_HTML
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 License-File: LICENSE
 
 Convert your json dump files with a certain format to HTML tables in a fast and efficient way.
 You may want to override the functions in order to match any format that you want, with specific customizable column values.
+
```

### Comparing `json_x_table-0.0.1/json_x_table.egg-info/PKG-INFO` & `json_x_table-0.0.2/json_x_table.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 Metadata-Version: 2.1
-Name: json_x_table
-Version: 0.0.1
+Name: json-x-table
+Version: 0.0.2
 Summary: Convert your json dump files with a certain format to HTML tables in a fast and efficient way
+Home-page: UNKNOWN
 Author: Sagar Dhande
 Author-email: dhandesagar78@gmail.com
+License: UNKNOWN
 Keywords: python3,Json_to_HTML
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 License-File: LICENSE
 
 Convert your json dump files with a certain format to HTML tables in a fast and efficient way.
 You may want to override the functions in order to match any format that you want, with specific customizable column values.
+
```

### Comparing `json_x_table-0.0.1/setup.py` & `json_x_table-0.0.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import find_packages, setup
 
-VERSION = '0.0.1' 
+VERSION = '0.0.2' 
 DESCRIPTION = 'Convert your json dump files with a certain format to HTML tables in a fast and efficient way'
 LONG_DESCRIPTION = '''Convert your json dump files with a certain format to HTML tables in a fast and efficient way.\nYou may want to override the functions in order to match any format that you want, with specific customizable column values.'''
 
 setup(
     name="json_x_table", 
     version=VERSION,
     author="Sagar Dhande",
     author_email="dhandesagar78@gmail.com",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
-    packages=find_packages("jsoncomment"),
-    install_requires=[],
+    packages=find_packages(),
+    install_requires=["jsoncomment", "pathlib"],
     keywords=['python3', 'Json_to_HTML'],
     classifiers= [
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Education",
         "Programming Language :: Python :: 3",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
```

