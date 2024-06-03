# Comparing `tmp/tf_nightly-2.17.0.dev20240602-cp39-cp39-win_amd64.whl.zip` & `tmp/tf_nightly-2.17.0.dev20240603-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
 Zip file size: 2172 bytes, number of entries: 4
--rw-rw-r--  2.0 unx     3263 b- defN 24-Jun-02 07:57 tf_nightly-2.17.0.dev20240602.dist-info/METADATA
--rw-rw-r--  2.0 unx       99 b- defN 24-Jun-02 07:57 tf_nightly-2.17.0.dev20240602.dist-info/WHEEL
--rw-rw-r--  2.0 unx        1 b- defN 24-Jun-02 07:57 tf_nightly-2.17.0.dev20240602.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      361 b- defN 24-Jun-02 07:57 tf_nightly-2.17.0.dev20240602.dist-info/RECORD
+-rw-rw-r--  2.0 unx     3263 b- defN 24-Jun-03 07:59 tf_nightly-2.17.0.dev20240603.dist-info/METADATA
+-rw-rw-r--  2.0 unx       99 b- defN 24-Jun-03 07:59 tf_nightly-2.17.0.dev20240603.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        1 b- defN 24-Jun-03 07:59 tf_nightly-2.17.0.dev20240603.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      361 b- defN 24-Jun-03 07:59 tf_nightly-2.17.0.dev20240603.dist-info/RECORD
 4 files, 3724 bytes uncompressed, 1462 bytes compressed:  60.7%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: tf_nightly-2.17.0.dev20240602.dist-info/METADATA
+Filename: tf_nightly-2.17.0.dev20240603.dist-info/METADATA
 Comment: 
 
-Filename: tf_nightly-2.17.0.dev20240602.dist-info/WHEEL
+Filename: tf_nightly-2.17.0.dev20240603.dist-info/WHEEL
 Comment: 
 
-Filename: tf_nightly-2.17.0.dev20240602.dist-info/top_level.txt
+Filename: tf_nightly-2.17.0.dev20240603.dist-info/top_level.txt
 Comment: 
 
-Filename: tf_nightly-2.17.0.dev20240602.dist-info/RECORD
+Filename: tf_nightly-2.17.0.dev20240603.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `tf_nightly-2.17.0.dev20240602.dist-info/METADATA` & `tf_nightly-2.17.0.dev20240603.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tf-nightly
-Version: 2.17.0.dev20240602
+Version: 2.17.0.dev20240603
 Summary: TensorFlow is an open source machine learning framework for everyone.
 Home-page: https://www.tensorflow.org/
 Author: Google Inc.
 Author-email: packages@tensorflow.org
 License: Apache 2.0
 Download-URL: https://github.com/tensorflow/tensorflow/tags
 Keywords: tensorflow tensor machine learning
@@ -26,15 +26,15 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: tf-nightly-intel ==2.17.0-dev20240602 ; platform_system == "Windows"
+Requires-Dist: tf-nightly-intel ==2.17.0-dev20240603 ; platform_system == "Windows"
 Provides-Extra: and-cuda
 Requires-Dist: nvidia-cublas-cu12 ==12.3.4.1 ; extra == 'and-cuda'
 Requires-Dist: nvidia-cuda-cupti-cu12 ==12.3.101 ; extra == 'and-cuda'
 Requires-Dist: nvidia-cuda-nvcc-cu12 ==12.3.107 ; extra == 'and-cuda'
 Requires-Dist: nvidia-cuda-nvrtc-cu12 ==12.3.107 ; extra == 'and-cuda'
 Requires-Dist: nvidia-cuda-runtime-cu12 ==12.3.101 ; extra == 'and-cuda'
 Requires-Dist: nvidia-cudnn-cu12 ==8.9.7.29 ; extra == 'and-cuda'
```

