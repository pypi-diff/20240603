# Comparing `tmp/cyclicpeptide-1.0.6.tar.gz` & `tmp/cyclicpeptide-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyclicpeptide-1.0.6.tar", last modified: Mon Jun  3 02:18:01 2024, max compression
+gzip compressed data, was "cyclicpeptide-1.0.7.tar", last modified: Mon Jun  3 02:36:49 2024, max compression
```

## Comparing `cyclicpeptide-1.0.6.tar` & `cyclicpeptide-1.0.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 willow     (501) staff       (20)        0 2024-06-03 02:18:01.779192 cyclicpeptide-1.0.6/
--rw-r--r--   0 willow     (501) staff       (20)     1093 2024-05-31 02:24:37.000000 cyclicpeptide-1.0.6/LICENSE.md
--rw-r--r--   0 willow     (501) staff       (20)     2571 2024-06-03 02:18:01.779129 cyclicpeptide-1.0.6/PKG-INFO
--rw-r--r--   0 willow     (501) staff       (20)     1918 2024-05-31 03:28:51.000000 cyclicpeptide-1.0.6/README.md
-drwxr-xr-x   0 willow     (501) staff       (20)        0 2024-06-03 02:18:01.777878 cyclicpeptide-1.0.6/cyclicpeptide/
--rw-r--r--   0 willow     (501) staff       (20)     1134 2024-03-07 07:35:40.000000 cyclicpeptide-1.0.6/cyclicpeptide/AminoAcids.txt
--rw-r--r--   0 willow     (501) staff       (20)     1662 2024-03-19 07:31:14.000000 cyclicpeptide-1.0.6/cyclicpeptide/Chemical_P.csv
--rwxr-xr-x   0 willow     (501) staff       (20)     5859 2024-05-24 07:25:18.000000 cyclicpeptide-1.0.6/cyclicpeptide/GraphAlignment.py
--rw-r--r--   0 willow     (501) staff       (20)     2476 2024-05-31 06:42:27.000000 cyclicpeptide-1.0.6/cyclicpeptide/IOManager.py
--rw-r--r--   0 willow     (501) staff       (20)     5380 2024-05-31 03:39:15.000000 cyclicpeptide-1.0.6/cyclicpeptide/PropertyAnalysis.py
--rwxr-xr-x   0 willow     (501) staff       (20)     9977 2024-06-03 02:11:18.000000 cyclicpeptide-1.0.6/cyclicpeptide/Sequence2Structure.py
--rw-r--r--   0 willow     (501) staff       (20)    10985 2024-06-03 02:09:58.000000 cyclicpeptide-1.0.6/cyclicpeptide/SequenceTransformer.py
--rwxr-xr-x   0 willow     (501) staff       (20)    39366 2024-06-03 02:13:14.000000 cyclicpeptide-1.0.6/cyclicpeptide/Structure2Sequence.py
--rw-r--r--   0 willow     (501) staff       (20)     2476 2024-04-08 03:27:53.000000 cyclicpeptide-1.0.6/cyclicpeptide/StructureTransformer.py
--rw-r--r--   0 willow     (501) staff       (20)        0 2024-05-31 02:15:42.000000 cyclicpeptide-1.0.6/cyclicpeptide/__init__.py
--rw-r--r--   0 willow     (501) staff       (20)      502 2024-03-08 01:11:36.000000 cyclicpeptide-1.0.6/cyclicpeptide/aa_smiles.txt
--rw-r--r--   0 willow     (501) staff       (20)      116 2024-03-08 01:12:56.000000 cyclicpeptide-1.0.6/cyclicpeptide/aas.txt
--rw-r--r--   0 willow     (501) staff       (20)    79050 2024-05-28 02:09:41.000000 cyclicpeptide-1.0.6/cyclicpeptide/monomer.tsv
--rw-r--r--   0 willow     (501) staff       (20)      365 2024-06-03 02:15:21.000000 cyclicpeptide-1.0.6/cyclicpeptide/setting.py
-drwxr-xr-x   0 willow     (501) staff       (20)        0 2024-06-03 02:18:01.778809 cyclicpeptide-1.0.6/cyclicpeptide.egg-info/
--rw-r--r--   0 willow     (501) staff       (20)     2571 2024-06-03 02:18:01.000000 cyclicpeptide-1.0.6/cyclicpeptide.egg-info/PKG-INFO
--rw-r--r--   0 willow     (501) staff       (20)      648 2024-06-03 02:18:01.000000 cyclicpeptide-1.0.6/cyclicpeptide.egg-info/SOURCES.txt
--rw-r--r--   0 willow     (501) staff       (20)        1 2024-06-03 02:18:01.000000 cyclicpeptide-1.0.6/cyclicpeptide.egg-info/dependency_links.txt
--rw-r--r--   0 willow     (501) staff       (20)       92 2024-06-03 02:18:01.000000 cyclicpeptide-1.0.6/cyclicpeptide.egg-info/requires.txt
--rw-r--r--   0 willow     (501) staff       (20)       14 2024-06-03 02:18:01.000000 cyclicpeptide-1.0.6/cyclicpeptide.egg-info/top_level.txt
--rw-r--r--   0 willow     (501) staff       (20)       78 2024-06-03 02:18:01.779571 cyclicpeptide-1.0.6/setup.cfg
--rw-r--r--   0 willow     (501) staff       (20)     1124 2024-06-03 02:17:39.000000 cyclicpeptide-1.0.6/setup.py
+drwxr-xr-x   0 willow     (501) staff       (20)        0 2024-06-03 02:36:49.124698 cyclicpeptide-1.0.7/
+-rw-r--r--   0 willow     (501) staff       (20)     1093 2024-05-31 02:24:37.000000 cyclicpeptide-1.0.7/LICENSE.md
+-rw-r--r--   0 willow     (501) staff       (20)     2569 2024-06-03 02:36:49.124635 cyclicpeptide-1.0.7/PKG-INFO
+-rw-r--r--   0 willow     (501) staff       (20)     1918 2024-05-31 03:28:51.000000 cyclicpeptide-1.0.7/README.md
+drwxr-xr-x   0 willow     (501) staff       (20)        0 2024-06-03 02:36:49.123345 cyclicpeptide-1.0.7/cyclicpeptide/
+-rw-r--r--   0 willow     (501) staff       (20)     1134 2024-03-07 07:35:40.000000 cyclicpeptide-1.0.7/cyclicpeptide/AminoAcids.txt
+-rw-r--r--   0 willow     (501) staff       (20)     1662 2024-03-19 07:31:14.000000 cyclicpeptide-1.0.7/cyclicpeptide/Chemical_P.csv
+-rwxr-xr-x   0 willow     (501) staff       (20)     5859 2024-05-24 07:25:18.000000 cyclicpeptide-1.0.7/cyclicpeptide/GraphAlignment.py
+-rw-r--r--   0 willow     (501) staff       (20)     2476 2024-05-31 06:42:27.000000 cyclicpeptide-1.0.7/cyclicpeptide/IOManager.py
+-rw-r--r--   0 willow     (501) staff       (20)     5380 2024-05-31 03:39:15.000000 cyclicpeptide-1.0.7/cyclicpeptide/PropertyAnalysis.py
+-rwxr-xr-x   0 willow     (501) staff       (20)     9977 2024-06-03 02:11:18.000000 cyclicpeptide-1.0.7/cyclicpeptide/Sequence2Structure.py
+-rw-r--r--   0 willow     (501) staff       (20)    10985 2024-06-03 02:09:58.000000 cyclicpeptide-1.0.7/cyclicpeptide/SequenceTransformer.py
+-rwxr-xr-x   0 willow     (501) staff       (20)    39366 2024-06-03 02:13:14.000000 cyclicpeptide-1.0.7/cyclicpeptide/Structure2Sequence.py
+-rw-r--r--   0 willow     (501) staff       (20)     2476 2024-04-08 03:27:53.000000 cyclicpeptide-1.0.7/cyclicpeptide/StructureTransformer.py
+-rw-r--r--   0 willow     (501) staff       (20)        0 2024-05-31 02:15:42.000000 cyclicpeptide-1.0.7/cyclicpeptide/__init__.py
+-rw-r--r--   0 willow     (501) staff       (20)      502 2024-03-08 01:11:36.000000 cyclicpeptide-1.0.7/cyclicpeptide/aa_smiles.txt
+-rw-r--r--   0 willow     (501) staff       (20)      116 2024-03-08 01:12:56.000000 cyclicpeptide-1.0.7/cyclicpeptide/aas.txt
+-rw-r--r--   0 willow     (501) staff       (20)    79050 2024-05-28 02:09:41.000000 cyclicpeptide-1.0.7/cyclicpeptide/monomer.tsv
+-rw-r--r--   0 willow     (501) staff       (20)      365 2024-06-03 02:15:21.000000 cyclicpeptide-1.0.7/cyclicpeptide/setting.py
+drwxr-xr-x   0 willow     (501) staff       (20)        0 2024-06-03 02:36:49.124375 cyclicpeptide-1.0.7/cyclicpeptide.egg-info/
+-rw-r--r--   0 willow     (501) staff       (20)     2569 2024-06-03 02:36:49.000000 cyclicpeptide-1.0.7/cyclicpeptide.egg-info/PKG-INFO
+-rw-r--r--   0 willow     (501) staff       (20)      648 2024-06-03 02:36:49.000000 cyclicpeptide-1.0.7/cyclicpeptide.egg-info/SOURCES.txt
+-rw-r--r--   0 willow     (501) staff       (20)        1 2024-06-03 02:36:49.000000 cyclicpeptide-1.0.7/cyclicpeptide.egg-info/dependency_links.txt
+-rw-r--r--   0 willow     (501) staff       (20)       90 2024-06-03 02:36:49.000000 cyclicpeptide-1.0.7/cyclicpeptide.egg-info/requires.txt
+-rw-r--r--   0 willow     (501) staff       (20)       14 2024-06-03 02:36:49.000000 cyclicpeptide-1.0.7/cyclicpeptide.egg-info/top_level.txt
+-rw-r--r--   0 willow     (501) staff       (20)       78 2024-06-03 02:36:49.124940 cyclicpeptide-1.0.7/setup.cfg
+-rw-r--r--   0 willow     (501) staff       (20)     1122 2024-06-03 02:36:34.000000 cyclicpeptide-1.0.7/setup.py
```

### Comparing `cyclicpeptide-1.0.6/LICENSE.md` & `cyclicpeptide-1.0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cyclicpeptide-1.0.6/PKG-INFO` & `cyclicpeptide-1.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cyclicpeptide
-Version: 1.0.6
+Version: 1.0.7
 Summary: A python package for cyclic peptides drug design
 Home-page: https://github.com/Willow0316/cyclicpeptide/tree/master
 Author: Willow
 Author-email: willow.yang.b@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: ipython>=8.12.3
