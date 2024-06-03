# Comparing `tmp/gen_vm_image-0.0.1a1.tar.gz` & `tmp/gen_vm_image-0.0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen_vm_image-0.0.1a1.tar", last modified: Mon May 27 18:54:50 2024, max compression
+gzip compressed data, was "gen_vm_image-0.0.1a2.tar", last modified: Mon Jun  3 10:01:58 2024, max compression
```

## Comparing `gen_vm_image-0.0.1a1.tar` & `gen_vm_image-0.0.1a2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-sr-x   0 go        (1000) root         (0)        0 2024-05-27 18:54:50.267986 gen_vm_image-0.0.1a1/
--rw-r--r--   0 go        (1000) root         (0)     5391 2024-05-27 18:54:50.267986 gen_vm_image-0.0.1a1/PKG-INFO
--rw-r--r--   0 go        (1000) root         (0)     4324 2024-05-27 18:54:35.000000 gen_vm_image-0.0.1a1/README.rst
-drwxr-sr-x   0 go        (1000) root         (0)        0 2024-05-27 18:54:50.263986 gen_vm_image-0.0.1a1/gen_vm_image/
--rw-r--r--   0 go        (1000) root         (0)        0 2024-05-27 18:54:35.000000 gen_vm_image-0.0.1a1/gen_vm_image/__init__.py
--rw-r--r--   0 go        (1000) root         (0)     1557 2024-05-27 18:54:35.000000 gen_vm_image-0.0.1a1/gen_vm_image/architecture.py
-drwxr-sr-x   0 go        (1000) root         (0)        0 2024-05-27 18:54:50.264986 gen_vm_image-0.0.1a1/gen_vm_image/cli/
--rw-r--r--   0 go        (1000) root         (0)        0 2024-05-27 18:54:35.000000 gen_vm_image-0.0.1a1/gen_vm_image/cli/__init__.py
--rw-r--r--   0 go        (1000) root         (0)    15468 2024-05-27 18:54:35.000000 gen_vm_image-0.0.1a1/gen_vm_image/cli/build_image.py
-drwxr-sr-x   0 go        (1000) root         (0)        0 2024-05-27 18:54:50.265986 gen_vm_image-0.0.1a1/gen_vm_image/common/
--rw-r--r--   0 go        (1000) root         (0)        0 2024-05-27 18:54:35.000000 gen_vm_image-0.0.1a1/gen_vm_image/common/__init__.py
--rw-r--r--   0 go        (1000) root         (0)      362 2024-05-27 18:54:35.000000 gen_vm_image-0.0.1a1/gen_vm_image/common/defaults.py
--rw-r--r--   0 go        (1000) root         (0)      611 2024-05-27 18:54:35.000000 gen_vm_image-0.0.1a1/gen_vm_image/common/errors.py
-drwxr-sr-x   0 go        (1000) root         (0)        0 2024-05-27 18:54:50.266986 gen_vm_image-0.0.1a1/gen_vm_image/utils/
--rw-r--r--   0 go        (1000) root         (0)        0 2024-05-27 18:54:35.000000 gen_vm_image-0.0.1a1/gen_vm_image/utils/__init__.py
--rw-r--r--   0 go        (1000) root         (0)     3939 2024-05-27 18:54:35.000000 gen_vm_image-0.0.1a1/gen_vm_image/utils/io.py
--rw-r--r--   0 go        (1000) root         (0)     1623 2024-05-27 18:54:35.000000 gen_vm_image-0.0.1a1/gen_vm_image/utils/job.py
--rw-r--r--   0 go        (1000) root         (0)      491 2024-05-27 18:54:35.000000 gen_vm_image-0.0.1a1/gen_vm_image/utils/net.py
--rw-r--r--   0 go        (1000) root         (0)      759 2024-05-27 18:54:35.000000 gen_vm_image-0.0.1a1/gen_vm_image/utils/user.py
-drwxr-sr-x   0 go        (1000) root         (0)        0 2024-05-27 18:54:50.266986 gen_vm_image-0.0.1a1/gen_vm_image.egg-info/
--rw-r--r--   0 go        (1000) root         (0)     5391 2024-05-27 18:54:50.000000 gen_vm_image-0.0.1a1/gen_vm_image.egg-info/PKG-INFO
--rw-r--r--   0 go        (1000) root         (0)      640 2024-05-27 18:54:50.000000 gen_vm_image-0.0.1a1/gen_vm_image.egg-info/SOURCES.txt
--rw-r--r--   0 go        (1000) root         (0)        1 2024-05-27 18:54:50.000000 gen_vm_image-0.0.1a1/gen_vm_image.egg-info/dependency_links.txt
--rw-r--r--   0 go        (1000) root         (0)       66 2024-05-27 18:54:50.000000 gen_vm_image-0.0.1a1/gen_vm_image.egg-info/entry_points.txt
--rw-r--r--   0 go        (1000) root         (0)      109 2024-05-27 18:54:50.000000 gen_vm_image-0.0.1a1/gen_vm_image.egg-info/requires.txt
--rw-r--r--   0 go        (1000) root         (0)       13 2024-05-27 18:54:50.000000 gen_vm_image-0.0.1a1/gen_vm_image.egg-info/top_level.txt
--rw-r--r--   0 go        (1000) root         (0)       38 2024-05-27 18:54:50.267986 gen_vm_image-0.0.1a1/setup.cfg
--rw-r--r--   0 go        (1000) root         (0)     1690 2024-05-27 18:54:35.000000 gen_vm_image-0.0.1a1/setup.py
-drwxr-sr-x   0 go        (1000) root         (0)        0 2024-05-27 18:54:50.266986 gen_vm_image-0.0.1a1/tests/
--rw-r--r--   0 go        (1000) root         (0)     3324 2024-05-27 18:54:35.000000 gen_vm_image-0.0.1a1/tests/test_image_architecture.py
--rw-r--r--   0 go        (1000) root         (0)     2781 2024-05-27 18:54:35.000000 gen_vm_image-0.0.1a1/tests/test_image_build.py
+drwxr-sr-x   0 go        (1000) root         (0)        0 2024-06-03 10:01:58.940759 gen_vm_image-0.0.1a2/
+-rw-r--r--   0 go        (1000) root         (0)     5391 2024-06-03 10:01:58.940759 gen_vm_image-0.0.1a2/PKG-INFO
+-rw-r--r--   0 go        (1000) root         (0)     4324 2024-06-03 10:01:48.000000 gen_vm_image-0.0.1a2/README.rst
+drwxr-sr-x   0 go        (1000) root         (0)        0 2024-06-03 10:01:58.936759 gen_vm_image-0.0.1a2/gen_vm_image/
+-rw-r--r--   0 go        (1000) root         (0)        0 2024-06-03 10:01:48.000000 gen_vm_image-0.0.1a2/gen_vm_image/__init__.py
+-rw-r--r--   0 go        (1000) root         (0)     1557 2024-06-03 10:01:48.000000 gen_vm_image-0.0.1a2/gen_vm_image/architecture.py
+drwxr-sr-x   0 go        (1000) root         (0)        0 2024-06-03 10:01:58.938759 gen_vm_image-0.0.1a2/gen_vm_image/cli/
+-rw-r--r--   0 go        (1000) root         (0)        0 2024-06-03 10:01:48.000000 gen_vm_image-0.0.1a2/gen_vm_image/cli/__init__.py
+-rw-r--r--   0 go        (1000) root         (0)    15468 2024-06-03 10:01:48.000000 gen_vm_image-0.0.1a2/gen_vm_image/cli/build_image.py
+drwxr-sr-x   0 go        (1000) root         (0)        0 2024-06-03 10:01:58.938759 gen_vm_image-0.0.1a2/gen_vm_image/common/
+-rw-r--r--   0 go        (1000) root         (0)        0 2024-06-03 10:01:48.000000 gen_vm_image-0.0.1a2/gen_vm_image/common/__init__.py
+-rw-r--r--   0 go        (1000) root         (0)      362 2024-06-03 10:01:48.000000 gen_vm_image-0.0.1a2/gen_vm_image/common/defaults.py
+-rw-r--r--   0 go        (1000) root         (0)      611 2024-06-03 10:01:48.000000 gen_vm_image-0.0.1a2/gen_vm_image/common/errors.py
+drwxr-sr-x   0 go        (1000) root         (0)        0 2024-06-03 10:01:58.939759 gen_vm_image-0.0.1a2/gen_vm_image/utils/
+-rw-r--r--   0 go        (1000) root         (0)        0 2024-06-03 10:01:48.000000 gen_vm_image-0.0.1a2/gen_vm_image/utils/__init__.py
+-rw-r--r--   0 go        (1000) root         (0)     3939 2024-06-03 10:01:48.000000 gen_vm_image-0.0.1a2/gen_vm_image/utils/io.py
+-rw-r--r--   0 go        (1000) root         (0)     1623 2024-06-03 10:01:48.000000 gen_vm_image-0.0.1a2/gen_vm_image/utils/job.py
+-rw-r--r--   0 go        (1000) root         (0)      704 2024-06-03 10:01:48.000000 gen_vm_image-0.0.1a2/gen_vm_image/utils/net.py
+-rw-r--r--   0 go        (1000) root         (0)      759 2024-06-03 10:01:48.000000 gen_vm_image-0.0.1a2/gen_vm_image/utils/user.py
+drwxr-sr-x   0 go        (1000) root         (0)        0 2024-06-03 10:01:58.939759 gen_vm_image-0.0.1a2/gen_vm_image.egg-info/
+-rw-r--r--   0 go        (1000) root         (0)     5391 2024-06-03 10:01:58.000000 gen_vm_image-0.0.1a2/gen_vm_image.egg-info/PKG-INFO
+-rw-r--r--   0 go        (1000) root         (0)      640 2024-06-03 10:01:58.000000 gen_vm_image-0.0.1a2/gen_vm_image.egg-info/SOURCES.txt
+-rw-r--r--   0 go        (1000) root         (0)        1 2024-06-03 10:01:58.000000 gen_vm_image-0.0.1a2/gen_vm_image.egg-info/dependency_links.txt
+-rw-r--r--   0 go        (1000) root         (0)       66 2024-06-03 10:01:58.000000 gen_vm_image-0.0.1a2/gen_vm_image.egg-info/entry_points.txt
+-rw-r--r--   0 go        (1000) root         (0)      109 2024-06-03 10:01:58.000000 gen_vm_image-0.0.1a2/gen_vm_image.egg-info/requires.txt
+-rw-r--r--   0 go        (1000) root         (0)       13 2024-06-03 10:01:58.000000 gen_vm_image-0.0.1a2/gen_vm_image.egg-info/top_level.txt
+-rw-r--r--   0 go        (1000) root         (0)       38 2024-06-03 10:01:58.940759 gen_vm_image-0.0.1a2/setup.cfg
+-rw-r--r--   0 go        (1000) root         (0)     1690 2024-06-03 10:01:48.000000 gen_vm_image-0.0.1a2/setup.py
+drwxr-sr-x   0 go        (1000) root         (0)        0 2024-06-03 10:01:58.939759 gen_vm_image-0.0.1a2/tests/
+-rw-r--r--   0 go        (1000) root         (0)     3324 2024-06-03 10:01:48.000000 gen_vm_image-0.0.1a2/tests/test_image_architecture.py
+-rw-r--r--   0 go        (1000) root         (0)     2862 2024-06-03 10:01:48.000000 gen_vm_image-0.0.1a2/tests/test_image_build.py
```

### Comparing `gen_vm_image-0.0.1a1/PKG-INFO` & `gen_vm_image-0.0.1a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen-vm-image
-Version: 0.0.1a1
+Version: 0.0.1a2
 Summary: This tool can be used for generating virtual machine images.
 Home-page: https://github.com/ucphhpc/gen-vm-image
 Author: Rasmus Munk
 Author-email: munk1@live.dk
 License: MIT
 Keywords: Virtual Machine,VM,Images
 Classifier: Intended Audience :: Developers
