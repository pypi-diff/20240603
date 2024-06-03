# Comparing `tmp/cs_ob_mini_scikit_learn-0.1.8.tar.gz` & `tmp/cs_ob_mini_scikit_learn-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs_ob_mini_scikit_learn-0.1.8.tar", last modified: Mon Jun  3 01:31:44 2024, max compression
+gzip compressed data, was "cs_ob_mini_scikit_learn-0.1.9.tar", last modified: Mon Jun  3 01:34:58 2024, max compression
```

## Comparing `cs_ob_mini_scikit_learn-0.1.8.tar` & `cs_ob_mini_scikit_learn-0.1.9.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:31:44.100054 cs_ob_mini_scikit_learn-0.1.8/
--rw-r--r--   0 mac        (501) staff       (20)     2715 2024-06-03 01:31:44.088093 cs_ob_mini_scikit_learn-0.1.8/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     2346 2024-05-22 21:15:43.000000 cs_ob_mini_scikit_learn-0.1.8/README.md
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:31:43.981340 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/
--rw-r--r--   0 mac        (501) staff       (20)     1450 2024-06-03 01:31:22.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)       40 2024-06-03 00:38:20.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/cctest.py
--rw-r--r--   0 mac        (501) staff       (20)      632 2024-05-22 22:23:16.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/clone.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:31:43.998424 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/ensemble/
--rw-r--r--   0 mac        (501) staff       (20)     4283 2024-06-02 21:46:43.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/ensemble/AdaBoost.py
--rw-r--r--   0 mac        (501) staff       (20)     4689 2024-06-02 21:21:42.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/ensemble/GradientBoostingClassifier.py
--rw-r--r--   0 mac        (501) staff       (20)     3705 2024-06-02 21:22:38.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/ensemble/GradientBoostingRegressor.py
--rw-r--r--   0 mac        (501) staff       (20)     5053 2024-06-02 21:23:06.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/ensemble/RandomForestClassifier.py
--rw-r--r--   0 mac        (501) staff       (20)     4000 2024-06-02 21:24:02.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/ensemble/RandomForestRegressor.py
--rw-r--r--   0 mac        (501) staff       (20)      147 2024-06-03 01:31:28.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/ensemble/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:31:44.012598 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/metrics/
--rw-r--r--   0 mac        (501) staff       (20)      846 2024-06-02 20:32:40.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/metrics/Accuracy.py
--rw-r--r--   0 mac        (501) staff       (20)      657 2024-06-02 20:33:25.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/metrics/BaseMetric.py
--rw-r--r--   0 mac        (501) staff       (20)     1127 2024-06-02 20:34:14.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/metrics/ConfusionMatrix.py
--rw-r--r--   0 mac        (501) staff       (20)      937 2024-06-02 20:34:23.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/metrics/F1Score.py
--rw-r--r--   0 mac        (501) staff       (20)      742 2024-06-02 20:34:35.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/metrics/MeanAbsoluteError.py
--rw-r--r--   0 mac        (501) staff       (20)      736 2024-06-02 20:35:27.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/metrics/MeanSquaredError.py
--rw-r--r--   0 mac        (501) staff       (20)      910 2024-06-02 20:35:39.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/metrics/Precision.py
--rw-r--r--   0 mac        (501) staff       (20)      901 2024-06-02 20:36:41.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/metrics/RSquared.py
--rw-r--r--   0 mac        (501) staff       (20)      888 2024-06-02 20:35:49.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/metrics/Recall.py
--rw-r--r--   0 mac        (501) staff       (20)      805 2024-06-02 20:35:58.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/metrics/RootMeanSquaredError.py
--rw-r--r--   0 mac        (501) staff       (20)      381 2024-06-02 18:18:52.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/metrics/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:31:44.016474 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/model_selection/
--rw-r--r--   0 mac        (501) staff       (20)     4012 2024-06-02 21:49:06.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/model_selection/GridSearchCV.py
--rw-r--r--   0 mac        (501) staff       (20)     2154 2024-06-02 21:28:12.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/model_selection/KFold.py
--rw-r--r--   0 mac        (501) staff       (20)      967 2024-06-02 21:28:00.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/model_selection/ParameterGrid.py
--rw-r--r--   0 mac        (501) staff       (20)      151 2024-06-02 18:19:39.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/model_selection/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     3797 2024-06-02 21:51:24.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/model_selection/train_test_split.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:31:44.021072 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/neural_networks/
--rw-r--r--   0 mac        (501) staff       (20)     3875 2024-06-02 21:28:42.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/neural_networks/MLP.py
--rw-r--r--   0 mac        (501) staff       (20)     7182 2024-06-02 21:29:49.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/neural_networks/MLPRegressor.py
--rw-r--r--   0 mac        (501) staff       (20)     3025 2024-06-02 21:30:03.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/neural_networks/Perceptron.py
--rw-r--r--   0 mac        (501) staff       (20)       60 2024-06-02 18:20:00.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/neural_networks/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:31:44.035900 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/preprocessing/
--rw-r--r--   0 mac        (501) staff       (20)     2825 2024-06-02 21:31:50.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/preprocessing/LabelEncoder.py
--rw-r--r--   0 mac        (501) staff       (20)     2317 2024-06-02 21:32:10.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/preprocessing/MinMaxScaler.py
--rw-r--r--   0 mac        (501) staff       (20)     2468 2024-06-02 21:32:27.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/preprocessing/OneHotEncoder.py
--rw-r--r--   0 mac        (501) staff       (20)     3041 2024-06-02 21:34:15.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/preprocessing/SimpleImputer.py
--rw-r--r--   0 mac        (501) staff       (20)     2333 2024-06-02 21:34:44.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/preprocessing/StandardScaler.py
--rw-r--r--   0 mac        (501) staff       (20)      202 2024-06-02 18:20:46.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/preprocessing/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:31:44.037583 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/supervised_learning/
--rw-r--r--   0 mac        (501) staff       (20)     1810 2024-06-02 20:56:39.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/supervised_learning/BaseEstimator.py
--rw-r--r--   0 mac        (501) staff       (20)       40 2024-06-02 18:23:05.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/supervised_learning/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:31:44.068617 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/supervised_learning/classification/
--rw-r--r--   0 mac        (501) staff       (20)     6719 2024-06-02 21:17:12.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/supervised_learning/classification/DecisionTreeClassifier.py
--rw-r--r--   0 mac        (501) staff       (20)     3339 2024-06-02 21:16:04.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/supervised_learning/classification/KNNClassifier.py
--rw-r--r--   0 mac        (501) staff       (20)     5232 2024-06-02 21:14:23.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/supervised_learning/classification/LogisticRegression.py
--rw-r--r--   0 mac        (501) staff       (20)     2722 2024-06-02 21:54:57.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/supervised_learning/classification/NaiveBayes.py
--rw-r--r--   0 mac        (501) staff       (20)     2291 2024-06-02 21:04:16.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/supervised_learning/classification/SVM.py
--rw-r--r--   0 mac        (501) staff       (20)      206 2024-06-02 20:58:44.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/supervised_learning/classification/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:31:44.082844 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/supervised_learning/regression/
--rw-r--r--   0 mac        (501) staff       (20)     5598 2024-06-02 21:13:44.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/supervised_learning/regression/DecisionTreeRegressor.py
--rw-r--r--   0 mac        (501) staff       (20)     2368 2024-06-02 21:05:04.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/supervised_learning/regression/LinearRegression.py
--rw-r--r--   0 mac        (501) staff       (20)      104 2024-06-02 20:58:18.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/supervised_learning/regression/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:31:44.086867 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/utilities/
--rw-r--r--   0 mac        (501) staff       (20)       94 2024-06-02 18:29:01.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/utilities/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)      825 2024-06-02 18:28:48.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/utilities/data_manipulation.py
--rw-r--r--   0 mac        (501) staff       (20)      355 2024-06-02 18:26:21.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/utilities/file_handling.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:31:43.988092 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)     2715 2024-06-03 01:31:43.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     2957 2024-06-03 01:31:43.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2024-06-03 01:31:43.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)       38 2024-06-03 01:31:43.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)       24 2024-06-03 01:31:43.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn.egg-info/top_level.txt
--rw-r--r--   0 mac        (501) staff       (20)       38 2024-06-03 01:31:44.101308 cs_ob_mini_scikit_learn-0.1.8/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)      625 2024-06-03 01:31:34.000000 cs_ob_mini_scikit_learn-0.1.8/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:34:58.526079 cs_ob_mini_scikit_learn-0.1.9/
+-rw-r--r--   0 mac        (501) staff       (20)     2715 2024-06-03 01:34:58.525477 cs_ob_mini_scikit_learn-0.1.9/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     2346 2024-05-22 21:15:43.000000 cs_ob_mini_scikit_learn-0.1.9/README.md
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:34:58.395127 cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/
+-rw-r--r--   0 mac        (501) staff       (20)     1450 2024-06-03 01:31:22.000000 cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)       40 2024-06-03 00:38:20.000000 cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/cctest.py
+-rw-r--r--   0 mac        (501) staff       (20)      632 2024-05-22 22:23:16.000000 cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/clone.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:34:58.413862 cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/ensemble/
+-rw-r--r--   0 mac        (501) staff       (20)     4317 2024-06-03 01:34:38.000000 cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/ensemble/AdaBoost.py
+-rw-r--r--   0 mac        (501) staff       (20)     4689 2024-06-02 21:21:42.000000 cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/ensemble/GradientBoostingClassifier.py
+-rw-r--r--   0 mac        (501) staff       (20)     3705 2024-06-02 21:22:38.000000 cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/ensemble/GradientBoostingRegressor.py
+-rw-r--r--   0 mac        (501) staff       (20)     5053 2024-06-02 21:23:06.000000 cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/ensemble/RandomForestClassifier.py
+-rw-r--r--   0 mac        (501) staff       (20)     4000 2024-06-02 21:24:02.000000 cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/ensemble/RandomForestRegressor.py
+-rw-r--r--   0 mac        (501) staff       (20)      147 2024-06-03 01:31:28.000000 cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/ensemble/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:34:58.431524 cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/metrics/
+-rw-r--r--   0 mac        (501) staff       (20)      846 2024-06-02 20:32:40.000000 cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/metrics/Accuracy.py
+-rw-r--r--   0 mac        (501) staff       (20)      657 2024-06-02 20:33:25.000000 cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/metrics/BaseMetric.py
+-rw-r--r--   0 mac        (501) staff       (20)     1127 2024-06-02 20:34:14.000000 cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/metrics/ConfusionMatrix.py
+-rw-r--r--   0 mac        (501) staff       (20)      937 2024-06-02 20:34:23.000000 cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/metrics/F1Score.py
+-rw-r--r--   0 mac        (501) staff       (20)      742 2024-06-02 20:34:35.000000 cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/metrics/MeanAbsoluteError.py
+-rw-r--r--   0 mac        (501) staff       (20)      736 2024-06-02 20:35:27.000000 cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/metrics/MeanSquaredError.py
+-rw-r--r--   0 mac        (501) staff       (20)      910 2024-06-02 20:35:39.000000 cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/metrics/Precision.py
+-rw-r--r--   0 mac        (501) staff       (20)      901 2024-06-02 20:36:41.000000 cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/metrics/RSquared.py
+-rw-r--r--   0 mac        (501) staff       (20)      888 2024-06-02 20:35:49.000000 cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/metrics/Recall.py
+-rw-r--r--   0 mac        (501) staff       (20)      805 2024-06-02 20:35:58.000000 cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/metrics/RootMeanSquaredError.py
+-rw-r--r--   0 mac        (501) staff       (20)      381 2024-06-02 18:18:52.000000 cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/metrics/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:34:58.442869 cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/model_selection/
+-rw-r--r--   0 mac        (501) staff       (20)     4012 2024-06-02 21:49:06.000000 cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/model_selection/GridSearchCV.py
+-rw-r--r--   0 mac        (501) staff       (20)     2154 2024-06-02 21:28:12.000000 cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/model_selection/KFold.py
+-rw-r--r--   0 mac        (501) staff       (20)      967 2024-06-02 21:28:00.000000 cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/model_selection/ParameterGrid.py
+-rw-r--r--   0 mac        (501) staff       (20)      151 2024-06-02 18:19:39.000000 cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/model_selection/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     3797 2024-06-02 21:51:24.000000 cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/model_selection/train_test_split.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:34:58.455768 cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/neural_networks/
+-rw-r--r--   0 mac        (501) staff       (20)     3875 2024-06-02 21:28:42.000000 cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/neural_networks/MLP.py
+-rw-r--r--   0 mac        (501) staff       (20)     7182 2024-06-02 21:29:49.000000 cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/neural_networks/MLPRegressor.py
+-rw-r--r--   0 mac        (501) staff       (20)     3025 2024-06-02 21:30:03.000000 cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/neural_networks/Perceptron.py
+-rw-r--r--   0 mac        (501) staff       (20)       60 2024-06-02 18:20:00.000000 cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/neural_networks/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:34:58.489057 cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/preprocessing/
+-rw-r--r--   0 mac        (501) staff       (20)     2825 2024-06-02 21:31:50.000000 cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/preprocessing/LabelEncoder.py
+-rw-r--r--   0 mac        (501) staff       (20)     2317 2024-06-02 21:32:10.000000 cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/preprocessing/MinMaxScaler.py
+-rw-r--r--   0 mac        (501) staff       (20)     2468 2024-06-02 21:32:27.000000 cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/preprocessing/OneHotEncoder.py
+-rw-r--r--   0 mac        (501) staff       (20)     3041 2024-06-02 21:34:15.000000 cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/preprocessing/SimpleImputer.py
+-rw-r--r--   0 mac        (501) staff       (20)     2333 2024-06-02 21:34:44.000000 cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/preprocessing/StandardScaler.py
+-rw-r--r--   0 mac        (501) staff       (20)      202 2024-06-02 18:20:46.000000 cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/preprocessing/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:34:58.493300 cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/supervised_learning/
+-rw-r--r--   0 mac        (501) staff       (20)     1810 2024-06-02 20:56:39.000000 cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/supervised_learning/BaseEstimator.py
+-rw-r--r--   0 mac        (501) staff       (20)       40 2024-06-02 18:23:05.000000 cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/supervised_learning/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:34:58.505091 cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/supervised_learning/classification/
+-rw-r--r--   0 mac        (501) staff       (20)     6719 2024-06-02 21:17:12.000000 cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/supervised_learning/classification/DecisionTreeClassifier.py
+-rw-r--r--   0 mac        (501) staff       (20)     3339 2024-06-02 21:16:04.000000 cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/supervised_learning/classification/KNNClassifier.py
+-rw-r--r--   0 mac        (501) staff       (20)     5232 2024-06-02 21:14:23.000000 cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/supervised_learning/classification/LogisticRegression.py
+-rw-r--r--   0 mac        (501) staff       (20)     2722 2024-06-02 21:54:57.000000 cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/supervised_learning/classification/NaiveBayes.py
+-rw-r--r--   0 mac        (501) staff       (20)     2291 2024-06-02 21:04:16.000000 cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/supervised_learning/classification/SVM.py
+-rw-r--r--   0 mac        (501) staff       (20)      206 2024-06-02 20:58:44.000000 cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/supervised_learning/classification/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:34:58.510936 cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/supervised_learning/regression/
+-rw-r--r--   0 mac        (501) staff       (20)     5598 2024-06-02 21:13:44.000000 cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/supervised_learning/regression/DecisionTreeRegressor.py
+-rw-r--r--   0 mac        (501) staff       (20)     2368 2024-06-02 21:05:04.000000 cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/supervised_learning/regression/LinearRegression.py
+-rw-r--r--   0 mac        (501) staff       (20)      104 2024-06-02 20:58:18.000000 cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/supervised_learning/regression/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:34:58.522441 cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/utilities/
+-rw-r--r--   0 mac        (501) staff       (20)       94 2024-06-02 18:29:01.000000 cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/utilities/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)      825 2024-06-02 18:28:48.000000 cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/utilities/data_manipulation.py
+-rw-r--r--   0 mac        (501) staff       (20)      355 2024-06-02 18:26:21.000000 cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/utilities/file_handling.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:34:58.400792 cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)     2715 2024-06-03 01:34:58.000000 cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     2957 2024-06-03 01:34:58.000000 cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2024-06-03 01:34:58.000000 cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)       38 2024-06-03 01:34:58.000000 cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)       24 2024-06-03 01:34:58.000000 cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn.egg-info/top_level.txt
+-rw-r--r--   0 mac        (501) staff       (20)       38 2024-06-03 01:34:58.526297 cs_ob_mini_scikit_learn-0.1.9/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)      625 2024-06-03 01:34:51.000000 cs_ob_mini_scikit_learn-0.1.9/setup.py
```

### Comparing `cs_ob_mini_scikit_learn-0.1.8/PKG-INFO` & `cs_ob_mini_scikit_learn-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs_ob_mini_scikit_learn
-Version: 0.1.8
+Version: 0.1.9
 Summary: A minimal implementation of scikit-learn like functionalities
 Home-page: https://github.com/Basma-Arnaoui/Mini-Scikit-Learn/tree/main
 Author: basma-arnaoui
 Author-email: basma.arnaoui@um6p.ma
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `cs_ob_mini_scikit_learn-0.1.8/README.md` & `cs_ob_mini_scikit_learn-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/__init__.py` & `cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/__init__.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/clone.py` & `cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/clone.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/ensemble/AdaBoost.py` & `cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/ensemble/AdaBoost.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import numpy as np
+import sys
+sys.path.append("../")
 from supervised_learning.classification.DecisionTreeClassifier import DecisionTreeClassifier
 
 
 class AdaBoost:
     """
     AdaBoost (Adaptive Boosting) implementation using DecisionTreeClassifier as the base estimator.
```

