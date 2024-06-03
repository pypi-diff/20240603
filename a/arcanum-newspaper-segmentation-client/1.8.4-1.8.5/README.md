# Comparing `tmp/arcanum-newspaper-segmentation-client-1.8.4.tar.gz` & `tmp/arcanum_newspaper_segmentation_client-1.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcanum-newspaper-segmentation-client-1.8.4.tar", last modified: Mon Jan 29 12:01:09 2024, max compression
+gzip compressed data, was "arcanum_newspaper_segmentation_client-1.8.5.tar", last modified: Mon Jun  3 11:58:02 2024, max compression
```

## Comparing `arcanum-newspaper-segmentation-client-1.8.4.tar` & `arcanum_newspaper_segmentation_client-1.8.5.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-01-29 12:01:09.654803 arcanum-newspaper-segmentation-client-1.8.4/
--rw-rw-rw-   0        0        0     1101 2022-01-17 15:03:50.000000 arcanum-newspaper-segmentation-client-1.8.4/LICENSE
--rw-rw-rw-   0        0        0      755 2024-01-29 12:01:09.653841 arcanum-newspaper-segmentation-client-1.8.4/PKG-INFO
--rw-rw-rw-   0        0        0      156 2022-01-17 15:03:50.000000 arcanum-newspaper-segmentation-client-1.8.4/README.md
--rw-rw-rw-   0        0        0      110 2022-01-17 15:03:50.000000 arcanum-newspaper-segmentation-client-1.8.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-01-29 12:01:09.654803 arcanum-newspaper-segmentation-client-1.8.4/setup.cfg
--rw-rw-rw-   0        0        0      901 2024-01-29 11:59:54.000000 arcanum-newspaper-segmentation-client-1.8.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-01-29 12:01:09.623886 arcanum-newspaper-segmentation-client-1.8.4/src/
-drwxrwxrwx   0        0        0        0 2024-01-29 12:01:09.652825 arcanum-newspaper-segmentation-client-1.8.4/src/arcanum_newspaper_segmentation_client.egg-info/
--rw-rw-rw-   0        0        0      755 2024-01-29 12:01:09.000000 arcanum-newspaper-segmentation-client-1.8.4/src/arcanum_newspaper_segmentation_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      494 2024-01-29 12:01:09.000000 arcanum-newspaper-segmentation-client-1.8.4/src/arcanum_newspaper_segmentation_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-29 12:01:09.000000 arcanum-newspaper-segmentation-client-1.8.4/src/arcanum_newspaper_segmentation_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-01-29 12:01:09.000000 arcanum-newspaper-segmentation-client-1.8.4/src/arcanum_newspaper_segmentation_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       30 2024-01-29 12:01:09.000000 arcanum-newspaper-segmentation-client-1.8.4/src/arcanum_newspaper_segmentation_client.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-01-29 12:01:09.652825 arcanum-newspaper-segmentation-client-1.8.4/src/newspaper_segmentation_client/
--rw-rw-rw-   0        0        0     1314 2024-01-29 12:00:02.000000 arcanum-newspaper-segmentation-client-1.8.4/src/newspaper_segmentation_client/__init__.py
--rw-rw-rw-   0        0        0     1434 2023-04-07 19:07:15.000000 arcanum-newspaper-segmentation-client-1.8.4/src/newspaper_segmentation_client/clip.py
--rw-rw-rw-   0        0        0      546 2024-01-29 11:59:32.000000 arcanum-newspaper-segmentation-client-1.8.4/src/newspaper_segmentation_client/pdf.py
+drwxrwxrwx   0        0        0        0 2024-06-03 11:58:02.496073 arcanum_newspaper_segmentation_client-1.8.5/
+-rw-rw-rw-   0        0        0     1101 2022-01-17 15:03:50.000000 arcanum_newspaper_segmentation_client-1.8.5/LICENSE
+-rw-rw-rw-   0        0        0      723 2024-06-03 11:58:02.495083 arcanum_newspaper_segmentation_client-1.8.5/PKG-INFO
+-rw-rw-rw-   0        0        0      156 2022-01-17 15:03:50.000000 arcanum_newspaper_segmentation_client-1.8.5/README.md
+-rw-rw-rw-   0        0        0      110 2022-01-17 15:03:50.000000 arcanum_newspaper_segmentation_client-1.8.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-06-03 11:58:02.496073 arcanum_newspaper_segmentation_client-1.8.5/setup.cfg
+-rw-rw-rw-   0        0        0      873 2024-06-03 11:57:38.000000 arcanum_newspaper_segmentation_client-1.8.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 11:58:02.471013 arcanum_newspaper_segmentation_client-1.8.5/src/
+drwxrwxrwx   0        0        0        0 2024-06-03 11:58:02.494077 arcanum_newspaper_segmentation_client-1.8.5/src/arcanum_newspaper_segmentation_client.egg-info/
+-rw-rw-rw-   0        0        0      723 2024-06-03 11:58:02.000000 arcanum_newspaper_segmentation_client-1.8.5/src/arcanum_newspaper_segmentation_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      453 2024-06-03 11:58:02.000000 arcanum_newspaper_segmentation_client-1.8.5/src/arcanum_newspaper_segmentation_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 11:58:02.000000 arcanum_newspaper_segmentation_client-1.8.5/src/arcanum_newspaper_segmentation_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-06-03 11:58:02.000000 arcanum_newspaper_segmentation_client-1.8.5/src/arcanum_newspaper_segmentation_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       30 2024-06-03 11:58:02.000000 arcanum_newspaper_segmentation_client-1.8.5/src/arcanum_newspaper_segmentation_client.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-03 11:58:02.493080 arcanum_newspaper_segmentation_client-1.8.5/src/newspaper_segmentation_client/
+-rw-rw-rw-   0        0        0     1314 2024-03-05 09:53:37.000000 arcanum_newspaper_segmentation_client-1.8.5/src/newspaper_segmentation_client/__init__.py
+-rw-rw-rw-   0        0        0     1434 2023-04-07 19:07:15.000000 arcanum_newspaper_segmentation_client-1.8.5/src/newspaper_segmentation_client/clip.py
```

### Comparing `arcanum-newspaper-segmentation-client-1.8.4/LICENSE` & `arcanum_newspaper_segmentation_client-1.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `arcanum-newspaper-segmentation-client-1.8.4/PKG-INFO` & `arcanum_newspaper_segmentation_client-1.8.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: arcanum-newspaper-segmentation-client
-Version: 1.8.4
+Version: 1.8.5
 Summary: Client for Arcanum's Newspaper Segmentation API
 Home-page: https://www.arcanum.com/en/newspaper-segmentation/
 Author: Biszak Előd (Arcanum Ltd)
 Author-email: elod.biszak@arcanum.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pillow
 Requires-Dist: requests
-Requires-Dist: pymupdf>=1.21.1
 
 # Arcanum Newspaper Segmentation client
 
 Client for Arcanum Newspaper Segmentation API.
 [Read more](https://www.arcanum.com/en/newspaper-segmentation/)
```

