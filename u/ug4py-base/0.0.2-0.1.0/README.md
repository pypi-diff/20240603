# Comparing `tmp/ug4py_base-0.0.2-cp312-cp312-win_amd64.whl.zip` & `tmp/ug4py_base-0.1.0-cp312-cp312-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5269851 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat  2790400 b- defN 24-Jun-03 09:21 ug4py/pyconvectiondiffusion.cp312-win_amd64.pyd
--rw-rw-rw-  2.0 fat  2846208 b- defN 24-Jun-03 09:23 ug4py/pylimex.cp312-win_amd64.pyd
--rw-rw-rw-  2.0 fat 11852288 b- defN 24-Jun-03 09:23 ug4py/pyugcore.cp312-win_amd64.pyd
--rw-rw-r--  2.0 fat     1249 b- defN 24-Jun-03 09:23 ug4py_base-0.0.2.dist-info/METADATA
--rw-rw-r--  2.0 fat      105 b- defN 24-Jun-03 09:23 ug4py_base-0.0.2.dist-info/WHEEL
--rw-rw-r--  2.0 fat     1116 b- defN 24-Jun-03 09:23 ug4py_base-0.0.2.dist-info/licenses/LICENSE
--rw-rw-r--  2.0 fat      611 b- defN 24-Jun-03 09:23 ug4py_base-0.0.2.dist-info/RECORD
-7 files, 17491977 bytes uncompressed, 5268783 bytes compressed:  69.9%
+Zip file size: 2636301 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat   688640 b- defN 24-Jun-03 11:10 ug4py/pyconvectiondiffusion.cp312-win_amd64.pyd
+-rw-rw-rw-  2.0 fat  1300480 b- defN 24-Jun-03 11:12 ug4py/pylimex.cp312-win_amd64.pyd
+-rw-rw-rw-  2.0 fat  6952448 b- defN 24-Jun-03 11:12 ug4py/pyugcore.cp312-win_amd64.pyd
+-rw-rw-r--  2.0 fat     1249 b- defN 24-Jun-03 11:12 ug4py_base-0.1.0.dist-info/METADATA
+-rw-rw-r--  2.0 fat      105 b- defN 24-Jun-03 11:12 ug4py_base-0.1.0.dist-info/WHEEL
+-rw-rw-r--  2.0 fat     1116 b- defN 24-Jun-03 11:12 ug4py_base-0.1.0.dist-info/licenses/LICENSE
+-rw-rw-r--  2.0 fat      609 b- defN 24-Jun-03 11:12 ug4py_base-0.1.0.dist-info/RECORD
+7 files, 8944647 bytes uncompressed, 2635233 bytes compressed:  70.5%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: ug4py/pylimex.cp312-win_amd64.pyd
 Comment: 
 
 Filename: ug4py/pyugcore.cp312-win_amd64.pyd
 Comment: 
 
-Filename: ug4py_base-0.0.2.dist-info/METADATA
+Filename: ug4py_base-0.1.0.dist-info/METADATA
 Comment: 
 
-Filename: ug4py_base-0.0.2.dist-info/WHEEL
+Filename: ug4py_base-0.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: ug4py_base-0.0.2.dist-info/licenses/LICENSE
+Filename: ug4py_base-0.1.0.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: ug4py_base-0.0.2.dist-info/RECORD
+Filename: ug4py_base-0.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `ug4py_base-0.0.2.dist-info/METADATA` & `ug4py_base-0.1.0.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ug4py-base
-Version: 0.0.2
+Version: 0.1.0
 Summary: This is a basic python package for UG4.
 Description-Content-Type: text/markdown
 
 # ug4py-basic-wheels
 
 [![Build wheels](https://github.com/UG4/py-basic-wheels/actions/workflows/wheels.yml/badge.svg)](https://github.com/UG4/ugpip/actions/workflows/wheels.yml)
```

## Comparing `ug4py_base-0.0.2.dist-info/licenses/LICENSE` & `ug4py_base-0.1.0.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `ug4py_base-0.0.2.dist-info/RECORD` & `ug4py_base-0.1.0.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-ug4py/pyconvectiondiffusion.cp312-win_amd64.pyd,sha256=OSNwo6vnZdJBOhUrgr2FQQOvsg1l4F4blby_-U06QKM,2790400
-ug4py/pylimex.cp312-win_amd64.pyd,sha256=D8pNJo3j0ei2xXLlArUpn4dXxmDarN_AvfrXQr-HBAQ,2846208
-ug4py/pyugcore.cp312-win_amd64.pyd,sha256=v7qGlH1GQ1h4lWg25vXZTQJtmka5UqQ_-_vndsfqntg,11852288
-ug4py_base-0.0.2.dist-info/METADATA,sha256=QuK2i2dfsouCnrhSx9X_id1fIV2WkANVXRAC7nsoGJU,1249
-ug4py_base-0.0.2.dist-info/WHEEL,sha256=QGejE-29qHdvo-x9pCICVWVWKdrsgc_rseByQp_tx9U,105
-ug4py_base-0.0.2.dist-info/licenses/LICENSE,sha256=4W_AZ3paFOk9Tf2efYRUETQsdIe_kD5yQC-1ZtJLilM,1116
-ug4py_base-0.0.2.dist-info/RECORD,,
+ug4py/pyconvectiondiffusion.cp312-win_amd64.pyd,sha256=ZNISlxN5ZAOxyj5gxv42ZMwFmZIlfgz6BLK2W6X7WQ0,688640
+ug4py/pylimex.cp312-win_amd64.pyd,sha256=8MM1GsZby-MeYU00vqrq2DP6hFoqWkeWj9rBn8BlquY,1300480
+ug4py/pyugcore.cp312-win_amd64.pyd,sha256=l369k7_m2w3dQ_e3IAuCFiGTU0xRBgLX1pN5LKFYUO4,6952448
+ug4py_base-0.1.0.dist-info/METADATA,sha256=oRA-6OUGqSA8GcLtnLA0fOTk1umgA4ExRed2GV5IT8U,1249
+ug4py_base-0.1.0.dist-info/WHEEL,sha256=QGejE-29qHdvo-x9pCICVWVWKdrsgc_rseByQp_tx9U,105
+ug4py_base-0.1.0.dist-info/licenses/LICENSE,sha256=4W_AZ3paFOk9Tf2efYRUETQsdIe_kD5yQC-1ZtJLilM,1116
+ug4py_base-0.1.0.dist-info/RECORD,,
```