### Comparing `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/ensemble/GradientBoostingClassifier.py` & `cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/ensemble/GradientBoostingClassifier.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/ensemble/GradientBoostingRegressor.py` & `cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/ensemble/GradientBoostingRegressor.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/ensemble/RandomForestClassifier.py` & `cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/ensemble/RandomForestClassifier.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/ensemble/RandomForestRegressor.py` & `cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/ensemble/RandomForestRegressor.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/metrics/Accuracy.py` & `cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/metrics/Accuracy.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/metrics/BaseMetric.py` & `cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/metrics/BaseMetric.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/metrics/ConfusionMatrix.py` & `cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/metrics/ConfusionMatrix.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/metrics/F1Score.py` & `cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/metrics/F1Score.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/metrics/MeanAbsoluteError.py` & `cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/metrics/MeanAbsoluteError.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/metrics/MeanSquaredError.py` & `cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/metrics/MeanSquaredError.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/metrics/Precision.py` & `cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/metrics/Precision.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/metrics/RSquared.py` & `cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/metrics/RSquared.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/metrics/Recall.py` & `cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/metrics/Recall.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/metrics/RootMeanSquaredError.py` & `cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/metrics/RootMeanSquaredError.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/model_selection/GridSearchCV.py` & `cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/model_selection/GridSearchCV.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/model_selection/KFold.py` & `cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/model_selection/KFold.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/model_selection/ParameterGrid.py` & `cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/model_selection/ParameterGrid.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/model_selection/train_test_split.py` & `cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/model_selection/train_test_split.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/neural_networks/MLP.py` & `cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/neural_networks/MLP.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/neural_networks/MLPRegressor.py` & `cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/neural_networks/MLPRegressor.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/neural_networks/Perceptron.py` & `cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/neural_networks/Perceptron.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/preprocessing/LabelEncoder.py` & `cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/preprocessing/LabelEncoder.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/preprocessing/MinMaxScaler.py` & `cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/preprocessing/MinMaxScaler.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/preprocessing/OneHotEncoder.py` & `cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/preprocessing/OneHotEncoder.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/preprocessing/SimpleImputer.py` & `cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/preprocessing/SimpleImputer.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/preprocessing/StandardScaler.py` & `cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/preprocessing/StandardScaler.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/supervised_learning/BaseEstimator.py` & `cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/supervised_learning/BaseEstimator.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/supervised_learning/classification/DecisionTreeClassifier.py` & `cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/supervised_learning/classification/DecisionTreeClassifier.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/supervised_learning/classification/KNNClassifier.py` & `cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/supervised_learning/classification/KNNClassifier.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/supervised_learning/classification/LogisticRegression.py` & `cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/supervised_learning/classification/LogisticRegression.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/supervised_learning/classification/NaiveBayes.py` & `cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/supervised_learning/classification/NaiveBayes.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/supervised_learning/classification/SVM.py` & `cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/supervised_learning/classification/SVM.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/supervised_learning/regression/DecisionTreeRegressor.py` & `cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/supervised_learning/regression/DecisionTreeRegressor.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/supervised_learning/regression/LinearRegression.py` & `cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/supervised_learning/regression/LinearRegression.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/utilities/data_manipulation.py` & `cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn/utilities/data_manipulation.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn.egg-info/PKG-INFO` & `cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs-ob-mini-scikit-learn
-Version: 0.1.8
+Version: 0.1.9
 Summary: A minimal implementation of scikit-learn like functionalities
 Home-page: https://github.com/Basma-Arnaoui/Mini-Scikit-Learn/tree/main
 Author: basma-arnaoui
 Author-email: basma.arnaoui@um6p.ma
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn.egg-info/SOURCES.txt` & `cs_ob_mini_scikit_learn-0.1.9/cs_ob_mini_scikit_learn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.8/setup.py` & `cs_ob_mini_scikit_learn-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cs_ob_mini_scikit_learn',
-    version='0.1.8',
+    version='0.1.9',
     author='basma-arnaoui',
     author_email='basma.arnaoui@um6p.ma',
     packages=find_packages(),
     install_requires=[
         'numpy',
         'scipy',
         'scikit-learn',
```
