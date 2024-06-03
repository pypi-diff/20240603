# Comparing `tmp/cyclicpeptide-1.0.5.tar.gz` & `tmp/cyclicpeptide-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyclicpeptide-1.0.5.tar", last modified: Fri May 31 07:10:34 2024, max compression
+gzip compressed data, was "cyclicpeptide-1.0.6.tar", last modified: Mon Jun  3 02:18:01 2024, max compression
```

## Comparing `cyclicpeptide-1.0.5.tar` & `cyclicpeptide-1.0.6.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 willow     (501) staff       (20)        0 2024-05-31 07:10:34.758734 cyclicpeptide-1.0.5/
--rw-r--r--   0 willow     (501) staff       (20)     1093 2024-05-31 02:24:37.000000 cyclicpeptide-1.0.5/LICENSE.md
--rw-r--r--   0 willow     (501) staff       (20)     2571 2024-05-31 07:10:34.758672 cyclicpeptide-1.0.5/PKG-INFO
--rw-r--r--   0 willow     (501) staff       (20)     1918 2024-05-31 03:28:51.000000 cyclicpeptide-1.0.5/README.md
-drwxr-xr-x   0 willow     (501) staff       (20)        0 2024-05-31 07:10:34.757153 cyclicpeptide-1.0.5/cyclicpeptide/
--rw-r--r--   0 willow     (501) staff       (20)     1134 2024-03-07 07:35:40.000000 cyclicpeptide-1.0.5/cyclicpeptide/AminoAcids.txt
--rw-r--r--   0 willow     (501) staff       (20)     1662 2024-03-19 07:31:14.000000 cyclicpeptide-1.0.5/cyclicpeptide/Chemical_P.csv
--rwxr-xr-x   0 willow     (501) staff       (20)     5859 2024-05-24 07:25:18.000000 cyclicpeptide-1.0.5/cyclicpeptide/GraphAlignment.py
--rw-r--r--   0 willow     (501) staff       (20)     2476 2024-05-31 06:42:27.000000 cyclicpeptide-1.0.5/cyclicpeptide/IOManager.py
--rw-r--r--   0 willow     (501) staff       (20)     5380 2024-05-31 03:39:15.000000 cyclicpeptide-1.0.5/cyclicpeptide/PropertyAnalysis.py
--rwxr-xr-x   0 willow     (501) staff       (20)     9972 2024-05-31 06:52:09.000000 cyclicpeptide-1.0.5/cyclicpeptide/Sequence2Structure.py
--rw-r--r--   0 willow     (501) staff       (20)    11017 2024-05-13 03:22:59.000000 cyclicpeptide-1.0.5/cyclicpeptide/SequenceTransformer.py
--rwxr-xr-x   0 willow     (501) staff       (20)    39615 2024-05-31 07:06:18.000000 cyclicpeptide-1.0.5/cyclicpeptide/Structure2Sequence.py
--rw-r--r--   0 willow     (501) staff       (20)     2476 2024-04-08 03:27:53.000000 cyclicpeptide-1.0.5/cyclicpeptide/StructureTransformer.py
--rw-r--r--   0 willow     (501) staff       (20)        0 2024-05-31 02:15:42.000000 cyclicpeptide-1.0.5/cyclicpeptide/__init__.py
--rw-r--r--   0 willow     (501) staff       (20)      502 2024-03-08 01:11:36.000000 cyclicpeptide-1.0.5/cyclicpeptide/aa_smiles.txt
--rw-r--r--   0 willow     (501) staff       (20)      116 2024-03-08 01:12:56.000000 cyclicpeptide-1.0.5/cyclicpeptide/aas.txt
--rw-r--r--   0 willow     (501) staff       (20)    79050 2024-05-28 02:09:41.000000 cyclicpeptide-1.0.5/cyclicpeptide/monomer.tsv
-drwxr-xr-x   0 willow     (501) staff       (20)        0 2024-05-31 07:10:34.758420 cyclicpeptide-1.0.5/cyclicpeptide.egg-info/
--rw-r--r--   0 willow     (501) staff       (20)     2571 2024-05-31 07:10:34.000000 cyclicpeptide-1.0.5/cyclicpeptide.egg-info/PKG-INFO
--rw-r--r--   0 willow     (501) staff       (20)      623 2024-05-31 07:10:34.000000 cyclicpeptide-1.0.5/cyclicpeptide.egg-info/SOURCES.txt
--rw-r--r--   0 willow     (501) staff       (20)        1 2024-05-31 07:10:34.000000 cyclicpeptide-1.0.5/cyclicpeptide.egg-info/dependency_links.txt
--rw-r--r--   0 willow     (501) staff       (20)       92 2024-05-31 07:10:34.000000 cyclicpeptide-1.0.5/cyclicpeptide.egg-info/requires.txt
--rw-r--r--   0 willow     (501) staff       (20)       14 2024-05-31 07:10:34.000000 cyclicpeptide-1.0.5/cyclicpeptide.egg-info/top_level.txt
--rw-r--r--   0 willow     (501) staff       (20)       78 2024-05-31 07:10:34.758973 cyclicpeptide-1.0.5/setup.cfg
--rw-r--r--   0 willow     (501) staff       (20)     1124 2024-05-31 07:06:38.000000 cyclicpeptide-1.0.5/setup.py
+drwxr-xr-x   0 willow     (501) staff       (20)        0 2024-06-03 02:18:01.779192 cyclicpeptide-1.0.6/
+-rw-r--r--   0 willow     (501) staff       (20)     1093 2024-05-31 02:24:37.000000 cyclicpeptide-1.0.6/LICENSE.md
+-rw-r--r--   0 willow     (501) staff       (20)     2571 2024-06-03 02:18:01.779129 cyclicpeptide-1.0.6/PKG-INFO
+-rw-r--r--   0 willow     (501) staff       (20)     1918 2024-05-31 03:28:51.000000 cyclicpeptide-1.0.6/README.md
+drwxr-xr-x   0 willow     (501) staff       (20)        0 2024-06-03 02:18:01.777878 cyclicpeptide-1.0.6/cyclicpeptide/
+-rw-r--r--   0 willow     (501) staff       (20)     1134 2024-03-07 07:35:40.000000 cyclicpeptide-1.0.6/cyclicpeptide/AminoAcids.txt
+-rw-r--r--   0 willow     (501) staff       (20)     1662 2024-03-19 07:31:14.000000 cyclicpeptide-1.0.6/cyclicpeptide/Chemical_P.csv
+-rwxr-xr-x   0 willow     (501) staff       (20)     5859 2024-05-24 07:25:18.000000 cyclicpeptide-1.0.6/cyclicpeptide/GraphAlignment.py
+-rw-r--r--   0 willow     (501) staff       (20)     2476 2024-05-31 06:42:27.000000 cyclicpeptide-1.0.6/cyclicpeptide/IOManager.py
+-rw-r--r--   0 willow     (501) staff       (20)     5380 2024-05-31 03:39:15.000000 cyclicpeptide-1.0.6/cyclicpeptide/PropertyAnalysis.py
+-rwxr-xr-x   0 willow     (501) staff       (20)     9977 2024-06-03 02:11:18.000000 cyclicpeptide-1.0.6/cyclicpeptide/Sequence2Structure.py
+-rw-r--r--   0 willow     (501) staff       (20)    10985 2024-06-03 02:09:58.000000 cyclicpeptide-1.0.6/cyclicpeptide/SequenceTransformer.py
+-rwxr-xr-x   0 willow     (501) staff       (20)    39366 2024-06-03 02:13:14.000000 cyclicpeptide-1.0.6/cyclicpeptide/Structure2Sequence.py
+-rw-r--r--   0 willow     (501) staff       (20)     2476 2024-04-08 03:27:53.000000 cyclicpeptide-1.0.6/cyclicpeptide/StructureTransformer.py
+-rw-r--r--   0 willow     (501) staff       (20)        0 2024-05-31 02:15:42.000000 cyclicpeptide-1.0.6/cyclicpeptide/__init__.py
+-rw-r--r--   0 willow     (501) staff       (20)      502 2024-03-08 01:11:36.000000 cyclicpeptide-1.0.6/cyclicpeptide/aa_smiles.txt
+-rw-r--r--   0 willow     (501) staff       (20)      116 2024-03-08 01:12:56.000000 cyclicpeptide-1.0.6/cyclicpeptide/aas.txt
+-rw-r--r--   0 willow     (501) staff       (20)    79050 2024-05-28 02:09:41.000000 cyclicpeptide-1.0.6/cyclicpeptide/monomer.tsv
+-rw-r--r--   0 willow     (501) staff       (20)      365 2024-06-03 02:15:21.000000 cyclicpeptide-1.0.6/cyclicpeptide/setting.py
+drwxr-xr-x   0 willow     (501) staff       (20)        0 2024-06-03 02:18:01.778809 cyclicpeptide-1.0.6/cyclicpeptide.egg-info/
+-rw-r--r--   0 willow     (501) staff       (20)     2571 2024-06-03 02:18:01.000000 cyclicpeptide-1.0.6/cyclicpeptide.egg-info/PKG-INFO
+-rw-r--r--   0 willow     (501) staff       (20)      648 2024-06-03 02:18:01.000000 cyclicpeptide-1.0.6/cyclicpeptide.egg-info/SOURCES.txt
+-rw-r--r--   0 willow     (501) staff       (20)        1 2024-06-03 02:18:01.000000 cyclicpeptide-1.0.6/cyclicpeptide.egg-info/dependency_links.txt
+-rw-r--r--   0 willow     (501) staff       (20)       92 2024-06-03 02:18:01.000000 cyclicpeptide-1.0.6/cyclicpeptide.egg-info/requires.txt
+-rw-r--r--   0 willow     (501) staff       (20)       14 2024-06-03 02:18:01.000000 cyclicpeptide-1.0.6/cyclicpeptide.egg-info/top_level.txt
+-rw-r--r--   0 willow     (501) staff       (20)       78 2024-06-03 02:18:01.779571 cyclicpeptide-1.0.6/setup.cfg
+-rw-r--r--   0 willow     (501) staff       (20)     1124 2024-06-03 02:17:39.000000 cyclicpeptide-1.0.6/setup.py
```

### Comparing `cyclicpeptide-1.0.5/LICENSE.md` & `cyclicpeptide-1.0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cyclicpeptide-1.0.5/PKG-INFO` & `cyclicpeptide-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyclicpeptide
-Version: 1.0.5
+Version: 1.0.6
 Summary: A python package for cyclic peptides drug design
 Home-page: https://github.com/Willow0316/cyclicpeptide/tree/master
 Author: Willow
 Author-email: willow.yang.b@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `cyclicpeptide-1.0.5/README.md` & `cyclicpeptide-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `cyclicpeptide-1.0.5/cyclicpeptide/AminoAcids.txt` & `cyclicpeptide-1.0.6/cyclicpeptide/AminoAcids.txt`

 * *Files identical despite different names*

### Comparing `cyclicpeptide-1.0.5/cyclicpeptide/Chemical_P.csv` & `cyclicpeptide-1.0.6/cyclicpeptide/Chemical_P.csv`

 * *Files identical despite different names*

### Comparing `cyclicpeptide-1.0.5/cyclicpeptide/GraphAlignment.py` & `cyclicpeptide-1.0.6/cyclicpeptide/GraphAlignment.py`

 * *Files identical despite different names*

### Comparing `cyclicpeptide-1.0.5/cyclicpeptide/IOManager.py` & `cyclicpeptide-1.0.6/cyclicpeptide/IOManager.py`

 * *Files identical despite different names*

### Comparing `cyclicpeptide-1.0.5/cyclicpeptide/PropertyAnalysis.py` & `cyclicpeptide-1.0.6/cyclicpeptide/PropertyAnalysis.py`

 * *Files identical despite different names*

### Comparing `cyclicpeptide-1.0.5/cyclicpeptide/Sequence2Structure.py` & `cyclicpeptide-1.0.6/cyclicpeptide/Sequence2Structure.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 """
 
 import pandas as pd
 from IPython.display import SVG, display
 from rdkit import Chem
 from rdkit.Chem.Draw import rdMolDraw2D
 import re
+from setting import *
 
 def transfrom(seequence, references, cyclic=True):#没写完
     Essential_AA = {'Ala', 'Arg', 'Asn', 'Asp', 'Cys', 'Glu', 'Gln', 'Gly', 'His', 'Ile', 'Leu', 'Lys',
     'Met', 'Phe', 'Pro', 'Trp', 'Tyr', 'Val', 'Ser', 'Thr'}
 
 def seq2stru_essentialAA(sequence, cyclic=True):
 
@@ -120,15 +121,15 @@
     :param code: sequence.
     :type code: amino acid chain format
     :return: One letter code
 
     """
 
     # 打开文本文件并读取内容
