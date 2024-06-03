# Comparing `tmp/cs_ob_mini_scikit_learn-0.1.6.tar.gz` & `tmp/cs_ob_mini_scikit_learn-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs_ob_mini_scikit_learn-0.1.6.tar", last modified: Mon Jun  3 01:27:08 2024, max compression
+gzip compressed data, was "cs_ob_mini_scikit_learn-0.1.7.tar", last modified: Mon Jun  3 01:28:25 2024, max compression
```

## Comparing `cs_ob_mini_scikit_learn-0.1.6.tar` & `cs_ob_mini_scikit_learn-0.1.7.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:27:08.621003 cs_ob_mini_scikit_learn-0.1.6/
--rw-r--r--   0 mac        (501) staff       (20)     2715 2024-06-03 01:27:08.620028 cs_ob_mini_scikit_learn-0.1.6/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     2346 2024-05-22 21:15:43.000000 cs_ob_mini_scikit_learn-0.1.6/README.md
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:27:08.521179 cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/
--rw-r--r--   0 mac        (501) staff       (20)     1488 2024-06-02 23:18:34.000000 cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)       40 2024-06-03 00:38:20.000000 cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/cctest.py
--rw-r--r--   0 mac        (501) staff       (20)      632 2024-05-22 22:23:16.000000 cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/clone.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:27:08.536816 cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/ensemble/
--rw-r--r--   0 mac        (501) staff       (20)     4283 2024-06-02 21:46:43.000000 cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/ensemble/AdaBoost.py
--rw-r--r--   0 mac        (501) staff       (20)     4689 2024-06-02 21:21:42.000000 cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/ensemble/GradientBoostingClassifier.py
--rw-r--r--   0 mac        (501) staff       (20)     3705 2024-06-02 21:22:38.000000 cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/ensemble/GradientBoostingRegressor.py
--rw-r--r--   0 mac        (501) staff       (20)     5053 2024-06-02 21:23:06.000000 cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/ensemble/RandomForestClassifier.py
--rw-r--r--   0 mac        (501) staff       (20)     4000 2024-06-02 21:24:02.000000 cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/ensemble/RandomForestRegressor.py
--rw-r--r--   0 mac        (501) staff       (20)     3094 2024-06-02 21:25:08.000000 cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/ensemble/VotingClassifier.py
--rw-r--r--   0 mac        (501) staff       (20)      245 2024-06-02 20:58:50.000000 cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/ensemble/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:27:08.556563 cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/metrics/
--rw-r--r--   0 mac        (501) staff       (20)      846 2024-06-02 20:32:40.000000 cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/metrics/Accuracy.py
--rw-r--r--   0 mac        (501) staff       (20)      657 2024-06-02 20:33:25.000000 cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/metrics/BaseMetric.py
--rw-r--r--   0 mac        (501) staff       (20)     1127 2024-06-02 20:34:14.000000 cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/metrics/ConfusionMatrix.py
--rw-r--r--   0 mac        (501) staff       (20)      937 2024-06-02 20:34:23.000000 cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/metrics/F1Score.py
--rw-r--r--   0 mac        (501) staff       (20)      742 2024-06-02 20:34:35.000000 cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/metrics/MeanAbsoluteError.py
--rw-r--r--   0 mac        (501) staff       (20)      736 2024-06-02 20:35:27.000000 cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/metrics/MeanSquaredError.py
--rw-r--r--   0 mac        (501) staff       (20)      910 2024-06-02 20:35:39.000000 cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/metrics/Precision.py
--rw-r--r--   0 mac        (501) staff       (20)      901 2024-06-02 20:36:41.000000 cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/metrics/RSquared.py
--rw-r--r--   0 mac        (501) staff       (20)      888 2024-06-02 20:35:49.000000 cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/metrics/Recall.py
--rw-r--r--   0 mac        (501) staff       (20)      805 2024-06-02 20:35:58.000000 cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/metrics/RootMeanSquaredError.py
--rw-r--r--   0 mac        (501) staff       (20)      381 2024-06-02 18:18:52.000000 cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/metrics/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:27:08.563446 cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/model_selection/
--rw-r--r--   0 mac        (501) staff       (20)     4012 2024-06-02 21:49:06.000000 cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/model_selection/GridSearchCV.py
--rw-r--r--   0 mac        (501) staff       (20)     2154 2024-06-02 21:28:12.000000 cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/model_selection/KFold.py
--rw-r--r--   0 mac        (501) staff       (20)      967 2024-06-02 21:28:00.000000 cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/model_selection/ParameterGrid.py
--rw-r--r--   0 mac        (501) staff       (20)      151 2024-06-02 18:19:39.000000 cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/model_selection/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     3797 2024-06-02 21:51:24.000000 cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/model_selection/train_test_split.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:27:08.572376 cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/neural_networks/
--rw-r--r--   0 mac        (501) staff       (20)     3875 2024-06-02 21:28:42.000000 cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/neural_networks/MLP.py
--rw-r--r--   0 mac        (501) staff       (20)     7182 2024-06-02 21:29:49.000000 cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/neural_networks/MLPRegressor.py
--rw-r--r--   0 mac        (501) staff       (20)     3025 2024-06-02 21:30:03.000000 cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/neural_networks/Perceptron.py
--rw-r--r--   0 mac        (501) staff       (20)       60 2024-06-02 18:20:00.000000 cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/neural_networks/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:27:08.581893 cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/preprocessing/
--rw-r--r--   0 mac        (501) staff       (20)     2825 2024-06-02 21:31:50.000000 cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/preprocessing/LabelEncoder.py
--rw-r--r--   0 mac        (501) staff       (20)     2317 2024-06-02 21:32:10.000000 cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/preprocessing/MinMaxScaler.py
--rw-r--r--   0 mac        (501) staff       (20)     2468 2024-06-02 21:32:27.000000 cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/preprocessing/OneHotEncoder.py
--rw-r--r--   0 mac        (501) staff       (20)     3041 2024-06-02 21:34:15.000000 cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/preprocessing/SimpleImputer.py
--rw-r--r--   0 mac        (501) staff       (20)     2333 2024-06-02 21:34:44.000000 cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/preprocessing/StandardScaler.py
--rw-r--r--   0 mac        (501) staff       (20)      202 2024-06-02 18:20:46.000000 cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/preprocessing/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:27:08.589237 cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/supervised_learning/
--rw-r--r--   0 mac        (501) staff       (20)     1810 2024-06-02 20:56:39.000000 cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/supervised_learning/BaseEstimator.py
--rw-r--r--   0 mac        (501) staff       (20)       40 2024-06-02 18:23:05.000000 cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/supervised_learning/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:27:08.599238 cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/supervised_learning/classification/
--rw-r--r--   0 mac        (501) staff       (20)     6719 2024-06-02 21:17:12.000000 cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/supervised_learning/classification/DecisionTreeClassifier.py
--rw-r--r--   0 mac        (501) staff       (20)     3339 2024-06-02 21:16:04.000000 cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/supervised_learning/classification/KNNClassifier.py
--rw-r--r--   0 mac        (501) staff       (20)     5232 2024-06-02 21:14:23.000000 cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/supervised_learning/classification/LogisticRegression.py
--rw-r--r--   0 mac        (501) staff       (20)     2722 2024-06-02 21:54:57.000000 cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/supervised_learning/classification/NaiveBayes.py
--rw-r--r--   0 mac        (501) staff       (20)     2291 2024-06-02 21:04:16.000000 cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/supervised_learning/classification/SVM.py
--rw-r--r--   0 mac        (501) staff       (20)      206 2024-06-02 20:58:44.000000 cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/supervised_learning/classification/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:27:08.608542 cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/supervised_learning/regression/
--rw-r--r--   0 mac        (501) staff       (20)     5598 2024-06-02 21:13:44.000000 cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/supervised_learning/regression/DecisionTreeRegressor.py
--rw-r--r--   0 mac        (501) staff       (20)     2368 2024-06-02 21:05:04.000000 cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/supervised_learning/regression/LinearRegression.py
--rw-r--r--   0 mac        (501) staff       (20)      104 2024-06-02 20:58:18.000000 cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/supervised_learning/regression/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:27:08.613871 cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/utilities/
--rw-r--r--   0 mac        (501) staff       (20)       94 2024-06-02 18:29:01.000000 cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/utilities/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)      825 2024-06-02 18:28:48.000000 cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/utilities/data_manipulation.py
--rw-r--r--   0 mac        (501) staff       (20)      355 2024-06-02 18:26:21.000000 cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/utilities/file_handling.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:27:08.525783 cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)     2715 2024-06-03 01:27:08.000000 cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     3010 2024-06-03 01:27:08.000000 cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2024-06-03 01:27:08.000000 cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)       38 2024-06-03 01:27:08.000000 cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)       24 2024-06-03 01:27:08.000000 cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn.egg-info/top_level.txt
--rw-r--r--   0 mac        (501) staff       (20)       38 2024-06-03 01:27:08.621312 cs_ob_mini_scikit_learn-0.1.6/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)      625 2024-06-03 01:27:02.000000 cs_ob_mini_scikit_learn-0.1.6/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:28:25.138449 cs_ob_mini_scikit_learn-0.1.7/
+-rw-r--r--   0 mac        (501) staff       (20)     2715 2024-06-03 01:28:25.137146 cs_ob_mini_scikit_learn-0.1.7/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     2346 2024-05-22 21:15:43.000000 cs_ob_mini_scikit_learn-0.1.7/README.md
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:28:25.035590 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/
+-rw-r--r--   0 mac        (501) staff       (20)     1468 2024-06-03 01:28:03.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)       40 2024-06-03 00:38:20.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/cctest.py
+-rw-r--r--   0 mac        (501) staff       (20)      632 2024-05-22 22:23:16.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/clone.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:28:25.047015 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/ensemble/
+-rw-r--r--   0 mac        (501) staff       (20)     4283 2024-06-02 21:46:43.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/ensemble/AdaBoost.py
+-rw-r--r--   0 mac        (501) staff       (20)     4689 2024-06-02 21:21:42.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/ensemble/GradientBoostingClassifier.py
+-rw-r--r--   0 mac        (501) staff       (20)     3705 2024-06-02 21:22:38.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/ensemble/GradientBoostingRegressor.py
+-rw-r--r--   0 mac        (501) staff       (20)     5053 2024-06-02 21:23:06.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/ensemble/RandomForestClassifier.py
+-rw-r--r--   0 mac        (501) staff       (20)     4000 2024-06-02 21:24:02.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/ensemble/RandomForestRegressor.py
+-rw-r--r--   0 mac        (501) staff       (20)     3094 2024-06-02 21:25:08.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/ensemble/VotingClassifier.py
+-rw-r--r--   0 mac        (501) staff       (20)      194 2024-06-03 01:28:11.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/ensemble/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:28:25.065850 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/metrics/
+-rw-r--r--   0 mac        (501) staff       (20)      846 2024-06-02 20:32:40.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/metrics/Accuracy.py
+-rw-r--r--   0 mac        (501) staff       (20)      657 2024-06-02 20:33:25.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/metrics/BaseMetric.py
+-rw-r--r--   0 mac        (501) staff       (20)     1127 2024-06-02 20:34:14.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/metrics/ConfusionMatrix.py
+-rw-r--r--   0 mac        (501) staff       (20)      937 2024-06-02 20:34:23.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/metrics/F1Score.py
+-rw-r--r--   0 mac        (501) staff       (20)      742 2024-06-02 20:34:35.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/metrics/MeanAbsoluteError.py
+-rw-r--r--   0 mac        (501) staff       (20)      736 2024-06-02 20:35:27.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/metrics/MeanSquaredError.py
+-rw-r--r--   0 mac        (501) staff       (20)      910 2024-06-02 20:35:39.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/metrics/Precision.py
+-rw-r--r--   0 mac        (501) staff       (20)      901 2024-06-02 20:36:41.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/metrics/RSquared.py
+-rw-r--r--   0 mac        (501) staff       (20)      888 2024-06-02 20:35:49.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/metrics/Recall.py
+-rw-r--r--   0 mac        (501) staff       (20)      805 2024-06-02 20:35:58.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/metrics/RootMeanSquaredError.py
+-rw-r--r--   0 mac        (501) staff       (20)      381 2024-06-02 18:18:52.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/metrics/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:28:25.072830 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/model_selection/
+-rw-r--r--   0 mac        (501) staff       (20)     4012 2024-06-02 21:49:06.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/model_selection/GridSearchCV.py
+-rw-r--r--   0 mac        (501) staff       (20)     2154 2024-06-02 21:28:12.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/model_selection/KFold.py
+-rw-r--r--   0 mac        (501) staff       (20)      967 2024-06-02 21:28:00.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/model_selection/ParameterGrid.py
+-rw-r--r--   0 mac        (501) staff       (20)      151 2024-06-02 18:19:39.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/model_selection/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     3797 2024-06-02 21:51:24.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/model_selection/train_test_split.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:28:25.077617 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/neural_networks/
+-rw-r--r--   0 mac        (501) staff       (20)     3875 2024-06-02 21:28:42.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/neural_networks/MLP.py
+-rw-r--r--   0 mac        (501) staff       (20)     7182 2024-06-02 21:29:49.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/neural_networks/MLPRegressor.py
+-rw-r--r--   0 mac        (501) staff       (20)     3025 2024-06-02 21:30:03.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/neural_networks/Perceptron.py
+-rw-r--r--   0 mac        (501) staff       (20)       60 2024-06-02 18:20:00.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/neural_networks/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:28:25.105035 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/preprocessing/
+-rw-r--r--   0 mac        (501) staff       (20)     2825 2024-06-02 21:31:50.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/preprocessing/LabelEncoder.py
+-rw-r--r--   0 mac        (501) staff       (20)     2317 2024-06-02 21:32:10.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/preprocessing/MinMaxScaler.py
+-rw-r--r--   0 mac        (501) staff       (20)     2468 2024-06-02 21:32:27.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/preprocessing/OneHotEncoder.py
+-rw-r--r--   0 mac        (501) staff       (20)     3041 2024-06-02 21:34:15.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/preprocessing/SimpleImputer.py
+-rw-r--r--   0 mac        (501) staff       (20)     2333 2024-06-02 21:34:44.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/preprocessing/StandardScaler.py
+-rw-r--r--   0 mac        (501) staff       (20)      202 2024-06-02 18:20:46.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/preprocessing/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:28:25.107666 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/supervised_learning/
+-rw-r--r--   0 mac        (501) staff       (20)     1810 2024-06-02 20:56:39.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/supervised_learning/BaseEstimator.py
+-rw-r--r--   0 mac        (501) staff       (20)       40 2024-06-02 18:23:05.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/supervised_learning/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:28:25.122314 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/supervised_learning/classification/
+-rw-r--r--   0 mac        (501) staff       (20)     6719 2024-06-02 21:17:12.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/supervised_learning/classification/DecisionTreeClassifier.py
+-rw-r--r--   0 mac        (501) staff       (20)     3339 2024-06-02 21:16:04.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/supervised_learning/classification/KNNClassifier.py
+-rw-r--r--   0 mac        (501) staff       (20)     5232 2024-06-02 21:14:23.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/supervised_learning/classification/LogisticRegression.py
+-rw-r--r--   0 mac        (501) staff       (20)     2722 2024-06-02 21:54:57.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/supervised_learning/classification/NaiveBayes.py
+-rw-r--r--   0 mac        (501) staff       (20)     2291 2024-06-02 21:04:16.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/supervised_learning/classification/SVM.py
+-rw-r--r--   0 mac        (501) staff       (20)      206 2024-06-02 20:58:44.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/supervised_learning/classification/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:28:25.126306 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/supervised_learning/regression/
+-rw-r--r--   0 mac        (501) staff       (20)     5598 2024-06-02 21:13:44.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/supervised_learning/regression/DecisionTreeRegressor.py
+-rw-r--r--   0 mac        (501) staff       (20)     2368 2024-06-02 21:05:04.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/supervised_learning/regression/LinearRegression.py
+-rw-r--r--   0 mac        (501) staff       (20)      104 2024-06-02 20:58:18.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/supervised_learning/regression/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:28:25.136014 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/utilities/
+-rw-r--r--   0 mac        (501) staff       (20)       94 2024-06-02 18:29:01.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/utilities/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)      825 2024-06-02 18:28:48.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/utilities/data_manipulation.py
+-rw-r--r--   0 mac        (501) staff       (20)      355 2024-06-02 18:26:21.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/utilities/file_handling.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:28:25.038760 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)     2715 2024-06-03 01:28:24.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     3010 2024-06-03 01:28:24.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2024-06-03 01:28:24.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)       38 2024-06-03 01:28:24.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)       24 2024-06-03 01:28:24.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn.egg-info/top_level.txt
+-rw-r--r--   0 mac        (501) staff       (20)       38 2024-06-03 01:28:25.138723 cs_ob_mini_scikit_learn-0.1.7/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)      625 2024-06-03 01:28:17.000000 cs_ob_mini_scikit_learn-0.1.7/setup.py
```

### Comparing `cs_ob_mini_scikit_learn-0.1.6/PKG-INFO` & `cs_ob_mini_scikit_learn-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs_ob_mini_scikit_learn
-Version: 0.1.6
+Version: 0.1.7
 Summary: A minimal implementation of scikit-learn like functionalities
 Home-page: https://github.com/Basma-Arnaoui/Mini-Scikit-Learn/tree/main
 Author: basma-arnaoui
 Author-email: basma.arnaoui@um6p.ma
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `cs_ob_mini_scikit_learn-0.1.6/README.md` & `cs_ob_mini_scikit_learn-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/__init__.py` & `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # mini-scikit-learn/__init__.py
 
 
 # Exposing high-level interfaces
-from .ensemble import AdaBoost, GradientBoostingClassifier, GradientBoostingRegressor, StackingClassifier, VotingClassifier
+from .ensemble import AdaBoost, GradientBoostingClassifier, GradientBoostingRegressor, VotingClassifier
 from .metrics import Accuracy, Precision, Recall, F1Score, MeanAbsoluteError, MeanSquaredError, RootMeanSquaredError, RSquared, BaseMetric, ConfusionMatrix
 from .model_selection import GridSearchCV, KFold, ParameterGrid, train_test_split
 from .neural_networks import MLP, MLPRegressor, Perceptron
 from .preprocessing import LabelEncoder, MinMaxScaler, OneHotEncoder, SimpleImputer, StandardScaler
 from .supervised_learning.classification import DecisionTreeClassifier, KNNClassifier, LogisticRegression, NaiveBayes, SVM
 from .supervised_learning.regression import DecisionTreeRegressor, LinearRegression
```

