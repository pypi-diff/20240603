# Comparing `tmp/TiRank-0.1.tar.gz` & `tmp/tirank-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TiRank-0.1.tar", last modified: Thu Jan 18 05:00:20 2024, max compression
+gzip compressed data, was "tirank-0.1.4.tar", last modified: Mon Jun  3 11:43:42 2024, max compression
```

## Comparing `TiRank-0.1.tar` & `tirank-0.1.4.tar`

### file list

```diff
@@ -1,23 +1,50 @@
-drwxrwxr-x   0 lenislin  (1000) lenislin  (1000)        0 2024-01-18 05:00:20.532778 TiRank-0.1/
--rw-rw-r--   0 lenislin  (1000) lenislin  (1000)     1055 2024-01-17 08:21:02.000000 TiRank-0.1/LICENSE
--rw-r--r--   0 lenislin  (1000) lenislin  (1000)     2719 2024-01-18 05:00:20.532778 TiRank-0.1/PKG-INFO
--rw-rw-r--   0 lenislin  (1000) lenislin  (1000)     1712 2024-01-18 04:59:07.000000 TiRank-0.1/README.md
-drwxrwxr-x   0 lenislin  (1000) lenislin  (1000)        0 2024-01-18 05:00:20.532778 TiRank-0.1/TiRank/
--rw-rw-r--   0 lenislin  (1000) lenislin  (1000)    10018 2024-01-17 09:33:38.000000 TiRank-0.1/TiRank/Dataloader.py
--rw-rw-r--   0 lenislin  (1000) lenislin  (1000)    14816 2024-01-17 09:22:12.000000 TiRank-0.1/TiRank/GPextractor.py
--rw-rw-r--   0 lenislin  (1000) lenislin  (1000)     7175 2024-01-17 12:58:48.000000 TiRank-0.1/TiRank/Imageprocessing.py
--rw-rw-r--   0 lenislin  (1000) lenislin  (1000)     2914 2024-01-17 12:17:30.000000 TiRank-0.1/TiRank/LoadData.py
--rw-rw-r--   0 lenislin  (1000) lenislin  (1000)     4551 2024-01-17 09:33:12.000000 TiRank-0.1/TiRank/Loss.py
--rw-rw-r--   0 lenislin  (1000) lenislin  (1000)    10978 2024-01-17 09:23:04.000000 TiRank-0.1/TiRank/Model.py
--rw-rw-r--   0 lenislin  (1000) lenislin  (1000)     9007 2024-01-17 08:21:02.000000 TiRank-0.1/TiRank/SCSTpreprocess.py
--rw-rw-r--   0 lenislin  (1000) lenislin  (1000)    31101 2024-01-17 09:23:07.000000 TiRank-0.1/TiRank/TrainPre.py
--rw-rw-r--   0 lenislin  (1000) lenislin  (1000)    13380 2024-01-17 09:23:10.000000 TiRank-0.1/TiRank/Visualization.py
--rw-rw-r--   0 lenislin  (1000) lenislin  (1000)      577 2024-01-17 09:36:46.000000 TiRank-0.1/TiRank/__init__.py
-drwxrwxr-x   0 lenislin  (1000) lenislin  (1000)        0 2024-01-18 05:00:20.532778 TiRank-0.1/TiRank.egg-info/
--rw-r--r--   0 lenislin  (1000) lenislin  (1000)     2719 2024-01-18 05:00:20.000000 TiRank-0.1/TiRank.egg-info/PKG-INFO
--rw-rw-r--   0 lenislin  (1000) lenislin  (1000)      381 2024-01-18 05:00:20.000000 TiRank-0.1/TiRank.egg-info/SOURCES.txt
--rw-rw-r--   0 lenislin  (1000) lenislin  (1000)        1 2024-01-18 05:00:20.000000 TiRank-0.1/TiRank.egg-info/dependency_links.txt
--rw-rw-r--   0 lenislin  (1000) lenislin  (1000)      288 2024-01-18 05:00:20.000000 TiRank-0.1/TiRank.egg-info/requires.txt
--rw-rw-r--   0 lenislin  (1000) lenislin  (1000)        7 2024-01-18 05:00:20.000000 TiRank-0.1/TiRank.egg-info/top_level.txt
--rw-rw-r--   0 lenislin  (1000) lenislin  (1000)       38 2024-01-18 05:00:20.532778 TiRank-0.1/setup.cfg
--rw-rw-r--   0 lenislin  (1000) lenislin  (1000)     1642 2024-01-18 04:52:44.000000 TiRank-0.1/setup.py
+drwxrwxr-x   0 lenislin  (1000) lenislin  (1000)        0 2024-06-03 11:43:42.920971 tirank-0.1.4/
+-rw-rw-r--   0 lenislin  (1000) lenislin  (1000)     1055 2024-06-03 07:46:12.000000 tirank-0.1.4/LICENSE
+-rw-r--r--   0 lenislin  (1000) lenislin  (1000)     9089 2024-06-03 11:43:42.920971 tirank-0.1.4/PKG-INFO
+-rw-rw-r--   0 lenislin  (1000) lenislin  (1000)     7997 2024-06-03 07:46:12.000000 tirank-0.1.4/README.md
+drwxrwxr-x   0 lenislin  (1000) lenislin  (1000)        0 2024-06-03 11:43:42.920971 tirank-0.1.4/TiRank/
+-rw-rw-r--   0 lenislin  (1000) lenislin  (1000)    11508 2024-06-03 07:46:12.000000 tirank-0.1.4/TiRank/Dataloader.py
+-rw-rw-r--   0 lenislin  (1000) lenislin  (1000)    14422 2024-06-03 07:46:12.000000 tirank-0.1.4/TiRank/GPextractor.py
+-rw-rw-r--   0 lenislin  (1000) lenislin  (1000)     7226 2024-06-03 07:46:12.000000 tirank-0.1.4/TiRank/Imageprocessing.py
+-rw-rw-r--   0 lenislin  (1000) lenislin  (1000)     2914 2024-06-03 07:46:12.000000 tirank-0.1.4/TiRank/LoadData.py
+-rw-rw-r--   0 lenislin  (1000) lenislin  (1000)     4551 2024-06-03 07:46:12.000000 tirank-0.1.4/TiRank/Loss.py
+-rw-rw-r--   0 lenislin  (1000) lenislin  (1000)    10972 2024-06-03 07:46:12.000000 tirank-0.1.4/TiRank/Model.py
+-rw-rw-r--   0 lenislin  (1000) lenislin  (1000)     9003 2024-06-03 07:46:12.000000 tirank-0.1.4/TiRank/SCSTpreprocess.py
+-rw-rw-r--   0 lenislin  (1000) lenislin  (1000)    31184 2024-06-03 07:46:12.000000 tirank-0.1.4/TiRank/TrainPre.py
+-rw-rw-r--   0 lenislin  (1000) lenislin  (1000)    23386 2024-06-03 07:46:12.000000 tirank-0.1.4/TiRank/Visualization.py
+-rw-rw-r--   0 lenislin  (1000) lenislin  (1000)      639 2024-06-03 09:09:41.000000 tirank-0.1.4/TiRank/__init__.py
+-rw-rw-r--   0 lenislin  (1000) lenislin  (1000)    38171 2024-06-03 11:23:16.000000 tirank-0.1.4/TiRank/app.py
+drwxrwxr-x   0 lenislin  (1000) lenislin  (1000)        0 2024-06-03 11:43:42.920971 tirank-0.1.4/TiRank/components/
+-rw-rw-r--   0 lenislin  (1000) lenislin  (1000)      211 2024-06-03 09:25:14.000000 tirank-0.1.4/TiRank/components/__init__.py
+-rw-rw-r--   0 lenislin  (1000) lenislin  (1000)    14965 2024-06-03 07:46:12.000000 tirank-0.1.4/TiRank/components/modes.py
+-rw-rw-r--   0 lenislin  (1000) lenislin  (1000)     1715 2024-06-03 07:46:12.000000 tirank-0.1.4/TiRank/ctran.py
+drwxrwxr-x   0 lenislin  (1000) lenislin  (1000)        0 2024-06-03 11:43:42.920971 tirank-0.1.4/TiRank/layout/
+-rw-rw-r--   0 lenislin  (1000) lenislin  (1000)      500 2024-06-03 09:24:07.000000 tirank-0.1.4/TiRank/layout/__init__.py
+-rw-rw-r--   0 lenislin  (1000) lenislin  (1000)     9296 2024-06-03 07:46:12.000000 tirank-0.1.4/TiRank/layout/degpe.py
+-rw-rw-r--   0 lenislin  (1000) lenislin  (1000)      839 2024-06-03 07:46:12.000000 tirank-0.1.4/TiRank/layout/faq.py
+-rw-rw-r--   0 lenislin  (1000) lenislin  (1000)      515 2024-06-03 07:46:12.000000 tirank-0.1.4/TiRank/layout/homepage.py
+-rw-rw-r--   0 lenislin  (1000) lenislin  (1000)     7407 2024-06-03 07:46:12.000000 tirank-0.1.4/TiRank/layout/others.py
+-rw-rw-r--   0 lenislin  (1000) lenislin  (1000)    20236 2024-06-03 07:46:12.000000 tirank-0.1.4/TiRank/layout/preprocess.py
+-rw-rw-r--   0 lenislin  (1000) lenislin  (1000)     8852 2024-06-03 07:46:12.000000 tirank-0.1.4/TiRank/layout/tirank.py
+-rw-rw-r--   0 lenislin  (1000) lenislin  (1000)    31920 2024-06-03 07:46:12.000000 tirank-0.1.4/TiRank/layout/tutorial.py
+-rw-rw-r--   0 lenislin  (1000) lenislin  (1000)    23612 2024-06-03 07:46:12.000000 tirank-0.1.4/TiRank/layout/upload.py
+-rw-rw-r--   0 lenislin  (1000) lenislin  (1000)     4237 2024-06-03 07:46:12.000000 tirank-0.1.4/TiRank/main.py
+drwxrwxr-x   0 lenislin  (1000) lenislin  (1000)        0 2024-06-03 11:43:42.920971 tirank-0.1.4/TiRank/tirankWeb/
+-rw-rw-r--   0 lenislin  (1000) lenislin  (1000)      578 2024-06-03 09:07:10.000000 tirank-0.1.4/TiRank/tirankWeb/__init__.py
+-rw-rw-r--   0 lenislin  (1000) lenislin  (1000)    15062 2024-06-03 07:46:12.000000 tirank-0.1.4/TiRank/tirankWeb/dataloader.py
+-rw-rw-r--   0 lenislin  (1000) lenislin  (1000)    15024 2024-06-03 11:06:52.000000 tirank-0.1.4/TiRank/tirankWeb/gpextractor.py
+-rw-rw-r--   0 lenislin  (1000) lenislin  (1000)     7151 2024-06-03 09:08:23.000000 tirank-0.1.4/TiRank/tirankWeb/imageprocessing.py
+-rw-rw-r--   0 lenislin  (1000) lenislin  (1000)     1776 2024-06-03 09:08:20.000000 tirank-0.1.4/TiRank/tirankWeb/loaddata.py
+-rw-rw-r--   0 lenislin  (1000) lenislin  (1000)     4551 2024-06-03 07:46:12.000000 tirank-0.1.4/TiRank/tirankWeb/loss.py
+-rw-rw-r--   0 lenislin  (1000) lenislin  (1000)    10779 2024-06-03 09:08:18.000000 tirank-0.1.4/TiRank/tirankWeb/model.py
+-rw-rw-r--   0 lenislin  (1000) lenislin  (1000)     4097 2024-06-03 07:46:12.000000 tirank-0.1.4/TiRank/tirankWeb/scstpreprocess.py
+-rw-rw-r--   0 lenislin  (1000) lenislin  (1000)    28413 2024-06-03 09:08:16.000000 tirank-0.1.4/TiRank/tirankWeb/trainpre.py
+-rw-rw-r--   0 lenislin  (1000) lenislin  (1000)    17143 2024-06-03 07:46:12.000000 tirank-0.1.4/TiRank/tirankWeb/visualization.py
+drwxrwxr-x   0 lenislin  (1000) lenislin  (1000)        0 2024-06-03 11:43:42.920971 tirank-0.1.4/TiRank.egg-info/
+-rw-r--r--   0 lenislin  (1000) lenislin  (1000)     9089 2024-06-03 11:43:42.000000 tirank-0.1.4/TiRank.egg-info/PKG-INFO
+-rw-rw-r--   0 lenislin  (1000) lenislin  (1000)     1011 2024-06-03 11:43:42.000000 tirank-0.1.4/TiRank.egg-info/SOURCES.txt
+-rw-rw-r--   0 lenislin  (1000) lenislin  (1000)        1 2024-06-03 11:43:42.000000 tirank-0.1.4/TiRank.egg-info/dependency_links.txt
+-rw-rw-r--   0 lenislin  (1000) lenislin  (1000)      317 2024-06-03 11:43:42.000000 tirank-0.1.4/TiRank.egg-info/requires.txt
+-rw-rw-r--   0 lenislin  (1000) lenislin  (1000)        7 2024-06-03 11:43:42.000000 tirank-0.1.4/TiRank.egg-info/top_level.txt
+-rw-rw-r--   0 lenislin  (1000) lenislin  (1000)       38 2024-06-03 11:43:42.920971 tirank-0.1.4/setup.cfg
+-rw-rw-r--   0 lenislin  (1000) lenislin  (1000)     1982 2024-06-03 11:41:40.000000 tirank-0.1.4/setup.py
```

### Comparing `TiRank-0.1/LICENSE` & `tirank-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `TiRank-0.1/TiRank/Dataloader.py` & `tirank-0.1.4/TiRank/Dataloader.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,57 +2,81 @@
 import numpy as np
 import pandas as pd
 import random, pickle, os
 
 import torch
 from torch.utils.data import Dataset, DataLoader
 
-def view_clinical_variables(savePath):
-    savePath_1 = os.path.join(savePath,"1_loaddata")
+# def view_clinical_variables(savePath):
+#     savePath_1 = os.path.join(savePath,"1_loaddata")
 
-    # Load data
-    f = open(os.path.join(savePath_1, 'bulk_clinical.pkl'), 'rb')
-    bulkClinical = pickle.load(f)
-    f.close()
+#     # Load data
+#     f = open(os.path.join(savePath_1, 'bulk_clinical.pkl'), 'rb')
+#     bulkClinical = pickle.load(f)
+#     f.close()
 
-    print(bulkClinical.columns)
+#     print(bulkClinical.columns)
 
-    return bulkClinical
+#     return bulkClinical
 
-def choose_clinical_variable(savePath, bulkClinical, mode, var_1, var_2 = None):
-    savePath_2 = os.path.join(savePath,"2_preprocessing")
+# def assign_binary_values(df, column_name):
+#     # transfer into dataframe
+#     df = pd.DataFrame(df)
 
-    # selecting mode
-    if mode == "Cox":
-        Time_col = var_1
-        Status_col = var_2
-        bulkClinical = bulkClinical.loc[:,[Time_col,Status_col]]
-
-    elif mode == "Bionomial" or "Regression":
-        Variable_col = var_1
-        bulkClinical = bulkClinical.loc[:,Variable_col]
+#     # Ensure the column exists in the DataFrame
+#     if column_name not in df.columns:
+#         raise ValueError(f"Column '{column_name}' not found in DataFrame.")
 
-    else:
-        raise(TypeError("Unexpected Mode had been selected."))
+#     # Step 1: Identify the unique categories in the specified column
+#     unique_categories = df[column_name].unique().tolist()
+    
+#     # Safety check: Ensure there are only two unique categories
+#     if len(unique_categories) != 2:
+#         raise ValueError("The column does not contain exactly two unique categories.")
+    
+#     # Step 2: Assign numerical values to these categories
+#     category_to_number = {unique_categories[0]: 0, unique_categories[1]: 1}
+    
+#     # Convert the specified column in the DataFrame based on the detected categories
+#     df[column_name] = df[column_name].map(category_to_number)
+    
+#     return df, category_to_number
 
-    with open(os.path.join(savePath_2, 'bulk_clinical.pkl'), 'wb') as f:
-        pickle.dump(bulkClinical, f)
-    f.close()
+# def choose_clinical_variable(savePath, bulkClinical, mode, var_1, var_2 = None):
+# def choose_clinical_variable(savePath, bulkClinical):
+#     savePath_2 = os.path.join(savePath,"2_preprocessing")
+
+#     # selecting mode
+#     if mode == "Cox":
+#         Time_col = var_1
+#         Status_col = var_2
+#     elif mode == "Classification" or "Regression":
+
+#     elif mode == "Regression":
+#         Variable_col = var_1
+#         bulkClinical = bulkClinical.loc[:,Variable_col]
+
+#     else:
+#         raise(TypeError("Unexpected Mode had been selected."))
+
+#     with open(os.path.join(savePath_2, 'bulk_clinical.pkl'), 'wb') as f:
+#         pickle.dump(bulkClinical, f)
+#     f.close()
 
-    return None
+#     return None
 
 def generate_val(savePath, validation_proportion=0.15, mode =  None):
     savePath_1 = os.path.join(savePath,"1_loaddata")
     savePath_2 = os.path.join(savePath,"2_preprocessing")
 
     f = open(os.path.join(savePath_1, 'bulk_exp.pkl'), 'rb')
     bulkExp = pickle.load(f)
     f.close()
     
-    f = open(os.path.join(savePath_2, 'bulk_clinical.pkl'), 'rb')
+    f = open(os.path.join(savePath_1, 'bulk_clinical.pkl'), 'rb')
     bulkClinical = pickle.load(f)
     f.close()
 
     # Load data
     bulkExp, bulkClinical
     # Transpose bulkExp so that samples are rows
     bulkExp_transposed = bulkExp.T
@@ -65,29 +89,38 @@
     num_val = int(combined.shape[0] * validation_proportion)
     validx = random.sample(range(combined.shape[0]),num_val)
 
     combined_val = combined.iloc[validx,]
     mask = ~combined.index.isin(combined_val.index)
     combined_train = combined[mask]
 
-    if mode == "Bionomial":
+    if mode == "Classification":
+    # if mode == "Bionomial":
         # Separate the training and validation sets back into bulkExp and bulkClinical
         bulkExp_train = combined_train.iloc[:, :-1].T
         bulkClinical_train = combined_train.iloc[:, -1]
 
         bulkExp_val = combined_val.iloc[:, :-1].T
         bulkClinical_val = combined_val.iloc[:, -1]
     
     elif mode == "Cox":
         # Separate the training and validation sets back into bulkExp and bulkClinical
         bulkExp_train = combined_train.iloc[:, :-2].T
         bulkClinical_train = combined_train.iloc[:, -2:]
 
         bulkExp_val = combined_val.iloc[:, :-2].T
-        bulkClinical_val = combined_val.iloc[:, -2:]       
+        bulkClinical_val = combined_val.iloc[:, -2:]
+
+    elif mode == "Regression":
+        # Separate the training and validation sets back into bulkExp and bulkClinical
+        bulkExp_train = combined_train.iloc[:, :-1].T
+        bulkClinical_train = combined_train.iloc[:, -1]
+
+        bulkExp_val = combined_val.iloc[:, :-1].T
+        bulkClinical_val = combined_val.iloc[:, -1]      
 
     ## save
     savePath_splitData = os.path.join(savePath_2,"split_data")
     if not os.path.exists(savePath_splitData):
         os.makedirs(savePath_splitData,exist_ok=True)
 
     with open(os.path.join(savePath_splitData, 'bulkExp_train.pkl'), 'wb') as f:
@@ -118,15 +151,16 @@
         if mode == 'Cox':
             self.Xa = torch.tensor(df_Xa.values, dtype=torch.float32)
 
             # Handle 'Cox' type: df_cli is expected to be a DataFrame with columns ['t', 'e']
             self.t = torch.tensor(df_cli.iloc[:,0].values, dtype=torch.float32)
             self.e = torch.tensor(df_cli.iloc[:,1].values, dtype=torch.float32)
 
-        elif mode == 'Bionomial':
+        # elif mode == 'Bionomial':
+        elif mode == 'Classification':
             self.Xa = torch.tensor(df_Xa.values, dtype=torch.float32)
 
             # Handle 'Bionomial' type: df_cli is expected to be a Series/1D array with group labels
             self.label = torch.tensor(df_cli.iloc[:,0].values, dtype=torch.long)
 
         elif mode == 'Regression':
             self.Xa = torch.tensor(df_Xa.values, dtype=torch.float32)
@@ -207,25 +241,26 @@
     similarity_df = pickle.load(f)
     f.close() 
 
     train_dataset_Bulk = BulkDataset(train_bulk_gene_pairs_mat, bulkClinical_train, mode=mode)
     val_dataset_Bulk = BulkDataset(val_bulkExp_gene_pairs_mat, bulkClinical_val, mode=mode)
     train_loader_Bulk = DataLoader(train_dataset_Bulk, batch_size=batch_size, shuffle=False)
     val_loader_Bulk = DataLoader(val_dataset_Bulk, batch_size=batch_size, shuffle=False)
-
-
-    if infer_mode == "Spot":
+    
+    if infer_mode == "ST":
+    # if infer_mode == "Spot":
         adj_A = torch.from_numpy(similarity_df.values)
         adj_B = None
         patholabels = scAnndata.obs["patho_class"]
 
         train_dataset_SC = STDataset(sc_gene_pairs_mat)
         train_loader_SC = DataLoader(train_dataset_SC, batch_size=batch_size, shuffle=True)
 
-    elif infer_mode == "Cell":
+    elif infer_mode == "SC":
+    # elif infer_mode == "Cell":
         adj_A = torch.from_numpy(similarity_df.values)
         adj_B = None
         patholabels = None
 
         train_dataset_SC = STDataset(sc_gene_pairs_mat)
         train_loader_SC = DataLoader(train_dataset_SC, batch_size=batch_size, shuffle=True)
```

