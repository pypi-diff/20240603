# Comparing `tmp/comseg-0.1.tar.gz` & `tmp/comseg-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comseg-0.1.tar", last modified: Thu May 30 14:03:26 2024, max compression
+gzip compressed data, was "comseg-0.2.tar", last modified: Mon Jun  3 14:21:49 2024, max compression
```

## Comparing `comseg-0.1.tar` & `comseg-0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-05-30 14:03:26.884800 comseg-0.1/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1056 2023-10-04 17:16:12.000000 comseg-0.1/LICENSE
--rw-r--r--   0 tom       (1000) tom       (1000)     1233 2024-05-30 14:03:26.884800 comseg-0.1/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)      800 2024-05-28 17:16:59.000000 comseg-0.1/README.md
--rw-rw-r--   0 tom       (1000) tom       (1000)      511 2024-05-30 13:59:02.000000 comseg-0.1/pyproject.toml
--rw-rw-r--   0 tom       (1000) tom       (1000)      374 2024-05-28 17:08:31.000000 comseg-0.1/requirements.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)       38 2024-05-30 14:03:26.888800 comseg-0.1/setup.cfg
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-05-30 14:03:26.884800 comseg-0.1/src/
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-05-30 14:03:26.884800 comseg-0.1/src/ComSeg.egg-info/
--rw-r--r--   0 tom       (1000) tom       (1000)     1233 2024-05-30 14:03:26.000000 comseg-0.1/src/ComSeg.egg-info/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)      471 2024-05-30 14:03:26.000000 comseg-0.1/src/ComSeg.egg-info/SOURCES.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)        1 2024-05-30 14:03:26.000000 comseg-0.1/src/ComSeg.egg-info/dependency_links.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)       16 2024-05-30 14:03:26.000000 comseg-0.1/src/ComSeg.egg-info/top_level.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)        9 2024-02-13 12:19:38.000000 comseg-0.1/src/__init__.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-05-30 14:03:26.884800 comseg-0.1/src/comseg/
--rw-rw-r--   0 tom       (1000) tom       (1000)      403 2024-05-30 13:59:37.000000 comseg-0.1/src/comseg/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    18288 2024-05-15 12:06:26.000000 comseg-0.1/src/comseg/clustering.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    20754 2024-05-30 13:50:27.000000 comseg-0.1/src/comseg/dataset.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    23470 2024-05-30 13:54:32.000000 comseg-0.1/src/comseg/dictionary.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    40560 2024-05-30 13:15:59.000000 comseg-0.1/src/comseg/model.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-05-30 14:03:26.884800 comseg-0.1/src/comseg/utils/
--rw-rw-r--   0 tom       (1000) tom       (1000)        0 2023-08-02 11:20:30.000000 comseg-0.1/src/comseg/utils/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    18897 2024-05-27 07:57:03.000000 comseg-0.1/src/comseg/utils/custom_louvain.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1887 2023-10-03 13:00:25.000000 comseg-0.1/src/comseg/utils/plot.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     8640 2023-11-21 18:48:35.000000 comseg-0.1/src/comseg/utils/preprocessing.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     3292 2023-10-25 14:42:29.000000 comseg-0.1/src/comseg/utils/utils_graph.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-06-03 14:21:49.228663 comseg-0.2/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1056 2023-10-04 17:16:12.000000 comseg-0.2/LICENSE
+-rw-r--r--   0 tom       (1000) tom       (1000)     1327 2024-06-03 14:21:49.224662 comseg-0.2/PKG-INFO
+-rw-rw-r--   0 tom       (1000) tom       (1000)      894 2024-05-30 14:08:02.000000 comseg-0.2/README.md
+-rw-rw-r--   0 tom       (1000) tom       (1000)      511 2024-06-03 13:33:36.000000 comseg-0.2/pyproject.toml
+-rw-rw-r--   0 tom       (1000) tom       (1000)      374 2024-05-28 17:08:31.000000 comseg-0.2/requirements.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)       38 2024-06-03 14:21:49.228663 comseg-0.2/setup.cfg
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-06-03 14:21:49.224662 comseg-0.2/src/
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-06-03 14:21:49.224662 comseg-0.2/src/ComSeg.egg-info/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1327 2024-06-03 14:21:49.000000 comseg-0.2/src/ComSeg.egg-info/PKG-INFO
+-rw-rw-r--   0 tom       (1000) tom       (1000)      471 2024-06-03 14:21:49.000000 comseg-0.2/src/ComSeg.egg-info/SOURCES.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)        1 2024-06-03 14:21:49.000000 comseg-0.2/src/ComSeg.egg-info/dependency_links.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)       16 2024-06-03 14:21:49.000000 comseg-0.2/src/ComSeg.egg-info/top_level.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)        9 2024-02-13 12:19:38.000000 comseg-0.2/src/__init__.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-06-03 14:21:49.224662 comseg-0.2/src/comseg/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      403 2024-06-03 13:33:36.000000 comseg-0.2/src/comseg/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    18219 2024-06-03 13:08:08.000000 comseg-0.2/src/comseg/clustering.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    22031 2024-06-03 13:15:30.000000 comseg-0.2/src/comseg/dataset.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    27330 2024-06-03 14:06:25.000000 comseg-0.2/src/comseg/dictionary.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    40560 2024-06-03 12:49:35.000000 comseg-0.2/src/comseg/model.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-06-03 14:21:49.224662 comseg-0.2/src/comseg/utils/
+-rw-rw-r--   0 tom       (1000) tom       (1000)        0 2023-08-02 11:20:30.000000 comseg-0.2/src/comseg/utils/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    18897 2024-05-27 07:57:03.000000 comseg-0.2/src/comseg/utils/custom_louvain.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1887 2023-10-03 13:00:25.000000 comseg-0.2/src/comseg/utils/plot.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     8640 2023-11-21 18:48:35.000000 comseg-0.2/src/comseg/utils/preprocessing.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3292 2023-10-25 14:42:29.000000 comseg-0.2/src/comseg/utils/utils_graph.py
```

### Comparing `comseg-0.1/LICENSE` & `comseg-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `comseg-0.1/PKG-INFO` & `comseg-0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: ComSeg
-Version: 0.1
+Version: 0.2
 Summary: single cell RNA profiling analysis of imaging-based spatial transcriptomics data
 Author-email: Thomas Defard <thomas.defard@mines-paristech.fr>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 <img src="./comseg.png" width="650" height="263">
 
 # News
+- Update with comseg 0.0.8. Compatibility with SOPA : https://gustaveroussy.github.io/sopa/
 
-Update with comseg 0.0.7. Computation of the co-expression matrix is now faster.
+- Update with comseg 0.0.7. Computation of the co-expression matrix is now faster.
 
 # Support
 
 If you have any questions relative to the package or bug, please open an issue in this repository.
 
 
 # ComSeg framework
```

