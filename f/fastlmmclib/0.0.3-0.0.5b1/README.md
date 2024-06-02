# Comparing `tmp/fastlmmclib-0.0.3-cp39-cp39-win_amd64.whl.zip` & `tmp/fastlmmclib-0.0.5b1-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 37288 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat      743 b- defN 23-Aug-09 00:07 fastlmmclib/quadform/__init__.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Aug-09 00:07 fastlmmclib/quadform/qfc_src/__init__.py
--rw-rw-rw-  2.0 fat    64512 b- defN 23-Aug-09 00:12 fastlmmclib/quadform/qfc_src/wrap_qfc.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat    11558 b- defN 23-Aug-09 00:12 fastlmmclib-0.0.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      929 b- defN 23-Aug-09 00:12 fastlmmclib-0.0.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Aug-09 00:12 fastlmmclib-0.0.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       62 b- defN 23-Aug-09 00:12 fastlmmclib-0.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      703 b- defN 23-Aug-09 00:12 fastlmmclib-0.0.3.dist-info/RECORD
-8 files, 78607 bytes uncompressed, 36044 bytes compressed:  54.1%
+Zip file size: 37170 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat      786 b- defN 24-Jun-02 18:48 fastlmmclib/quadform/__init__.py
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Jun-02 18:48 fastlmmclib/quadform/qfc_src/__init__.py
+-rw-rw-rw-  2.0 fat    65024 b- defN 24-Jun-02 18:50 fastlmmclib/quadform/qfc_src/wrap_qfc.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat    11558 b- defN 24-Jun-02 18:50 fastlmmclib-0.0.5b1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      934 b- defN 24-Jun-02 18:50 fastlmmclib-0.0.5b1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 24-Jun-02 18:50 fastlmmclib-0.0.5b1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       62 b- defN 24-Jun-02 18:50 fastlmmclib-0.0.5b1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      713 b- defN 24-Jun-02 18:50 fastlmmclib-0.0.5b1.dist-info/RECORD
+8 files, 79177 bytes uncompressed, 35906 bytes compressed:  54.7%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: fastlmmclib/quadform/qfc_src/__init__.py
 Comment: 
 
 Filename: fastlmmclib/quadform/qfc_src/wrap_qfc.cp39-win_amd64.pyd
 Comment: 
 
-Filename: fastlmmclib-0.0.3.dist-info/LICENSE
+Filename: fastlmmclib-0.0.5b1.dist-info/LICENSE
 Comment: 
 
-Filename: fastlmmclib-0.0.3.dist-info/METADATA
+Filename: fastlmmclib-0.0.5b1.dist-info/METADATA
 Comment: 
 
-Filename: fastlmmclib-0.0.3.dist-info/WHEEL
+Filename: fastlmmclib-0.0.5b1.dist-info/WHEEL
 Comment: 
 
-Filename: fastlmmclib-0.0.3.dist-info/top_level.txt
+Filename: fastlmmclib-0.0.5b1.dist-info/top_level.txt
 Comment: 
 
-Filename: fastlmmclib-0.0.3.dist-info/RECORD
+Filename: fastlmmclib-0.0.5b1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fastlmmclib/quadform/__init__.py

```diff
@@ -2,14 +2,15 @@
 
 from fastlmmclib.quadform.qfc_src import wrap_qfc
 
 
 def qf(
     chi2val, coeffs, dof=None, noncentrality=None, sigma=0.0, lim=1000000, acc=1e-08
 ):
+    coeffs = np.ascontiguousarray(coeffs)
     size = coeffs.shape[0]
     if dof is None:
         dof = np.ones(size, dtype="int32")
         # dof = np.ones(size)
     if noncentrality is None:
         noncentrality = np.zeros(size)
     ifault = np.zeros(1, dtype="int32")
```

## Comparing `fastlmmclib-0.0.3.dist-info/LICENSE` & `fastlmmclib-0.0.5b1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fastlmmclib-0.0.3.dist-info/METADATA` & `fastlmmclib-0.0.5b1.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: fastlmmclib
-Version: 0.0.3
+Version: 0.0.5b1
 Summary: Fast GWAS C library
 Home-page: https://fastlmm.github.io/
 Author: FaST-LMM Team
 Author-email: fastlmm-dev@python.org
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/fastlmm/fastlmmclib/issues
 Project-URL: Source Code, https://github.com/fastlmm/fastlmmclib
 Keywords: gwas bioinformatics LMMs MLMs linear mixed models genomics genetics python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 
 # fastlmmclib
+
 C extensions for FaST-LMM Python Project
```

