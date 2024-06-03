# Comparing `tmp/modrinth_downloader-0.9.2.tar.gz` & `tmp/modrinth_downloader-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modrinth_downloader-0.9.2.tar", last modified: Mon Jun  3 13:13:34 2024, max compression
+gzip compressed data, was "modrinth_downloader-0.9.3.tar", last modified: Mon Jun  3 13:43:52 2024, max compression
```

## Comparing `modrinth_downloader-0.9.2.tar` & `modrinth_downloader-0.9.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-06-03 13:13:34.763603 modrinth_downloader-0.9.2/
--rw-r--r--   0 tim       (1000) tim       (1000)       48 2024-06-03 13:00:27.000000 modrinth_downloader-0.9.2/MANIFEST.in
--rw-r--r--   0 tim       (1000) tim       (1000)      433 2024-06-03 13:13:34.763603 modrinth_downloader-0.9.2/PKG-INFO
--rw-r--r--   0 tim       (1000) tim       (1000)       91 2024-06-02 20:53:13.000000 modrinth_downloader-0.9.2/README.md
-drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-06-03 13:13:34.763603 modrinth_downloader-0.9.2/modrinth_downloader/
--rw-r--r--   0 tim       (1000) tim       (1000)        0 2024-06-02 20:51:42.000000 modrinth_downloader-0.9.2/modrinth_downloader/__init__.py
--rw-r--r--   0 tim       (1000) tim       (1000)     1523 2024-06-03 11:23:46.000000 modrinth_downloader-0.9.2/modrinth_downloader/api.py
--rw-r--r--   0 tim       (1000) tim       (1000)      579 2024-06-03 11:26:30.000000 modrinth_downloader-0.9.2/modrinth_downloader/downloader.py
-drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-06-03 13:13:34.763603 modrinth_downloader-0.9.2/modrinth_downloader/scripts/
--rw-r--r--   0 tim       (1000) tim       (1000)        0 2024-06-03 12:11:39.000000 modrinth_downloader-0.9.2/modrinth_downloader/scripts/__init__.py
--rw-r--r--   0 tim       (1000) tim       (1000)      179 2024-06-03 11:30:46.000000 modrinth_downloader-0.9.2/modrinth_downloader/scripts/config.toml
--rw-r--r--   0 tim       (1000) tim       (1000)     2569 2024-06-03 13:13:26.000000 modrinth_downloader-0.9.2/modrinth_downloader/scripts/run_downloader.py
--rw-r--r--   0 tim       (1000) tim       (1000)     1118 2024-06-03 13:10:19.000000 modrinth_downloader-0.9.2/modrinth_downloader/utils.py
-drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-06-03 13:13:34.763603 modrinth_downloader-0.9.2/modrinth_downloader.egg-info/
--rw-r--r--   0 tim       (1000) tim       (1000)      433 2024-06-03 13:13:34.000000 modrinth_downloader-0.9.2/modrinth_downloader.egg-info/PKG-INFO
--rw-r--r--   0 tim       (1000) tim       (1000)      581 2024-06-03 13:13:34.000000 modrinth_downloader-0.9.2/modrinth_downloader.egg-info/SOURCES.txt
--rw-r--r--   0 tim       (1000) tim       (1000)        1 2024-06-03 13:13:34.000000 modrinth_downloader-0.9.2/modrinth_downloader.egg-info/dependency_links.txt
--rw-r--r--   0 tim       (1000) tim       (1000)       88 2024-06-03 13:13:34.000000 modrinth_downloader-0.9.2/modrinth_downloader.egg-info/entry_points.txt
--rw-r--r--   0 tim       (1000) tim       (1000)       23 2024-06-03 13:13:34.000000 modrinth_downloader-0.9.2/modrinth_downloader.egg-info/requires.txt
--rw-r--r--   0 tim       (1000) tim       (1000)       26 2024-06-03 13:13:34.000000 modrinth_downloader-0.9.2/modrinth_downloader.egg-info/top_level.txt
--rw-r--r--   0 tim       (1000) tim       (1000)       38 2024-06-03 13:13:34.763603 modrinth_downloader-0.9.2/setup.cfg
--rw-r--r--   0 tim       (1000) tim       (1000)      972 2024-06-03 13:13:33.000000 modrinth_downloader-0.9.2/setup.py
-drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-06-03 13:13:34.763603 modrinth_downloader-0.9.2/tests/
--rw-r--r--   0 tim       (1000) tim       (1000)        0 2024-06-02 20:57:12.000000 modrinth_downloader-0.9.2/tests/__init__.py
--rw-r--r--   0 tim       (1000) tim       (1000)      341 2024-06-02 20:57:21.000000 modrinth_downloader-0.9.2/tests/test_downloader.py
+drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-06-03 13:43:52.283714 modrinth_downloader-0.9.3/
+-rw-r--r--   0 tim       (1000) tim       (1000)       48 2024-06-03 13:00:27.000000 modrinth_downloader-0.9.3/MANIFEST.in
+-rw-r--r--   0 tim       (1000) tim       (1000)      433 2024-06-03 13:43:52.283714 modrinth_downloader-0.9.3/PKG-INFO
+-rw-r--r--   0 tim       (1000) tim       (1000)       91 2024-06-02 20:53:13.000000 modrinth_downloader-0.9.3/README.md
+drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-06-03 13:43:52.283714 modrinth_downloader-0.9.3/modrinth_downloader/
+-rw-r--r--   0 tim       (1000) tim       (1000)        0 2024-06-02 20:51:42.000000 modrinth_downloader-0.9.3/modrinth_downloader/__init__.py
+-rw-r--r--   0 tim       (1000) tim       (1000)     1523 2024-06-03 11:23:46.000000 modrinth_downloader-0.9.3/modrinth_downloader/api.py
+-rw-r--r--   0 tim       (1000) tim       (1000)      579 2024-06-03 11:26:30.000000 modrinth_downloader-0.9.3/modrinth_downloader/downloader.py
+drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-06-03 13:43:52.283714 modrinth_downloader-0.9.3/modrinth_downloader/scripts/
+-rw-r--r--   0 tim       (1000) tim       (1000)        0 2024-06-03 12:11:39.000000 modrinth_downloader-0.9.3/modrinth_downloader/scripts/__init__.py
+-rw-r--r--   0 tim       (1000) tim       (1000)      214 2024-06-03 13:26:40.000000 modrinth_downloader-0.9.3/modrinth_downloader/scripts/config.toml
+-rw-r--r--   0 tim       (1000) tim       (1000)     2747 2024-06-03 13:42:20.000000 modrinth_downloader-0.9.3/modrinth_downloader/scripts/run_downloader.py
+-rw-r--r--   0 tim       (1000) tim       (1000)     1652 2024-06-03 13:42:56.000000 modrinth_downloader-0.9.3/modrinth_downloader/utils.py
+drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-06-03 13:43:52.283714 modrinth_downloader-0.9.3/modrinth_downloader.egg-info/
+-rw-r--r--   0 tim       (1000) tim       (1000)      433 2024-06-03 13:43:52.000000 modrinth_downloader-0.9.3/modrinth_downloader.egg-info/PKG-INFO
+-rw-r--r--   0 tim       (1000) tim       (1000)      581 2024-06-03 13:43:52.000000 modrinth_downloader-0.9.3/modrinth_downloader.egg-info/SOURCES.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)        1 2024-06-03 13:43:52.000000 modrinth_downloader-0.9.3/modrinth_downloader.egg-info/dependency_links.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)       88 2024-06-03 13:43:52.000000 modrinth_downloader-0.9.3/modrinth_downloader.egg-info/entry_points.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)       23 2024-06-03 13:43:52.000000 modrinth_downloader-0.9.3/modrinth_downloader.egg-info/requires.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)       26 2024-06-03 13:43:52.000000 modrinth_downloader-0.9.3/modrinth_downloader.egg-info/top_level.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)       38 2024-06-03 13:43:52.283714 modrinth_downloader-0.9.3/setup.cfg
+-rw-r--r--   0 tim       (1000) tim       (1000)      972 2024-06-03 13:43:11.000000 modrinth_downloader-0.9.3/setup.py
+drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-06-03 13:43:52.283714 modrinth_downloader-0.9.3/tests/
+-rw-r--r--   0 tim       (1000) tim       (1000)        0 2024-06-02 20:57:12.000000 modrinth_downloader-0.9.3/tests/__init__.py
+-rw-r--r--   0 tim       (1000) tim       (1000)      341 2024-06-02 20:57:21.000000 modrinth_downloader-0.9.3/tests/test_downloader.py
```

### Comparing `modrinth_downloader-0.9.2/modrinth_downloader/api.py` & `modrinth_downloader-0.9.3/modrinth_downloader/api.py`

 * *Files identical despite different names*

### Comparing `modrinth_downloader-0.9.2/modrinth_downloader/downloader.py` & `modrinth_downloader-0.9.3/modrinth_downloader/downloader.py`

 * *Files identical despite different names*

### Comparing `modrinth_downloader-0.9.2/modrinth_downloader/scripts/run_downloader.py` & `modrinth_downloader-0.9.3/modrinth_downloader/scripts/run_downloader.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,21 +8,24 @@
 config_path = os.path.join(current_dir, 'config.toml')
 with open(config_path, 'r') as config_file:
     config = toml.load(config_file)
 
 config_list_path = config['paths']['lists']
 config_download_path = config['paths']['downloads']
 config_backup_path = config['paths']['backups']
