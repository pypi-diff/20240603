# Comparing `tmp/featuremap-learn-1.0.1.tar.gz` & `tmp/featuremap-learn-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featuremap-learn-1.0.1.tar", last modified: Thu May 30 03:44:34 2024, max compression
+gzip compressed data, was "featuremap-learn-1.0.2.tar", last modified: Mon Jun  3 00:44:40 2024, max compression
```

## Comparing `featuremap-learn-1.0.1.tar` & `featuremap-learn-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 uqyyao4    (503) staff       (20)        0 2024-05-30 03:44:34.113550 featuremap-learn-1.0.1/
--rw-r--r--   0 uqyyao4    (503) staff       (20)     1496 2024-05-29 05:12:06.000000 featuremap-learn-1.0.1/LICENSE
--rw-r--r--   0 uqyyao4    (503) staff       (20)     5169 2024-05-30 03:44:34.112303 featuremap-learn-1.0.1/PKG-INFO
--rw-r--r--   0 uqyyao4    (503) staff       (20)     3957 2024-05-29 05:12:06.000000 featuremap-learn-1.0.1/README.md
-drwxr-xr-x   0 uqyyao4    (503) staff       (20)        0 2024-05-30 03:44:34.103928 featuremap-learn-1.0.1/featuremap/
--rw-r--r--   0 uqyyao4    (503) staff       (20)      341 2024-05-29 05:12:06.000000 featuremap-learn-1.0.1/featuremap/__init__.py
--rw-r--r--   0 uqyyao4    (503) staff       (20)    23586 2024-05-29 05:12:06.000000 featuremap-learn-1.0.1/featuremap/core_transition_state.py
--rw-r--r--   0 uqyyao4    (503) staff       (20)    97070 2024-05-29 05:12:06.000000 featuremap-learn-1.0.1/featuremap/featuremap_.py
--rw-r--r--   0 uqyyao4    (503) staff       (20)    39528 2024-05-29 05:12:06.000000 featuremap-learn-1.0.1/featuremap/features.py
--rw-r--r--   0 uqyyao4    (503) staff       (20)    28803 2024-05-29 05:12:06.000000 featuremap-learn-1.0.1/featuremap/layouts.py
--rw-r--r--   0 uqyyao4    (503) staff       (20)     1226 2024-05-29 05:12:06.000000 featuremap-learn-1.0.1/featuremap/plot.py
--rw-r--r--   0 uqyyao4    (503) staff       (20)     2460 2024-05-29 05:12:06.000000 featuremap-learn-1.0.1/featuremap/validation.py
-drwxr-xr-x   0 uqyyao4    (503) staff       (20)        0 2024-05-30 03:44:34.109769 featuremap-learn-1.0.1/featuremap_learn.egg-info/
--rw-r--r--   0 uqyyao4    (503) staff       (20)     5169 2024-05-30 03:44:33.000000 featuremap-learn-1.0.1/featuremap_learn.egg-info/PKG-INFO
--rwx------   0 uqyyao4    (503) staff       (20)      399 2024-05-30 03:44:33.000000 featuremap-learn-1.0.1/featuremap_learn.egg-info/SOURCES.txt
--rwx------   0 uqyyao4    (503) staff       (20)        1 2024-05-30 03:44:33.000000 featuremap-learn-1.0.1/featuremap_learn.egg-info/dependency_links.txt
--rwx------   0 uqyyao4    (503) staff       (20)      123 2024-05-30 03:44:33.000000 featuremap-learn-1.0.1/featuremap_learn.egg-info/requires.txt
--rwx------   0 uqyyao4    (503) staff       (20)       11 2024-05-30 03:44:33.000000 featuremap-learn-1.0.1/featuremap_learn.egg-info/top_level.txt
--rw-r--r--   0 uqyyao4    (503) staff       (20)       38 2024-05-30 03:44:34.113842 featuremap-learn-1.0.1/setup.cfg
--rw-r--r--   0 uqyyao4    (503) staff       (20)     1763 2024-05-30 03:44:27.000000 featuremap-learn-1.0.1/setup.py
+drwxr-xr-x   0 uqyyao4    (503) staff       (20)        0 2024-06-03 00:44:40.634018 featuremap-learn-1.0.2/
+-rw-r--r--   0 uqyyao4    (503) staff       (20)     1496 2024-05-31 01:01:19.000000 featuremap-learn-1.0.2/LICENSE
+-rw-r--r--   0 uqyyao4    (503) staff       (20)     5732 2024-06-03 00:44:40.633247 featuremap-learn-1.0.2/PKG-INFO
+-rw-r--r--   0 uqyyao4    (503) staff       (20)     4116 2024-05-31 01:01:19.000000 featuremap-learn-1.0.2/README.md
+drwxr-xr-x   0 uqyyao4    (503) staff       (20)        0 2024-06-03 00:44:40.627714 featuremap-learn-1.0.2/featuremap/
+-rw-r--r--   0 uqyyao4    (503) staff       (20)      341 2024-05-31 01:01:19.000000 featuremap-learn-1.0.2/featuremap/__init__.py
+-rw-r--r--   0 uqyyao4    (503) staff       (20)    23586 2024-05-31 01:01:19.000000 featuremap-learn-1.0.2/featuremap/core_transition_state.py
+-rw-r--r--   0 uqyyao4    (503) staff       (20)    97070 2024-05-31 01:01:19.000000 featuremap-learn-1.0.2/featuremap/featuremap_.py
+-rw-r--r--   0 uqyyao4    (503) staff       (20)    38661 2024-05-31 01:01:19.000000 featuremap-learn-1.0.2/featuremap/features.py
+-rw-r--r--   0 uqyyao4    (503) staff       (20)    28803 2024-05-31 01:01:19.000000 featuremap-learn-1.0.2/featuremap/layouts.py
+-rw-r--r--   0 uqyyao4    (503) staff       (20)     1226 2024-05-31 01:01:19.000000 featuremap-learn-1.0.2/featuremap/plot.py
+-rw-r--r--   0 uqyyao4    (503) staff       (20)     2460 2024-05-31 01:01:19.000000 featuremap-learn-1.0.2/featuremap/validation.py
+drwxr-xr-x   0 uqyyao4    (503) staff       (20)        0 2024-06-03 00:44:40.630673 featuremap-learn-1.0.2/featuremap_learn.egg-info/
+-rw-r--r--   0 uqyyao4    (503) staff       (20)     5732 2024-06-03 00:44:40.000000 featuremap-learn-1.0.2/featuremap_learn.egg-info/PKG-INFO
+-rw-r--r--   0 uqyyao4    (503) staff       (20)      399 2024-06-03 00:44:40.000000 featuremap-learn-1.0.2/featuremap_learn.egg-info/SOURCES.txt
+-rw-r--r--   0 uqyyao4    (503) staff       (20)        1 2024-06-03 00:44:40.000000 featuremap-learn-1.0.2/featuremap_learn.egg-info/dependency_links.txt
+-rw-r--r--   0 uqyyao4    (503) staff       (20)      225 2024-06-03 00:44:40.000000 featuremap-learn-1.0.2/featuremap_learn.egg-info/requires.txt
+-rw-r--r--   0 uqyyao4    (503) staff       (20)       11 2024-06-03 00:44:40.000000 featuremap-learn-1.0.2/featuremap_learn.egg-info/top_level.txt
+-rw-r--r--   0 uqyyao4    (503) staff       (20)       38 2024-06-03 00:44:40.634205 featuremap-learn-1.0.2/setup.cfg
+-rw-r--r--   0 uqyyao4    (503) staff       (20)     2050 2024-06-03 00:44:37.000000 featuremap-learn-1.0.2/setup.py
```

### Comparing `featuremap-learn-1.0.1/LICENSE` & `featuremap-learn-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `featuremap-learn-1.0.1/PKG-INFO` & `featuremap-learn-1.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featuremap-learn
-Version: 1.0.1
+Version: 1.0.2
 Summary: FeatureMAP
 Home-page: https://github.com/YYT1002/FeatureMAP
 Maintainer: Yang Yang
 Maintainer-email: yangyangnwpu@gmail.com
 License: GPL
 Keywords: dimensionality reduction,manifold learning,tangent space embedding
 Classifier: Intended Audience :: Science/Research
@@ -23,45 +23,54 @@
 License-File: LICENSE
 Requires-Dist: numpy>=1.13
 Requires-Dist: scikit-learn>=0.16
 Requires-Dist: scipy>=0.19
 Requires-Dist: numba>=0.55.0
 Requires-Dist: umap-learn>=0.5.1
 Provides-Extra: plot
-Requires-Dist: scanpy; extra == "plot"
 Requires-Dist: pandas; extra == "plot"
-Requires-Dist: anndata; extra == "plot"
 Requires-Dist: matplotlib>=3.5.1; extra == "plot"
+Provides-Extra: features
+Requires-Dist: scanpy; extra == "features"
+Requires-Dist: pandas; extra == "features"
+Requires-Dist: anndata; extra == "features"
+Requires-Dist: matplotlib>=3.5.1; extra == "features"
+Provides-Extra: core-transition-state
+Requires-Dist: scanpy; extra == "core-transition-state"
+Requires-Dist: pandas; extra == "core-transition-state"
+Requires-Dist: anndata; extra == "core-transition-state"
+Requires-Dist: matplotlib>=3.5.1; extra == "core-transition-state"
 
 ![FeatureMAP Illustration](./figures/featureMAP.png)
 
 # FeatureMAP: Feature-preserving Manifold Approximation and Projection
 
 Visualizing single-cell data is crucial for understanding cellular heterogeneity and dynamics. Traditional methods like UMAP and t-SNE are effective for clustering but often miss critical gene information. FeatureMAP innovatively combines UMAP and PCA concepts to preserve both clustering structures and gene feature variations within a low-dimensional space.
-Z
+
 ## Description
 
 FeatureMAP introduces a novel approach by enhancing manifold learning with pairwise tangent space embedding, aiming to retain crucial aspects of cellular data.
-We introduce two visualization by FeatureMAP: expression (GEX) and variation (GVA) embedding.
-Here is an example over one synthetic dataset ([BEELINE](https://github.com/Murali-group/Beeline)) with bifurcation model. Compared with UMAP, FeatureMAP-GEX better preserves density (similar to densMAP), and FeatureMAP-GVA shows trajectories.
+We introduce two visualization plots by FeatureMAP: expression (GEX) and variation (GVA) embedding.
+Here is an example over one synthetic dataset ([BEELINE](https://github.com/Murali-group/Beeline)) with a bifurcation model. Compared with UMAP, FeatureMAP-GEX better preserves density, and FeatureMAP-GVA shows trajectories.
 ![Bifurcation Embedding](./figures/bifurcation_embedding.png)
 
-Besides the 2-dimensional visualization, FeatureMAP presents three core concepts:
+Besides the two-dimensional visualization, FeatureMAP presents three core concepts:
+
 1. **Gene Contribution**: Estimating and projecting gene feature loadings. The arrow represents the direction and magnitude of one gene's change. 
     ![Gene Contribution](./figures/gene_contribution.png)
 
 2. **Gene Variation Trajectory**: Tracking the cell differentiation across states. There are clear paths (transition states) connecting cell states (core states) in a knot-and-thread way.
     ![Gene Variation Trajectory](./figures/gene_variation_trajectory.png)
     [View 3D Plot](https://YYT1002.github.io/FeatureMAP/figures/3d_plot.html)
    
 3. **Core and Transition States**: Defined computationally through cell density and cell variation properties. Core states are cells with higher cell density and smaller cell variation, while transition states are lower cell density and larger cell variation.
     ![Core and Transition States](./figures/core_trans_states.png)
    
 
-These enhancements allow for differential gene variation analysis, highlighting key regulatory genes that drive transitions between cellular states. Tested on both synthetic and real single-cell RNA sequencing (scRNA-seq) data, including studies on pancreatic development and T-cell exhaustion, FeatureMAP provides a more detailed understanding of cellular trajectories and regulatory mechanisms.
+These enhancements allow for differential gene variation (DGV) analysis, highlighting key regulatory genes that drive transitions between cellular states. Tested on both synthetic and real single-cell RNA sequencing (scRNA-seq) data, including studies on pancreatic development and T-cell exhaustion (Tutorials in ??), FeatureMAP provides a more detailed understanding of cellular trajectories and regulatory mechanisms.
 
 
 ## Getting Started
 
 ### Dependencies
 
 - Python 3.8 or higher
@@ -74,52 +83,48 @@
 
 ```bash
 pip install featuremap-learn
 ```
 
 ### 2. Installation via Conda
 For users who prefer using Conda, especially for managing complex dependencies and environments in scientific computing.
+```
+conda install ???
+```
 
 ## How to use FeatureMAP
 
 ### Data Visualization
-For data visualization, FeatureMAP introduces expression embedding and variation embedding:
+For data visualization, FeatureMAP introduces expression embedding and variation embedding. Here is one example by MNIST datasets.
 ```
 import featuremap
 from sklearn.datasets import fetch_openml
 from sklearn.utils import resample
 
 digits = fetch_openml(name='mnist_784')
 subsample, subsample_labels = resample(digits.data, digits.target, n_samples=7000, stratify=digits.target, random_state=1)
 
 x_emb = featuremap.featureMAP().fit_transform(subsample)
 v_emb = featuremap.featureMAP(output_variation=True).fit_transform(subsample)
 
 ```
 
 #### Parameters:
-output_variation: bool (False by default). Decide to generate expression embedding or variation embedding.
+output_variation: bool (False by default). Decide to generate expression embedding or variation embedding. 
 
 #### Outputs
 x_emb: expession embedding to show the clustering
 
 v_emb: variation embedding to show the trajectory
 
-The tutorial is ??????
-
-## Example data and plots
-
 
 ## Documentation
+More tutorials are at https://featuremap.readthedocs.io/en/latest/index.html.
 
 ## Citation
-Our FeatureMAP alogrithm is 
+Our FeatureMAP alogrithm is based on the paper
 
+Yang, Yang, et al. "Interpretable Dimensionality Reduction by Feature Preserving Manifold Approximation and Projection." arXiv preprint arXiv:2211.09321 (2022).
 
 ## License
 The FeatureMAP package is under BSD-3-Clause license.
 
-## Contact
-
-### Acknowledgments
-Thanks to the researchers and developers who provided insights and code snippets, including:
-
```

