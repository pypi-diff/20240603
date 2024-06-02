# Comparing `tmp/SCDB_ML_app-1.0.5-py3-none-any.whl.zip` & `tmp/SCDB_ML_app-1.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 3446643 bytes, number of entries: 43
+Zip file size: 3446683 bytes, number of entries: 43
 -rw-rw-rw-  2.0 fat     8079 b- defN 24-Jun-02 20:55 flask_app/SCDB_ML_app.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Jun-02 23:02 flask_app/__init__.py
 -rw-rw-rw-  2.0 fat     3982 b- defN 24-Jun-02 20:55 flask_app/mine_decision_tree.py
 -rw-rw-rw-  2.0 fat     2165 b- defN 24-Jun-02 20:55 flask_app/predict_decision_tree.py
 -rw-rw-rw-  2.0 fat     2571 b- defN 24-Jun-02 20:55 flask_app/train_decision_tree.py
--rw-rw-rw-  2.0 fat     8079 b- defN 24-Jun-02 20:55 scdb_ml_app/SCDB_ML_app.py
+-rw-rw-rw-  2.0 fat     8082 b- defN 24-Jun-02 23:46 scdb_ml_app/SCDB_ML_app.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Jun-02 23:02 scdb_ml_app/__init__.py
 -rw-rw-rw-  2.0 fat     3982 b- defN 24-Jun-02 20:55 scdb_ml_app/mine_decision_tree.py
 -rw-rw-rw-  2.0 fat     2165 b- defN 24-Jun-02 20:55 scdb_ml_app/predict_decision_tree.py
 -rw-rw-rw-  2.0 fat     2571 b- defN 24-Jun-02 20:55 scdb_ml_app/train_decision_tree.py
 -rw-rw-rw-  2.0 fat  1669742 b- defN 24-May-29 15:42 scdb_ml_app/models/SCDB_2023_01_justiceCentered_Citation.csv.zip
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Jun-02 23:13 scdb_ml_app/models/__init__.py
 -rw-rw-rw-  2.0 fat       26 b- defN 24-May-31 16:02 scdb_ml_app/models/accuracy_tree.txt
@@ -32,14 +32,14 @@
 -rw-rw-rw-  2.0 fat    11255 b- defN 24-Jun-02 20:54 scdb_ml_app/templates/base.html
 -rw-rw-rw-  2.0 fat    44910 b- defN 24-Jun-02 20:54 scdb_ml_app/templates/index.html
 -rw-rw-rw-  2.0 fat     1920 b- defN 24-Jun-02 20:54 scdb_ml_app/templates/mine_tree.html
 -rw-rw-rw-  2.0 fat     1336 b- defN 24-Jun-02 20:54 scdb_ml_app/templates/notFound.html
 -rw-rw-rw-  2.0 fat     4304 b- defN 24-Jun-02 20:54 scdb_ml_app/templates/predict_tree.html
 -rw-rw-rw-  2.0 fat     3468 b- defN 24-Jun-02 20:54 scdb_ml_app/templates/predicted_tree.html
 -rw-rw-rw-  2.0 fat     2655 b- defN 24-Jun-02 20:52 scdb_ml_app/templates/train_tree.html
--rw-rw-rw-  2.0 fat    32005 b- defN 24-Jun-02 23:30 SCDB_ML_app-1.0.5.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat      892 b- defN 24-Jun-02 23:30 SCDB_ML_app-1.0.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Jun-02 23:30 SCDB_ML_app-1.0.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat      809 b- defN 24-Jun-02 23:30 SCDB_ML_app-1.0.5.dist-info/licenseheader.txt
--rw-rw-rw-  2.0 fat       12 b- defN 24-Jun-02 23:30 SCDB_ML_app-1.0.5.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     3966 b- defN 24-Jun-02 23:30 SCDB_ML_app-1.0.5.dist-info/RECORD
-43 files, 30882499 bytes uncompressed, 3440175 bytes compressed:  88.9%
+-rw-rw-rw-  2.0 fat    32005 b- defN 24-Jun-02 23:48 SCDB_ML_app-1.0.6.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat      892 b- defN 24-Jun-02 23:48 SCDB_ML_app-1.0.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Jun-02 23:48 SCDB_ML_app-1.0.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat      809 b- defN 24-Jun-02 23:48 SCDB_ML_app-1.0.6.dist-info/licenseheader.txt
+-rw-rw-rw-  2.0 fat       12 b- defN 24-Jun-02 23:48 SCDB_ML_app-1.0.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     3966 b- defN 24-Jun-02 23:48 SCDB_ML_app-1.0.6.dist-info/RECORD
+43 files, 30882502 bytes uncompressed, 3440215 bytes compressed:  88.9%
```

## zipnote {}

```diff
@@ -105,26 +105,26 @@
 
 Filename: scdb_ml_app/templates/predicted_tree.html
 Comment: 
 
 Filename: scdb_ml_app/templates/train_tree.html
 Comment: 
 
