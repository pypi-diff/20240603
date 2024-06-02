# Comparing `tmp/SCDB_ML_app-1.0.2-py3-none-any.whl.zip` & `tmp/SCDB_ML_app-1.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,13 @@
-Zip file size: 12836 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat    32005 b- defN 24-Jun-02 22:30 SCDB_ML_app-1.0.2.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat      892 b- defN 24-Jun-02 22:30 SCDB_ML_app-1.0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Jun-02 22:30 SCDB_ML_app-1.0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat      809 b- defN 24-Jun-02 22:30 SCDB_ML_app-1.0.2.dist-info/licenseheader.txt
--rw-rw-rw-  2.0 fat        1 b- defN 24-Jun-02 22:30 SCDB_ML_app-1.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      510 b- defN 24-Jun-02 22:30 SCDB_ML_app-1.0.2.dist-info/RECORD
-6 files, 34309 bytes uncompressed, 11902 bytes compressed:  65.3%
+Zip file size: 19770 bytes, number of entries: 11
+-rw-rw-rw-  2.0 fat     8079 b- defN 24-Jun-02 20:55 flask_app/SCDB_ML_app.py
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Jun-02 23:02 flask_app/__init__.py
+-rw-rw-rw-  2.0 fat     3982 b- defN 24-Jun-02 20:55 flask_app/mine_decision_tree.py
+-rw-rw-rw-  2.0 fat     2165 b- defN 24-Jun-02 20:55 flask_app/predict_decision_tree.py
+-rw-rw-rw-  2.0 fat     2571 b- defN 24-Jun-02 20:55 flask_app/train_decision_tree.py
+-rw-rw-rw-  2.0 fat    32005 b- defN 24-Jun-02 23:08 SCDB_ML_app-1.0.3.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat      892 b- defN 24-Jun-02 23:08 SCDB_ML_app-1.0.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Jun-02 23:08 SCDB_ML_app-1.0.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat      809 b- defN 24-Jun-02 23:08 SCDB_ML_app-1.0.3.dist-info/licenseheader.txt
+-rw-rw-rw-  2.0 fat       10 b- defN 24-Jun-02 23:08 SCDB_ML_app-1.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      935 b- defN 24-Jun-02 23:08 SCDB_ML_app-1.0.3.dist-info/RECORD
+11 files, 51540 bytes uncompressed, 18172 bytes compressed:  64.7%
```

## zipnote {}

```diff
@@ -1,19 +1,34 @@
-Filename: SCDB_ML_app-1.0.2.dist-info/LICENSE.txt
+Filename: flask_app/SCDB_ML_app.py
 Comment: 
 
-Filename: SCDB_ML_app-1.0.2.dist-info/METADATA
+Filename: flask_app/__init__.py
 Comment: 
 
-Filename: SCDB_ML_app-1.0.2.dist-info/WHEEL
+Filename: flask_app/mine_decision_tree.py
 Comment: 
 
-Filename: SCDB_ML_app-1.0.2.dist-info/licenseheader.txt
+Filename: flask_app/predict_decision_tree.py
 Comment: 
 
-Filename: SCDB_ML_app-1.0.2.dist-info/top_level.txt
+Filename: flask_app/train_decision_tree.py
 Comment: 
 
-Filename: SCDB_ML_app-1.0.2.dist-info/RECORD
+Filename: SCDB_ML_app-1.0.3.dist-info/LICENSE.txt
+Comment: 
+
+Filename: SCDB_ML_app-1.0.3.dist-info/METADATA
+Comment: 
+
+Filename: SCDB_ML_app-1.0.3.dist-info/WHEEL
+Comment: 
+
+Filename: SCDB_ML_app-1.0.3.dist-info/licenseheader.txt
+Comment: 
+
+Filename: SCDB_ML_app-1.0.3.dist-info/top_level.txt
+Comment: 
+
+Filename: SCDB_ML_app-1.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `SCDB_ML_app-1.0.2.dist-info/LICENSE.txt` & `SCDB_ML_app-1.0.3.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `SCDB_ML_app-1.0.2.dist-info/METADATA` & `SCDB_ML_app-1.0.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SCDB_ML_app
-Version: 1.0.2
+Version: 1.0.3
 Summary: A MACHINE LEARNING ANALYZER DEPLOYED INTO A WEBPAGE
 Home-page: https://github.com/havurquijo/Project-SCDB
 Download-URL: https://github.com/havurquijo/Project-SCDB/archive/refs/tags/v1.0.0-alpha.tar.gz
 Author: HERMES A V URQUIJO
 Author-email: hvurquijo@gmail.com
 License: AGPL 3.0
 Keywords: MACHINE,LEARNING,SCDB,SUPREME,COURT,WEBPAGE
```

## Comparing `SCDB_ML_app-1.0.2.dist-info/licenseheader.txt` & `SCDB_ML_app-1.0.3.dist-info/licenseheader.txt`

 * *Files identical despite different names*