### Comparing `comseg-0.1/README.md` & `comseg-0.2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 
 <img src="./comseg.png" width="650" height="263">
 
 # News
+- Update with comseg 0.0.8. Compatibility with SOPA : https://gustaveroussy.github.io/sopa/
 
-Update with comseg 0.0.7. Computation of the co-expression matrix is now faster.
+- Update with comseg 0.0.7. Computation of the co-expression matrix is now faster.
 
 # Support
 
 If you have any questions relative to the package or bug, please open an issue in this repository.
 
 
 # ComSeg framework
```

### Comparing `comseg-0.1/src/ComSeg.egg-info/PKG-INFO` & `comseg-0.2/src/ComSeg.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: ComSeg
-Version: 0.1
+Version: 0.2
 Summary: single cell RNA profiling analysis of imaging-based spatial transcriptomics data
 Author-email: Thomas Defard <thomas.defard@mines-paristech.fr>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 <img src="./comseg.png" width="650" height="263">
 
 # News
+- Update with comseg 0.0.8. Compatibility with SOPA : https://gustaveroussy.github.io/sopa/
 
-Update with comseg 0.0.7. Computation of the co-expression matrix is now faster.
+- Update with comseg 0.0.7. Computation of the co-expression matrix is now faster.
 
 # Support
 
 If you have any questions relative to the package or bug, please open an issue in this repository.
 
 
 # ComSeg framework
