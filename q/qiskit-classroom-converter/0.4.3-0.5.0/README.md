# Comparing `tmp/qiskit-classroom-converter-0.4.3.tar.gz` & `tmp/qiskit-classroom-converter-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit-classroom-converter-0.4.3.tar", last modified: Sat Dec  2 00:47:06 2023, max compression
+gzip compressed data, was "qiskit-classroom-converter-0.5.0.tar", last modified: Wed Mar  6 03:41:45 2024, max compression
```

## Comparing `qiskit-classroom-converter-0.4.3.tar` & `qiskit-classroom-converter-0.5.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 00:47:06.554238 qiskit-classroom-converter-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11350 2023-12-02 00:46:56.000000 qiskit-classroom-converter-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       59 2023-12-02 00:46:56.000000 qiskit-classroom-converter-0.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3991 2023-12-02 00:47:06.554238 qiskit-classroom-converter-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2890 2023-12-02 00:46:56.000000 qiskit-classroom-converter-0.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2023-12-02 00:46:56.000000 qiskit-classroom-converter-0.4.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 00:47:06.550238 qiskit-classroom-converter-0.4.3/qiskit_class_converter/
--rw-r--r--   0 runner    (1001) docker     (127)     3761 2023-12-02 00:46:56.000000 qiskit-classroom-converter-0.4.3/qiskit_class_converter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 00:47:06.550238 qiskit-classroom-converter-0.4.3/qiskit_class_converter/converters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-02 00:46:56.000000 qiskit-classroom-converter-0.4.3/qiskit_class_converter/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2023-12-02 00:46:56.000000 qiskit-classroom-converter-0.4.3/qiskit_class_converter/converters/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2023-12-02 00:46:56.000000 qiskit-classroom-converter-0.4.3/qiskit_class_converter/converters/matrix_to_quantum_circuit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2023-12-02 00:46:56.000000 qiskit-classroom-converter-0.4.3/qiskit_class_converter/converters/quantum_circuit_to_braket_notation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4750 2023-12-02 00:46:56.000000 qiskit-classroom-converter-0.4.3/qiskit_class_converter/converters/quantum_circuit_to_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     3911 2023-12-02 00:46:56.000000 qiskit-classroom-converter-0.4.3/qiskit_class_converter/converters/string_to_braket_notation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 00:47:06.550238 qiskit-classroom-converter-0.4.3/qiskit_class_converter/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-02 00:46:56.000000 qiskit-classroom-converter-0.4.3/qiskit_class_converter/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4331 2023-12-02 00:46:56.000000 qiskit-classroom-converter-0.4.3/qiskit_class_converter/services/converter_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 00:47:06.554238 qiskit-classroom-converter-0.4.3/qiskit_classroom_converter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3991 2023-12-02 00:47:06.000000 qiskit-classroom-converter-0.4.3/qiskit_classroom_converter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      801 2023-12-02 00:47:06.000000 qiskit-classroom-converter-0.4.3/qiskit_classroom_converter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-02 00:47:06.000000 qiskit-classroom-converter-0.4.3/qiskit_classroom_converter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      210 2023-12-02 00:47:06.000000 qiskit-classroom-converter-0.4.3/qiskit_classroom_converter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-02 00:47:06.000000 qiskit-classroom-converter-0.4.3/qiskit_classroom_converter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      118 2023-12-02 00:46:56.000000 qiskit-classroom-converter-0.4.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2023-12-02 00:47:06.554238 qiskit-classroom-converter-0.4.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 03:41:45.177227 qiskit-classroom-converter-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11350 2024-03-06 03:41:40.000000 qiskit-classroom-converter-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-06 03:41:40.000000 qiskit-classroom-converter-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-03-06 03:41:45.177227 qiskit-classroom-converter-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-03-06 03:41:40.000000 qiskit-classroom-converter-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-03-06 03:41:40.000000 qiskit-classroom-converter-0.5.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 03:41:45.177227 qiskit-classroom-converter-0.5.0/qiskit_class_converter/
+-rw-r--r--   0 runner    (1001) docker     (127)     3761 2024-03-06 03:41:40.000000 qiskit-classroom-converter-0.5.0/qiskit_class_converter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 03:41:45.177227 qiskit-classroom-converter-0.5.0/qiskit_class_converter/converters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 03:41:40.000000 qiskit-classroom-converter-0.5.0/qiskit_class_converter/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-03-06 03:41:40.000000 qiskit-classroom-converter-0.5.0/qiskit_class_converter/converters/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-03-06 03:41:40.000000 qiskit-classroom-converter-0.5.0/qiskit_class_converter/converters/matrix_to_quantum_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-03-06 03:41:40.000000 qiskit-classroom-converter-0.5.0/qiskit_class_converter/converters/quantum_circuit_to_braket_notation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3721 2024-03-06 03:41:40.000000 qiskit-classroom-converter-0.5.0/qiskit_class_converter/converters/quantum_circuit_to_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-03-06 03:41:40.000000 qiskit-classroom-converter-0.5.0/qiskit_class_converter/converters/string_to_braket_notation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 03:41:45.177227 qiskit-classroom-converter-0.5.0/qiskit_class_converter/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 03:41:40.000000 qiskit-classroom-converter-0.5.0/qiskit_class_converter/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-03-06 03:41:40.000000 qiskit-classroom-converter-0.5.0/qiskit_class_converter/services/converter_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 03:41:45.177227 qiskit-classroom-converter-0.5.0/qiskit_classroom_converter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-03-06 03:41:45.000000 qiskit-classroom-converter-0.5.0/qiskit_classroom_converter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-03-06 03:41:45.000000 qiskit-classroom-converter-0.5.0/qiskit_classroom_converter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 03:41:45.000000 qiskit-classroom-converter-0.5.0/qiskit_classroom_converter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-03-06 03:41:45.000000 qiskit-classroom-converter-0.5.0/qiskit_classroom_converter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-06 03:41:45.000000 qiskit-classroom-converter-0.5.0/qiskit_classroom_converter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-03-06 03:41:40.000000 qiskit-classroom-converter-0.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-06 03:41:45.181227 qiskit-classroom-converter-0.5.0/setup.cfg
```

### Comparing `qiskit-classroom-converter-0.4.3/LICENSE` & `qiskit-classroom-converter-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qiskit-classroom-converter-0.4.3/PKG-INFO` & `qiskit-classroom-converter-0.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 Metadata-Version: 2.1
 Name: qiskit-classroom-converter
