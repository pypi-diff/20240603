# Comparing `tmp/SynapseTrie-0.1.tar.gz` & `tmp/SynapseTrie-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SynapseTrie-0.1.tar", last modified: Tue May 28 13:28:58 2024, max compression
+gzip compressed data, was "SynapseTrie-0.2.tar", last modified: Mon Jun  3 08:18:02 2024, max compression
```

## Comparing `SynapseTrie-0.1.tar` & `SynapseTrie-0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:28:58.052326 SynapseTrie-0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-28 13:28:40.000000 SynapseTrie-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-28 13:28:58.052326 SynapseTrie-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-28 13:28:40.000000 SynapseTrie-0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:28:58.052326 SynapseTrie-0.1/SynapseTrie/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-28 13:28:40.000000 SynapseTrie-0.1/SynapseTrie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-05-28 13:28:40.000000 SynapseTrie-0.1/SynapseTrie/trie.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-28 13:28:40.000000 SynapseTrie-0.1/SynapseTrie/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:28:58.052326 SynapseTrie-0.1/SynapseTrie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-28 13:28:57.000000 SynapseTrie-0.1/SynapseTrie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-28 13:28:57.000000 SynapseTrie-0.1/SynapseTrie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 13:28:57.000000 SynapseTrie-0.1/SynapseTrie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-28 13:28:57.000000 SynapseTrie-0.1/SynapseTrie.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-28 13:28:57.000000 SynapseTrie-0.1/SynapseTrie.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 13:28:58.056326 SynapseTrie-0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-28 13:28:40.000000 SynapseTrie-0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:28:58.052326 SynapseTrie-0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 13:28:40.000000 SynapseTrie-0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-28 13:28:40.000000 SynapseTrie-0.1/tests/test_trie.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:18:02.493180 SynapseTrie-0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-06-03 08:17:53.000000 SynapseTrie-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-06-03 08:18:02.493180 SynapseTrie-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-06-03 08:17:53.000000 SynapseTrie-0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:18:02.493180 SynapseTrie-0.2/SynapseTrie/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-06-03 08:17:53.000000 SynapseTrie-0.2/SynapseTrie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17241 2024-06-03 08:17:53.000000 SynapseTrie-0.2/SynapseTrie/trie.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-06-03 08:17:53.000000 SynapseTrie-0.2/SynapseTrie/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:18:02.493180 SynapseTrie-0.2/SynapseTrie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-06-03 08:18:02.000000 SynapseTrie-0.2/SynapseTrie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-06-03 08:18:02.000000 SynapseTrie-0.2/SynapseTrie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 08:18:02.000000 SynapseTrie-0.2/SynapseTrie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-06-03 08:18:02.000000 SynapseTrie-0.2/SynapseTrie.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-06-03 08:18:02.000000 SynapseTrie-0.2/SynapseTrie.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 08:18:02.493180 SynapseTrie-0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-06-03 08:17:53.000000 SynapseTrie-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:18:02.493180 SynapseTrie-0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 08:17:53.000000 SynapseTrie-0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8933 2024-06-03 08:17:53.000000 SynapseTrie-0.2/tests/test_trie.py
```

### Comparing `SynapseTrie-0.1/LICENSE` & `SynapseTrie-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `SynapseTrie-0.1/PKG-INFO` & `SynapseTrie-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SynapseTrie
-Version: 0.1
+Version: 0.2
 Summary: Efficient trie for storing and searching phrases.
 Home-page: https://github.com/J0nasW/SynapseTrie
 Author: Jonas Wilinski
 Author-email: jonas@wilinski.me
 License: UNKNOWN
 Description: # Synapse Trie
```

### Comparing `SynapseTrie-0.1/SynapseTrie/utilities.py` & `SynapseTrie-0.2/SynapseTrie/utilities.py`

 * *Files identical despite different names*

### Comparing `SynapseTrie-0.1/SynapseTrie.egg-info/PKG-INFO` & `SynapseTrie-0.2/SynapseTrie.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SynapseTrie
-Version: 0.1
+Version: 0.2
 Summary: Efficient trie for storing and searching phrases.
 Home-page: https://github.com/J0nasW/SynapseTrie
 Author: Jonas Wilinski
 Author-email: jonas@wilinski.me
 License: UNKNOWN
 Description: # Synapse Trie
```

### Comparing `SynapseTrie-0.1/setup.py` & `SynapseTrie-0.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from setuptools import setup, find_packages
 
 setup(
     name='SynapseTrie',
-    version='0.1',
+    version='0.2',
     packages=find_packages(),
     description='Efficient trie for storing and searching phrases.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Jonas Wilinski',
     author_email='jonas@wilinski.me',
     url='https://github.com/J0nasW/SynapseTrie',
     install_requires=[
         'pandas>=1.1.5',
         'nltk>=3.5',
         'scipy>=1.5.4',
-        'tqdm>=4.56.0'
+        'tqdm>=4.56.0',
+        'pyyaml>=5.4.1',
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
```

