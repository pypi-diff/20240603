# Comparing `tmp/pymodins-2.0.6.tar.gz` & `tmp/pymodins-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Vimal\Desktop\pymodins\dist\.tmp-nq35zjv7\pymodins-2.0.6.tar", last modified: Sun Jun  2 19:08:19 2024, max compression
+gzip compressed data, was "C:\Users\Vimal\Desktop\pymodins\dist\.tmp-lt5l474m\pymodins-2.0.7.tar", last modified: Sun Jun  2 19:13:05 2024, max compression
```

## Comparing `pymodins-2.0.6.tar` & `pymodins-2.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-06-02 19:08:19.943999 pymodins-2.0.6/
--rw-rw-rw-   0        0        0     1133 2024-06-02 18:25:44.000000 pymodins-2.0.6/LICENSE
--rw-rw-rw-   0        0        0     4406 2024-06-02 19:08:19.940515 pymodins-2.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     3733 2024-06-02 18:25:47.000000 pymodins-2.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-06-02 19:08:19.910436 pymodins-2.0.6/pymodins/
--rw-rw-rw-   0        0        0      331 2024-06-02 19:07:49.000000 pymodins-2.0.6/pymodins/__init__.py
--rw-rw-rw-   0        0        0    60371 2024-06-02 19:03:55.000000 pymodins-2.0.6/pymodins/installer.py
-drwxrwxrwx   0        0        0        0 2024-06-02 19:08:19.937574 pymodins-2.0.6/pymodins.egg-info/
--rw-rw-rw-   0        0        0     4406 2024-06-02 19:08:19.000000 pymodins-2.0.6/pymodins.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2024-06-02 19:08:19.000000 pymodins-2.0.6/pymodins.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 19:08:19.000000 pymodins-2.0.6/pymodins.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2024-06-02 19:08:19.000000 pymodins-2.0.6/pymodins.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2024-06-02 19:08:19.000000 pymodins-2.0.6/pymodins.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-06-02 19:08:19.000000 pymodins-2.0.6/pymodins.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-06-02 19:08:19.943999 pymodins-2.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1230 2024-06-02 19:08:02.000000 pymodins-2.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 19:13:05.559224 pymodins-2.0.7/
+-rw-rw-rw-   0        0        0     1133 2024-06-02 18:25:44.000000 pymodins-2.0.7/LICENSE
+-rw-rw-rw-   0        0        0     4406 2024-06-02 19:13:05.554655 pymodins-2.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3733 2024-06-02 18:25:47.000000 pymodins-2.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-06-02 19:13:05.522699 pymodins-2.0.7/pymodins/
+-rw-rw-rw-   0        0        0      331 2024-06-02 19:12:39.000000 pymodins-2.0.7/pymodins/__init__.py
+-rw-rw-rw-   0        0        0    60371 2024-06-02 19:03:55.000000 pymodins-2.0.7/pymodins/installer.py
+drwxrwxrwx   0        0        0        0 2024-06-02 19:13:05.551723 pymodins-2.0.7/pymodins.egg-info/
+-rw-rw-rw-   0        0        0     4406 2024-06-02 19:13:05.000000 pymodins-2.0.7/pymodins.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2024-06-02 19:13:05.000000 pymodins-2.0.7/pymodins.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 19:13:05.000000 pymodins-2.0.7/pymodins.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-06-02 19:13:05.000000 pymodins-2.0.7/pymodins.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2024-06-02 19:13:05.000000 pymodins-2.0.7/pymodins.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-06-02 19:13:05.000000 pymodins-2.0.7/pymodins.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-02 19:13:05.559224 pymodins-2.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1377 2024-06-02 19:12:43.000000 pymodins-2.0.7/setup.py
```

### Comparing `pymodins-2.0.6/LICENSE` & `pymodins-2.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pymodins-2.0.6/PKG-INFO` & `pymodins-2.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymodins
-Version: 2.0.6
+Version: 2.0.7
 Summary: A module to install various Python packages.
 Home-page: https://github.com/Nandhan-KA/pymodins
 Author: Nandhan K
 Author-email: nandhan2003alamelu@gmail.com
 Keywords: Python Module Installer,Python Package Installer,python modules installer,python package installer,Nandhan-KA,PYMODINS,pymodins
 Platform: win32
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pymodins-2.0.6/README.md` & `pymodins-2.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pymodins-2.0.6/pymodins/installer.py` & `pymodins-2.0.7/pymodins/installer.py`

 * *Files identical despite different names*

### Comparing `pymodins-2.0.6/pymodins.egg-info/PKG-INFO` & `pymodins-2.0.7/pymodins.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymodins
-Version: 2.0.6
+Version: 2.0.7
 Summary: A module to install various Python packages.
 Home-page: https://github.com/Nandhan-KA/pymodins
 Author: Nandhan K
 Author-email: nandhan2003alamelu@gmail.com
 Keywords: Python Module Installer,Python Package Installer,python modules installer,python package installer,Nandhan-KA,PYMODINS,pymodins
 Platform: win32
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pymodins-2.0.6/setup.py` & `pymodins-2.0.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,42 @@
-import sys
+import platform
 from setuptools import setup, find_packages
 
-if sys.platform != "win32":
-    sys.stderr.write("This program is designed to run on Windows systems only.\n")
-    sys.exit(1)
-
-setup(
-    name="pymodins",
-    version="2.0.6",
-    packages=find_packages(),
-    install_requires=[
-        "rich",
-        "pymsgbox"
-    ],
-    entry_points={
-        "console_scripts": [
-            "pymodins=pymodins.installer:run",
+if platform.system() == "Windows":
+    setup(
+        name="pymodins",
+        version="2.0.7",
+        packages=find_packages(),
+        install_requires=[
+            "rich",
+            "pymsgbox"
+        ],
+        entry_points={
+            "console_scripts": [
+                "pymodins=pymodins.installer:run",
+            ],
+        },
+        author="Nandhan K",
+        author_email="nandhan2003alamelu@gmail.com",
+        description="A module to install various Python packages.",
+        keywords=[
+            "Python Module Installer", 
+            "Python Package Installer", 
+            "python modules installer", 
+            "python package installer", 
+            "Nandhan-KA", 
+            "PYMODINS", 
+            "pymodins"
+        ],
+        long_description=open('README.md').read(),
+        long_description_content_type='text/markdown',
+        url="https://github.com/Nandhan-KA/pymodins",
+        classifiers=[
+            "Programming Language :: Python :: 3",
+            "License :: OSI Approved :: MIT License",
+            "Operating System :: Microsoft :: Windows",
         ],
-    },
-    author="Nandhan K",
-    author_email="nandhan2003alamelu@gmail.com",
-    description="A module to install various Python packages.",
-    keywords=[
-        "Python Module Installer", 
-        "Python Package Installer", 
-        "python modules installer", 
-        "python package installer", 
-        "Nandhan-KA", 
-        "PYMODINS", 
-        "pymodins"
-    ],
-    long_description=open('README.md').read(),
-    long_description_content_type='text/markdown',
-    url="https://github.com/Nandhan-KA/pymodins",
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: Microsoft :: Windows",
-    ],
-    python_requires='>=3.6',
-    platforms=["win32"]
-)
+        python_requires='>=3.6',
+        platforms=["win32"],  
+    )
+else:
+    raise RuntimeError("This program is designed to run on Windows systems only.")
```