### Comparing `featuremap-learn-1.0.1/README.md` & `featuremap-learn-1.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 ![FeatureMAP Illustration](./figures/featureMAP.png)
 
 # FeatureMAP: Feature-preserving Manifold Approximation and Projection
 
 Visualizing single-cell data is crucial for understanding cellular heterogeneity and dynamics. Traditional methods like UMAP and t-SNE are effective for clustering but often miss critical gene information. FeatureMAP innovatively combines UMAP and PCA concepts to preserve both clustering structures and gene feature variations within a low-dimensional space.
-Z
+
 ## Description
 
 FeatureMAP introduces a novel approach by enhancing manifold learning with pairwise tangent space embedding, aiming to retain crucial aspects of cellular data.
-We introduce two visualization by FeatureMAP: expression (GEX) and variation (GVA) embedding.
-Here is an example over one synthetic dataset ([BEELINE](https://github.com/Murali-group/Beeline)) with bifurcation model. Compared with UMAP, FeatureMAP-GEX better preserves density (similar to densMAP), and FeatureMAP-GVA shows trajectories.
+We introduce two visualization plots by FeatureMAP: expression (GEX) and variation (GVA) embedding.
+Here is an example over one synthetic dataset ([BEELINE](https://github.com/Murali-group/Beeline)) with a bifurcation model. Compared with UMAP, FeatureMAP-GEX better preserves density, and FeatureMAP-GVA shows trajectories.
 ![Bifurcation Embedding](./figures/bifurcation_embedding.png)
 
-Besides the 2-dimensional visualization, FeatureMAP presents three core concepts:
+Besides the two-dimensional visualization, FeatureMAP presents three core concepts:
+
 1. **Gene Contribution**: Estimating and projecting gene feature loadings. The arrow represents the direction and magnitude of one gene's change. 
     ![Gene Contribution](./figures/gene_contribution.png)
 
 2. **Gene Variation Trajectory**: Tracking the cell differentiation across states. There are clear paths (transition states) connecting cell states (core states) in a knot-and-thread way.
     ![Gene Variation Trajectory](./figures/gene_variation_trajectory.png)
     [View 3D Plot](https://YYT1002.github.io/FeatureMAP/figures/3d_plot.html)
    
 3. **Core and Transition States**: Defined computationally through cell density and cell variation properties. Core states are cells with higher cell density and smaller cell variation, while transition states are lower cell density and larger cell variation.
     ![Core and Transition States](./figures/core_trans_states.png)
    
 
-These enhancements allow for differential gene variation analysis, highlighting key regulatory genes that drive transitions between cellular states. Tested on both synthetic and real single-cell RNA sequencing (scRNA-seq) data, including studies on pancreatic development and T-cell exhaustion, FeatureMAP provides a more detailed understanding of cellular trajectories and regulatory mechanisms.
+These enhancements allow for differential gene variation (DGV) analysis, highlighting key regulatory genes that drive transitions between cellular states. Tested on both synthetic and real single-cell RNA sequencing (scRNA-seq) data, including studies on pancreatic development and T-cell exhaustion (Tutorials in ??), FeatureMAP provides a more detailed understanding of cellular trajectories and regulatory mechanisms.
 
 
 ## Getting Started
 
 ### Dependencies
 
 - Python 3.8 or higher
@@ -40,52 +41,48 @@
 
 ```bash
 pip install featuremap-learn
 ```
 
 ### 2. Installation via Conda
 For users who prefer using Conda, especially for managing complex dependencies and environments in scientific computing.
+```
+conda install ???
+```
 
 ## How to use FeatureMAP
 
 ### Data Visualization
-For data visualization, FeatureMAP introduces expression embedding and variation embedding:
+For data visualization, FeatureMAP introduces expression embedding and variation embedding. Here is one example by MNIST datasets.
 ```
 import featuremap
 from sklearn.datasets import fetch_openml
 from sklearn.utils import resample
 
 digits = fetch_openml(name='mnist_784')
 subsample, subsample_labels = resample(digits.data, digits.target, n_samples=7000, stratify=digits.target, random_state=1)
 
 x_emb = featuremap.featureMAP().fit_transform(subsample)
 v_emb = featuremap.featureMAP(output_variation=True).fit_transform(subsample)
 
 ```
 
 #### Parameters:
-output_variation: bool (False by default). Decide to generate expression embedding or variation embedding.
+output_variation: bool (False by default). Decide to generate expression embedding or variation embedding. 
 
 #### Outputs
 x_emb: expession embedding to show the clustering
 
 v_emb: variation embedding to show the trajectory
 
-The tutorial is ??????
-
-## Example data and plots
-
 
 ## Documentation
+More tutorials are at https://featuremap.readthedocs.io/en/latest/index.html.
 
 ## Citation
-Our FeatureMAP alogrithm is 
+Our FeatureMAP alogrithm is based on the paper
 
+Yang, Yang, et al. "Interpretable Dimensionality Reduction by Feature Preserving Manifold Approximation and Projection." arXiv preprint arXiv:2211.09321 (2022).
 
 ## License
 The FeatureMAP package is under BSD-3-Clause license.
 
-## Contact
-
-### Acknowledgments
-Thanks to the researchers and developers who provided insights and code snippets, including:
-
```

### Comparing `featuremap-learn-1.0.1/featuremap/core_transition_state.py` & `featuremap-learn-1.0.2/featuremap/core_transition_state.py`

 * *Files identical despite different names*

### Comparing `featuremap-learn-1.0.1/featuremap/featuremap_.py` & `featuremap-learn-1.0.2/featuremap/featuremap_.py`

 * *Files identical despite different names*

### Comparing `featuremap-learn-1.0.1/featuremap/features.py` & `featuremap-learn-1.0.2/featuremap/features.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,19 +137,14 @@
         smooth=0.5,
         n_neighbors=None,
         min_mass=1,
         autoscale=True,
         ):
     # Set grid as the support
     X_emb=adata.obsm[embedding]  # Exclude one leiden cluster;
-    # rotational_matrix = adata.uns['emb_umap']._densmap_kwds['VH_embedding']
-    # rotational_matrix = adata.obsm['VH_embedding']
-    # r_emb = adata.obsm['rad_emb_no_log']
-    # s = Scms(X_emb, 0.5, min_radius=5)
-
     # X_emb=adata.obsm[embedding]
     V_emb=adata.obsm[vkey] 
     idx_valid = np.isfinite(X_emb.sum(1) + V_emb.sum(1))
     X_emb = X_emb[idx_valid]
     V_emb = V_emb[idx_valid]
 
     # prepare grid
@@ -223,19 +218,14 @@
         smooth=0.5,
         n_neighbors=None,
         min_mass=1,
         autoscale=True,
         ):
     # Set grid as the support
     X_emb=adata.obsm[embedding]  # Exclude one leiden cluster;
-    # rotational_matrix = adata.uns['emb_umap']._densmap_kwds['VH_embedding']
-    # rotational_matrix = adata.obsm['VH_embedding']
-    # r_emb = adata.obsm['rad_emb_no_log']
-    # s = Scms(X_emb, 0.5, min_radius=5)
-
     # X_emb=adata.obsm[embedding]
     vkey='gauge_v1_emb'
     V_emb=adata.obsm[vkey] 
     idx_valid = np.isfinite(X_emb.sum(1) + V_emb.sum(1))
     X_emb = X_emb[idx_valid]
     V_emb = V_emb[idx_valid]
 
@@ -601,18 +591,14 @@
     vkey=f'feature_{feature}_loading'
 
     feature_id = np.where(adata.var_names == feature)[0][0]
     adata.obsm[vkey] = adata.obsm[feature_loading_emb][:,:,feature_id]
 
     # Set grid as the support
     X_emb=adata.obsm[embedding]
-    # rotational_matrix = adata.uns['emb_umap']._densmap_kwds['VH_embedding']
-    # rotational_matrix = adata.obsm['VH_embedding']
-    # r_emb = adata.obsm['rad_emb_no_log']
-    # s = Scms(X_emb, 0.5, min_radius=5)
     
     V_emb=adata.obsm[vkey] 
     idx_valid = np.isfinite(X_emb.sum(1) + V_emb.sum(1))
     X_emb = X_emb[idx_valid]
     V_emb = V_emb[idx_valid]
 
     # prepare grid
@@ -807,19 +793,14 @@
     vkey=f'feature_{feature}_loading'
 
     feature_id = np.where(adata.var_names == feature)[0][0]
     # adata.obsm[vkey] = adata.obsm[feature_loading_emb][:,:,feature_id]
 
     # Set grid as the support
     X_emb=adata.obsm[embedding]
-    # rotational_matrix = adata.uns['emb_umap']._densmap_kwds['VH_embedding']
-    # rotational_matrix = adata.obsm['VH_embedding']
-    # r_emb = adata.obsm['rad_emb_no_log']
-    # s = Scms(X_emb, 0.5, min_radius=5)
-    
     V_emb=adata.obsm[vkey] 
     idx_valid = np.isfinite(X_emb.sum(1) + V_emb.sum(1))
     X_emb = X_emb[idx_valid]
     V_emb = V_emb[idx_valid]
 
     # prepare grid
     n_obs, n_dim = X_emb.shape
```

### Comparing `featuremap-learn-1.0.1/featuremap/layouts.py` & `featuremap-learn-1.0.2/featuremap/layouts.py`

 * *Files identical despite different names*

### Comparing `featuremap-learn-1.0.1/featuremap/plot.py` & `featuremap-learn-1.0.2/featuremap/plot.py`

 * *Files identical despite different names*

### Comparing `featuremap-learn-1.0.1/featuremap/validation.py` & `featuremap-learn-1.0.2/featuremap/validation.py`

 * *Files identical despite different names*

### Comparing `featuremap-learn-1.0.1/featuremap_learn.egg-info/PKG-INFO` & `featuremap-learn-1.0.2/featuremap_learn.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featuremap-learn
-Version: 1.0.1
+Version: 1.0.2
 Summary: FeatureMAP
 Home-page: https://github.com/YYT1002/FeatureMAP
 Maintainer: Yang Yang
 Maintainer-email: yangyangnwpu@gmail.com
 License: GPL
 Keywords: dimensionality reduction,manifold learning,tangent space embedding
 Classifier: Intended Audience :: Science/Research
@@ -23,45 +23,54 @@
 License-File: LICENSE
 Requires-Dist: numpy>=1.13
 Requires-Dist: scikit-learn>=0.16
 Requires-Dist: scipy>=0.19
 Requires-Dist: numba>=0.55.0
 Requires-Dist: umap-learn>=0.5.1
 Provides-Extra: plot
-Requires-Dist: scanpy; extra == "plot"
 Requires-Dist: pandas; extra == "plot"
-Requires-Dist: anndata; extra == "plot"
 Requires-Dist: matplotlib>=3.5.1; extra == "plot"
+Provides-Extra: features
+Requires-Dist: scanpy; extra == "features"
+Requires-Dist: pandas; extra == "features"
+Requires-Dist: anndata; extra == "features"
+Requires-Dist: matplotlib>=3.5.1; extra == "features"
+Provides-Extra: core-transition-state
+Requires-Dist: scanpy; extra == "core-transition-state"
+Requires-Dist: pandas; extra == "core-transition-state"
+Requires-Dist: anndata; extra == "core-transition-state"
+Requires-Dist: matplotlib>=3.5.1; extra == "core-transition-state"
 
 ![FeatureMAP Illustration](./figures/featureMAP.png)
 
 # FeatureMAP: Feature-preserving Manifold Approximation and Projection
 
 Visualizing single-cell data is crucial for understanding cellular heterogeneity and dynamics. Traditional methods like UMAP and t-SNE are effective for clustering but often miss critical gene information. FeatureMAP innovatively combines UMAP and PCA concepts to preserve both clustering structures and gene feature variations within a low-dimensional space.
-Z
+
 ## Description
 
 FeatureMAP introduces a novel approach by enhancing manifold learning with pairwise tangent space embedding, aiming to retain crucial aspects of cellular data.
-We introduce two visualization by FeatureMAP: expression (GEX) and variation (GVA) embedding.
-Here is an example over one synthetic dataset ([BEELINE](https://github.com/Murali-group/Beeline)) with bifurcation model. Compared with UMAP, FeatureMAP-GEX better preserves density (similar to densMAP), and FeatureMAP-GVA shows trajectories.
+We introduce two visualization plots by FeatureMAP: expression (GEX) and variation (GVA) embedding.
+Here is an example over one synthetic dataset ([BEELINE](https://github.com/Murali-group/Beeline)) with a bifurcation model. Compared with UMAP, FeatureMAP-GEX better preserves density, and FeatureMAP-GVA shows trajectories.
 ![Bifurcation Embedding](./figures/bifurcation_embedding.png)
 
-Besides the 2-dimensional visualization, FeatureMAP presents three core concepts:
+Besides the two-dimensional visualization, FeatureMAP presents three core concepts:
+
 1. **Gene Contribution**: Estimating and projecting gene feature loadings. The arrow represents the direction and magnitude of one gene's change. 
     ![Gene Contribution](./figures/gene_contribution.png)
 
 2. **Gene Variation Trajectory**: Tracking the cell differentiation across states. There are clear paths (transition states) connecting cell states (core states) in a knot-and-thread way.
     ![Gene Variation Trajectory](./figures/gene_variation_trajectory.png)
     [View 3D Plot](https://YYT1002.github.io/FeatureMAP/figures/3d_plot.html)
    
 3. **Core and Transition States**: Defined computationally through cell density and cell variation properties. Core states are cells with higher cell density and smaller cell variation, while transition states are lower cell density and larger cell variation.
     ![Core and Transition States](./figures/core_trans_states.png)
    
 
-These enhancements allow for differential gene variation analysis, highlighting key regulatory genes that drive transitions between cellular states. Tested on both synthetic and real single-cell RNA sequencing (scRNA-seq) data, including studies on pancreatic development and T-cell exhaustion, FeatureMAP provides a more detailed understanding of cellular trajectories and regulatory mechanisms.
+These enhancements allow for differential gene variation (DGV) analysis, highlighting key regulatory genes that drive transitions between cellular states. Tested on both synthetic and real single-cell RNA sequencing (scRNA-seq) data, including studies on pancreatic development and T-cell exhaustion (Tutorials in ??), FeatureMAP provides a more detailed understanding of cellular trajectories and regulatory mechanisms.
 
 
 ## Getting Started
 
 ### Dependencies
 
 - Python 3.8 or higher
@@ -74,52 +83,48 @@
 
 ```bash
 pip install featuremap-learn
 ```
 
 ### 2. Installation via Conda
 For users who prefer using Conda, especially for managing complex dependencies and environments in scientific computing.
+```
+conda install ???
+```
 
 ## How to use FeatureMAP
 
 ### Data Visualization
-For data visualization, FeatureMAP introduces expression embedding and variation embedding:
+For data visualization, FeatureMAP introduces expression embedding and variation embedding. Here is one example by MNIST datasets.
 ```
 import featuremap
 from sklearn.datasets import fetch_openml
 from sklearn.utils import resample
 
 digits = fetch_openml(name='mnist_784')
 subsample, subsample_labels = resample(digits.data, digits.target, n_samples=7000, stratify=digits.target, random_state=1)
 
 x_emb = featuremap.featureMAP().fit_transform(subsample)
 v_emb = featuremap.featureMAP(output_variation=True).fit_transform(subsample)
 
 ```
 
 #### Parameters:
-output_variation: bool (False by default). Decide to generate expression embedding or variation embedding.
+output_variation: bool (False by default). Decide to generate expression embedding or variation embedding. 
 
 #### Outputs
 x_emb: expession embedding to show the clustering
 
 v_emb: variation embedding to show the trajectory
 
-The tutorial is ??????
-
-## Example data and plots
-
 
 ## Documentation
+More tutorials are at https://featuremap.readthedocs.io/en/latest/index.html.
 
 ## Citation
-Our FeatureMAP alogrithm is 
+Our FeatureMAP alogrithm is based on the paper
 
+Yang, Yang, et al. "Interpretable Dimensionality Reduction by Feature Preserving Manifold Approximation and Projection." arXiv preprint arXiv:2211.09321 (2022).
 
 ## License
 The FeatureMAP package is under BSD-3-Clause license.
 
-## Contact
-
-### Acknowledgments
-Thanks to the researchers and developers who provided insights and code snippets, including:
-
```

### Comparing `featuremap-learn-1.0.1/setup.py` & `featuremap-learn-1.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #        return readme_file.read()
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 configuration = {
     'name' : 'featuremap-learn',
-    'version': '1.0.1',
+    'version': '1.0.2',
     'description' : 'FeatureMAP',
     'long_description' : long_description,
     'long_description_content_type' : "text/markdown",
     'classifiers' : [
         'Intended Audience :: Science/Research',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: BSD License',
@@ -44,14 +44,26 @@
                          'scikit-learn >= 0.16',
                           'scipy >= 0.19',
                          'numba >= 0.55.0',
                          'umap-learn >= 0.5.1',
                          ],
     "extras_require": {
         "plot": [
+            # "scanpy",
+            "pandas",
+            # "anndata",
+            "matplotlib >= 3.5.1"
+        ],
+         "features": [
+            "scanpy",
+            "pandas",
+            "anndata",
+            "matplotlib >= 3.5.1"
+        ],
+         "core_transition_state": [
             "scanpy",
             "pandas",
             "anndata",
             "matplotlib >= 3.5.1"
         ],
     
     }
```

