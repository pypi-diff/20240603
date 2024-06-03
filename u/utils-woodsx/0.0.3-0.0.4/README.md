# Comparing `tmp/utils_woodsx-0.0.3.tar.gz` & `tmp/utils_woodsx-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utils_woodsx-0.0.3.tar", last modified: Mon May 13 13:21:21 2024, max compression
+gzip compressed data, was "utils_woodsx-0.0.4.tar", last modified: Mon Jun  3 07:46:34 2024, max compression
```

## Comparing `utils_woodsx-0.0.3.tar` & `utils_woodsx-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 woods      (501) staff       (20)        0 2024-05-13 13:21:21.631574 utils_woodsx-0.0.3/
--rw-r--r--   0 woods      (501) staff       (20)     1065 2024-05-10 09:11:30.000000 utils_woodsx-0.0.3/LICENSE
--rw-r--r--   0 woods      (501) staff       (20)      411 2024-05-13 13:21:21.631384 utils_woodsx-0.0.3/PKG-INFO
--rw-r--r--   0 woods      (501) staff       (20)       49 2024-05-10 09:11:30.000000 utils_woodsx-0.0.3/README.md
--rw-r--r--   0 woods      (501) staff       (20)      435 2024-05-13 13:21:01.000000 utils_woodsx-0.0.3/pyproject.toml
--rw-r--r--   0 woods      (501) staff       (20)       38 2024-05-13 13:21:21.631608 utils_woodsx-0.0.3/setup.cfg
-drwxr-xr-x   0 woods      (501) staff       (20)        0 2024-05-13 13:21:21.630162 utils_woodsx-0.0.3/src/
--rw-r--r--   0 woods      (501) staff       (20)       82 2024-05-13 13:17:25.000000 utils_woodsx-0.0.3/src/text.py
-drwxr-xr-x   0 woods      (501) staff       (20)        0 2024-05-13 13:21:21.630657 utils_woodsx-0.0.3/src/utils_woodsx/
--rw-r--r--   0 woods      (501) staff       (20)        0 2024-05-10 09:11:02.000000 utils_woodsx-0.0.3/src/utils_woodsx/__init__.py
--rw-r--r--   0 woods      (501) staff       (20)       53 2024-05-10 10:06:37.000000 utils_woodsx-0.0.3/src/utils_woodsx/example.py
--rw-r--r--   0 woods      (501) staff       (20)     1323 2024-05-10 09:51:36.000000 utils_woodsx-0.0.3/src/utils_woodsx/excel.py
--rw-r--r--   0 woods      (501) staff       (20)      335 2024-05-13 13:17:25.000000 utils_woodsx-0.0.3/src/utils_woodsx/file.py
--rw-r--r--   0 woods      (501) staff       (20)      867 2024-05-10 09:34:51.000000 utils_woodsx-0.0.3/src/utils_woodsx/html.py
-drwxr-xr-x   0 woods      (501) staff       (20)        0 2024-05-13 13:21:21.631204 utils_woodsx-0.0.3/src/utils_woodsx.egg-info/
--rw-r--r--   0 woods      (501) staff       (20)      411 2024-05-13 13:21:21.000000 utils_woodsx-0.0.3/src/utils_woodsx.egg-info/PKG-INFO
--rw-r--r--   0 woods      (501) staff       (20)      337 2024-05-13 13:21:21.000000 utils_woodsx-0.0.3/src/utils_woodsx.egg-info/SOURCES.txt
--rw-r--r--   0 woods      (501) staff       (20)        1 2024-05-13 13:21:21.000000 utils_woodsx-0.0.3/src/utils_woodsx.egg-info/dependency_links.txt
--rw-r--r--   0 woods      (501) staff       (20)       18 2024-05-13 13:21:21.000000 utils_woodsx-0.0.3/src/utils_woodsx.egg-info/top_level.txt
+drwxr-xr-x   0 woods      (501) staff       (20)        0 2024-06-03 07:46:34.861116 utils_woodsx-0.0.4/
+-rw-r--r--   0 woods      (501) staff       (20)     1065 2024-05-10 09:11:30.000000 utils_woodsx-0.0.4/LICENSE
+-rw-r--r--   0 woods      (501) staff       (20)      411 2024-06-03 07:46:34.860936 utils_woodsx-0.0.4/PKG-INFO
+-rw-r--r--   0 woods      (501) staff       (20)       49 2024-05-10 09:11:30.000000 utils_woodsx-0.0.4/README.md
+-rw-r--r--   0 woods      (501) staff       (20)      435 2024-06-03 07:44:43.000000 utils_woodsx-0.0.4/pyproject.toml
+-rw-r--r--   0 woods      (501) staff       (20)       38 2024-06-03 07:46:34.861148 utils_woodsx-0.0.4/setup.cfg
+drwxr-xr-x   0 woods      (501) staff       (20)        0 2024-06-03 07:46:34.859517 utils_woodsx-0.0.4/src/
+-rw-r--r--   0 woods      (501) staff       (20)       82 2024-06-03 07:44:26.000000 utils_woodsx-0.0.4/src/test.py
+drwxr-xr-x   0 woods      (501) staff       (20)        0 2024-06-03 07:46:34.860122 utils_woodsx-0.0.4/src/utils_woodsx/
+-rw-r--r--   0 woods      (501) staff       (20)        0 2024-05-10 09:11:02.000000 utils_woodsx-0.0.4/src/utils_woodsx/__init__.py
+-rw-r--r--   0 woods      (501) staff       (20)       53 2024-05-10 10:06:37.000000 utils_woodsx-0.0.4/src/utils_woodsx/example.py
+-rw-r--r--   0 woods      (501) staff       (20)     2704 2024-06-03 07:44:26.000000 utils_woodsx-0.0.4/src/utils_woodsx/excel.py
+-rw-r--r--   0 woods      (501) staff       (20)      335 2024-05-30 05:16:31.000000 utils_woodsx-0.0.4/src/utils_woodsx/file.py
+-rw-r--r--   0 woods      (501) staff       (20)      867 2024-05-10 09:34:51.000000 utils_woodsx-0.0.4/src/utils_woodsx/html.py
+drwxr-xr-x   0 woods      (501) staff       (20)        0 2024-06-03 07:46:34.860752 utils_woodsx-0.0.4/src/utils_woodsx.egg-info/
+-rw-r--r--   0 woods      (501) staff       (20)      411 2024-06-03 07:46:34.000000 utils_woodsx-0.0.4/src/utils_woodsx.egg-info/PKG-INFO
+-rw-r--r--   0 woods      (501) staff       (20)      337 2024-06-03 07:46:34.000000 utils_woodsx-0.0.4/src/utils_woodsx.egg-info/SOURCES.txt
+-rw-r--r--   0 woods      (501) staff       (20)        1 2024-06-03 07:46:34.000000 utils_woodsx-0.0.4/src/utils_woodsx.egg-info/dependency_links.txt
+-rw-r--r--   0 woods      (501) staff       (20)       18 2024-06-03 07:46:34.000000 utils_woodsx-0.0.4/src/utils_woodsx.egg-info/top_level.txt
```

### Comparing `utils_woodsx-0.0.3/LICENSE` & `utils_woodsx-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `utils_woodsx-0.0.3/src/utils_woodsx/excel.py` & `utils_woodsx-0.0.4/src/utils_woodsx/excel.py`

 * *Files 20% similar despite different names*

