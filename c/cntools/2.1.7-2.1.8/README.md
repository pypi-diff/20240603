# Comparing `tmp/cntools-2.1.7.tar.gz` & `tmp/cntools-2.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cntools-2.1.7.tar", last modified: Thu May 16 20:11:17 2024, max compression
+gzip compressed data, was "cntools-2.1.8.tar", last modified: Mon Jun  3 07:36:27 2024, max compression
```

## Comparing `cntools-2.1.7.tar` & `cntools-2.1.8.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 yichengtao   (501) staff       (20)        0 2024-05-16 20:11:17.514279 cntools-2.1.7/
--rw-r--r--   0 yichengtao   (501) staff       (20)     1063 2024-05-08 03:17:12.000000 cntools-2.1.7/LICENSE
--rw-r--r--   0 yichengtao   (501) staff       (20)       44 2024-05-08 03:17:12.000000 cntools-2.1.7/MANIFEST.in
--rw-r--r--   0 yichengtao   (501) staff       (20)     5930 2024-05-16 20:11:17.513740 cntools-2.1.7/PKG-INFO
--rw-r--r--   0 yichengtao   (501) staff       (20)     3374 2024-05-08 03:17:12.000000 cntools-2.1.7/README.md
-drwxr-xr-x   0 yichengtao   (501) staff       (20)        0 2024-05-16 20:11:17.505424 cntools-2.1.7/cntools/
--rw-r--r--   0 yichengtao   (501) staff       (20)        0 2024-05-08 03:17:12.000000 cntools-2.1.7/cntools/__init__.py
-drwxr-xr-x   0 yichengtao   (501) staff       (20)        0 2024-05-16 20:11:17.507364 cntools-2.1.7/cntools/datasets/
--rw-r--r--   0 yichengtao   (501) staff       (20)      285 2024-05-14 23:20:55.000000 cntools-2.1.7/cntools/datasets/__init__.py
--rw-r--r--   0 yichengtao   (501) staff       (20)     3666 2024-05-15 02:31:09.000000 cntools-2.1.7/cntools/datasets/make_ds.py
--rw-r--r--   0 yichengtao   (501) staff       (20)     4178 2024-05-15 22:41:48.000000 cntools-2.1.7/cntools/datasets/prep.py
-drwxr-xr-x   0 yichengtao   (501) staff       (20)        0 2024-05-16 20:11:17.509084 cntools-2.1.7/cntools/identification/
--rw-r--r--   0 yichengtao   (501) staff       (20)     1921 2024-05-08 03:17:12.000000 cntools-2.1.7/cntools/identification/CC.py
--rw-r--r--   0 yichengtao   (501) staff       (20)     4938 2024-05-08 03:17:12.000000 cntools-2.1.7/cntools/identification/CFIDF.py
--rw-r--r--   0 yichengtao   (501) staff       (20)     3348 2024-05-16 20:10:43.000000 cntools-2.1.7/cntools/identification/CNE.py
--rw-r--r--   0 yichengtao   (501) staff       (20)     3884 2024-05-08 03:17:12.000000 cntools-2.1.7/cntools/identification/Spatial_LDA.py
--rw-r--r--   0 yichengtao   (501) staff       (20)      151 2024-05-08 03:17:12.000000 cntools-2.1.7/cntools/identification/__init__.py
--rw-r--r--   0 yichengtao   (501) staff       (20)      498 2024-05-08 03:17:12.000000 cntools-2.1.7/cntools/identification/base.py
-drwxr-xr-x   0 yichengtao   (501) staff       (20)        0 2024-05-16 20:11:17.510173 cntools-2.1.7/cntools/smoothing/
--rw-r--r--   0 yichengtao   (501) staff       (20)     5500 2024-05-08 03:17:12.000000 cntools-2.1.7/cntools/smoothing/HMRF.py
--rw-r--r--   0 yichengtao   (501) staff       (20)     3841 2024-05-08 03:17:12.000000 cntools-2.1.7/cntools/smoothing/NaiveSmooth.py
--rw-r--r--   0 yichengtao   (501) staff       (20)       95 2024-05-08 03:17:12.000000 cntools-2.1.7/cntools/smoothing/__init__.py
--rw-r--r--   0 yichengtao   (501) staff       (20)      392 2024-05-08 03:17:12.000000 cntools-2.1.7/cntools/smoothing/base.py
-drwxr-xr-x   0 yichengtao   (501) staff       (20)        0 2024-05-16 20:11:17.512896 cntools-2.1.7/cntools/utils/
--rw-r--r--   0 yichengtao   (501) staff       (20)      135 2024-05-08 03:17:12.000000 cntools-2.1.7/cntools/utils/__init__.py
--rw-r--r--   0 yichengtao   (501) staff       (20)  1156429 2024-05-16 20:11:16.000000 cntools-2.1.7/cntools/utils/_k_means_lloyd_reg.c
--rw-r--r--   0 yichengtao   (501) staff       (20)    10741 2024-05-08 03:17:12.000000 cntools-2.1.7/cntools/utils/_k_means_lloyd_reg.pyx
--rw-r--r--   0 yichengtao   (501) staff       (20)     6889 2024-05-08 03:17:12.000000 cntools-2.1.7/cntools/utils/kmeans_reg.py
--rw-r--r--   0 yichengtao   (501) staff       (20)     1745 2024-05-08 03:17:12.000000 cntools-2.1.7/cntools/utils/utils.py
-drwxr-xr-x   0 yichengtao   (501) staff       (20)        0 2024-05-16 20:11:17.513216 cntools-2.1.7/cntools.egg-info/
--rw-r--r--   0 yichengtao   (501) staff       (20)     5930 2024-05-16 20:11:17.000000 cntools-2.1.7/cntools.egg-info/PKG-INFO
--rw-r--r--   0 yichengtao   (501) staff       (20)      768 2024-05-16 20:11:17.000000 cntools-2.1.7/cntools.egg-info/SOURCES.txt
--rw-r--r--   0 yichengtao   (501) staff       (20)        1 2024-05-16 20:11:17.000000 cntools-2.1.7/cntools.egg-info/dependency_links.txt
--rw-r--r--   0 yichengtao   (501) staff       (20)      285 2024-05-16 20:11:17.000000 cntools-2.1.7/cntools.egg-info/requires.txt
--rw-r--r--   0 yichengtao   (501) staff       (20)       27 2024-05-16 20:11:17.000000 cntools-2.1.7/cntools.egg-info/top_level.txt
--rw-r--r--   0 yichengtao   (501) staff       (20)     1376 2024-05-16 20:10:51.000000 cntools-2.1.7/pyproject.toml
--rw-r--r--   0 yichengtao   (501) staff       (20)       38 2024-05-16 20:11:17.514553 cntools-2.1.7/setup.cfg
--rw-r--r--   0 yichengtao   (501) staff       (20)      239 2024-05-08 03:17:12.000000 cntools-2.1.7/setup.py
+drwxr-xr-x   0 yichengtao   (501) staff       (20)        0 2024-06-03 07:36:27.885227 cntools-2.1.8/
+-rw-r--r--   0 yichengtao   (501) staff       (20)     1063 2024-05-08 03:17:12.000000 cntools-2.1.8/LICENSE
+-rw-r--r--   0 yichengtao   (501) staff       (20)       44 2024-05-08 03:17:12.000000 cntools-2.1.8/MANIFEST.in
+-rw-r--r--   0 yichengtao   (501) staff       (20)     5827 2024-06-03 07:36:27.884899 cntools-2.1.8/PKG-INFO
+-rw-r--r--   0 yichengtao   (501) staff       (20)     3271 2024-06-03 07:30:42.000000 cntools-2.1.8/README.md
+drwxr-xr-x   0 yichengtao   (501) staff       (20)        0 2024-06-03 07:36:27.870302 cntools-2.1.8/cntools/
+-rw-r--r--   0 yichengtao   (501) staff       (20)        0 2024-05-08 03:17:12.000000 cntools-2.1.8/cntools/__init__.py
+drwxr-xr-x   0 yichengtao   (501) staff       (20)        0 2024-06-03 07:36:27.875094 cntools-2.1.8/cntools/datasets/
+-rw-r--r--   0 yichengtao   (501) staff       (20)      285 2024-05-14 23:20:55.000000 cntools-2.1.8/cntools/datasets/__init__.py
+-rw-r--r--   0 yichengtao   (501) staff       (20)     3666 2024-05-15 02:31:09.000000 cntools-2.1.8/cntools/datasets/make_ds.py
+-rw-r--r--   0 yichengtao   (501) staff       (20)     4178 2024-05-15 22:41:48.000000 cntools-2.1.8/cntools/datasets/prep.py
+drwxr-xr-x   0 yichengtao   (501) staff       (20)        0 2024-06-03 07:36:27.877285 cntools-2.1.8/cntools/identification/
+-rw-r--r--   0 yichengtao   (501) staff       (20)     1926 2024-06-03 07:33:57.000000 cntools-2.1.8/cntools/identification/CC.py
+-rw-r--r--   0 yichengtao   (501) staff       (20)     4943 2024-06-03 07:34:04.000000 cntools-2.1.8/cntools/identification/CFIDF.py
+-rw-r--r--   0 yichengtao   (501) staff       (20)     3353 2024-06-03 07:34:10.000000 cntools-2.1.8/cntools/identification/CNE.py
+-rw-r--r--   0 yichengtao   (501) staff       (20)     3889 2024-06-03 07:34:16.000000 cntools-2.1.8/cntools/identification/Spatial_LDA.py
+-rw-r--r--   0 yichengtao   (501) staff       (20)      151 2024-05-08 03:17:12.000000 cntools-2.1.8/cntools/identification/__init__.py
+-rw-r--r--   0 yichengtao   (501) staff       (20)      498 2024-05-08 03:17:12.000000 cntools-2.1.8/cntools/identification/base.py
+drwxr-xr-x   0 yichengtao   (501) staff       (20)        0 2024-06-03 07:36:27.878429 cntools-2.1.8/cntools/smoothing/
+-rw-r--r--   0 yichengtao   (501) staff       (20)     5500 2024-05-08 03:17:12.000000 cntools-2.1.8/cntools/smoothing/HMRF.py
+-rw-r--r--   0 yichengtao   (501) staff       (20)     3841 2024-05-08 03:17:12.000000 cntools-2.1.8/cntools/smoothing/NaiveSmooth.py
+-rw-r--r--   0 yichengtao   (501) staff       (20)       95 2024-05-08 03:17:12.000000 cntools-2.1.8/cntools/smoothing/__init__.py
+-rw-r--r--   0 yichengtao   (501) staff       (20)      392 2024-05-08 03:17:12.000000 cntools-2.1.8/cntools/smoothing/base.py
+drwxr-xr-x   0 yichengtao   (501) staff       (20)        0 2024-06-03 07:36:27.882651 cntools-2.1.8/cntools/utils/
+-rw-r--r--   0 yichengtao   (501) staff       (20)      135 2024-05-08 03:17:12.000000 cntools-2.1.8/cntools/utils/__init__.py
+-rw-r--r--   0 yichengtao   (501) staff       (20)  1156429 2024-06-03 07:36:27.000000 cntools-2.1.8/cntools/utils/_k_means_lloyd_reg.c
+-rw-r--r--   0 yichengtao   (501) staff       (20)    10741 2024-05-08 03:17:12.000000 cntools-2.1.8/cntools/utils/_k_means_lloyd_reg.pyx
+-rw-r--r--   0 yichengtao   (501) staff       (20)     6889 2024-05-08 03:17:12.000000 cntools-2.1.8/cntools/utils/kmeans_reg.py
+-rw-r--r--   0 yichengtao   (501) staff       (20)     1787 2024-06-03 07:33:40.000000 cntools-2.1.8/cntools/utils/utils.py
+drwxr-xr-x   0 yichengtao   (501) staff       (20)        0 2024-06-03 07:36:27.884434 cntools-2.1.8/cntools.egg-info/
+-rw-r--r--   0 yichengtao   (501) staff       (20)     5827 2024-06-03 07:36:27.000000 cntools-2.1.8/cntools.egg-info/PKG-INFO
+-rw-r--r--   0 yichengtao   (501) staff       (20)      768 2024-06-03 07:36:27.000000 cntools-2.1.8/cntools.egg-info/SOURCES.txt
+-rw-r--r--   0 yichengtao   (501) staff       (20)        1 2024-06-03 07:36:27.000000 cntools-2.1.8/cntools.egg-info/dependency_links.txt
+-rw-r--r--   0 yichengtao   (501) staff       (20)      285 2024-06-03 07:36:27.000000 cntools-2.1.8/cntools.egg-info/requires.txt
+-rw-r--r--   0 yichengtao   (501) staff       (20)       27 2024-06-03 07:36:27.000000 cntools-2.1.8/cntools.egg-info/top_level.txt
+-rw-r--r--   0 yichengtao   (501) staff       (20)     1376 2024-06-03 07:35:11.000000 cntools-2.1.8/pyproject.toml
+-rw-r--r--   0 yichengtao   (501) staff       (20)       38 2024-06-03 07:36:27.885297 cntools-2.1.8/setup.cfg
+-rw-r--r--   0 yichengtao   (501) staff       (20)      239 2024-05-08 03:17:12.000000 cntools-2.1.8/setup.py
```

### Comparing `cntools-2.1.7/LICENSE` & `cntools-2.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cntools-2.1.7/PKG-INFO` & `cntools-2.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cntools
-Version: 2.1.7
+Version: 2.1.8
 Summary: A package for identifying cellular neighborhoods
 Author-email: Yicheng Tao <yctao@umich.edu>
 Maintainer-email: Yicheng Tao <yctao@umich.edu>
 License: MIT License
         
         Copyright (c) 2022 yctao7
         