```

### Comparing `comseg-0.1/src/comseg/clustering.py` & `comseg-0.2/src/comseg/clustering.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,18 +66,18 @@
         self.norm_genes = new_selected_genes
         self.norm_bool_index = bool_index
         row_indice = np.nonzero(np.sum(self.anndata.X[:, bool_index], axis=1) > 0)[0]
         row_indice = np.isin(list(range(len(self.anndata))), row_indice)
         count_matrix = self.anndata.X[:, bool_index].toarray()
         count_matrix = count_matrix[row_indice, :]
 
-        print(f'shape count matrix {count_matrix.shape}')
+        #print(f'shape count matrix {count_matrix.shape}')
         np.save("count_matrix", count_matrix)
         count_matrix = pd.DataFrame(count_matrix, columns=[str(e) for e in range(count_matrix.shape[1])])
-        print(count_matrix.columns)
+        #print(count_matrix.columns)
         norm_expression_vectors, param_sctransform = run_sctransform(count_matrix,
                                                                           debug_path=debug_path)
 
         self.param_sctransform = param_sctransform
         self.genes_to_take = bool_index
 
 
@@ -207,15 +207,15 @@
         :rtype: list[np.array], list[str]
 
         """
         assert aggregation_mode in ["mean", "median"], "arrgration_mode must be 'mean' or 'median'"
         scrna_unique_clusters = np.unique(list(self.anndata_cluster.obs[cluster_column_name]))
         scrna_centroids = []
         for cl in scrna_unique_clusters:
-            print(cl)
+            #print(cl)
             if aggregation_mode == "median":
                 centroid = np.median(self.anndata_cluster[self.anndata_cluster.obs[cluster_column_name] == cl].X, axis=0)
             else:
                 assert aggregation_mode == "mean"
                 centroid = np.mean(self.anndata_cluster[self.anndata_cluster.obs[cluster_column_name] == cl].X, axis=0)
         # print(mean)
             scrna_centroids.append(np.asarray(centroid)[0])
@@ -254,15 +254,15 @@
 
         array_label = np.array(self.anndata_cluster.obs[cluster_column_name]).astype(int)
         nb_cluster = len(np.unique(scrna_unique_clusters))
         for i in range(len(Z[:-1])):
             dist_corr = Z[i, 2]
             if dist_corr > 1 - min_merge_correlation or nb_cluster <= nb_min_cluster:
                 break
-            print(Z[i].round(2))
+            #print(Z[i].round(2))
             c1_to_merge = Z[i, 0]
             c2_to_merge = Z[i, 1]
             new_cluster = len(scrna_centroids) + i
             array_label[array_label == c1_to_merge] = new_cluster
             array_label[array_label == c2_to_merge] = new_cluster
             nb_cluster -= 1
 
@@ -286,20 +286,16 @@
 
         ### merge also anndata normal
         list_ori_leiden = np.array(self.anndata.obs[cluster_column_name])
         new_list_ori_leiden = []
         for cluster_id in list_ori_leiden:
             new_list_ori_leiden.append(dico_ori_merge[cluster_id])
         self.anndata.obs[column_name] = new_list_ori_leiden
+        print(f"number of cluster after merging {len(dico_merge_ori) }")
 
-        try:
-
-            print(f"number of cluster after merging {len(dico_merge_ori) }")
-        except:
-            print(" no merging done?")
 
         return self.anndata_cluster.obs[column_name]
 
     def classify_by_nn(self,
                         array_of_vect,
                        pca_model,
                        kn_neighb,
```

### Comparing `comseg-0.1/src/comseg/dataset.py` & `comseg-0.2/src/comseg/dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,17 +51,17 @@
         :default mask_file_extension: ".tiff"
         :param dict_scale: dictionary containing the pixel/voxel size of the images in µm default is {"x": 0.103, 'y': 0.103, "z": 0.3}
         :type dict_scale: dict
         :param mean_cell_diameter: the expected mean cell diameter in µm default is 15µm
         :type mean_cell_diameter: float
         :param gene_column: name of the column containing the gene name in the csv files
         :type gene_column: str
-        :param image_names_csv_file: list of image name as csv_file to consider in the dataset if None consider all the csv files in the folder
+        :param image_names_csv_file: list of image csv file name to consider in the dataset if None consider all the csv files in the folder
         :type image_names_csv_file: list
-        :param centroid_name: list of the centroid as to be in the same order as the image_names_csv_file
+        :param centroid_name: list of the centroid csv file name , as to be in the same order as the image_names_csv_file
         :type centroid_name: list
         """
 
         self.path_dataset_folder = Path(path_dataset_folder)
         if path_to_mask_prior is not None:
             self.path_to_mask_prior = Path(path_to_mask_prior)
         else:
@@ -152,33 +152,42 @@
                 df_spots.to_csv(image_path_df.parent /(image_path_df.stem+'_pixel.csv'), index=False)
 
 
 
     #### fct adding prior
 
     def add_prior_from_mask(self,
-                            prior_keys_name = 'in_nucleus',
+                            config = None,
+                            prior_name = 'in_nucleus',
                             overwrite = False,
-                            compute_centroid = False,
+                            compute_centroid = True,
                             regex_df = "*.csv"
                             ):
 
         """
 
         This function add prior knowledge to the dataset. It adds a column in the csv files indicating prior label of each spot.
-        It takes the positition of each spot and add the corresponding value of the mask prior at this position.
+        It takes the positition of each spot and add the corresponding value of the segmentation mask prior (.tiff) at this position.
 
-        :param prior_keys_name: name of the column to add in the csv files containing the prior label of each spot
+        :param prior_name: name of the column to add in the csv files containing the prior label of each spot
         :type str
-        :param overwrite: if True, overwrite the prior_keys_name column if it already exists
+        :param overwrite: if True, overwrite the prior_name column if it already exists
         :type bool
         :param compute_centroid : if True, compute the centroid of each cell/nucleus in segmentation mask for to use it for RNA-cell association
         :type bool
         :return: None
         """
+
+        if config is not None:
+            print("config dict overwritting default parameters")
+            prior_name = config.get("prior_name", prior_name)
+            overwrite = config.get("overwrite", overwrite)
+            compute_centroid = config.get("compute_centroid", compute_centroid)
+            regex_df = config.get("regex_df", regex_df)
+
         if compute_centroid:
             self.dict_centroid = {}
         for image_path_df in self.path_dataset_folder.glob(regex_df):
             print(f"add prior to {image_path_df.stem}")
             df_spots = pd.read_csv(image_path_df)
 
             assert (self.path_to_mask_prior / (image_path_df.stem + self.mask_file_extension)  ).exists(), f"no mask prior found for {image_path_df.stem}"
@@ -196,17 +205,17 @@
                 prior_list = [mask[z, y, x] for (z, y, x) in pixel_coordinates]
 
             else:
                 pixel_coordinates = (df_spots[["y",  "x"]]).astype(int).values
                 prior_list = [mask[y, x] for (y, x) in pixel_coordinates]
 
 
-            if prior_keys_name in df_spots.columns and overwrite == False:
-                raise Exception(f"prior_keys_name {prior_keys_name} already in df_spots and overwrite is False")
-            df_spots[prior_keys_name] = prior_list
+            if prior_name in df_spots.columns and overwrite == False:
+                raise Exception(f"prior_name {prior_name} already in df_spots and overwrite is False")
+            df_spots[prior_name] = prior_list
             df_spots.to_csv(image_path_df,  index=False)
             print(f"prior added to {image_path_df.stem} and saved in csv file")
 
 
             if compute_centroid:
                 dict_centroid = compute_dict_centroid(mask_nuclei = mask,
                                                       background=0)
@@ -230,14 +239,18 @@
         Compute the co-expression score matrix for the RNA spatial distribution
 
         :param df_spots_label:  dataframe with the columns x,y,z,gene. the coordinates are rescaled in µm by dict_scale attribute of the dataset object
         :type df_spots_label: pd.DataFrame
         :param n_neighbors: maximum number of neighbors default is 40
         :type n_neighbors: int
         :param radius: maximum radius of neighbors. It should be set proportionnaly to expected cell size, default is radius =  mean_cell_diameter / 2
