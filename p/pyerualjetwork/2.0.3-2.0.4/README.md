# Comparing `tmp/pyerualjetwork-2.0.3.tar.gz` & `tmp/pyerualjetwork-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyerualjetwork-2.0.3.tar", last modified: Sun Jun  2 20:10:17 2024, max compression
+gzip compressed data, was "pyerualjetwork-2.0.4.tar", last modified: Sun Jun  2 20:15:27 2024, max compression
```

## Comparing `pyerualjetwork-2.0.3.tar` & `pyerualjetwork-2.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-06-02 20:10:17.316032 pyerualjetwork-2.0.3/
--rw-rw-rw-   0        0        0      429 2024-06-02 20:10:17.315028 pyerualjetwork-2.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-06-02 20:10:17.291034 pyerualjetwork-2.0.3/plan/
--rw-rw-rw-   0        0        0      377 2024-06-02 19:03:35.000000 pyerualjetwork-2.0.3/plan/__init__.py
--rw-rw-rw-   0        0        0    32839 2024-06-02 20:09:22.000000 pyerualjetwork-2.0.3/plan/plan.py
-drwxrwxrwx   0        0        0        0 2024-06-02 20:10:17.311980 pyerualjetwork-2.0.3/pyerualjetwork.egg-info/
--rw-rw-rw-   0        0        0      429 2024-06-02 20:10:16.000000 pyerualjetwork-2.0.3/pyerualjetwork.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2024-06-02 20:10:17.000000 pyerualjetwork-2.0.3/pyerualjetwork.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 20:10:16.000000 pyerualjetwork-2.0.3/pyerualjetwork.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-06-02 20:10:16.000000 pyerualjetwork-2.0.3/pyerualjetwork.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-06-02 20:10:17.317035 pyerualjetwork-2.0.3/setup.cfg
--rw-rw-rw-   0        0        0      608 2024-06-02 20:10:07.000000 pyerualjetwork-2.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 20:15:27.670363 pyerualjetwork-2.0.4/
+-rw-rw-rw-   0        0        0      429 2024-06-02 20:15:27.669332 pyerualjetwork-2.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-06-02 20:15:27.643788 pyerualjetwork-2.0.4/plan/
+-rw-rw-rw-   0        0        0      377 2024-06-02 19:03:35.000000 pyerualjetwork-2.0.4/plan/__init__.py
+-rw-rw-rw-   0        0        0    33028 2024-06-02 20:14:40.000000 pyerualjetwork-2.0.4/plan/plan.py
+drwxrwxrwx   0        0        0        0 2024-06-02 20:15:27.666331 pyerualjetwork-2.0.4/pyerualjetwork.egg-info/
+-rw-rw-rw-   0        0        0      429 2024-06-02 20:15:26.000000 pyerualjetwork-2.0.4/pyerualjetwork.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2024-06-02 20:15:27.000000 pyerualjetwork-2.0.4/pyerualjetwork.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 20:15:26.000000 pyerualjetwork-2.0.4/pyerualjetwork.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-06-02 20:15:26.000000 pyerualjetwork-2.0.4/pyerualjetwork.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-02 20:15:27.670363 pyerualjetwork-2.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      608 2024-06-02 20:15:16.000000 pyerualjetwork-2.0.4/setup.py
```

### Comparing `pyerualjetwork-2.0.3/plan/plan.py` & `pyerualjetwork-2.0.4/plan/plan.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,19 @@
         action_potential (float): Input ACTION potential 
     
     Returns:
         list([num]): (Weight matrices list, train_predictions list, Trainacc).
         error handled ?: Process status ('e')
 """
 
+    if action_potential < 0 or action_potential > 1:
+        
+        print(Fore.RED + "ERROR101: ACTION potential value must be in range 0-1. from: fit",infoPLAN)
+        return 'e'
+
     if len(x_train) != len(y_train):
        print(Fore.RED + "ERROR301: x_train list and y_train list must be same length. from: fit",infoPLAN)
        return 'e'
    
     class_count = set()
     for sublist in y_train:
```

### Comparing `pyerualjetwork-2.0.3/setup.py` & `pyerualjetwork-2.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 # Setting Up
 
 setup(
       
       name = "pyerualjetwork",
-      version = "2.0.3",
+      version = "2.0.4",
       author = "Hasan Can Beydili",
       author_email = "tchasancan@gmail.com",
       description= "Advanced python deep learning library. New features: More simple and practical, all functions and variables are snake_case. (Documentation in desc. Examples in GİTHUB: https://github.com/HCB06/PyerualJetwork)",
       packages = find_packages(),
       keywords = ["model evaluation", "classifcation", 'pruning learning artficial neural networks'],
```