### Comparing `TiRank-0.1/TiRank/GPextractor.py` & `tirank-0.1.4/TiRank/tirankWeb/gpextractor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,84 +1,85 @@
-# Gene-pairs (GP) extractor
-
 import numpy as np
 import pandas as pd
-import os,pickle
+import os, pickle
 
 from lifelines import CoxPHFitter
 from scipy.stats import pearsonr, ttest_ind
 from statsmodels.stats.multitest import multipletests
+from .visualization import plot_genepair
 
-from .Dataloader import transform_test_exp
+from .dataloader import transform_test_exp_
 
 
-class GenePairExtractor():
-    def __init__(self, savePath, analysis_mode, top_var_genes=500, top_gene_pairs=2000, p_value_threshold=None, padj_value_threshold=None, max_cutoff=0.8, min_cutoff=0.2):
-        self.savePath = savePath
+class GenePairExtractor:
+    def __init__(self, save_path, analysis_mode, top_var_genes=500, top_gene_pairs=2000, p_value_threshold=None,
+                 padj_value_threshold=None, max_cutoff=0.8, min_cutoff=0.2):
+        self.savePath = save_path
         self.analysis_mode = analysis_mode
         self.top_var_genes = top_var_genes
         self.top_gene_pairs = top_gene_pairs
         self.p_value_threshold = p_value_threshold
         self.padj_value_threshold = padj_value_threshold
         self.max_cutoff = max_cutoff
         self.min_cutoff = min_cutoff
