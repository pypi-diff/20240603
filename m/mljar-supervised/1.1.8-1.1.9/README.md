# Comparing `tmp/mljar-supervised-1.1.8.tar.gz` & `tmp/mljar-supervised-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mljar-supervised-1.1.8.tar", last modified: Wed May 22 12:58:33 2024, max compression
+gzip compressed data, was "mljar-supervised-1.1.9.tar", last modified: Mon Jun  3 11:49:43 2024, max compression
```

## Comparing `mljar-supervised-1.1.8.tar` & `mljar-supervised-1.1.9.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-22 12:58:33.169940 mljar-supervised-1.1.8/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1073 2022-03-28 10:53:20.000000 mljar-supervised-1.1.8/LICENSE
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       47 2021-09-02 08:06:45.000000 mljar-supervised-1.1.8/MANIFEST.in
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    26633 2024-05-22 12:58:33.165940 mljar-supervised-1.1.8/PKG-INFO
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    25845 2024-05-22 12:37:47.000000 mljar-supervised-1.1.8/README.md
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-22 12:58:33.161940 mljar-supervised-1.1.8/mljar_supervised.egg-info/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    26633 2024-05-22 12:58:33.000000 mljar-supervised-1.1.8/mljar_supervised.egg-info/PKG-INFO
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3493 2024-05-22 12:58:33.000000 mljar-supervised-1.1.8/mljar_supervised.egg-info/SOURCES.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        1 2024-05-22 12:58:33.000000 mljar-supervised-1.1.8/mljar_supervised.egg-info/dependency_links.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      325 2024-05-22 12:58:33.000000 mljar-supervised-1.1.8/mljar_supervised.egg-info/requires.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       11 2024-05-22 12:58:33.000000 mljar-supervised-1.1.8/mljar_supervised.egg-info/top_level.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      325 2024-04-10 12:35:04.000000 mljar-supervised-1.1.8/requirements.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       33 2023-09-21 12:45:57.000000 mljar-supervised-1.1.8/requirements_dev.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       38 2024-05-22 12:58:33.169940 mljar-supervised-1.1.8/setup.cfg
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1506 2024-05-22 12:57:56.000000 mljar-supervised-1.1.8/setup.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-22 12:58:33.161940 mljar-supervised-1.1.8/supervised/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       60 2024-05-22 12:58:01.000000 mljar-supervised-1.1.8/supervised/__init__.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-22 12:58:33.161940 mljar-supervised-1.1.8/supervised/algorithms/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2021-09-02 08:06:45.000000 mljar-supervised-1.1.8/supervised/algorithms/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4174 2023-09-20 06:26:40.000000 mljar-supervised-1.1.8/supervised/algorithms/algorithm.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2475 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/algorithms/baseline.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    14679 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/algorithms/catboost.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     9190 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/algorithms/decision_tree.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5161 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/algorithms/extra_trees.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      911 2023-12-01 11:37:16.000000 mljar-supervised-1.1.8/supervised/algorithms/factory.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3710 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/algorithms/knn.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    12349 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/algorithms/lightgbm.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5833 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/algorithms/linear.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4842 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/algorithms/nn.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5282 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/algorithms/random_forest.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2346 2024-03-04 09:46:14.000000 mljar-supervised-1.1.8/supervised/algorithms/registry.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6245 2023-12-01 11:37:16.000000 mljar-supervised-1.1.8/supervised/algorithms/sklearn.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    12532 2024-03-04 13:30:52.000000 mljar-supervised-1.1.8/supervised/algorithms/xgboost.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    26170 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/automl.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    99573 2024-05-22 12:50:25.000000 mljar-supervised-1.1.8/supervised/base_automl.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-22 12:58:33.161940 mljar-supervised-1.1.8/supervised/callbacks/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2021-09-02 08:06:45.000000 mljar-supervised-1.1.8/supervised/callbacks/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      592 2021-09-02 08:06:45.000000 mljar-supervised-1.1.8/supervised/callbacks/callback.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1027 2021-09-02 08:06:45.000000 mljar-supervised-1.1.8/supervised/callbacks/callback_list.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     9018 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/callbacks/early_stopping.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1701 2023-09-20 06:26:40.000000 mljar-supervised-1.1.8/supervised/callbacks/learner_time_constraint.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      568 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/callbacks/max_iters_constraint.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1847 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/callbacks/metric_logger.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      933 2023-09-20 06:26:40.000000 mljar-supervised-1.1.8/supervised/callbacks/terminate_on_nan.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3353 2023-09-20 06:26:40.000000 mljar-supervised-1.1.8/supervised/callbacks/total_time_constraint.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    22911 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/ensemble.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      547 2023-09-20 06:26:40.000000 mljar-supervised-1.1.8/supervised/exceptions.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-22 12:58:33.165940 mljar-supervised-1.1.8/supervised/fairness/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-06-26 08:29:57.000000 mljar-supervised-1.1.8/supervised/fairness/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    26141 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/fairness/metrics.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    15001 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/fairness/optimization.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4049 2023-06-26 11:40:40.000000 mljar-supervised-1.1.8/supervised/fairness/plots.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4975 2023-09-20 06:26:40.000000 mljar-supervised-1.1.8/supervised/fairness/report.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      701 2023-06-26 08:29:57.000000 mljar-supervised-1.1.8/supervised/fairness/utils.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    29288 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/model_framework.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-22 12:58:33.165940 mljar-supervised-1.1.8/supervised/preprocessing/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2021-09-02 08:06:45.000000 mljar-supervised-1.1.8/supervised/preprocessing/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3535 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/preprocessing/datetime_transformer.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    12603 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/preprocessing/eda.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      889 2023-12-01 11:37:16.000000 mljar-supervised-1.1.8/supervised/preprocessing/encoding_selector.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1488 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/preprocessing/exclude_missing_target.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    10807 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/preprocessing/goldenfeatures_transformer.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3819 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/preprocessing/kmeans_transformer.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2446 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/preprocessing/label_binarizer.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1793 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/preprocessing/label_encoder.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1555 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/preprocessing/loo_encoder.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    26388 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/preprocessing/preprocessing.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4616 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/preprocessing/preprocessing_categorical.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3737 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/preprocessing/preprocessing_missing.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4038 2021-09-02 08:06:45.000000 mljar-supervised-1.1.8/supervised/preprocessing/preprocessing_utils.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3646 2024-03-04 12:03:16.000000 mljar-supervised-1.1.8/supervised/preprocessing/scale.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2557 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/preprocessing/text_transformer.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-22 12:58:33.165940 mljar-supervised-1.1.8/supervised/tuner/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2021-09-02 08:06:45.000000 mljar-supervised-1.1.8/supervised/tuner/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2361 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/tuner/data_info.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2346 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/tuner/hill_climbing.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    59416 2024-03-04 11:50:15.000000 mljar-supervised-1.1.8/supervised/tuner/mljar_tuner.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-22 12:58:33.165940 mljar-supervised-1.1.8/supervised/tuner/optuna/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2021-09-02 08:06:45.000000 mljar-supervised-1.1.8/supervised/tuner/optuna/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5539 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/tuner/optuna/catboost.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2510 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/tuner/optuna/extra_trees.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1910 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/tuner/optuna/knn.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5896 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/tuner/optuna/lightgbm.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2122 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/tuner/optuna/nn.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2511 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/tuner/optuna/random_forest.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    11606 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/tuner/optuna/tuner.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4727 2024-03-04 13:31:00.000000 mljar-supervised-1.1.8/supervised/tuner/optuna/xgboost.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6273 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/tuner/preprocessing_tuner.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      564 2021-09-02 08:06:45.000000 mljar-supervised-1.1.8/supervised/tuner/random_parameters.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     8944 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/tuner/time_controller.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-22 12:58:33.165940 mljar-supervised-1.1.8/supervised/utils/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      259 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/utils/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    37054 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/utils/additional_metrics.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     8148 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/utils/additional_plots.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5352 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/utils/automl_plots.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1052 2021-09-02 08:06:45.000000 mljar-supervised-1.1.8/supervised/utils/common.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      524 2023-09-21 12:19:11.000000 mljar-supervised-1.1.8/supervised/utils/config.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      173 2021-09-02 08:06:45.000000 mljar-supervised-1.1.8/supervised/utils/constants.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1481 2023-06-26 11:40:40.000000 mljar-supervised-1.1.8/supervised/utils/data_validation.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3015 2024-03-04 10:30:50.000000 mljar-supervised-1.1.8/supervised/utils/importance.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      823 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/utils/jsonencoder.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4951 2023-09-20 06:26:40.000000 mljar-supervised-1.1.8/supervised/utils/leaderboard_plots.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4972 2024-03-04 12:16:25.000000 mljar-supervised-1.1.8/supervised/utils/learning_curves.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    13465 2024-03-04 11:46:43.000000 mljar-supervised-1.1.8/supervised/utils/metric.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    12128 2024-03-04 11:50:51.000000 mljar-supervised-1.1.8/supervised/utils/shap.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      424 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/utils/subsample.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      589 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/utils/utils.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-22 12:58:33.165940 mljar-supervised-1.1.8/supervised/validation/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2021-09-02 08:06:45.000000 mljar-supervised-1.1.8/supervised/validation/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1210 2023-09-20 06:26:41.000000 mljar-supervised-1.1.8/supervised/validation/validation_step.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      264 2021-09-02 08:06:45.000000 mljar-supervised-1.1.8/supervised/validation/validator_base.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4075 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/validation/validator_custom.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5505 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/validation/validator_kfold.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4708 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/validation/validator_split.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-06-03 11:49:43.112759 mljar-supervised-1.1.9/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1073 2022-03-28 10:53:20.000000 mljar-supervised-1.1.9/LICENSE
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       47 2021-09-02 08:06:45.000000 mljar-supervised-1.1.9/MANIFEST.in
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    26633 2024-06-03 11:49:43.112759 mljar-supervised-1.1.9/PKG-INFO
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    25845 2024-05-22 12:37:47.000000 mljar-supervised-1.1.9/README.md
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-06-03 11:49:43.104759 mljar-supervised-1.1.9/mljar_supervised.egg-info/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    26633 2024-06-03 11:49:43.000000 mljar-supervised-1.1.9/mljar_supervised.egg-info/PKG-INFO
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3493 2024-06-03 11:49:43.000000 mljar-supervised-1.1.9/mljar_supervised.egg-info/SOURCES.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        1 2024-06-03 11:49:43.000000 mljar-supervised-1.1.9/mljar_supervised.egg-info/dependency_links.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      326 2024-06-03 11:49:43.000000 mljar-supervised-1.1.9/mljar_supervised.egg-info/requires.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       11 2024-06-03 11:49:43.000000 mljar-supervised-1.1.9/mljar_supervised.egg-info/top_level.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      326 2024-06-03 11:46:54.000000 mljar-supervised-1.1.9/requirements.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       33 2023-09-21 12:45:57.000000 mljar-supervised-1.1.9/requirements_dev.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       38 2024-06-03 11:49:43.112759 mljar-supervised-1.1.9/setup.cfg
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1506 2024-06-03 11:47:45.000000 mljar-supervised-1.1.9/setup.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-06-03 11:49:43.108759 mljar-supervised-1.1.9/supervised/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       60 2024-06-03 11:47:50.000000 mljar-supervised-1.1.9/supervised/__init__.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-06-03 11:49:43.108759 mljar-supervised-1.1.9/supervised/algorithms/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2021-09-02 08:06:45.000000 mljar-supervised-1.1.9/supervised/algorithms/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4174 2023-09-20 06:26:40.000000 mljar-supervised-1.1.9/supervised/algorithms/algorithm.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2475 2024-03-01 11:22:55.000000 mljar-supervised-1.1.9/supervised/algorithms/baseline.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    14679 2024-03-01 11:22:55.000000 mljar-supervised-1.1.9/supervised/algorithms/catboost.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     9190 2024-03-01 11:22:55.000000 mljar-supervised-1.1.9/supervised/algorithms/decision_tree.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5161 2024-03-01 11:22:55.000000 mljar-supervised-1.1.9/supervised/algorithms/extra_trees.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      911 2023-12-01 11:37:16.000000 mljar-supervised-1.1.9/supervised/algorithms/factory.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3710 2024-06-03 09:35:47.000000 mljar-supervised-1.1.9/supervised/algorithms/knn.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    12349 2024-03-01 11:22:55.000000 mljar-supervised-1.1.9/supervised/algorithms/lightgbm.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5833 2024-03-01 11:22:55.000000 mljar-supervised-1.1.9/supervised/algorithms/linear.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4842 2024-03-01 11:22:55.000000 mljar-supervised-1.1.9/supervised/algorithms/nn.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5282 2024-03-01 11:22:55.000000 mljar-supervised-1.1.9/supervised/algorithms/random_forest.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2346 2024-03-04 09:46:14.000000 mljar-supervised-1.1.9/supervised/algorithms/registry.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6245 2023-12-01 11:37:16.000000 mljar-supervised-1.1.9/supervised/algorithms/sklearn.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    12532 2024-03-04 13:30:52.000000 mljar-supervised-1.1.9/supervised/algorithms/xgboost.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    26170 2024-03-01 11:22:55.000000 mljar-supervised-1.1.9/supervised/automl.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    99573 2024-05-22 12:50:25.000000 mljar-supervised-1.1.9/supervised/base_automl.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-06-03 11:49:43.108759 mljar-supervised-1.1.9/supervised/callbacks/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2021-09-02 08:06:45.000000 mljar-supervised-1.1.9/supervised/callbacks/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      592 2021-09-02 08:06:45.000000 mljar-supervised-1.1.9/supervised/callbacks/callback.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1027 2021-09-02 08:06:45.000000 mljar-supervised-1.1.9/supervised/callbacks/callback_list.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     9018 2024-03-01 11:22:55.000000 mljar-supervised-1.1.9/supervised/callbacks/early_stopping.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1701 2023-09-20 06:26:40.000000 mljar-supervised-1.1.9/supervised/callbacks/learner_time_constraint.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      568 2024-03-01 11:22:55.000000 mljar-supervised-1.1.9/supervised/callbacks/max_iters_constraint.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1847 2024-03-01 11:22:55.000000 mljar-supervised-1.1.9/supervised/callbacks/metric_logger.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      933 2023-09-20 06:26:40.000000 mljar-supervised-1.1.9/supervised/callbacks/terminate_on_nan.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3353 2023-09-20 06:26:40.000000 mljar-supervised-1.1.9/supervised/callbacks/total_time_constraint.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    22911 2024-03-01 11:22:55.000000 mljar-supervised-1.1.9/supervised/ensemble.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      547 2023-09-20 06:26:40.000000 mljar-supervised-1.1.9/supervised/exceptions.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-06-03 11:49:43.108759 mljar-supervised-1.1.9/supervised/fairness/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-06-26 08:29:57.000000 mljar-supervised-1.1.9/supervised/fairness/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    26141 2024-03-01 11:22:55.000000 mljar-supervised-1.1.9/supervised/fairness/metrics.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    15001 2024-03-01 11:22:55.000000 mljar-supervised-1.1.9/supervised/fairness/optimization.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4049 2023-06-26 11:40:40.000000 mljar-supervised-1.1.9/supervised/fairness/plots.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4975 2023-09-20 06:26:40.000000 mljar-supervised-1.1.9/supervised/fairness/report.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      701 2023-06-26 08:29:57.000000 mljar-supervised-1.1.9/supervised/fairness/utils.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    29288 2024-06-03 11:46:21.000000 mljar-supervised-1.1.9/supervised/model_framework.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-06-03 11:49:43.108759 mljar-supervised-1.1.9/supervised/preprocessing/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2021-09-02 08:06:45.000000 mljar-supervised-1.1.9/supervised/preprocessing/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3535 2024-03-01 11:22:55.000000 mljar-supervised-1.1.9/supervised/preprocessing/datetime_transformer.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    12603 2024-03-01 11:22:55.000000 mljar-supervised-1.1.9/supervised/preprocessing/eda.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      889 2023-12-01 11:37:16.000000 mljar-supervised-1.1.9/supervised/preprocessing/encoding_selector.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1488 2024-03-01 11:22:55.000000 mljar-supervised-1.1.9/supervised/preprocessing/exclude_missing_target.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    10807 2024-03-01 11:22:55.000000 mljar-supervised-1.1.9/supervised/preprocessing/goldenfeatures_transformer.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3819 2024-03-01 11:22:55.000000 mljar-supervised-1.1.9/supervised/preprocessing/kmeans_transformer.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2446 2024-03-01 11:22:55.000000 mljar-supervised-1.1.9/supervised/preprocessing/label_binarizer.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1793 2024-03-01 11:22:55.000000 mljar-supervised-1.1.9/supervised/preprocessing/label_encoder.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1555 2024-03-01 11:22:55.000000 mljar-supervised-1.1.9/supervised/preprocessing/loo_encoder.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    26388 2024-03-01 11:22:55.000000 mljar-supervised-1.1.9/supervised/preprocessing/preprocessing.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4616 2024-03-01 11:22:55.000000 mljar-supervised-1.1.9/supervised/preprocessing/preprocessing_categorical.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3737 2024-03-01 11:22:55.000000 mljar-supervised-1.1.9/supervised/preprocessing/preprocessing_missing.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4038 2021-09-02 08:06:45.000000 mljar-supervised-1.1.9/supervised/preprocessing/preprocessing_utils.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3646 2024-03-04 12:03:16.000000 mljar-supervised-1.1.9/supervised/preprocessing/scale.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2557 2024-03-01 11:22:55.000000 mljar-supervised-1.1.9/supervised/preprocessing/text_transformer.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-06-03 11:49:43.108759 mljar-supervised-1.1.9/supervised/tuner/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2021-09-02 08:06:45.000000 mljar-supervised-1.1.9/supervised/tuner/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2361 2024-03-01 11:22:55.000000 mljar-supervised-1.1.9/supervised/tuner/data_info.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2346 2024-03-01 11:22:55.000000 mljar-supervised-1.1.9/supervised/tuner/hill_climbing.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    59699 2024-06-03 09:17:14.000000 mljar-supervised-1.1.9/supervised/tuner/mljar_tuner.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-06-03 11:49:43.108759 mljar-supervised-1.1.9/supervised/tuner/optuna/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2021-09-02 08:06:45.000000 mljar-supervised-1.1.9/supervised/tuner/optuna/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5539 2024-03-01 11:22:55.000000 mljar-supervised-1.1.9/supervised/tuner/optuna/catboost.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2510 2024-03-01 11:22:55.000000 mljar-supervised-1.1.9/supervised/tuner/optuna/extra_trees.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1910 2024-03-01 11:22:55.000000 mljar-supervised-1.1.9/supervised/tuner/optuna/knn.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5896 2024-03-01 11:22:55.000000 mljar-supervised-1.1.9/supervised/tuner/optuna/lightgbm.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2122 2024-03-01 11:22:55.000000 mljar-supervised-1.1.9/supervised/tuner/optuna/nn.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2511 2024-03-01 11:22:55.000000 mljar-supervised-1.1.9/supervised/tuner/optuna/random_forest.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    11606 2024-03-01 11:22:55.000000 mljar-supervised-1.1.9/supervised/tuner/optuna/tuner.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4727 2024-03-04 13:31:00.000000 mljar-supervised-1.1.9/supervised/tuner/optuna/xgboost.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6273 2024-03-01 11:22:55.000000 mljar-supervised-1.1.9/supervised/tuner/preprocessing_tuner.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      564 2021-09-02 08:06:45.000000 mljar-supervised-1.1.9/supervised/tuner/random_parameters.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     8944 2024-03-01 11:22:55.000000 mljar-supervised-1.1.9/supervised/tuner/time_controller.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-06-03 11:49:43.112759 mljar-supervised-1.1.9/supervised/utils/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      259 2024-03-01 11:22:55.000000 mljar-supervised-1.1.9/supervised/utils/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    37054 2024-06-03 11:46:21.000000 mljar-supervised-1.1.9/supervised/utils/additional_metrics.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     8148 2024-06-03 11:46:21.000000 mljar-supervised-1.1.9/supervised/utils/additional_plots.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5352 2024-03-01 11:22:55.000000 mljar-supervised-1.1.9/supervised/utils/automl_plots.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1052 2021-09-02 08:06:45.000000 mljar-supervised-1.1.9/supervised/utils/common.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      524 2024-06-03 11:46:21.000000 mljar-supervised-1.1.9/supervised/utils/config.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      173 2021-09-02 08:06:45.000000 mljar-supervised-1.1.9/supervised/utils/constants.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1481 2023-06-26 11:40:40.000000 mljar-supervised-1.1.9/supervised/utils/data_validation.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3015 2024-06-03 11:46:21.000000 mljar-supervised-1.1.9/supervised/utils/importance.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      823 2024-03-01 11:22:55.000000 mljar-supervised-1.1.9/supervised/utils/jsonencoder.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4951 2023-09-20 06:26:40.000000 mljar-supervised-1.1.9/supervised/utils/leaderboard_plots.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4972 2024-03-04 12:16:25.000000 mljar-supervised-1.1.9/supervised/utils/learning_curves.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    13242 2024-06-03 11:46:37.000000 mljar-supervised-1.1.9/supervised/utils/metric.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    12128 2024-03-04 11:50:51.000000 mljar-supervised-1.1.9/supervised/utils/shap.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      424 2024-03-01 11:22:55.000000 mljar-supervised-1.1.9/supervised/utils/subsample.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      589 2024-03-01 11:22:55.000000 mljar-supervised-1.1.9/supervised/utils/utils.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-06-03 11:49:43.112759 mljar-supervised-1.1.9/supervised/validation/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2021-09-02 08:06:45.000000 mljar-supervised-1.1.9/supervised/validation/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1210 2023-09-20 06:26:41.000000 mljar-supervised-1.1.9/supervised/validation/validation_step.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      264 2021-09-02 08:06:45.000000 mljar-supervised-1.1.9/supervised/validation/validator_base.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4087 2024-06-03 09:16:43.000000 mljar-supervised-1.1.9/supervised/validation/validator_custom.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5505 2024-03-01 11:22:55.000000 mljar-supervised-1.1.9/supervised/validation/validator_kfold.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4708 2024-03-01 11:22:55.000000 mljar-supervised-1.1.9/supervised/validation/validator_split.py
```

### Comparing `mljar-supervised-1.1.8/LICENSE` & `mljar-supervised-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/PKG-INFO` & `mljar-supervised-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mljar-supervised
-Version: 1.1.8
+Version: 1.1.9
 Summary: Automated Machine Learning for Humans
 Home-page: https://github.com/mljar/mljar-supervised
 Author: MLJAR, Sp. z o.o.
 Author-email: contact@mljar.com
 License: MIT
 Keywords: automated machine learning,automl,machine learning,data science,data mining,mljar,random forest,decision tree,xgboost,lightgbm,catboost,neural network,extra trees,linear model,features selection,features engineering
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mljar-supervised Version: 1.1.8 Summary: Automated
+Metadata-Version: 2.1 Name: mljar-supervised Version: 1.1.9 Summary: Automated
 Machine Learning for Humans Home-page: https://github.com/mljar/mljar-
 supervised Author: MLJAR, Sp. z o.o. Author-email: contact@mljar.com License:
 MIT Keywords: automated machine learning,automl,machine learning,data
 science,data mining,mljar,random forest,decision
 tree,xgboost,lightgbm,catboost,neural network,extra trees,linear model,features
 selection,features engineering Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
