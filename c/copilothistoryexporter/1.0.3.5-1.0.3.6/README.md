# Comparing `tmp/copilothistoryexporter-1.0.3.5.tar.gz` & `tmp/copilothistoryexporter-1.0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copilothistoryexporter-1.0.3.5.tar", last modified: Sun Jun  2 20:22:06 2024, max compression
+gzip compressed data, was "copilothistoryexporter-1.0.3.6.tar", last modified: Sun Jun  2 20:57:46 2024, max compression
```

## Comparing `copilothistoryexporter-1.0.3.5.tar` & `copilothistoryexporter-1.0.3.6.tar`

### file list

```diff
@@ -1,18 +1,32 @@
-drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-02 20:22:06.754324 copilothistoryexporter-1.0.3.5/
--rw-r--r--   0 mustafakilic   (501) staff       (20)     1073 2024-06-01 16:20:49.000000 copilothistoryexporter-1.0.3.5/LICENCE
--rw-r--r--   0 mustafakilic   (501) staff       (20)      467 2024-06-02 20:22:06.754129 copilothistoryexporter-1.0.3.5/PKG-INFO
--rw-r--r--   0 mustafakilic   (501) staff       (20)     2232 2024-06-02 16:13:30.000000 copilothistoryexporter-1.0.3.5/README.md
-drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-02 20:22:06.753932 copilothistoryexporter-1.0.3.5/copilothistoryexporter.egg-info/
--rw-r--r--   0 mustafakilic   (501) staff       (20)      467 2024-06-02 20:22:06.000000 copilothistoryexporter-1.0.3.5/copilothistoryexporter.egg-info/PKG-INFO
--rw-r--r--   0 mustafakilic   (501) staff       (20)      412 2024-06-02 20:22:06.000000 copilothistoryexporter-1.0.3.5/copilothistoryexporter.egg-info/SOURCES.txt
--rw-r--r--   0 mustafakilic   (501) staff       (20)        1 2024-06-02 20:22:06.000000 copilothistoryexporter-1.0.3.5/copilothistoryexporter.egg-info/dependency_links.txt
--rw-r--r--   0 mustafakilic   (501) staff       (20)       80 2024-06-02 20:22:06.000000 copilothistoryexporter-1.0.3.5/copilothistoryexporter.egg-info/entry_points.txt
--rw-r--r--   0 mustafakilic   (501) staff       (20)       42 2024-06-02 20:22:06.000000 copilothistoryexporter-1.0.3.5/copilothistoryexporter.egg-info/requires.txt
--rw-r--r--   0 mustafakilic   (501) staff       (20)        1 2024-06-02 20:22:06.000000 copilothistoryexporter-1.0.3.5/copilothistoryexporter.egg-info/top_level.txt
--rw-r--r--   0 mustafakilic   (501) staff       (20)       38 2024-06-02 20:22:06.754360 copilothistoryexporter-1.0.3.5/setup.cfg
--rw-r--r--   0 mustafakilic   (501) staff       (20)      759 2024-06-02 20:21:54.000000 copilothistoryexporter-1.0.3.5/setup.py
-drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-02 20:22:06.752344 copilothistoryexporter-1.0.3.5/src/
-drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-02 20:22:06.753766 copilothistoryexporter-1.0.3.5/src/copilothistoryexporter/
--rw-r--r--   0 mustafakilic   (501) staff       (20)      768 2024-06-02 20:19:26.000000 copilothistoryexporter-1.0.3.5/src/copilothistoryexporter/main.py
--rw-r--r--   0 mustafakilic   (501) staff       (20)       92 2024-06-02 16:13:00.000000 copilothistoryexporter-1.0.3.5/src/copilothistoryexporter/sample.md
--rw-r--r--   0 mustafakilic   (501) staff       (20)     2359 2024-06-02 19:54:24.000000 copilothistoryexporter-1.0.3.5/src/copilothistoryexporter/utils.py
+drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-02 20:57:46.966991 copilothistoryexporter-1.0.3.6/
+-rw-r--r--   0 mustafakilic   (501) staff       (20)     1073 2024-06-01 16:20:49.000000 copilothistoryexporter-1.0.3.6/LICENCE
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      467 2024-06-02 20:57:46.966819 copilothistoryexporter-1.0.3.6/PKG-INFO
+-rw-r--r--   0 mustafakilic   (501) staff       (20)     2232 2024-06-02 16:13:30.000000 copilothistoryexporter-1.0.3.6/README.md
+drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-02 20:57:46.966653 copilothistoryexporter-1.0.3.6/copilothistoryexporter.egg-info/
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      467 2024-06-02 20:57:46.000000 copilothistoryexporter-1.0.3.6/copilothistoryexporter.egg-info/PKG-INFO
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      610 2024-06-02 20:57:46.000000 copilothistoryexporter-1.0.3.6/copilothistoryexporter.egg-info/SOURCES.txt
+-rw-r--r--   0 mustafakilic   (501) staff       (20)        1 2024-06-02 20:57:46.000000 copilothistoryexporter-1.0.3.6/copilothistoryexporter.egg-info/dependency_links.txt
+-rw-r--r--   0 mustafakilic   (501) staff       (20)       53 2024-06-02 20:57:46.000000 copilothistoryexporter-1.0.3.6/copilothistoryexporter.egg-info/entry_points.txt
+-rw-r--r--   0 mustafakilic   (501) staff       (20)       42 2024-06-02 20:57:46.000000 copilothistoryexporter-1.0.3.6/copilothistoryexporter.egg-info/requires.txt
+-rw-r--r--   0 mustafakilic   (501) staff       (20)        4 2024-06-02 20:57:46.000000 copilothistoryexporter-1.0.3.6/copilothistoryexporter.egg-info/top_level.txt
+-rw-r--r--   0 mustafakilic   (501) staff       (20)       38 2024-06-02 20:57:46.967025 copilothistoryexporter-1.0.3.6/setup.cfg
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      732 2024-06-02 20:57:40.000000 copilothistoryexporter-1.0.3.6/setup.py
+drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-02 20:57:46.965382 copilothistoryexporter-1.0.3.6/src/
+-rw-r--r--   0 mustafakilic   (501) staff       (20)        0 2024-06-02 20:51:23.000000 copilothistoryexporter-1.0.3.6/src/__init__.py
+drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-02 20:57:46.965582 copilothistoryexporter-1.0.3.6/src/addons/
+-rw-r--r--   0 mustafakilic   (501) staff       (20)        0 2024-06-02 20:52:06.000000 copilothistoryexporter-1.0.3.6/src/addons/__init__.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)     1457 2024-06-02 20:55:47.000000 copilothistoryexporter-1.0.3.6/src/addons/binding.py
+drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-02 20:57:46.966212 copilothistoryexporter-1.0.3.6/src/intercp/
+-rw-r--r--   0 mustafakilic   (501) staff       (20)        0 2024-06-02 20:55:28.000000 copilothistoryexporter-1.0.3.6/src/intercp/__init__.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      460 2024-06-02 20:55:47.000000 copilothistoryexporter-1.0.3.6/src/intercp/cache.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      575 2024-06-02 20:55:47.000000 copilothistoryexporter-1.0.3.6/src/intercp/chain.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      186 2024-06-02 20:55:47.000000 copilothistoryexporter-1.0.3.6/src/intercp/interceptor.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      305 2024-06-02 20:55:47.000000 copilothistoryexporter-1.0.3.6/src/intercp/markdown.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      549 2024-06-02 20:55:47.000000 copilothistoryexporter-1.0.3.6/src/intercp/vote.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)     1136 2024-06-02 20:55:47.000000 copilothistoryexporter-1.0.3.6/src/main.py
+drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-02 20:57:46.966507 copilothistoryexporter-1.0.3.6/src/model/
+-rw-r--r--   0 mustafakilic   (501) staff       (20)        0 2024-06-02 20:55:47.000000 copilothistoryexporter-1.0.3.6/src/model/__init__.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      395 2024-06-02 16:13:00.000000 copilothistoryexporter-1.0.3.6/src/model/conversation.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      232 2024-06-02 20:55:47.000000 copilothistoryexporter-1.0.3.6/src/model/request.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)       92 2024-06-02 16:13:00.000000 copilothistoryexporter-1.0.3.6/src/sample.md
+-rw-r--r--   0 mustafakilic   (501) staff       (20)     2364 2024-06-02 20:55:47.000000 copilothistoryexporter-1.0.3.6/src/utils.py
```

### Comparing `copilothistoryexporter-1.0.3.5/LICENCE` & `copilothistoryexporter-1.0.3.6/LICENCE`

 * *Files identical despite different names*

### Comparing `copilothistoryexporter-1.0.3.5/README.md` & `copilothistoryexporter-1.0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `copilothistoryexporter-1.0.3.5/setup.py` & `copilothistoryexporter-1.0.3.6/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 
 from setuptools import setup, find_packages
 
 setup(
     name="copilothistoryexporter",
-    version='1.0.3.5',
+    version='1.0.3.6',
     url='https://github.com/enciyo/gh-copilot-history-export',
     author='Mustafa Kilic',
     author_email='enciyomk61@gmail.com',
     description='This package exports the history of GitHub Copilot chat history.',
     long_description="This package exports the history of GitHub Copilot chat history.",
     packages=find_packages(),
     package_data={'': ['*.md']},
@@ -17,11 +17,11 @@
         "click",
         "mitmproxy",
         "wheel",
         "setuptools",
     ],
     entry_points={
         'console_scripts': [
-            'copilothistoryexporter = copilothistoryexporter.__main__:main'
+            'copilothistoryexporter = main:main'
         ]
     },
 )
```

### Comparing `copilothistoryexporter-1.0.3.5/src/copilothistoryexporter/utils.py` & `copilothistoryexporter-1.0.3.6/src/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import json
 import os
-from model.conversation import Conversation
 
 import subprocess
 
+from src.model.conversation import Conversation
+
 
 class SharedValues:
     WORKSPACE = ""
 
     @staticmethod
     def change_workspace(src: str):
         SharedValues.WORKSPACE = src
```

