# Comparing `tmp/cc-mini-scikit-learn-0.1.2.tar.gz` & `tmp/cc_mini_scikit_learn-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cc-mini-scikit-learn-0.1.2.tar", last modified: Sun Jun  2 23:12:57 2024, max compression
+gzip compressed data, was "cc_mini_scikit_learn-0.1.3.tar", last modified: Sun Jun  2 23:19:07 2024, max compression
```

## Comparing `cc-mini-scikit-learn-0.1.2.tar` & `cc_mini_scikit_learn-0.1.3.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-02 23:12:57.039051 cc-mini-scikit-learn-0.1.2/
--rw-r--r--   0 mac        (501) staff       (20)     2712 2024-06-02 23:12:57.038012 cc-mini-scikit-learn-0.1.2/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     2346 2024-05-22 21:15:43.000000 cc-mini-scikit-learn-0.1.2/README.md
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-02 23:12:56.729741 cc-mini-scikit-learn-0.1.2/cc_mini_scikit_learn.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)     2712 2024-06-02 23:12:56.000000 cc-mini-scikit-learn-0.1.2/cc_mini_scikit_learn.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     1795 2024-06-02 23:12:56.000000 cc-mini-scikit-learn-0.1.2/cc_mini_scikit_learn.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2024-06-02 23:12:56.000000 cc-mini-scikit-learn-0.1.2/cc_mini_scikit_learn.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)       25 2024-06-02 23:12:56.000000 cc-mini-scikit-learn-0.1.2/cc_mini_scikit_learn.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)       93 2024-06-02 23:12:56.000000 cc-mini-scikit-learn-0.1.2/cc_mini_scikit_learn.egg-info/top_level.txt
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-02 23:12:56.786225 cc-mini-scikit-learn-0.1.2/ensemble/
--rw-r--r--   0 mac        (501) staff       (20)     4283 2024-06-02 21:46:43.000000 cc-mini-scikit-learn-0.1.2/ensemble/AdaBoost.py
--rw-r--r--   0 mac        (501) staff       (20)     4689 2024-06-02 21:21:42.000000 cc-mini-scikit-learn-0.1.2/ensemble/GradientBoostingClassifier.py
--rw-r--r--   0 mac        (501) staff       (20)     3705 2024-06-02 21:22:38.000000 cc-mini-scikit-learn-0.1.2/ensemble/GradientBoostingRegressor.py
--rw-r--r--   0 mac        (501) staff       (20)     5053 2024-06-02 21:23:06.000000 cc-mini-scikit-learn-0.1.2/ensemble/RandomForestClassifier.py
--rw-r--r--   0 mac        (501) staff       (20)     4000 2024-06-02 21:24:02.000000 cc-mini-scikit-learn-0.1.2/ensemble/RandomForestRegressor.py
--rw-r--r--   0 mac        (501) staff       (20)     3882 2024-06-02 21:24:41.000000 cc-mini-scikit-learn-0.1.2/ensemble/StackingClassifier.py
--rw-r--r--   0 mac        (501) staff       (20)     3094 2024-06-02 21:25:08.000000 cc-mini-scikit-learn-0.1.2/ensemble/VotingClassifier.py
--rw-r--r--   0 mac        (501) staff       (20)      245 2024-06-02 20:58:50.000000 cc-mini-scikit-learn-0.1.2/ensemble/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-02 23:12:56.850013 cc-mini-scikit-learn-0.1.2/metrics/
--rw-r--r--   0 mac        (501) staff       (20)      846 2024-06-02 20:32:40.000000 cc-mini-scikit-learn-0.1.2/metrics/Accuracy.py
--rw-r--r--   0 mac        (501) staff       (20)      657 2024-06-02 20:33:25.000000 cc-mini-scikit-learn-0.1.2/metrics/BaseMetric.py
--rw-r--r--   0 mac        (501) staff       (20)     1127 2024-06-02 20:34:14.000000 cc-mini-scikit-learn-0.1.2/metrics/ConfusionMatrix.py
--rw-r--r--   0 mac        (501) staff       (20)      937 2024-06-02 20:34:23.000000 cc-mini-scikit-learn-0.1.2/metrics/F1Score.py
--rw-r--r--   0 mac        (501) staff       (20)      742 2024-06-02 20:34:35.000000 cc-mini-scikit-learn-0.1.2/metrics/MeanAbsoluteError.py
--rw-r--r--   0 mac        (501) staff       (20)      736 2024-06-02 20:35:27.000000 cc-mini-scikit-learn-0.1.2/metrics/MeanSquaredError.py
--rw-r--r--   0 mac        (501) staff       (20)      910 2024-06-02 20:35:39.000000 cc-mini-scikit-learn-0.1.2/metrics/Precision.py
--rw-r--r--   0 mac        (501) staff       (20)      901 2024-06-02 20:36:41.000000 cc-mini-scikit-learn-0.1.2/metrics/RSquared.py
--rw-r--r--   0 mac        (501) staff       (20)      888 2024-06-02 20:35:49.000000 cc-mini-scikit-learn-0.1.2/metrics/Recall.py
--rw-r--r--   0 mac        (501) staff       (20)      805 2024-06-02 20:35:58.000000 cc-mini-scikit-learn-0.1.2/metrics/RootMeanSquaredError.py
--rw-r--r--   0 mac        (501) staff       (20)      381 2024-06-02 18:18:52.000000 cc-mini-scikit-learn-0.1.2/metrics/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-02 23:12:56.987132 cc-mini-scikit-learn-0.1.2/model_selection/
--rw-r--r--   0 mac        (501) staff       (20)     4012 2024-06-02 21:49:06.000000 cc-mini-scikit-learn-0.1.2/model_selection/GridSearchCV.py
--rw-r--r--   0 mac        (501) staff       (20)     2154 2024-06-02 21:28:12.000000 cc-mini-scikit-learn-0.1.2/model_selection/KFold.py
--rw-r--r--   0 mac        (501) staff       (20)      967 2024-06-02 21:28:00.000000 cc-mini-scikit-learn-0.1.2/model_selection/ParameterGrid.py
--rw-r--r--   0 mac        (501) staff       (20)      151 2024-06-02 18:19:39.000000 cc-mini-scikit-learn-0.1.2/model_selection/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     3797 2024-06-02 21:51:24.000000 cc-mini-scikit-learn-0.1.2/model_selection/train_test_split.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-02 23:12:56.998818 cc-mini-scikit-learn-0.1.2/neural_networks/
--rw-r--r--   0 mac        (501) staff       (20)     3875 2024-06-02 21:28:42.000000 cc-mini-scikit-learn-0.1.2/neural_networks/MLP.py
--rw-r--r--   0 mac        (501) staff       (20)     7182 2024-06-02 21:29:49.000000 cc-mini-scikit-learn-0.1.2/neural_networks/MLPRegressor.py
--rw-r--r--   0 mac        (501) staff       (20)     3025 2024-06-02 21:30:03.000000 cc-mini-scikit-learn-0.1.2/neural_networks/Perceptron.py
--rw-r--r--   0 mac        (501) staff       (20)       60 2024-06-02 18:20:00.000000 cc-mini-scikit-learn-0.1.2/neural_networks/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-02 23:12:57.014963 cc-mini-scikit-learn-0.1.2/preprocessing/
--rw-r--r--   0 mac        (501) staff       (20)     2825 2024-06-02 21:31:50.000000 cc-mini-scikit-learn-0.1.2/preprocessing/LabelEncoder.py
--rw-r--r--   0 mac        (501) staff       (20)     2317 2024-06-02 21:32:10.000000 cc-mini-scikit-learn-0.1.2/preprocessing/MinMaxScaler.py
--rw-r--r--   0 mac        (501) staff       (20)     2468 2024-06-02 21:32:27.000000 cc-mini-scikit-learn-0.1.2/preprocessing/OneHotEncoder.py
--rw-r--r--   0 mac        (501) staff       (20)     3041 2024-06-02 21:34:15.000000 cc-mini-scikit-learn-0.1.2/preprocessing/SimpleImputer.py
--rw-r--r--   0 mac        (501) staff       (20)     2333 2024-06-02 21:34:44.000000 cc-mini-scikit-learn-0.1.2/preprocessing/StandardScaler.py
--rw-r--r--   0 mac        (501) staff       (20)      202 2024-06-02 18:20:46.000000 cc-mini-scikit-learn-0.1.2/preprocessing/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)       38 2024-06-02 23:12:57.041452 cc-mini-scikit-learn-0.1.2/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)      587 2024-06-02 23:12:49.000000 cc-mini-scikit-learn-0.1.2/setup.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-02 23:12:57.019544 cc-mini-scikit-learn-0.1.2/supervised_learning/
--rw-r--r--   0 mac        (501) staff       (20)     1810 2024-06-02 20:56:39.000000 cc-mini-scikit-learn-0.1.2/supervised_learning/BaseEstimator.py
--rw-r--r--   0 mac        (501) staff       (20)       40 2024-06-02 18:23:05.000000 cc-mini-scikit-learn-0.1.2/supervised_learning/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-02 23:12:57.028791 cc-mini-scikit-learn-0.1.2/supervised_learning/classification/
--rw-r--r--   0 mac        (501) staff       (20)     6719 2024-06-02 21:17:12.000000 cc-mini-scikit-learn-0.1.2/supervised_learning/classification/DecisionTreeClassifier.py
--rw-r--r--   0 mac        (501) staff       (20)     3339 2024-06-02 21:16:04.000000 cc-mini-scikit-learn-0.1.2/supervised_learning/classification/KNNClassifier.py
--rw-r--r--   0 mac        (501) staff       (20)     5232 2024-06-02 21:14:23.000000 cc-mini-scikit-learn-0.1.2/supervised_learning/classification/LogisticRegression.py
--rw-r--r--   0 mac        (501) staff       (20)     2722 2024-06-02 21:54:57.000000 cc-mini-scikit-learn-0.1.2/supervised_learning/classification/NaiveBayes.py
--rw-r--r--   0 mac        (501) staff       (20)     2291 2024-06-02 21:04:16.000000 cc-mini-scikit-learn-0.1.2/supervised_learning/classification/SVM.py
--rw-r--r--   0 mac        (501) staff       (20)      206 2024-06-02 20:58:44.000000 cc-mini-scikit-learn-0.1.2/supervised_learning/classification/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-02 23:12:57.033212 cc-mini-scikit-learn-0.1.2/supervised_learning/regression/
--rw-r--r--   0 mac        (501) staff       (20)     5598 2024-06-02 21:13:44.000000 cc-mini-scikit-learn-0.1.2/supervised_learning/regression/DecisionTreeRegressor.py
--rw-r--r--   0 mac        (501) staff       (20)     2368 2024-06-02 21:05:04.000000 cc-mini-scikit-learn-0.1.2/supervised_learning/regression/LinearRegression.py
--rw-r--r--   0 mac        (501) staff       (20)      104 2024-06-02 20:58:18.000000 cc-mini-scikit-learn-0.1.2/supervised_learning/regression/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-02 23:12:57.036635 cc-mini-scikit-learn-0.1.2/utilities/
--rw-r--r--   0 mac        (501) staff       (20)       94 2024-06-02 18:29:01.000000 cc-mini-scikit-learn-0.1.2/utilities/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)      825 2024-06-02 18:28:48.000000 cc-mini-scikit-learn-0.1.2/utilities/data_manipulation.py
--rw-r--r--   0 mac        (501) staff       (20)      355 2024-06-02 18:26:21.000000 cc-mini-scikit-learn-0.1.2/utilities/file_handling.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-02 23:19:07.815022 cc_mini_scikit_learn-0.1.3/
+-rw-r--r--   0 mac        (501) staff       (20)     2712 2024-06-02 23:19:07.814392 cc_mini_scikit_learn-0.1.3/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     2346 2024-05-22 21:15:43.000000 cc_mini_scikit_learn-0.1.3/README.md
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-02 23:19:07.634419 cc_mini_scikit_learn-0.1.3/cc_mini_scikit_learn.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)     2712 2024-06-02 23:19:07.000000 cc_mini_scikit_learn-0.1.3/cc_mini_scikit_learn.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     1795 2024-06-02 23:19:07.000000 cc_mini_scikit_learn-0.1.3/cc_mini_scikit_learn.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2024-06-02 23:19:07.000000 cc_mini_scikit_learn-0.1.3/cc_mini_scikit_learn.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)       25 2024-06-02 23:19:07.000000 cc_mini_scikit_learn-0.1.3/cc_mini_scikit_learn.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)       93 2024-06-02 23:19:07.000000 cc_mini_scikit_learn-0.1.3/cc_mini_scikit_learn.egg-info/top_level.txt
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-02 23:19:07.650388 cc_mini_scikit_learn-0.1.3/ensemble/
+-rw-r--r--   0 mac        (501) staff       (20)     4283 2024-06-02 21:46:43.000000 cc_mini_scikit_learn-0.1.3/ensemble/AdaBoost.py
+-rw-r--r--   0 mac        (501) staff       (20)     4689 2024-06-02 21:21:42.000000 cc_mini_scikit_learn-0.1.3/ensemble/GradientBoostingClassifier.py
+-rw-r--r--   0 mac        (501) staff       (20)     3705 2024-06-02 21:22:38.000000 cc_mini_scikit_learn-0.1.3/ensemble/GradientBoostingRegressor.py
+-rw-r--r--   0 mac        (501) staff       (20)     5053 2024-06-02 21:23:06.000000 cc_mini_scikit_learn-0.1.3/ensemble/RandomForestClassifier.py
+-rw-r--r--   0 mac        (501) staff       (20)     4000 2024-06-02 21:24:02.000000 cc_mini_scikit_learn-0.1.3/ensemble/RandomForestRegressor.py
+-rw-r--r--   0 mac        (501) staff       (20)     3882 2024-06-02 21:24:41.000000 cc_mini_scikit_learn-0.1.3/ensemble/StackingClassifier.py
+-rw-r--r--   0 mac        (501) staff       (20)     3094 2024-06-02 21:25:08.000000 cc_mini_scikit_learn-0.1.3/ensemble/VotingClassifier.py
+-rw-r--r--   0 mac        (501) staff       (20)      245 2024-06-02 20:58:50.000000 cc_mini_scikit_learn-0.1.3/ensemble/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-02 23:19:07.682782 cc_mini_scikit_learn-0.1.3/metrics/
+-rw-r--r--   0 mac        (501) staff       (20)      846 2024-06-02 20:32:40.000000 cc_mini_scikit_learn-0.1.3/metrics/Accuracy.py
+-rw-r--r--   0 mac        (501) staff       (20)      657 2024-06-02 20:33:25.000000 cc_mini_scikit_learn-0.1.3/metrics/BaseMetric.py
+-rw-r--r--   0 mac        (501) staff       (20)     1127 2024-06-02 20:34:14.000000 cc_mini_scikit_learn-0.1.3/metrics/ConfusionMatrix.py
+-rw-r--r--   0 mac        (501) staff       (20)      937 2024-06-02 20:34:23.000000 cc_mini_scikit_learn-0.1.3/metrics/F1Score.py
+-rw-r--r--   0 mac        (501) staff       (20)      742 2024-06-02 20:34:35.000000 cc_mini_scikit_learn-0.1.3/metrics/MeanAbsoluteError.py
+-rw-r--r--   0 mac        (501) staff       (20)      736 2024-06-02 20:35:27.000000 cc_mini_scikit_learn-0.1.3/metrics/MeanSquaredError.py
+-rw-r--r--   0 mac        (501) staff       (20)      910 2024-06-02 20:35:39.000000 cc_mini_scikit_learn-0.1.3/metrics/Precision.py
+-rw-r--r--   0 mac        (501) staff       (20)      901 2024-06-02 20:36:41.000000 cc_mini_scikit_learn-0.1.3/metrics/RSquared.py
+-rw-r--r--   0 mac        (501) staff       (20)      888 2024-06-02 20:35:49.000000 cc_mini_scikit_learn-0.1.3/metrics/Recall.py
+-rw-r--r--   0 mac        (501) staff       (20)      805 2024-06-02 20:35:58.000000 cc_mini_scikit_learn-0.1.3/metrics/RootMeanSquaredError.py
+-rw-r--r--   0 mac        (501) staff       (20)      381 2024-06-02 18:18:52.000000 cc_mini_scikit_learn-0.1.3/metrics/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-02 23:19:07.698868 cc_mini_scikit_learn-0.1.3/model_selection/
+-rw-r--r--   0 mac        (501) staff       (20)     4012 2024-06-02 21:49:06.000000 cc_mini_scikit_learn-0.1.3/model_selection/GridSearchCV.py
+-rw-r--r--   0 mac        (501) staff       (20)     2154 2024-06-02 21:28:12.000000 cc_mini_scikit_learn-0.1.3/model_selection/KFold.py
+-rw-r--r--   0 mac        (501) staff       (20)      967 2024-06-02 21:28:00.000000 cc_mini_scikit_learn-0.1.3/model_selection/ParameterGrid.py
+-rw-r--r--   0 mac        (501) staff       (20)      151 2024-06-02 18:19:39.000000 cc_mini_scikit_learn-0.1.3/model_selection/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     3797 2024-06-02 21:51:24.000000 cc_mini_scikit_learn-0.1.3/model_selection/train_test_split.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-02 23:19:07.707742 cc_mini_scikit_learn-0.1.3/neural_networks/
+-rw-r--r--   0 mac        (501) staff       (20)     3875 2024-06-02 21:28:42.000000 cc_mini_scikit_learn-0.1.3/neural_networks/MLP.py
+-rw-r--r--   0 mac        (501) staff       (20)     7182 2024-06-02 21:29:49.000000 cc_mini_scikit_learn-0.1.3/neural_networks/MLPRegressor.py
+-rw-r--r--   0 mac        (501) staff       (20)     3025 2024-06-02 21:30:03.000000 cc_mini_scikit_learn-0.1.3/neural_networks/Perceptron.py
+-rw-r--r--   0 mac        (501) staff       (20)       60 2024-06-02 18:20:00.000000 cc_mini_scikit_learn-0.1.3/neural_networks/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-02 23:19:07.727712 cc_mini_scikit_learn-0.1.3/preprocessing/
+-rw-r--r--   0 mac        (501) staff       (20)     2825 2024-06-02 21:31:50.000000 cc_mini_scikit_learn-0.1.3/preprocessing/LabelEncoder.py
+-rw-r--r--   0 mac        (501) staff       (20)     2317 2024-06-02 21:32:10.000000 cc_mini_scikit_learn-0.1.3/preprocessing/MinMaxScaler.py
+-rw-r--r--   0 mac        (501) staff       (20)     2468 2024-06-02 21:32:27.000000 cc_mini_scikit_learn-0.1.3/preprocessing/OneHotEncoder.py
+-rw-r--r--   0 mac        (501) staff       (20)     3041 2024-06-02 21:34:15.000000 cc_mini_scikit_learn-0.1.3/preprocessing/SimpleImputer.py
+-rw-r--r--   0 mac        (501) staff       (20)     2333 2024-06-02 21:34:44.000000 cc_mini_scikit_learn-0.1.3/preprocessing/StandardScaler.py
+-rw-r--r--   0 mac        (501) staff       (20)      202 2024-06-02 18:20:46.000000 cc_mini_scikit_learn-0.1.3/preprocessing/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)       38 2024-06-02 23:19:07.815228 cc_mini_scikit_learn-0.1.3/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)      587 2024-06-02 23:18:59.000000 cc_mini_scikit_learn-0.1.3/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-02 23:19:07.735190 cc_mini_scikit_learn-0.1.3/supervised_learning/
+-rw-r--r--   0 mac        (501) staff       (20)     1810 2024-06-02 20:56:39.000000 cc_mini_scikit_learn-0.1.3/supervised_learning/BaseEstimator.py
+-rw-r--r--   0 mac        (501) staff       (20)       40 2024-06-02 18:23:05.000000 cc_mini_scikit_learn-0.1.3/supervised_learning/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-02 23:19:07.778351 cc_mini_scikit_learn-0.1.3/supervised_learning/classification/
+-rw-r--r--   0 mac        (501) staff       (20)     6719 2024-06-02 21:17:12.000000 cc_mini_scikit_learn-0.1.3/supervised_learning/classification/DecisionTreeClassifier.py
+-rw-r--r--   0 mac        (501) staff       (20)     3339 2024-06-02 21:16:04.000000 cc_mini_scikit_learn-0.1.3/supervised_learning/classification/KNNClassifier.py
+-rw-r--r--   0 mac        (501) staff       (20)     5232 2024-06-02 21:14:23.000000 cc_mini_scikit_learn-0.1.3/supervised_learning/classification/LogisticRegression.py
+-rw-r--r--   0 mac        (501) staff       (20)     2722 2024-06-02 21:54:57.000000 cc_mini_scikit_learn-0.1.3/supervised_learning/classification/NaiveBayes.py
+-rw-r--r--   0 mac        (501) staff       (20)     2291 2024-06-02 21:04:16.000000 cc_mini_scikit_learn-0.1.3/supervised_learning/classification/SVM.py
+-rw-r--r--   0 mac        (501) staff       (20)      206 2024-06-02 20:58:44.000000 cc_mini_scikit_learn-0.1.3/supervised_learning/classification/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-02 23:19:07.790436 cc_mini_scikit_learn-0.1.3/supervised_learning/regression/
+-rw-r--r--   0 mac        (501) staff       (20)     5598 2024-06-02 21:13:44.000000 cc_mini_scikit_learn-0.1.3/supervised_learning/regression/DecisionTreeRegressor.py
+-rw-r--r--   0 mac        (501) staff       (20)     2368 2024-06-02 21:05:04.000000 cc_mini_scikit_learn-0.1.3/supervised_learning/regression/LinearRegression.py
+-rw-r--r--   0 mac        (501) staff       (20)      104 2024-06-02 20:58:18.000000 cc_mini_scikit_learn-0.1.3/supervised_learning/regression/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-02 23:19:07.803987 cc_mini_scikit_learn-0.1.3/utilities/
+-rw-r--r--   0 mac        (501) staff       (20)       94 2024-06-02 18:29:01.000000 cc_mini_scikit_learn-0.1.3/utilities/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)      825 2024-06-02 18:28:48.000000 cc_mini_scikit_learn-0.1.3/utilities/data_manipulation.py
+-rw-r--r--   0 mac        (501) staff       (20)      355 2024-06-02 18:26:21.000000 cc_mini_scikit_learn-0.1.3/utilities/file_handling.py
```

### Comparing `cc-mini-scikit-learn-0.1.2/PKG-INFO` & `cc_mini_scikit_learn-0.1.3/cc_mini_scikit_learn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cc-mini-scikit-learn
-Version: 0.1.2
+Version: 0.1.3
 Summary: A minimal implementation of scikit-learn like functionalities
 Home-page: https://github.com/Basma-Arnaoui/Mini-Scikit-Learn/tree/main
 Author: basma-arnaoui
 Author-email: basma.arnaoui@um6p.ma
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `cc-mini-scikit-learn-0.1.2/README.md` & `cc_mini_scikit_learn-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.2/cc_mini_scikit_learn.egg-info/PKG-INFO` & `cc_mini_scikit_learn-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cc-mini-scikit-learn
-Version: 0.1.2
+Name: cc_mini_scikit_learn
+Version: 0.1.3
 Summary: A minimal implementation of scikit-learn like functionalities
 Home-page: https://github.com/Basma-Arnaoui/Mini-Scikit-Learn/tree/main
 Author: basma-arnaoui
 Author-email: basma.arnaoui@um6p.ma
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `cc-mini-scikit-learn-0.1.2/cc_mini_scikit_learn.egg-info/SOURCES.txt` & `cc_mini_scikit_learn-0.1.3/cc_mini_scikit_learn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.2/ensemble/AdaBoost.py` & `cc_mini_scikit_learn-0.1.3/ensemble/AdaBoost.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.2/ensemble/GradientBoostingClassifier.py` & `cc_mini_scikit_learn-0.1.3/ensemble/GradientBoostingClassifier.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.2/ensemble/GradientBoostingRegressor.py` & `cc_mini_scikit_learn-0.1.3/ensemble/GradientBoostingRegressor.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.2/ensemble/RandomForestClassifier.py` & `cc_mini_scikit_learn-0.1.3/ensemble/RandomForestClassifier.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.2/ensemble/RandomForestRegressor.py` & `cc_mini_scikit_learn-0.1.3/ensemble/RandomForestRegressor.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.2/ensemble/StackingClassifier.py` & `cc_mini_scikit_learn-0.1.3/ensemble/StackingClassifier.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.2/ensemble/VotingClassifier.py` & `cc_mini_scikit_learn-0.1.3/ensemble/VotingClassifier.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.2/metrics/Accuracy.py` & `cc_mini_scikit_learn-0.1.3/metrics/Accuracy.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.2/metrics/BaseMetric.py` & `cc_mini_scikit_learn-0.1.3/metrics/BaseMetric.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.2/metrics/ConfusionMatrix.py` & `cc_mini_scikit_learn-0.1.3/metrics/ConfusionMatrix.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.2/metrics/F1Score.py` & `cc_mini_scikit_learn-0.1.3/metrics/F1Score.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.2/metrics/MeanAbsoluteError.py` & `cc_mini_scikit_learn-0.1.3/metrics/MeanAbsoluteError.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.2/metrics/MeanSquaredError.py` & `cc_mini_scikit_learn-0.1.3/metrics/MeanSquaredError.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.2/metrics/Precision.py` & `cc_mini_scikit_learn-0.1.3/metrics/Precision.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.2/metrics/RSquared.py` & `cc_mini_scikit_learn-0.1.3/metrics/RSquared.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.2/metrics/Recall.py` & `cc_mini_scikit_learn-0.1.3/metrics/Recall.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.2/metrics/RootMeanSquaredError.py` & `cc_mini_scikit_learn-0.1.3/metrics/RootMeanSquaredError.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.2/model_selection/GridSearchCV.py` & `cc_mini_scikit_learn-0.1.3/model_selection/GridSearchCV.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.2/model_selection/KFold.py` & `cc_mini_scikit_learn-0.1.3/model_selection/KFold.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.2/model_selection/ParameterGrid.py` & `cc_mini_scikit_learn-0.1.3/model_selection/ParameterGrid.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.2/model_selection/train_test_split.py` & `cc_mini_scikit_learn-0.1.3/model_selection/train_test_split.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.2/neural_networks/MLP.py` & `cc_mini_scikit_learn-0.1.3/neural_networks/MLP.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.2/neural_networks/MLPRegressor.py` & `cc_mini_scikit_learn-0.1.3/neural_networks/MLPRegressor.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.2/neural_networks/Perceptron.py` & `cc_mini_scikit_learn-0.1.3/neural_networks/Perceptron.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.2/preprocessing/LabelEncoder.py` & `cc_mini_scikit_learn-0.1.3/preprocessing/LabelEncoder.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.2/preprocessing/MinMaxScaler.py` & `cc_mini_scikit_learn-0.1.3/preprocessing/MinMaxScaler.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.2/preprocessing/OneHotEncoder.py` & `cc_mini_scikit_learn-0.1.3/preprocessing/OneHotEncoder.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.2/preprocessing/SimpleImputer.py` & `cc_mini_scikit_learn-0.1.3/preprocessing/SimpleImputer.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.2/preprocessing/StandardScaler.py` & `cc_mini_scikit_learn-0.1.3/preprocessing/StandardScaler.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.2/setup.py` & `cc_mini_scikit_learn-0.1.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
-    name='cc-mini-scikit-learn',
-    version='0.1.2',
+    name='cc_mini_scikit_learn',
+    version='0.1.3',
     author='basma-arnaoui',
     author_email='basma.arnaoui@um6p.ma',
     packages=find_packages(),
     install_requires=[
         'numpy',
         'scipy',
         'scikit-learn',
```

### Comparing `cc-mini-scikit-learn-0.1.2/supervised_learning/BaseEstimator.py` & `cc_mini_scikit_learn-0.1.3/supervised_learning/BaseEstimator.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.2/supervised_learning/classification/DecisionTreeClassifier.py` & `cc_mini_scikit_learn-0.1.3/supervised_learning/classification/DecisionTreeClassifier.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.2/supervised_learning/classification/KNNClassifier.py` & `cc_mini_scikit_learn-0.1.3/supervised_learning/classification/KNNClassifier.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.2/supervised_learning/classification/LogisticRegression.py` & `cc_mini_scikit_learn-0.1.3/supervised_learning/classification/LogisticRegression.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.2/supervised_learning/classification/NaiveBayes.py` & `cc_mini_scikit_learn-0.1.3/supervised_learning/classification/NaiveBayes.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.2/supervised_learning/classification/SVM.py` & `cc_mini_scikit_learn-0.1.3/supervised_learning/classification/SVM.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.2/supervised_learning/regression/DecisionTreeRegressor.py` & `cc_mini_scikit_learn-0.1.3/supervised_learning/regression/DecisionTreeRegressor.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.2/supervised_learning/regression/LinearRegression.py` & `cc_mini_scikit_learn-0.1.3/supervised_learning/regression/LinearRegression.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.2/utilities/data_manipulation.py` & `cc_mini_scikit_learn-0.1.3/utilities/data_manipulation.py`

 * *Files identical despite different names*