-Version: 0.4.3
+Version: 0.5.0
 Summary: extend the Qiskit classroom applications.
 Author: KMU-quantum-classroom
 Project-URL: Homepage, https://github.com/KMU-quantum-classroom/qiskit-classroom-converter
 Project-URL: Bug Tracker, https://github.com/KMU-quantum-classroom/qiskit-classroom-converter/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: qiskit==0.45.1
-Requires-Dist: qiskit-aer==0.13.1
+Requires-Dist: qiskit==1.0.1
+Requires-Dist: qiskit-aer==0.13.3
 Requires-Dist: loguru==0.7.2
 Requires-Dist: sympy==1.12
 Requires-Dist: antlr4-python3-runtime==4.11
 Requires-Dist: ipython==8.18.1
-Requires-Dist: numpy==1.26.2
+Requires-Dist: numpy==1.26.4
 Provides-Extra: dev
-Requires-Dist: coverage==7.3.2; extra == "dev"
-Requires-Dist: pylint==3.0.2; extra == "dev"
+Requires-Dist: coverage==7.4.3; extra == "dev"
+Requires-Dist: pylint==3.1.0; extra == "dev"
 Requires-Dist: tox==4.11.4; extra == "dev"
 Requires-Dist: build==1.0.3; extra == "dev"
-Requires-Dist: pdoc==14.1.0; extra == "dev"
-Requires-Dist: notebook==7.0.6; extra == "dev"
+Requires-Dist: pdoc==14.4.0; extra == "dev"
+Requires-Dist: notebook==7.1.1; extra == "dev"
 
 # qiskit-classroom-converter
 Qiskit classroom Converter
 
+> 0.5.0 (2024-03-06) : The Version has been updated to be compatible with **Qiskit 1.0.0** and **Python 3.12**.
+
+
 ## Documents
 
 https://kmu-quantum-classroom.github.io/qiskit-classroom-converter/qiskit_class_converter.html
 
 ## Official USER Guide
 
 https://kmu-quantum-classroom.github.io/documents/overview.html
```

### Comparing `qiskit-classroom-converter-0.4.3/README.md` & `qiskit-classroom-converter-0.5.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 # qiskit-classroom-converter
 Qiskit classroom Converter
 
+> 0.5.0 (2024-03-06) : The Version has been updated to be compatible with **Qiskit 1.0.0** and **Python 3.12**.
+
+
 ## Documents
 
 https://kmu-quantum-classroom.github.io/qiskit-classroom-converter/qiskit_class_converter.html
 
 ## Official USER Guide
 
 https://kmu-quantum-classroom.github.io/documents/overview.html
```

### Comparing `qiskit-classroom-converter-0.4.3/pyproject.toml` & `qiskit-classroom-converter-0.5.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -9,42 +9,42 @@
 
 [tool.setuptools.packages.find]
 include = ['qiskit_class_converter*']
 exclude = ['qiskit_class_converter*tests']
 
 [project]
 name = "qiskit-classroom-converter"
-version = "0.4.3"
+version = "0.5.0"
 authors = [
     { name = "KMU-quantum-classroom" },
 ]
 description = "extend the Qiskit classroom applications."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "qiskit==0.45.1",