-    file_path = 'AminoAcids.txt'  # 替换为你的文件路径
+    file_path = AminoAcids_path  # 替换为你的文件路径
     AminoAcids = []
     with open(file_path, 'r', encoding='utf-8') as file:
         """Reads the contents of the file line by line and adds it to the list"""
         for line in file:
             """# 去除行尾的换行符，并将参数添加到列表中"""
             AminoAcids.append(eval(line.strip()))
     c2s = {i[1]: [i[0], i[2]] for i in AminoAcids}
@@ -201,15 +202,15 @@
         backbone, backbone_idx = detect_backbone(mol)
         c_index = backbone[0]
         n_index = backbone[-1]
         mol = link_aa_by_peptide_bond(mol, c_index, n_index)
     return mol
 
 
-def reference_aa_monomer(monomers_path=r'cyclicpeptide/monomer.tsv'): #未修改
+def reference_aa_monomer(monomers_path=monomer_path): #未修改
     """
 
     :param monomers_path: sequence of essential AA.
     :type sequence: One letter code
     :param cyclic: Optional "cyclic".
     :type cyclic: True or False
     :return: mol
```

### Comparing `cyclicpeptide-1.0.5/cyclicpeptide/SequenceTransformer.py` & `cyclicpeptide-1.0.6/cyclicpeptide/SequenceTransformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import re
+from setting import *
 
 # 打开文本文件并读取内容
-file_path = r'/Users/willow/Desktop/CP_tool-PyPI/src/cyclicpeptide/AminoAcids.txt'  # 替换为你的文件路径
+file_path = AminoAcids_path  # 替换为你的文件路径
 AminoAcids = []
 with open(file_path, 'r', encoding='utf-8') as file:
     # 逐行读取文件内容并添加到列表中
     for line in file:
         # 去除行尾的换行符，并将参数添加到列表中
         AminoAcids.append(eval(line.strip()))
```

### Comparing `cyclicpeptide-1.0.5/cyclicpeptide/Structure2Sequence.py` & `cyclicpeptide-1.0.6/cyclicpeptide/Structure2Sequence.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from IPython.display import SVG, display
 from rdkit import Chem
 from rdkit.Chem.Draw import rdMolDraw2D
 import pkg_resources
+from setting import *
 from rdkit.Chem.rdchem import RWMol, AtomPDBResidueInfo
 
 def mol2seq_for_essentialAA(m):
     """
     **Using the RDKit function "Chem.MolToSequence" conversion**
 
     * Can convert peptide sequences with essential amino acids;
