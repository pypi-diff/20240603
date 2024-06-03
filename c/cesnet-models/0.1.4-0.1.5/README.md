# Comparing `tmp/cesnet_models-0.1.4.tar.gz` & `tmp/cesnet_models-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cesnet_models-0.1.4.tar", last modified: Fri May 10 12:22:28 2024, max compression
+gzip compressed data, was "cesnet_models-0.1.5.tar", last modified: Mon Jun  3 11:41:12 2024, max compression
```

## Comparing `cesnet_models-0.1.4.tar` & `cesnet_models-0.1.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 12:22:28.236442 cesnet_models-0.1.4/
--rw-rw-rw-   0        0        0     1541 2023-09-18 09:03:44.000000 cesnet_models-0.1.4/LICENCE
--rw-rw-rw-   0        0        0     3557 2024-05-10 12:22:28.236442 cesnet_models-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     2200 2024-04-10 08:36:57.000000 cesnet_models-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 12:22:28.203055 cesnet_models-0.1.4/cesnet_models/
--rw-rw-rw-   0        0        0        0 2023-01-18 16:43:04.000000 cesnet_models-0.1.4/cesnet_models/__init__.py
--rw-rw-rw-   0        0        0     5949 2024-04-08 09:20:47.000000 cesnet_models-0.1.4/cesnet_models/_models_meta.py
-drwxrwxrwx   0        0        0        0 2024-05-10 12:22:28.233040 cesnet_models-0.1.4/cesnet_models/architectures/
--rw-rw-rw-   0        0        0        0 2023-01-18 16:43:04.000000 cesnet_models-0.1.4/cesnet_models/architectures/__init__.py
--rw-rw-rw-   0        0        0     2340 2024-05-10 10:10:30.000000 cesnet_models-0.1.4/cesnet_models/architectures/cnn_resblock.py
--rw-rw-rw-   0        0        0     8675 2024-05-10 10:10:18.000000 cesnet_models-0.1.4/cesnet_models/architectures/multimodal_cesnet.py
--rw-rw-rw-   0        0        0    17841 2024-05-10 12:21:05.000000 cesnet_models-0.1.4/cesnet_models/architectures/multimodal_cesnet_enhanced.py
--rw-rw-rw-   0        0        0       71 2024-04-29 12:31:20.000000 cesnet_models-0.1.4/cesnet_models/constants.py
--rw-rw-rw-   0        0        0     1112 2024-03-18 11:22:51.000000 cesnet_models-0.1.4/cesnet_models/helpers.py
--rw-rw-rw-   0        0        0    11966 2024-05-07 10:23:57.000000 cesnet_models-0.1.4/cesnet_models/models.py
--rw-rw-rw-   0        0        0    14604 2024-04-30 12:17:48.000000 cesnet_models-0.1.4/cesnet_models/transforms.py
-drwxrwxrwx   0        0        0        0 2024-05-10 12:22:28.235042 cesnet_models-0.1.4/cesnet_models.egg-info/
--rw-rw-rw-   0        0        0     3557 2024-05-10 12:22:28.000000 cesnet_models-0.1.4/cesnet_models.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      567 2024-05-10 12:22:28.000000 cesnet_models-0.1.4/cesnet_models.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 12:22:28.000000 cesnet_models-0.1.4/cesnet_models.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      149 2024-05-10 12:22:28.000000 cesnet_models-0.1.4/cesnet_models.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-10 12:22:28.000000 cesnet_models-0.1.4/cesnet_models.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1448 2024-05-10 12:21:53.000000 cesnet_models-0.1.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-10 12:22:28.237852 cesnet_models-0.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-06-03 11:41:12.309680 cesnet_models-0.1.5/
+-rw-rw-rw-   0        0        0     1541 2023-09-18 09:03:44.000000 cesnet_models-0.1.5/LICENCE
+-rw-rw-rw-   0        0        0     3557 2024-06-03 11:41:12.308174 cesnet_models-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2200 2024-04-10 08:36:57.000000 cesnet_models-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-06-03 11:41:12.277657 cesnet_models-0.1.5/cesnet_models/
+-rw-rw-rw-   0        0        0        0 2023-01-18 16:43:04.000000 cesnet_models-0.1.5/cesnet_models/__init__.py
+-rw-rw-rw-   0        0        0     5949 2024-04-08 09:20:47.000000 cesnet_models-0.1.5/cesnet_models/_models_meta.py
+drwxrwxrwx   0        0        0        0 2024-06-03 11:41:12.305565 cesnet_models-0.1.5/cesnet_models/architectures/
+-rw-rw-rw-   0        0        0        0 2023-01-18 16:43:04.000000 cesnet_models-0.1.5/cesnet_models/architectures/__init__.py
+-rw-rw-rw-   0        0        0     2340 2024-05-10 10:10:30.000000 cesnet_models-0.1.5/cesnet_models/architectures/cnn_resblock.py
+-rw-rw-rw-   0        0        0     8675 2024-05-10 10:10:18.000000 cesnet_models-0.1.5/cesnet_models/architectures/multimodal_cesnet.py
+-rw-rw-rw-   0        0        0    17747 2024-06-03 11:38:57.000000 cesnet_models-0.1.5/cesnet_models/architectures/multimodal_cesnet_enhanced.py
+-rw-rw-rw-   0        0        0       71 2024-04-29 12:31:20.000000 cesnet_models-0.1.5/cesnet_models/constants.py
+-rw-rw-rw-   0        0        0     1112 2024-03-18 11:22:51.000000 cesnet_models-0.1.5/cesnet_models/helpers.py
+-rw-rw-rw-   0        0        0    11966 2024-05-07 10:23:57.000000 cesnet_models-0.1.5/cesnet_models/models.py
+-rw-rw-rw-   0        0        0    14604 2024-04-30 12:17:48.000000 cesnet_models-0.1.5/cesnet_models/transforms.py
+drwxrwxrwx   0        0        0        0 2024-06-03 11:41:12.307161 cesnet_models-0.1.5/cesnet_models.egg-info/
+-rw-rw-rw-   0        0        0     3557 2024-06-03 11:41:12.000000 cesnet_models-0.1.5/cesnet_models.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      567 2024-06-03 11:41:12.000000 cesnet_models-0.1.5/cesnet_models.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 11:41:12.000000 cesnet_models-0.1.5/cesnet_models.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      149 2024-06-03 11:41:12.000000 cesnet_models-0.1.5/cesnet_models.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-06-03 11:41:12.000000 cesnet_models-0.1.5/cesnet_models.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1448 2024-06-03 11:39:35.000000 cesnet_models-0.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-06-03 11:41:12.309680 cesnet_models-0.1.5/setup.cfg
```

### Comparing `cesnet_models-0.1.4/LICENCE` & `cesnet_models-0.1.5/LICENCE`

 * *Files identical despite different names*

### Comparing `cesnet_models-0.1.4/PKG-INFO` & `cesnet_models-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cesnet-models
-Version: 0.1.4
+Version: 0.1.5
 Summary: Pre-trained neural networks for encrypted traffic classification
 Author-email: Jan Luxemburk <luxemburk@cesnet.cz>, Karel Hynek <hynekkar@cesnet.cz>
 Maintainer-email: Jan Luxemburk <luxemburk@cesnet.cz>, Karel Hynek <hynekkar@cesnet.cz>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/CESNET/cesnet-models
 Project-URL: Documentation, https://cesnet.github.io/cesnet-models/
 Project-URL: Bug Tracker, https://github.com/CESNET/cesnet-models/issues
