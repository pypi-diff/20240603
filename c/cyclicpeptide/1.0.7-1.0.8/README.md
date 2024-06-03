# Comparing `tmp/cyclicpeptide-1.0.7.tar.gz` & `tmp/cyclicpeptide-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyclicpeptide-1.0.7.tar", last modified: Mon Jun  3 02:36:49 2024, max compression
+gzip compressed data, was "cyclicpeptide-1.0.8.tar", last modified: Mon Jun  3 02:45:03 2024, max compression
```

## Comparing `cyclicpeptide-1.0.7.tar` & `cyclicpeptide-1.0.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 willow     (501) staff       (20)        0 2024-06-03 02:36:49.124698 cyclicpeptide-1.0.7/
--rw-r--r--   0 willow     (501) staff       (20)     1093 2024-05-31 02:24:37.000000 cyclicpeptide-1.0.7/LICENSE.md
--rw-r--r--   0 willow     (501) staff       (20)     2569 2024-06-03 02:36:49.124635 cyclicpeptide-1.0.7/PKG-INFO
--rw-r--r--   0 willow     (501) staff       (20)     1918 2024-05-31 03:28:51.000000 cyclicpeptide-1.0.7/README.md
-drwxr-xr-x   0 willow     (501) staff       (20)        0 2024-06-03 02:36:49.123345 cyclicpeptide-1.0.7/cyclicpeptide/
--rw-r--r--   0 willow     (501) staff       (20)     1134 2024-03-07 07:35:40.000000 cyclicpeptide-1.0.7/cyclicpeptide/AminoAcids.txt
--rw-r--r--   0 willow     (501) staff       (20)     1662 2024-03-19 07:31:14.000000 cyclicpeptide-1.0.7/cyclicpeptide/Chemical_P.csv
--rwxr-xr-x   0 willow     (501) staff       (20)     5859 2024-05-24 07:25:18.000000 cyclicpeptide-1.0.7/cyclicpeptide/GraphAlignment.py
--rw-r--r--   0 willow     (501) staff       (20)     2476 2024-05-31 06:42:27.000000 cyclicpeptide-1.0.7/cyclicpeptide/IOManager.py
--rw-r--r--   0 willow     (501) staff       (20)     5380 2024-05-31 03:39:15.000000 cyclicpeptide-1.0.7/cyclicpeptide/PropertyAnalysis.py
--rwxr-xr-x   0 willow     (501) staff       (20)     9977 2024-06-03 02:11:18.000000 cyclicpeptide-1.0.7/cyclicpeptide/Sequence2Structure.py
--rw-r--r--   0 willow     (501) staff       (20)    10985 2024-06-03 02:09:58.000000 cyclicpeptide-1.0.7/cyclicpeptide/SequenceTransformer.py
--rwxr-xr-x   0 willow     (501) staff       (20)    39366 2024-06-03 02:13:14.000000 cyclicpeptide-1.0.7/cyclicpeptide/Structure2Sequence.py
--rw-r--r--   0 willow     (501) staff       (20)     2476 2024-04-08 03:27:53.000000 cyclicpeptide-1.0.7/cyclicpeptide/StructureTransformer.py
--rw-r--r--   0 willow     (501) staff       (20)        0 2024-05-31 02:15:42.000000 cyclicpeptide-1.0.7/cyclicpeptide/__init__.py
--rw-r--r--   0 willow     (501) staff       (20)      502 2024-03-08 01:11:36.000000 cyclicpeptide-1.0.7/cyclicpeptide/aa_smiles.txt
--rw-r--r--   0 willow     (501) staff       (20)      116 2024-03-08 01:12:56.000000 cyclicpeptide-1.0.7/cyclicpeptide/aas.txt
--rw-r--r--   0 willow     (501) staff       (20)    79050 2024-05-28 02:09:41.000000 cyclicpeptide-1.0.7/cyclicpeptide/monomer.tsv
--rw-r--r--   0 willow     (501) staff       (20)      365 2024-06-03 02:15:21.000000 cyclicpeptide-1.0.7/cyclicpeptide/setting.py
-drwxr-xr-x   0 willow     (501) staff       (20)        0 2024-06-03 02:36:49.124375 cyclicpeptide-1.0.7/cyclicpeptide.egg-info/
--rw-r--r--   0 willow     (501) staff       (20)     2569 2024-06-03 02:36:49.000000 cyclicpeptide-1.0.7/cyclicpeptide.egg-info/PKG-INFO
--rw-r--r--   0 willow     (501) staff       (20)      648 2024-06-03 02:36:49.000000 cyclicpeptide-1.0.7/cyclicpeptide.egg-info/SOURCES.txt
--rw-r--r--   0 willow     (501) staff       (20)        1 2024-06-03 02:36:49.000000 cyclicpeptide-1.0.7/cyclicpeptide.egg-info/dependency_links.txt
--rw-r--r--   0 willow     (501) staff       (20)       90 2024-06-03 02:36:49.000000 cyclicpeptide-1.0.7/cyclicpeptide.egg-info/requires.txt
--rw-r--r--   0 willow     (501) staff       (20)       14 2024-06-03 02:36:49.000000 cyclicpeptide-1.0.7/cyclicpeptide.egg-info/top_level.txt
--rw-r--r--   0 willow     (501) staff       (20)       78 2024-06-03 02:36:49.124940 cyclicpeptide-1.0.7/setup.cfg
--rw-r--r--   0 willow     (501) staff       (20)     1122 2024-06-03 02:36:34.000000 cyclicpeptide-1.0.7/setup.py
+drwxr-xr-x   0 willow     (501) staff       (20)        0 2024-06-03 02:45:03.233660 cyclicpeptide-1.0.8/
+-rw-r--r--   0 willow     (501) staff       (20)     1093 2024-05-31 02:24:37.000000 cyclicpeptide-1.0.8/LICENSE.md
+-rw-r--r--   0 willow     (501) staff       (20)     2569 2024-06-03 02:45:03.233602 cyclicpeptide-1.0.8/PKG-INFO
+-rw-r--r--   0 willow     (501) staff       (20)     1918 2024-05-31 03:28:51.000000 cyclicpeptide-1.0.8/README.md
+drwxr-xr-x   0 willow     (501) staff       (20)        0 2024-06-03 02:45:03.232271 cyclicpeptide-1.0.8/cyclicpeptide/
+-rw-r--r--   0 willow     (501) staff       (20)     1134 2024-03-07 07:35:40.000000 cyclicpeptide-1.0.8/cyclicpeptide/AminoAcids.txt
+-rw-r--r--   0 willow     (501) staff       (20)     1662 2024-03-19 07:31:14.000000 cyclicpeptide-1.0.8/cyclicpeptide/Chemical_P.csv
+-rwxr-xr-x   0 willow     (501) staff       (20)     5859 2024-06-03 02:44:10.000000 cyclicpeptide-1.0.8/cyclicpeptide/GraphAlignment.py
+-rw-r--r--   0 willow     (501) staff       (20)     2476 2024-05-31 06:42:27.000000 cyclicpeptide-1.0.8/cyclicpeptide/IOManager.py
+-rw-r--r--   0 willow     (501) staff       (20)     5380 2024-05-31 03:39:15.000000 cyclicpeptide-1.0.8/cyclicpeptide/PropertyAnalysis.py
+-rwxr-xr-x   0 willow     (501) staff       (20)     9978 2024-06-03 02:44:02.000000 cyclicpeptide-1.0.8/cyclicpeptide/Sequence2Structure.py
+-rw-r--r--   0 willow     (501) staff       (20)    10986 2024-06-03 02:43:57.000000 cyclicpeptide-1.0.8/cyclicpeptide/SequenceTransformer.py
+-rwxr-xr-x   0 willow     (501) staff       (20)    39367 2024-06-03 02:43:44.000000 cyclicpeptide-1.0.8/cyclicpeptide/Structure2Sequence.py
+-rw-r--r--   0 willow     (501) staff       (20)     2476 2024-04-08 03:27:53.000000 cyclicpeptide-1.0.8/cyclicpeptide/StructureTransformer.py
+-rw-r--r--   0 willow     (501) staff       (20)        0 2024-05-31 02:15:42.000000 cyclicpeptide-1.0.8/cyclicpeptide/__init__.py
+-rw-r--r--   0 willow     (501) staff       (20)      502 2024-03-08 01:11:36.000000 cyclicpeptide-1.0.8/cyclicpeptide/aa_smiles.txt
+-rw-r--r--   0 willow     (501) staff       (20)      116 2024-03-08 01:12:56.000000 cyclicpeptide-1.0.8/cyclicpeptide/aas.txt
+-rw-r--r--   0 willow     (501) staff       (20)    79050 2024-05-28 02:09:41.000000 cyclicpeptide-1.0.8/cyclicpeptide/monomer.tsv
+-rw-r--r--   0 willow     (501) staff       (20)      365 2024-06-03 02:15:21.000000 cyclicpeptide-1.0.8/cyclicpeptide/setting.py
+drwxr-xr-x   0 willow     (501) staff       (20)        0 2024-06-03 02:45:03.233352 cyclicpeptide-1.0.8/cyclicpeptide.egg-info/
+-rw-r--r--   0 willow     (501) staff       (20)     2569 2024-06-03 02:45:03.000000 cyclicpeptide-1.0.8/cyclicpeptide.egg-info/PKG-INFO
+-rw-r--r--   0 willow     (501) staff       (20)      648 2024-06-03 02:45:03.000000 cyclicpeptide-1.0.8/cyclicpeptide.egg-info/SOURCES.txt
+-rw-r--r--   0 willow     (501) staff       (20)        1 2024-06-03 02:45:03.000000 cyclicpeptide-1.0.8/cyclicpeptide.egg-info/dependency_links.txt
+-rw-r--r--   0 willow     (501) staff       (20)       90 2024-06-03 02:45:03.000000 cyclicpeptide-1.0.8/cyclicpeptide.egg-info/requires.txt
+-rw-r--r--   0 willow     (501) staff       (20)       14 2024-06-03 02:45:03.000000 cyclicpeptide-1.0.8/cyclicpeptide.egg-info/top_level.txt
+-rw-r--r--   0 willow     (501) staff       (20)       78 2024-06-03 02:45:03.233877 cyclicpeptide-1.0.8/setup.cfg
+-rw-r--r--   0 willow     (501) staff       (20)     1122 2024-06-03 02:44:59.000000 cyclicpeptide-1.0.8/setup.py
```

### Comparing `cyclicpeptide-1.0.7/LICENSE.md` & `cyclicpeptide-1.0.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cyclicpeptide-1.0.7/PKG-INFO` & `cyclicpeptide-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyclicpeptide
-Version: 1.0.7
+Version: 1.0.8
 Summary: A python package for cyclic peptides drug design
 Home-page: https://github.com/Willow0316/cyclicpeptide/tree/master
 Author: Willow
 Author-email: willow.yang.b@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `cyclicpeptide-1.0.7/README.md` & `cyclicpeptide-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `cyclicpeptide-1.0.7/cyclicpeptide/AminoAcids.txt` & `cyclicpeptide-1.0.8/cyclicpeptide/AminoAcids.txt`

 * *Files identical despite different names*

### Comparing `cyclicpeptide-1.0.7/cyclicpeptide/Chemical_P.csv` & `cyclicpeptide-1.0.8/cyclicpeptide/Chemical_P.csv`

 * *Files identical despite different names*

### Comparing `cyclicpeptide-1.0.7/cyclicpeptide/GraphAlignment.py` & `cyclicpeptide-1.0.8/cyclicpeptide/GraphAlignment.py`

 * *Files identical despite different names*

### Comparing `cyclicpeptide-1.0.7/cyclicpeptide/IOManager.py` & `cyclicpeptide-1.0.8/cyclicpeptide/IOManager.py`

 * *Files identical despite different names*

### Comparing `cyclicpeptide-1.0.7/cyclicpeptide/PropertyAnalysis.py` & `cyclicpeptide-1.0.8/cyclicpeptide/PropertyAnalysis.py`

 * *Files identical despite different names*

### Comparing `cyclicpeptide-1.0.7/cyclicpeptide/Sequence2Structure.py` & `cyclicpeptide-1.0.8/cyclicpeptide/Sequence2Structure.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 """
 
 import pandas as pd
 from IPython.display import SVG, display
 from rdkit import Chem
 from rdkit.Chem.Draw import rdMolDraw2D
 import re
-from setting import *
+from .setting import *
 
 def transfrom(seequence, references, cyclic=True):#没写完
     Essential_AA = {'Ala', 'Arg', 'Asn', 'Asp', 'Cys', 'Glu', 'Gln', 'Gly', 'His', 'Ile', 'Leu', 'Lys',
     'Met', 'Phe', 'Pro', 'Trp', 'Tyr', 'Val', 'Ser', 'Thr'}
 
 def seq2stru_essentialAA(sequence, cyclic=True):
```

### Comparing `cyclicpeptide-1.0.7/cyclicpeptide/SequenceTransformer.py` & `cyclicpeptide-1.0.8/cyclicpeptide/SequenceTransformer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import re
-from setting import *
+from .setting import *
 
 # 打开文本文件并读取内容
 file_path = AminoAcids_path  # 替换为你的文件路径
 AminoAcids = []
 with open(file_path, 'r', encoding='utf-8') as file:
     # 逐行读取文件内容并添加到列表中
     for line in file:
```

### Comparing `cyclicpeptide-1.0.7/cyclicpeptide/Structure2Sequence.py` & `cyclicpeptide-1.0.8/cyclicpeptide/Structure2Sequence.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from IPython.display import SVG, display
 from rdkit import Chem
 from rdkit.Chem.Draw import rdMolDraw2D
 import pkg_resources
-from setting import *
+from .setting import *
 from rdkit.Chem.rdchem import RWMol, AtomPDBResidueInfo
 
 def mol2seq_for_essentialAA(m):
     """
     **Using the RDKit function "Chem.MolToSequence" conversion**
 
     * Can convert peptide sequences with essential amino acids;