-    "qiskit-aer==0.13.1",
+    "qiskit==1.0.1",
+    "qiskit-aer==0.13.3",
     "loguru==0.7.2",
     "sympy==1.12",
     "antlr4-python3-runtime==4.11",
     "ipython==8.18.1",
-    "numpy==1.26.2"
+    "numpy==1.26.4"
 ]
 
 [project.optional-dependencies]
 dev = [
-    "coverage==7.3.2",
-    "pylint==3.0.2",
+    "coverage==7.4.3",
+    "pylint==3.1.0",
     "tox==4.11.4",
     "build==1.0.3",
-    "pdoc==14.1.0",
-    "notebook==7.0.6"
+    "pdoc==14.4.0",
+    "notebook==7.1.1"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/KMU-quantum-classroom/qiskit-classroom-converter"
 "Bug Tracker" = "https://github.com/KMU-quantum-classroom/qiskit-classroom-converter/issues"
```

### Comparing `qiskit-classroom-converter-0.4.3/qiskit_class_converter/__init__.py` & `qiskit-classroom-converter-0.5.0/qiskit_class_converter/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-classroom-converter-0.4.3/qiskit_class_converter/converters/base.py` & `qiskit-classroom-converter-0.5.0/qiskit_class_converter/converters/base.py`

 * *Files identical despite different names*

### Comparing `qiskit-classroom-converter-0.4.3/qiskit_class_converter/converters/matrix_to_quantum_circuit.py` & `qiskit-classroom-converter-0.5.0/qiskit_class_converter/converters/matrix_to_quantum_circuit.py`

 * *Files identical despite different names*

### Comparing `qiskit-classroom-converter-0.4.3/qiskit_class_converter/converters/quantum_circuit_to_braket_notation.py` & `qiskit-classroom-converter-0.5.0/qiskit_class_converter/converters/quantum_circuit_to_braket_notation.py`

 * *Files identical despite different names*

### Comparing `qiskit-classroom-converter-0.4.3/qiskit_class_converter/converters/string_to_braket_notation.py` & `qiskit-classroom-converter-0.5.0/qiskit_class_converter/converters/string_to_braket_notation.py`

 * *Files identical despite different names*

### Comparing `qiskit-classroom-converter-0.4.3/qiskit_class_converter/services/converter_service.py` & `qiskit-classroom-converter-0.5.0/qiskit_class_converter/services/converter_service.py`

 * *Files identical despite different names*

### Comparing `qiskit-classroom-converter-0.4.3/qiskit_classroom_converter.egg-info/PKG-INFO` & `qiskit-classroom-converter-0.5.0/qiskit_classroom_converter.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 Metadata-Version: 2.1
 Name: qiskit-classroom-converter
-Version: 0.4.3
+Version: 0.5.0
 Summary: extend the Qiskit classroom applications.
 Author: KMU-quantum-classroom
 Project-URL: Homepage, https://github.com/KMU-quantum-classroom/qiskit-classroom-converter
 Project-URL: Bug Tracker, https://github.com/KMU-quantum-classroom/qiskit-classroom-converter/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: qiskit==0.45.1
-Requires-Dist: qiskit-aer==0.13.1
+Requires-Dist: qiskit==1.0.1
+Requires-Dist: qiskit-aer==0.13.3
 Requires-Dist: loguru==0.7.2
 Requires-Dist: sympy==1.12
 Requires-Dist: antlr4-python3-runtime==4.11
 Requires-Dist: ipython==8.18.1
-Requires-Dist: numpy==1.26.2
+Requires-Dist: numpy==1.26.4
 Provides-Extra: dev
-Requires-Dist: coverage==7.3.2; extra == "dev"
-Requires-Dist: pylint==3.0.2; extra == "dev"
+Requires-Dist: coverage==7.4.3; extra == "dev"
+Requires-Dist: pylint==3.1.0; extra == "dev"
 Requires-Dist: tox==4.11.4; extra == "dev"
 Requires-Dist: build==1.0.3; extra == "dev"
-Requires-Dist: pdoc==14.1.0; extra == "dev"
-Requires-Dist: notebook==7.0.6; extra == "dev"
+Requires-Dist: pdoc==14.4.0; extra == "dev"
+Requires-Dist: notebook==7.1.1; extra == "dev"
 
 # qiskit-classroom-converter
 Qiskit classroom Converter
 
+> 0.5.0 (2024-03-06) : The Version has been updated to be compatible with **Qiskit 1.0.0** and **Python 3.12**.
+
+
 ## Documents
 
 https://kmu-quantum-classroom.github.io/qiskit-classroom-converter/qiskit_class_converter.html
 
 ## Official USER Guide
 
 https://kmu-quantum-classroom.github.io/documents/overview.html
```

### Comparing `qiskit-classroom-converter-0.4.3/qiskit_classroom_converter.egg-info/SOURCES.txt` & `qiskit-classroom-converter-0.5.0/qiskit_classroom_converter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

