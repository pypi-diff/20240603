# Comparing `tmp/Mzhtools-0.1.1-py3-none-any.whl.zip` & `tmp/Mzhtools-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 14140 bytes, number of entries: 11
+Zip file size: 14188 bytes, number of entries: 11
 -rw-rw-rw-  2.0 fat    12430 b- defN 24-Jun-03 13:46 MzhFunc/MzhFunc.py
 -rw-rw-rw-  2.0 fat      222 b- defN 24-Jun-03 13:46 MzhFunc/__init__.py
 -rw-rw-rw-  2.0 fat    12430 b- defN 24-Jun-03 13:46 Mzhtools/Mzhtools.py
--rw-rw-rw-  2.0 fat      222 b- defN 24-Jun-03 13:46 Mzhtools/__init__.py
--rw-rw-rw-  2.0 fat       74 b- defN 24-Jun-02 16:21 Mzhtools-0.1.1.data/data/requirements.txt
+-rw-rw-rw-  2.0 fat      246 b- defN 24-Jun-03 13:53 Mzhtools/__init__.py
+-rw-rw-rw-  2.0 fat       74 b- defN 24-Jun-02 16:21 Mzhtools-0.1.2.data/data/requirements.txt
 -rw-rw-rw-  2.0 fat    12430 b- defN 24-Jun-03 13:46 db/MzhFunc.py
 -rw-rw-rw-  2.0 fat      222 b- defN 24-Jun-03 13:46 db/__init__.py
--rw-rw-rw-  2.0 fat      399 b- defN 24-Jun-03 13:46 Mzhtools-0.1.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Jun-03 13:46 Mzhtools-0.1.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 24-Jun-03 13:46 Mzhtools-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      842 b- defN 24-Jun-03 13:46 Mzhtools-0.1.1.dist-info/RECORD
-11 files, 39372 bytes uncompressed, 12728 bytes compressed:  67.7%
+-rw-rw-rw-  2.0 fat      399 b- defN 24-Jun-03 13:54 Mzhtools-0.1.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Jun-03 13:54 Mzhtools-0.1.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 24-Jun-03 13:54 Mzhtools-0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      842 b- defN 24-Jun-03 13:54 Mzhtools-0.1.2.dist-info/RECORD
+11 files, 39396 bytes uncompressed, 12776 bytes compressed:  67.6%
```

## zipnote {}

```diff
@@ -6,29 +6,29 @@
 
 Filename: Mzhtools/Mzhtools.py
 Comment: 
 
 Filename: Mzhtools/__init__.py
 Comment: 
 
-Filename: Mzhtools-0.1.1.data/data/requirements.txt
+Filename: Mzhtools-0.1.2.data/data/requirements.txt
 Comment: 
 
 Filename: db/MzhFunc.py
 Comment: 
 
 Filename: db/__init__.py
 Comment: 
 
-Filename: Mzhtools-0.1.1.dist-info/METADATA
+Filename: Mzhtools-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: Mzhtools-0.1.1.dist-info/WHEEL
+Filename: Mzhtools-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: Mzhtools-0.1.1.dist-info/top_level.txt
+Filename: Mzhtools-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: Mzhtools-0.1.1.dist-info/RECORD
+Filename: Mzhtools-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Mzhtools/__init__.py

```diff
@@ -1,5 +1,6 @@
 # -*- coding: utf-8 -*-
 r"""
 Created on 2024/6/2 0:55
 rd /S /Q "d:\pybuild"&&mkdir "d:\pybuild"&&pyinstaller D:/python/函数/pip_Mzhtools/Mzhtools\__init__.py.py --workpath d:\pybuild  --distpath d:\pybuild\dist
 """
+import Mzhtools.Mzhtools
```

## Comparing `Mzhtools-0.1.1.dist-info/RECORD` & `Mzhtools-0.1.2.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 MzhFunc/MzhFunc.py,sha256=Zu8FIkqgNUx2eMAuZjnFqPz1hzJKa3xt9NiJKpuxVus,12430
 MzhFunc/__init__.py,sha256=cPl4CWduC2SiDJUU_t41kwcOSnhyQ2ui3c6QWkB2vYI,222
 Mzhtools/Mzhtools.py,sha256=Zu8FIkqgNUx2eMAuZjnFqPz1hzJKa3xt9NiJKpuxVus,12430
-Mzhtools/__init__.py,sha256=cPl4CWduC2SiDJUU_t41kwcOSnhyQ2ui3c6QWkB2vYI,222
-Mzhtools-0.1.1.data/data/requirements.txt,sha256=OS_dEls24CUMLgCDof-NKXHA1Fw5XA_wEnPimzeE8pY,74
+Mzhtools/__init__.py,sha256=PDITAKOBQQFWIbpEExdax1dYLOxTce7-eoChF-Rey7A,246
+Mzhtools-0.1.2.data/data/requirements.txt,sha256=OS_dEls24CUMLgCDof-NKXHA1Fw5XA_wEnPimzeE8pY,74
 db/MzhFunc.py,sha256=Zu8FIkqgNUx2eMAuZjnFqPz1hzJKa3xt9NiJKpuxVus,12430
 db/__init__.py,sha256=cPl4CWduC2SiDJUU_t41kwcOSnhyQ2ui3c6QWkB2vYI,222
-Mzhtools-0.1.1.dist-info/METADATA,sha256=yj9R88zhojTUsIeQQ_l2W3OaTDHWEMYOQwcdvhK6MQc,399
-Mzhtools-0.1.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-Mzhtools-0.1.1.dist-info/top_level.txt,sha256=R6dd-_nPsdYB0H6rcqwUd6HQgxsg_tZpWlMvi5cuU1Y,9
-Mzhtools-0.1.1.dist-info/RECORD,,
+Mzhtools-0.1.2.dist-info/METADATA,sha256=8Jd9nQJziDP3wK5JjNxNH8bJttErPJM2qDXbv1kzIIY,399
+Mzhtools-0.1.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+Mzhtools-0.1.2.dist-info/top_level.txt,sha256=R6dd-_nPsdYB0H6rcqwUd6HQgxsg_tZpWlMvi5cuU1Y,9
+Mzhtools-0.1.2.dist-info/RECORD,,
```

