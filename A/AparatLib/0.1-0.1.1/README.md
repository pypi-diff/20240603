# Comparing `tmp/aparatlib-0.1.tar.gz` & `tmp/aparatlib-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aparatlib-0.1.tar", last modified: Sun Jun  2 10:28:17 2024, max compression
+gzip compressed data, was "aparatlib-0.1.1.tar", last modified: Sun Jun  2 10:55:58 2024, max compression
```

## Comparing `aparatlib-0.1.tar` & `aparatlib-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-06-02 10:28:17.531121 aparatlib-0.1/
-drwxrwxrwx   0        0        0        0 2024-06-02 10:28:17.529040 aparatlib-0.1/AparatLib.egg-info/
--rw-rw-rw-   0        0        0      258 2024-06-02 10:28:17.000000 aparatlib-0.1/AparatLib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2024-06-02 10:28:17.000000 aparatlib-0.1/AparatLib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 10:28:17.000000 aparatlib-0.1/AparatLib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-06-02 10:28:17.000000 aparatlib-0.1/AparatLib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-06-02 10:28:17.000000 aparatlib-0.1/AparatLib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1090 2024-06-02 06:49:28.000000 aparatlib-0.1/LICENSE
--rw-rw-rw-   0        0        0      258 2024-06-02 10:28:17.529040 aparatlib-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      113 2024-06-02 06:46:16.000000 aparatlib-0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-06-02 10:28:17.525136 aparatlib-0.1/aparat/
--rw-rw-rw-   0        0        0       52 2024-06-02 06:45:10.000000 aparatlib-0.1/aparat/__init__.py
--rw-rw-rw-   0        0        0     9131 2024-06-02 09:34:21.000000 aparatlib-0.1/aparat/aparat.py
--rw-rw-rw-   0        0        0       42 2024-06-02 10:28:17.531121 aparatlib-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1067 2024-06-02 10:28:02.000000 aparatlib-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-06-02 10:28:17.527094 aparatlib-0.1/tests/
--rw-rw-rw-   0        0        0        0 2024-06-02 06:44:06.000000 aparatlib-0.1/tests/__init__.py
--rw-rw-rw-   0        0        0      977 2024-06-02 09:38:58.000000 aparatlib-0.1/tests/test_aparat.py
+drwxrwxrwx   0        0        0        0 2024-06-02 10:55:58.994670 aparatlib-0.1.1/
+drwxrwxrwx   0        0        0        0 2024-06-02 10:55:58.993688 aparatlib-0.1.1/AparatLib.egg-info/
+-rw-rw-rw-   0        0        0      707 2024-06-02 10:55:58.000000 aparatlib-0.1.1/AparatLib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2024-06-02 10:55:58.000000 aparatlib-0.1.1/AparatLib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 10:55:58.000000 aparatlib-0.1.1/AparatLib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-06-02 10:55:58.000000 aparatlib-0.1.1/AparatLib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-06-02 10:55:58.000000 aparatlib-0.1.1/AparatLib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1090 2024-06-02 06:49:28.000000 aparatlib-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      707 2024-06-02 10:55:58.993688 aparatlib-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      404 2024-06-02 10:47:18.000000 aparatlib-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-06-02 10:55:58.990132 aparatlib-0.1.1/aparat/
+-rw-rw-rw-   0        0        0       52 2024-06-02 06:45:10.000000 aparatlib-0.1.1/aparat/__init__.py
+-rw-rw-rw-   0        0        0     9131 2024-06-02 09:34:21.000000 aparatlib-0.1.1/aparat/aparat.py
+-rw-rw-rw-   0        0        0       42 2024-06-02 10:55:58.994670 aparatlib-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1241 2024-06-02 10:55:54.000000 aparatlib-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 10:55:58.992212 aparatlib-0.1.1/tests/
+-rw-rw-rw-   0        0        0        0 2024-06-02 06:44:06.000000 aparatlib-0.1.1/tests/__init__.py
+-rw-rw-rw-   0        0        0      977 2024-06-02 09:38:58.000000 aparatlib-0.1.1/tests/test_aparat.py
```

### Comparing `aparatlib-0.1/LICENSE` & `aparatlib-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aparatlib-0.1/aparat/aparat.py` & `aparatlib-0.1.1/aparat/aparat.py`

 * *Files identical despite different names*

### Comparing `aparatlib-0.1/setup.py` & `aparatlib-0.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,17 +21,19 @@
 #     python_requires='>=3.6',
 # )
 
 from setuptools import setup, find_packages
 
 setup(
     name='AparatLib',
-    version='0.1',
+    version='0.1.1',
     packages=find_packages(),
     install_requires=[
         'requests',
     ],
     author='Abol',
     author_email='abaqry8686@gmail.com',
     description='A library for interacting with the Aparat API',
+    long_description=open('C:\\Users\\Bagheri\\Desktop\\projects\\python\\Github projects\\aparat\\README.md').read(),
+    long_description_content_type='text/markdown',
     url='https://github.com/AbolDev/aparat-api',
 )
```

### Comparing `aparatlib-0.1/tests/test_aparat.py` & `aparatlib-0.1.1/tests/test_aparat.py`

 * *Files identical despite different names*