-Requires-Dist: matplotlib>=3.7.5
+Requires-Dist: matplotlib==3.8
 Requires-Dist: networkx>=3.1
 Requires-Dist: numpy>=1.24.4
 Requires-Dist: pandas>=2.0.3
 Requires-Dist: rdkit>=2023.9.5
 
 # Project Name
```

### Comparing `cyclicpeptide-1.0.6/README.md` & `cyclicpeptide-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `cyclicpeptide-1.0.6/cyclicpeptide/AminoAcids.txt` & `cyclicpeptide-1.0.7/cyclicpeptide/AminoAcids.txt`

 * *Files identical despite different names*

### Comparing `cyclicpeptide-1.0.6/cyclicpeptide/Chemical_P.csv` & `cyclicpeptide-1.0.7/cyclicpeptide/Chemical_P.csv`

 * *Files identical despite different names*

### Comparing `cyclicpeptide-1.0.6/cyclicpeptide/GraphAlignment.py` & `cyclicpeptide-1.0.7/cyclicpeptide/GraphAlignment.py`

 * *Files identical despite different names*

### Comparing `cyclicpeptide-1.0.6/cyclicpeptide/IOManager.py` & `cyclicpeptide-1.0.7/cyclicpeptide/IOManager.py`

 * *Files identical despite different names*

