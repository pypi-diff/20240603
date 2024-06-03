# Comparing `tmp/multiclass_interface-1.6.tar.gz` & `tmp/multiclass_interface-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multiclass_interface-1.6.tar", last modified: Mon Jun  3 10:08:12 2024, max compression
+gzip compressed data, was "multiclass_interface-1.7.tar", last modified: Mon Jun  3 11:31:58 2024, max compression
```

## Comparing `multiclass_interface-1.6.tar` & `multiclass_interface-1.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 10:08:12.614250 multiclass_interface-1.6/
--rw-rw-rw-   0 root         (0) root         (0)      141 2024-03-18 14:23:06.000000 multiclass_interface-1.6/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     2124 2024-05-24 05:52:15.000000 multiclass_interface-1.6/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1094 2024-03-19 07:05:00.000000 multiclass_interface-1.6/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 10:08:12.614250 multiclass_interface-1.6/Multiclass_interface.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1578 2024-06-03 10:08:12.000000 multiclass_interface-1.6/Multiclass_interface.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      718 2024-06-03 10:08:12.000000 multiclass_interface-1.6/Multiclass_interface.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-06-03 10:08:12.000000 multiclass_interface-1.6/Multiclass_interface.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2024-06-03 10:08:12.000000 multiclass_interface-1.6/Multiclass_interface.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2024-06-03 10:08:12.000000 multiclass_interface-1.6/Multiclass_interface.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1578 2024-06-03 10:08:12.614250 multiclass_interface-1.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      899 2024-03-19 07:07:38.000000 multiclass_interface-1.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 10:08:12.614250 multiclass_interface-1.6/multiclass_interface/
--rw-rw-rw-   0 root         (0) root         (0)      114 2024-03-18 12:26:49.000000 multiclass_interface-1.6/multiclass_interface/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6703 2024-06-03 09:59:32.000000 multiclass_interface-1.6/multiclass_interface/mpi_interface.py
--rw-rw-rw-   0 root         (0) root         (0)     2022 2024-03-18 19:36:25.000000 multiclass_interface-1.6/multiclass_interface/multi_object_list.py
--rw-rw-rw-   0 root         (0) root         (0)     8169 2024-03-21 09:39:37.000000 multiclass_interface-1.6/multiclass_interface/multiprocess_interface.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 10:08:12.614250 multiclass_interface-1.6/multiclass_interface/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-03 10:06:05.000000 multiclass_interface-1.6/multiclass_interface/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      826 2024-03-18 19:36:25.000000 multiclass_interface-1.6/multiclass_interface/tests/my_test_cls.py
--rw-rw-rw-   0 root         (0) root         (0)     2826 2024-05-28 09:44:04.000000 multiclass_interface-1.6/multiclass_interface/tests/test_mpi.py
--rw-rw-rw-   0 root         (0) root         (0)      515 2024-03-18 19:36:25.000000 multiclass_interface-1.6/multiclass_interface/tests/test_multiclass_list.py
--rw-rw-rw-   0 root         (0) root         (0)     3165 2024-03-21 09:39:37.000000 multiclass_interface-1.6/multiclass_interface/tests/test_multiprocessinterface.py
--rw-r--r--   0 root         (0) root         (0)      406 2024-06-03 10:08:12.000000 multiclass_interface-1.6/multiclass_interface/version.py
--rw-rw-rw-   0 root         (0) root         (0)     1179 2024-03-19 07:05:00.000000 multiclass_interface-1.6/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     6561 2024-05-28 10:04:03.000000 multiclass_interface-1.6/sequence_diagrams.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-06-03 10:08:12.614250 multiclass_interface-1.6/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:31:58.231079 multiclass_interface-1.7/
+-rw-rw-rw-   0 root         (0) root         (0)      141 2024-03-18 14:23:06.000000 multiclass_interface-1.7/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     2124 2024-05-24 05:52:15.000000 multiclass_interface-1.7/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1094 2024-03-19 07:05:00.000000 multiclass_interface-1.7/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:31:58.231079 multiclass_interface-1.7/Multiclass_interface.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1578 2024-06-03 11:31:58.000000 multiclass_interface-1.7/Multiclass_interface.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      718 2024-06-03 11:31:58.000000 multiclass_interface-1.7/Multiclass_interface.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-06-03 11:31:58.000000 multiclass_interface-1.7/Multiclass_interface.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2024-06-03 11:31:58.000000 multiclass_interface-1.7/Multiclass_interface.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2024-06-03 11:31:58.000000 multiclass_interface-1.7/Multiclass_interface.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1578 2024-06-03 11:31:58.231079 multiclass_interface-1.7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      899 2024-03-19 07:07:38.000000 multiclass_interface-1.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:31:58.199079 multiclass_interface-1.7/multiclass_interface/
+-rw-rw-rw-   0 root         (0) root         (0)      114 2024-03-18 12:26:49.000000 multiclass_interface-1.7/multiclass_interface/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6703 2024-06-03 11:30:26.000000 multiclass_interface-1.7/multiclass_interface/mpi_interface.py
+-rw-rw-rw-   0 root         (0) root         (0)     2022 2024-03-18 19:36:25.000000 multiclass_interface-1.7/multiclass_interface/multi_object_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     8169 2024-03-21 09:39:37.000000 multiclass_interface-1.7/multiclass_interface/multiprocess_interface.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:31:58.215079 multiclass_interface-1.7/multiclass_interface/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-03 11:30:27.000000 multiclass_interface-1.7/multiclass_interface/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      826 2024-03-18 19:36:25.000000 multiclass_interface-1.7/multiclass_interface/tests/my_test_cls.py
+-rw-rw-rw-   0 root         (0) root         (0)     2826 2024-06-03 11:30:26.000000 multiclass_interface-1.7/multiclass_interface/tests/test_mpi.py
+-rw-rw-rw-   0 root         (0) root         (0)      515 2024-03-18 19:36:25.000000 multiclass_interface-1.7/multiclass_interface/tests/test_multiclass_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     3165 2024-03-21 09:39:37.000000 multiclass_interface-1.7/multiclass_interface/tests/test_multiprocessinterface.py
+-rw-r--r--   0 root         (0) root         (0)      406 2024-06-03 11:31:58.000000 multiclass_interface-1.7/multiclass_interface/version.py
+-rw-rw-rw-   0 root         (0) root         (0)     1179 2024-03-19 07:05:00.000000 multiclass_interface-1.7/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     6561 2024-05-28 10:04:03.000000 multiclass_interface-1.7/sequence_diagrams.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-06-03 11:31:58.231079 multiclass_interface-1.7/setup.cfg
```

### Comparing `multiclass_interface-1.6/.gitlab-ci.yml` & `multiclass_interface-1.7/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `multiclass_interface-1.6/LICENSE` & `multiclass_interface-1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `multiclass_interface-1.6/Multiclass_interface.egg-info/PKG-INFO` & `multiclass_interface-1.7/Multiclass_interface.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Multiclass_interface
-Version: 1.6
+Version: 1.7
 Summary: Multiclass interface
 Author-email: "Mads M. Pedersen" <mmpe@dtu.dk>
 Project-URL: Homepage, https://gitlab.windenergy.dtu.dk/DYNAMIKS/multiclass_interface
 Project-URL: Bug Tracker, https://gitlab.windenergy.dtu.dk/DYNAMIKS/multiclass_interface/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `multiclass_interface-1.6/Multiclass_interface.egg-info/SOURCES.txt` & `multiclass_interface-1.7/Multiclass_interface.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `multiclass_interface-1.6/PKG-INFO` & `multiclass_interface-1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Multiclass_interface
