# Comparing `tmp/qsv_duct-0.0.1.tar.gz` & `tmp/qsv_duct-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qsv_duct-0.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "qsv_duct-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `qsv_duct-0.0.1.tar` & `qsv_duct-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     2046 2024-06-02 16:32:26.392921 qsv_duct-0.0.1/README.md
--rw-r--r--   0        0        0      485 2024-06-02 17:05:12.247665 qsv_duct-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      187 2024-06-02 17:06:06.296472 qsv_duct-0.0.1/src/qsv/__init__.py
--rw-r--r--   0        0        0     3290 2024-06-02 04:19:20.657248 qsv_duct-0.0.1/src/qsv/count.py
--rw-r--r--   0        0        0     3978 2024-06-02 04:19:55.316493 qsv_duct-0.0.1/src/qsv/sample.py
--rw-r--r--   0        0        0     3062 2024-06-02 04:19:12.966393 qsv_duct-0.0.1/src/qsv/slice.py
--rw-r--r--   0        0        0     2914 2024-06-02 04:44:55.300417 qsv_duct-0.0.1/src/qsv/table.py
--rw-r--r--   0        0        0     2360 1970-01-01 00:00:00.000000 qsv_duct-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2142 2024-06-03 10:40:57.141458 qsv_duct-0.0.2/README.md
+-rw-r--r--   0        0        0      485 2024-06-03 10:40:57.141458 qsv_duct-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      212 2024-06-03 10:40:57.141458 qsv_duct-0.0.2/src/qsv/__init__.py
+-rw-r--r--   0        0        0     3290 2024-06-03 10:40:57.141458 qsv_duct-0.0.2/src/qsv/count.py
+-rw-r--r--   0        0        0     1381 2024-06-03 10:40:57.141458 qsv_duct-0.0.2/src/qsv/index.py
+-rw-r--r--   0        0        0     3978 2024-06-03 10:40:57.141458 qsv_duct-0.0.2/src/qsv/sample.py
+-rw-r--r--   0        0        0     3062 2024-06-03 10:40:57.141458 qsv_duct-0.0.2/src/qsv/slice.py
+-rw-r--r--   0        0        0     2882 2024-06-03 10:40:57.141458 qsv_duct-0.0.2/src/qsv/table.py
+-rw-r--r--   0        0        0     2456 1970-01-01 00:00:00.000000 qsv_duct-0.0.2/PKG-INFO
```

### Comparing `qsv_duct-0.0.1/README.md` & `qsv_duct-0.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# qsv_duct
+# qsv-duct
 
 Python wrapper you may use to call [qsv](https://github.com/jqnatividad/qsv) commands using [duct.py](https://github.com/oconnor663/duct.py) for composability.
 
-This library is compatible with qsv v0.128.0. Not all commands are available.
+This library is compatible with qsv v0.128.0. Not all commands are available (see [`src/qsv/__init__.py`](src/qsv/__init__.py) for available commands).
 
 **Make sure you have qsv installed on your system first and can access it anywhere as a `PATH` command.**
 
 To install this library run:
 
 ```bash
 pip install qsv-duct
@@ -16,15 +16,15 @@
 
 We have a file `fruits.csv` with the following contents:
 
 ```csv
 fruit,price
 apple,2.50
 banana,3.00
-carrot,1.50
+strawberry,1.50
 ```
 
 Let's count the total number of non-header rows in `fruits.csv` using `qsv.count`:
 
 ```python
 import qsv
 
@@ -72,26 +72,26 @@
 fruit   price
 apple   2.50
 banana  3.00
 ```
 
 If you use the `duct.py` library you can also pipe qsv commands with other bash-related commands using the `duct` library's `cmd` function. For example:
 
-```bash
+```python
 import qsv
 from duct import cmd
 
 cmd("cat", "fruits.csv").pipe(qsv.table()).run()
 ```
 
 ```console
-fruit   price
-apple   2.50
-banana  3.00
-carrot  1.50
+fruit       price
+apple       2.50
+banana      3.00
+strawberry  1.50
 ```
 
 ## Testing
 
 You can run the tests with the pytest package:
 
 ```bash
```

### Comparing `qsv_duct-0.0.1/src/qsv/count.py` & `qsv_duct-0.0.2/src/qsv/count.py`

 * *Files identical despite different names*

### Comparing `qsv_duct-0.0.1/src/qsv/sample.py` & `qsv_duct-0.0.2/src/qsv/sample.py`

 * *Files identical despite different names*

### Comparing `qsv_duct-0.0.1/src/qsv/slice.py` & `qsv_duct-0.0.2/src/qsv/slice.py`

 * *Files identical despite different names*

### Comparing `qsv_duct-0.0.1/src/qsv/table.py` & `qsv_duct-0.0.2/src/qsv/table.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from duct import cmd
 
 
 def table(
     file_path: str = "-",
     run: bool = False,
     read: bool = False,
-    include_header_row: bool = True,
     width: int = 2,
     pad: int = 2,
     align: str | None = "left",
     condense: int | None = None,
     output: str | None = None,
     delimiter: str | None = ",",
     memcheck: bool = False,
@@ -72,15 +71,15 @@
     if width:
         args.extend(["-w", str(width)])
     if pad:
         args.extend(["-p", str(pad)])
     if align:
         args.extend(["-a", align])
     if condense:
-        args.extend(["-c", condense])
+        args.extend(["-c", str(condense)])
     if output:
         args.extend(["-o", output])
     if delimiter:
         args.extend(["-d", delimiter])
     if memcheck:
         args.append("--memcheck")
```

### Comparing `qsv_duct-0.0.1/PKG-INFO` & `qsv_duct-0.0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: qsv-duct
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python wrapper based on the qsv CLI tool
 Keywords: qsv,csv
 Author: Mueez Khan
 Description-Content-Type: text/markdown
 Requires-Dist: duct
 Requires-Dist: pytest ; extra == "test"
 Project-URL: Home, https://github.com/rzmk/qsv-duct
 Provides-Extra: test
 
-# qsv_duct
+# qsv-duct
 
 Python wrapper you may use to call [qsv](https://github.com/jqnatividad/qsv) commands using [duct.py](https://github.com/oconnor663/duct.py) for composability.
 
-This library is compatible with qsv v0.128.0. Not all commands are available.
+This library is compatible with qsv v0.128.0. Not all commands are available (see [`src/qsv/__init__.py`](src/qsv/__init__.py) for available commands).
 
 **Make sure you have qsv installed on your system first and can access it anywhere as a `PATH` command.**
 
 To install this library run:
 
 ```bash
 pip install qsv-duct
@@ -28,15 +28,15 @@
 
 We have a file `fruits.csv` with the following contents:
 
 ```csv
 fruit,price
 apple,2.50
 banana,3.00
-carrot,1.50
+strawberry,1.50
 ```
 
 Let's count the total number of non-header rows in `fruits.csv` using `qsv.count`:
 
 ```python
 import qsv
 
@@ -84,26 +84,26 @@
 fruit   price
 apple   2.50
 banana  3.00
 ```
 
 If you use the `duct.py` library you can also pipe qsv commands with other bash-related commands using the `duct` library's `cmd` function. For example:
 
-```bash
+```python
 import qsv
 from duct import cmd
 
 cmd("cat", "fruits.csv").pipe(qsv.table()).run()
 ```
 
 ```console
-fruit   price
-apple   2.50
-banana  3.00
-carrot  1.50
+fruit       price
+apple       2.50
+banana      3.00
+strawberry  1.50
 ```
 
 ## Testing
 
 You can run the tests with the pytest package:
 
 ```bash
```