+        self.is_empty = 0
 
     def load_data(self):
         print(f"Starting load data for gene pair transformation.")
-        savePath_2 = os.path.join(self.savePath,"2_preprocessing")
-        savePath_splitData = os.path.join(savePath_2,"split_data")
+        save_path = self.savePath
+        savePath_splitData = os.path.join(save_path, "split_data")
 
         ## bulk
         f = open(os.path.join(savePath_splitData, 'bulkExp_train.pkl'), 'rb')
         self.bulk_expression = pickle.load(f)
         f.close()
         f = open(os.path.join(savePath_splitData, 'bulkClinical_train.pkl'), 'rb')
         self.clinical_data = pickle.load(f)
         f.close()
 
         ## sc
-        f = open(os.path.join(savePath_2, 'scAnndata.pkl'), 'rb')
+        f = open(os.path.join(save_path, 'scAnndata.pkl'), 'rb')
         scAnndata = pickle.load(f)
         f.close()
 
         if type(scAnndata.X) == type(np.array(1)):
             scExp = pd.DataFrame(scAnndata.X.T)
         else:
             scExp = pd.DataFrame(scAnndata.X.toarray().T)
 
         scExp.index = scAnndata.var_names
         scExp.columns = scAnndata.obs.index
         self.single_cell_expression = scExp
 
         return None
-    
+
     def save_data(self):
         print(f"Starting save gene pair matrices.")
-        savePath_2 = os.path.join(self.savePath,"2_preprocessing")
-        savePath_splitData = os.path.join(savePath_2,"split_data")
+        save_path = self.savePath
+        savePath_splitData = os.path.join(save_path, "split_data")
 
         ## Load val bulk
         f = open(os.path.join(savePath_splitData, 'bulkExp_val.pkl'), 'rb')
         bulkExp_val = pickle.load(f)
         f.close()
 
         train_bulk_gene_pairs_mat = pd.DataFrame(self.bulk_gene_pairs_mat.T)
-        val_bulkExp_gene_pairs_mat = transform_test_exp(train_exp = train_bulk_gene_pairs_mat,test_exp = bulkExp_val)
+        val_bulkExp_gene_pairs_mat = transform_test_exp_(train_exp=train_bulk_gene_pairs_mat, test_exp=bulkExp_val)
         sc_gene_pairs_mat = pd.DataFrame(self.single_cell_gene_pairs_mat.T)
 
-        with open(os.path.join(savePath_2, 'train_bulk_gene_pairs_mat.pkl'), 'wb') as f:
-            pickle.dump(train_bulk_gene_pairs_mat, f) ## training bulk gene pair matrix
+        with open(os.path.join(save_path, 'train_bulk_gene_pairs_mat.pkl'), 'wb') as f:
+            pickle.dump(train_bulk_gene_pairs_mat, f)  ## training bulk gene pair matrix
         f.close()
 
-        with open(os.path.join(savePath_2, 'val_bulkExp_gene_pairs_mat.pkl'), 'wb') as f:
-            pickle.dump(val_bulkExp_gene_pairs_mat, f) ## validating bulk gene pair matrix
+        with open(os.path.join(save_path, 'val_bulkExp_gene_pairs_mat.pkl'), 'wb') as f:
+            pickle.dump(val_bulkExp_gene_pairs_mat, f)  ## validating bulk gene pair matrix
         f.close()
 
-        with open(os.path.join(savePath_2, 'sc_gene_pairs_mat.pkl'), 'wb') as f:
-            pickle.dump(sc_gene_pairs_mat, f) ## single cell gene pair matrix
+        with open(os.path.join(save_path, 'sc_gene_pairs_mat.pkl'), 'wb') as f:
+            pickle.dump(sc_gene_pairs_mat, f)  ## single cell gene pair matrix
         f.close()
         print(f"Save gene pair matrices done.")
 
         return None
 
     def run_extraction(self):
         print(f"Starting gene pair extraction.")
@@ -98,32 +99,36 @@
         # Extract the candidate genes
         self.bulk_expression, self.single_cell_expression = self.extract_candidate_genes(
             top_variable_genes)
 
         print(f"Get candidate genes done.")
 
         # Obtain the list of candidate genes
-        if self.analysis_mode == "Bionomial":
+        if self.analysis_mode == "Classification":
             regulated_genes_r, regulated_genes_p = self.calculate_binomial_gene_pairs()
-            print(f"There are {len(regulated_genes_r)} genes up-regulated in Group 0 and {len(regulated_genes_p)} genes up-regulated in Group 1.")
+            print(
+                f"There are {len(regulated_genes_r)} genes up-regulated in Group 0"
+                f" and {len(regulated_genes_p)} genes up-regulated in Group 1.")
 
         elif self.analysis_mode == "Cox":
             regulated_genes_r, regulated_genes_p = self.calculate_survival_gene_pairs()
             print(f"There are {len(regulated_genes_r)} Risk genes and {len(regulated_genes_p)} Protective genes.")
 
         elif self.analysis_mode == "Regression":
             regulated_genes_r, regulated_genes_p = self.calculate_regression_gene_pairs()
-            print(f"There are {len(regulated_genes_r)} positive-associated genes and {len(regulated_genes_p)} negative-associated genes.")
+            print(
+                f"There are {len(regulated_genes_r)} positive-associated gene"
+                f"s and {len(regulated_genes_p)} negative-associated genes.")
 
         else:
             raise ValueError(f"Unsupported mode: {self.analysis_mode}")
 
         if (len(regulated_genes_r) == 0) or (len(regulated_genes_p) == 0):
-            raise ValueError(
-                "A set of genes is empty. Try increasing the 'top_var_genes' value or loosening the 'p.value' threshold.")
+            self.is_empty = 1
+            return None
 
         print(f"Get candidate gene pairs done.")
 
         # Transform the bulk gene pairs
         bulk_gene_pairs = self.transform_bulk_gene_pairs(
             regulated_genes_r, regulated_genes_p)
         # Filter the gene pairs
@@ -135,24 +140,28 @@
 
         print(f"Profile transformation done.")
 
         # Return the bulk and single-cell gene pairs
         self.bulk_gene_pairs_mat = bulk_gene_pairs_mat
         self.single_cell_gene_pairs_mat = single_cell_gene_pairs_mat
 
+        # Visualize the gene pair
+        plot_genepair(self.bulk_gene_pairs_mat, "bulk", './assets')
+        plot_genepair(self.single_cell_gene_pairs_mat, "sc", './assets')
+
         return None
 
     def extract_candidate_genes(self, gene_names):
         # Construct gene pairs
         single_cell_gene_subset = self.single_cell_expression.loc[gene_names]
         bulk_gene_subset = self.bulk_expression.loc[gene_names, :]
 
         # Remove rows in bulk dataset where all entries are 0
         bulk_gene_subset = bulk_gene_subset.loc[(
-            bulk_gene_subset != 0).any(axis=1)]
+                bulk_gene_subset != 0).any(axis=1)]
         gene_names = bulk_gene_subset.index.tolist()
         single_cell_gene_subset = single_cell_gene_subset.loc[gene_names]
 
         return bulk_gene_subset, single_cell_gene_subset
 
     def calculate_binomial_gene_pairs(self):
         # Calculate group means and perform t-test
@@ -177,15 +186,15 @@
             'gene': self.bulk_expression.index
         })
 
         # Drop the row which p_values is NULL
         DEGs = DEGs.dropna()
 
         # Adjust p-values for multiple testing
-        DEGs['adj.P.Val'] = multipletests(DEGs['P.Value'], method='fdr_bh')[1]
+        # DEGs['adj.P.Val'] = multipletests(DEGs['P.Value'], method='fdr_bh')[1]
 
         # Filter significant genes
         if (self.p_value_threshold is None) and (self.padj_value_threshold is not None):
             DEGs = DEGs[DEGs['adj.P.Val'] < self.padj_value_threshold]
         elif (self.p_value_threshold is not None) and (self.padj_value_threshold is None):
             DEGs = DEGs[DEGs['P.Value'] < self.p_value_threshold]
         else:
@@ -242,18 +251,17 @@
             columns=["gene", "correlation", "pvalue"])
         for i in range(self.bulk_expression.shape[0]):
             exp_gene = self.bulk_expression.iloc[i, :].astype(float)
             correlation, pvalue = pearsonr(
                 exp_gene, self.clinical_data.iloc[:, 0])
 
             correlation_results = pd.concat([
-                correlation_results,pd.Series({"gene": self.bulk_expression.index[i], 
-                "correlation": correlation, 
-                "pvalue": pvalue}).to_frame().T], axis=0, ignore_index=True)
-
+                correlation_results, pd.Series({"gene": self.bulk_expression.index[i],
+                                                "correlation": correlation,
+                                                "pvalue": pvalue}).to_frame().T], axis=0, ignore_index=True)
 
         correlation_results = correlation_results.dropna()
         correlation_results["correlation"] = correlation_results["correlation"].astype(
             float)
         correlation_results["pvalue"] = correlation_results["pvalue"].astype(
             float)