-Filename: SCDB_ML_app-1.0.5.dist-info/LICENSE.txt
+Filename: SCDB_ML_app-1.0.6.dist-info/LICENSE.txt
 Comment: 
 
-Filename: SCDB_ML_app-1.0.5.dist-info/METADATA
+Filename: SCDB_ML_app-1.0.6.dist-info/METADATA
 Comment: 
 
-Filename: SCDB_ML_app-1.0.5.dist-info/WHEEL
+Filename: SCDB_ML_app-1.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: SCDB_ML_app-1.0.5.dist-info/licenseheader.txt
+Filename: SCDB_ML_app-1.0.6.dist-info/licenseheader.txt
 Comment: 
 
-Filename: SCDB_ML_app-1.0.5.dist-info/top_level.txt
+Filename: SCDB_ML_app-1.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: SCDB_ML_app-1.0.5.dist-info/RECORD
+Filename: SCDB_ML_app-1.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## scdb_ml_app/SCDB_ML_app.py

```diff
@@ -12,17 +12,17 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU Affero General Public License for more details.
 
 You should have received a copy of the GNU Affero General Public License
 along with this program.  If not, see <http://www.gnu.org/licenses/>.
 '''
 from flask import Flask,redirect,url_for,render_template,request,jsonify,send_file # type: ignore
-from mine_decision_tree import mine_decision_tree as mine_tree_class
-from predict_decision_tree import predict_decision_tree as predict_tree_class
-from train_decision_tree import train_decision_tree as train_tree_class
+from .mine_decision_tree import mine_decision_tree as mine_tree_class
+from .predict_decision_tree import predict_decision_tree as predict_tree_class
+from .train_decision_tree import train_decision_tree as train_tree_class
 import time
 from os import remove
 from os.path import exists
 from numpy import savetxt, loadtxt
 from pandas import DataFrame
 
 app = Flask(__name__)
```

## Comparing `SCDB_ML_app-1.0.5.dist-info/LICENSE.txt` & `SCDB_ML_app-1.0.6.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `SCDB_ML_app-1.0.5.dist-info/METADATA` & `SCDB_ML_app-1.0.6.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SCDB_ML_app
-Version: 1.0.5
+Version: 1.0.6
 Summary: A MACHINE LEARNING ANALYZER DEPLOYED INTO A WEBPAGE
 Home-page: https://github.com/havurquijo/Project-SCDB
 Download-URL: https://github.com/havurquijo/Project-SCDB/archive/refs/tags/v1.0.0-alpha.tar.gz
 Author: HERMES A V URQUIJO
 Author-email: hvurquijo@gmail.com
 License: AGPL 3.0
 Keywords: MACHINE,LEARNING,SCDB,SUPREME,COURT,WEBPAGE
```

## Comparing `SCDB_ML_app-1.0.5.dist-info/licenseheader.txt` & `SCDB_ML_app-1.0.6.dist-info/licenseheader.txt`

 * *Files identical despite different names*

## Comparing `SCDB_ML_app-1.0.5.dist-info/RECORD` & `SCDB_ML_app-1.0.6.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 flask_app/SCDB_ML_app.py,sha256=GRhwJaozxoC56Bg8_YbX8XM0lBbcNCncIcEQxxH1oaE,8079
 flask_app/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 flask_app/mine_decision_tree.py,sha256=SqAtrhZ16pVR4DaaNhFgRa8_XpI0C28fXcyTvz9t-JY,3982
 flask_app/predict_decision_tree.py,sha256=oaryXTg8g0q5df-7lYW2FD64n39UcUt2cJOBl5e7bCg,2165
 flask_app/train_decision_tree.py,sha256=mqRdrzxNnB9yzzaxtbKbVrPJJDjkGz5GfgE7Hb2Cw9g,2571