@@ -56,15 +56,15 @@
 Requires-Dist: tensorly==0.5.1
 Requires-Dist: tqdm==4.62.1
 Requires-Dist: spatial-lda==0.1.3
 
 # CNTools
 
 ## System requirements
-The software denpendencies are listed in `pyproject.toml`. The software is independent of operating systems. The version the software has been tested on is v2.1.0. *Do not work on clang 16 because of some C++ compile error, which may happen when you have latest ana/mini conda (e.g., 24.3.0).*
+The software denpendencies are listed in `pyproject.toml`. The software is independent of operating systems. The version the software has been tested on is v2.1.8. *Only work on Clang <=15.*
 
 ## Installation guide
 As we need a conda package pydot=1.4.2 (not a pip one), the package should be installed by
 ```
 conda create -n cntools python=3.8 pydot=1.4.2
 conda activate cntools
 python -m pip install cntools
```

### Comparing `cntools-2.1.7/README.md` & `cntools-2.1.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # CNTools
 
 ## System requirements
-The software denpendencies are listed in `pyproject.toml`. The software is independent of operating systems. The version the software has been tested on is v2.1.0. *Do not work on clang 16 because of some C++ compile error, which may happen when you have latest ana/mini conda (e.g., 24.3.0).*
+The software denpendencies are listed in `pyproject.toml`. The software is independent of operating systems. The version the software has been tested on is v2.1.8. *Only work on Clang <=15.*
 
 ## Installation guide
 As we need a conda package pydot=1.4.2 (not a pip one), the package should be installed by
 ```
 conda create -n cntools python=3.8 pydot=1.4.2
 conda activate cntools
 python -m pip install cntools
```

