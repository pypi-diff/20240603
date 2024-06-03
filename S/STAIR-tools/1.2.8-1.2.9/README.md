# Comparing `tmp/STAIR-tools-1.2.8.tar.gz` & `tmp/STAIR-tools-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "STAIR-tools-1.2.8.tar", last modified: Sat May 11 08:21:29 2024, max compression
+gzip compressed data, was "STAIR-tools-1.2.9.tar", last modified: Mon Jun  3 09:21:06 2024, max compression
```

## Comparing `STAIR-tools-1.2.8.tar` & `STAIR-tools-1.2.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-05-11 08:21:29.076707 STAIR-tools-1.2.8/
--rw-r--r--   0 yuanyuan   (501) staff       (20)      253 2024-05-11 08:21:29.076477 STAIR-tools-1.2.8/PKG-INFO
--rwxr-xr-x   0 yuanyuan   (501) staff       (20)     1320 2023-12-25 02:00:08.000000 STAIR-tools-1.2.8/README.md
-drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-05-11 08:21:29.072338 STAIR-tools-1.2.8/STAIR/
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     8661 2023-12-23 11:23:09.000000 STAIR-tools-1.2.8/STAIR/ABA_annotation.py
-drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-05-11 08:21:29.072565 STAIR-tools-1.2.8/STAIR/ABAanno/
--rw-------   0 yuanyuan   (501) staff       (20)      120 2023-08-11 07:05:03.000000 STAIR-tools-1.2.8/STAIR/ABAanno/__init__.py
--rw-------   0 yuanyuan   (501) staff       (20)      120 2023-08-11 07:05:03.000000 STAIR-tools-1.2.8/STAIR/__init__.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)    18514 2024-05-06 15:17:54.000000 STAIR-tools-1.2.8/STAIR/emb_alignment.py
-drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-05-11 08:21:29.074397 STAIR-tools-1.2.8/STAIR/embedding/
--rw-------   0 yuanyuan   (501) staff       (20)      120 2024-04-25 02:41:10.000000 STAIR-tools-1.2.8/STAIR/embedding/__init__.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     3804 2024-05-04 11:27:47.000000 STAIR-tools-1.2.8/STAIR/embedding/dataset_ae.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     6047 2024-05-07 05:16:40.000000 STAIR-tools-1.2.8/STAIR/embedding/dataset_hgat.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)      988 2023-12-23 11:23:12.000000 STAIR-tools-1.2.8/STAIR/embedding/loss.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     5493 2023-12-23 11:23:12.000000 STAIR-tools-1.2.8/STAIR/embedding/module_ae.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     8658 2023-12-23 11:23:12.000000 STAIR-tools-1.2.8/STAIR/embedding/module_hgat.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     6954 2023-12-23 11:23:12.000000 STAIR-tools-1.2.8/STAIR/embedding/module_hgat1.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)    12477 2024-05-11 08:20:36.000000 STAIR-tools-1.2.8/STAIR/loc_alignment.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)    14363 2024-05-11 08:19:13.000000 STAIR-tools-1.2.8/STAIR/loc_prediction.py
-drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-05-11 08:21:29.075744 STAIR-tools-1.2.8/STAIR/location/
--rw-------   0 yuanyuan   (501) staff       (20)      120 2023-08-11 07:05:03.000000 STAIR-tools-1.2.8/STAIR/location/__init__.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     7819 2023-12-23 11:23:12.000000 STAIR-tools-1.2.8/STAIR/location/align_fine.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)    12278 2024-05-11 08:16:53.000000 STAIR-tools-1.2.8/STAIR/location/align_init.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     8534 2023-12-23 11:23:13.000000 STAIR-tools-1.2.8/STAIR/location/edge_detection.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     9354 2023-12-23 11:23:13.000000 STAIR-tools-1.2.8/STAIR/location/edge_detection1.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     2298 2023-12-23 11:23:13.000000 STAIR-tools-1.2.8/STAIR/location/transformation.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     2821 2023-12-23 11:23:13.000000 STAIR-tools-1.2.8/STAIR/utils.py
-drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-05-11 08:21:29.076293 STAIR-tools-1.2.8/STAIR_tools.egg-info/
--rw-r--r--   0 yuanyuan   (501) staff       (20)      253 2024-05-11 08:21:29.000000 STAIR-tools-1.2.8/STAIR_tools.egg-info/PKG-INFO
--rw-r--r--   0 yuanyuan   (501) staff       (20)      702 2024-05-11 08:21:29.000000 STAIR-tools-1.2.8/STAIR_tools.egg-info/SOURCES.txt
--rw-r--r--   0 yuanyuan   (501) staff       (20)        1 2024-05-11 08:21:29.000000 STAIR-tools-1.2.8/STAIR_tools.egg-info/dependency_links.txt
--rw-r--r--   0 yuanyuan   (501) staff       (20)        6 2024-05-11 08:21:29.000000 STAIR-tools-1.2.8/STAIR_tools.egg-info/top_level.txt
--rw-r--r--   0 yuanyuan   (501) staff       (20)       38 2024-05-11 08:21:29.076754 STAIR-tools-1.2.8/setup.cfg
--rw-------   0 yuanyuan   (501) staff       (20)      489 2024-05-11 08:21:05.000000 STAIR-tools-1.2.8/setup.py
+drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-06-03 09:21:06.716671 STAIR-tools-1.2.9/
+-rw-r--r--   0 yuanyuan   (501) staff       (20)      253 2024-06-03 09:21:06.716479 STAIR-tools-1.2.9/PKG-INFO
+-rwxr-xr-x   0 yuanyuan   (501) staff       (20)     1320 2023-12-25 02:00:08.000000 STAIR-tools-1.2.9/README.md
+drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-06-03 09:21:06.711553 STAIR-tools-1.2.9/STAIR/
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     8661 2023-12-23 11:23:09.000000 STAIR-tools-1.2.9/STAIR/ABA_annotation.py
+drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-06-03 09:21:06.711878 STAIR-tools-1.2.9/STAIR/ABAanno/
+-rw-------   0 yuanyuan   (501) staff       (20)      120 2023-08-11 07:05:03.000000 STAIR-tools-1.2.9/STAIR/ABAanno/__init__.py
+-rw-------   0 yuanyuan   (501) staff       (20)      120 2023-08-11 07:05:03.000000 STAIR-tools-1.2.9/STAIR/__init__.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)    18514 2024-05-06 15:17:54.000000 STAIR-tools-1.2.9/STAIR/emb_alignment.py
+drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-06-03 09:21:06.714237 STAIR-tools-1.2.9/STAIR/embedding/
+-rw-------   0 yuanyuan   (501) staff       (20)      120 2024-04-25 02:41:10.000000 STAIR-tools-1.2.9/STAIR/embedding/__init__.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     3804 2024-05-04 11:27:47.000000 STAIR-tools-1.2.9/STAIR/embedding/dataset_ae.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     6047 2024-05-07 05:16:40.000000 STAIR-tools-1.2.9/STAIR/embedding/dataset_hgat.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)      988 2023-12-23 11:23:12.000000 STAIR-tools-1.2.9/STAIR/embedding/loss.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     5493 2023-12-23 11:23:12.000000 STAIR-tools-1.2.9/STAIR/embedding/module_ae.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     8658 2023-12-23 11:23:12.000000 STAIR-tools-1.2.9/STAIR/embedding/module_hgat.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     6954 2023-12-23 11:23:12.000000 STAIR-tools-1.2.9/STAIR/embedding/module_hgat1.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)    12580 2024-06-03 09:18:05.000000 STAIR-tools-1.2.9/STAIR/loc_alignment.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)    14363 2024-05-11 08:19:13.000000 STAIR-tools-1.2.9/STAIR/loc_prediction.py
+drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-06-03 09:21:06.715680 STAIR-tools-1.2.9/STAIR/location/
+-rw-------   0 yuanyuan   (501) staff       (20)      120 2023-08-11 07:05:03.000000 STAIR-tools-1.2.9/STAIR/location/__init__.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     7819 2023-12-23 11:23:12.000000 STAIR-tools-1.2.9/STAIR/location/align_fine.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)    12378 2024-06-03 09:19:06.000000 STAIR-tools-1.2.9/STAIR/location/align_init.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     8534 2023-12-23 11:23:13.000000 STAIR-tools-1.2.9/STAIR/location/edge_detection.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     9354 2023-12-23 11:23:13.000000 STAIR-tools-1.2.9/STAIR/location/edge_detection1.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     2298 2023-12-23 11:23:13.000000 STAIR-tools-1.2.9/STAIR/location/transformation.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     2821 2023-12-23 11:23:13.000000 STAIR-tools-1.2.9/STAIR/utils.py
+drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-06-03 09:21:06.716249 STAIR-tools-1.2.9/STAIR_tools.egg-info/
+-rw-r--r--   0 yuanyuan   (501) staff       (20)      253 2024-06-03 09:21:06.000000 STAIR-tools-1.2.9/STAIR_tools.egg-info/PKG-INFO
+-rw-r--r--   0 yuanyuan   (501) staff       (20)      702 2024-06-03 09:21:06.000000 STAIR-tools-1.2.9/STAIR_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 yuanyuan   (501) staff       (20)        1 2024-06-03 09:21:06.000000 STAIR-tools-1.2.9/STAIR_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 yuanyuan   (501) staff       (20)        6 2024-06-03 09:21:06.000000 STAIR-tools-1.2.9/STAIR_tools.egg-info/top_level.txt
+-rw-r--r--   0 yuanyuan   (501) staff       (20)       38 2024-06-03 09:21:06.716736 STAIR-tools-1.2.9/setup.cfg
+-rw-------   0 yuanyuan   (501) staff       (20)      489 2024-06-03 09:21:04.000000 STAIR-tools-1.2.9/setup.py
```

### Comparing `STAIR-tools-1.2.8/README.md` & `STAIR-tools-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.8/STAIR/ABA_annotation.py` & `STAIR-tools-1.2.9/STAIR/ABA_annotation.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.8/STAIR/emb_alignment.py` & `STAIR-tools-1.2.9/STAIR/emb_alignment.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.8/STAIR/embedding/dataset_ae.py` & `STAIR-tools-1.2.9/STAIR/embedding/dataset_ae.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.8/STAIR/embedding/dataset_hgat.py` & `STAIR-tools-1.2.9/STAIR/embedding/dataset_hgat.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.8/STAIR/embedding/loss.py` & `STAIR-tools-1.2.9/STAIR/embedding/loss.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.8/STAIR/embedding/module_ae.py` & `STAIR-tools-1.2.9/STAIR/embedding/module_ae.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.8/STAIR/embedding/module_hgat.py` & `STAIR-tools-1.2.9/STAIR/embedding/module_hgat.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.8/STAIR/embedding/module_hgat1.py` & `STAIR-tools-1.2.9/STAIR/embedding/module_hgat1.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.8/STAIR/loc_alignment.py` & `STAIR-tools-1.2.9/STAIR/loc_alignment.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,16 @@
         '''
         self.init_align_key = init_align_key
         self.init_adatas, anchors, self.Ts_init, scales = initial_alignment(self.adata_list, 
 		                                                                    spatial_key = spatial_key,
 		                                                                    emb_key = emb_key,
 		                                                                    num_mnn = num_mnn,
 		                                                                    key_added = init_align_key,
-		                                                                    use_scale = use_scale
+		                                                                    use_scale = use_scale,
+                                                                            batch_order = batch_order
 		                                                                )
         # self.boundary = [(anchor[:,0].tolist(), anchor[:,1].tolist()) for anchor in anchors]
         
         if self.make_log:
             self.makeLog(f"Parameter set for initial alignment")
             self.makeLog(f"  Starting coordinates: {spatial_key}")
             self.makeLog(f"  K of MNN: {num_mnn}")
```

### Comparing `STAIR-tools-1.2.8/STAIR/loc_prediction.py` & `STAIR-tools-1.2.9/STAIR/loc_prediction.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.8/STAIR/location/align_fine.py` & `STAIR-tools-1.2.9/STAIR/location/align_fine.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.8/STAIR/location/align_init.py` & `STAIR-tools-1.2.9/STAIR/location/align_init.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     Returns:
       adata1 with 'transformed' in .obsm
       adata2 with 'transformed' in .obsm
       pair: np.array of indices of nearest neighbor pairs
       T: transformation matrix with 3 x 3
     '''
     
