# Comparing `tmp/medicraft-0.9.0.tar.gz` & `tmp/medicraft-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medicraft-0.9.0.tar", max compression
+gzip compressed data, was "medicraft-0.9.1.tar", max compression
```

## Comparing `medicraft-0.9.0.tar` & `medicraft-0.9.1.tar`

### file list

```diff
@@ -1,41 +1,42 @@
--rw-r--r--   0        0        0     1333 2024-06-02 19:44:52.723705 medicraft-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      989 2024-05-31 15:18:57.050798 medicraft-0.9.0/src/medicraft/config.py
--rw-r--r--   0        0        0      278 2024-05-31 15:18:57.050798 medicraft-0.9.0/src/medicraft/datasets/__init__.py
--rw-r--r--   0        0        0     5938 2024-05-31 15:18:57.050798 medicraft-0.9.0/src/medicraft/datasets/eye_scans.py
--rw-r--r--   0        0        0     4662 2024-05-31 15:18:57.050798 medicraft-0.9.0/src/medicraft/datasets/opthal_anonymized.py
--rw-r--r--   0        0        0     5348 2024-05-31 15:18:57.050798 medicraft-0.9.0/src/medicraft/datasets/prepare_dataset.py
--rw-r--r--   0        0        0     1842 2024-05-31 15:18:57.050798 medicraft-0.9.0/src/medicraft/datasets/preprocess.py
--rw-r--r--   0        0        0     1847 2024-04-30 11:48:34.271053 medicraft-0.9.0/src/medicraft/experiments/local_run_experiment.py
--rw-r--r--   0        0        0     1130 2024-05-31 15:18:57.050798 medicraft-0.9.0/src/medicraft/experiments/old_run_experiment.py
--rw-r--r--   0        0        0     1579 2024-05-31 15:18:57.050798 medicraft-0.9.0/src/medicraft/experiments/test_run_experiment.py
--rw-r--r--   0        0        0     4382 2024-06-02 18:57:17.294145 medicraft-0.9.0/src/medicraft/generate_dataset_temp.py
--rw-r--r--   0        0        0     2092 2024-05-31 15:18:57.050798 medicraft-0.9.0/src/medicraft/generate_samples.py
--rw-r--r--   0        0        0      796 2024-05-31 15:18:57.050798 medicraft-0.9.0/src/medicraft/main.py
--rw-r--r--   0        0        0      308 2024-05-31 15:18:57.050798 medicraft-0.9.0/src/medicraft/models/__init__.py
--rw-r--r--   0        0        0     6642 2024-05-31 15:18:57.051797 medicraft-0.9.0/src/medicraft/models/classifier.py
--rw-r--r--   0        0        0     1877 2024-05-31 15:18:57.051797 medicraft-0.9.0/src/medicraft/models/gausian_diffusion.py
--rw-r--r--   0        0        0      525 2024-05-31 15:18:57.051797 medicraft-0.9.0/src/medicraft/pipeline/__init__.py
--rw-r--r--   0        0        0      493 2024-05-31 15:18:57.051797 medicraft-0.9.0/src/medicraft/pipeline/blocks/__init__.py
--rw-r--r--   0        0        0      339 2024-05-31 15:18:57.051797 medicraft-0.9.0/src/medicraft/pipeline/blocks/blocks.py
--rw-r--r--   0        0        0      847 2024-05-31 15:18:57.051797 medicraft-0.9.0/src/medicraft/pipeline/blocks/data_dto.py
--rw-r--r--   0        0        0     4578 2024-05-31 15:18:57.051797 medicraft-0.9.0/src/medicraft/pipeline/blocks/experiment_dto.py
--rw-r--r--   0        0        0      255 2024-05-31 15:18:57.051797 medicraft-0.9.0/src/medicraft/pipeline/blocks/general_dto.py
--rw-r--r--   0        0        0      232 2024-05-31 15:18:57.051797 medicraft-0.9.0/src/medicraft/pipeline/blocks/models_dto.py
--rw-r--r--   0        0        0      166 2024-05-31 15:18:57.051797 medicraft-0.9.0/src/medicraft/pipeline/blocks/output_dto.py
--rw-r--r--   0        0        0     4356 2024-05-31 15:18:57.051797 medicraft-0.9.0/src/medicraft/pipeline/parser.py
--rw-r--r--   0        0        0    16991 2024-05-31 15:18:57.051797 medicraft-0.9.0/src/medicraft/pipeline/pipeline.py
--rw-r--r--   0        0        0     2876 2024-05-31 15:18:57.051797 medicraft-0.9.0/src/medicraft/run_classification_experiment.py
--rw-r--r--   0        0        0     2700 2024-05-31 15:18:57.051797 medicraft-0.9.0/src/medicraft/run_experiment.py
--rw-r--r--   0        0        0      555 2024-05-31 15:18:57.052798 medicraft-0.9.0/src/medicraft/trackers/__init__.py
--rw-r--r--   0        0        0     1449 2024-05-31 15:18:57.052798 medicraft-0.9.0/src/medicraft/trackers/callbacks.py
--rw-r--r--   0        0        0     3889 2024-05-31 15:18:57.052798 medicraft-0.9.0/src/medicraft/trackers/wandb.py
--rw-r--r--   0        0        0      121 2024-05-31 15:18:57.052798 medicraft-0.9.0/src/medicraft/trainers/__init__.py
--rw-r--r--   0        0        0    13634 2024-05-31 15:18:57.052798 medicraft-0.9.0/src/medicraft/trainers/trainer.py
--rw-r--r--   0        0        0       90 2024-05-31 15:18:57.052798 medicraft-0.9.0/src/medicraft/utils/__init__.py
--rw-r--r--   0        0        0      338 2024-05-31 15:18:57.052798 medicraft-0.9.0/src/medicraft/utils/artifact_utilities.py
--rw-r--r--   0        0        0     1626 2024-05-31 15:18:57.052798 medicraft-0.9.0/src/medicraft/utils/files_managment.py
--rw-r--r--   0        0        0      926 2024-05-31 15:18:57.052798 medicraft-0.9.0/src/medicraft/utils/transforms.py
--rw-r--r--   0        0        0       61 2024-05-31 15:18:57.052798 medicraft-0.9.0/src/medicraft/validation/__init__.py
--rw-r--r--   0        0        0     8625 2024-05-31 15:18:57.052798 medicraft-0.9.0/src/medicraft/validation/embeddings.py
--rw-r--r--   0        0        0     1219 2024-06-02 19:46:04.209110 medicraft-0.9.0/setup.py
--rw-r--r--   0        0        0      864 2024-06-02 19:46:04.209589 medicraft-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     2455 2024-05-31 15:29:33.866882 medicraft-0.9.1/README.md
+-rw-r--r--   0        0        0     1908 2024-06-02 20:06:36.544336 medicraft-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0      989 2024-05-31 15:18:57.050798 medicraft-0.9.1/src/medicraft/config.py
+-rw-r--r--   0        0        0      278 2024-05-31 15:18:57.050798 medicraft-0.9.1/src/medicraft/datasets/__init__.py
+-rw-r--r--   0        0        0     5938 2024-05-31 15:18:57.050798 medicraft-0.9.1/src/medicraft/datasets/eye_scans.py
+-rw-r--r--   0        0        0     4662 2024-05-31 15:18:57.050798 medicraft-0.9.1/src/medicraft/datasets/opthal_anonymized.py
+-rw-r--r--   0        0        0     5348 2024-05-31 15:18:57.050798 medicraft-0.9.1/src/medicraft/datasets/prepare_dataset.py
+-rw-r--r--   0        0        0     1842 2024-05-31 15:18:57.050798 medicraft-0.9.1/src/medicraft/datasets/preprocess.py
+-rw-r--r--   0        0        0     1847 2024-04-30 11:48:34.271053 medicraft-0.9.1/src/medicraft/experiments/local_run_experiment.py
+-rw-r--r--   0        0        0     1130 2024-05-31 15:18:57.050798 medicraft-0.9.1/src/medicraft/experiments/old_run_experiment.py
+-rw-r--r--   0        0        0     1579 2024-05-31 15:18:57.050798 medicraft-0.9.1/src/medicraft/experiments/test_run_experiment.py
+-rw-r--r--   0        0        0     4382 2024-06-02 18:57:17.294145 medicraft-0.9.1/src/medicraft/generate_dataset_temp.py
+-rw-r--r--   0        0        0     2092 2024-05-31 15:18:57.050798 medicraft-0.9.1/src/medicraft/generate_samples.py
+-rw-r--r--   0        0        0      796 2024-05-31 15:18:57.050798 medicraft-0.9.1/src/medicraft/main.py
+-rw-r--r--   0        0        0      308 2024-05-31 15:18:57.050798 medicraft-0.9.1/src/medicraft/models/__init__.py
+-rw-r--r--   0        0        0     6642 2024-05-31 15:18:57.051797 medicraft-0.9.1/src/medicraft/models/classifier.py
+-rw-r--r--   0        0        0     1877 2024-05-31 15:18:57.051797 medicraft-0.9.1/src/medicraft/models/gausian_diffusion.py
+-rw-r--r--   0        0        0      525 2024-05-31 15:18:57.051797 medicraft-0.9.1/src/medicraft/pipeline/__init__.py
+-rw-r--r--   0        0        0      493 2024-05-31 15:18:57.051797 medicraft-0.9.1/src/medicraft/pipeline/blocks/__init__.py
+-rw-r--r--   0        0        0      339 2024-05-31 15:18:57.051797 medicraft-0.9.1/src/medicraft/pipeline/blocks/blocks.py
+-rw-r--r--   0        0        0      847 2024-05-31 15:18:57.051797 medicraft-0.9.1/src/medicraft/pipeline/blocks/data_dto.py
+-rw-r--r--   0        0        0     4578 2024-05-31 15:18:57.051797 medicraft-0.9.1/src/medicraft/pipeline/blocks/experiment_dto.py
+-rw-r--r--   0        0        0      255 2024-05-31 15:18:57.051797 medicraft-0.9.1/src/medicraft/pipeline/blocks/general_dto.py
+-rw-r--r--   0        0        0      232 2024-05-31 15:18:57.051797 medicraft-0.9.1/src/medicraft/pipeline/blocks/models_dto.py
+-rw-r--r--   0        0        0      166 2024-05-31 15:18:57.051797 medicraft-0.9.1/src/medicraft/pipeline/blocks/output_dto.py
+-rw-r--r--   0        0        0     4356 2024-05-31 15:18:57.051797 medicraft-0.9.1/src/medicraft/pipeline/parser.py
+-rw-r--r--   0        0        0    16991 2024-05-31 15:18:57.051797 medicraft-0.9.1/src/medicraft/pipeline/pipeline.py
+-rw-r--r--   0        0        0     2876 2024-05-31 15:18:57.051797 medicraft-0.9.1/src/medicraft/run_classification_experiment.py
+-rw-r--r--   0        0        0     2700 2024-05-31 15:18:57.051797 medicraft-0.9.1/src/medicraft/run_experiment.py
+-rw-r--r--   0        0        0      555 2024-05-31 15:18:57.052798 medicraft-0.9.1/src/medicraft/trackers/__init__.py
+-rw-r--r--   0        0        0     1449 2024-05-31 15:18:57.052798 medicraft-0.9.1/src/medicraft/trackers/callbacks.py
+-rw-r--r--   0        0        0     3889 2024-05-31 15:18:57.052798 medicraft-0.9.1/src/medicraft/trackers/wandb.py
+-rw-r--r--   0        0        0      121 2024-05-31 15:18:57.052798 medicraft-0.9.1/src/medicraft/trainers/__init__.py
+-rw-r--r--   0        0        0    13634 2024-05-31 15:18:57.052798 medicraft-0.9.1/src/medicraft/trainers/trainer.py
+-rw-r--r--   0        0        0       90 2024-05-31 15:18:57.052798 medicraft-0.9.1/src/medicraft/utils/__init__.py
+-rw-r--r--   0        0        0      338 2024-05-31 15:18:57.052798 medicraft-0.9.1/src/medicraft/utils/artifact_utilities.py
+-rw-r--r--   0        0        0     1626 2024-05-31 15:18:57.052798 medicraft-0.9.1/src/medicraft/utils/files_managment.py
+-rw-r--r--   0        0        0      926 2024-05-31 15:18:57.052798 medicraft-0.9.1/src/medicraft/utils/transforms.py
+-rw-r--r--   0        0        0       61 2024-05-31 15:18:57.052798 medicraft-0.9.1/src/medicraft/validation/__init__.py
+-rw-r--r--   0        0        0     8625 2024-05-31 15:18:57.052798 medicraft-0.9.1/src/medicraft/validation/embeddings.py
+-rw-r--r--   0        0        0     3755 2024-06-02 20:06:40.073116 medicraft-0.9.1/setup.py
+-rw-r--r--   0        0        0     3918 2024-06-02 20:06:40.073402 medicraft-0.9.1/PKG-INFO
```

### Comparing `medicraft-0.9.0/pyproject.toml` & `medicraft-0.9.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,33 @@
 [tool.poetry]
 name = "medicraft"
