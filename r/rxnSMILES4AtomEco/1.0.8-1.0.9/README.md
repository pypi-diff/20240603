# Comparing `tmp/rxnSMILES4AtomEco-1.0.8.tar.gz` & `tmp/rxnSMILES4AtomEco-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rxnSMILES4AtomEco-1.0.8.tar", last modified: Sat Jun  1 22:26:23 2024, max compression
+gzip compressed data, was "rxnSMILES4AtomEco-1.0.9.tar", last modified: Mon Jun  3 08:09:08 2024, max compression
```

## Comparing `rxnSMILES4AtomEco-1.0.8.tar` & `rxnSMILES4AtomEco-1.0.9.tar`

### file list

```diff
@@ -1,14 +1,9 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 22:26:23.876105 rxnSMILES4AtomEco-1.0.8/
--rw-rw-rw-   0        0        0      633 2024-05-17 18:38:51.000000 rxnSMILES4AtomEco-1.0.8/LICENSE
--rw-rw-rw-   0        0        0     1277 2024-06-01 22:26:23.866097 rxnSMILES4AtomEco-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     7108 2024-05-28 07:21:33.000000 rxnSMILES4AtomEco-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-06-01 22:26:23.820102 rxnSMILES4AtomEco-1.0.8/rxn4SMILESAtomEco/
--rw-rw-rw-   0        0        0       96 2024-06-01 22:13:07.000000 rxnSMILES4AtomEco-1.0.8/rxn4SMILESAtomEco/__init__.py
--rw-rw-rw-   0        0        0     4285 2024-06-01 21:47:38.000000 rxnSMILES4AtomEco-1.0.8/rxn4SMILESAtomEco/rxnSMILES4AtomEco.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:26:23.860101 rxnSMILES4AtomEco-1.0.8/rxnSMILES4AtomEco.egg-info/
--rw-rw-rw-   0        0        0     1277 2024-06-01 22:26:23.000000 rxnSMILES4AtomEco-1.0.8/rxnSMILES4AtomEco.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2024-06-01 22:26:23.000000 rxnSMILES4AtomEco-1.0.8/rxnSMILES4AtomEco.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 22:26:23.000000 rxnSMILES4AtomEco-1.0.8/rxnSMILES4AtomEco.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-06-01 22:26:23.000000 rxnSMILES4AtomEco-1.0.8/rxnSMILES4AtomEco.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-06-01 22:26:23.878100 rxnSMILES4AtomEco-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1407 2024-06-01 22:25:26.000000 rxnSMILES4AtomEco-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:09:08.697579 rxnSMILES4AtomEco-1.0.9/
+-rw-rw-rw-   0        0        0     1248 2024-06-03 08:09:08.695578 rxnSMILES4AtomEco-1.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-06-03 08:09:08.693579 rxnSMILES4AtomEco-1.0.9/rxnSMILES4AtomEco.egg-info/
+-rw-rw-rw-   0        0        0     1248 2024-06-03 08:09:08.000000 rxnSMILES4AtomEco-1.0.9/rxnSMILES4AtomEco.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2024-06-03 08:09:08.000000 rxnSMILES4AtomEco-1.0.9/rxnSMILES4AtomEco.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 08:09:08.000000 rxnSMILES4AtomEco-1.0.9/rxnSMILES4AtomEco.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 08:09:08.000000 rxnSMILES4AtomEco-1.0.9/rxnSMILES4AtomEco.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-03 08:09:08.698581 rxnSMILES4AtomEco-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1401 2024-06-03 08:06:33.000000 rxnSMILES4AtomEco-1.0.9/setup.py
```

### Comparing `rxnSMILES4AtomEco-1.0.8/PKG-INFO` & `rxnSMILES4AtomEco-1.0.9/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,15 @@
-Metadata-Version: 2.1
-Name: rxnSMILES4AtomEco
-Version: 1.0.8
-Summary: Calculate atom economy for chemical reactions using reaction SMILES
-Home-page: https://github.com/yourusername/rxnSMILES4AtomEco
-Author: Samuele Giani
-Author-email: samuele.giani@empa.ch
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-License-File: LICENSE
+from setuptools import setup, find_packages
 
+setup(
+    name='rxnSMILES4AtomEco',
+    version='1.0.9',
+    packages=find_packages(),
+    description='Calculate atom economy for chemical reactions using reaction SMILES',
+    long_description='''\
     This package provides functions to calculate the atom economy of chemical reactions using reaction SMILES.
     It utilizes the RDKit library to handle molecular structures and properties.
     
     Features:
     - Calculation of atom economy for reactions
     - Handling of multiple reactions in a single calculation
     - Support for different types of reaction SMILES
@@ -24,8 +20,17 @@
     
     from rxnSMILES4AtomEco import calculate_atom_economy
     
     reactions_smiles = "C(CO)O.CCO.CC(C)O>CCO>C(C)O.CCO"
     calculate_atom_economy(reactions_smiles)
     
     For more information, please refer to the documentation at https://github.com/yourusername/rxnSMILES4AtomEco.
-    
+    ''',
+    author='Samuele Giani',
+    author_email='samuele.giani@empa.ch',
+    url='https://pypi.org/project/rxnSMILES4AtomEco/',
+    classifiers=[
+        'Programming Language :: Python :: 3',
+        'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
+        'Operating System :: OS Independent',
+    ],
+)
```

### Comparing `rxnSMILES4AtomEco-1.0.8/rxnSMILES4AtomEco.egg-info/PKG-INFO` & `rxnSMILES4AtomEco-1.0.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: rxnSMILES4AtomEco
-Version: 1.0.8
+Version: 1.0.9
 Summary: Calculate atom economy for chemical reactions using reaction SMILES
-Home-page: https://github.com/yourusername/rxnSMILES4AtomEco
+Home-page: https://pypi.org/project/rxnSMILES4AtomEco/
 Author: Samuele Giani
 Author-email: samuele.giani@empa.ch
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
-License-File: LICENSE
 
     This package provides functions to calculate the atom economy of chemical reactions using reaction SMILES.
     It utilizes the RDKit library to handle molecular structures and properties.
     
     Features:
     - Calculation of atom economy for reactions
     - Handling of multiple reactions in a single calculation
```

