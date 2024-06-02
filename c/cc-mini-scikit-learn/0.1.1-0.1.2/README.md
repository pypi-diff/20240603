# Comparing `tmp/cc-mini-scikit-learn-0.1.1.tar.gz` & `tmp/cc-mini-scikit-learn-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cc-mini-scikit-learn-0.1.1.tar", last modified: Sun Jun  2 23:03:51 2024, max compression
+gzip compressed data, was "cc-mini-scikit-learn-0.1.2.tar", last modified: Sun Jun  2 23:12:57 2024, max compression
```

## Comparing `cc-mini-scikit-learn-0.1.1.tar` & `cc-mini-scikit-learn-0.1.2.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-02 23:03:51.450182 cc-mini-scikit-learn-0.1.1/
--rw-r--r--   0 mac        (501) staff       (20)     2712 2024-06-02 23:03:51.449375 cc-mini-scikit-learn-0.1.1/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     2346 2024-05-22 21:15:43.000000 cc-mini-scikit-learn-0.1.1/README.md
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-02 23:03:51.367681 cc-mini-scikit-learn-0.1.1/cc_mini_scikit_learn.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)     2712 2024-06-02 23:03:51.000000 cc-mini-scikit-learn-0.1.1/cc_mini_scikit_learn.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     1795 2024-06-02 23:03:51.000000 cc-mini-scikit-learn-0.1.1/cc_mini_scikit_learn.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2024-06-02 23:03:51.000000 cc-mini-scikit-learn-0.1.1/cc_mini_scikit_learn.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)       20 2024-06-02 23:03:51.000000 cc-mini-scikit-learn-0.1.1/cc_mini_scikit_learn.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)       93 2024-06-02 23:03:51.000000 cc-mini-scikit-learn-0.1.1/cc_mini_scikit_learn.egg-info/top_level.txt
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-02 23:03:51.380289 cc-mini-scikit-learn-0.1.1/ensemble/
--rw-r--r--   0 mac        (501) staff       (20)     4283 2024-06-02 21:46:43.000000 cc-mini-scikit-learn-0.1.1/ensemble/AdaBoost.py
--rw-r--r--   0 mac        (501) staff       (20)     4689 2024-06-02 21:21:42.000000 cc-mini-scikit-learn-0.1.1/ensemble/GradientBoostingClassifier.py
--rw-r--r--   0 mac        (501) staff       (20)     3705 2024-06-02 21:22:38.000000 cc-mini-scikit-learn-0.1.1/ensemble/GradientBoostingRegressor.py
--rw-r--r--   0 mac        (501) staff       (20)     5053 2024-06-02 21:23:06.000000 cc-mini-scikit-learn-0.1.1/ensemble/RandomForestClassifier.py
--rw-r--r--   0 mac        (501) staff       (20)     4000 2024-06-02 21:24:02.000000 cc-mini-scikit-learn-0.1.1/ensemble/RandomForestRegressor.py
--rw-r--r--   0 mac        (501) staff       (20)     3882 2024-06-02 21:24:41.000000 cc-mini-scikit-learn-0.1.1/ensemble/StackingClassifier.py
--rw-r--r--   0 mac        (501) staff       (20)     3094 2024-06-02 21:25:08.000000 cc-mini-scikit-learn-0.1.1/ensemble/VotingClassifier.py
--rw-r--r--   0 mac        (501) staff       (20)      245 2024-06-02 20:58:50.000000 cc-mini-scikit-learn-0.1.1/ensemble/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-02 23:03:51.398272 cc-mini-scikit-learn-0.1.1/metrics/
--rw-r--r--   0 mac        (501) staff       (20)      846 2024-06-02 20:32:40.000000 cc-mini-scikit-learn-0.1.1/metrics/Accuracy.py
--rw-r--r--   0 mac        (501) staff       (20)      657 2024-06-02 20:33:25.000000 cc-mini-scikit-learn-0.1.1/metrics/BaseMetric.py
--rw-r--r--   0 mac        (501) staff       (20)     1127 2024-06-02 20:34:14.000000 cc-mini-scikit-learn-0.1.1/metrics/ConfusionMatrix.py
--rw-r--r--   0 mac        (501) staff       (20)      937 2024-06-02 20:34:23.000000 cc-mini-scikit-learn-0.1.1/metrics/F1Score.py
--rw-r--r--   0 mac        (501) staff       (20)      742 2024-06-02 20:34:35.000000 cc-mini-scikit-learn-0.1.1/metrics/MeanAbsoluteError.py
--rw-r--r--   0 mac        (501) staff       (20)      736 2024-06-02 20:35:27.000000 cc-mini-scikit-learn-0.1.1/metrics/MeanSquaredError.py
--rw-r--r--   0 mac        (501) staff       (20)      910 2024-06-02 20:35:39.000000 cc-mini-scikit-learn-0.1.1/metrics/Precision.py
--rw-r--r--   0 mac        (501) staff       (20)      901 2024-06-02 20:36:41.000000 cc-mini-scikit-learn-0.1.1/metrics/RSquared.py
--rw-r--r--   0 mac        (501) staff       (20)      888 2024-06-02 20:35:49.000000 cc-mini-scikit-learn-0.1.1/metrics/Recall.py
--rw-r--r--   0 mac        (501) staff       (20)      805 2024-06-02 20:35:58.000000 cc-mini-scikit-learn-0.1.1/metrics/RootMeanSquaredError.py
--rw-r--r--   0 mac        (501) staff       (20)      381 2024-06-02 18:18:52.000000 cc-mini-scikit-learn-0.1.1/metrics/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-02 23:03:51.406304 cc-mini-scikit-learn-0.1.1/model_selection/
--rw-r--r--   0 mac        (501) staff       (20)     4012 2024-06-02 21:49:06.000000 cc-mini-scikit-learn-0.1.1/model_selection/GridSearchCV.py
--rw-r--r--   0 mac        (501) staff       (20)     2154 2024-06-02 21:28:12.000000 cc-mini-scikit-learn-0.1.1/model_selection/KFold.py
--rw-r--r--   0 mac        (501) staff       (20)      967 2024-06-02 21:28:00.000000 cc-mini-scikit-learn-0.1.1/model_selection/ParameterGrid.py
--rw-r--r--   0 mac        (501) staff       (20)      151 2024-06-02 18:19:39.000000 cc-mini-scikit-learn-0.1.1/model_selection/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     3797 2024-06-02 21:51:24.000000 cc-mini-scikit-learn-0.1.1/model_selection/train_test_split.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-02 23:03:51.416262 cc-mini-scikit-learn-0.1.1/neural_networks/
--rw-r--r--   0 mac        (501) staff       (20)     3875 2024-06-02 21:28:42.000000 cc-mini-scikit-learn-0.1.1/neural_networks/MLP.py
--rw-r--r--   0 mac        (501) staff       (20)     7182 2024-06-02 21:29:49.000000 cc-mini-scikit-learn-0.1.1/neural_networks/MLPRegressor.py
--rw-r--r--   0 mac        (501) staff       (20)     3025 2024-06-02 21:30:03.000000 cc-mini-scikit-learn-0.1.1/neural_networks/Perceptron.py
--rw-r--r--   0 mac        (501) staff       (20)       60 2024-06-02 18:20:00.000000 cc-mini-scikit-learn-0.1.1/neural_networks/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-02 23:03:51.426385 cc-mini-scikit-learn-0.1.1/preprocessing/
--rw-r--r--   0 mac        (501) staff       (20)     2825 2024-06-02 21:31:50.000000 cc-mini-scikit-learn-0.1.1/preprocessing/LabelEncoder.py
--rw-r--r--   0 mac        (501) staff       (20)     2317 2024-06-02 21:32:10.000000 cc-mini-scikit-learn-0.1.1/preprocessing/MinMaxScaler.py
--rw-r--r--   0 mac        (501) staff       (20)     2468 2024-06-02 21:32:27.000000 cc-mini-scikit-learn-0.1.1/preprocessing/OneHotEncoder.py
--rw-r--r--   0 mac        (501) staff       (20)     3041 2024-06-02 21:34:15.000000 cc-mini-scikit-learn-0.1.1/preprocessing/SimpleImputer.py
--rw-r--r--   0 mac        (501) staff       (20)     2333 2024-06-02 21:34:44.000000 cc-mini-scikit-learn-0.1.1/preprocessing/StandardScaler.py
--rw-r--r--   0 mac        (501) staff       (20)      202 2024-06-02 18:20:46.000000 cc-mini-scikit-learn-0.1.1/preprocessing/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)       38 2024-06-02 23:03:51.450447 cc-mini-scikit-learn-0.1.1/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)      573 2024-06-02 23:00:05.000000 cc-mini-scikit-learn-0.1.1/setup.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-02 23:03:51.429288 cc-mini-scikit-learn-0.1.1/supervised_learning/
--rw-r--r--   0 mac        (501) staff       (20)     1810 2024-06-02 20:56:39.000000 cc-mini-scikit-learn-0.1.1/supervised_learning/BaseEstimator.py
--rw-r--r--   0 mac        (501) staff       (20)       40 2024-06-02 18:23:05.000000 cc-mini-scikit-learn-0.1.1/supervised_learning/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-02 23:03:51.438660 cc-mini-scikit-learn-0.1.1/supervised_learning/classification/
--rw-r--r--   0 mac        (501) staff       (20)     6719 2024-06-02 21:17:12.000000 cc-mini-scikit-learn-0.1.1/supervised_learning/classification/DecisionTreeClassifier.py
--rw-r--r--   0 mac        (501) staff       (20)     3339 2024-06-02 21:16:04.000000 cc-mini-scikit-learn-0.1.1/supervised_learning/classification/KNNClassifier.py
--rw-r--r--   0 mac        (501) staff       (20)     5232 2024-06-02 21:14:23.000000 cc-mini-scikit-learn-0.1.1/supervised_learning/classification/LogisticRegression.py
--rw-r--r--   0 mac        (501) staff       (20)     2722 2024-06-02 21:54:57.000000 cc-mini-scikit-learn-0.1.1/supervised_learning/classification/NaiveBayes.py
--rw-r--r--   0 mac        (501) staff       (20)     2291 2024-06-02 21:04:16.000000 cc-mini-scikit-learn-0.1.1/supervised_learning/classification/SVM.py
--rw-r--r--   0 mac        (501) staff       (20)      206 2024-06-02 20:58:44.000000 cc-mini-scikit-learn-0.1.1/supervised_learning/classification/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-02 23:03:51.443024 cc-mini-scikit-learn-0.1.1/supervised_learning/regression/
--rw-r--r--   0 mac        (501) staff       (20)     5598 2024-06-02 21:13:44.000000 cc-mini-scikit-learn-0.1.1/supervised_learning/regression/DecisionTreeRegressor.py
--rw-r--r--   0 mac        (501) staff       (20)     2368 2024-06-02 21:05:04.000000 cc-mini-scikit-learn-0.1.1/supervised_learning/regression/LinearRegression.py
--rw-r--r--   0 mac        (501) staff       (20)      104 2024-06-02 20:58:18.000000 cc-mini-scikit-learn-0.1.1/supervised_learning/regression/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-02 23:03:51.447875 cc-mini-scikit-learn-0.1.1/utilities/
--rw-r--r--   0 mac        (501) staff       (20)       94 2024-06-02 18:29:01.000000 cc-mini-scikit-learn-0.1.1/utilities/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)      825 2024-06-02 18:28:48.000000 cc-mini-scikit-learn-0.1.1/utilities/data_manipulation.py
--rw-r--r--   0 mac        (501) staff       (20)      355 2024-06-02 18:26:21.000000 cc-mini-scikit-learn-0.1.1/utilities/file_handling.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-02 23:12:57.039051 cc-mini-scikit-learn-0.1.2/
+-rw-r--r--   0 mac        (501) staff       (20)     2712 2024-06-02 23:12:57.038012 cc-mini-scikit-learn-0.1.2/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     2346 2024-05-22 21:15:43.000000 cc-mini-scikit-learn-0.1.2/README.md
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-02 23:12:56.729741 cc-mini-scikit-learn-0.1.2/cc_mini_scikit_learn.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)     2712 2024-06-02 23:12:56.000000 cc-mini-scikit-learn-0.1.2/cc_mini_scikit_learn.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     1795 2024-06-02 23:12:56.000000 cc-mini-scikit-learn-0.1.2/cc_mini_scikit_learn.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2024-06-02 23:12:56.000000 cc-mini-scikit-learn-0.1.2/cc_mini_scikit_learn.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)       25 2024-06-02 23:12:56.000000 cc-mini-scikit-learn-0.1.2/cc_mini_scikit_learn.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)       93 2024-06-02 23:12:56.000000 cc-mini-scikit-learn-0.1.2/cc_mini_scikit_learn.egg-info/top_level.txt
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-02 23:12:56.786225 cc-mini-scikit-learn-0.1.2/ensemble/
+-rw-r--r--   0 mac        (501) staff       (20)     4283 2024-06-02 21:46:43.000000 cc-mini-scikit-learn-0.1.2/ensemble/AdaBoost.py
+-rw-r--r--   0 mac        (501) staff       (20)     4689 2024-06-02 21:21:42.000000 cc-mini-scikit-learn-0.1.2/ensemble/GradientBoostingClassifier.py
+-rw-r--r--   0 mac        (501) staff       (20)     3705 2024-06-02 21:22:38.000000 cc-mini-scikit-learn-0.1.2/ensemble/GradientBoostingRegressor.py
+-rw-r--r--   0 mac        (501) staff       (20)     5053 2024-06-02 21:23:06.000000 cc-mini-scikit-learn-0.1.2/ensemble/RandomForestClassifier.py
+-rw-r--r--   0 mac        (501) staff       (20)     4000 2024-06-02 21:24:02.000000 cc-mini-scikit-learn-0.1.2/ensemble/RandomForestRegressor.py
+-rw-r--r--   0 mac        (501) staff       (20)     3882 2024-06-02 21:24:41.000000 cc-mini-scikit-learn-0.1.2/ensemble/StackingClassifier.py
+-rw-r--r--   0 mac        (501) staff       (20)     3094 2024-06-02 21:25:08.000000 cc-mini-scikit-learn-0.1.2/ensemble/VotingClassifier.py
+-rw-r--r--   0 mac        (501) staff       (20)      245 2024-06-02 20:58:50.000000 cc-mini-scikit-learn-0.1.2/ensemble/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-02 23:12:56.850013 cc-mini-scikit-learn-0.1.2/metrics/
+-rw-r--r--   0 mac        (501) staff       (20)      846 2024-06-02 20:32:40.000000 cc-mini-scikit-learn-0.1.2/metrics/Accuracy.py
+-rw-r--r--   0 mac        (501) staff       (20)      657 2024-06-02 20:33:25.000000 cc-mini-scikit-learn-0.1.2/metrics/BaseMetric.py
+-rw-r--r--   0 mac        (501) staff       (20)     1127 2024-06-02 20:34:14.000000 cc-mini-scikit-learn-0.1.2/metrics/ConfusionMatrix.py
+-rw-r--r--   0 mac        (501) staff       (20)      937 2024-06-02 20:34:23.000000 cc-mini-scikit-learn-0.1.2/metrics/F1Score.py
+-rw-r--r--   0 mac        (501) staff       (20)      742 2024-06-02 20:34:35.000000 cc-mini-scikit-learn-0.1.2/metrics/MeanAbsoluteError.py
+-rw-r--r--   0 mac        (501) staff       (20)      736 2024-06-02 20:35:27.000000 cc-mini-scikit-learn-0.1.2/metrics/MeanSquaredError.py
+-rw-r--r--   0 mac        (501) staff       (20)      910 2024-06-02 20:35:39.000000 cc-mini-scikit-learn-0.1.2/metrics/Precision.py
+-rw-r--r--   0 mac        (501) staff       (20)      901 2024-06-02 20:36:41.000000 cc-mini-scikit-learn-0.1.2/metrics/RSquared.py
+-rw-r--r--   0 mac        (501) staff       (20)      888 2024-06-02 20:35:49.000000 cc-mini-scikit-learn-0.1.2/metrics/Recall.py
+-rw-r--r--   0 mac        (501) staff       (20)      805 2024-06-02 20:35:58.000000 cc-mini-scikit-learn-0.1.2/metrics/RootMeanSquaredError.py
+-rw-r--r--   0 mac        (501) staff       (20)      381 2024-06-02 18:18:52.000000 cc-mini-scikit-learn-0.1.2/metrics/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-02 23:12:56.987132 cc-mini-scikit-learn-0.1.2/model_selection/
+-rw-r--r--   0 mac        (501) staff       (20)     4012 2024-06-02 21:49:06.000000 cc-mini-scikit-learn-0.1.2/model_selection/GridSearchCV.py
+-rw-r--r--   0 mac        (501) staff       (20)     2154 2024-06-02 21:28:12.000000 cc-mini-scikit-learn-0.1.2/model_selection/KFold.py
+-rw-r--r--   0 mac        (501) staff       (20)      967 2024-06-02 21:28:00.000000 cc-mini-scikit-learn-0.1.2/model_selection/ParameterGrid.py
+-rw-r--r--   0 mac        (501) staff       (20)      151 2024-06-02 18:19:39.000000 cc-mini-scikit-learn-0.1.2/model_selection/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     3797 2024-06-02 21:51:24.000000 cc-mini-scikit-learn-0.1.2/model_selection/train_test_split.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-02 23:12:56.998818 cc-mini-scikit-learn-0.1.2/neural_networks/
+-rw-r--r--   0 mac        (501) staff       (20)     3875 2024-06-02 21:28:42.000000 cc-mini-scikit-learn-0.1.2/neural_networks/MLP.py
+-rw-r--r--   0 mac        (501) staff       (20)     7182 2024-06-02 21:29:49.000000 cc-mini-scikit-learn-0.1.2/neural_networks/MLPRegressor.py
+-rw-r--r--   0 mac        (501) staff       (20)     3025 2024-06-02 21:30:03.000000 cc-mini-scikit-learn-0.1.2/neural_networks/Perceptron.py
+-rw-r--r--   0 mac        (501) staff       (20)       60 2024-06-02 18:20:00.000000 cc-mini-scikit-learn-0.1.2/neural_networks/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-02 23:12:57.014963 cc-mini-scikit-learn-0.1.2/preprocessing/
+-rw-r--r--   0 mac        (501) staff       (20)     2825 2024-06-02 21:31:50.000000 cc-mini-scikit-learn-0.1.2/preprocessing/LabelEncoder.py
+-rw-r--r--   0 mac        (501) staff       (20)     2317 2024-06-02 21:32:10.000000 cc-mini-scikit-learn-0.1.2/preprocessing/MinMaxScaler.py
+-rw-r--r--   0 mac        (501) staff       (20)     2468 2024-06-02 21:32:27.000000 cc-mini-scikit-learn-0.1.2/preprocessing/OneHotEncoder.py
+-rw-r--r--   0 mac        (501) staff       (20)     3041 2024-06-02 21:34:15.000000 cc-mini-scikit-learn-0.1.2/preprocessing/SimpleImputer.py
+-rw-r--r--   0 mac        (501) staff       (20)     2333 2024-06-02 21:34:44.000000 cc-mini-scikit-learn-0.1.2/preprocessing/StandardScaler.py
+-rw-r--r--   0 mac        (501) staff       (20)      202 2024-06-02 18:20:46.000000 cc-mini-scikit-learn-0.1.2/preprocessing/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)       38 2024-06-02 23:12:57.041452 cc-mini-scikit-learn-0.1.2/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)      587 2024-06-02 23:12:49.000000 cc-mini-scikit-learn-0.1.2/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-02 23:12:57.019544 cc-mini-scikit-learn-0.1.2/supervised_learning/
+-rw-r--r--   0 mac        (501) staff       (20)     1810 2024-06-02 20:56:39.000000 cc-mini-scikit-learn-0.1.2/supervised_learning/BaseEstimator.py
+-rw-r--r--   0 mac        (501) staff       (20)       40 2024-06-02 18:23:05.000000 cc-mini-scikit-learn-0.1.2/supervised_learning/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-02 23:12:57.028791 cc-mini-scikit-learn-0.1.2/supervised_learning/classification/
+-rw-r--r--   0 mac        (501) staff       (20)     6719 2024-06-02 21:17:12.000000 cc-mini-scikit-learn-0.1.2/supervised_learning/classification/DecisionTreeClassifier.py
+-rw-r--r--   0 mac        (501) staff       (20)     3339 2024-06-02 21:16:04.000000 cc-mini-scikit-learn-0.1.2/supervised_learning/classification/KNNClassifier.py
+-rw-r--r--   0 mac        (501) staff       (20)     5232 2024-06-02 21:14:23.000000 cc-mini-scikit-learn-0.1.2/supervised_learning/classification/LogisticRegression.py
+-rw-r--r--   0 mac        (501) staff       (20)     2722 2024-06-02 21:54:57.000000 cc-mini-scikit-learn-0.1.2/supervised_learning/classification/NaiveBayes.py
+-rw-r--r--   0 mac        (501) staff       (20)     2291 2024-06-02 21:04:16.000000 cc-mini-scikit-learn-0.1.2/supervised_learning/classification/SVM.py
+-rw-r--r--   0 mac        (501) staff       (20)      206 2024-06-02 20:58:44.000000 cc-mini-scikit-learn-0.1.2/supervised_learning/classification/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-02 23:12:57.033212 cc-mini-scikit-learn-0.1.2/supervised_learning/regression/
+-rw-r--r--   0 mac        (501) staff       (20)     5598 2024-06-02 21:13:44.000000 cc-mini-scikit-learn-0.1.2/supervised_learning/regression/DecisionTreeRegressor.py
+-rw-r--r--   0 mac        (501) staff       (20)     2368 2024-06-02 21:05:04.000000 cc-mini-scikit-learn-0.1.2/supervised_learning/regression/LinearRegression.py
+-rw-r--r--   0 mac        (501) staff       (20)      104 2024-06-02 20:58:18.000000 cc-mini-scikit-learn-0.1.2/supervised_learning/regression/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-02 23:12:57.036635 cc-mini-scikit-learn-0.1.2/utilities/
+-rw-r--r--   0 mac        (501) staff       (20)       94 2024-06-02 18:29:01.000000 cc-mini-scikit-learn-0.1.2/utilities/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)      825 2024-06-02 18:28:48.000000 cc-mini-scikit-learn-0.1.2/utilities/data_manipulation.py
+-rw-r--r--   0 mac        (501) staff       (20)      355 2024-06-02 18:26:21.000000 cc-mini-scikit-learn-0.1.2/utilities/file_handling.py
```

### Comparing `cc-mini-scikit-learn-0.1.1/PKG-INFO` & `cc-mini-scikit-learn-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cc-mini-scikit-learn
-Version: 0.1.1
+Version: 0.1.2
 Summary: A minimal implementation of scikit-learn like functionalities
 Home-page: https://github.com/Basma-Arnaoui/Mini-Scikit-Learn/tree/main
 Author: basma-arnaoui
 Author-email: basma.arnaoui@um6p.ma
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `cc-mini-scikit-learn-0.1.1/README.md` & `cc-mini-scikit-learn-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.1/cc_mini_scikit_learn.egg-info/PKG-INFO` & `cc-mini-scikit-learn-0.1.2/cc_mini_scikit_learn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cc-mini-scikit-learn
-Version: 0.1.1
+Version: 0.1.2
 Summary: A minimal implementation of scikit-learn like functionalities
 Home-page: https://github.com/Basma-Arnaoui/Mini-Scikit-Learn/tree/main
 Author: basma-arnaoui
 Author-email: basma.arnaoui@um6p.ma
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `cc-mini-scikit-learn-0.1.1/cc_mini_scikit_learn.egg-info/SOURCES.txt` & `cc-mini-scikit-learn-0.1.2/cc_mini_scikit_learn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.1/ensemble/AdaBoost.py` & `cc-mini-scikit-learn-0.1.2/ensemble/AdaBoost.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.1/ensemble/GradientBoostingClassifier.py` & `cc-mini-scikit-learn-0.1.2/ensemble/GradientBoostingClassifier.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.1/ensemble/GradientBoostingRegressor.py` & `cc-mini-scikit-learn-0.1.2/ensemble/GradientBoostingRegressor.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.1/ensemble/RandomForestClassifier.py` & `cc-mini-scikit-learn-0.1.2/ensemble/RandomForestClassifier.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.1/ensemble/RandomForestRegressor.py` & `cc-mini-scikit-learn-0.1.2/ensemble/RandomForestRegressor.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.1/ensemble/StackingClassifier.py` & `cc-mini-scikit-learn-0.1.2/ensemble/StackingClassifier.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.1/ensemble/VotingClassifier.py` & `cc-mini-scikit-learn-0.1.2/ensemble/VotingClassifier.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.1/metrics/Accuracy.py` & `cc-mini-scikit-learn-0.1.2/metrics/Accuracy.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.1/metrics/BaseMetric.py` & `cc-mini-scikit-learn-0.1.2/metrics/BaseMetric.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.1/metrics/ConfusionMatrix.py` & `cc-mini-scikit-learn-0.1.2/metrics/ConfusionMatrix.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.1/metrics/F1Score.py` & `cc-mini-scikit-learn-0.1.2/metrics/F1Score.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.1/metrics/MeanAbsoluteError.py` & `cc-mini-scikit-learn-0.1.2/metrics/MeanAbsoluteError.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.1/metrics/MeanSquaredError.py` & `cc-mini-scikit-learn-0.1.2/metrics/MeanSquaredError.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.1/metrics/Precision.py` & `cc-mini-scikit-learn-0.1.2/metrics/Precision.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.1/metrics/RSquared.py` & `cc-mini-scikit-learn-0.1.2/metrics/RSquared.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.1/metrics/Recall.py` & `cc-mini-scikit-learn-0.1.2/metrics/Recall.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.1/metrics/RootMeanSquaredError.py` & `cc-mini-scikit-learn-0.1.2/metrics/RootMeanSquaredError.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.1/model_selection/GridSearchCV.py` & `cc-mini-scikit-learn-0.1.2/model_selection/GridSearchCV.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.1/model_selection/KFold.py` & `cc-mini-scikit-learn-0.1.2/model_selection/KFold.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.1/model_selection/ParameterGrid.py` & `cc-mini-scikit-learn-0.1.2/model_selection/ParameterGrid.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.1/model_selection/train_test_split.py` & `cc-mini-scikit-learn-0.1.2/model_selection/train_test_split.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.1/neural_networks/MLP.py` & `cc-mini-scikit-learn-0.1.2/neural_networks/MLP.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.1/neural_networks/MLPRegressor.py` & `cc-mini-scikit-learn-0.1.2/neural_networks/MLPRegressor.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.1/neural_networks/Perceptron.py` & `cc-mini-scikit-learn-0.1.2/neural_networks/Perceptron.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.1/preprocessing/LabelEncoder.py` & `cc-mini-scikit-learn-0.1.2/preprocessing/LabelEncoder.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.1/preprocessing/MinMaxScaler.py` & `cc-mini-scikit-learn-0.1.2/preprocessing/MinMaxScaler.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.1/preprocessing/OneHotEncoder.py` & `cc-mini-scikit-learn-0.1.2/preprocessing/OneHotEncoder.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.1/preprocessing/SimpleImputer.py` & `cc-mini-scikit-learn-0.1.2/preprocessing/SimpleImputer.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.1/preprocessing/StandardScaler.py` & `cc-mini-scikit-learn-0.1.2/preprocessing/StandardScaler.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.1/setup.py` & `cc-mini-scikit-learn-0.1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cc-mini-scikit-learn',
-    version='0.1.1',
+    version='0.1.2',
     author='basma-arnaoui',
     author_email='basma.arnaoui@um6p.ma',
     packages=find_packages(),
     install_requires=[
         'numpy',
         'scipy',
-        'sklearn',  
+        'scikit-learn', 
+         
     ],
     python_requires='>=3.6',
     description='A minimal implementation of scikit-learn like functionalities',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/Basma-Arnaoui/Mini-Scikit-Learn/tree/main',
 )