### Comparing `arcanum-newspaper-segmentation-client-1.8.4/setup.py` & `arcanum_newspaper_segmentation_client-1.8.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="arcanum-newspaper-segmentation-client",
-    version="1.8.4",
+    version="1.8.5",
     author="Biszak Előd (Arcanum Ltd)",
     author_email="elod.biszak@arcanum.com",
     description="Client for Arcanum's Newspaper Segmentation API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.arcanum.com/en/newspaper-segmentation/",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
         'pillow',
-        'requests',
-        'pymupdf>=1.21.1'
+        'requests'
     ],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
     python_requires=">=3.8",
 )
```

### Comparing `arcanum-newspaper-segmentation-client-1.8.4/src/arcanum_newspaper_segmentation_client.egg-info/PKG-INFO` & `arcanum_newspaper_segmentation_client-1.8.5/src/arcanum_newspaper_segmentation_client.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: arcanum-newspaper-segmentation-client
-Version: 1.8.4
+Version: 1.8.5
 Summary: Client for Arcanum's Newspaper Segmentation API
 Home-page: https://www.arcanum.com/en/newspaper-segmentation/
 Author: Biszak Előd (Arcanum Ltd)
 Author-email: elod.biszak@arcanum.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pillow
 Requires-Dist: requests
-Requires-Dist: pymupdf>=1.21.1
 
 # Arcanum Newspaper Segmentation client
 
 Client for Arcanum Newspaper Segmentation API.
 [Read more](https://www.arcanum.com/en/newspaper-segmentation/)
```

### Comparing `arcanum-newspaper-segmentation-client-1.8.4/src/newspaper_segmentation_client/__init__.py` & `arcanum_newspaper_segmentation_client-1.8.5/src/newspaper_segmentation_client/__init__.py`

 * *Files identical despite different names*

### Comparing `arcanum-newspaper-segmentation-client-1.8.4/src/newspaper_segmentation_client/clip.py` & `arcanum_newspaper_segmentation_client-1.8.5/src/newspaper_segmentation_client/clip.py`

 * *Files identical despite different names*