-version = "0.9.0"
+version = "0.9.1"
 description = "Medicraft synthetic dataset generator"
 authors = ["Filip Patyk <fp.patyk@gmail.com>"]
+repository = "https://github.com/drfifonz/medicraft"
+documentation  = "https://drfifonz.github.io/medicraft/"
+keywords = ["diffusion", "generating","medical","images","synthetic dataset","pytorch","torch","diffusion","denoising"]
+readme = "README.md"
 license = "MIT"
+
+classifiers = [
+    "Development Status :: 4 - Beta",
+    "Environment :: GPU :: NVIDIA CUDA :: 12",
+    "License :: OSI Approved :: MIT License",
+    "Programming Language :: Python :: 3.11",
+    "Topic :: Scientific/Engineering :: Artificial Intelligence",
+    "Topic :: Scientific/Engineering :: Image Processing",
+
+]
+
 packages = [
     { include = "medicraft", from = "src" }
 ]
 
+
 [tool.poetry.dependencies]
 python = "^3.11"
 torch = "2.3.0"
 denoising-diffusion-pytorch = "1.9.4"
 ema-pytorch = "0.3.1"
 lightning = "2.2.1"
 matplotlib = "3.8.4"
```

### Comparing `medicraft-0.9.0/src/medicraft/config.py` & `medicraft-0.9.1/src/medicraft/config.py`

 * *Files identical despite different names*

### Comparing `medicraft-0.9.0/src/medicraft/datasets/eye_scans.py` & `medicraft-0.9.1/src/medicraft/datasets/eye_scans.py`

 * *Files identical despite different names*

### Comparing `medicraft-0.9.0/src/medicraft/datasets/opthal_anonymized.py` & `medicraft-0.9.1/src/medicraft/datasets/opthal_anonymized.py`

 * *Files identical despite different names*

### Comparing `medicraft-0.9.0/src/medicraft/datasets/prepare_dataset.py` & `medicraft-0.9.1/src/medicraft/datasets/prepare_dataset.py`

 * *Files identical despite different names*

### Comparing `medicraft-0.9.0/src/medicraft/datasets/preprocess.py` & `medicraft-0.9.1/src/medicraft/datasets/preprocess.py`

 * *Files identical despite different names*

### Comparing `medicraft-0.9.0/src/medicraft/experiments/local_run_experiment.py` & `medicraft-0.9.1/src/medicraft/experiments/local_run_experiment.py`

 * *Files identical despite different names*

### Comparing `medicraft-0.9.0/src/medicraft/experiments/old_run_experiment.py` & `medicraft-0.9.1/src/medicraft/experiments/old_run_experiment.py`

 * *Files identical despite different names*

### Comparing `medicraft-0.9.0/src/medicraft/experiments/test_run_experiment.py` & `medicraft-0.9.1/src/medicraft/experiments/test_run_experiment.py`

 * *Files identical despite different names*

### Comparing `medicraft-0.9.0/src/medicraft/generate_dataset_temp.py` & `medicraft-0.9.1/src/medicraft/generate_dataset_temp.py`

 * *Files identical despite different names*

### Comparing `medicraft-0.9.0/src/medicraft/generate_samples.py` & `medicraft-0.9.1/src/medicraft/generate_samples.py`

 * *Files identical despite different names*

### Comparing `medicraft-0.9.0/src/medicraft/main.py` & `medicraft-0.9.1/src/medicraft/main.py`

 * *Files identical despite different names*

### Comparing `medicraft-0.9.0/src/medicraft/models/classifier.py` & `medicraft-0.9.1/src/medicraft/models/classifier.py`

 * *Files identical despite different names*

### Comparing `medicraft-0.9.0/src/medicraft/models/gausian_diffusion.py` & `medicraft-0.9.1/src/medicraft/models/gausian_diffusion.py`

 * *Files identical despite different names*

### Comparing `medicraft-0.9.0/src/medicraft/pipeline/__init__.py` & `medicraft-0.9.1/src/medicraft/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `medicraft-0.9.0/src/medicraft/pipeline/blocks/data_dto.py` & `medicraft-0.9.1/src/medicraft/pipeline/blocks/data_dto.py`

 * *Files identical despite different names*