```

### Comparing `mljar-supervised-1.1.8/README.md` & `mljar-supervised-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/mljar_supervised.egg-info/PKG-INFO` & `mljar-supervised-1.1.9/mljar_supervised.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mljar-supervised
-Version: 1.1.8
+Version: 1.1.9
 Summary: Automated Machine Learning for Humans
 Home-page: https://github.com/mljar/mljar-supervised
 Author: MLJAR, Sp. z o.o.
 Author-email: contact@mljar.com
 License: MIT
 Keywords: automated machine learning,automl,machine learning,data science,data mining,mljar,random forest,decision tree,xgboost,lightgbm,catboost,neural network,extra trees,linear model,features selection,features engineering
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mljar-supervised Version: 1.1.8 Summary: Automated
+Metadata-Version: 2.1 Name: mljar-supervised Version: 1.1.9 Summary: Automated
 Machine Learning for Humans Home-page: https://github.com/mljar/mljar-
 supervised Author: MLJAR, Sp. z o.o. Author-email: contact@mljar.com License:
 MIT Keywords: automated machine learning,automl,machine learning,data
 science,data mining,mljar,random forest,decision
 tree,xgboost,lightgbm,catboost,neural network,extra trees,linear model,features
 selection,features engineering Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
```

### Comparing `mljar-supervised-1.1.8/mljar_supervised.egg-info/SOURCES.txt` & `mljar-supervised-1.1.9/mljar_supervised.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/setup.py` & `mljar-supervised-1.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="mljar-supervised",
-    version="1.1.8",
+    version="1.1.9",
     description="Automated Machine Learning for Humans",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mljar/mljar-supervised",
     author="MLJAR, Sp. z o.o.",
     author_email="contact@mljar.com",
     license="MIT",