+config_config_path = config['paths']['config']
 
 list_path = os.path.expanduser(config_list_path)
 download_path = os.path.expanduser(config_download_path)
 backup_path = os.path.expanduser(config_backup_path)
+config_path = os.path.expanduser(config_config_path)
 
 def main():
-    setup_dirs(list_path)
+    setup_dirs(list_path, download_path, backup_path, config_path)
+    link_config(config_path, config)
 
     parser = argparse.ArgumentParser(description="Parse Arguments for "
                                                  "Modrinth Downloader. "
                                                  "List Path is at" +
                                                  list_path)
 
     parser.add_argument('-v', '--verbose', action='store_true',
```

### Comparing `modrinth_downloader-0.9.2/modrinth_downloader/utils.py` & `modrinth_downloader-0.9.3/modrinth_downloader/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import shutil
+import toml
 def rotate_backups(list_name, download_path, backup_path, max_backups=5):
     specific_backup_path = os.path.join(backup_path, list_name)
 
     if not os.path.exists(backup_path):
         os.makedirs(backup_path)
 
     # Rotate existing backups
@@ -20,10 +21,23 @@
                     os.path.join(str(specific_backup_path), "backup_1"))
 
     # Create a new current backup
     if not os.path.exists(specific_backup_path):
         os.makedirs(specific_backup_path)
     shutil.move(os.path.join(str(download_path), list_name), current_backup)
 
-def setup_dirs(list_path):
+def setup_dirs(list_path, download_path, backup_path, config_path):
     if not os.path.exists(list_path):
         os.makedirs(list_path)
+    if not os.path.exists(download_path):
+        os.makedirs(download_path)
+    if not os.path.exists(backup_path):
+        os.makedirs(backup_path)
+    if not os.path.exists(config_path):
+        os.makedirs(config_path)
+
+def link_config(config_path, config):
+    if not os.path.exists(config_path):
+        os.makedirs(config_path)
+    output_path = os.path.join(config_path, 'config.toml')
+    with open(output_path, 'w') as output_file:
+        toml.dump(config, output_file)
```

### Comparing `modrinth_downloader-0.9.2/modrinth_downloader.egg-info/SOURCES.txt` & `modrinth_downloader-0.9.3/modrinth_downloader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modrinth_downloader-0.9.2/setup.py` & `modrinth_downloader-0.9.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='modrinth_downloader',
-    version='0.9.2',
+    version='0.9.3',
     author='Alexander Brightwater',
     description="Download projects from Modrinth",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     packages=find_packages(),  # Automatically find packages
     classifiers=[
         'Programming Language :: Python :: 3',
```