### Comparing `cntools-2.1.7/cntools/datasets/make_ds.py` & `cntools-2.1.8/cntools/datasets/make_ds.py`

 * *Files identical despite different names*

### Comparing `cntools-2.1.7/cntools/datasets/prep.py` & `cntools-2.1.8/cntools/datasets/prep.py`

 * *Files identical despite different names*

### Comparing `cntools-2.1.7/cntools/identification/CC.py` & `cntools-2.1.8/cntools/identification/CC.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,9 +49,9 @@
         feats = np.delete(feats, exclude_ids, axis=1)
         
         feats = normalize(feats, norm='l1', axis=1)
         cns = ds.flat_to_dic(MiniBatchKMeans(n_clusters=self.n_cns, random_state=self.seed).fit_predict(feats))
         
         self.feats = feats
         if self.verbose:
-            cns_info(ds, self.n_cns, cns)
+            cns_info(ds.data, self.n_cns, cns)
         return cns
```

### Comparing `cntools-2.1.7/cntools/identification/CFIDF.py` & `cntools-2.1.8/cntools/identification/CFIDF.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,9 +100,9 @@
                     feats_normed_tmp[nb] = feats_nb[sample][image][nb_id]
                     i += 1
                 feats_normed.append(feats_normed_tmp)
         feats_normed = np.concatenate(feats_normed)
 
         self.feats = feats_normed
         if self.verbose:
-            cns_info(ds, self.n_cns, cns)
+            cns_info(ds.data, self.n_cns, cns)
         return cns
```

### Comparing `cntools-2.1.7/cntools/identification/CNE.py` & `cntools-2.1.8/cntools/identification/CNE.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,9 +68,9 @@
         
         if self.normalize:
             feats = normalize(feats, norm='l1', axis=1) * np.log(ct_counts.sum() / (ct_counts + 1))
         cns = ds.flat_to_dic(KMeans_reg(n_clusters=self.n_cns, random_state=self.seed, lam=self.lam, edges=delauney_edges(ds)).fit_predict(feats))
 
         self.feats = feats
         if self.verbose:
-            cns_info(ds, self.n_cns, cns)
+            cns_info(ds.data, self.n_cns, cns)
         return cns
```

### Comparing `cntools-2.1.7/cntools/identification/Spatial_LDA.py` & `cntools-2.1.8/cntools/identification/Spatial_LDA.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,9 +82,9 @@
             image = int(image) if image.isnumeric() else image
             for i, _ in dfs_image[sample_image].iterrows():
                 cns[sample][image].append(np.argmax(dfs_image_cns.loc(axis=0)[(sample_image, i),]))
         feats = feats.reindex(sorted(feats.columns), axis=1).to_numpy()
         
         self.feats = feats
         if self.verbose:
-            cns_info(ds, self.n_cns, cns)
+            cns_info(ds.data, self.n_cns, cns)
         return cns
```

### Comparing `cntools-2.1.7/cntools/smoothing/HMRF.py` & `cntools-2.1.8/cntools/smoothing/HMRF.py`

 * *Files identical despite different names*

### Comparing `cntools-2.1.7/cntools/smoothing/NaiveSmooth.py` & `cntools-2.1.8/cntools/smoothing/NaiveSmooth.py`

 * *Files identical despite different names*

### Comparing `cntools-2.1.7/cntools/utils/_k_means_lloyd_reg.c` & `cntools-2.1.8/cntools/utils/_k_means_lloyd_reg.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 /* Generated by Cython 0.29.36 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "include_dirs": [
-            "/private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/core/include"
+            "/private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/core/include"
         ],
         "name": "_k_means_lloyd_reg",
         "sources": [
             "cntools/utils/_k_means_lloyd_reg.pyx"
         ]
     },
     "module_name": "_k_means_lloyd_reg"
@@ -1120,195 +1120,195 @@
 
 /* ForceInitThreads.proto */
 #ifndef __PYX_FORCE_INIT_THREADS
   #define __PYX_FORCE_INIT_THREADS 0
 #endif
 
 
-/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":690
+/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":690
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":691
+/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":691
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":692
+/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":693
+/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":693
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":697
+/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":697
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":698
+/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":698
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":699
+/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":700
+/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":700
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":704
+/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":704
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":705
+/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":705
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":714
+/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":714
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":715
+/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":715
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":716
+/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":716
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":718
+/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":719
+/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":720
+/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":720
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":722
+/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":722
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":723
+/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":723
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":725
+/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":726
+/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":727
+/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1339,42 +1339,42 @@
 
 /*--- Type declarations ---*/
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":729
+/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":730
+/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":730
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":731
+/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":733
+/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":733
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -7077,15 +7077,15 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("_k_means_lloyd_reg._update_chunk_dense", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 1);
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 1);
 }
 