### Comparing `medicraft-0.9.0/src/medicraft/pipeline/blocks/experiment_dto.py` & `medicraft-0.9.1/src/medicraft/pipeline/blocks/experiment_dto.py`

 * *Files identical despite different names*

### Comparing `medicraft-0.9.0/src/medicraft/pipeline/parser.py` & `medicraft-0.9.1/src/medicraft/pipeline/parser.py`

 * *Files identical despite different names*

### Comparing `medicraft-0.9.0/src/medicraft/pipeline/pipeline.py` & `medicraft-0.9.1/src/medicraft/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `medicraft-0.9.0/src/medicraft/run_classification_experiment.py` & `medicraft-0.9.1/src/medicraft/run_classification_experiment.py`

 * *Files identical despite different names*

### Comparing `medicraft-0.9.0/src/medicraft/run_experiment.py` & `medicraft-0.9.1/src/medicraft/run_experiment.py`

 * *Files identical despite different names*

### Comparing `medicraft-0.9.0/src/medicraft/trackers/__init__.py` & `medicraft-0.9.1/src/medicraft/trackers/__init__.py`

 * *Files identical despite different names*

### Comparing `medicraft-0.9.0/src/medicraft/trackers/callbacks.py` & `medicraft-0.9.1/src/medicraft/trackers/callbacks.py`

 * *Files identical despite different names*

### Comparing `medicraft-0.9.0/src/medicraft/trackers/wandb.py` & `medicraft-0.9.1/src/medicraft/trackers/wandb.py`

 * *Files identical despite different names*

### Comparing `medicraft-0.9.0/src/medicraft/trainers/trainer.py` & `medicraft-0.9.1/src/medicraft/trainers/trainer.py`

 * *Files identical despite different names*

### Comparing `medicraft-0.9.0/src/medicraft/utils/files_managment.py` & `medicraft-0.9.1/src/medicraft/utils/files_managment.py`

 * *Files identical despite different names*

### Comparing `medicraft-0.9.0/src/medicraft/utils/transforms.py` & `medicraft-0.9.1/src/medicraft/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `medicraft-0.9.0/src/medicraft/validation/embeddings.py` & `medicraft-0.9.1/src/medicraft/validation/embeddings.py`

 * *Files identical despite different names*