```

### Comparing `cyclicpeptide-1.0.7/cyclicpeptide/StructureTransformer.py` & `cyclicpeptide-1.0.8/cyclicpeptide/StructureTransformer.py`

 * *Files identical despite different names*

### Comparing `cyclicpeptide-1.0.7/cyclicpeptide/monomer.tsv` & `cyclicpeptide-1.0.8/cyclicpeptide/monomer.tsv`

 * *Files identical despite different names*

### Comparing `cyclicpeptide-1.0.7/cyclicpeptide.egg-info/PKG-INFO` & `cyclicpeptide-1.0.8/cyclicpeptide.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyclicpeptide
-Version: 1.0.7
+Version: 1.0.8
 Summary: A python package for cyclic peptides drug design
 Home-page: https://github.com/Willow0316/cyclicpeptide/tree/master
 Author: Willow
 Author-email: willow.yang.b@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `cyclicpeptide-1.0.7/cyclicpeptide.egg-info/SOURCES.txt` & `cyclicpeptide-1.0.8/cyclicpeptide.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cyclicpeptide-1.0.7/setup.py` & `cyclicpeptide-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 setup(
     name='cyclicpeptide',
-    version='1.0.7',
+    version='1.0.8',
     packages=find_packages(),
     description='A python package for cyclic peptides drug design',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/Willow0316/cyclicpeptide/tree/master',
     author='Willow',
     author_email='willow.yang.b@gmail.com',
```

