# Comparing `tmp/qdrive-0.2.17-py3-none-any.whl.zip` & `tmp/qdrive-0.2.19-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 36012 bytes, number of entries: 38
--rw-r--r--  2.0 unx      580 b- defN 24-May-31 15:42 qdrive/__init__.py
+Zip file size: 36009 bytes, number of entries: 38
+-rw-r--r--  2.0 unx      580 b- defN 24-Jun-03 07:25 qdrive/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Dec-13 10:03 qdrive/dataset/__init__.py
 -rw-r--r--  2.0 unx     2574 b- defN 24-May-28 07:49 qdrive/dataset/dataset.py
 -rw-r--r--  2.0 unx     5038 b- defN 24-May-13 07:58 qdrive/dataset/file_manager.py
 -rw-r--r--  2.0 unx     3995 b- defN 24-Apr-04 09:44 qdrive/dataset/files/HDF5.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Dec-13 10:03 qdrive/dataset/files/__init__.py
 -rw-r--r--  2.0 unx      929 b- defN 23-Dec-13 10:03 qdrive/dataset/files/file.py
 -rw-r--r--  2.0 unx     3213 b- defN 24-Apr-04 09:51 qdrive/dataset/files/file_mgr_single.py
@@ -27,14 +27,14 @@
 -rw-r--r--  2.0 unx     6271 b- defN 23-Dec-13 10:03 qdrive/testing/dataset_file_feature_overview.py
 -rw-r--r--  2.0 unx      214 b- defN 23-Dec-13 10:03 qdrive/testing/interfaces_dataset.py
 -rw-r--r--  2.0 unx      635 b- defN 24-Feb-29 15:23 qdrive/testing/measurement_with_qdrive.py
 -rw-r--r--  2.0 unx     6360 b- defN 23-Dec-13 10:03 qdrive/testing/qcodes_test_param.py
 -rw-r--r--  2.0 unx     1105 b- defN 23-Dec-13 10:03 qdrive/testing/qdrive_dataset_test.py
 -rw-r--r--  2.0 unx     2181 b- defN 23-Dec-13 10:03 qdrive/testing/test.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Dec-13 10:03 qdrive/utility/__init__.py
--rw-r--r--  2.0 unx    16695 b- defN 24-May-31 15:43 qdrive-0.2.17.dist-info/LICENCE
--rw-r--r--  2.0 unx      671 b- defN 24-May-31 15:43 qdrive-0.2.17.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-31 15:43 qdrive-0.2.17.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 24-May-31 15:43 qdrive-0.2.17.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Dec-13 12:27 qdrive-0.2.17.dist-info/zip-safe
--rw-rw-r--  2.0 unx     3409 b- defN 24-May-31 15:43 qdrive-0.2.17.dist-info/RECORD
-38 files, 97622 bytes uncompressed, 30438 bytes compressed:  68.8%
+-rw-r--r--  2.0 unx    16695 b- defN 24-Jun-03 07:25 qdrive-0.2.19.dist-info/LICENCE
+-rw-r--r--  2.0 unx      671 b- defN 24-Jun-03 07:25 qdrive-0.2.19.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Jun-03 07:25 qdrive-0.2.19.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 24-Jun-03 07:25 qdrive-0.2.19.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Dec-13 12:27 qdrive-0.2.19.dist-info/zip-safe
+-rw-rw-r--  2.0 unx     3409 b- defN 24-Jun-03 07:25 qdrive-0.2.19.dist-info/RECORD
+38 files, 97622 bytes uncompressed, 30435 bytes compressed:  68.8%
```

## zipnote {}

```diff
@@ -90,26 +90,26 @@
 
 Filename: qdrive/testing/test.py
 Comment: 
 
 Filename: qdrive/utility/__init__.py
 Comment: 
 
-Filename: qdrive-0.2.17.dist-info/LICENCE
+Filename: qdrive-0.2.19.dist-info/LICENCE
 Comment: 
 
-Filename: qdrive-0.2.17.dist-info/METADATA
+Filename: qdrive-0.2.19.dist-info/METADATA
 Comment: 
 
-Filename: qdrive-0.2.17.dist-info/WHEEL
+Filename: qdrive-0.2.19.dist-info/WHEEL
 Comment: 
 
-Filename: qdrive-0.2.17.dist-info/top_level.txt
+Filename: qdrive-0.2.19.dist-info/top_level.txt
 Comment: 
 
-Filename: qdrive-0.2.17.dist-info/zip-safe
+Filename: qdrive-0.2.19.dist-info/zip-safe
 Comment: 
 
-Filename: qdrive-0.2.17.dist-info/RECORD
+Filename: qdrive-0.2.19.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## qdrive/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.2.17'
+__version__ = '0.2.19'
 
 try:
     from etiket_client.local.dao.app import dao_app_registerer
     from etiket_client.local.types import ProcTypes
 
     dao_app_registerer.register(__version__, ProcTypes.qDrive, __file__)
 except Exception as e:
```

## Comparing `qdrive-0.2.17.dist-info/LICENCE` & `qdrive-0.2.19.dist-info/LICENCE`

 * *Files identical despite different names*

## Comparing `qdrive-0.2.17.dist-info/METADATA` & `qdrive-0.2.19.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: qdrive
-Version: 0.2.17
+Version: 0.2.19
 Summary: Qdrive dataset library
 Author: QDrive team
 Requires-Python: >=3.7
 License-File: LICENCE
 Requires-Dist: PyYAML >=6.0.0
 Requires-Dist: platformdirs >=4.0.0
 Requires-Dist: numpy >=1.16.0
 Requires-Dist: qcodes >=0.3.0
-Requires-Dist: etiket-client >=0.2.17
+Requires-Dist: etiket-client >=0.2.19
 Requires-Dist: xarray <=0.20.2,>=0.15.0 ; python_version < "3.8"
 Requires-Dist: h5py <=3.8.0,>=3.0.0 ; python_version < "3.8"
 Requires-Dist: netCDF4 <=1.5.8,>=1.5.0 ; python_version < "3.8"
 Requires-Dist: xarray >=0.15.0 ; python_version >= "3.8"
 Requires-Dist: h5py >=3.0.0 ; python_version >= "3.8"
 Requires-Dist: netCDF4 >=1.5.0 ; python_version >= "3.8"
```

## Comparing `qdrive-0.2.17.dist-info/RECORD` & `qdrive-0.2.19.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-qdrive/__init__.py,sha256=6ApPpveKV2N_JgTrD7EKKaw9mgdlcJ2xXM9PcNl7_uQ,580
+qdrive/__init__.py,sha256=m9EkUGFagunzXfpc5CLeE7nidGMm4uFjSx2DC4-iywA,580
 qdrive/dataset/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 qdrive/dataset/dataset.py,sha256=2rqqF0DGwvsP1YKKrkxXyTzsW9niyRAHC-e_uFqq9nk,2574
 qdrive/dataset/file_manager.py,sha256=l_t0cjRbUACiu5KflF0HMbVtzUSRt3cpwmp4sf0GWNc,5038
 qdrive/dataset/files/HDF5.py,sha256=20nYipbsqqIoE6rN3xxsQS2mL4FKBSX8LyA4bE2ePlI,3995
 qdrive/dataset/files/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 qdrive/dataset/files/file.py,sha256=qz6n1_b4wvUovMF3UGj7JpvfDP8sndegD3OSfZWOjEg,929
 qdrive/dataset/files/file_mgr_single.py,sha256=XW1NsmLWX6bn6EKVF8MwO4icVgEPKxClMOeL880B-IY,3213
@@ -26,13 +26,13 @@
 qdrive/testing/dataset_file_feature_overview.py,sha256=GQBka3vPO57bY9t5vtUsMWqeO-4WqY3IJcYFsBBlULg,6271
 qdrive/testing/interfaces_dataset.py,sha256=zJEG8EVx7Rf6Bu5upmBCK8rrdNanB3jIKe0rW-NF2aM,214
 qdrive/testing/measurement_with_qdrive.py,sha256=FOKDWqD11XmD8dXBvTZFZfweT-JR6st8ltT9fOkSQTI,635
 qdrive/testing/qcodes_test_param.py,sha256=YF1AW-qpVhBKEgxQxnODOU_taijtHsM-r-u6H7wWle8,6360
 qdrive/testing/qdrive_dataset_test.py,sha256=AFhbgJONRj-lRsIEI_L6zeMHLCepMyvtIms-dAeMzIU,1105
 qdrive/testing/test.py,sha256=QbMylU_a80YIqPzpM_-eVvOrbYn1jQYQrMeEDWS4bcA,2181
 qdrive/utility/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-qdrive-0.2.17.dist-info/LICENCE,sha256=BNXChWe7aLPGR3QkVckAkeLqK2cI2idnmInh-A3YOO0,16695
-qdrive-0.2.17.dist-info/METADATA,sha256=whbAIrbiYu6DBJ8oM-N4_JtJ-tj9q1L07Ifr-bsKGfw,671
-qdrive-0.2.17.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-qdrive-0.2.17.dist-info/top_level.txt,sha256=B1Ij35CV2H-FfDMctSIRLfZ9EIU_GshRACjkLDpc4I8,7
-qdrive-0.2.17.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-qdrive-0.2.17.dist-info/RECORD,,
+qdrive-0.2.19.dist-info/LICENCE,sha256=BNXChWe7aLPGR3QkVckAkeLqK2cI2idnmInh-A3YOO0,16695
+qdrive-0.2.19.dist-info/METADATA,sha256=1tnvsASaxlIrw35rwL7vxxRG8eEtRr8Cba8bXFhX0CE,671
+qdrive-0.2.19.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+qdrive-0.2.19.dist-info/top_level.txt,sha256=B1Ij35CV2H-FfDMctSIRLfZ9EIU_GshRACjkLDpc4I8,7
+qdrive-0.2.19.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+qdrive-0.2.19.dist-info/RECORD,,
```

