# Comparing `tmp/SCRIP-0.1.240527-py3-none-any.whl.zip` & `tmp/SCRIP-0.1.240603-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 7541004 bytes, number of entries: 33
+Zip file size: 7540985 bytes, number of entries: 33
 -rw-r--r--  2.0 unx       87 b- defN 23-Feb-13 03:19 SCRIP/Constants.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Feb-13 03:19 SCRIP/__init__.py
 -rw-r--r--  2.0 unx    11143 b- defN 24-May-27 07:06 SCRIP/start.py
 -rw-r--r--  2.0 unx 25673202 b- defN 23-Feb-13 03:19 SCRIP/conf/GRCh38_refgenes.txt
 -rw-r--r--  2.0 unx 13253565 b- defN 23-Feb-13 03:19 SCRIP/conf/GRCm38_refgenes.txt
 -rw-r--r--  2.0 unx        0 b- defN 23-Feb-13 03:19 SCRIP/conf/__init__.py
 -rw-r--r--  2.0 unx     1018 b- defN 23-Feb-13 03:19 SCRIP/conf/config.py
@@ -22,14 +22,14 @@
 -rw-r--r--  2.0 unx     1416 b- defN 23-Feb-13 03:19 SCRIP/index/index.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Feb-13 03:19 SCRIP/targets/__init__.py
 -rw-r--r--  2.0 unx    15780 b- defN 23-Feb-13 03:19 SCRIP/targets/target.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Feb-13 03:19 SCRIP/utilities/__init__.py
 -rw-r--r--  2.0 unx      658 b- defN 23-Feb-13 03:19 SCRIP/utilities/convert_format.py
 -rw-r--r--  2.0 unx      855 b- defN 23-Feb-13 03:19 SCRIP/utilities/convert_seurat2anndata.py
 -rw-r--r--  2.0 unx     2245 b- defN 23-Feb-13 03:19 SCRIP/utilities/utils.py
--rw-r--r--  2.0 unx     1065 b- defN 24-May-27 07:24 SCRIP-0.1.240527.dist-info/LICENSE
--rw-r--r--  2.0 unx      630 b- defN 24-May-27 07:24 SCRIP-0.1.240527.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-27 07:24 SCRIP-0.1.240527.dist-info/WHEEL
--rw-r--r--  2.0 unx       43 b- defN 24-May-27 07:24 SCRIP-0.1.240527.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        6 b- defN 24-May-27 07:24 SCRIP-0.1.240527.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     2732 b- defN 24-May-27 07:24 SCRIP-0.1.240527.dist-info/RECORD
-33 files, 39012025 bytes uncompressed, 7536618 bytes compressed:  80.7%
+-rw-r--r--  2.0 unx     1065 b- defN 24-Jun-03 07:48 SCRIP-0.1.240603.dist-info/LICENSE
+-rw-r--r--  2.0 unx      608 b- defN 24-Jun-03 07:48 SCRIP-0.1.240603.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Jun-03 07:48 SCRIP-0.1.240603.dist-info/WHEEL
+-rw-r--r--  2.0 unx       43 b- defN 24-Jun-03 07:48 SCRIP-0.1.240603.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        6 b- defN 24-Jun-03 07:48 SCRIP-0.1.240603.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2732 b- defN 24-Jun-03 07:48 SCRIP-0.1.240603.dist-info/RECORD
+33 files, 39012003 bytes uncompressed, 7536599 bytes compressed:  80.7%
```

## zipnote {}

```diff
@@ -75,26 +75,26 @@
 
 Filename: SCRIP/utilities/convert_seurat2anndata.py
 Comment: 
 
 Filename: SCRIP/utilities/utils.py
 Comment: 
 
-Filename: SCRIP-0.1.240527.dist-info/LICENSE
+Filename: SCRIP-0.1.240603.dist-info/LICENSE
 Comment: 
 
-Filename: SCRIP-0.1.240527.dist-info/METADATA
+Filename: SCRIP-0.1.240603.dist-info/METADATA
 Comment: 
 
-Filename: SCRIP-0.1.240527.dist-info/WHEEL
+Filename: SCRIP-0.1.240603.dist-info/WHEEL
 Comment: 
 
-Filename: SCRIP-0.1.240527.dist-info/entry_points.txt
+Filename: SCRIP-0.1.240603.dist-info/entry_points.txt
 Comment: 
 