```

### Comparing `TiRank-0.1/TiRank/Imageprocessing.py` & `tirank-0.1.4/TiRank/Imageprocessing.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from torchvision.transforms import functional as F
 
 import numpy as np
 from sklearn.decomposition import PCA
 from sklearn.cluster import KMeans
 from itertools import repeat
 import collections.abc
+import os
 
 def _ntuple(n):
     def parse(x):
         if isinstance(x, collections.abc.Iterable):
             return x
         return tuple(repeat(x, n))
     return parse
@@ -171,15 +172,15 @@
     plt.legend()
     plt.xlabel("Image Column")
     plt.ylabel("Image Row")
     plt.title("Patho Class Heatmap")
     
     # Display the plot
     plt.gca().invert_yaxis()  # Invert y-axis for typical image display
-    plt.savefig(save_path)
+    plt.savefig(os.path.join(save_path, 'patho_class_heatmap.png'))
     return None
 
 def GetPathoClass(adata, pretrain_path, n_components = 50, n_clusters = 6, plot_classes = True, image_save_path = None):
     images = crop_images(adata)
     features = infer_by_pretrain(images, pretrain_path)
 
     # Example values for PCA and clustering
```

### Comparing `TiRank-0.1/TiRank/LoadData.py` & `tirank-0.1.4/TiRank/LoadData.py`

 * *Files identical despite different names*

### Comparing `TiRank-0.1/TiRank/Loss.py` & `tirank-0.1.4/TiRank/Loss.py`

 * *Files identical despite different names*

### Comparing `TiRank-0.1/TiRank/Model.py` & `tirank-0.1.4/TiRank/Model.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,18 +26,17 @@
         savePath,
         nhead = 2,
         nhid1=96, 
         nhid2=8, 
         n_output=32,
         nlayers=3,
         n_pred=1, 
-        n_patho=0,
         dropout=0.5,
         mode = "Cox",
-        infer_mode="Cell",
+        infer_mode="SC",
         encoder_type = "MLP"
 ):
     savePath_2 = os.path.join(savePath,"2_preprocessing")
     savePath_3 = os.path.join(savePath,"3_Analysis")
     savePath_data2train = os.path.join(savePath_3,"data2train")
 
     ## Load train bulk gene pair matrix 
@@ -282,17 +281,17 @@
     def forward(self, embedding):
         pathology_score = F.softmax(self.PathologyMLP(embedding))
         return pathology_score
 
 # Main network
 
 
-class TiRank(nn.Module):
+class TiRankModel(nn.Module):
     def __init__(self, n_features, nhead, nhid1, nhid2, nlayers, n_output, n_pred=1, n_patho=0, dropout=0.5, mode="Cox", encoder_type="MLP"):
-        super(TiRank, self).__init__()
+        super(TiRankModel, self).__init__()
 
         # Initialize the learnable weight matrix
         self.feature_weights = nn.Parameter(torch.Tensor(n_features, 1),requires_grad=True)
         nn.init.xavier_uniform_(self.feature_weights)
 
         ## Encoder
         self.encoder_type = encoder_type
@@ -314,15 +313,15 @@
             self.predictor = RiskscorePredictor(
                 n_output, nhid2, n_pred, dropout)
 
         elif mode == "Regression":
             self.predictor = RegscorePredictor(
                 n_output, nhid2, n_pred, dropout)
 
-        elif mode == "Bionomial":
+        elif mode == "Classification":
             self.predictor = ClassscorePredictor(
                 n_output, nhid2, n_pred, dropout)
                 
         else:
             raise ValueError(f"Unsupported Mode: {mode}")
 
         self.pathologpredictor = PathologyPredictor(
```

### Comparing `TiRank-0.1/TiRank/SCSTpreprocess.py` & `tirank-0.1.4/TiRank/SCSTpreprocess.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,19 +161,19 @@
         sc.tl.pca(ann_data)
         # Computing the neighborhood graph
         sc.pp.neighbors(ann_data, use_rep='X_pca')
         # UMAP and leiden
         sc.tl.umap(ann_data)
         sc.tl.leiden(ann_data, key_added="leiden_clusters")
 
-    if infer_mode == "Cell":
+    if infer_mode == "SC":
         sc.pl.umap(ann_data, color=['leiden_clusters'],show = False)
         plt.savefig(os.path.join(savePath_2,"leiden cluster.png"))
 
-    if infer_mode == "Spot":
+    if infer_mode == "ST":
         fig, axs = plt.subplots(1, 2, figsize=(8, 4))  # Create a 1x2 grid for the plots
         sc.pl.spatial(ann_data, img_key="hires", color=["leiden_clusters"],show = False,ax=axs[0])
         sc.pl.umap(ann_data, color=["leiden_clusters"],show = False, ax=axs[1])
         plt.tight_layout()  # Ensure proper spacing between the two plots
         plt.savefig(os.path.join(savePath_2,"leiden cluster.png"))
         plt.close()
```

### Comparing `TiRank-0.1/TiRank/TrainPre.py` & `tirank-0.1.4/TiRank/TrainPre.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,22 +9,22 @@
 import pickle
 import pandas as pd
 import numpy as np
 import scipy.stats as stats
 from sklearn.mixture import GaussianMixture
 
 from .Loss import *
-from .Model import *
+from .Model import TiRankModel
 from .Visualization import plot_loss
 from .Dataloader import transform_test_exp
 
 # Training
 
 
-def Train_one_epoch(model, dataloader_A, dataloader_B, mode='Cox', infer_mode="Cell", adj_A=None, adj_B=None, pre_patho_labels=None, optimizer=None, alphas=[1, 1, 1, 1], device="cpu"):
+def Train_one_epoch(model, dataloader_A, dataloader_B, mode='Cox', infer_mode="SC", adj_A=None, adj_B=None, pre_patho_labels=None, optimizer=None, alphas=[1, 1, 1, 1], device="cpu"):
 
     model.train()
 
     # Initialize variables for loss components
     total_loss_all = 0.0
     regularization_loss_all = 0.0
     bulk_loss_all = 0.0
@@ -35,15 +35,15 @@
     ## DataLoader Bulk
     if mode == 'Cox':
         (X_a, t, e) = next(iter(dataloader_A))
         X_a = X_a.to(device)
         t = t.to(device)
         e = e.to(device)
 
-    if mode in ['Bionomial', 'Regression']:
+    if mode in ['Classification', 'Regression']:
         (X_a, label) = next(iter(dataloader_A))
         X_a = X_a.to(device)
         label = label.to(device)
 
     for batch_B in dataloader_B:
         ## DataLoader SC or ST
         (X_b, idx) = batch_B
@@ -74,42 +74,42 @@
 
         regularization_loss_ = regularization_loss(model.feature_weights)
 
         # Calculate loss
         if mode == 'Cox':
             bulk_loss_ = cox_loss(risk_scores_a, t, e)
 
-        elif mode == 'Bionomial':
+        elif mode == 'Classification':
             bulk_loss_ = CrossEntropy_loss(risk_scores_a, label)
 
         elif mode == 'Regression':
             bulk_loss_ = MSE_loss(risk_scores_a, label)
 
-        if infer_mode == 'Cell':
+        if infer_mode == 'SC':
             cosine_loss_exp_ = cosine_loss(embeddings_b, A)
 
             # total loss
             total_loss = regularization_loss_ * alphas[0] + \
                 bulk_loss_ * alphas[1] + \
                 cosine_loss_exp_ * alphas[2]
             
             pathoLloss = torch.tensor(0)
 
-        elif infer_mode == 'Spot' and adj_B is not None:
+        elif infer_mode == 'ST' and adj_B is not None:
             cosine_loss_exp_ = cosine_loss(embeddings_b, A)
             cosine_loss_spatial_ = cosine_loss(embeddings_b, B)
 
 
             # total loss
             total_loss = regularization_loss_ * alphas[0] + \
                 bulk_loss_ * alphas[1] + \
                 cosine_loss_exp_ * alphas[2] + \
                 cosine_loss_spatial_ * alphas[3]
 
-        elif infer_mode == 'Spot' and pre_patho is not None:
+        elif infer_mode == 'ST' and pre_patho is not None:
             cosine_loss_exp_ = cosine_loss(embeddings_b, A)
             pathoLloss = CrossEntropy_loss(pred_patho, pre_patho)
 
             # total loss
 
             total_loss = regularization_loss_ * alphas[0] + \
                 bulk_loss_ * alphas[1] + \
@@ -126,41 +126,40 @@
         total_loss_all += total_loss.item()
         regularization_loss_all += regularization_loss_.item()
         bulk_loss_all += bulk_loss_.item()
         cosine_loss_all += cosine_loss_exp_.item()
         patho_loss_all += pathoLloss.item()
 
     loss_dict["all_loss_"] = total_loss_all / len(dataloader_B)
-    loss_dict["regularization_loss_"] = regularization_loss_all / \
-        len(dataloader_B)
+    loss_dict["regularization_loss_"] = regularization_loss_all / len(dataloader_B)
     loss_dict["bulk_loss_"] = bulk_loss_all / len(dataloader_B)
     loss_dict["cosine_loss_"] = cosine_loss_all / len(dataloader_B)
     loss_dict["patho_loss_all"] = patho_loss_all / len(dataloader_B)
 
     return loss_dict
 
 # Validate
 
 
-def Validate_model(model, dataloader_A, dataloader_B, mode='Cox', infer_mode="Cell", adj_A=None, adj_B=None, pre_patho_labels=None, alphas=[1, 1, 1, 1], device="cpu"):
+def Validate_model(model, dataloader_A, dataloader_B, mode='Cox', infer_mode="SC", adj_A=None, adj_B=None, pre_patho_labels=None, alphas=[1, 1, 1, 1], device="cpu"):
 
     model.eval()  # Set the model to evaluation mode
 
     validation_loss = 0.0
     with torch.no_grad():  # No need to track the gradients
         # RNA-seq data whole batch validation
         iter_A = iter(dataloader_A)
 
         if mode == 'Cox':
             (X_a, t, e) = next(iter_A)
             X_a = X_a.to(device)
             t = t.to(device)
             e = e.to(device)
 
-        if mode in ['Bionomial', 'Regression']:
+        if mode in ['Classification', 'Regression']:
             (X_a, label) = next(iter_A)
             X_a = X_a.to(device)
             label = label.to(device)
 
         for batch_B in dataloader_B:
             # Similar setup as in the training function
             (X_b, idx) = batch_B
@@ -188,37 +187,37 @@
             # The computation here assumes that the loss functions and infer_mode conditions are the same as in training
             # Please adapt if your validation conditions differ from the training
 
             # Calculate loss
             if mode == 'Cox':
                 bulk_loss_ = cox_loss(risk_scores_a, t, e)
 
-            elif mode == 'Bionomial':
+            elif mode == 'Classification':
                 bulk_loss_ = CrossEntropy_loss(risk_scores_a, label)
 
             elif mode == 'Regression':
                 bulk_loss_ = MSE_loss(risk_scores_a, label)
 
-            if infer_mode == 'Cell':
+            if infer_mode == 'SC':
                 cosine_loss_exp_ = cosine_loss(embeddings_b, A)
 
                 # total loss
                 total_loss = bulk_loss_ * alphas[0] + cosine_loss_exp_ * alphas[1]
 
-            elif infer_mode == 'Spot' and adj_B is not None:
+            elif infer_mode == 'ST' and adj_B is not None:
                 cosine_loss_exp_ = cosine_loss(embeddings_b, A)
                 cosine_loss_spatial_ = cosine_loss(embeddings_b, B)
 
                 # total loss
 
                 total_loss = bulk_loss_ * alphas[0] + \
                     cosine_loss_exp_ * alphas[1] + \
                     cosine_loss_spatial_ * alphas[2]
 
-            elif infer_mode == 'Spot' and pre_patho is not None:
+            elif infer_mode == 'ST' and pre_patho is not None:
                 cosine_loss_exp_ = cosine_loss(embeddings_b, A)
                 pathoLloss = CrossEntropy_loss(pred_patho, pre_patho)
 
                 # total loss
 
                 total_loss = bulk_loss_ * alphas[0] + \
                     cosine_loss_exp_ * alphas[1] + \
@@ -444,20 +443,20 @@
     return mask
 
 # Hyper-paremeters tuning
 
 
 def objective(trial,
               n_features, nhead, nhid1,
-              nhid2, n_output, nlayers, n_pred, dropout, mode, encoder_type,
+              nhid2, n_output, nlayers, n_pred, dropout, n_patho, mode, encoder_type,
               train_loader_Bulk, val_loader_Bulk, train_loader_SC, adj_A, adj_B, pre_patho_labels, device, infer_mode, model_save_path):
 
     print(f"Initiate model in trail {trial.number} with mode: {mode}, infer mode: {infer_mode} encoder type: {encoder_type} on device: {device}.")
-    model = TiRank(n_features=n_features, nhead=nhead, nhid1=nhid1, nhid2=nhid2, n_output=n_output,
-                   nlayers=nlayers, n_pred=n_pred, dropout=dropout, mode=mode, encoder_type=encoder_type)
+    model = TiRankModel(n_features=n_features, nhead=nhead, nhid1=nhid1, nhid2=nhid2, n_output=n_output,
+                   nlayers=nlayers, n_pred=n_pred, dropout=dropout, n_patho = n_patho, mode=mode, encoder_type=encoder_type)
     model = model.to(device)
 
     # Define hyperparameters with trial object
     lr_choices = [1e-2, 6e-3, 3e-3, 1e-3, 6e-4, 3e-4, 1e-4,1e-5,1e-6]
     lr = trial.suggest_categorical("lr", lr_choices)
 
     n_epochs_choices = [300, 350, 400, 450, 500]
@@ -547,15 +546,15 @@
     f = open(os.path.join(savePath_data2train, 'adj_A.pkl'), 'rb')
     adj_A = pickle.load(f)
     f.close()
     f = open(os.path.join(savePath_data2train, 'adj_B.pkl'), 'rb')
     adj_B = pickle.load(f)
     f.close()
     f = open(os.path.join(savePath_data2train, 'patholabels.pkl'), 'rb')
-    patholabels = pickle.load(f)
+    pre_patho_labels = pickle.load(f)
     f.close()
 
     # Initial model parameters
     f = open(os.path.join(savePath_3, 'model_para.pkl'), 'rb')
     model_para = pickle.load(f)
     f.close()
 
@@ -563,30 +562,30 @@
     n_features = model_para.get('n_features', None)
     nhead = model_para.get('nhead', 8)
     nhid1 = model_para.get('nhid1', 256)
     nhid2 = model_para.get('nhid2', 128)
     n_output = model_para.get('n_output', 10)
     nlayers = model_para.get('nlayers', 2)
     n_pred = model_para.get('n_pred', 1)
-    n_patho = model_para.get('n_patho', 0)
     dropout = model_para.get('dropout', 0.5)
+    n_patho = model_para.get('n_patho', 0)
     mode = model_para.get('mode', 'Cox')
     infer_mode = model_para.get('infer_mode', 'Cell')
     encoder_type = model_para.get('encoder_type', 'MLP')
     model_save_path = model_para.get('model_save_path', './checkpoints/')
 
     if not os.path.exists(model_save_path):
         os.mkdir(model_save_path)
 
     study = optuna.create_study(direction='minimize')
     study.optimize(lambda trial: objective(trial,
                                            n_features, nhead, nhid1,
-                                           nhid2, n_output, nlayers, n_pred, dropout, mode, encoder_type,
+                                           nhid2, n_output, nlayers, n_pred, dropout, n_patho, mode, encoder_type,
                                            train_loader_Bulk, val_loader_Bulk, train_loader_SC, 
-                                           adj_A ,adj_B, patholabels, device, infer_mode, model_save_path), n_trials=n_trials)
+                                           adj_A ,adj_B, pre_patho_labels, device, infer_mode, model_save_path), n_trials=n_trials)
     
     # save the best hyperparameters
     best_params = study.best_trial.params
     with open(os.path.join(savePath_3, 'best_params.pkl'), 'wb') as f:
         print("Best hyperparameters:", best_params)
         pickle.dump(best_params, f) ## bet parameters set
     f.close()