```

### Comparing `cesnet_models-0.1.4/README.md` & `cesnet_models-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `cesnet_models-0.1.4/cesnet_models/_models_meta.py` & `cesnet_models-0.1.5/cesnet_models/_models_meta.py`

 * *Files identical despite different names*

### Comparing `cesnet_models-0.1.4/cesnet_models/architectures/cnn_resblock.py` & `cesnet_models-0.1.5/cesnet_models/architectures/cnn_resblock.py`

 * *Files identical despite different names*

### Comparing `cesnet_models-0.1.4/cesnet_models/architectures/multimodal_cesnet.py` & `cesnet_models-0.1.5/cesnet_models/architectures/multimodal_cesnet.py`

 * *Files identical despite different names*

### Comparing `cesnet_models-0.1.4/cesnet_models/architectures/multimodal_cesnet_enhanced.py` & `cesnet_models-0.1.5/cesnet_models/architectures/multimodal_cesnet_enhanced.py`

 * *Files 2% similar despite different names*

```diff
@@ -263,20 +263,20 @@
 class Multimodal_CESNET_Enhanced(nn.Module):
     def __init__(self, num_classes: int,
                        flowstats_input_size: int,
                        ppi_input_channels: int,
                        use_flowstats: bool = True,
                        init_weights: bool = True,
                        cnn_ppi_stem_type: StemType = StemType.EMBED_CONV, packet_embedding_size: int = 7, packet_embedding_include_dirs: bool = True, packet_embedding_init: bool = True,
-                       conv_normalization: NormalizationEnum = NormalizationEnum.GROUP_NORM, linear_normalization: NormalizationEnum = NormalizationEnum.LAYER_NORM, group_norm_groups: int = 16,
+                       conv_normalization: NormalizationEnum = NormalizationEnum.BATCH_NORM, linear_normalization: NormalizationEnum = NormalizationEnum.BATCH_NORM, group_norm_groups: int = 16,
                        cnn_ppi_channels: tuple[int, ...] = (128, 256, 384, 384), cnn_ppi_strides: tuple[int, ...] = (1, 1, 2, 1), cnn_ppi_kernel_sizes: tuple[int, ...] = (7, 5, 5, 3),
                        cnn_ppi_use_stdconv: bool = True, cnn_ppi_downsample_avg: bool = True, cnn_ppi_blocks_dropout_rate: float = 0.0,
                        cnn_ppi_global_pool: GlobalPoolEnum = GlobalPoolEnum.AVG, cnn_ppi_dropout_rate: float = 0.0,
-                       mlp_flowstats_size1: int = 256, mlp_flowstats_size2: int = 64, mlp_flowstats_num_hidden: int = 2, mlp_flowstats_dropout_rate: float = 0.1,
-                       mlp_shared_size: int = 512, mlp_shared_num_hidden: int = 0, mlp_shared_dropout_rate: float = 0.2,
+                       mlp_flowstats_size1: int = 256, mlp_flowstats_size2: int = 64, mlp_flowstats_num_hidden: int = 1, mlp_flowstats_dropout_rate: float = 0.0,
+                       mlp_shared_size: int = 512, mlp_shared_dropout_rate: float = 0.0,
                        ):
         super().__init__()
         assert ppi_input_channels == 3
         self.num_classes = num_classes
         self.flowstats_input_size = flowstats_input_size
         self.use_flowstats = use_flowstats
         self.packet_embedding_include_dirs = packet_embedding_include_dirs
@@ -300,45 +300,39 @@
                                      stem_output_channels=stem_output_channels,
                                      dropout_rate_path=cnn_ppi_blocks_dropout_rate,
                                      downsample_avg=cnn_ppi_downsample_avg,
                                      conv=conv, norm=conv_norm)
         self.cnn_global_pooling = nn.Sequential(
             nn.AdaptiveAvgPool1d(output_size=1) if cnn_ppi_global_pool == GlobalPoolEnum.AVG else nn.AdaptiveMaxPool1d(output_size=1),
             nn.Flatten(),
-            nn.Dropout(cnn_ppi_dropout_rate),
+            nn.Dropout(cnn_ppi_dropout_rate) if cnn_ppi_dropout_rate > 0 else nn.Identity(),
             nn.ReLU(inplace=True),
         )
         self.mlp_flowstats = nn.Sequential(
             nn.Linear(flowstats_input_size, mlp_flowstats_size1),
             linear_norm(mlp_flowstats_size1),
             nn.ReLU(inplace=True),
 
             *(nn.Sequential(
                 nn.Linear(mlp_flowstats_size1, mlp_flowstats_size1),
                 linear_norm(mlp_flowstats_size1),
                 nn.ReLU(inplace=True),) for _ in range(mlp_flowstats_num_hidden)),
 
             nn.Linear(mlp_flowstats_size1, mlp_flowstats_size2),
             linear_norm(mlp_flowstats_size2),
-            nn.Dropout(mlp_flowstats_dropout_rate),
+            nn.Dropout(mlp_flowstats_dropout_rate) if mlp_flowstats_dropout_rate > 0 else nn.Identity(),
             nn.ReLU(inplace=True),
         )
         self.mlp_shared = nn.Sequential(
             nn.Linear(mlp_shared_input_size, mlp_shared_size),
             linear_norm(mlp_shared_size),
-            nn.Dropout(mlp_shared_dropout_rate),
             nn.ReLU(inplace=True),
-
-            *(nn.Sequential(
-                nn.Linear(mlp_shared_size, mlp_shared_size),
-                linear_norm(mlp_shared_size),
-                nn.Dropout(mlp_shared_dropout_rate),
-                nn.ReLU(inplace=True),) for _ in range(mlp_shared_num_hidden)),
+            nn.Dropout(mlp_shared_dropout_rate) if mlp_shared_dropout_rate > 0 else nn.Identity(),
         )
-        self.classifier = nn.Linear(mlp_shared_size, num_classes)
+        self.classifier = nn.Linear(self.mlp_shared_size, num_classes)
         if init_weights:
             self.apply(init_weights_fn)
 
     def forward_features(self, ppi, flowstats):
         if self.cnn_ppi_stem_type == StemType.EMBED or self.cnn_ppi_stem_type == StemType.EMBED_CONV:
             assert self.packet_embedding is not None
             if self.packet_embedding_include_dirs:
@@ -352,14 +346,15 @@
                 ppi_embedded = torch.cat((
                     ppi[:, PPI_IPT_POS, :].unsqueeze(-1),
                     ppi[:, PPI_DIR_POS, :].unsqueeze(-1),
                     self.packet_embedding(embedding_input)
                 ), dim=2).transpose(1, 2)
         else:
             ppi_embedded = ppi
+            # One-hot encode directions without embedding
             # ppi_embedded = torch.cat((
             #         ppi[:, PPI_IPT_POS, :].unsqueeze(-1),
             #         (ppi[:, PPI_DIR_POS, :] > 0).int().unsqueeze(-1),
             #         (ppi[:, PPI_DIR_POS, :] < 0).int().unsqueeze(-1),
             #         ppi[:, PPI_SIZE_POS, :].unsqueeze(-1),
             #     ), dim=2).transpose(1, 2)
         out = self.cnn_ppi_stem(ppi_embedded)
```

