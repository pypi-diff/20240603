# Comparing `tmp/gess-0.1.0.tar.gz` & `tmp/gess-0.1.1.tar.gz`

## Comparing `gess-0.1.0.tar` & `gess-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gess-0.1.0/src/GESS/.Rhistory
--rw-r--r--   0        0        0     4619 2020-02-02 00:00:00.000000 gess-0.1.0/src/GESS/GESSPercentIDMatrix.py
--rw-r--r--   0        0        0    31956 2020-02-02 00:00:00.000000 gess-0.1.0/src/GESS/GESS_core.py
--rw-r--r--   0        0        0     4255 2020-02-02 00:00:00.000000 gess-0.1.0/src/GESS/GESSfinder.py
--rw-r--r--   0        0        0    10045 2020-02-02 00:00:00.000000 gess-0.1.0/src/GESS/GESSmatricise.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 gess-0.1.0/src/GESS/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gess-0.1.0/src/GESS/__init__.py
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 gess-0.1.0/src/GESS/Testing/Batch_compare_ages.sh
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 gess-0.1.0/src/GESS/Testing/GESS_mass_unittest.sh
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 gess-0.1.0/src/GESS/Testing/InterpretGESSTesting.py
--rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 gess-0.1.0/src/GESS/Utils/GESSargs.py
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 gess-0.1.0/src/GESS/Utils/GetH5Genes.py
--rw-r--r--   0        0        0     7733 2020-02-02 00:00:00.000000 gess-0.1.0/src/GESS/Utils/HandleH5s.py
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 gess-0.1.0/LICENSE
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 gess-0.1.0/README.md
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 gess-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 gess-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gess-0.1.1/src/GESS/.Rhistory
+-rw-r--r--   0        0        0     4619 2020-02-02 00:00:00.000000 gess-0.1.1/src/GESS/GESSPercentIDMatrix.py
+-rw-r--r--   0        0        0    19791 2020-02-02 00:00:00.000000 gess-0.1.1/src/GESS/GESS_Tutorial.ipynb
+-rw-r--r--   0        0        0    31956 2020-02-02 00:00:00.000000 gess-0.1.1/src/GESS/GESS_core.py
+-rw-r--r--   0        0        0     4255 2020-02-02 00:00:00.000000 gess-0.1.1/src/GESS/GESSfinder.py
+-rw-r--r--   0        0        0     9670 2020-02-02 00:00:00.000000 gess-0.1.1/src/GESS/GESSmatricise.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 gess-0.1.1/src/GESS/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gess-0.1.1/src/GESS/__init__.py
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 gess-0.1.1/src/GESS/Testing/Batch_compare_ages.sh
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 gess-0.1.1/src/GESS/Testing/GESS_mass_unittest.sh
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 gess-0.1.1/src/GESS/Testing/InterpretGESSTesting.py
+-rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 gess-0.1.1/src/GESS/Utils/GESSargs.py
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 gess-0.1.1/src/GESS/Utils/GetH5Genes.py
+-rw-r--r--   0        0        0     7249 2020-02-02 00:00:00.000000 gess-0.1.1/src/GESS/Utils/HandleH5s.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 gess-0.1.1/LICENSE
+-rw-r--r--   0        0        0     5123 2020-02-02 00:00:00.000000 gess-0.1.1/README.md
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 gess-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5853 2020-02-02 00:00:00.000000 gess-0.1.1/PKG-INFO
```

### Comparing `gess-0.1.0/src/GESS/GESSPercentIDMatrix.py` & `gess-0.1.1/src/GESS/GESSPercentIDMatrix.py`

 * *Files identical despite different names*

### Comparing `gess-0.1.0/src/GESS/GESS_core.py` & `gess-0.1.1/src/GESS/GESS_core.py`

 * *Files identical despite different names*

### Comparing `gess-0.1.0/src/GESS/GESSfinder.py` & `gess-0.1.1/src/GESS/GESSfinder.py`

 * *Files identical despite different names*

### Comparing `gess-0.1.0/src/GESS/GESSmatricise.py` & `gess-0.1.1/src/GESS/GESSmatricise.py`

 * *Files 3% similar despite different names*

```diff
@@ -153,23 +153,20 @@
         plt.savefig(args.save)
     else:
         #Displays the generated matrix
         plt.show()
 
 #A function to quickly check that the user settings appear to be valid for matrix generation
 def test_validity(args):
