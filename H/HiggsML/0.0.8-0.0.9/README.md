# Comparing `tmp/higgsml-0.0.8.tar.gz` & `tmp/higgsml-0.0.9.tar.gz`

## Comparing `higgsml-0.0.8.tar` & `higgsml-0.0.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 higgsml-0.0.8/HiggsML/__init__.py
--rw-r--r--   0        0        0     9247 2020-02-02 00:00:00.000000 higgsml-0.0.8/HiggsML/datasets.py
--rw-r--r--   0        0        0     6464 2020-02-02 00:00:00.000000 higgsml-0.0.8/HiggsML/ingestion.py
--rw-r--r--   0        0        0     9772 2020-02-02 00:00:00.000000 higgsml-0.0.8/HiggsML/score.py
--rw-r--r--   0        0        0    19932 2020-02-02 00:00:00.000000 higgsml-0.0.8/HiggsML/systematics.py
--rw-r--r--   0        0        0    12366 2020-02-02 00:00:00.000000 higgsml-0.0.8/HiggsML/visualization.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 higgsml-0.0.8/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 higgsml-0.0.8/LICENSE
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 higgsml-0.0.8/README.md
--rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 higgsml-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 higgsml-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 higgsml-0.0.9/HiggsML/__init__.py
+-rw-r--r--   0        0        0     9247 2020-02-02 00:00:00.000000 higgsml-0.0.9/HiggsML/datasets.py
+-rw-r--r--   0        0        0     6464 2020-02-02 00:00:00.000000 higgsml-0.0.9/HiggsML/ingestion.py
+-rw-r--r--   0        0        0     9678 2020-02-02 00:00:00.000000 higgsml-0.0.9/HiggsML/score.py
+-rw-r--r--   0        0        0    19933 2020-02-02 00:00:00.000000 higgsml-0.0.9/HiggsML/systematics.py
+-rw-r--r--   0        0        0    12366 2020-02-02 00:00:00.000000 higgsml-0.0.9/HiggsML/visualization.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 higgsml-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 higgsml-0.0.9/LICENSE
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 higgsml-0.0.9/README.md
+-rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 higgsml-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 higgsml-0.0.9/PKG-INFO
```

### Comparing `higgsml-0.0.8/HiggsML/datasets.py` & `higgsml-0.0.9/HiggsML/datasets.py`

 * *Files 2% similar despite different names*

```diff
@@ -236,15 +236,15 @@
     file_read_loc = os.path.join(current_path, "public_data")
     if not os.path.isdir(file_read_loc):
         os.mkdir(file_read_loc)
 
     file = "public_data.zip"
     if file not in os.listdir(file_read_loc):
         wget.download(
-            "https://www.codabench.org/datasets/download/2af33dff-7283-4256-8eda-2190a477c9ca/",
+            "https://www.codabench.org/datasets/download/58117a6d-af3a-4aa2-8e3d-f2848ea6db8b/",
             out=os.path.join(file_read_loc, "public_data.zip"),
         )
 
     if "input_data" not in os.listdir(file_read_loc):
         subprocess.run(
             ["unzip", os.path.join(file_read_loc, file), "-d", file_read_loc]
         )
@@ -261,15 +261,15 @@
     file_read_loc = os.path.join(current_path, "public_data")
     if not os.path.isdir(file_read_loc):
         os.mkdir(file_read_loc)
 
     file = "public_data.zip"
     if file not in os.listdir(file_read_loc):
         wget.download(
-            "https://www.codabench.org/datasets/download/a22b4d16-2cb6-4070-b10e-5778f4a9a365/",
+            "https://www.codabench.org/datasets/download/58117a6d-af3a-4aa2-8e3d-f2848ea6db8b/",
             out=os.path.join(file_read_loc, "public_data.zip"),
         )
 
     if "input_data" not in os.listdir(file_read_loc):
         subprocess.run(
             ["unzip", os.path.join(file_read_loc, file), "-d", file_read_loc]
         )
```

### Comparing `higgsml-0.0.8/HiggsML/ingestion.py` & `higgsml-0.0.9/HiggsML/ingestion.py`

 * *Files identical despite different names*

### Comparing `higgsml-0.0.8/HiggsML/score.py` & `higgsml-0.0.9/HiggsML/score.py`

 * *Files 9% similar despite different names*

```diff
@@ -55,37 +55,35 @@
     def load_ingestion_duration(self,ingestion_duration_file):
         print("[*] Reading ingestion duration")
         with open(ingestion_duration_file) as f:
             self.ingestion_duration = json.load(f)["ingestion_duration"]
 
         print("[✔]")
 
-    def load_ingestion_results(self, prediction_dir = "./"):
+    def load_ingestion_results(self, prediction_dir = "./",score_dir = "./"):
         print("[*] Reading predictions")
         self.ingestion_results = []
         # loop over sets (1 set = 1 value of mu)
         for file in os.listdir(prediction_dir):
             if file.startswith("result_"):
                 results_file = os.path.join(prediction_dir, file)
                 with open(results_file) as f:
                     self.ingestion_results.append(json.load(f))
         
