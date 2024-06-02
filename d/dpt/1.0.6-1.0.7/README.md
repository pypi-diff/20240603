# Comparing `tmp/dpt-1.0.6.tar.gz` & `tmp/dpt-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dpt-1.0.6.tar", last modified: Sun Jun  2 19:32:03 2024, max compression
+gzip compressed data, was "dpt-1.0.7.tar", last modified: Sun Jun  2 20:12:52 2024, max compression
```

## Comparing `dpt-1.0.6.tar` & `dpt-1.0.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-06-02 19:32:03.032671 dpt-1.0.6/
--rw-rw-rw-   0        0        0      188 2024-06-02 19:32:03.031669 dpt-1.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-06-02 19:32:02.954392 dpt-1.0.6/dpt/
--rw-rw-rw-   0        0        0      123 2024-03-05 23:00:59.000000 dpt-1.0.6/dpt/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-02 19:32:03.016671 dpt-1.0.6/dpt/deployment/
--rw-rw-rw-   0        0        0        4 2024-02-01 03:57:26.000000 dpt-1.0.6/dpt/deployment/__init__.py
--rw-rw-rw-   0        0        0      110 2024-02-01 20:25:45.000000 dpt-1.0.6/dpt/deployment/common.py
--rw-rw-rw-   0        0        0     9539 2024-04-14 15:36:27.000000 dpt-1.0.6/dpt/deployment/deploy.py
--rw-rw-rw-   0        0        0     1054 2024-02-01 20:24:35.000000 dpt-1.0.6/dpt/deployment/extract.py
--rw-rw-rw-   0        0        0     1981 2024-02-01 20:24:46.000000 dpt-1.0.6/dpt/management.py
-drwxrwxrwx   0        0        0        0 2024-06-02 19:32:03.027670 dpt-1.0.6/dpt/mongo/
--rw-rw-rw-   0        0        0        4 2024-02-01 03:59:35.000000 dpt-1.0.6/dpt/mongo/__init__.py
--rw-rw-rw-   0        0        0      266 2024-01-27 22:13:49.000000 dpt-1.0.6/dpt/mongo/commands.py
--rw-rw-rw-   0        0        0     1032 2024-01-28 00:52:12.000000 dpt-1.0.6/dpt/mongo/files.py
--rw-rw-rw-   0        0        0    13690 2024-06-02 19:07:54.000000 dpt-1.0.6/dpt/processor.py
--rw-rw-rw-   0        0        0     8888 2024-06-02 19:30:53.000000 dpt-1.0.6/dpt/storage.py
-drwxrwxrwx   0        0        0        0 2024-06-02 19:32:03.000671 dpt-1.0.6/dpt.egg-info/
--rw-rw-rw-   0        0        0      188 2024-06-02 19:32:02.000000 dpt-1.0.6/dpt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2024-06-02 19:32:02.000000 dpt-1.0.6/dpt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 19:32:02.000000 dpt-1.0.6/dpt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-06-02 19:32:02.000000 dpt-1.0.6/dpt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-06-02 19:32:02.000000 dpt-1.0.6/dpt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-06-02 19:32:03.033671 dpt-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0      338 2024-06-02 19:31:58.000000 dpt-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 20:12:52.121158 dpt-1.0.7/
+-rw-rw-rw-   0        0        0      188 2024-06-02 20:12:52.119126 dpt-1.0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-06-02 20:12:52.044178 dpt-1.0.7/dpt/
+-rw-rw-rw-   0        0        0      123 2024-03-05 23:00:59.000000 dpt-1.0.7/dpt/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-02 20:12:52.102128 dpt-1.0.7/dpt/deployment/
+-rw-rw-rw-   0        0        0        4 2024-02-01 03:57:26.000000 dpt-1.0.7/dpt/deployment/__init__.py
+-rw-rw-rw-   0        0        0      110 2024-02-01 20:25:45.000000 dpt-1.0.7/dpt/deployment/common.py
+-rw-rw-rw-   0        0        0     9539 2024-04-14 15:36:27.000000 dpt-1.0.7/dpt/deployment/deploy.py
+-rw-rw-rw-   0        0        0     1054 2024-02-01 20:24:35.000000 dpt-1.0.7/dpt/deployment/extract.py
+-rw-rw-rw-   0        0        0     1981 2024-02-01 20:24:46.000000 dpt-1.0.7/dpt/management.py
+drwxrwxrwx   0        0        0        0 2024-06-02 20:12:52.115130 dpt-1.0.7/dpt/mongo/
+-rw-rw-rw-   0        0        0        4 2024-02-01 03:59:35.000000 dpt-1.0.7/dpt/mongo/__init__.py
+-rw-rw-rw-   0        0        0      266 2024-01-27 22:13:49.000000 dpt-1.0.7/dpt/mongo/commands.py
+-rw-rw-rw-   0        0        0     1032 2024-01-28 00:52:12.000000 dpt-1.0.7/dpt/mongo/files.py
+-rw-rw-rw-   0        0        0    13690 2024-06-02 19:07:54.000000 dpt-1.0.7/dpt/processor.py
+-rw-rw-rw-   0        0        0     8882 2024-06-02 20:12:36.000000 dpt-1.0.7/dpt/storage.py
+drwxrwxrwx   0        0        0        0 2024-06-02 20:12:52.086126 dpt-1.0.7/dpt.egg-info/
+-rw-rw-rw-   0        0        0      188 2024-06-02 20:12:51.000000 dpt-1.0.7/dpt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2024-06-02 20:12:51.000000 dpt-1.0.7/dpt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 20:12:51.000000 dpt-1.0.7/dpt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-06-02 20:12:51.000000 dpt-1.0.7/dpt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-06-02 20:12:51.000000 dpt-1.0.7/dpt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-02 20:12:52.122128 dpt-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      338 2024-06-02 20:12:47.000000 dpt-1.0.7/setup.py
```

### Comparing `dpt-1.0.6/dpt/deployment/deploy.py` & `dpt-1.0.7/dpt/deployment/deploy.py`

 * *Files identical despite different names*

### Comparing `dpt-1.0.6/dpt/deployment/extract.py` & `dpt-1.0.7/dpt/deployment/extract.py`

 * *Files identical despite different names*

### Comparing `dpt-1.0.6/dpt/management.py` & `dpt-1.0.7/dpt/management.py`

 * *Files identical despite different names*

### Comparing `dpt-1.0.6/dpt/mongo/files.py` & `dpt-1.0.7/dpt/mongo/files.py`

 * *Files identical despite different names*

### Comparing `dpt-1.0.6/dpt/processor.py` & `dpt-1.0.7/dpt/processor.py`

 * *Files identical despite different names*

### Comparing `dpt-1.0.6/dpt/storage.py` & `dpt-1.0.7/dpt/storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -243,15 +243,15 @@
             return
         for item in self._data:
             jsonschema.validate(instance=item, schema=self.schema)
 
     def get_count(self):
         return len(self._data)
 
-    def get_collection_name(self):
+    def get_coll_name(self):
         return None
 
     def get_info(self):
         return f"list[]"
 
     def read_all(self):
         self._validate()
```