+        :param sampling : if True, sample the dataset to compute the correlation
+        :type sampling: bool
+        :param sampling_size: if sampling is True : number of proximity weighted expression vector to sample
+        :type sampling_size: int
         :return: count_matrix of shape (N_rna,  n_genes) where n_genes is the number of unique genes in df_spots_label
         each row is an 'RNA expression vector' summarizing local expression neighborhood of a molecule
         :rtype: np.array
         """
 
         gene_index_dico = {}
         for gene_id in range(len(self.selected_genes)):
@@ -358,27 +371,32 @@
                     corr = -1
                 dico_proba_edge[self.selected_genes[gene_source]][self.selected_genes[gene_target]] = corr
                 dico_proba_edge[self.selected_genes[gene_target]][self.selected_genes[gene_source]] = corr
         return dico_proba_edge
 
     def compute_edge_weight(
             self,
+            config = None,
             images_subset = None,
             n_neighbors=40,
             radius= None ,  # in micormeter
             distance="pearson",
             sampling=True,
             sampling_size=10000,
     remove_self_node = False):
 
+
+
         #print("adapt to when I prune")
 
         """
         compute the gene co-expression correlation at the dataset scale
 
+        :param config: dictionary of parameters to overwrite the default parameters, default is None
+        :type config: dict
         :param images_subset: default None, if not None, only compute the correlation on the images in the list
         :type images_subset: list
         :param n_neighbors:  default 40 ,number of neighbors to consider in the knn graph
         :type n_neighbors: int
         :param radius: radius of the knn graph in micrometer default None, if None, radius = mean_cell_diameter/2
         :type radius: float
         :param distance: choose in ["pearson", "spearman"] default is pearson
@@ -388,14 +406,25 @@
         :param sampling_size: if sampling is True : number of proximity weighted expression vector to sample
         :return:
            - dico_proba_edge - a dictionary of dictionary correlation between genes. dict[gene_source][gene_target] = correlation
            - count_matrix - the count matrix used to compute the correlation
         :rtype:  dict, np.array
         """
 
+
+        if config is not None:
+            #print("config dict overwritting default parameters")
+            images_subset = config.get("images_subset", images_subset)
+            n_neighbors = config.get("n_neighbors", n_neighbors)
+            radius = config.get("radius", radius)
+            distance = config.get("distance", distance)
+            sampling = config.get("sampling", sampling)
+            sampling_size = config.get("sampling_size", sampling_size)
+
+
         if radius is None:
             radius = self.mean_cell_diameter / 2
 
         dico_proba_edge = {}
 
         list_of_count_matrix = []
         assert self.__len__() > 0, "no images in the dataset"
@@ -419,18 +448,18 @@
                                                         remove_self_node=remove_self_node,
                                                               sampling=True,
                                                               sampling_size=int(sampling_size/len(list_img) +1))
             list_of_count_matrix.append(count_matrix)
             count_matrix = np.concatenate(list_of_count_matrix, axis=0)
         if sampling:
             if len(count_matrix) > sampling_size:
-                print("count_matrix.shape", count_matrix.shape)
-                print(f"sampling {sampling} vectors")
+                #print("count_matrix.shape", count_matrix.shape)
+                #print(f"sampling {sampling} vectors")
                 count_matrix = count_matrix[np.random.choice(count_matrix.shape[0], sampling_size, replace=False), :]
-                print("count_matrix.shape", count_matrix.shape)
+                #print("count_matrix.shape", count_matrix.shape)
 
         dict_co_expression = self.get_dict_proba_edge_in_situ(count_matrix=count_matrix,
                                                           distance=distance,
                                                           )
         self.dict_co_expression = dict_co_expression
         return dico_proba_edge, count_matrix
```

### Comparing `comseg-0.1/src/comseg/dictionary.py` & `comseg-0.2/src/comseg/dictionary.py`

 * *Files 6% similar despite different names*

```diff
@@ -364,15 +364,15 @@
 
         :param path_dict_cell_centroid: If computed already by the ``ComSegDataset`` class from prior Maks leave it None.
         Otherwise : path_dict_cell_centroid is a  Path to the folder containing the centroid dictionary {cell : {z:,y:,x:}} for each image.
                          Each centroid dictionary has to be stored in a file in a npy format,  named as the image name.
         :type path_dict_cell_centroid: str
         :param n_neighbors: number of neighbors to consider for the classification of the centroid (default 15)
         :type n_neighbors: int
-        :param dict_in_pixel: if True the centroid are in pixel and rescal if False the centroid are in um (default True)
+        :param dict_in_pixel: if True the centroid are in the same scale than the input csv of spots coorrdinates and rescale with dict_scale if False the centroid are in um (default True)
         :type dict_in_pixel: bool
         :param max_dist_centroid: maximum distance to consider for the centroid (default None)
         :type max_dist_centroid: int
         :param key_pred: key of the node attribute containing the cluster id (default "leiden_merged")
         :type key_pred: str
         :param convex_hull_centroid: check that cell centroid is in the convex hull of its RNA neighbors (default True). If not the cell centroid is not classify to avoid artefact misclassification
         :type convex_hull_centroid: bool
@@ -420,14 +420,15 @@
     #### Apply diskjtra
 
 
     def associate_rna2landmark(self,
         key_pred="leiden_merged",
         distance='distance',
         max_cell_radius=100):
+
         """
         Associate RNAs to landmarks based on the both transcriptomic landscape and the
         distance between the RNAs and the centroids of the landmark
 
 
         :param key_pred: key of the node attribute containing the cluster id (default "leiden_merged")
         :type key_pred: str