@@ -620,23 +619,23 @@
     n_features = model_para.get('n_features', None)
     nhead = model_para.get('nhead', 8)
     nhid1 = model_para.get('nhid1', 256)
     nhid2 = model_para.get('nhid2', 128)
     n_output = model_para.get('n_output', 10)
     nlayers = model_para.get('nlayers', 2)
     n_pred = model_para.get('n_pred', 1)
-    n_patho = model_para.get('n_patho', 0)
     dropout = model_para.get('dropout', 0.5)
+    n_patho = model_para.get('n_patho', 0)
     mode = model_para.get('mode', 'Cox')
     encoder_type = model_para.get('encoder_type', 'MLP')
     model_save_path = model_para.get('model_save_path', './checkpoints/')
 
 
-    model = TiRank(n_features=n_features, nhead=nhead, nhid1=nhid1,
-                nhid2=nhid2, n_output=n_output, nlayers=nlayers, n_pred=n_pred, n_patho=n_patho,dropout=dropout, mode=mode, encoder_type=encoder_type)
+    model = TiRankModel(n_features=n_features, nhead=nhead, nhid1=nhid1,
+                nhid2=nhid2, n_output=n_output, nlayers=nlayers, n_pred=n_pred, dropout=dropout, n_patho=n_patho, mode=mode, encoder_type=encoder_type)
     model.load_state_dict(torch.load(filename))
     model = model.to("cpu")
 
     return model
 
 # Predict
 
@@ -657,15 +656,15 @@
     f.close()
 
     ### All bulk
     f = open(os.path.join(savePath_1, 'bulk_exp.pkl'), 'rb')
     bulkExp = pickle.load(f)
     f.close()
 
-    f = open(os.path.join(savePath_2, 'bulk_clinical.pkl'), 'rb')
+    f = open(os.path.join(savePath_1, 'bulk_clinical.pkl'), 'rb')
     bulkClinical = pickle.load(f)
     f.close()
 
     bulk_rownames=bulkClinical.index.tolist()
 
     ### Transfer all bulk into gene pairs
     bulk_GPmat = transform_test_exp(train_exp = train_bulk_gene_pairs_mat,test_exp = bulkExp)
@@ -693,36 +692,36 @@
     Exp_Tensor_bulk = torch.tensor(Exp_Tensor_bulk, dtype=torch.float32)
     embeddings_bulk, pred_bulk, _ = model(Exp_Tensor_bulk)
 
     if mode == "Cox":
         pred_bulk = pred_bulk.detach().numpy().reshape(-1, 1)
         pred_sc = pred_sc.detach().numpy().reshape(-1, 1)
 
-    elif mode == "Bionomial":
+    elif mode == "Classification":
         pred_sc = pred_sc[:, 1].detach().numpy().reshape(-1, 1)
         pred_bulk = pred_bulk[:, 1].detach().numpy().reshape(-1, 1)
 
     elif mode == "Regression":
         pred_sc = pred_sc.detach().numpy().reshape(-1, 1)
         pred_bulk = pred_bulk.detach().numpy().reshape(-1, 1)
 
     embeddings_sc = embeddings_sc.detach().numpy()
     embeddings_bulk = embeddings_bulk.detach().numpy()
 
     if do_reject:
         if reject_mode == "GMM":
-            if mode in ["Cox", "Bionomial"]:
+            if mode in ["Cox", "Classification"]:
                 reject_mask = Reject_With_GMM_Bio(pred_bulk, pred_sc,
                                                   tolerance=tolerance, min_components=3, max_components=15)
             if mode == "Regression":
                 reject_mask = Reject_With_GMM_Reg(
                     pred_bulk, pred_sc, tolerance=tolerance)
 
         elif reject_mode == "Strict":
-            if mode in ["Cox", "Bionomial"]:
+            if mode in ["Cox", "Classification"]:
                 reject_mask = Reject_With_StrictNumber(
                     pred_bulk, pred_sc, tolerance=tolerance)
 
             if mode == "Regression":
                 print("Test")
         else:
             raise ValueError(f"Unsupported Rejcetion Mode: {reject_mode}")
@@ -761,19 +760,19 @@
         raise ValueError(
             "The prediction matrix was not match with original scAnndata.")
 
     scAnndata.obsm["Rank_Embedding"] = saveDF_sc.iloc[:, 2:]
     scAnndata.obs["Reject"] = saveDF_sc.iloc[:, 0]
     scAnndata.obs["Rank_Score"] = saveDF_sc.iloc[:, 1]
 
-    if mode in ["Cox", "Bionomial"]:
+    if mode in ["Cox", "Classification"]:
         temp = scAnndata.obs["Rank_Score"] * (1 - scAnndata.obs["Reject"])
         scAnndata.obs["Rank_Label"] = [
             "Background" if i == 0 else
-            "Rank-" if 0 < i < 0.5 else
+            "Rank-" if 0 <= i < 0.5 else
             "Rank+"
             for i in temp
         ]
 
         print(f"We set Rank score < 0.5 as Rank- () while > 0.5 as Rank+ ")
 
     if mode == "Regression":
```

### Comparing `TiRank-0.1/TiRank/Visualization.py` & `tirank-0.1.4/TiRank/tirankWeb/visualization.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,319 +5,475 @@
 
 import seaborn as sns
 import scanpy as sc
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import gseapy as gp
+from scipy.cluster.hierarchy import linkage, dendrogram
 
 from scipy.stats import mannwhitneyu
 from sklearn.metrics import confusion_matrix
-from .Dataloader import transform_test_exp
+from .dataloader import transform_test_exp
 