```

### Comparing `cc-mini-scikit-learn-0.1.1/supervised_learning/BaseEstimator.py` & `cc-mini-scikit-learn-0.1.2/supervised_learning/BaseEstimator.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.1/supervised_learning/classification/DecisionTreeClassifier.py` & `cc-mini-scikit-learn-0.1.2/supervised_learning/classification/DecisionTreeClassifier.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.1/supervised_learning/classification/KNNClassifier.py` & `cc-mini-scikit-learn-0.1.2/supervised_learning/classification/KNNClassifier.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.1/supervised_learning/classification/LogisticRegression.py` & `cc-mini-scikit-learn-0.1.2/supervised_learning/classification/LogisticRegression.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.1/supervised_learning/classification/NaiveBayes.py` & `cc-mini-scikit-learn-0.1.2/supervised_learning/classification/NaiveBayes.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.1/supervised_learning/classification/SVM.py` & `cc-mini-scikit-learn-0.1.2/supervised_learning/classification/SVM.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.1/supervised_learning/regression/DecisionTreeRegressor.py` & `cc-mini-scikit-learn-0.1.2/supervised_learning/regression/DecisionTreeRegressor.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.1/supervised_learning/regression/LinearRegression.py` & `cc-mini-scikit-learn-0.1.2/supervised_learning/regression/LinearRegression.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-0.1.1/utilities/data_manipulation.py` & `cc-mini-scikit-learn-0.1.2/utilities/data_manipulation.py`

 * *Files identical despite different names*