@@ -444,46 +445,57 @@
             self[img_name].associate_rna2landmark(
                 key_pred=key_pred,
                 prior_name=self.prior_name,
                 distance=distance,
                 max_cell_radius=max_cell_radius)
 
     def anndata_from_comseg_result(self,
-                                   key_cell_pred='cell_index_pred',
-                                   return_polygon=False,
+                                   config : dict = None,
+                                   min_rna_per_cell=5,
+                                   return_polygon=True,
                                    alpha=0.5,
-                                   min_rna_per_cell=5
+                                   allow_disconnected_polygon=False
                                    ):
 
         """
         Return an anndata with the estimated expression vector of each cell in the dataset plus the spot positions.
 
         :param self:
-        :param key_cell_pred: leave it to default
-        :type key_cell_pred: str
-        :param return_polygon: if True return the polygon of the cells
+        :param config: dictionary of parameters to overwrite the default parameters, default is None
+        :type config: dict
+        :param min_rna_per_cell: minimum number of RNA to consider a cell
+        :type min_rna_per_cell: int
+        :param return_polygon: if True return the polygon of the cells, the polygon are computed using the alphashape library
         :type return_polygon: bool
         :param alpha: alpha parameter to compute the alphashape polygone : https://pypi.org/project/alphashape/.
          alpha is between 0 and 1, 1 correspond to the convex hull of the cell
         :type alpha: float
-        :param min_rna_per_cell: minimum number of RNA to consider a cell
-        :type min_rna_per_cell: int
+        :param allow_disconnected_polygon: if True allow disconnected polygon
+
         :return:
         """
         list_image_name = []
         anndata_list = []
         dict_df_spots = {}
         dict_json_img = {}
 
+        if config is not None:
+            print("config dict overwritting the default parameters")
+            min_rna_per_cell = config.get("min_rna_per_cell", min_rna_per_cell)
+            return_polygon = config.get("return_polygon", return_polygon)
+            alpha = config.get("alpha", alpha)
+            allow_disconnected_polygon = config.get("allow_disconnected_polygon", allow_disconnected_polygon)
+
         for img_name in tqdm(self):
             anndata, json_dict = self[img_name].get_anndata_from_result(
-                key_cell_pred=key_cell_pred,
+                key_cell_pred='cell_index_pred',
+                min_rna_per_cell=min_rna_per_cell,
                 return_polygon=return_polygon,
                 alpha=alpha,
-                min_rna_per_cell=min_rna_per_cell)
+                allow_disconnected_polygon=allow_disconnected_polygon)
             dict_json_img[img_name] = json_dict
 
             anndata_list.append(anndata)
             list_image_name += [img_name] * len(anndata)
             dict_df_spots[img_name] = anndata.uns["df_spots"]
 
             assert np.array_equal(anndata.var_names, self.dataset.selected_genes), "The anndata var names are not the same as the dataset selected genes"