### Comparing `cesnet_models-0.1.4/cesnet_models/helpers.py` & `cesnet_models-0.1.5/cesnet_models/helpers.py`

 * *Files identical despite different names*

### Comparing `cesnet_models-0.1.4/cesnet_models/models.py` & `cesnet_models-0.1.5/cesnet_models/models.py`

 * *Files identical despite different names*

### Comparing `cesnet_models-0.1.4/cesnet_models/transforms.py` & `cesnet_models-0.1.5/cesnet_models/transforms.py`

 * *Files identical despite different names*

### Comparing `cesnet_models-0.1.4/cesnet_models.egg-info/PKG-INFO` & `cesnet_models-0.1.5/cesnet_models.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cesnet-models
-Version: 0.1.4
+Version: 0.1.5
 Summary: Pre-trained neural networks for encrypted traffic classification
 Author-email: Jan Luxemburk <luxemburk@cesnet.cz>, Karel Hynek <hynekkar@cesnet.cz>
 Maintainer-email: Jan Luxemburk <luxemburk@cesnet.cz>, Karel Hynek <hynekkar@cesnet.cz>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/CESNET/cesnet-models
 Project-URL: Documentation, https://cesnet.github.io/cesnet-models/
 Project-URL: Bug Tracker, https://github.com/CESNET/cesnet-models/issues
```

### Comparing `cesnet_models-0.1.4/cesnet_models.egg-info/SOURCES.txt` & `cesnet_models-0.1.5/cesnet_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cesnet_models-0.1.4/pyproject.toml` & `cesnet_models-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cesnet-models"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   {name = "Jan Luxemburk", email = "luxemburk@cesnet.cz"},
   {name = "Karel Hynek", email = "hynekkar@cesnet.cz"},
 ]
 maintainers = [
   {name = "Jan Luxemburk", email = "luxemburk@cesnet.cz"},
   {name = "Karel Hynek", email = "hynekkar@cesnet.cz"},
```