```

### Comparing `mljar-supervised-1.1.8/supervised/algorithms/algorithm.py` & `mljar-supervised-1.1.9/supervised/algorithms/algorithm.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/algorithms/baseline.py` & `mljar-supervised-1.1.9/supervised/algorithms/baseline.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/algorithms/catboost.py` & `mljar-supervised-1.1.9/supervised/algorithms/catboost.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/algorithms/decision_tree.py` & `mljar-supervised-1.1.9/supervised/algorithms/decision_tree.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/algorithms/extra_trees.py` & `mljar-supervised-1.1.9/supervised/algorithms/extra_trees.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/algorithms/factory.py` & `mljar-supervised-1.1.9/supervised/algorithms/factory.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/algorithms/knn.py` & `mljar-supervised-1.1.9/supervised/algorithms/knn.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/algorithms/lightgbm.py` & `mljar-supervised-1.1.9/supervised/algorithms/lightgbm.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/algorithms/linear.py` & `mljar-supervised-1.1.9/supervised/algorithms/linear.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/algorithms/nn.py` & `mljar-supervised-1.1.9/supervised/algorithms/nn.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/algorithms/random_forest.py` & `mljar-supervised-1.1.9/supervised/algorithms/random_forest.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/algorithms/registry.py` & `mljar-supervised-1.1.9/supervised/algorithms/registry.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/algorithms/sklearn.py` & `mljar-supervised-1.1.9/supervised/algorithms/sklearn.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/algorithms/xgboost.py` & `mljar-supervised-1.1.9/supervised/algorithms/xgboost.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/automl.py` & `mljar-supervised-1.1.9/supervised/automl.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/base_automl.py` & `mljar-supervised-1.1.9/supervised/base_automl.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/callbacks/callback.py` & `mljar-supervised-1.1.9/supervised/callbacks/callback.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/callbacks/callback_list.py` & `mljar-supervised-1.1.9/supervised/callbacks/callback_list.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/callbacks/early_stopping.py` & `mljar-supervised-1.1.9/supervised/callbacks/early_stopping.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/callbacks/learner_time_constraint.py` & `mljar-supervised-1.1.9/supervised/callbacks/learner_time_constraint.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/callbacks/max_iters_constraint.py` & `mljar-supervised-1.1.9/supervised/callbacks/max_iters_constraint.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/callbacks/metric_logger.py` & `mljar-supervised-1.1.9/supervised/callbacks/metric_logger.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/callbacks/terminate_on_nan.py` & `mljar-supervised-1.1.9/supervised/callbacks/terminate_on_nan.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/callbacks/total_time_constraint.py` & `mljar-supervised-1.1.9/supervised/callbacks/total_time_constraint.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/ensemble.py` & `mljar-supervised-1.1.9/supervised/ensemble.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/exceptions.py` & `mljar-supervised-1.1.9/supervised/exceptions.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/fairness/metrics.py` & `mljar-supervised-1.1.9/supervised/fairness/metrics.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/fairness/optimization.py` & `mljar-supervised-1.1.9/supervised/fairness/optimization.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/fairness/plots.py` & `mljar-supervised-1.1.9/supervised/fairness/plots.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/fairness/report.py` & `mljar-supervised-1.1.9/supervised/fairness/report.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/fairness/utils.py` & `mljar-supervised-1.1.9/supervised/fairness/utils.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/model_framework.py` & `mljar-supervised-1.1.9/supervised/model_framework.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/preprocessing/datetime_transformer.py` & `mljar-supervised-1.1.9/supervised/preprocessing/datetime_transformer.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/preprocessing/eda.py` & `mljar-supervised-1.1.9/supervised/preprocessing/eda.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/preprocessing/encoding_selector.py` & `mljar-supervised-1.1.9/supervised/preprocessing/encoding_selector.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/preprocessing/exclude_missing_target.py` & `mljar-supervised-1.1.9/supervised/preprocessing/exclude_missing_target.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/preprocessing/goldenfeatures_transformer.py` & `mljar-supervised-1.1.9/supervised/preprocessing/goldenfeatures_transformer.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/preprocessing/kmeans_transformer.py` & `mljar-supervised-1.1.9/supervised/preprocessing/kmeans_transformer.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/preprocessing/label_binarizer.py` & `mljar-supervised-1.1.9/supervised/preprocessing/label_binarizer.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/preprocessing/label_encoder.py` & `mljar-supervised-1.1.9/supervised/preprocessing/label_encoder.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/preprocessing/loo_encoder.py` & `mljar-supervised-1.1.9/supervised/preprocessing/loo_encoder.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/preprocessing/preprocessing.py` & `mljar-supervised-1.1.9/supervised/preprocessing/preprocessing.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/preprocessing/preprocessing_categorical.py` & `mljar-supervised-1.1.9/supervised/preprocessing/preprocessing_categorical.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/preprocessing/preprocessing_missing.py` & `mljar-supervised-1.1.9/supervised/preprocessing/preprocessing_missing.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/preprocessing/preprocessing_utils.py` & `mljar-supervised-1.1.9/supervised/preprocessing/preprocessing_utils.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/preprocessing/scale.py` & `mljar-supervised-1.1.9/supervised/preprocessing/scale.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/preprocessing/text_transformer.py` & `mljar-supervised-1.1.9/supervised/preprocessing/text_transformer.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/tuner/data_info.py` & `mljar-supervised-1.1.9/supervised/tuner/data_info.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/tuner/hill_climbing.py` & `mljar-supervised-1.1.9/supervised/tuner/hill_climbing.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/tuner/mljar_tuner.py` & `mljar-supervised-1.1.9/supervised/tuner/mljar_tuner.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,16 +177,22 @@
         if self._kmeans_features and self._can_apply_kmeans_features():
             all_steps += ["kmeans_features"]
         if self._features_selection:
             all_steps += ["insert_random_feature"]
             all_steps += ["features_selection"]
         for i in range(self._hill_climbing_steps):
             all_steps += [f"hill_climbing_{i+1}"]