-# Data Preparation
 
 def create_tensor(data_matrix):
     tensor = torch.from_numpy(np.array(data_matrix))
     return torch.tensor(tensor, dtype=torch.float32)
 
+
 # Plot loss function
-def plot_loss(train_loss_dict, alphas, savePath="./loss_on_epoch.png"):
+def plot_loss(train_loss_dict, alphas, savePath="./img/loss_on_epoch.png"):
     """
     Plots the change in different types of loss values across epochs.
 
     Args:
-    train_loss_dict (dict): Dictionary containing the loss values for each epoch. 
-                            The keys should be 'Epoch_x' and the values should be 
+    train_loss_dict (dict): Dictionary containing the loss values for each epoch.
+                            The keys should be 'Epoch_x' and the values should be
                             dictionaries of different loss types.
     """
     # Check if the dictionary is empty
     if not train_loss_dict:
         print("The loss dictionary is empty.")
         return
 
     # Determine the loss types from the first epoch
     loss_types = list(train_loss_dict[next(iter(train_loss_dict))].keys())
-    
+
     # Extracting the number of epochs
     epochs = range(1, len(train_loss_dict) + 1)
-    
+
     # Reformatting the data for plotting
-    loss_data = {loss_type: [epoch_data[loss_type] for epoch_data in train_loss_dict.values()] for loss_type in loss_types}
-    
+    loss_data = {loss_type: [epoch_data[loss_type] for epoch_data in train_loss_dict.values()] for loss_type in
+                 loss_types}
+
     # Plotting
     plt.figure(figsize=(10, 6))
 
     for loss_type, losses in loss_data.items():
         plt.plot(epochs, losses, label=loss_type)
 
     plt.title('Loss Value Change Per Epoch')
     plt.xlabel('Epoch')
     plt.ylabel('Loss Value')
     plt.legend()
     plt.grid(True)
-    plt.savefig(savePath, bbox_inches='tight', pad_inches=1) 
+    plt.savefig(savePath, bbox_inches='tight', pad_inches=1)
     plt.show()
     plt.clf()
     plt.close()
 
     return None
 
 
-# Model Prediction
-
-def model_predict(model, data_tensor, mode):
-    _, prob_scores, _ = model(data_tensor)
-
-    if mode == "Cox":
-        pred_prob = prob_scores.detach().numpy().reshape(-1, 1)
-
-    elif mode == "Bionomial":
-        pred_label = torch.max(prob_scores, dim=1).indices.detach().numpy().reshape(-1, 1)
-        pred_prob = prob_scores[:, 1].detach().numpy().reshape(-1, 1)
-
-    elif mode == "Regression":
-        pred_prob = prob_scores.detach().numpy().reshape(-1, 1)
-        pred_label = pred_prob
-
-
-    return pred_label, pred_prob
-
-# Probability Score Distribution Visualization
-def plot_score_distribution(savePath):
-    savePath_3 = os.path.join(savePath,"3_Analysis")
-
-    ## Load data
-    f = open(os.path.join(savePath_3, 'saveDF_bulk.pkl'), 'rb')
+def plot_score_distribution_(save_path):
+    # Load data
+    f = open(os.path.join(save_path, 'saveDF_bulk.pkl'), 'rb')
     bulk_PredDF = pickle.load(f)
     f.close()
 
-    f = open(os.path.join(savePath_3, 'saveDF_sc.pkl'), 'rb')
+    f = open(os.path.join(save_path, 'saveDF_sc.pkl'), 'rb')
     sc_PredDF = pickle.load(f)
     f.close()
 
     pred_prob_sc = sc_PredDF["Pred_score"]  # scRNA
     pred_prob_bulk = bulk_PredDF["Pred_score"]  # Bulk RNA
 
-    ## Plot
+    # Plot
     sns.distplot(pred_prob_bulk, hist=False, kde=True, kde_kws={'shade': True, 'linewidth': 3}, label='Bulk')
     sns.distplot(pred_prob_sc, hist=False, kde=True, kde_kws={'shade': True, 'linewidth': 3}, label='Single Cell')
 
     plt.title('Density Plot')
     plt.xlabel('Values')
     plt.ylabel('Density')
     plt.legend(title='Sample Type', loc='upper left')
-    plt.savefig(os.path.join(savePath_3, 'TiRank Pred Score Distribution.png'), bbox_inches='tight', pad_inches=1)
-    plt.show()
+    plt.savefig(os.path.join('./img/', 'TiRank Pred Score Distribution.png'), bbox_inches='tight', pad_inches=1)
+    plt.savefig(os.path.join('./assets/', 'TiRank Pred Score Distribution.png'), bbox_inches='tight', pad_inches=1)
     plt.close()
 
     return None
 
-# DEG analysis
-def DEG_analysis(savePath, fc_threshold = 2, Pvalue_threshold = 0.05, do_p_adjust = True):
-    savePath_3 = os.path.join(savePath,"3_Analysis")
 
-    ## Load final single-cell data
-    adata = sc.read_h5ad(os.path.join(savePath_3,"final_anndata.h5ad"))
+def deg_analysis_(save_path, fc_threshold=2, Pvalue_threshold=0.05, do_p_adjust=True):
+    # Load final single-cell data
+    adata = sc.read_h5ad(os.path.join(save_path, "final_anndata.h5ad"))
 
-    ## DEG
+    # DEG
     sc.tl.rank_genes_groups(adata, 'Rank_Label', groups=['Rank+'], reference='Rank-', method='wilcoxon')
 
-    ## Extract dataframe
+    # Extract dataframe
     df_DEG = pd.concat([
         pd.DataFrame(adata.uns['rank_genes_groups']['names']),
         pd.DataFrame(adata.uns['rank_genes_groups']['scores']),
         pd.DataFrame(adata.uns['rank_genes_groups']['pvals']),
         pd.DataFrame(adata.uns['rank_genes_groups']['pvals_adj']),
-        pd.DataFrame(adata.uns['rank_genes_groups']['logfoldchanges'])], 
+        pd.DataFrame(adata.uns['rank_genes_groups']['logfoldchanges'])],
         axis=1)
-    
+
     df_DEG.columns = ['GeneSymbol', 'Scores', 'Pvalue', 'Pvalue_adj', 'LogFoldChange']
     df_DEG.index = df_DEG["GeneSymbol"]
-    
-    df_DEG.to_csv(os.path.join(savePath_3,"All DEGs dataframe.csv"))
+
+    df_DEG.to_csv(os.path.join(save_path, "All DEGs dataframe.csv"))
 
     df_DEG = df_DEG[np.abs(df_DEG['LogFoldChange']) >= math.log2(fc_threshold)]
-    
+
     if do_p_adjust:
         df_DEG = df_DEG[np.abs(df_DEG['Pvalue_adj']) <= Pvalue_threshold]
     else:
         df_DEG = df_DEG[np.abs(df_DEG['Pvalue']) <= Pvalue_threshold]
-    
+
     df_DEG = df_DEG.sort_values(by='LogFoldChange', ascending=False)
-    df_DEG.to_csv(os.path.join(savePath_3,"Differentially expressed genes data frame.csv"))
+    df_DEG.to_csv(os.path.join(save_path, "Differentially expressed genes data frame.csv"))
 
     return None
 
-# volcano plot display the differential expressed genes
-def DEG_volcano(savePath, fc_threshold=2, Pvalue_threshold=0.05, do_p_adjust=True, top_n = 5):
-    # Path for saving analysis results
-    savePath_3 = os.path.join(savePath, "3_Analysis")
 
+# volcano plot display the differential expressed genes
+def deg_volcano_(save_path, fc_threshold=2, Pvalue_threshold=0.05, do_p_adjust=True, top_n=5):
     # Load data from the specified file
-    result = pd.read_csv(os.path.join(savePath_3, "All DEGs dataframe.csv"), index_col=1)
+    result = pd.read_csv(os.path.join(save_path, "All DEGs dataframe.csv"), index_col=1)
     result['group'] = 'black'  # Default color for all points
 
     log2FC = math.log2(fc_threshold)
     result['-lg10Qvalue'] = -(np.log10(result['Pvalue_adj']))
     result['-lg10Pvalue'] = -(np.log10(result['Pvalue']))
 
     # Coloring points based on thresholds and adjusted P-values
     if do_p_adjust:
         # Marking significant upregulated genes in red
-        result.loc[(result['LogFoldChange'] >= log2FC) & (result["Pvalue_adj"] <= Pvalue_threshold), 'group'] = 'tab:red'
+        result.loc[
+            (result['LogFoldChange'] >= log2FC) & (result["Pvalue_adj"] <= Pvalue_threshold), 'group'] = 'tab:red'
         # Marking significant downregulated genes in blue
-        result.loc[(result['LogFoldChange'] <= (-log2FC)) & (result["Pvalue_adj"] <= Pvalue_threshold), 'group'] = 'tab:blue'
+        result.loc[
+            (result['LogFoldChange'] <= (-log2FC)) & (result["Pvalue_adj"] <= Pvalue_threshold), 'group'] = 'tab:blue'
         # Marking non-significant genes in grey
         result.loc[result["Pvalue_adj"] > Pvalue_threshold, 'group'] = 'dimgrey'
     else:
         result.loc[(result['LogFoldChange'] >= log2FC) & (result["Pvalue"] <= Pvalue_threshold), 'group'] = 'tab:red'
-        result.loc[(result['LogFoldChange'] <= (-log2FC)) & (result["Pvalue"] <= Pvalue_threshold), 'group'] = 'tab:blue'
+        result.loc[
+            (result['LogFoldChange'] <= (-log2FC)) & (result["Pvalue"] <= Pvalue_threshold), 'group'] = 'tab:blue'
         result.loc[result["Pvalue"] > Pvalue_threshold, 'group'] = 'dimgrey'
 
     # Define axis display range
     xmin, xmax, ymin, ymax = -8, 8, -10, 100
 
     # Create scatter plot
-    fig = plt.figure(figsize=plt.figaspect(7/6))  # Set figure aspect ratio (height/width)
+    fig = plt.figure(figsize=plt.figaspect(7 / 6))  # Set figure aspect ratio (height/width)
     ax = fig.add_subplot()
     ax.set(xlim=(xmin, xmax), ylim=(ymin, ymax), title='')
     ax.scatter(result['LogFoldChange'], result['-lg10Qvalue'], s=2, c=result['group'])
-    
+
     # Annotate points
     # top N up-regulated genes
-    top_up = result[(result['LogFoldChange'] >= log2FC) & (result['Pvalue_adj'] <= Pvalue_threshold)].nlargest(top_n, 'LogFoldChange')
+    top_up = result[(result['LogFoldChange'] >= log2FC) & (result['Pvalue_adj'] <= Pvalue_threshold)].nlargest(top_n,
+                                                                                                               'LogFoldChange')
     for index, row in top_up.iterrows():