@@ -496,53 +508,83 @@
         self.final_anndata.var_names = self.dataset.selected_genes
         self.final_anndata.uns["df_spots"] = dict_df_spots
         return self.final_anndata, dict_json_img
 
 
 
     def run_all(self,
-                max_cell_radius,
+                config : dict = None,
+                k_nearest_neighbors: int = 10,
+                max_cell_radius : float = 15,
                 ## in situ clutering parameter
-                size_commu_min = 3,
-                norm_vector = False,
-                    ### parameter clustering
-                n_pcs = 3,
-                n_comps = 3,
-                clustering_method = "leiden",
-                n_neighbors = 20,
-                resolution = 1,
+                size_commu_min : int | int  = 3,
+                norm_vector : bool = False,
+                n_pcs : int = 3,
+                clustering_method : str | str = "leiden",
+                n_neighbors : int | int = 20,
+                resolution  : float | float = 1,
                 n_clusters_kmeans = 4,
-                palette = None,
-                nb_min_cluster = 0,
-                min_merge_correlation = 0.8,
+                nb_min_cluster : int | int = 0,
+                min_merge_correlation : float | float = 0.8,
                 ### classify centroid
-                path_dataset_folder_centroid=None,
-                file_extension=".csv"
+                path_dataset_folder_centroid: str | str =None,
+                file_extension: str | str = ".csv",
                 ):
         """
         function running all the ComSeg steps: (compute_community_vector(),
         compute_insitu_clustering(), add_cluster_id_to_graph(), classify_centroid(), associate_rna2landmark() )
-        :param max_cell_radius:
-        :param size_commu_min:
-        :param norm_vector:
-        :param n_pcs:
-        :param n_comps:
-        :param clustering_method:
-        :param n_neighbors:
-        :param resolution:
-        :param n_clusters_kmeans:
-        :param palette:
-        :param nb_min_cluster:
-        :param min_merge_correlation:
-        :param path_dataset_folder_centroid:
-        :param file_extension:
+        :param config: dictionary of parameters to overwrite the default parameters, default is None
+        :type config: dict
+        :param k_nearest_neighbors: number of nearest neighbors to consider for the KNN graph creation, reduce K to speed computation
+        :type k_nearest_neighbors: int
+        :param max_cell_radius: maximum distance between a cell centroid and an RNA to be associated
+        :type max_cell_radius: float
+        :param size_commu_min: minimum number of RNA in a community to be considered for the clustering (default 3)
+        :type size_commu_min: int
+        :param norm_vector: if True, the expression vector will be normalized using the scTRANSFORM normalization parameters, the normaliztion requires the following R package : sctransform, feather, arrow
+        The normalization is important to do on dataset with a high number of gene.
+        :type norm_vector: bool
+        :param n_pcs: number of principal component to compute for the clustering of the RNA communities expression vector; Lets 0 if no pca
+        :type n_pcs: int
+        :param clustering_method: choose in ["leiden", "kmeans", "louvain"]
+        :type clustering_method: str
+        :param n_neighbors: number of neighbors similarity graph of the RNA communities expression vector clustering
+        :type n_neighbors: int
+        :param resolution:  resolution paramter  for the in-situ-clustering step if louvain or leiden are used
+        :type resolution: float
+        :param n_clusters_kmeans: number of cluster for the kmeans clustering for ```clustering_method```= "kmeans"
+        :type n_clusters_kmeans: int
+        :param nb_min_cluster: minimum number of cluster to keep after the merge of the cluster
+        :type nb_min_cluster: int
+        :param min_merge_correlation: minimum correlation to merge cluster in the in situ clustering
+        :type min_merge_correlation: float
+        :param path_dataset_folder_centroid: path to the folder containing the centroid in a csv or dictionary {cell : {z:,y:,x:}} for each image, use the same scale than then input csv
+        :type path_dataset_folder_centroid: str
+        :param file_extension: file extension of the centroid dictionary (.npy) or csv file (.csv)
+        :type file_extension: str
         :return:
         """