-    print(f'Finding similar pairs using {emb_key}...')
+    # print(f'Finding similar pairs using {emb_key}...')
     
     # Extract features used to calculate spot similarity
     emb1_tmp = adata1.obsm[emb_key]
     emb2_tmp = adata2.obsm[emb_key]
     
     # Search for mutual nearest neighbors of two slices
     neigh1 = NearestNeighbors(n_neighbors=num_mnn, metric='cosine')
@@ -85,15 +85,16 @@
 
 
 def initial_alignment(  adatas, 
                         spatial_key = 'spatial',
                         emb_key = 'HAN_SE',
                         num_mnn = 1, 
                         key_added = 'transform_init',
-                        use_scale = False
+                        use_scale = False,
+                        batch_order = None
                       ):
     
     '''
     Perform initial alignment for adatas according to the similarity of emb_key.
     Input:
       adatas:       Adata list to be aligned
       spatial_key:  Key of spatial coordinates in .obsm 
@@ -107,15 +108,16 @@
     
     aligned_init = []
     anchors = []
     Ts = []
     scales = []
     
 
-    print('Performing initial alignment of the 1 pair of data...')
+    print('Performing initial alignment...')
+    print(f'    Aligning slice {batch_order[1]} to {batch_order[0]}...')
     
     # initial alignment of the first two adatas
     adata1, adata2 = adatas[0], adatas[1]
     
     adata1, adata2, anchor_tmp, T_tmp, scale_tmp = align_init_pair( adata1, 
                                                                     adata2, 
                                                                     spatial_key1 = spatial_key,
@@ -132,15 +134,15 @@
     Ts.append(T_tmp)
     scales.append(scale_tmp)
     
     # initial alignment of the rest adatas
     if len(aligned_init)!=len(adatas):
         for i in range(1, len(adatas)-1):
             
-            print(f'Performing initial alignment of the {i+1} pair of data...')
+            print(f'    Aligning slice {batch_order[i+1]} to {batch_order[i]}...')
             
             adata1_tmp = aligned_init[-1]
             adata2_tmp = adatas[i+1]
             
             for T_ in Ts:
                 adata2_tmp.obsm[spatial_key] = transform(adata2_tmp.obsm[spatial_key], T_)
```

### Comparing `STAIR-tools-1.2.8/STAIR/location/edge_detection.py` & `STAIR-tools-1.2.9/STAIR/location/edge_detection.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.8/STAIR/location/edge_detection1.py` & `STAIR-tools-1.2.9/STAIR/location/edge_detection1.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.8/STAIR/location/transformation.py` & `STAIR-tools-1.2.9/STAIR/location/transformation.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.8/STAIR/utils.py` & `STAIR-tools-1.2.9/STAIR/utils.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.8/STAIR_tools.egg-info/SOURCES.txt` & `STAIR-tools-1.2.9/STAIR_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