-        if self._boost_on_errors and self._fairness_metric is None:
-            # we can tun boost on errors only if there is not fairness optimization
+        if (
+            self._boost_on_errors
+            and self._fairness_metric is None
+            and self._validation_strategy.get("validation_type", "") != "custom"
+        ):
+            # we can turn boost on errors only if there is not fairness optimization
+            # boost on errors will not work for custom validation strategy
+            # because we cant assure that we have all samples in out-of-folds predictions
             all_steps += ["boost_on_errors"]
         if self._train_ensemble:
             all_steps += ["ensemble"]
         if self._stack_models:
             all_steps += ["stack"]
             if self._train_ensemble:
                 all_steps += ["ensemble_stacked"]
```

### Comparing `mljar-supervised-1.1.8/supervised/tuner/optuna/catboost.py` & `mljar-supervised-1.1.9/supervised/tuner/optuna/catboost.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/tuner/optuna/extra_trees.py` & `mljar-supervised-1.1.9/supervised/tuner/optuna/extra_trees.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/tuner/optuna/knn.py` & `mljar-supervised-1.1.9/supervised/tuner/optuna/knn.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/tuner/optuna/lightgbm.py` & `mljar-supervised-1.1.9/supervised/tuner/optuna/lightgbm.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/tuner/optuna/nn.py` & `mljar-supervised-1.1.9/supervised/tuner/optuna/nn.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/tuner/optuna/random_forest.py` & `mljar-supervised-1.1.9/supervised/tuner/optuna/random_forest.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/tuner/optuna/tuner.py` & `mljar-supervised-1.1.9/supervised/tuner/optuna/tuner.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/tuner/optuna/xgboost.py` & `mljar-supervised-1.1.9/supervised/tuner/optuna/xgboost.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/tuner/preprocessing_tuner.py` & `mljar-supervised-1.1.9/supervised/tuner/preprocessing_tuner.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/tuner/random_parameters.py` & `mljar-supervised-1.1.9/supervised/tuner/random_parameters.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/tuner/time_controller.py` & `mljar-supervised-1.1.9/supervised/tuner/time_controller.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/utils/additional_metrics.py` & `mljar-supervised-1.1.9/supervised/utils/additional_metrics.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/utils/additional_plots.py` & `mljar-supervised-1.1.9/supervised/utils/additional_plots.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/utils/automl_plots.py` & `mljar-supervised-1.1.9/supervised/utils/automl_plots.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/utils/common.py` & `mljar-supervised-1.1.9/supervised/utils/common.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/utils/config.py` & `mljar-supervised-1.1.9/supervised/utils/config.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/utils/data_validation.py` & `mljar-supervised-1.1.9/supervised/utils/data_validation.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/utils/importance.py` & `mljar-supervised-1.1.9/supervised/utils/importance.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/utils/jsonencoder.py` & `mljar-supervised-1.1.9/supervised/utils/jsonencoder.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/utils/leaderboard_plots.py` & `mljar-supervised-1.1.9/supervised/utils/leaderboard_plots.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/utils/learning_curves.py` & `mljar-supervised-1.1.9/supervised/utils/learning_curves.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/utils/metric.py` & `mljar-supervised-1.1.9/supervised/utils/metric.py`

 * *Files 2% similar despite different names*

```diff
@@ -221,20 +221,14 @@
     return "average_precision", -negative_average_precision(target, preds, weight), True
 
 
 def lightgbm_eval_metric_accuracy(preds, dtrain):
     target = dtrain.get_label()
     weight = dtrain.get_weight()
 