-/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":735
+/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -7096,29 +7096,29 @@
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
   __Pyx_TraceCall("PyArray_MultiIterNew1", __pyx_f[1], 735, 0, __PYX_ERR(1, 735, __pyx_L1_error));
 
-  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":736
+  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":736
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 736, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -7130,15 +7130,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":738
+/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -7149,29 +7149,29 @@
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
   __Pyx_TraceCall("PyArray_MultiIterNew2", __pyx_f[1], 738, 0, __PYX_ERR(1, 738, __pyx_L1_error));
 
-  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":739
+  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":739
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 739, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -7183,15 +7183,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":741
+/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -7202,29 +7202,29 @@
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
   __Pyx_TraceCall("PyArray_MultiIterNew3", __pyx_f[1], 741, 0, __PYX_ERR(1, 741, __pyx_L1_error));
 
-  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":742
+  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":742
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 742, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -7236,15 +7236,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":744
+/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -7255,29 +7255,29 @@
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
   __Pyx_TraceCall("PyArray_MultiIterNew4", __pyx_f[1], 744, 0, __PYX_ERR(1, 744, __pyx_L1_error));
 
-  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":745
+  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":745
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 745, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -7289,15 +7289,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":747
+/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -7308,29 +7308,29 @@
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
   __Pyx_TraceCall("PyArray_MultiIterNew5", __pyx_f[1], 747, 0, __PYX_ERR(1, 747, __pyx_L1_error));
 
-  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":748
+  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":748
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 748, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -7342,15 +7342,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":750
+/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
@@ -7361,60 +7361,60 @@
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
   __Pyx_TraceCall("PyDataType_SHAPE", __pyx_f[1], 750, 0, __PYX_ERR(1, 750, __pyx_L1_error));
 
-  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":751
+  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":752
+    /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":752
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":754
+  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":754
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
@@ -7425,15 +7425,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":931
+/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":931
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -7442,33 +7442,33 @@
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_array_base", 0);
   __Pyx_TraceCall("set_array_base", __pyx_f[1], 931, 0, __PYX_ERR(1, 931, __pyx_L1_error));
 
-  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":932
+  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":932
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":933
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":931
+  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":931
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -7477,15 +7477,15 @@
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":935
+/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":935
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
@@ -7497,66 +7497,66 @@
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_array_base", 0);
   __Pyx_TraceCall("get_array_base", __pyx_f[1], 935, 0, __PYX_ERR(1, 935, __pyx_L1_error));
 
-  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":936
+  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":936
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":937
+  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":937
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":938
+    /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":938
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":937
+    /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":937
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":939
+  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":939
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":935
+  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":935
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
@@ -7567,15 +7567,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":943
+/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":943
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -7593,15 +7593,15 @@
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
   __Pyx_TraceCall("import_array", __pyx_f[1], 943, 0, __PYX_ERR(1, 943, __pyx_L1_error));
 
-  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":944
+  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":944
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -7609,53 +7609,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":945
+      /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":945
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 945, __pyx_L3_error)
 
