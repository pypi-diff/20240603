# Comparing `tmp/imageio-ffmpeg-0.5.0.tar.gz` & `tmp/imageio-ffmpeg-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imageio-ffmpeg-0.5.0.tar", last modified: Fri May 31 18:56:27 2024, max compression
+gzip compressed data, was "imageio-ffmpeg-0.5.1.tar", last modified: Mon Jun  3 15:11:44 2024, max compression
```

## Comparing `imageio-ffmpeg-0.5.0.tar` & `imageio-ffmpeg-0.5.1.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 almar      (501) staff       (20)        0 2024-05-31 18:56:27.209455 imageio-ffmpeg-0.5.0/
--rw-r--r--   0 almar      (501) staff       (20)     1312 2022-01-25 10:14:00.000000 imageio-ffmpeg-0.5.0/LICENSE
--rw-r--r--   0 almar      (501) staff       (20)       70 2024-03-08 09:37:49.000000 imageio-ffmpeg-0.5.0/MANIFEST.in
--rw-r--r--   0 almar      (501) staff       (20)     1577 2024-05-31 18:56:27.209336 imageio-ffmpeg-0.5.0/PKG-INFO
--rw-r--r--   0 almar      (501) staff       (20)     9941 2024-05-31 18:56:13.000000 imageio-ffmpeg-0.5.0/README.md
-drwxr-xr-x   0 almar      (501) staff       (20)        0 2024-05-31 18:56:27.206748 imageio-ffmpeg-0.5.0/imageio_ffmpeg/
--rw-r--r--   0 almar      (501) staff       (20)      227 2023-09-11 13:59:57.000000 imageio-ffmpeg-0.5.0/imageio_ffmpeg/__init__.py
--rw-r--r--   0 almar      (501) staff       (20)     1739 2024-05-31 18:55:04.000000 imageio-ffmpeg-0.5.0/imageio_ffmpeg/_definitions.py
--rw-r--r--   0 almar      (501) staff       (20)    27048 2024-05-31 18:53:29.000000 imageio-ffmpeg-0.5.0/imageio_ffmpeg/_io.py
--rw-r--r--   0 almar      (501) staff       (20)     6840 2023-09-12 09:52:53.000000 imageio-ffmpeg-0.5.0/imageio_ffmpeg/_parsing.py
--rw-r--r--   0 almar      (501) staff       (20)     3833 2024-03-08 09:37:49.000000 imageio-ffmpeg-0.5.0/imageio_ffmpeg/_utils.py
-drwxr-xr-x   0 almar      (501) staff       (20)        0 2024-05-31 18:56:27.209040 imageio-ffmpeg-0.5.0/imageio_ffmpeg/binaries/
--rw-r--r--   0 almar      (501) staff       (20)       45 2022-01-25 10:14:00.000000 imageio-ffmpeg-0.5.0/imageio_ffmpeg/binaries/README.md
-drwxr-xr-x   0 almar      (501) staff       (20)        0 2024-05-31 18:56:27.208835 imageio-ffmpeg-0.5.0/imageio_ffmpeg.egg-info/
--rw-r--r--   0 almar      (501) staff       (20)     1577 2024-05-31 18:56:27.000000 imageio-ffmpeg-0.5.0/imageio_ffmpeg.egg-info/PKG-INFO
--rw-r--r--   0 almar      (501) staff       (20)      430 2024-05-31 18:56:27.000000 imageio-ffmpeg-0.5.0/imageio_ffmpeg.egg-info/SOURCES.txt
--rw-r--r--   0 almar      (501) staff       (20)        1 2024-05-31 18:56:27.000000 imageio-ffmpeg-0.5.0/imageio_ffmpeg.egg-info/dependency_links.txt
--rw-r--r--   0 almar      (501) staff       (20)        1 2024-05-31 18:56:27.000000 imageio-ffmpeg-0.5.0/imageio_ffmpeg.egg-info/not-zip-safe
--rw-r--r--   0 almar      (501) staff       (20)       11 2024-05-31 18:56:27.000000 imageio-ffmpeg-0.5.0/imageio_ffmpeg.egg-info/requires.txt
--rw-r--r--   0 almar      (501) staff       (20)       15 2024-05-31 18:56:27.000000 imageio-ffmpeg-0.5.0/imageio_ffmpeg.egg-info/top_level.txt
--rw-r--r--   0 almar      (501) staff       (20)       38 2024-05-31 18:56:27.209497 imageio-ffmpeg-0.5.0/setup.cfg
--rw-r--r--   0 almar      (501) staff       (20)     2677 2024-05-31 18:53:29.000000 imageio-ffmpeg-0.5.0/setup.py
+drwxr-xr-x   0 almar      (501) staff       (20)        0 2024-06-03 15:11:44.855936 imageio-ffmpeg-0.5.1/
+-rw-r--r--   0 almar      (501) staff       (20)     1312 2022-01-25 10:14:00.000000 imageio-ffmpeg-0.5.1/LICENSE
+-rw-r--r--   0 almar      (501) staff       (20)       70 2024-03-08 09:37:49.000000 imageio-ffmpeg-0.5.1/MANIFEST.in
+-rw-r--r--   0 almar      (501) staff       (20)     1577 2024-06-03 15:11:44.855819 imageio-ffmpeg-0.5.1/PKG-INFO
+-rw-r--r--   0 almar      (501) staff       (20)     9941 2024-05-31 18:56:13.000000 imageio-ffmpeg-0.5.1/README.md
+drwxr-xr-x   0 almar      (501) staff       (20)        0 2024-06-03 15:11:44.854154 imageio-ffmpeg-0.5.1/imageio_ffmpeg/
+-rw-r--r--   0 almar      (501) staff       (20)      227 2023-09-11 13:59:57.000000 imageio-ffmpeg-0.5.1/imageio_ffmpeg/__init__.py
+-rw-r--r--   0 almar      (501) staff       (20)     1739 2024-06-03 15:11:16.000000 imageio-ffmpeg-0.5.1/imageio_ffmpeg/_definitions.py
+-rw-r--r--   0 almar      (501) staff       (20)    27048 2024-05-31 18:53:29.000000 imageio-ffmpeg-0.5.1/imageio_ffmpeg/_io.py
+-rw-r--r--   0 almar      (501) staff       (20)     6840 2023-09-12 09:52:53.000000 imageio-ffmpeg-0.5.1/imageio_ffmpeg/_parsing.py
+-rw-r--r--   0 almar      (501) staff       (20)     3833 2024-03-08 09:37:49.000000 imageio-ffmpeg-0.5.1/imageio_ffmpeg/_utils.py
+drwxr-xr-x   0 almar      (501) staff       (20)        0 2024-06-03 15:11:44.855526 imageio-ffmpeg-0.5.1/imageio_ffmpeg/binaries/
+-rw-r--r--   0 almar      (501) staff       (20)       45 2022-01-25 10:14:00.000000 imageio-ffmpeg-0.5.1/imageio_ffmpeg/binaries/README.md
+-rw-r--r--   0 almar      (501) staff       (20)       45 2024-06-03 15:05:44.000000 imageio-ffmpeg-0.5.1/imageio_ffmpeg/binaries/__init__.py
+drwxr-xr-x   0 almar      (501) staff       (20)        0 2024-06-03 15:11:44.855129 imageio-ffmpeg-0.5.1/imageio_ffmpeg.egg-info/
+-rw-r--r--   0 almar      (501) staff       (20)     1577 2024-06-03 15:11:44.000000 imageio-ffmpeg-0.5.1/imageio_ffmpeg.egg-info/PKG-INFO
+-rw-r--r--   0 almar      (501) staff       (20)      466 2024-06-03 15:11:44.000000 imageio-ffmpeg-0.5.1/imageio_ffmpeg.egg-info/SOURCES.txt
+-rw-r--r--   0 almar      (501) staff       (20)        1 2024-06-03 15:11:44.000000 imageio-ffmpeg-0.5.1/imageio_ffmpeg.egg-info/dependency_links.txt
+-rw-r--r--   0 almar      (501) staff       (20)        1 2024-06-03 15:11:44.000000 imageio-ffmpeg-0.5.1/imageio_ffmpeg.egg-info/not-zip-safe
+-rw-r--r--   0 almar      (501) staff       (20)       11 2024-06-03 15:11:44.000000 imageio-ffmpeg-0.5.1/imageio_ffmpeg.egg-info/requires.txt
+-rw-r--r--   0 almar      (501) staff       (20)       15 2024-06-03 15:11:44.000000 imageio-ffmpeg-0.5.1/imageio_ffmpeg.egg-info/top_level.txt
+-rw-r--r--   0 almar      (501) staff       (20)       38 2024-06-03 15:11:44.855976 imageio-ffmpeg-0.5.1/setup.cfg
+-rw-r--r--   0 almar      (501) staff       (20)     2698 2024-06-03 15:11:07.000000 imageio-ffmpeg-0.5.1/setup.py
```

### Comparing `imageio-ffmpeg-0.5.0/LICENSE` & `imageio-ffmpeg-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `imageio-ffmpeg-0.5.0/PKG-INFO` & `imageio-ffmpeg-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imageio-ffmpeg
-Version: 0.5.0
+Version: 0.5.1
 Summary: FFMPEG wrapper for Python
 Home-page: https://github.com/imageio/imageio-ffmpeg
 Download-URL: http://pypi.python.org/pypi/imageio-ffmpeg
 Author: imageio contributors
 Author-email: almar.klein@gmail.com
 License: BSD-2-Clause
 Keywords: video ffmpeg
```