@@ -42,21 +43,22 @@
         m = Chem.MolFromSmiles(smiles)
         m_renum, seq = struc2seq.mol2seq_for_essentialAA(m)
         print('SEQ:', seq)
 
     SEQ: IRHTCCVGVCFLMACICIEQFDPCEM
     """
     aa_smiles = {}
-    file_path1 = r'/Users/willow/Desktop/CP_tool-PyPI/src/cyclicpeptide/aa_smiles.txt'  # 替换为你的文件路径
+    file_path1 = aa_smiles_path  # 替换为你的文件路径
+    print(file_path1)
     with open(file_path1, 'r') as file:
         for line in file:
             if line.strip():  # 跳过空行
                 aa, smile = line.strip().split(':')
                 aa_smiles[aa.strip()] = smile.strip()
-    file_path2 = r'/Users/willow/Desktop/CP_tool-PyPI/src/cyclicpeptide/aas.txt'  # 替换为你的文件路径
+    file_path2 = aas_path  # 替换为你的文件路径
     with open(file_path2, 'r') as file:
         aas = [line.strip() for line in file if line.strip()]
         # order important because gly is substructure of other aas
     # detect the atoms of the backbone and assign them with info
     CAatoms = m.GetSubstructMatches(Chem.MolFromSmarts("[C:0](=[O:1])[C:2][N:3]"))
     # print(CAatoms)
     for atoms in CAatoms:
@@ -281,15 +283,15 @@
                     # new_mol.AddBond(atom_mapping[inner_idx], new_idx, bond.GetBondType())
         new_mol = new_mol.GetMol()
         Chem.SanitizeMol(new_mol)
         aas.append(new_mol)
     return aas, atom_mappings
 
 
-def reference_aa_monomer(monomers_path='monomer.tsv'):
+def reference_aa_monomer(monomers_path=monomer_path):
     """
     Identify amino acids based on the monomer reference library
 
     * Identify the type of each amino acid unit;
     * If it can be directly recognized by 20 essential amino acids, then the amino acid can be directly determined;
     * If it cannot be directly recognized by essential amino acids, use library to find the maximum matching reference unit;
     * For cross amino acid units, select the two reference units with the most matching atoms and no cross;