+        if config is not None:
+            #print("config dict overwritting the default parameter")
+            k_nearest_neighbors = config.get("k_nearest_neighbors", k_nearest_neighbors)
+            max_cell_radius = config.get("max_cell_radius", max_cell_radius)
+            size_commu_min = config.get("size_commu_min", size_commu_min)
+            norm_vector = config.get("norm_vector", norm_vector)
+            n_pcs = config.get("n_pcs", n_pcs)
+            clustering_method = config.get("clustering_method", clustering_method)
+            n_neighbors = config.get("n_neighbors", n_neighbors)
+            resolution = config.get("resolution", resolution)
+            n_clusters_kmeans = config.get("n_clusters_kmeans", n_clusters_kmeans)
+            nb_min_cluster = config.get("nb_min_cluster", nb_min_cluster)
+            min_merge_correlation = config.get("min_merge_correlation", min_merge_correlation)
+            path_dataset_folder_centroid = config.get("path_dataset_folder_centroid", path_dataset_folder_centroid)
+            file_extension = config.get("file_extension", file_extension)
+
 
-        self.compute_community_vector()
+        self.compute_community_vector(k_nearest_neighbors = k_nearest_neighbors)
 
         self.compute_insitu_clustering(
             size_commu_min=size_commu_min,
             norm_vector=norm_vector,
             ### parameter clustering
             n_pcs=n_pcs,
             n_comps=n_pcs,
@@ -557,15 +599,14 @@
 
         self.add_cluster_id_to_graph(clustering_method="leiden_merged")
 
         self.classify_centroid(
             path_cell_centroid=path_dataset_folder_centroid,
             n_neighbors=15,
             dict_in_pixel=True,
-            max_dist_centroid=None,
             key_pred="leiden_merged",
             distance="ngb_distance_weights",
             file_extension=file_extension
         )
 
         self.associate_rna2landmark(
             key_pred="leiden_merged",
```

### Comparing `comseg-0.1/src/comseg/model.py` & `comseg-0.2/src/comseg/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -687,29 +687,29 @@
 
     def get_anndata_from_result(
                 self,
                key_cell_pred =  'cell_index_pred',
                 return_polygon = False,
                 alpha = 0.5,
                 min_rna_per_cell = 5,
-                allow_disconnected_polygone = False
+                allow_disconnected_polygon = False
                ):
         """
         Generate an anndata storing the estimated expression vector and their spots coordinates
 
         :param key_cell_pred:  key of the cell prediction in the graph (default cell_index_pred)
         :type key_cell_pred: str
         :param return_polygon: if True return the polygon of the cells
         :type return_polygon: bool
         :param alpha: alpha parameter to compute the alphashape polygone : https://pypi.org/project/alphashape/.
          alpha is between 0 and 1, 1 correspond to the convex hull of the cell
         :type alpha: float
         :param min_rna_per_cell: minimum number of RNA to consider a cell
         :type min_rna_per_cell: int
-        :param allow_disconnected_polygone: if True allow disconnected polygon
+        :param allow_disconnected_polygon: if True allow disconnected polygon
         :return:
         """
 
         dict_cell_genes = {}
         dict_cell_genes_coordinate = {}
         dict_cell_genes_name = {}
         dict_cell_genes_mol_index = {}
@@ -851,11 +851,11 @@
                     if allow_disconnected_polygone:
                         json_dict["geometries"].append({
                             "type": "Polygon",
                             "coordinates": [list(poly.exterior.coords)],
                             "cell": cell
                         })
                     else:
-                        raise ValueError("disconnected polygon are not allowed change allow_disconnected_polygon=True")
+                        raise ValueError("disconnected polygons are not allowed, change allow_disconnected_polygon=True")
             else:
                 continue
         return anndata, json_dict
```

### Comparing `comseg-0.1/src/comseg/utils/custom_louvain.py` & `comseg-0.2/src/comseg/utils/custom_louvain.py`

 * *Files identical despite different names*

### Comparing `comseg-0.1/src/comseg/utils/plot.py` & `comseg-0.2/src/comseg/utils/plot.py`

 * *Files identical despite different names*

### Comparing `comseg-0.1/src/comseg/utils/preprocessing.py` & `comseg-0.2/src/comseg/utils/preprocessing.py`

 * *Files identical despite different names*

### Comparing `comseg-0.1/src/comseg/utils/utils_graph.py` & `comseg-0.2/src/comseg/utils/utils_graph.py`

 * *Files identical despite different names*