### Comparing `cyclicpeptide-1.0.6/cyclicpeptide/PropertyAnalysis.py` & `cyclicpeptide-1.0.7/cyclicpeptide/PropertyAnalysis.py`

 * *Files identical despite different names*

### Comparing `cyclicpeptide-1.0.6/cyclicpeptide/Sequence2Structure.py` & `cyclicpeptide-1.0.7/cyclicpeptide/Sequence2Structure.py`

 * *Files identical despite different names*

### Comparing `cyclicpeptide-1.0.6/cyclicpeptide/SequenceTransformer.py` & `cyclicpeptide-1.0.7/cyclicpeptide/SequenceTransformer.py`

 * *Files identical despite different names*

### Comparing `cyclicpeptide-1.0.6/cyclicpeptide/Structure2Sequence.py` & `cyclicpeptide-1.0.7/cyclicpeptide/Structure2Sequence.py`

 * *Files identical despite different names*

### Comparing `cyclicpeptide-1.0.6/cyclicpeptide/StructureTransformer.py` & `cyclicpeptide-1.0.7/cyclicpeptide/StructureTransformer.py`

 * *Files identical despite different names*

### Comparing `cyclicpeptide-1.0.6/cyclicpeptide/monomer.tsv` & `cyclicpeptide-1.0.7/cyclicpeptide/monomer.tsv`

 * *Files identical despite different names*

### Comparing `cyclicpeptide-1.0.6/cyclicpeptide.egg-info/PKG-INFO` & `cyclicpeptide-1.0.7/cyclicpeptide.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cyclicpeptide
-Version: 1.0.6
+Version: 1.0.7
 Summary: A python package for cyclic peptides drug design
 Home-page: https://github.com/Willow0316/cyclicpeptide/tree/master
 Author: Willow
 Author-email: willow.yang.b@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: ipython>=8.12.3
-Requires-Dist: matplotlib>=3.7.5
+Requires-Dist: matplotlib==3.8
 Requires-Dist: networkx>=3.1
 Requires-Dist: numpy>=1.24.4
 Requires-Dist: pandas>=2.0.3
 Requires-Dist: rdkit>=2023.9.5
 
 # Project Name
```

### Comparing `cyclicpeptide-1.0.6/cyclicpeptide.egg-info/SOURCES.txt` & `cyclicpeptide-1.0.7/cyclicpeptide.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cyclicpeptide-1.0.6/setup.py` & `cyclicpeptide-1.0.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 setup(
     name='cyclicpeptide',
-    version='1.0.6',
+    version='1.0.7',
     packages=find_packages(),
     description='A python package for cyclic peptides drug design',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/Willow0316/cyclicpeptide/tree/master',
     author='Willow',
     author_email='willow.yang.b@gmail.com',
     python_requires='>=3.8',  # Python 版本要求
     license='MIT',
     install_requires=[
         'ipython>=8.12.3',
-        'matplotlib>=3.7.5',
+        'matplotlib==3.8',
         'networkx>=3.1',
         'numpy>=1.24.4',
         'pandas>=2.0.3',
         'rdkit>=2023.9.5',
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
```