@@ -298,21 +300,16 @@
 
     :param monomers_path: The "monomers_path" to the monomer library file.
     :type monomers_path: **tsv**
     :return: essential = {'code': [aa, symbol, num_atoms]}, others = {'code': [aa, symbol, num_atoms]}, 
     :rtype: dict[str, list[str]], dict[str, list[str]]
 
     """
-    if monomers_path:
-        monomers = pd.read_csv(monomers_path, sep='\t', index_col=0)
+    monomers = pd.read_csv(monomers_path, sep='\t', index_col=0)
 
-    else:
-        file_path = pkg_resources.resource_filename('monomer.tsv')
-        with open(file_path, 'r') as file:
-            monomers = file.read()
     essentials = {}
     others = {}
     temp = monomers.loc[monomers['Essential amino acids'] == 1, :]
     for i in temp.index:
         smile = temp.loc[i, 'Smiles']
         code = temp.loc[i, 'Code']
         weight = float(temp.loc[i, 'Weight'])
@@ -584,15 +581,15 @@
             display(SVG(svg_data))
         return svg_data
     else:
         print('Image failed to draw!')
         return ''
 
 
-def transform(smiles, monomers_path='monomer.tsv'):
+def transform(smiles, monomers_path=monomer_path):
     """
     Transform and report generation through an integrated function.
     
     Example::
 
         from IPython.display import HTML
