# Comparing `tmp/um6p_cc_learn-0.2.3.tar.gz` & `tmp/um6p_cc_learn-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "um6p_cc_learn-0.2.3.tar", last modified: Mon Jun  3 03:38:47 2024, max compression
+gzip compressed data, was "um6p_cc_learn-0.2.4.tar", last modified: Mon Jun  3 03:42:05 2024, max compression
```

## Comparing `um6p_cc_learn-0.2.3.tar` & `um6p_cc_learn-0.2.4.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxrwxrwx   0        0        0        0 2024-06-03 03:38:47.531803 um6p_cc_learn-0.2.3/
--rw-rw-rw-   0        0        0      435 2024-06-03 03:38:47.528862 um6p_cc_learn-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-06-03 03:38:47.531803 um6p_cc_learn-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0      584 2024-06-03 03:38:40.000000 um6p_cc_learn-0.2.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-06-03 03:38:46.812706 um6p_cc_learn-0.2.3/um6p_CC_learn/
--rw-rw-rw-   0        0        0       67 2024-06-03 03:20:37.000000 um6p_cc_learn-0.2.3/um6p_CC_learn/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-03 03:38:46.859694 um6p_cc_learn-0.2.3/um6p_CC_learn/base/
--rw-rw-rw-   0        0        0        0 2024-05-10 23:42:45.000000 um6p_cc_learn-0.2.3/um6p_CC_learn/base/__init__.py
--rw-rw-rw-   0        0        0     1573 2024-06-03 03:29:23.000000 um6p_cc_learn-0.2.3/um6p_CC_learn/base/base.py
-drwxrwxrwx   0        0        0        0 2024-06-03 03:38:46.878186 um6p_cc_learn-0.2.3/um6p_CC_learn/decomposition/
--rw-rw-rw-   0        0        0        0 2024-05-10 23:53:18.000000 um6p_cc_learn-0.2.3/um6p_CC_learn/decomposition/__init__.py
--rw-rw-rw-   0        0        0      925 2024-06-03 03:29:33.000000 um6p_cc_learn-0.2.3/um6p_CC_learn/decomposition/pca.py
-drwxrwxrwx   0        0        0        0 2024-06-03 03:38:46.955349 um6p_cc_learn-0.2.3/um6p_CC_learn/ensemble/
--rw-rw-rw-   0        0        0        0 2024-05-11 00:04:22.000000 um6p_cc_learn-0.2.3/um6p_CC_learn/ensemble/__init__.py
--rw-rw-rw-   0        0        0     2747 2024-06-03 03:29:46.000000 um6p_cc_learn-0.2.3/um6p_CC_learn/ensemble/bagging.py
--rw-rw-rw-   0        0        0     5548 2024-06-03 03:29:55.000000 um6p_cc_learn-0.2.3/um6p_CC_learn/ensemble/boosting.py
--rw-rw-rw-   0        0        0     7499 2024-06-03 03:30:01.000000 um6p_cc_learn-0.2.3/um6p_CC_learn/ensemble/random_forest.py
--rw-rw-rw-   0        0        0     2543 2024-06-03 03:30:09.000000 um6p_cc_learn-0.2.3/um6p_CC_learn/ensemble/stacking.py
--rw-rw-rw-   0        0        0     1885 2024-06-03 03:30:14.000000 um6p_cc_learn-0.2.3/um6p_CC_learn/ensemble/voting.py
-drwxrwxrwx   0        0        0        0 2024-06-03 03:38:47.027577 um6p_cc_learn-0.2.3/um6p_CC_learn/feature_selection/
--rw-rw-rw-   0        0        0     2686 2024-06-03 03:30:21.000000 um6p_cc_learn-0.2.3/um6p_CC_learn/feature_selection/RFE.py
--rw-rw-rw-   0        0        0        0 2024-05-10 23:52:02.000000 um6p_cc_learn-0.2.3/um6p_CC_learn/feature_selection/__init__.py
--rw-rw-rw-   0        0        0     2354 2024-06-03 03:30:26.000000 um6p_cc_learn-0.2.3/um6p_CC_learn/feature_selection/select_from_model.py
--rw-rw-rw-   0        0        0     1599 2024-06-03 03:30:30.000000 um6p_cc_learn-0.2.3/um6p_CC_learn/feature_selection/variance_threshold.py
-drwxrwxrwx   0        0        0        0 2024-06-03 03:38:47.085347 um6p_cc_learn-0.2.3/um6p_CC_learn/linear_model/
--rw-rw-rw-   0        0        0        0 2024-05-11 00:01:31.000000 um6p_cc_learn-0.2.3/um6p_CC_learn/linear_model/__init__.py
--rw-rw-rw-   0        0        0     3810 2024-06-03 03:30:37.000000 um6p_cc_learn-0.2.3/um6p_CC_learn/linear_model/logistic_regression.py
--rw-rw-rw-   0        0        0     1667 2024-06-03 03:30:41.000000 um6p_cc_learn-0.2.3/um6p_CC_learn/linear_model/regression.py
-drwxrwxrwx   0        0        0        0 2024-06-03 03:38:47.156436 um6p_cc_learn-0.2.3/um6p_CC_learn/metrics/
--rw-rw-rw-   0        0        0        0 2024-05-11 21:32:29.000000 um6p_cc_learn-0.2.3/um6p_CC_learn/metrics/__init__.py
--rw-rw-rw-   0        0        0     1041 2024-06-03 02:23:05.000000 um6p_cc_learn-0.2.3/um6p_CC_learn/metrics/auc.py
--rw-rw-rw-   0        0        0     3480 2024-05-11 14:50:11.000000 um6p_cc_learn-0.2.3/um6p_CC_learn/metrics/classification.py
--rw-rw-rw-   0        0        0      299 2024-06-03 03:31:10.000000 um6p_cc_learn-0.2.3/um6p_CC_learn/metrics/cosine_distances.py
--rw-rw-rw-   0        0        0      784 2024-05-11 14:51:52.000000 um6p_cc_learn-0.2.3/um6p_CC_learn/metrics/cosine_similarity.py
--rw-rw-rw-   0        0        0     1335 2024-06-03 02:23:05.000000 um6p_cc_learn-0.2.3/um6p_CC_learn/metrics/euclidian_distances.py
--rw-rw-rw-   0        0        0      398 2024-06-02 16:33:57.000000 um6p_cc_learn-0.2.3/um6p_CC_learn/metrics/regression.py
--rw-rw-rw-   0        0        0      859 2024-06-03 03:31:39.000000 um6p_cc_learn-0.2.3/um6p_CC_learn/metrics/roc_auc_score.py
--rw-rw-rw-   0        0        0      653 2024-05-11 15:25:20.000000 um6p_cc_learn-0.2.3/um6p_CC_learn/metrics/roc_curve.py
-drwxrwxrwx   0        0        0        0 2024-06-03 03:38:47.203592 um6p_cc_learn-0.2.3/um6p_CC_learn/model_selection/
--rw-rw-rw-   0        0        0     2710 2024-06-03 03:32:07.000000 um6p_cc_learn-0.2.3/um6p_CC_learn/model_selection/GridSearch.py
--rw-rw-rw-   0        0        0        0 2024-05-10 23:59:54.000000 um6p_cc_learn-0.2.3/um6p_CC_learn/model_selection/__init__.py
--rw-rw-rw-   0        0        0     4804 2024-06-03 02:43:18.000000 um6p_cc_learn-0.2.3/um6p_CC_learn/model_selection/__split.py
--rw-rw-rw-   0        0        0      746 2024-06-03 03:31:56.000000 um6p_cc_learn-0.2.3/um6p_CC_learn/model_selection/__validation.py
--rw-rw-rw-   0        0        0     3847 2024-06-03 03:38:24.000000 um6p_cc_learn-0.2.3/um6p_CC_learn/naive_bayes.py
-drwxrwxrwx   0        0        0        0 2024-06-03 03:38:47.228293 um6p_cc_learn-0.2.3/um6p_CC_learn/neural_network/
--rw-rw-rw-   0        0        0        0 2024-05-11 00:05:34.000000 um6p_cc_learn-0.2.3/um6p_CC_learn/neural_network/__init__.py
--rw-rw-rw-   0        0        0     5036 2024-06-03 03:32:27.000000 um6p_cc_learn-0.2.3/um6p_CC_learn/neural_network/multilayer_perceptron.py
--rw-rw-rw-   0        0        0        0 2024-05-11 00:02:42.000000 um6p_cc_learn-0.2.3/um6p_CC_learn/pipeline.py
-drwxrwxrwx   0        0        0        0 2024-06-03 03:38:47.241285 um6p_cc_learn-0.2.3/um6p_CC_learn/preprocessing/
--rw-rw-rw-   0        0        0        0 2024-05-10 23:43:42.000000 um6p_cc_learn-0.2.3/um6p_CC_learn/preprocessing/__init__.py
--rw-rw-rw-   0        0        0      258 2024-06-02 20:26:01.000000 um6p_cc_learn-0.2.3/um6p_CC_learn/preprocessing/check_X_y.py
-drwxrwxrwx   0        0        0        0 2024-06-03 03:38:47.320481 um6p_cc_learn-0.2.3/um6p_CC_learn/preprocessing/encoding/
--rw-rw-rw-   0        0        0        0 2024-05-10 23:46:19.000000 um6p_cc_learn-0.2.3/um6p_CC_learn/preprocessing/encoding/__init__.py
--rw-rw-rw-   0        0        0     2074 2024-06-03 03:32:40.000000 um6p_cc_learn-0.2.3/um6p_CC_learn/preprocessing/encoding/label_encoder.py
--rw-rw-rw-   0        0        0     1716 2024-06-03 03:32:46.000000 um6p_cc_learn-0.2.3/um6p_CC_learn/preprocessing/encoding/one_hot_encoder.py
--rw-rw-rw-   0        0        0     1681 2024-06-03 03:32:50.000000 um6p_cc_learn-0.2.3/um6p_CC_learn/preprocessing/encoding/ordinal_encoder.py
-drwxrwxrwx   0        0        0        0 2024-06-03 03:38:47.362926 um6p_cc_learn-0.2.3/um6p_CC_learn/preprocessing/imputation/
--rw-rw-rw-   0        0        0        0 2024-05-10 23:45:11.000000 um6p_cc_learn-0.2.3/um6p_CC_learn/preprocessing/imputation/__init__.py
--rw-rw-rw-   0        0        0     1551 2024-06-03 03:32:59.000000 um6p_cc_learn-0.2.3/um6p_CC_learn/preprocessing/imputation/missing_indicator.py
--rw-rw-rw-   0        0        0     1673 2024-06-03 03:33:07.000000 um6p_cc_learn-0.2.3/um6p_CC_learn/preprocessing/imputation/simple_imputer.py
-drwxrwxrwx   0        0        0        0 2024-06-03 03:38:47.398408 um6p_cc_learn-0.2.3/um6p_CC_learn/preprocessing/transformers/
--rw-rw-rw-   0        0        0        0 2024-05-10 23:47:35.000000 um6p_cc_learn-0.2.3/um6p_CC_learn/preprocessing/transformers/__init__.py
--rw-rw-rw-   0        0        0     1944 2024-06-03 03:33:14.000000 um6p_cc_learn-0.2.3/um6p_CC_learn/preprocessing/transformers/normalizer.py
--rw-rw-rw-   0        0        0     4387 2024-06-03 03:33:19.000000 um6p_cc_learn-0.2.3/um6p_CC_learn/preprocessing/transformers/scaler.py
-drwxrwxrwx   0        0        0        0 2024-06-03 03:38:47.489909 um6p_cc_learn-0.2.3/um6p_CC_learn/tests/
--rw-rw-rw-   0        0        0        0 2024-06-03 03:37:32.000000 um6p_cc_learn-0.2.3/um6p_CC_learn/tests/__init__.py
--rw-rw-rw-   0        0        0     2884 2024-06-03 03:37:37.000000 um6p_cc_learn-0.2.3/um6p_CC_learn/tests/decision_trees.py
--rw-rw-rw-   0        0        0     2024 2024-06-03 03:37:41.000000 um6p_cc_learn-0.2.3/um6p_CC_learn/tests/knn_test.py
--rw-rw-rw-   0        0        0     1868 2024-06-03 03:37:47.000000 um6p_cc_learn-0.2.3/um6p_CC_learn/tests/naive_bayes.py
--rw-rw-rw-   0        0        0     2176 2024-06-03 03:37:51.000000 um6p_cc_learn-0.2.3/um6p_CC_learn/tests/neural_network.py
--rw-rw-rw-   0        0        0     2382 2024-06-03 03:37:57.000000 um6p_cc_learn-0.2.3/um6p_CC_learn/tests/regression.py
-drwxrwxrwx   0        0        0        0 2024-06-03 03:38:47.501287 um6p_cc_learn-0.2.3/um6p_CC_learn/tree/
--rw-rw-rw-   0        0        0        0 2024-05-11 00:02:07.000000 um6p_cc_learn-0.2.3/um6p_CC_learn/tree/__init__.py
--rw-rw-rw-   0        0        0    15334 2024-06-03 03:27:49.000000 um6p_cc_learn-0.2.3/um6p_CC_learn/tree/decision_tree.py
-drwxrwxrwx   0        0        0        0 2024-06-03 03:38:47.521136 um6p_cc_learn-0.2.3/um6p_CC_learn/utils/
--rw-rw-rw-   0        0        0     1965 2024-06-02 23:44:19.000000 um6p_cc_learn-0.2.3/um6p_CC_learn/utils/__clone.py
--rw-rw-rw-   0        0        0        0 2024-05-11 00:06:39.000000 um6p_cc_learn-0.2.3/um6p_CC_learn/utils/__init__.py
--rw-rw-rw-   0        0        0     3822 2024-06-03 02:47:08.000000 um6p_cc_learn-0.2.3/um6p_CC_learn/utils/__validation.py
--rw-rw-rw-   0        0        0     6308 2024-06-03 02:23:05.000000 um6p_cc_learn-0.2.3/um6p_CC_learn/utils/_encode.py
-drwxrwxrwx   0        0        0        0 2024-06-03 03:38:47.523521 um6p_cc_learn-0.2.3/um6p_CC_learn.egg-info/
--rw-rw-rw-   0        0        0      435 2024-06-03 03:38:46.000000 um6p_cc_learn-0.2.3/um6p_CC_learn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2578 2024-06-03 03:38:46.000000 um6p_cc_learn-0.2.3/um6p_CC_learn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-03 03:38:46.000000 um6p_cc_learn-0.2.3/um6p_CC_learn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-06-03 03:38:46.000000 um6p_cc_learn-0.2.3/um6p_CC_learn.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-06-03 03:38:46.000000 um6p_cc_learn-0.2.3/um6p_CC_learn.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-03 03:42:05.161965 um6p_cc_learn-0.2.4/
+-rw-rw-rw-   0        0        0      435 2024-06-03 03:42:05.149270 um6p_cc_learn-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-06-03 03:42:05.161965 um6p_cc_learn-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0      584 2024-06-03 03:41:58.000000 um6p_cc_learn-0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 03:42:04.949450 um6p_cc_learn-0.2.4/um6p_CC_learn/
+-rw-rw-rw-   0        0        0       67 2024-06-03 03:20:37.000000 um6p_cc_learn-0.2.4/um6p_CC_learn/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 03:42:04.982596 um6p_cc_learn-0.2.4/um6p_CC_learn/base/
+-rw-rw-rw-   0        0        0        0 2024-05-10 23:42:45.000000 um6p_cc_learn-0.2.4/um6p_CC_learn/base/__init__.py
+-rw-rw-rw-   0        0        0     1573 2024-06-03 03:29:23.000000 um6p_cc_learn-0.2.4/um6p_CC_learn/base/base.py
+drwxrwxrwx   0        0        0        0 2024-06-03 03:42:04.987661 um6p_cc_learn-0.2.4/um6p_CC_learn/decomposition/
+-rw-rw-rw-   0        0        0        0 2024-05-10 23:53:18.000000 um6p_cc_learn-0.2.4/um6p_CC_learn/decomposition/__init__.py
+-rw-rw-rw-   0        0        0      925 2024-06-03 03:29:33.000000 um6p_cc_learn-0.2.4/um6p_CC_learn/decomposition/pca.py
+drwxrwxrwx   0        0        0        0 2024-06-03 03:42:05.001173 um6p_cc_learn-0.2.4/um6p_CC_learn/ensemble/
+-rw-rw-rw-   0        0        0        0 2024-05-11 00:04:22.000000 um6p_cc_learn-0.2.4/um6p_CC_learn/ensemble/__init__.py
+-rw-rw-rw-   0        0        0     2747 2024-06-03 03:29:46.000000 um6p_cc_learn-0.2.4/um6p_CC_learn/ensemble/bagging.py
+-rw-rw-rw-   0        0        0     5548 2024-06-03 03:29:55.000000 um6p_cc_learn-0.2.4/um6p_CC_learn/ensemble/boosting.py
+-rw-rw-rw-   0        0        0     7499 2024-06-03 03:30:01.000000 um6p_cc_learn-0.2.4/um6p_CC_learn/ensemble/random_forest.py
+-rw-rw-rw-   0        0        0     2543 2024-06-03 03:30:09.000000 um6p_cc_learn-0.2.4/um6p_CC_learn/ensemble/stacking.py
+-rw-rw-rw-   0        0        0     1885 2024-06-03 03:30:14.000000 um6p_cc_learn-0.2.4/um6p_CC_learn/ensemble/voting.py
+drwxrwxrwx   0        0        0        0 2024-06-03 03:42:05.019053 um6p_cc_learn-0.2.4/um6p_CC_learn/feature_selection/
+-rw-rw-rw-   0        0        0     2686 2024-06-03 03:30:21.000000 um6p_cc_learn-0.2.4/um6p_CC_learn/feature_selection/RFE.py
+-rw-rw-rw-   0        0        0        0 2024-05-10 23:52:02.000000 um6p_cc_learn-0.2.4/um6p_CC_learn/feature_selection/__init__.py
+-rw-rw-rw-   0        0        0     2354 2024-06-03 03:30:26.000000 um6p_cc_learn-0.2.4/um6p_CC_learn/feature_selection/select_from_model.py
+-rw-rw-rw-   0        0        0     1599 2024-06-03 03:30:30.000000 um6p_cc_learn-0.2.4/um6p_CC_learn/feature_selection/variance_threshold.py
+drwxrwxrwx   0        0        0        0 2024-06-03 03:42:05.027325 um6p_cc_learn-0.2.4/um6p_CC_learn/linear_model/
+-rw-rw-rw-   0        0        0        0 2024-05-11 00:01:31.000000 um6p_cc_learn-0.2.4/um6p_CC_learn/linear_model/__init__.py
+-rw-rw-rw-   0        0        0     3810 2024-06-03 03:30:37.000000 um6p_cc_learn-0.2.4/um6p_CC_learn/linear_model/logistic_regression.py
+-rw-rw-rw-   0        0        0     1667 2024-06-03 03:30:41.000000 um6p_cc_learn-0.2.4/um6p_CC_learn/linear_model/regression.py
+drwxrwxrwx   0        0        0        0 2024-06-03 03:42:05.056945 um6p_cc_learn-0.2.4/um6p_CC_learn/metrics/
+-rw-rw-rw-   0        0        0        0 2024-05-11 21:32:29.000000 um6p_cc_learn-0.2.4/um6p_CC_learn/metrics/__init__.py
+-rw-rw-rw-   0        0        0     1041 2024-06-03 02:23:05.000000 um6p_cc_learn-0.2.4/um6p_CC_learn/metrics/auc.py
+-rw-rw-rw-   0        0        0     3480 2024-05-11 14:50:11.000000 um6p_cc_learn-0.2.4/um6p_CC_learn/metrics/classification.py
+-rw-rw-rw-   0        0        0      299 2024-06-03 03:31:10.000000 um6p_cc_learn-0.2.4/um6p_CC_learn/metrics/cosine_distances.py
+-rw-rw-rw-   0        0        0      784 2024-05-11 14:51:52.000000 um6p_cc_learn-0.2.4/um6p_CC_learn/metrics/cosine_similarity.py
+-rw-rw-rw-   0        0        0     1335 2024-06-03 02:23:05.000000 um6p_cc_learn-0.2.4/um6p_CC_learn/metrics/euclidian_distances.py
+-rw-rw-rw-   0        0        0      398 2024-06-02 16:33:57.000000 um6p_cc_learn-0.2.4/um6p_CC_learn/metrics/regression.py
+-rw-rw-rw-   0        0        0      859 2024-06-03 03:31:39.000000 um6p_cc_learn-0.2.4/um6p_CC_learn/metrics/roc_auc_score.py
+-rw-rw-rw-   0        0        0      653 2024-05-11 15:25:20.000000 um6p_cc_learn-0.2.4/um6p_CC_learn/metrics/roc_curve.py
+drwxrwxrwx   0        0        0        0 2024-06-03 03:42:05.069067 um6p_cc_learn-0.2.4/um6p_CC_learn/model_selection/
+-rw-rw-rw-   0        0        0     2710 2024-06-03 03:32:07.000000 um6p_cc_learn-0.2.4/um6p_CC_learn/model_selection/GridSearch.py
+-rw-rw-rw-   0        0        0        0 2024-05-10 23:59:54.000000 um6p_cc_learn-0.2.4/um6p_CC_learn/model_selection/__init__.py
+-rw-rw-rw-   0        0        0     4804 2024-06-03 02:43:18.000000 um6p_cc_learn-0.2.4/um6p_CC_learn/model_selection/__split.py
+-rw-rw-rw-   0        0        0      746 2024-06-03 03:31:56.000000 um6p_cc_learn-0.2.4/um6p_CC_learn/model_selection/__validation.py
+-rw-rw-rw-   0        0        0     3847 2024-06-03 03:38:24.000000 um6p_cc_learn-0.2.4/um6p_CC_learn/naive_bayes.py
+drwxrwxrwx   0        0        0        0 2024-06-03 03:42:05.074170 um6p_cc_learn-0.2.4/um6p_CC_learn/neural_network/
+-rw-rw-rw-   0        0        0        0 2024-05-11 00:05:34.000000 um6p_cc_learn-0.2.4/um6p_CC_learn/neural_network/__init__.py
+-rw-rw-rw-   0        0        0     5036 2024-06-03 03:32:27.000000 um6p_cc_learn-0.2.4/um6p_CC_learn/neural_network/multilayer_perceptron.py
+-rw-rw-rw-   0        0        0        0 2024-05-11 00:02:42.000000 um6p_cc_learn-0.2.4/um6p_CC_learn/pipeline.py
+drwxrwxrwx   0        0        0        0 2024-06-03 03:42:05.080654 um6p_cc_learn-0.2.4/um6p_CC_learn/preprocessing/
+-rw-rw-rw-   0        0        0        0 2024-05-10 23:43:42.000000 um6p_cc_learn-0.2.4/um6p_CC_learn/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0      258 2024-06-02 20:26:01.000000 um6p_cc_learn-0.2.4/um6p_CC_learn/preprocessing/check_X_y.py
+drwxrwxrwx   0        0        0        0 2024-06-03 03:42:05.086696 um6p_cc_learn-0.2.4/um6p_CC_learn/preprocessing/encoding/
+-rw-rw-rw-   0        0        0        0 2024-05-10 23:46:19.000000 um6p_cc_learn-0.2.4/um6p_CC_learn/preprocessing/encoding/__init__.py
+-rw-rw-rw-   0        0        0     2074 2024-06-03 03:32:40.000000 um6p_cc_learn-0.2.4/um6p_CC_learn/preprocessing/encoding/label_encoder.py
+-rw-rw-rw-   0        0        0     1716 2024-06-03 03:32:46.000000 um6p_cc_learn-0.2.4/um6p_CC_learn/preprocessing/encoding/one_hot_encoder.py
+-rw-rw-rw-   0        0        0     1681 2024-06-03 03:32:50.000000 um6p_cc_learn-0.2.4/um6p_CC_learn/preprocessing/encoding/ordinal_encoder.py
+drwxrwxrwx   0        0        0        0 2024-06-03 03:42:05.100372 um6p_cc_learn-0.2.4/um6p_CC_learn/preprocessing/imputation/
+-rw-rw-rw-   0        0        0        0 2024-05-10 23:45:11.000000 um6p_cc_learn-0.2.4/um6p_CC_learn/preprocessing/imputation/__init__.py
+-rw-rw-rw-   0        0        0     1551 2024-06-03 03:32:59.000000 um6p_cc_learn-0.2.4/um6p_CC_learn/preprocessing/imputation/missing_indicator.py
+-rw-rw-rw-   0        0        0     1673 2024-06-03 03:33:07.000000 um6p_cc_learn-0.2.4/um6p_CC_learn/preprocessing/imputation/simple_imputer.py
+drwxrwxrwx   0        0        0        0 2024-06-03 03:42:05.115489 um6p_cc_learn-0.2.4/um6p_CC_learn/preprocessing/transformers/
+-rw-rw-rw-   0        0        0        0 2024-05-10 23:47:35.000000 um6p_cc_learn-0.2.4/um6p_CC_learn/preprocessing/transformers/__init__.py
+-rw-rw-rw-   0        0        0     1944 2024-06-03 03:33:14.000000 um6p_cc_learn-0.2.4/um6p_CC_learn/preprocessing/transformers/normalizer.py
+-rw-rw-rw-   0        0        0     4387 2024-06-03 03:33:19.000000 um6p_cc_learn-0.2.4/um6p_CC_learn/preprocessing/transformers/scaler.py
+drwxrwxrwx   0        0        0        0 2024-06-03 03:42:05.132391 um6p_cc_learn-0.2.4/um6p_CC_learn/tests/
+-rw-rw-rw-   0        0        0        0 2024-06-03 03:37:32.000000 um6p_cc_learn-0.2.4/um6p_CC_learn/tests/__init__.py
+-rw-rw-rw-   0        0        0     2884 2024-06-03 03:37:37.000000 um6p_cc_learn-0.2.4/um6p_CC_learn/tests/decision_trees.py
+-rw-rw-rw-   0        0        0     2024 2024-06-03 03:37:41.000000 um6p_cc_learn-0.2.4/um6p_CC_learn/tests/knn_test.py
+-rw-rw-rw-   0        0        0     1868 2024-06-03 03:37:47.000000 um6p_cc_learn-0.2.4/um6p_CC_learn/tests/naive_bayes.py
+-rw-rw-rw-   0        0        0     2176 2024-06-03 03:37:51.000000 um6p_cc_learn-0.2.4/um6p_CC_learn/tests/neural_network.py
+-rw-rw-rw-   0        0        0     2382 2024-06-03 03:37:57.000000 um6p_cc_learn-0.2.4/um6p_CC_learn/tests/regression.py
+drwxrwxrwx   0        0        0        0 2024-06-03 03:42:05.138643 um6p_cc_learn-0.2.4/um6p_CC_learn/tree/
+-rw-rw-rw-   0        0        0        0 2024-05-11 00:02:07.000000 um6p_cc_learn-0.2.4/um6p_CC_learn/tree/__init__.py
+-rw-rw-rw-   0        0        0    15334 2024-06-03 03:27:49.000000 um6p_cc_learn-0.2.4/um6p_CC_learn/tree/decision_tree.py
+drwxrwxrwx   0        0        0        0 2024-06-03 03:42:05.149270 um6p_cc_learn-0.2.4/um6p_CC_learn/utils/
+-rw-rw-rw-   0        0        0     1965 2024-06-02 23:44:19.000000 um6p_cc_learn-0.2.4/um6p_CC_learn/utils/__clone.py
+-rw-rw-rw-   0        0        0        0 2024-05-11 00:06:39.000000 um6p_cc_learn-0.2.4/um6p_CC_learn/utils/__init__.py
+-rw-rw-rw-   0        0        0     3822 2024-06-03 02:47:08.000000 um6p_cc_learn-0.2.4/um6p_CC_learn/utils/__validation.py
+-rw-rw-rw-   0        0        0     6308 2024-06-03 02:23:05.000000 um6p_cc_learn-0.2.4/um6p_CC_learn/utils/_encode.py
+drwxrwxrwx   0        0        0        0 2024-06-03 03:42:05.149270 um6p_cc_learn-0.2.4/um6p_CC_learn.egg-info/
+-rw-rw-rw-   0        0        0      435 2024-06-03 03:42:04.000000 um6p_cc_learn-0.2.4/um6p_CC_learn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2578 2024-06-03 03:42:04.000000 um6p_cc_learn-0.2.4/um6p_CC_learn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 03:42:04.000000 um6p_cc_learn-0.2.4/um6p_CC_learn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-06-03 03:42:04.000000 um6p_cc_learn-0.2.4/um6p_CC_learn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-06-03 03:42:04.000000 um6p_cc_learn-0.2.4/um6p_CC_learn.egg-info/top_level.txt
```

### Comparing `um6p_cc_learn-0.2.3/setup.py` & `um6p_cc_learn-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="um6p_CC_learn",
-    version="0.2.3",
+    version="0.2.4",
     author="Sami AGOURRAM , Ilyass Hakkou",
     author_email="Sami.AGOURRAM@um6p.ma",
     description="A home made sklearn",
     packages=find_packages(),
     install_requires=[
         "numpy>=1.21.0",
         "scipy>=1.7.0",
```

### Comparing `um6p_cc_learn-0.2.3/um6p_CC_learn/base/base.py` & `um6p_cc_learn-0.2.4/um6p_CC_learn/base/base.py`

 * *Files identical despite different names*

### Comparing `um6p_cc_learn-0.2.3/um6p_CC_learn/decomposition/pca.py` & `um6p_cc_learn-0.2.4/um6p_CC_learn/decomposition/pca.py`

 * *Files identical despite different names*

### Comparing `um6p_cc_learn-0.2.3/um6p_CC_learn/ensemble/bagging.py` & `um6p_cc_learn-0.2.4/um6p_CC_learn/ensemble/bagging.py`

 * *Files identical despite different names*

### Comparing `um6p_cc_learn-0.2.3/um6p_CC_learn/ensemble/boosting.py` & `um6p_cc_learn-0.2.4/um6p_CC_learn/ensemble/boosting.py`

 * *Files identical despite different names*

### Comparing `um6p_cc_learn-0.2.3/um6p_CC_learn/ensemble/random_forest.py` & `um6p_cc_learn-0.2.4/um6p_CC_learn/ensemble/random_forest.py`

 * *Files identical despite different names*

### Comparing `um6p_cc_learn-0.2.3/um6p_CC_learn/ensemble/stacking.py` & `um6p_cc_learn-0.2.4/um6p_CC_learn/ensemble/stacking.py`

 * *Files identical despite different names*

### Comparing `um6p_cc_learn-0.2.3/um6p_CC_learn/ensemble/voting.py` & `um6p_cc_learn-0.2.4/um6p_CC_learn/ensemble/voting.py`

 * *Files identical despite different names*

### Comparing `um6p_cc_learn-0.2.3/um6p_CC_learn/feature_selection/RFE.py` & `um6p_cc_learn-0.2.4/um6p_CC_learn/feature_selection/RFE.py`

 * *Files identical despite different names*

### Comparing `um6p_cc_learn-0.2.3/um6p_CC_learn/feature_selection/select_from_model.py` & `um6p_cc_learn-0.2.4/um6p_CC_learn/feature_selection/select_from_model.py`

 * *Files identical despite different names*

### Comparing `um6p_cc_learn-0.2.3/um6p_CC_learn/feature_selection/variance_threshold.py` & `um6p_cc_learn-0.2.4/um6p_CC_learn/feature_selection/variance_threshold.py`

 * *Files identical despite different names*

### Comparing `um6p_cc_learn-0.2.3/um6p_CC_learn/linear_model/logistic_regression.py` & `um6p_cc_learn-0.2.4/um6p_CC_learn/linear_model/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `um6p_cc_learn-0.2.3/um6p_CC_learn/linear_model/regression.py` & `um6p_cc_learn-0.2.4/um6p_CC_learn/linear_model/regression.py`

 * *Files identical despite different names*

### Comparing `um6p_cc_learn-0.2.3/um6p_CC_learn/metrics/auc.py` & `um6p_cc_learn-0.2.4/um6p_CC_learn/metrics/auc.py`

 * *Files identical despite different names*

### Comparing `um6p_cc_learn-0.2.3/um6p_CC_learn/metrics/classification.py` & `um6p_cc_learn-0.2.4/um6p_CC_learn/metrics/classification.py`

 * *Files identical despite different names*

### Comparing `um6p_cc_learn-0.2.3/um6p_CC_learn/metrics/cosine_similarity.py` & `um6p_cc_learn-0.2.4/um6p_CC_learn/metrics/cosine_similarity.py`

 * *Files identical despite different names*

### Comparing `um6p_cc_learn-0.2.3/um6p_CC_learn/metrics/euclidian_distances.py` & `um6p_cc_learn-0.2.4/um6p_CC_learn/metrics/euclidian_distances.py`

 * *Files identical despite different names*

### Comparing `um6p_cc_learn-0.2.3/um6p_CC_learn/metrics/roc_auc_score.py` & `um6p_cc_learn-0.2.4/um6p_CC_learn/metrics/roc_auc_score.py`

 * *Files identical despite different names*

### Comparing `um6p_cc_learn-0.2.3/um6p_CC_learn/metrics/roc_curve.py` & `um6p_cc_learn-0.2.4/um6p_CC_learn/metrics/roc_curve.py`

 * *Files identical despite different names*

### Comparing `um6p_cc_learn-0.2.3/um6p_CC_learn/model_selection/GridSearch.py` & `um6p_cc_learn-0.2.4/um6p_CC_learn/model_selection/GridSearch.py`

 * *Files identical despite different names*

### Comparing `um6p_cc_learn-0.2.3/um6p_CC_learn/model_selection/__split.py` & `um6p_cc_learn-0.2.4/um6p_CC_learn/model_selection/__split.py`

 * *Files identical despite different names*

### Comparing `um6p_cc_learn-0.2.3/um6p_CC_learn/model_selection/__validation.py` & `um6p_cc_learn-0.2.4/um6p_CC_learn/model_selection/__validation.py`

 * *Files identical despite different names*

### Comparing `um6p_cc_learn-0.2.3/um6p_CC_learn/naive_bayes.py` & `um6p_cc_learn-0.2.4/um6p_CC_learn/naive_bayes.py`

 * *Files identical despite different names*

### Comparing `um6p_cc_learn-0.2.3/um6p_CC_learn/neural_network/multilayer_perceptron.py` & `um6p_cc_learn-0.2.4/um6p_CC_learn/neural_network/multilayer_perceptron.py`

 * *Files identical despite different names*

### Comparing `um6p_cc_learn-0.2.3/um6p_CC_learn/preprocessing/encoding/label_encoder.py` & `um6p_cc_learn-0.2.4/um6p_CC_learn/preprocessing/encoding/label_encoder.py`

 * *Files identical despite different names*

### Comparing `um6p_cc_learn-0.2.3/um6p_CC_learn/preprocessing/encoding/one_hot_encoder.py` & `um6p_cc_learn-0.2.4/um6p_CC_learn/preprocessing/encoding/one_hot_encoder.py`

 * *Files identical despite different names*

### Comparing `um6p_cc_learn-0.2.3/um6p_CC_learn/preprocessing/encoding/ordinal_encoder.py` & `um6p_cc_learn-0.2.4/um6p_CC_learn/preprocessing/encoding/ordinal_encoder.py`

 * *Files identical despite different names*

### Comparing `um6p_cc_learn-0.2.3/um6p_CC_learn/preprocessing/imputation/missing_indicator.py` & `um6p_cc_learn-0.2.4/um6p_CC_learn/preprocessing/imputation/missing_indicator.py`

 * *Files identical despite different names*

### Comparing `um6p_cc_learn-0.2.3/um6p_CC_learn/preprocessing/imputation/simple_imputer.py` & `um6p_cc_learn-0.2.4/um6p_CC_learn/preprocessing/imputation/simple_imputer.py`

 * *Files identical despite different names*

### Comparing `um6p_cc_learn-0.2.3/um6p_CC_learn/preprocessing/transformers/normalizer.py` & `um6p_cc_learn-0.2.4/um6p_CC_learn/preprocessing/transformers/normalizer.py`

 * *Files identical despite different names*

### Comparing `um6p_cc_learn-0.2.3/um6p_CC_learn/preprocessing/transformers/scaler.py` & `um6p_cc_learn-0.2.4/um6p_CC_learn/preprocessing/transformers/scaler.py`

 * *Files identical despite different names*

### Comparing `um6p_cc_learn-0.2.3/um6p_CC_learn/tests/decision_trees.py` & `um6p_cc_learn-0.2.4/um6p_CC_learn/tests/decision_trees.py`

 * *Files identical despite different names*

### Comparing `um6p_cc_learn-0.2.3/um6p_CC_learn/tests/knn_test.py` & `um6p_cc_learn-0.2.4/um6p_CC_learn/tests/knn_test.py`

 * *Files identical despite different names*

### Comparing `um6p_cc_learn-0.2.3/um6p_CC_learn/tests/naive_bayes.py` & `um6p_cc_learn-0.2.4/um6p_CC_learn/tests/naive_bayes.py`

 * *Files identical despite different names*

### Comparing `um6p_cc_learn-0.2.3/um6p_CC_learn/tests/neural_network.py` & `um6p_cc_learn-0.2.4/um6p_CC_learn/tests/neural_network.py`

 * *Files identical despite different names*

### Comparing `um6p_cc_learn-0.2.3/um6p_CC_learn/tests/regression.py` & `um6p_cc_learn-0.2.4/um6p_CC_learn/tests/regression.py`

 * *Files identical despite different names*

### Comparing `um6p_cc_learn-0.2.3/um6p_CC_learn/tree/decision_tree.py` & `um6p_cc_learn-0.2.4/um6p_CC_learn/tree/decision_tree.py`

 * *Files identical despite different names*

### Comparing `um6p_cc_learn-0.2.3/um6p_CC_learn/utils/__clone.py` & `um6p_cc_learn-0.2.4/um6p_CC_learn/utils/__clone.py`

 * *Files identical despite different names*

### Comparing `um6p_cc_learn-0.2.3/um6p_CC_learn/utils/__validation.py` & `um6p_cc_learn-0.2.4/um6p_CC_learn/utils/__validation.py`

 * *Files identical despite different names*

### Comparing `um6p_cc_learn-0.2.3/um6p_CC_learn/utils/_encode.py` & `um6p_cc_learn-0.2.4/um6p_CC_learn/utils/_encode.py`

 * *Files identical despite different names*

### Comparing `um6p_cc_learn-0.2.3/um6p_CC_learn.egg-info/SOURCES.txt` & `um6p_cc_learn-0.2.4/um6p_CC_learn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