-Version: 1.6
+Version: 1.7
 Summary: Multiclass interface
 Author-email: "Mads M. Pedersen" <mmpe@dtu.dk>
 Project-URL: Homepage, https://gitlab.windenergy.dtu.dk/DYNAMIKS/multiclass_interface
 Project-URL: Bug Tracker, https://gitlab.windenergy.dtu.dk/DYNAMIKS/multiclass_interface/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `multiclass_interface-1.6/README.md` & `multiclass_interface-1.7/README.md`

 * *Files identical despite different names*

### Comparing `multiclass_interface-1.6/multiclass_interface/mpi_interface.py` & `multiclass_interface-1.7/multiclass_interface/mpi_interface.py`

 * *Files identical despite different names*

### Comparing `multiclass_interface-1.6/multiclass_interface/multi_object_list.py` & `multiclass_interface-1.7/multiclass_interface/multi_object_list.py`

 * *Files identical despite different names*

### Comparing `multiclass_interface-1.6/multiclass_interface/multiprocess_interface.py` & `multiclass_interface-1.7/multiclass_interface/multiprocess_interface.py`

 * *Files identical despite different names*

### Comparing `multiclass_interface-1.6/multiclass_interface/tests/my_test_cls.py` & `multiclass_interface-1.7/multiclass_interface/tests/my_test_cls.py`

 * *Files identical despite different names*

### Comparing `multiclass_interface-1.6/multiclass_interface/tests/test_mpi.py` & `multiclass_interface-1.7/multiclass_interface/tests/test_mpi.py`

 * *Files identical despite different names*

### Comparing `multiclass_interface-1.6/multiclass_interface/tests/test_multiclass_list.py` & `multiclass_interface-1.7/multiclass_interface/tests/test_multiclass_list.py`

 * *Files identical despite different names*

### Comparing `multiclass_interface-1.6/multiclass_interface/tests/test_multiprocessinterface.py` & `multiclass_interface-1.7/multiclass_interface/tests/test_multiprocessinterface.py`

 * *Files identical despite different names*

### Comparing `multiclass_interface-1.6/pyproject.toml` & `multiclass_interface-1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `multiclass_interface-1.6/sequence_diagrams.md` & `multiclass_interface-1.7/sequence_diagrams.md`

 * *Files identical despite different names*