```

### Comparing `cyclicpeptide-1.0.5/cyclicpeptide/StructureTransformer.py` & `cyclicpeptide-1.0.6/cyclicpeptide/StructureTransformer.py`

 * *Files identical despite different names*

### Comparing `cyclicpeptide-1.0.5/cyclicpeptide/monomer.tsv` & `cyclicpeptide-1.0.6/cyclicpeptide/monomer.tsv`

 * *Files identical despite different names*

### Comparing `cyclicpeptide-1.0.5/cyclicpeptide.egg-info/PKG-INFO` & `cyclicpeptide-1.0.6/cyclicpeptide.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyclicpeptide
-Version: 1.0.5
+Version: 1.0.6
 Summary: A python package for cyclic peptides drug design
 Home-page: https://github.com/Willow0316/cyclicpeptide/tree/master
 Author: Willow
 Author-email: willow.yang.b@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `cyclicpeptide-1.0.5/cyclicpeptide.egg-info/SOURCES.txt` & `cyclicpeptide-1.0.6/cyclicpeptide.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -11,12 +11,13 @@
 cyclicpeptide/SequenceTransformer.py
 cyclicpeptide/Structure2Sequence.py
 cyclicpeptide/StructureTransformer.py
 cyclicpeptide/__init__.py
 cyclicpeptide/aa_smiles.txt
 cyclicpeptide/aas.txt
 cyclicpeptide/monomer.tsv
+cyclicpeptide/setting.py
 cyclicpeptide.egg-info/PKG-INFO
 cyclicpeptide.egg-info/SOURCES.txt
 cyclicpeptide.egg-info/dependency_links.txt
 cyclicpeptide.egg-info/requires.txt
 cyclicpeptide.egg-info/top_level.txt
```

### Comparing `cyclicpeptide-1.0.5/setup.py` & `cyclicpeptide-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 setup(
     name='cyclicpeptide',
-    version='1.0.5',
+    version='1.0.6',
     packages=find_packages(),
     description='A python package for cyclic peptides drug design',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/Willow0316/cyclicpeptide/tree/master',
     author='Willow',
     author_email='willow.yang.b@gmail.com',
```