-scdb_ml_app/SCDB_ML_app.py,sha256=GRhwJaozxoC56Bg8_YbX8XM0lBbcNCncIcEQxxH1oaE,8079
+scdb_ml_app/SCDB_ML_app.py,sha256=mbBM6UsMC7I4GJcbtjvnUGcxDO3yrgauyILomhtRO_w,8082
 scdb_ml_app/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 scdb_ml_app/mine_decision_tree.py,sha256=SqAtrhZ16pVR4DaaNhFgRa8_XpI0C28fXcyTvz9t-JY,3982
 scdb_ml_app/predict_decision_tree.py,sha256=oaryXTg8g0q5df-7lYW2FD64n39UcUt2cJOBl5e7bCg,2165
 scdb_ml_app/train_decision_tree.py,sha256=mqRdrzxNnB9yzzaxtbKbVrPJJDjkGz5GfgE7Hb2Cw9g,2571
 scdb_ml_app/models/SCDB_2023_01_justiceCentered_Citation.csv.zip,sha256=53tcHjpQthNPjEBYmjCsfs_sr-6TiWcBiTNCkUrTlV8,1669742
 scdb_ml_app/models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 scdb_ml_app/models/accuracy_tree.txt,sha256=K3RkpKh9-QNYa8rcixBy2tvQdb7HpEynLrBf4Bg0kaw,26
@@ -31,13 +31,13 @@
 scdb_ml_app/templates/base.html,sha256=twvte2NM7x25X7K2FcqV4E7h9PkrrHMWxGZpEIW-sOs,11255
 scdb_ml_app/templates/index.html,sha256=0NlFm2e0FG-VaRkQ1EHpscoclBbglKF-i72vC6uSswc,44910
 scdb_ml_app/templates/mine_tree.html,sha256=MOqLlumSEnTDTGXHrX9LaFBFRpKAgjNkBvjAR039ANM,1920
 scdb_ml_app/templates/notFound.html,sha256=mOB1CgVNaXDNNrns5SG-t4ee6dGeTzc_iR1Jcr8nKak,1336
 scdb_ml_app/templates/predict_tree.html,sha256=0NBJN4mnBs0egBqXAZkngM_mS_2O6C05qCQGCebPqL0,4304
 scdb_ml_app/templates/predicted_tree.html,sha256=odDUHnh_mRlWlFLM1I6FtLb7ZN1iUpYjorbreaJCEh0,3468
 scdb_ml_app/templates/train_tree.html,sha256=kZC9uYco-H3tboXGo3G4hCj6RJQgfWwJF5lbpurxAJs,2655
-SCDB_ML_app-1.0.5.dist-info/LICENSE.txt,sha256=Hurj_dIXJ4vLhNNj6kGsyOLiyhuCSk3Aoa1E_7qn8mk,32005
-SCDB_ML_app-1.0.5.dist-info/METADATA,sha256=aJbAcC54TaFWcL6PUbYES9AVsgxKhXXVTrWEpQ8VvQw,892
-SCDB_ML_app-1.0.5.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-SCDB_ML_app-1.0.5.dist-info/licenseheader.txt,sha256=Y1KOyokTtaInPq-UZUQYIFQ__BTrUApFy7Ux76oDnpI,809
-SCDB_ML_app-1.0.5.dist-info/top_level.txt,sha256=Lv86V-a1LPhIMlWm2Hufd5a4AN-Te3aXzD7B4tI2jFc,12
-SCDB_ML_app-1.0.5.dist-info/RECORD,,
+SCDB_ML_app-1.0.6.dist-info/LICENSE.txt,sha256=Hurj_dIXJ4vLhNNj6kGsyOLiyhuCSk3Aoa1E_7qn8mk,32005
+SCDB_ML_app-1.0.6.dist-info/METADATA,sha256=GD65SR4RMjUeMJP335y6L-PCJ1s8j_pO50UE9iKBakE,892
+SCDB_ML_app-1.0.6.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+SCDB_ML_app-1.0.6.dist-info/licenseheader.txt,sha256=Y1KOyokTtaInPq-UZUQYIFQ__BTrUApFy7Ux76oDnpI,809
+SCDB_ML_app-1.0.6.dist-info/top_level.txt,sha256=Lv86V-a1LPhIMlWm2Hufd5a4AN-Te3aXzD7B4tI2jFc,12
+SCDB_ML_app-1.0.6.dist-info/RECORD,,
```