-        self.score_file = os.path.join(prediction_dir, "scores.json")
-        self.html_file = os.path.join(prediction_dir, "detailed_results.html")
+        self.score_file = os.path.join(score_dir, "scores.json")
+        self.html_file = os.path.join(score_dir, "detailed_results.html")
 
         print("[✔]")
 
     def compute_scores(self, test_settings):
         print("[*] Computing scores")
 
         # loop over ingestion results
         rmses, maes = [], []
         all_p16s, all_p84s, all_mus = [], [], []
-        print("[*] ",self.ingestion_results)
-        print("[*] ",test_settings["ground_truth_mus"])
 
         for i in range(len(self.ingestion_results)):
             ingestion_result = self.ingestion_results[i]
             mu = test_settings["ground_truth_mus"][i]
             
             print(f"[*] mu_hats: {ingestion_result}")
             mu_hats = ingestion_result["mu_hats"]
```

### Comparing `higgsml-0.0.8/HiggsML/systematics.py` & `higgsml-0.0.9/HiggsML/systematics.py`

 * *Files 0% similar despite different names*

```diff
@@ -568,15 +568,15 @@
         if key is not "data":
             data_syst_set[key] = data_syst.pop(key)
     data_syst_set["data"] = data_syst
 
     return data_syst_set
 
 LHC_NUMBERS = {
-    "ztautau": 823327,
+    "ztautau": 3544019,
     "diboson": 40590,
     "ttbar": 158761,
     "htautau": 3639,
 }
 
 def get_bootstraped_dataset(
     test_set,
```

### Comparing `higgsml-0.0.8/HiggsML/visualization.py` & `higgsml-0.0.9/HiggsML/visualization.py`

 * *Files identical despite different names*

### Comparing `higgsml-0.0.8/.gitignore` & `higgsml-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `higgsml-0.0.8/LICENSE` & `higgsml-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `higgsml-0.0.8/README.md` & `higgsml-0.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,14 @@
 pip install HiggsML
 ```
 
 The Package consists of 5 modules :
 
 * 1 `ingestion`: This module contains the `Ingestion` class which takes case of the ingestion process of the competition. i.e. loading data into the model, initialization of the model, prediction etc. 
 * 2 `datasets` This module contains the `Data` class which has the train and test data in required formats, It loads the data according to the file format. it also contains function to make pseudo experiments. 
-* 3 `systematics` This module has functions to add systematics to the data with based in Neusance parameter like 
+* 3 `systematics` This module has functions to add systematics to the data with based in Nuisance parameter like 
     * Tau Hadron Energy scale
     * Jet Energy Scale 
     * Soft MET
     * W Background Normalisation
     * Overall Background Normalisation 
-* 4 `visualisation` This module contains the `Dataset_visualise` class which has methods to help visualise the data 
+* 4 `visualisation` This module contains the `Dataset_visualise` class which has methods to help visualise the data
```

### Comparing `higgsml-0.0.8/pyproject.toml` & `higgsml-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "HiggsML"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Ragansu Chakkappai", email="ragansu.chakkappai@universite-paris-saclay.fr"},
   { name="David Rousseau", email="david.rousseau@uijclab.in2p3.fr" },
   { name="V. Estrade", email="v.estrade@centralesupelec.fr" },
   { name="Ihsan Ullah", email="ihsan.ullah@universite-paris-saclay.fr"}
 ]
 description = "A Black Swan test package"
```

### Comparing `higgsml-0.0.8/PKG-INFO` & `higgsml-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: HiggsML
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Black Swan test package
 Project-URL: Homepage, https://github.com/blackSwanCS/black_swan_pkg
 Project-URL: Issues, https://github.com/blackSwanCS/black_swan_pkg/issues
 Author-email: Ragansu Chakkappai <ragansu.chakkappai@universite-paris-saclay.fr>, David Rousseau <david.rousseau@uijclab.in2p3.fr>, "V. Estrade" <v.estrade@centralesupelec.fr>, Ihsan Ullah <ihsan.ullah@universite-paris-saclay.fr>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -27,14 +27,14 @@
 pip install HiggsML
 ```
 
 The Package consists of 5 modules :
 
 * 1 `ingestion`: This module contains the `Ingestion` class which takes case of the ingestion process of the competition. i.e. loading data into the model, initialization of the model, prediction etc. 
 * 2 `datasets` This module contains the `Data` class which has the train and test data in required formats, It loads the data according to the file format. it also contains function to make pseudo experiments. 
-* 3 `systematics` This module has functions to add systematics to the data with based in Neusance parameter like 
+* 3 `systematics` This module has functions to add systematics to the data with based in Nuisance parameter like 
     * Tau Hadron Energy scale
     * Jet Energy Scale 
     * Soft MET
     * W Background Normalisation
     * Overall Background Normalisation 
-* 4 `visualisation` This module contains the `Dataset_visualise` class which has methods to help visualise the data 
+* 4 `visualisation` This module contains the `Dataset_visualise` class which has methods to help visualise the data
```