### Comparing `cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/clone.py` & `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/clone.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/ensemble/AdaBoost.py` & `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/ensemble/AdaBoost.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/ensemble/GradientBoostingClassifier.py` & `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/ensemble/GradientBoostingClassifier.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/ensemble/GradientBoostingRegressor.py` & `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/ensemble/GradientBoostingRegressor.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/ensemble/RandomForestClassifier.py` & `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/ensemble/RandomForestClassifier.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/ensemble/RandomForestRegressor.py` & `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/ensemble/RandomForestRegressor.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/ensemble/VotingClassifier.py` & `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/ensemble/VotingClassifier.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/metrics/Accuracy.py` & `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/metrics/Accuracy.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/metrics/BaseMetric.py` & `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/metrics/BaseMetric.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/metrics/ConfusionMatrix.py` & `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/metrics/ConfusionMatrix.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/metrics/F1Score.py` & `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/metrics/F1Score.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/metrics/MeanAbsoluteError.py` & `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/metrics/MeanAbsoluteError.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/metrics/MeanSquaredError.py` & `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/metrics/MeanSquaredError.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/metrics/Precision.py` & `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/metrics/Precision.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/metrics/RSquared.py` & `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/metrics/RSquared.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/metrics/Recall.py` & `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/metrics/Recall.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/metrics/RootMeanSquaredError.py` & `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/metrics/RootMeanSquaredError.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/model_selection/GridSearchCV.py` & `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/model_selection/GridSearchCV.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/model_selection/KFold.py` & `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/model_selection/KFold.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/model_selection/ParameterGrid.py` & `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/model_selection/ParameterGrid.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/model_selection/train_test_split.py` & `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/model_selection/train_test_split.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/neural_networks/MLP.py` & `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/neural_networks/MLP.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/neural_networks/MLPRegressor.py` & `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/neural_networks/MLPRegressor.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/neural_networks/Perceptron.py` & `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/neural_networks/Perceptron.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/preprocessing/LabelEncoder.py` & `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/preprocessing/LabelEncoder.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/preprocessing/MinMaxScaler.py` & `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/preprocessing/MinMaxScaler.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/preprocessing/OneHotEncoder.py` & `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/preprocessing/OneHotEncoder.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/preprocessing/SimpleImputer.py` & `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/preprocessing/SimpleImputer.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/preprocessing/StandardScaler.py` & `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/preprocessing/StandardScaler.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/supervised_learning/BaseEstimator.py` & `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/supervised_learning/BaseEstimator.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/supervised_learning/classification/DecisionTreeClassifier.py` & `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/supervised_learning/classification/DecisionTreeClassifier.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/supervised_learning/classification/KNNClassifier.py` & `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/supervised_learning/classification/KNNClassifier.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/supervised_learning/classification/LogisticRegression.py` & `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/supervised_learning/classification/LogisticRegression.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/supervised_learning/classification/NaiveBayes.py` & `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/supervised_learning/classification/NaiveBayes.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/supervised_learning/classification/SVM.py` & `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/supervised_learning/classification/SVM.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/supervised_learning/regression/DecisionTreeRegressor.py` & `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/supervised_learning/regression/DecisionTreeRegressor.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/supervised_learning/regression/LinearRegression.py` & `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/supervised_learning/regression/LinearRegression.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn/utilities/data_manipulation.py` & `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/utilities/data_manipulation.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn.egg-info/PKG-INFO` & `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs-ob-mini-scikit-learn
-Version: 0.1.6
+Version: 0.1.7
 Summary: A minimal implementation of scikit-learn like functionalities
 Home-page: https://github.com/Basma-Arnaoui/Mini-Scikit-Learn/tree/main
 Author: basma-arnaoui
 Author-email: basma.arnaoui@um6p.ma
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `cs_ob_mini_scikit_learn-0.1.6/cs_ob_mini_scikit_learn.egg-info/SOURCES.txt` & `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.6/setup.py` & `cs_ob_mini_scikit_learn-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cs_ob_mini_scikit_learn',
-    version='0.1.6',
+    version='0.1.7',
     author='basma-arnaoui',
     author_email='basma.arnaoui@um6p.ma',
     packages=find_packages(),
     install_requires=[
         'numpy',
         'scipy',
         'scikit-learn',
```