### Comparing `imageio-ffmpeg-0.5.0/README.md` & `imageio-ffmpeg-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `imageio-ffmpeg-0.5.0/imageio_ffmpeg/_definitions.py` & `imageio-ffmpeg-0.5.1/imageio_ffmpeg/_definitions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import platform
 import struct
 import sys
 
-__version__ = "0.5.0"
+__version__ = "0.5.1"
 
 
 def get_platform():
     bits = struct.calcsize("P") * 8
     if sys.platform.startswith("linux"):
         architecture = platform.machine()
         if architecture == "aarch64":
```

### Comparing `imageio-ffmpeg-0.5.0/imageio_ffmpeg/_io.py` & `imageio-ffmpeg-0.5.1/imageio_ffmpeg/_io.py`

 * *Files identical despite different names*

### Comparing `imageio-ffmpeg-0.5.0/imageio_ffmpeg/_parsing.py` & `imageio-ffmpeg-0.5.1/imageio_ffmpeg/_parsing.py`

 * *Files identical despite different names*

### Comparing `imageio-ffmpeg-0.5.0/imageio_ffmpeg/_utils.py` & `imageio-ffmpeg-0.5.1/imageio_ffmpeg/_utils.py`

 * *Files identical despite different names*

### Comparing `imageio-ffmpeg-0.5.0/imageio_ffmpeg.egg-info/PKG-INFO` & `imageio-ffmpeg-0.5.1/imageio_ffmpeg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imageio-ffmpeg
-Version: 0.5.0
+Version: 0.5.1
 Summary: FFMPEG wrapper for Python
 Home-page: https://github.com/imageio/imageio-ffmpeg
 Download-URL: http://pypi.python.org/pypi/imageio-ffmpeg
 Author: imageio contributors
 Author-email: almar.klein@gmail.com
 License: BSD-2-Clause
 Keywords: video ffmpeg
```

### Comparing `imageio-ffmpeg-0.5.0/setup.py` & `imageio-ffmpeg-0.5.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     raise RuntimeError("Running setup.py upload is not the proper release procedure!")
 
 
 # If making a source dist, clear the binaries directory
 if "sdist" in sys.argv:
     target_dir = os.path.abspath(os.path.join(this_dir, "imageio_ffmpeg", "binaries"))
     for fname in os.listdir(target_dir):
-        if fname != "README.md":
+        if fname not in ["README.md", "__init__.py"]:
             os.remove(os.path.join(target_dir, fname))
 
 
 long_description = """
 FFMPEG wrapper for Python.
 
 Note that the platform-specific wheels contain the binary executable
```