```

### Comparing `gen_vm_image-0.0.1a1/README.rst` & `gen_vm_image-0.0.1a2/README.rst`

 * *Files identical despite different names*

### Comparing `gen_vm_image-0.0.1a1/gen_vm_image/architecture.py` & `gen_vm_image-0.0.1a2/gen_vm_image/architecture.py`

 * *Files identical despite different names*

### Comparing `gen_vm_image-0.0.1a1/gen_vm_image/cli/build_image.py` & `gen_vm_image-0.0.1a2/gen_vm_image/cli/build_image.py`

 * *Files identical despite different names*

### Comparing `gen_vm_image-0.0.1a1/gen_vm_image/common/errors.py` & `gen_vm_image-0.0.1a2/gen_vm_image/common/errors.py`

 * *Files identical despite different names*

### Comparing `gen_vm_image-0.0.1a1/gen_vm_image/utils/io.py` & `gen_vm_image-0.0.1a2/gen_vm_image/utils/io.py`

 * *Files identical despite different names*

### Comparing `gen_vm_image-0.0.1a1/gen_vm_image/utils/job.py` & `gen_vm_image-0.0.1a2/gen_vm_image/utils/job.py`

 * *Files identical despite different names*

### Comparing `gen_vm_image-0.0.1a1/gen_vm_image/utils/user.py` & `gen_vm_image-0.0.1a2/gen_vm_image/utils/user.py`

 * *Files identical despite different names*

### Comparing `gen_vm_image-0.0.1a1/gen_vm_image.egg-info/PKG-INFO` & `gen_vm_image-0.0.1a2/gen_vm_image.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen-vm-image
-Version: 0.0.1a1
+Version: 0.0.1a2
 Summary: This tool can be used for generating virtual machine images.
 Home-page: https://github.com/ucphhpc/gen-vm-image
 Author: Rasmus Munk
 Author-email: munk1@live.dk
 License: MIT
 Keywords: Virtual Machine,VM,Images
 Classifier: Intended Audience :: Developers
```

### Comparing `gen_vm_image-0.0.1a1/gen_vm_image.egg-info/SOURCES.txt` & `gen_vm_image-0.0.1a2/gen_vm_image.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gen_vm_image-0.0.1a1/setup.py` & `gen_vm_image-0.0.1a2/setup.py`

 * *Files identical despite different names*

### Comparing `gen_vm_image-0.0.1a1/tests/test_image_architecture.py` & `gen_vm_image-0.0.1a2/tests/test_image_architecture.py`

 * *Files identical despite different names*

### Comparing `gen_vm_image-0.0.1a1/tests/test_image_build.py` & `gen_vm_image-0.0.1a2/tests/test_image_build.py`

 * *Files 9% similar despite different names*

```diff
@@ -65,7 +65,8 @@
             output_format=debian_12["format"],
         )
         self.assertNotIsInstance(result, int)
         self.assertIsInstance(result, dict)
         self.assertEqual(result["returncode"], "0")
         self.assertIsNone(msg)
         self.assertTrue(exists(output_path))
+        # TODO, validate that the output image is of the correct size and format
```