-      /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":944
+      /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":944
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":946
+    /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":946
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 946, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":947
+      /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":947
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 947, __pyx_L5_except_error)
@@ -7663,30 +7663,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 947, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":944
+    /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":944
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":943
+  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":943
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -7702,15 +7702,15 @@
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":949
+/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":949
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -7728,15 +7728,15 @@
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
   __Pyx_TraceCall("import_umath", __pyx_f[1], 949, 0, __PYX_ERR(1, 949, __pyx_L1_error));
 
-  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":950
+  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -7744,53 +7744,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":951
+      /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":951
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 951, __pyx_L3_error)
 
-      /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":950
+      /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":952
+    /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":952
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 952, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":953
+      /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":953
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 953, __pyx_L5_except_error)
@@ -7798,30 +7798,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 953, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":950
+    /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":949
+  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":949
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -7837,15 +7837,15 @@
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":955
+/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":955
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -7863,15 +7863,15 @@
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
   __Pyx_TraceCall("import_ufunc", __pyx_f[1], 955, 0, __PYX_ERR(1, 955, __pyx_L1_error));
 
-  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":956
+  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":956
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -7879,53 +7879,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":957
+      /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":957
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 957, __pyx_L3_error)
 
-      /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":956
+      /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":956
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":958
+    /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":958
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 958, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":959
+      /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":959
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 959, __pyx_L5_except_error)
@@ -7933,30 +7933,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 959, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":956
+    /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":956
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":955
+  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":955
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -7972,15 +7972,15 @@
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":969
+/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":969
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
@@ -7990,25 +7990,25 @@
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
   __Pyx_TraceCall("is_timedelta64_object", __pyx_f[1], 969, 0, __PYX_ERR(1, 969, __pyx_L1_error));
 
-  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":981
+  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":981
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":969
+  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":969
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
@@ -8018,15 +8018,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":984
+/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":984
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
@@ -8036,25 +8036,25 @@
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
   __Pyx_TraceCall("is_datetime64_object", __pyx_f[1], 984, 0, __PYX_ERR(1, 984, __pyx_L1_error));
 
-  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":996
+  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":996
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":984
+  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":984
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
@@ -8064,15 +8064,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":999
+/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":999
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
@@ -8080,25 +8080,25 @@
   npy_datetime __pyx_r;
   __Pyx_TraceDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_TraceCall("get_datetime64_value", __pyx_f[1], 999, 1, __PYX_ERR(1, 999, __pyx_L1_error));
 
-  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":1006
+  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":1006
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":999
+  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":999
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
@@ -8107,15 +8107,15 @@
   __Pyx_WriteUnraisable("numpy.get_datetime64_value", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 1);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 1);
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":1009
+/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":1009
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
@@ -8123,25 +8123,25 @@
   npy_timedelta __pyx_r;
   __Pyx_TraceDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_TraceCall("get_timedelta64_value", __pyx_f[1], 1009, 1, __PYX_ERR(1, 1009, __pyx_L1_error));
 