```diff
@@ -43,8 +43,57 @@
     for i in range(len(content)):
         content[i] = "|" + "|".join([str(c) for c in content[i]]) + "|"
 
     content_str = "\n".join(content)
 
     return header_str + "|".join(["----" for g in header]) + "\n" + content_str
 
-excel2mardowntablestr = excel2mdtablestr
+def excel2jsonlist(excel_file_path: str):
+    """
+    Convert excel file to json list.
+    The first row of excel file is the keys of json.
+    The other rows of excel file are the values of json.
+    Remind: the data in the ecxel file should be paste as value first in order to clear the formula! 
+    @param excel_file_path: str, the path of excel file.
+    @return: dict, the json data.
+    """
+    data = get_excel_data(excel_file_path)
+
+    if data is None or len(data) == 0:
+        return None
+    
+    keys = data[0]
+    values = data[1:]
+
+    json_data = []
+
+    for v in values:
+        json_data.append(dict(zip(keys, v)))
+
+    return json_data
+
+def jsonlist2excel(json_list: list, excel_file_path: str):
+    """
+    Convert json list to excel file.
+    The keys of json are the 1st row of excel file.
+    @param json_list: list, the json list.
+    @param excel_file_path: str, the save path of excel file.
+    """
+    import openpyxl
+
+    wb = openpyxl.Workbook()
+    sheet = wb.active
+
+    # The keys of json are the 1st row of excel file.
+    keys = list(json_list[0].keys())
+    sheet.append(keys)
+
+    # The values of json are the other rows of excel file.
+    for json in json_list:
+        values = [json[k] if k in json else None for k in keys]
+        sheet.append(values)
+
+    wb.save(excel_file_path)
+
+excel2mardowntablestr = excel2mdtablestr
+excel2json = excel2jsonlist
+json2excel = jsonlist2excel
```

### Comparing `utils_woodsx-0.0.3/src/utils_woodsx/html.py` & `utils_woodsx-0.0.4/src/utils_woodsx/html.py`

 * *Files identical despite different names*