-Filename: SCRIP-0.1.240527.dist-info/top_level.txt
+Filename: SCRIP-0.1.240603.dist-info/top_level.txt
 Comment: 
 
-Filename: SCRIP-0.1.240527.dist-info/RECORD
+Filename: SCRIP-0.1.240603.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `SCRIP-0.1.240527.dist-info/LICENSE` & `SCRIP-0.1.240603.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `SCRIP-0.1.240527.dist-info/METADATA` & `SCRIP-0.1.240603.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: SCRIP
-Version: 0.1.240527
+Version: 0.1.240603
 Summary: A package for single cell ATAC-seq analysis
 Author: Xin Dong
 Author-email: xindong9511@gmail.com
 Requires-Python: >=3.8.12, !=3.9
 License-File: LICENSE
 Requires-Dist: numba >=0.51.2
-Requires-Dist: numpy <1.24,>=1.18
+Requires-Dist: numpy >=1.18
 Requires-Dist: pandas >=1.3.3
 Requires-Dist: cython >=0.29.22
 Requires-Dist: ruamel.yaml
-Requires-Dist: anndata <=0.7.6
-Requires-Dist: anndata2ri <=1.0.6
+Requires-Dist: anndata >=0.7.6
+Requires-Dist: anndata2ri >=1.0.6
 Requires-Dist: pyranges >=0.0.95
 Requires-Dist: pybedtools >=0.8.2
-Requires-Dist: matplotlib <=3.3.2,>=3.1.2
+Requires-Dist: matplotlib >=3.1.2
 Requires-Dist: scikit-learn
 Requires-Dist: scipy
-Requires-Dist: scanpy <=1.8.1,>=1.7.1
+Requires-Dist: scanpy >=1.7.1
```

## Comparing `SCRIP-0.1.240527.dist-info/RECORD` & `SCRIP-0.1.240603.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -21,13 +21,13 @@
 SCRIP/index/index.py,sha256=Gqfhu-k0r0lFZlPwLjKccGzmhpQCGSxX_8DfXgAEVLo,1416
 SCRIP/targets/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 SCRIP/targets/target.py,sha256=PkiHk3dZcymWbrRZspKEkdYnDVIFIomqUElhDirEkK0,15780
 SCRIP/utilities/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 SCRIP/utilities/convert_format.py,sha256=wCusAaKLz5iC_SSCQXDt4DyGh8WlNfX1ZuPzmlpkMFw,658
 SCRIP/utilities/convert_seurat2anndata.py,sha256=-lYd_QxiglmK42GOwusWHWdU9GsVsnz9PvqLZn4gWdU,855
 SCRIP/utilities/utils.py,sha256=AIS0kkNcktFkNSWscSGQSsweeXDhQlMML_900u65sc8,2245
-SCRIP-0.1.240527.dist-info/LICENSE,sha256=2OyhOxXCmFuvOyAckfAeYn9FPVpx8Z8cKOowCmkB6Zg,1065
-SCRIP-0.1.240527.dist-info/METADATA,sha256=IQZbBw2qB4vlGzpXqmedd5Fm_9np0sGZqTmsX50lpSs,630
-SCRIP-0.1.240527.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-SCRIP-0.1.240527.dist-info/entry_points.txt,sha256=jps6jrAzJ-9aHAcuIiKTjCOB0l2ABlLkszGEqdRwxZE,43
-SCRIP-0.1.240527.dist-info/top_level.txt,sha256=F9AWp9GwlV2NxKYekD9_Iaj8EAzEkS-waVaEgF11qmg,6
-SCRIP-0.1.240527.dist-info/RECORD,,
+SCRIP-0.1.240603.dist-info/LICENSE,sha256=2OyhOxXCmFuvOyAckfAeYn9FPVpx8Z8cKOowCmkB6Zg,1065
+SCRIP-0.1.240603.dist-info/METADATA,sha256=K6kdIGij5b4aBooX2UtMBWexeq4VXQUgja-GuivKxq8,608
+SCRIP-0.1.240603.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+SCRIP-0.1.240603.dist-info/entry_points.txt,sha256=jps6jrAzJ-9aHAcuIiKTjCOB0l2ABlLkszGEqdRwxZE,43
+SCRIP-0.1.240603.dist-info/top_level.txt,sha256=F9AWp9GwlV2NxKYekD9_Iaj8EAzEkS-waVaEgF11qmg,6
+SCRIP-0.1.240603.dist-info/RECORD,,
```