-        ax.annotate(row.name, (row['LogFoldChange'], row['-lg10Qvalue']), textcoords="offset points", xytext=(0,10), ha='center')
+        ax.annotate(row.name, (row['LogFoldChange'], row['-lg10Qvalue']), textcoords="offset points", xytext=(0, 10),
+                    ha='center')
 
     # top N down-regulated genes
-    top_down = result[(result['LogFoldChange'] <= -log2FC) & (result['Pvalue_adj'] <= Pvalue_threshold)].nsmallest(top_n, 'LogFoldChange')
+    top_down = result[(result['LogFoldChange'] <= -log2FC) & (result['Pvalue_adj'] <= Pvalue_threshold)].nsmallest(
+        top_n, 'LogFoldChange')
     for index, row in top_down.iterrows():
-        ax.annotate(row.name, (row['LogFoldChange'], row['-lg10Qvalue']), textcoords="offset points", xytext=(0,10), ha='center')
+        ax.annotate(row.name, (row['LogFoldChange'], row['-lg10Qvalue']), textcoords="offset points", xytext=(0, 10),
+                    ha='center')
 
-    
     ax.set_ylabel('-Log10(Q value)', fontweight='bold')
     ax.set_xlabel('Log2 (fold change)', fontweight='bold')
     ax.spines['right'].set_visible(False)  # Remove right border
-    ax.spines['top'].set_visible(False)    # Remove top border
+    ax.spines['top'].set_visible(False)  # Remove top border
     # Draw horizontal and vertical lines
-    ax.vlines(-log2FC, ymin, ymax, color='dimgrey', linestyle='dashed', linewidth=1) # Vertical line for negative log2FC
-    ax.vlines(log2FC, ymin, ymax, color='dimgrey', linestyle='dashed', linewidth=1) # Vertical line for positive log2FC
-    ax.hlines(-math.log10(Pvalue_threshold), xmin, xmax, color='dimgrey', linestyle='dashed', linewidth=1) # Horizontal line for Pvalue threshold
+    ax.vlines(-log2FC, ymin, ymax, color='dimgrey', linestyle='dashed',
+              linewidth=1)  # Vertical line for negative log2FC
+    ax.vlines(log2FC, ymin, ymax, color='dimgrey', linestyle='dashed', linewidth=1)  # Vertical line for positive log2FC
+    ax.hlines(-math.log10(Pvalue_threshold), xmin, xmax, color='dimgrey', linestyle='dashed',
+              linewidth=1)  # Horizontal line for Pvalue threshold
 
     # Set x and y axis ticks
     ax.set_xticks(range(-8, 8, 2))  # x-axis ticks with start point and step
     ax.set_yticks(range(-10, 100, 20))  # y-axis ticks with start point and step
 
     # Save the figure
-    fig.savefig(os.path.join(savePath_3, 'DEG_volcano_plot.png'), dpi=300)
-    plt.show()
+    fig.savefig(os.path.join('./img/', 'DEG_volcano_plot.png'), dpi=300)
+    fig.savefig(os.path.join('./assets/', 'DEG_volcano_plot.png'), dpi=300)
 
     return None
 
+
 # Pathway enrichment analysis
-def Pathway_Enrichment(savePath,database = "KEGG_2016"):
-    savePath_3 = os.path.join(savePath, "3_Analysis")
-    result = pd.read_csv(os.path.join(savePath_3, "Differentially expressed genes data frame.csv"), index_col=1)
+def pathway_enrichment(save_path, database="KEGG_2016"):
+    result = pd.read_csv(os.path.join(save_path, "Differentially expressed genes data frame.csv"), index_col=1)
 
     # up and down genes
-    upgenes = result[result["LogFoldChange"]>0]['GeneSymbol'].tolist()
-    downgenes = result[result["LogFoldChange"]<0]['GeneSymbol'].tolist()
-    
+    upgenes = result[result["LogFoldChange"] > 0]['GeneSymbol'].tolist()
+    downgenes = result[result["LogFoldChange"] < 0]['GeneSymbol'].tolist()
+
     upenr = gp.enrichr(
         gene_list=upgenes,
-                 gene_sets=database,
-                 organism='Human', # don't forget to set organism to the one you desired! e.g. Yeast
-                 outdir=os.path.join(savePath_3,'enrichr','up'),
-                 no_plot=True,
-                 cutoff=0.5 # test dataset, use lower value from range(0,1)
-                )
+        gene_sets=database,
+        organism='Human',  # don't forget to set organism to the one you desired! e.g. Yeast
+        outdir=os.path.join(save_path, 'enrichr', 'up'),
+        no_plot=True,
+        cutoff=0.5  # test dataset, use lower value from range(0,1)
+    )
 
     downenr = gp.enrichr(
         gene_list=downgenes,
-                 gene_sets=database,
-                 organism='Human', # don't forget to set organism to the one you desired! e.g. Yeast
-                 outdir=os.path.join(savePath_3,'enrichr','down'),
-                 no_plot=True,
-                 cutoff=0.5 # test dataset, use lower value from range(0,1)
-                )
-    
+        gene_sets=database,
+        organism='Human',  # don't forget to set organism to the one you desired! e.g. Yeast
+        outdir=os.path.join(save_path, 'enrichr', 'down'),
+        no_plot=True,
+        cutoff=0.5  # test dataset, use lower value from range(0,1)
+    )
+
     database_name = '_'.join(database)
 
-    if np.min(downenr.results["Adjusted P-value"]) > 0.05:
-        print("Up regulated genes do not enrich in any pathway of "+database_name+"!")
+    if np.min(upenr.results["Adjusted P-value"]) > 0.05:
+        print("Up regulated genes do not enrich in any pathway of " + database_name + "!")
     else:
-        gp.plot.dotplot(upenr.results, title="Up regulated genes enrich in "+database_name)
-        plt.savefig(os.path.join(savePath_3,'enrichr','up',"Up regulated genes enrich in "+database_name+".png"), bbox_inches='tight', pad_inches=1)
+        gp.plot.dotplot(upenr.results, title="Up regulated genes enrich in " + database_name)
+        plt.savefig(os.path.join('./img/', "Up regulated genes enrich in " + database_name + ".png"),
+                    bbox_inches='tight', pad_inches=1)
+        plt.savefig(
+            os.path.join('./assets/', "Up regulated genes enrich in " + database_name + ".png"),
+            bbox_inches='tight', pad_inches=1)
         plt.close()
 
     if np.min(downenr.results["Adjusted P-value"]) > 0.05:
-        print("Down regulated genes do not enrich in any pathway of "+database_name+"!")
+        print("Down regulated genes do not enrich in any pathway of " + database_name + "!")
     else:
-        gp.plot.dotplot(downenr.results, title="Down regulated genes enrich in "+database_name)
-        plt.savefig(os.path.join(savePath_3,'enrichr','down',"Down regulated genes enrich in "+database_name+".png"), bbox_inches='tight', pad_inches=1)
+        gp.plot.dotplot(downenr.results, title="Down regulated genes enrich in " + database_name)
+        plt.savefig(
+            os.path.join('./img/', "Down regulated genes enrich in " + database_name + ".png"),
+            bbox_inches='tight', pad_inches=1)
+        plt.savefig(
+            os.path.join('./assets/', "Down regulated genes enrich in " + database_name + ".png"),
+            bbox_inches='tight', pad_inches=1)
         plt.close()
 
-    upenr.results.to_csv(os.path.join(savePath_3,'enrichr','up',"Pathway enrichment in "+database_name+" data frame.csv"))
-    downenr.results.to_csv(os.path.join(savePath_3,'enrichr','down',"Pathway enrichment in "+database_name+" data frame.csv"))
+    upenr.results.to_csv(
+        os.path.join(save_path, 'enrichr', 'up', "Pathway enrichment in " + database_name + " data frame.csv"))
+    downenr.results.to_csv(
+        os.path.join(save_path, 'enrichr', 'down', "Pathway enrichment in " + database_name + " data frame.csv"))
 
     return None
 
-# Evaluation on Other Data
-
-def evaluate_on_test_data(model, test_set, data_path, save_path, bulk_gene_pairs_mat):
-    if not (os.path.exists(save_path)):
-        os.makedirs(save_path)
-
-    save_path_ = os.path.join(save_path, "bulk_test")
 
-    if not (os.path.exists(save_path_)):
-        os.makedirs(save_path_)
+def plot_score_umap_(save_path, infer_mode):
+    sc_PredDF = pd.read_csv(
+        os.path.join(save_path, "spot_predict_score.csv"), index_col=0
+    )
+
+    label_color_map = {
+        "Rank+": "#DE6E66",
+        "Rank-": "#5096DE",
+        "Background": "lightgrey",
+    }
+
+    if infer_mode == "Cell":
+        f = open(os.path.join(save_path, "scAnndata.pkl"), "rb")
+        scAnndata = pickle.load(f)
+        f.close()
+
+        scAnndata.obs["TiRank_Score"] = sc_PredDF["Rank_Score"]
+        scAnndata.obs["TiRank_Label"] = sc_PredDF["Rank_Label"]
+
+        sc.pl.umap(scAnndata, color="TiRank_Score", title="", show=False)
+        plt.savefig(
+            os.path.join('./assets/', "UMAP of TiRank Pred Score.png"),
+            bbox_inches="tight",
+            pad_inches=1,
+        )
+        plt.show()
+        plt.close()
 
-    for data_id in test_set:
-        test_bulk_clinical = pd.read_table(os.path.join(data_path, data_id + "_meta.csv"), sep=",", index_col=0)
-        test_bulk_clinical.columns = ["Group", "OS_status", "OS_time"]
-        test_bulk_clinical['Group'] = test_bulk_clinical['Group'].apply(lambda x: 0 if x in ['PR', 'CR', 'CRPR'] else 1)
+        sc.pl.umap(
+            scAnndata,
+            color="TiRank_Label",
+            title="",
+            show=False,
+            palette=label_color_map,
+        )
+        plt.savefig(
+            os.path.join('./assets/', "UMAP of TiRank Label Score.png"),
+            bbox_inches="tight",
+            pad_inches=1,
+        )
+        plt.close()
 
-        test_bulk_exp = pd.read_csv(os.path.join(data_path, data_id + "_exp.csv"), index_col=0)
-        test_bulk_exp_gene_pairs_mat = transform_test_exp(bulk_gene_pairs_mat, test_bulk_exp)
-        test_exp_tensor_bulk = create_tensor(test_bulk_exp_gene_pairs_mat)
+    elif infer_mode == "Spot":
+        f = open(os.path.join(save_path, "scAnndata.pkl"), "rb")
+        scAnndata = pickle.load(f)
+        f.close()
+
+        scAnndata.obs["TiRank_Score"] = sc_PredDF["Rank_Score"]
+        scAnndata.obs["TiRank_Label"] = sc_PredDF["Rank_Label"]
+
+        sc.pl.umap(scAnndata, color="TiRank_Score", title="", show=False)
+        plt.savefig(
+            os.path.join('./assets/', "UMAP of TiRank Pred Score.png"),
+            bbox_inches="tight",
+            pad_inches=1,
+        )
+        plt.close()
 