-    unique_targets = np.unique(target)
-    if len(unique_targets) > 2:
-        cols = len(unique_targets)
-        rows = int(preds.shape[0] / len(unique_targets))
-        preds = np.reshape(preds, (rows, cols), order="F")
-
     return "accuracy", -negative_accuracy(target, preds, weight), True
 
 
 class CatBoostEvalMetricSpearman(object):
     def get_final_error(self, error, weight):
         return error
```

### Comparing `mljar-supervised-1.1.8/supervised/utils/shap.py` & `mljar-supervised-1.1.9/supervised/utils/shap.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/utils/utils.py` & `mljar-supervised-1.1.9/supervised/utils/utils.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/validation/validation_step.py` & `mljar-supervised-1.1.9/supervised/validation/validation_step.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/validation/validator_custom.py` & `mljar-supervised-1.1.9/supervised/validation/validator_custom.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
             if self._sensitive_features_path is not None:
                 sensitive_features = load_data(self._sensitive_features_path)
 
             train_data = {"X": X.iloc[train_index], "y": y.iloc[train_index]}
             validation_data = {
                 "X": X.iloc[validation_index],
                 "y": y.iloc[validation_index],
-            }
+            }            
             if sample_weight is not None:
                 train_data["sample_weight"] = sample_weight.iloc[train_index]
                 validation_data["sample_weight"] = sample_weight.iloc[validation_index]
             if sensitive_features is not None:
                 train_data["sensitive_features"] = sensitive_features.iloc[train_index]
                 validation_data["sensitive_features"] = sensitive_features.iloc[
                     validation_index
```

### Comparing `mljar-supervised-1.1.8/supervised/validation/validator_kfold.py` & `mljar-supervised-1.1.9/supervised/validation/validator_kfold.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.8/supervised/validation/validator_split.py` & `mljar-supervised-1.1.9/supervised/validation/validator_split.py`

 * *Files identical despite different names*