-  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":1013
+  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":1013
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":1009
+  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":1009
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
@@ -8150,15 +8150,15 @@
   __Pyx_WriteUnraisable("numpy.get_timedelta64_value", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 1);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 1);
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":1016
+/* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":1016
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -8166,23 +8166,23 @@
   NPY_DATETIMEUNIT __pyx_r;
   __Pyx_TraceDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_TraceCall("get_datetime64_unit", __pyx_f[1], 1016, 1, __PYX_ERR(1, 1016, __pyx_L1_error));
 
-  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":1020
+  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":1020
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":1016
+  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":1016
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -22588,26 +22588,26 @@
   __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_s_No_matching_signature_found); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 38, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
   __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_s_Function_call_with_ambiguous_arg); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 38, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
 
-  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":947
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(1, 947, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__5);
   __Pyx_GIVEREF(__pyx_tuple__5);
 
-  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-y2be3c6p/lib/python3.8/site-packages/numpy/__init__.pxd":953
+  /* "../../../../../private/var/folders/hs/ljx_n2857y7g_lhq6hrr4dlw0000gn/T/build-env-egyvn66m/lib/python3.8/site-packages/numpy/__init__.pxd":953
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(1, 953, __pyx_L1_error)
```

### Comparing `cntools-2.1.7/cntools/utils/_k_means_lloyd_reg.pyx` & `cntools-2.1.8/cntools/utils/_k_means_lloyd_reg.pyx`

 * *Files identical despite different names*

### Comparing `cntools-2.1.7/cntools/utils/kmeans_reg.py` & `cntools-2.1.8/cntools/utils/kmeans_reg.py`

 * *Files identical despite different names*

### Comparing `cntools-2.1.7/cntools/utils/utils.py` & `cntools-2.1.8/cntools/utils/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import networkx as nx
 import numpy as np
 from scipy.sparse import csr_matrix
 
 
-def cns_info(ds, n_cns, cns):
-    data = ds.data
+def cns_info(data, n_cns, cns):
     info_ent, info_pat, info_size = {i: [] for i in range(n_cns)}, np.zeros(n_cns), np.zeros(n_cns)
     for sample in data:
         for image in data[sample]:
             graph = nx.Graph(data[sample][image].edge_indices)
             graph.add_nodes_from([i for i in range(data[sample][image].n_cells)])
             for edge in graph.edges:
                 if cns[sample][image][edge[0]] != cns[sample][image][edge[1]]:
@@ -21,15 +20,17 @@
         if not info_ent[i]:
             info_ent[i] = 0
         else:
             p = np.array(info_ent[i]).mean(axis=0)
             p = p[p.nonzero()]
             info_ent[i] = -(p * np.log2(p)).sum()
     info_ent = np.array(list(info_ent.values()))
-    print(f'Entropy: {(info_ent * info_size / info_size.sum()).sum():.3f}, Size: {sum(info_size) / sum(info_pat):.2f}')
+    entropy, size = (info_ent * info_size / info_size.sum()).sum(), sum(info_size) / sum(info_pat)
+    print(f'Entropy: {entropy:.3f}, Size: {size:.2f}')
+    return entropy, size
 
 
 def delauney_edges(ds):
     data = ds.data
     edges = [[], []]
     i = 0
     for sample in data:
```

### Comparing `cntools-2.1.7/cntools.egg-info/PKG-INFO` & `cntools-2.1.8/cntools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cntools
-Version: 2.1.7
+Version: 2.1.8
 Summary: A package for identifying cellular neighborhoods
 Author-email: Yicheng Tao <yctao@umich.edu>
 Maintainer-email: Yicheng Tao <yctao@umich.edu>
 License: MIT License
         
         Copyright (c) 2022 yctao7
         
@@ -56,15 +56,15 @@
 Requires-Dist: tensorly==0.5.1
 Requires-Dist: tqdm==4.62.1
 Requires-Dist: spatial-lda==0.1.3
 
 # CNTools
 
 ## System requirements
-The software denpendencies are listed in `pyproject.toml`. The software is independent of operating systems. The version the software has been tested on is v2.1.0. *Do not work on clang 16 because of some C++ compile error, which may happen when you have latest ana/mini conda (e.g., 24.3.0).*
+The software denpendencies are listed in `pyproject.toml`. The software is independent of operating systems. The version the software has been tested on is v2.1.8. *Only work on Clang <=15.*
 
 ## Installation guide
 As we need a conda package pydot=1.4.2 (not a pip one), the package should be installed by
 ```
 conda create -n cntools python=3.8 pydot=1.4.2
 conda activate cntools
 python -m pip install cntools
```

### Comparing `cntools-2.1.7/cntools.egg-info/SOURCES.txt` & `cntools-2.1.8/cntools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cntools-2.1.7/pyproject.toml` & `cntools-2.1.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "cntools"
-version = "2.1.7"
+version = "2.1.8"
 description = "A package for identifying cellular neighborhoods"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 keywords = ["cellular neighborhoods"]
 authors = [
     {name = "Yicheng Tao", email = "yctao@umich.edu" }
```