-        test_pred_label, _ = model_predict(model, test_exp_tensor_bulk, mode = "Bionomial")
-        test_bulk_clinical["TiRank_Label"] = test_pred_label.flatten()
-        test_bulk_clinical.to_csv(os.path.join(save_path_, data_id + "_predict_score.csv"))
+        sc.pl.spatial(
+            scAnndata, color="TiRank_Score", title="", show=False, alpha_img=0.6
+        )
+        plt.savefig(
+            os.path.join('./assets/', "Spatial of TiRank Pred Score.png"),
+            bbox_inches="tight",
+            pad_inches=1,
+        )
+        plt.close()
 
-        true_labels_bulk = test_bulk_clinical['Group']
-        predicted_labels_bulk = test_bulk_clinical["TiRank_Label"]
+        sc.pl.umap(
+            scAnndata,
+            color="TiRank_Label",
+            title="",
+            show=False,
+            palette=label_color_map,
+        )
+        plt.savefig(
+            os.path.join('./assets/', "UMAP of TiRank Label Score.png"),
+            bbox_inches="tight",
+            pad_inches=1,
+        )
+        plt.close()
 
-        cm = confusion_matrix(true_labels_bulk, predicted_labels_bulk)
-        sns.heatmap(cm, annot=True, fmt='d', cmap='Blues')
-        plt.savefig(os.path.join(save_path_, f'Pred on bulk: {data_id}.png'), bbox_inches='tight', pad_inches=1)
+        sc.pl.spatial(
+            scAnndata,
+            color="TiRank_Label",
+            title="",
+            show=False,
+            alpha_img=0.6,
+            palette=label_color_map,
+        )
+        plt.savefig(
+            os.path.join('./assets/', "Spatial of TiRank Label Score.png"),
+            bbox_inches="tight",
+            pad_inches=1,
+        )
         plt.show()
         plt.close()
 
-# Functions for RNA-seq to scRNA with Regression mode
+    else:
+        raise ValueError("Invalid infer_mode selected")
+
+    return None
+
+
+# Probability Score Distribution Visualization on UMAP
+def plot_label_distribution_among_conditions_(save_path, group):
+    sc_PredDF = pd.read_csv(
+        os.path.join(save_path, "spot_predict_score.csv"), index_col=0
+    )
+
+    if group not in sc_PredDF.columns:
+        raise ValueError("Invalid grouping condition selected")
+
+    # Creating a frequency table
+    freq_table = pd.crosstab(index=sc_PredDF[group], columns=sc_PredDF["Rank_Label"])
+    df = freq_table.stack().reset_index(name="Freq")
+    df = df[df[group] != ""]
+
+    # Calculating cluster totals and proportions
+    cluster_totals = df.groupby(group)["Freq"].sum().reset_index(name="TotalFreq")
+    df = pd.merge(df, cluster_totals, on=group, how="left")
+    df["Proportion"] = df["Freq"] / df["TotalFreq"]
+
+    # For now, skipping direct entropy calculation for brevity
+
+    # Order and adjust DataFrame for plotting
+    df[group] = pd.Categorical(df[group], categories=pd.unique(df[group]), ordered=True)
+    df = df.sort_values(by=[group, "Rank_Label"])
+
+    # Plotting
+    sns.set_style("white")
+    plt.figure(figsize=(10, 6))
+    sns.barplot(
+        data=df,
+        x=group,
+        y="Proportion",
+        hue="Rank_Label",
+        palette={"Rank-": "#4cb1c4", "Rank+": "#b5182b", "Background": "grey"},
+    )
+    plt.legend(title="Rank Label")
+    plt.xlabel(f"{group}")
+    plt.ylabel("Proportion")
+    plt.title(f"Proportion of Rank Labels by {group}")
+
+    # Construct the filename using the 'group' variable. This ensures the file name reflects the content of the plot.
+    filename = f"Distribution of TiRank label in {group}.png"
+    # Save the figure, using os.path.join to construct the file path correctly.
+    plt.savefig(
+        os.path.join('./assets/', filename),
+        bbox_inches="tight",
+        pad_inches=1,
+    )
+    plt.show()
+    plt.close()
+
+    return None
 
-def create_boxplot(data, title, ax, group_column='True Label', score_column='Predicted Score'):
-    sns.boxplot(x=group_column, y=score_column, data=data, ax=ax)
-    ax.set_title(title)
-
-    # Statistical test
-    group0 = data[data[group_column] == 0][score_column]
-    group1 = data[data[group_column] == 1][score_column]
-    stat, p_value = mannwhitneyu(group0, group1)
-    ax.text(0.5, 0.95, f'p = {p_value:.2e}', ha='center', va='center', transform=ax.transAxes)
-
-def create_density_plot(data, label, ax, title):
-    sns.kdeplot(data, shade=True, linewidth=3, label=label, ax=ax)
-    ax.set_title(title)
-    ax.legend()
-
-def create_hist_plot(data, ax, title):
-    sns.histplot(data, bins=20, kde=True, ax=ax)
-    ax.set_title(title)
-
-def create_comparison_density_plot(data1, label1, data2, label2, ax, title):
-    sns.kdeplot(data1, shade=True, linewidth=3, label=label1, ax=ax)
-    sns.kdeplot(data2, shade=True, linewidth=3, label=label2, ax=ax)
-    ax.set_title(title)
-    ax.legend()
+
+def plot_genepair(df, data_type, save_path=None):
+    """
+    Plots a heatmap with hierarchical clustering applied to rows and columns.
+
+    Parameters:
+    - df : pandas.DataFrame
+        DataFrame with binary values (e.g., 1 and -1).
+    - method : str, optional
+        The linkage algorithm to use for clustering (e.g., 'average', 'single', 'complete').
+    - metric : str, optional
+        The distance metric to use (e.g., 'euclidean', 'cityblock').
+    - cmap : str, optional
+        The colormap used to plot the heatmap. Default is 'coolwarm'.
+    - figsize : tuple, optional
+        Figure size as (width, height) in inches. Default is (10, 8).
+
+    Returns:
+    - None
+    """
+
+    ## difine the figure
+    figsize = (15, 12)
+    cmap = "coolwarm"
+
+    ## define cluster
+    method = "average"
+    metric = "euclidean"
+
+    nrow, ncol = df.shape
+
+    if nrow > ncol:
+        n_size = ncol
+        sampled_df = df.sample(n=n_size, random_state=42)
+    else:
+        sampled_df = df
+
+    # Generate the linkage matrices
+    row_clusters = linkage(sampled_df, method=method, metric=metric)
+    col_clusters = linkage(sampled_df.T, method=method, metric=metric)
+
+    # Create the row and column dendrogram orders
+    row_dendr = dendrogram(row_clusters, no_plot=True)
+    col_dendr = dendrogram(col_clusters, no_plot=True)
+
+    # Reorder the dataframe according to the dendrograms
+    df_clustered = sampled_df.iloc[row_dendr["leaves"], col_dendr["leaves"]]
+
+    # Plotting
+    plt.figure(figsize=figsize)
+    sns.heatmap(
+        df_clustered, cmap=cmap, annot=False
+    )  # Turn off tick labels if not meaningful
+    plt.title("Clustered Heatmap of Gene Pairs")
+    plt.savefig(
+        os.path.join(save_path, data_type + " gene pair heatmap.png"),
+        bbox_inches="tight",
+        pad_inches=0.1
+    )
+    plt.close()
+
+    return None
```

### Comparing `TiRank-0.1/TiRank/__init__.py` & `tirank-0.1.4/TiRank/tirankWeb/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # Import each module within the TiRank package
-from .Dataloader import *
-from .GPextractor import *
-from .Imageprocessing import *
-from .LoadData import *
-from .Loss import *
-from .Model import *
-from .SCSTpreprocess import *
-from .TrainPre import *
-from .Visualization import *
+from .dataloader import *
+from .gpextractor import *
+from .imageprocessing import *
+from .loaddata import *
+from .loss import *
+from .model import *
+from .scstpreprocess import *
+from .trainpre import *
+from .visualization import *
 
 # Define an __all__ list that specifies all the modules you want to be imported when 'from TiRank import *' is used
 __all__ = [
-    'Dataloader', 
-    'GPextractor', 
-    'Imageprocessing', 
-    'LoadData', 
-    'Loss', 
-    'Model', 
-    'SCSTpreprocess', 
-    'TrainPre', 
-    'Visualization'
+    'dataloader', 
+    'gpextractor', 
+    'imageprocessing', 
+    'loaddata', 
+    'loss', 
+    'model', 
+    'scstpreprocess', 
+    'trainpre', 
+    'visualization',
 ]
```

### Comparing `TiRank-0.1/setup.py` & `tirank-0.1.4/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from setuptools import setup, find_packages
 
 setup(
     name='TiRank',  # Replace with your own package name
-    version='0.1',  # Package version
+    version='0.1.4',  # Package version
     author='Lenis Lin',  # Replace with your name
     author_email='727682308@qq.com',  # Replace with your email
     license='MIT License',
     description='A comprehensive analysis tool for transfering phenotype of bulk transcritomic data to single cell or spatial transcriptomic data.',  # Short description
     long_description=open('README.md').read(),  # Long description read from the the readme file
+    long_description_content_type='text/markdown',  # Specify the content type as Markdown
     url='https://github.com/LenisLin/TiRank',  # URL to your package's repository
-    packages=find_packages(),  # List of all Python import packages that should be included in the Distribution Package
+    packages=find_packages(include=['TiRank', 'TiRank.*']),  # List of all Python import packages that should be included in the Distribution Package
+    include_package_data=True,
     install_requires=[
         'torch',
         'torchvision',
         'optuna==3.4.0',
 
         'numpy==1.22.3',
         'scipy==1.8.1',
@@ -29,17 +31,23 @@
         'seaborn==0.12.2',
         'pillow==9.4.0',
 
         'scanpy==1.9.5',
         'gseapy==1.1.1',
 
         'dash==2.14.2',
-        'dash-bootstrap-components==1.5.0'
+        'dash-bootstrap-components==1.5.0',
+        'dash-loading-spinners==1.0.3'
     ],
+    # entry_points={
+    #     'console_scripts': [
+    #         'tirank=TiRank.app:main',  # Entry point for the Dash app
+    #     ],
+    # },
     classifiers=[
         # Classifiers help users find your project by categorizing it.
         # For a list of valid classifiers, see https://pypi.org/classifiers/
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',  # Example license
     ],
-    python_requires='>=3.6',  # Minimum version requirement of the package
+    python_requires='>=3.9',  # Minimum version requirement of the package
 )
```

