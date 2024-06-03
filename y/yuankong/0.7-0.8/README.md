# Comparing `tmp/yuankong-0.7.tar.gz` & `tmp/yuankong-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yuankong-0.7.tar", last modified: Mon Apr 15 09:00:17 2024, max compression
+gzip compressed data, was "yuankong-0.8.tar", last modified: Mon Jun  3 02:28:13 2024, max compression
```

## Comparing `yuankong-0.7.tar` & `yuankong-0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-15 09:00:17.067022 yuankong-0.7/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-15 08:59:13.000000 yuankong-0.7/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      418 2024-04-15 09:00:17.067022 yuankong-0.7/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       12 2024-04-15 08:59:13.000000 yuankong-0.7/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-15 09:00:17.067022 yuankong-0.7/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      719 2024-04-15 09:00:13.000000 yuankong-0.7/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-15 09:00:17.067022 yuankong-0.7/yuankong/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       43 2024-04-15 08:59:13.000000 yuankong-0.7/yuankong/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-15 09:00:17.067022 yuankong-0.7/yuankong/rpa/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-15 08:59:13.000000 yuankong-0.7/yuankong/rpa/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-15 09:00:17.067022 yuankong-0.7/yuankong/utils/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      136 2024-04-15 08:59:13.000000 yuankong-0.7/yuankong/utils/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2860 2024-04-15 08:59:56.000000 yuankong-0.7/yuankong/utils/bucket.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3490 2024-04-15 08:59:13.000000 yuankong-0.7/yuankong/utils/logManager.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-15 09:00:17.067022 yuankong-0.7/yuankong.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      418 2024-04-15 09:00:17.000000 yuankong-0.7/yuankong.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      281 2024-04-15 09:00:17.000000 yuankong-0.7/yuankong.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-15 09:00:17.000000 yuankong-0.7/yuankong.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2024-04-15 09:00:17.000000 yuankong-0.7/yuankong.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 02:28:13.069124 yuankong-0.8/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 08:52:29.000000 yuankong-0.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      418 2024-06-03 02:28:13.069124 yuankong-0.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       12 2024-04-15 08:52:29.000000 yuankong-0.8/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-06-03 02:28:13.069124 yuankong-0.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      719 2024-06-03 02:27:53.000000 yuankong-0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 02:28:13.065124 yuankong-0.8/yuankong/
+-rw-r--r--   0 root         (0) root         (0)       44 2024-06-03 02:26:56.000000 yuankong-0.8/yuankong/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 02:28:13.065124 yuankong-0.8/yuankong/rpa/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 08:52:29.000000 yuankong-0.8/yuankong/rpa/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 02:28:13.065124 yuankong-0.8/yuankong/utils/
+-rw-r--r--   0 root         (0) root         (0)      136 2024-04-15 08:52:29.000000 yuankong-0.8/yuankong/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2860 2024-04-15 08:53:27.000000 yuankong-0.8/yuankong/utils/bucket.py
+-rw-r--r--   0 root         (0) root         (0)     3490 2024-04-15 08:52:29.000000 yuankong-0.8/yuankong/utils/logManager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 02:28:13.065124 yuankong-0.8/yuankong.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      418 2024-06-03 02:28:13.000000 yuankong-0.8/yuankong.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      281 2024-06-03 02:28:13.000000 yuankong-0.8/yuankong.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-06-03 02:28:13.000000 yuankong-0.8/yuankong.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-06-03 02:28:13.000000 yuankong-0.8/yuankong.egg-info/top_level.txt
```

### Comparing `yuankong-0.7/setup.py` & `yuankong-0.8/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='yuankong',
-    version='0.7',
+    version='0.8',
     packages=find_packages(),
     description='Basic function of YuankongAI',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',  # 这使得README.md可以正确渲染
     author='ltq_yuankong',
     author_email='1539365976@qq.com',
     # url='http://60.205.141.203:3000/ningkp/MetaAgent/src/user_isolation',
```

### Comparing `yuankong-0.7/yuankong/utils/bucket.py` & `yuankong-0.8/yuankong/utils/bucket.py`

 * *Files identical despite different names*

### Comparing `yuankong-0.7/yuankong/utils/logManager.py` & `yuankong-0.8/yuankong/utils/logManager.py`

 * *Files identical despite different names*

