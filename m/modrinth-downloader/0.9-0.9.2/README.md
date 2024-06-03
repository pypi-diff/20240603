# Comparing `tmp/modrinth_downloader-0.9.tar.gz` & `tmp/modrinth_downloader-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modrinth_downloader-0.9.tar", last modified: Mon Jun  3 13:12:39 2024, max compression
+gzip compressed data, was "modrinth_downloader-0.9.2.tar", last modified: Mon Jun  3 13:13:34 2024, max compression
```

## Comparing `modrinth_downloader-0.9.tar` & `modrinth_downloader-0.9.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-06-03 13:12:39.723600 modrinth_downloader-0.9/
--rw-r--r--   0 tim       (1000) tim       (1000)       48 2024-06-03 13:00:27.000000 modrinth_downloader-0.9/MANIFEST.in
--rw-r--r--   0 tim       (1000) tim       (1000)      431 2024-06-03 13:12:39.723600 modrinth_downloader-0.9/PKG-INFO
--rw-r--r--   0 tim       (1000) tim       (1000)       91 2024-06-02 20:53:13.000000 modrinth_downloader-0.9/README.md
-drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-06-03 13:12:39.723600 modrinth_downloader-0.9/modrinth_downloader/
--rw-r--r--   0 tim       (1000) tim       (1000)        0 2024-06-02 20:51:42.000000 modrinth_downloader-0.9/modrinth_downloader/__init__.py
--rw-r--r--   0 tim       (1000) tim       (1000)     1523 2024-06-03 11:23:46.000000 modrinth_downloader-0.9/modrinth_downloader/api.py
--rw-r--r--   0 tim       (1000) tim       (1000)      579 2024-06-03 11:26:30.000000 modrinth_downloader-0.9/modrinth_downloader/downloader.py
-drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-06-03 13:12:39.723600 modrinth_downloader-0.9/modrinth_downloader/scripts/
--rw-r--r--   0 tim       (1000) tim       (1000)        0 2024-06-03 12:11:39.000000 modrinth_downloader-0.9/modrinth_downloader/scripts/__init__.py
--rw-r--r--   0 tim       (1000) tim       (1000)      179 2024-06-03 11:30:46.000000 modrinth_downloader-0.9/modrinth_downloader/scripts/config.toml
--rw-r--r--   0 tim       (1000) tim       (1000)     2570 2024-06-03 13:12:14.000000 modrinth_downloader-0.9/modrinth_downloader/scripts/run_downloader.py
--rw-r--r--   0 tim       (1000) tim       (1000)     1118 2024-06-03 13:10:19.000000 modrinth_downloader-0.9/modrinth_downloader/utils.py
-drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-06-03 13:12:39.723600 modrinth_downloader-0.9/modrinth_downloader.egg-info/
--rw-r--r--   0 tim       (1000) tim       (1000)      431 2024-06-03 13:12:39.000000 modrinth_downloader-0.9/modrinth_downloader.egg-info/PKG-INFO
--rw-r--r--   0 tim       (1000) tim       (1000)      581 2024-06-03 13:12:39.000000 modrinth_downloader-0.9/modrinth_downloader.egg-info/SOURCES.txt
--rw-r--r--   0 tim       (1000) tim       (1000)        1 2024-06-03 13:12:39.000000 modrinth_downloader-0.9/modrinth_downloader.egg-info/dependency_links.txt
--rw-r--r--   0 tim       (1000) tim       (1000)       88 2024-06-03 13:12:39.000000 modrinth_downloader-0.9/modrinth_downloader.egg-info/entry_points.txt
--rw-r--r--   0 tim       (1000) tim       (1000)       23 2024-06-03 13:12:39.000000 modrinth_downloader-0.9/modrinth_downloader.egg-info/requires.txt
--rw-r--r--   0 tim       (1000) tim       (1000)       26 2024-06-03 13:12:39.000000 modrinth_downloader-0.9/modrinth_downloader.egg-info/top_level.txt
--rw-r--r--   0 tim       (1000) tim       (1000)       38 2024-06-03 13:12:39.723600 modrinth_downloader-0.9/setup.cfg
--rw-r--r--   0 tim       (1000) tim       (1000)      970 2024-06-03 13:12:38.000000 modrinth_downloader-0.9/setup.py
-drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-06-03 13:12:39.723600 modrinth_downloader-0.9/tests/
--rw-r--r--   0 tim       (1000) tim       (1000)        0 2024-06-02 20:57:12.000000 modrinth_downloader-0.9/tests/__init__.py
--rw-r--r--   0 tim       (1000) tim       (1000)      341 2024-06-02 20:57:21.000000 modrinth_downloader-0.9/tests/test_downloader.py
+drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-06-03 13:13:34.763603 modrinth_downloader-0.9.2/
+-rw-r--r--   0 tim       (1000) tim       (1000)       48 2024-06-03 13:00:27.000000 modrinth_downloader-0.9.2/MANIFEST.in
+-rw-r--r--   0 tim       (1000) tim       (1000)      433 2024-06-03 13:13:34.763603 modrinth_downloader-0.9.2/PKG-INFO
+-rw-r--r--   0 tim       (1000) tim       (1000)       91 2024-06-02 20:53:13.000000 modrinth_downloader-0.9.2/README.md
+drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-06-03 13:13:34.763603 modrinth_downloader-0.9.2/modrinth_downloader/
+-rw-r--r--   0 tim       (1000) tim       (1000)        0 2024-06-02 20:51:42.000000 modrinth_downloader-0.9.2/modrinth_downloader/__init__.py
+-rw-r--r--   0 tim       (1000) tim       (1000)     1523 2024-06-03 11:23:46.000000 modrinth_downloader-0.9.2/modrinth_downloader/api.py
+-rw-r--r--   0 tim       (1000) tim       (1000)      579 2024-06-03 11:26:30.000000 modrinth_downloader-0.9.2/modrinth_downloader/downloader.py
+drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-06-03 13:13:34.763603 modrinth_downloader-0.9.2/modrinth_downloader/scripts/
+-rw-r--r--   0 tim       (1000) tim       (1000)        0 2024-06-03 12:11:39.000000 modrinth_downloader-0.9.2/modrinth_downloader/scripts/__init__.py
+-rw-r--r--   0 tim       (1000) tim       (1000)      179 2024-06-03 11:30:46.000000 modrinth_downloader-0.9.2/modrinth_downloader/scripts/config.toml
+-rw-r--r--   0 tim       (1000) tim       (1000)     2569 2024-06-03 13:13:26.000000 modrinth_downloader-0.9.2/modrinth_downloader/scripts/run_downloader.py
+-rw-r--r--   0 tim       (1000) tim       (1000)     1118 2024-06-03 13:10:19.000000 modrinth_downloader-0.9.2/modrinth_downloader/utils.py
+drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-06-03 13:13:34.763603 modrinth_downloader-0.9.2/modrinth_downloader.egg-info/
+-rw-r--r--   0 tim       (1000) tim       (1000)      433 2024-06-03 13:13:34.000000 modrinth_downloader-0.9.2/modrinth_downloader.egg-info/PKG-INFO
+-rw-r--r--   0 tim       (1000) tim       (1000)      581 2024-06-03 13:13:34.000000 modrinth_downloader-0.9.2/modrinth_downloader.egg-info/SOURCES.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)        1 2024-06-03 13:13:34.000000 modrinth_downloader-0.9.2/modrinth_downloader.egg-info/dependency_links.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)       88 2024-06-03 13:13:34.000000 modrinth_downloader-0.9.2/modrinth_downloader.egg-info/entry_points.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)       23 2024-06-03 13:13:34.000000 modrinth_downloader-0.9.2/modrinth_downloader.egg-info/requires.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)       26 2024-06-03 13:13:34.000000 modrinth_downloader-0.9.2/modrinth_downloader.egg-info/top_level.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)       38 2024-06-03 13:13:34.763603 modrinth_downloader-0.9.2/setup.cfg
+-rw-r--r--   0 tim       (1000) tim       (1000)      972 2024-06-03 13:13:33.000000 modrinth_downloader-0.9.2/setup.py
+drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-06-03 13:13:34.763603 modrinth_downloader-0.9.2/tests/
+-rw-r--r--   0 tim       (1000) tim       (1000)        0 2024-06-02 20:57:12.000000 modrinth_downloader-0.9.2/tests/__init__.py
+-rw-r--r--   0 tim       (1000) tim       (1000)      341 2024-06-02 20:57:21.000000 modrinth_downloader-0.9.2/tests/test_downloader.py
```

### Comparing `modrinth_downloader-0.9/modrinth_downloader/api.py` & `modrinth_downloader-0.9.2/modrinth_downloader/api.py`

 * *Files identical despite different names*

### Comparing `modrinth_downloader-0.9/modrinth_downloader/downloader.py` & `modrinth_downloader-0.9.2/modrinth_downloader/downloader.py`

 * *Files identical despite different names*

### Comparing `modrinth_downloader-0.9/modrinth_downloader/scripts/run_downloader.py` & `modrinth_downloader-0.9.2/modrinth_downloader/scripts/run_downloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 download_path = os.path.expanduser(config_download_path)
 backup_path = os.path.expanduser(config_backup_path)
 
 def main():
     setup_dirs(list_path)
 
     parser = argparse.ArgumentParser(description="Parse Arguments for "
-                                                 "Modrinth Downloader"
-                                                 "\n List Path is at" +
+                                                 "Modrinth Downloader. "
+                                                 "List Path is at" +
                                                  list_path)
 
     parser.add_argument('-v', '--verbose', action='store_true',
                         help='Increase output verbosity')
     parser.add_argument('--list', type=str, help='The list name',
                         required=True)
     parser.add_argument('-m', '--game_version', type=str,
```

### Comparing `modrinth_downloader-0.9/modrinth_downloader/utils.py` & `modrinth_downloader-0.9.2/modrinth_downloader/utils.py`

 * *Files identical despite different names*

### Comparing `modrinth_downloader-0.9/modrinth_downloader.egg-info/SOURCES.txt` & `modrinth_downloader-0.9.2/modrinth_downloader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modrinth_downloader-0.9/setup.py` & `modrinth_downloader-0.9.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='modrinth_downloader',
-    version='0.9',
+    version='0.9.2',
     author='Alexander Brightwater',
     description="Download projects from Modrinth",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     packages=find_packages(),  # Automatically find packages
     classifiers=[
         'Programming Language :: Python :: 3',
```

