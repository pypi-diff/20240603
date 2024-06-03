# Comparing `tmp/zenodo_backpack-0.3.0.tar.gz` & `tmp/zenodo_backpack-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zenodo_backpack-0.3.0.tar", last modified: Wed May  1 00:22:50 2024, max compression
+gzip compressed data, was "zenodo_backpack-0.3.1.tar", last modified: Mon Jun  3 06:54:28 2024, max compression
```

## Comparing `zenodo_backpack-0.3.0.tar` & `zenodo_backpack-0.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:50.776973 zenodo_backpack-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-01 00:22:34.000000 zenodo_backpack-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4924 2024-05-01 00:22:50.776973 zenodo_backpack-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4214 2024-05-01 00:22:34.000000 zenodo_backpack-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:50.772973 zenodo_backpack-0.3.0/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)     5686 2024-05-01 00:22:34.000000 zenodo_backpack-0.3.0/bin/zenodo_backpack
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 00:22:50.776973 zenodo_backpack-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-01 00:22:34.000000 zenodo_backpack-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:50.776973 zenodo_backpack-0.3.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-05-01 00:22:34.000000 zenodo_backpack-0.3.0/test/test_downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:50.776973 zenodo_backpack-0.3.0/zenodo_backpack/
--rw-r--r--   0 runner    (1001) docker     (127)    21588 2024-05-01 00:22:34.000000 zenodo_backpack-0.3.0/zenodo_backpack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-01 00:22:34.000000 zenodo_backpack-0.3.0/zenodo_backpack/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:50.776973 zenodo_backpack-0.3.0/zenodo_backpack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4924 2024-05-01 00:22:50.000000 zenodo_backpack-0.3.0/zenodo_backpack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-01 00:22:50.000000 zenodo_backpack-0.3.0/zenodo_backpack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 00:22:50.000000 zenodo_backpack-0.3.0/zenodo_backpack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-01 00:22:50.000000 zenodo_backpack-0.3.0/zenodo_backpack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-01 00:22:50.000000 zenodo_backpack-0.3.0/zenodo_backpack.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:54:28.653165 zenodo_backpack-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-03 06:54:19.000000 zenodo_backpack-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4924 2024-06-03 06:54:28.653165 zenodo_backpack-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4214 2024-06-03 06:54:19.000000 zenodo_backpack-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:54:28.653165 zenodo_backpack-0.3.1/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5686 2024-06-03 06:54:19.000000 zenodo_backpack-0.3.1/bin/zenodo_backpack
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 06:54:28.657165 zenodo_backpack-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-06-03 06:54:19.000000 zenodo_backpack-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:54:28.653165 zenodo_backpack-0.3.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-06-03 06:54:19.000000 zenodo_backpack-0.3.1/test/test_downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:54:28.653165 zenodo_backpack-0.3.1/zenodo_backpack/
+-rw-r--r--   0 runner    (1001) docker     (127)    22138 2024-06-03 06:54:19.000000 zenodo_backpack-0.3.1/zenodo_backpack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-06-03 06:54:19.000000 zenodo_backpack-0.3.1/zenodo_backpack/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:54:28.653165 zenodo_backpack-0.3.1/zenodo_backpack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4924 2024-06-03 06:54:28.000000 zenodo_backpack-0.3.1/zenodo_backpack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-06-03 06:54:28.000000 zenodo_backpack-0.3.1/zenodo_backpack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 06:54:28.000000 zenodo_backpack-0.3.1/zenodo_backpack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-06-03 06:54:28.000000 zenodo_backpack-0.3.1/zenodo_backpack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-06-03 06:54:28.000000 zenodo_backpack-0.3.1/zenodo_backpack.egg-info/top_level.txt
```

### Comparing `zenodo_backpack-0.3.0/LICENSE` & `zenodo_backpack-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zenodo_backpack-0.3.0/PKG-INFO` & `zenodo_backpack-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zenodo_backpack
-Version: 0.3.0
+Version: 0.3.1
 Summary: Manage data bundled with bioinformatic software through Zenodo DOI integration
 Home-page: https://github.com/centre-for-microbiome-research/zenodo_backpack
 Author: ['Alex Chklovski', 'Ben Woodcroft']
 Author-email: chklovski@gmail.com
 License: GPL3+
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `zenodo_backpack-0.3.0/README.md` & `zenodo_backpack-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `zenodo_backpack-0.3.0/bin/zenodo_backpack` & `zenodo_backpack-0.3.1/bin/zenodo_backpack`

 * *Files identical despite different names*

### Comparing `zenodo_backpack-0.3.0/setup.py` & `zenodo_backpack-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `zenodo_backpack-0.3.0/zenodo_backpack/__init__.py` & `zenodo_backpack-0.3.1/zenodo_backpack/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,16 +197,17 @@
                 logging.debug('All files have been downloaded.')
 
         else:
             raise ZenodoConnectionException('Record could not get accessed.')
 
         # unzip
         # use md5sums.txt file created from metadata to get files
-        downloaded_files = [[str(i) for i in line.strip().split(',')] for line in
-                            open(os.path.join(directory, 'md5sums.txt'), 'r').readlines()]
+        with open(os.path.join(directory, 'md5sums.txt')) as f:
+            downloaded_files = [[str(i) for i in line.strip().split(',')] for line in
+                                f.readlines()]
         zipped_files = [item for sublist in downloaded_files for item in sublist if '.tar.gz' in item]
 
         logging.info('Extracting files from archive...')
         for f in zipped_files:
             filepath = (os.path.join(directory, f))
             logging.debug('Extracting {}'.format(filepath))
             tf = tarfile.open(filepath)
@@ -340,16 +341,24 @@
             r = requests.get(records_url + recordID + '/versions', timeout=15.)
         except Exception as e:
             raise ZenodoConnectionException('Error during metadata retrieval: {}'.format(e))
 
         js = json.loads(r.text)
         versions = js['hits']['hits']
         for v in versions:
+            if 'version' not in v['metadata']:
+                if 'doi' in v['metadata']:
+                    bad_doi = v['metadata']['doi']
+                else:
+                    bad_doi = '???'
+                logging.warning(f'Version not found in Zenodo record {bad_doi}. Is the version specified in the record\'s metadata? The authors can update this. But here, skipping this instance.')
+                continue
             if v['metadata']['version'] == version:
                 return v
+        raise ZenodoBackpackVersionException(f'Version {version} not found in Zenodo record {recordID}')
 
     def _retrieve_record_metadata(self, recordID, version):
         """Parses provided recordID to access Zenodo API records and download metadata json
         Arguments:
             recordID (str): Zenodo record number
             version: (None or str): If None, return the newest version. If specified, target that specific version.
         Returns:
```

### Comparing `zenodo_backpack-0.3.0/zenodo_backpack.egg-info/PKG-INFO` & `zenodo_backpack-0.3.1/zenodo_backpack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zenodo_backpack
-Version: 0.3.0
+Version: 0.3.1
 Summary: Manage data bundled with bioinformatic software through Zenodo DOI integration
 Home-page: https://github.com/centre-for-microbiome-research/zenodo_backpack
 Author: ['Alex Chklovski', 'Ben Woodcroft']
 Author-email: chklovski@gmail.com
 License: GPL3+
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Scientific/Engineering
```