-    #Warns the user about how long H5 processing can take
-    if '.h5' in args.querydata or '.h5' in args.targetdata:
-        print("\n--WARNING--\nProcessing large .h5 files can be very time consuming, especially if you have many genes of interest.\nThis can take up to 1 minute PER COMPARISON \nIf this becomes an issue, consider processing these in smaller chunks.")
-    
+
     #Checks that the user has included "Query" data
     if args.input_query == '' or args.querydata == '':
         print('\n~~~~~ERROR~~~~~\n')
         print('You must supply both query genes (as a line seperated .txt file or as a python list) AND query data(as .csv or .h5ad)')
-        #exit()
+        exit()
 
     #This block of code deals specifically with identifying whether one or two data sets are needed.
     #If no seperate target list is provided, the matrix will be formed all-against-all from query genes
     if args.input_target == '':
         target_in = args.input_query
         target_data = args.querydata
```

### Comparing `gess-0.1.0/src/GESS/Testing/Batch_compare_ages.sh` & `gess-0.1.1/src/GESS/Testing/Batch_compare_ages.sh`

 * *Files identical despite different names*

### Comparing `gess-0.1.0/src/GESS/Testing/GESS_mass_unittest.sh` & `gess-0.1.1/src/GESS/Testing/GESS_mass_unittest.sh`

 * *Files identical despite different names*

### Comparing `gess-0.1.0/src/GESS/Testing/InterpretGESSTesting.py` & `gess-0.1.1/src/GESS/Testing/InterpretGESSTesting.py`

 * *Files identical despite different names*

### Comparing `gess-0.1.0/src/GESS/Utils/GESSargs.py` & `gess-0.1.1/src/GESS/Utils/GESSargs.py`

 * *Files identical despite different names*

### Comparing `gess-0.1.0/src/GESS/Utils/GetH5Genes.py` & `gess-0.1.1/src/GESS/Utils/GetH5Genes.py`

 * *Files identical despite different names*

### Comparing `gess-0.1.0/src/GESS/Utils/HandleH5s.py` & `gess-0.1.1/src/GESS/Utils/HandleH5s.py`

 * *Files 3% similar despite different names*

```diff
@@ -151,25 +151,14 @@
     #We also let the users know which Annotations are inappropriate for GESS and why.
     if len(other_annotations) > 0:
 
         print('Some annotation levels have only one category - GESS cannot utilise these:')
         for level in other_annotations:
             print(f'{level}\t Only Category:   {other_annotations[level]}')
 
-def test():
-    #testfile = '/home/ag_jdowlab/r_fca_biohub_malpighian_tubule_10x.h5ad'
-    #testfile = '/home/ag_jdowlab/r_fca_biohub_all_wo_blood_10x.h5ad'
-    testfile = '/media/ag_jdowlab/Expansion/HandlingLFC/UpdatedH5s/MsIT_Updated.h5ad'
-    testanno = ["annotation", "annotation_broad"]
-    testgenes = 'LOC115452582'
-    analysis_mode = 'prevalence'
-
-    describe_file(testfile)
-    #H5_GESS(testanno, testfile, testgenes, analysis_mode)
-
 #This function is designed to try and handle a more broad range of H5 files
 #We aim to find where expression data and gene names are stored.
 def prep_h5(infile):
 
     adata = sp.read_h5ad(infile)
 
     frame_setting = adata
@@ -183,10 +172,7 @@
 
     adata, frame_setting = prep_h5(h5file)
 
     #Gets a list of all genes within the H5 files
     all_genes = frame_setting.var_names.to_list()
 
     return all_genes
-
-if __name__ == '__main__':
-    test()
```

### Comparing `gess-0.1.0/LICENSE` & `gess-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gess-0.1.0/pyproject.toml` & `gess-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "GESS"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Andrew Gillen", email="andrew.gillen@glasgow.ac.uk" },
 ]
 
 description = "A package designed to allow scoring of gene expression patterns using the Gene Expression Similarity Score system"
 readme = "README.md"
 requires-python = ">=3.10"
```

