# Comparing `tmp/cs_ob_mini_scikit_learn-0.1.7.tar.gz` & `tmp/cs_ob_mini_scikit_learn-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs_ob_mini_scikit_learn-0.1.7.tar", last modified: Mon Jun  3 01:28:25 2024, max compression
+gzip compressed data, was "cs_ob_mini_scikit_learn-0.1.8.tar", last modified: Mon Jun  3 01:31:44 2024, max compression
```

## Comparing `cs_ob_mini_scikit_learn-0.1.7.tar` & `cs_ob_mini_scikit_learn-0.1.8.tar`

### file list

```diff
@@ -1,71 +1,70 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:28:25.138449 cs_ob_mini_scikit_learn-0.1.7/
--rw-r--r--   0 mac        (501) staff       (20)     2715 2024-06-03 01:28:25.137146 cs_ob_mini_scikit_learn-0.1.7/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     2346 2024-05-22 21:15:43.000000 cs_ob_mini_scikit_learn-0.1.7/README.md
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:28:25.035590 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/
--rw-r--r--   0 mac        (501) staff       (20)     1468 2024-06-03 01:28:03.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)       40 2024-06-03 00:38:20.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/cctest.py
--rw-r--r--   0 mac        (501) staff       (20)      632 2024-05-22 22:23:16.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/clone.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:28:25.047015 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/ensemble/
--rw-r--r--   0 mac        (501) staff       (20)     4283 2024-06-02 21:46:43.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/ensemble/AdaBoost.py
--rw-r--r--   0 mac        (501) staff       (20)     4689 2024-06-02 21:21:42.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/ensemble/GradientBoostingClassifier.py
--rw-r--r--   0 mac        (501) staff       (20)     3705 2024-06-02 21:22:38.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/ensemble/GradientBoostingRegressor.py
--rw-r--r--   0 mac        (501) staff       (20)     5053 2024-06-02 21:23:06.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/ensemble/RandomForestClassifier.py
--rw-r--r--   0 mac        (501) staff       (20)     4000 2024-06-02 21:24:02.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/ensemble/RandomForestRegressor.py
--rw-r--r--   0 mac        (501) staff       (20)     3094 2024-06-02 21:25:08.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/ensemble/VotingClassifier.py
--rw-r--r--   0 mac        (501) staff       (20)      194 2024-06-03 01:28:11.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/ensemble/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:28:25.065850 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/metrics/
--rw-r--r--   0 mac        (501) staff       (20)      846 2024-06-02 20:32:40.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/metrics/Accuracy.py
--rw-r--r--   0 mac        (501) staff       (20)      657 2024-06-02 20:33:25.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/metrics/BaseMetric.py
--rw-r--r--   0 mac        (501) staff       (20)     1127 2024-06-02 20:34:14.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/metrics/ConfusionMatrix.py
--rw-r--r--   0 mac        (501) staff       (20)      937 2024-06-02 20:34:23.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/metrics/F1Score.py
--rw-r--r--   0 mac        (501) staff       (20)      742 2024-06-02 20:34:35.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/metrics/MeanAbsoluteError.py
--rw-r--r--   0 mac        (501) staff       (20)      736 2024-06-02 20:35:27.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/metrics/MeanSquaredError.py
--rw-r--r--   0 mac        (501) staff       (20)      910 2024-06-02 20:35:39.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/metrics/Precision.py
--rw-r--r--   0 mac        (501) staff       (20)      901 2024-06-02 20:36:41.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/metrics/RSquared.py
--rw-r--r--   0 mac        (501) staff       (20)      888 2024-06-02 20:35:49.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/metrics/Recall.py
--rw-r--r--   0 mac        (501) staff       (20)      805 2024-06-02 20:35:58.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/metrics/RootMeanSquaredError.py
--rw-r--r--   0 mac        (501) staff       (20)      381 2024-06-02 18:18:52.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/metrics/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:28:25.072830 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/model_selection/
--rw-r--r--   0 mac        (501) staff       (20)     4012 2024-06-02 21:49:06.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/model_selection/GridSearchCV.py
--rw-r--r--   0 mac        (501) staff       (20)     2154 2024-06-02 21:28:12.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/model_selection/KFold.py
--rw-r--r--   0 mac        (501) staff       (20)      967 2024-06-02 21:28:00.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/model_selection/ParameterGrid.py
--rw-r--r--   0 mac        (501) staff       (20)      151 2024-06-02 18:19:39.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/model_selection/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     3797 2024-06-02 21:51:24.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/model_selection/train_test_split.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:28:25.077617 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/neural_networks/
--rw-r--r--   0 mac        (501) staff       (20)     3875 2024-06-02 21:28:42.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/neural_networks/MLP.py
--rw-r--r--   0 mac        (501) staff       (20)     7182 2024-06-02 21:29:49.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/neural_networks/MLPRegressor.py
--rw-r--r--   0 mac        (501) staff       (20)     3025 2024-06-02 21:30:03.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/neural_networks/Perceptron.py
--rw-r--r--   0 mac        (501) staff       (20)       60 2024-06-02 18:20:00.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/neural_networks/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:28:25.105035 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/preprocessing/
--rw-r--r--   0 mac        (501) staff       (20)     2825 2024-06-02 21:31:50.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/preprocessing/LabelEncoder.py
--rw-r--r--   0 mac        (501) staff       (20)     2317 2024-06-02 21:32:10.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/preprocessing/MinMaxScaler.py
--rw-r--r--   0 mac        (501) staff       (20)     2468 2024-06-02 21:32:27.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/preprocessing/OneHotEncoder.py
--rw-r--r--   0 mac        (501) staff       (20)     3041 2024-06-02 21:34:15.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/preprocessing/SimpleImputer.py
--rw-r--r--   0 mac        (501) staff       (20)     2333 2024-06-02 21:34:44.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/preprocessing/StandardScaler.py
--rw-r--r--   0 mac        (501) staff       (20)      202 2024-06-02 18:20:46.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/preprocessing/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:28:25.107666 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/supervised_learning/
--rw-r--r--   0 mac        (501) staff       (20)     1810 2024-06-02 20:56:39.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/supervised_learning/BaseEstimator.py
--rw-r--r--   0 mac        (501) staff       (20)       40 2024-06-02 18:23:05.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/supervised_learning/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:28:25.122314 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/supervised_learning/classification/
--rw-r--r--   0 mac        (501) staff       (20)     6719 2024-06-02 21:17:12.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/supervised_learning/classification/DecisionTreeClassifier.py
--rw-r--r--   0 mac        (501) staff       (20)     3339 2024-06-02 21:16:04.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/supervised_learning/classification/KNNClassifier.py
--rw-r--r--   0 mac        (501) staff       (20)     5232 2024-06-02 21:14:23.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/supervised_learning/classification/LogisticRegression.py
--rw-r--r--   0 mac        (501) staff       (20)     2722 2024-06-02 21:54:57.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/supervised_learning/classification/NaiveBayes.py
--rw-r--r--   0 mac        (501) staff       (20)     2291 2024-06-02 21:04:16.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/supervised_learning/classification/SVM.py
--rw-r--r--   0 mac        (501) staff       (20)      206 2024-06-02 20:58:44.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/supervised_learning/classification/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:28:25.126306 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/supervised_learning/regression/
--rw-r--r--   0 mac        (501) staff       (20)     5598 2024-06-02 21:13:44.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/supervised_learning/regression/DecisionTreeRegressor.py
--rw-r--r--   0 mac        (501) staff       (20)     2368 2024-06-02 21:05:04.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/supervised_learning/regression/LinearRegression.py
--rw-r--r--   0 mac        (501) staff       (20)      104 2024-06-02 20:58:18.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/supervised_learning/regression/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:28:25.136014 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/utilities/
--rw-r--r--   0 mac        (501) staff       (20)       94 2024-06-02 18:29:01.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/utilities/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)      825 2024-06-02 18:28:48.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/utilities/data_manipulation.py
--rw-r--r--   0 mac        (501) staff       (20)      355 2024-06-02 18:26:21.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/utilities/file_handling.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:28:25.038760 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)     2715 2024-06-03 01:28:24.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     3010 2024-06-03 01:28:24.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2024-06-03 01:28:24.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)       38 2024-06-03 01:28:24.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)       24 2024-06-03 01:28:24.000000 cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn.egg-info/top_level.txt
--rw-r--r--   0 mac        (501) staff       (20)       38 2024-06-03 01:28:25.138723 cs_ob_mini_scikit_learn-0.1.7/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)      625 2024-06-03 01:28:17.000000 cs_ob_mini_scikit_learn-0.1.7/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:31:44.100054 cs_ob_mini_scikit_learn-0.1.8/
+-rw-r--r--   0 mac        (501) staff       (20)     2715 2024-06-03 01:31:44.088093 cs_ob_mini_scikit_learn-0.1.8/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     2346 2024-05-22 21:15:43.000000 cs_ob_mini_scikit_learn-0.1.8/README.md
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:31:43.981340 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/
+-rw-r--r--   0 mac        (501) staff       (20)     1450 2024-06-03 01:31:22.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)       40 2024-06-03 00:38:20.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/cctest.py
+-rw-r--r--   0 mac        (501) staff       (20)      632 2024-05-22 22:23:16.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/clone.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:31:43.998424 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/ensemble/
+-rw-r--r--   0 mac        (501) staff       (20)     4283 2024-06-02 21:46:43.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/ensemble/AdaBoost.py
+-rw-r--r--   0 mac        (501) staff       (20)     4689 2024-06-02 21:21:42.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/ensemble/GradientBoostingClassifier.py
+-rw-r--r--   0 mac        (501) staff       (20)     3705 2024-06-02 21:22:38.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/ensemble/GradientBoostingRegressor.py
+-rw-r--r--   0 mac        (501) staff       (20)     5053 2024-06-02 21:23:06.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/ensemble/RandomForestClassifier.py
+-rw-r--r--   0 mac        (501) staff       (20)     4000 2024-06-02 21:24:02.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/ensemble/RandomForestRegressor.py
+-rw-r--r--   0 mac        (501) staff       (20)      147 2024-06-03 01:31:28.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/ensemble/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:31:44.012598 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/metrics/
+-rw-r--r--   0 mac        (501) staff       (20)      846 2024-06-02 20:32:40.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/metrics/Accuracy.py
+-rw-r--r--   0 mac        (501) staff       (20)      657 2024-06-02 20:33:25.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/metrics/BaseMetric.py
+-rw-r--r--   0 mac        (501) staff       (20)     1127 2024-06-02 20:34:14.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/metrics/ConfusionMatrix.py
+-rw-r--r--   0 mac        (501) staff       (20)      937 2024-06-02 20:34:23.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/metrics/F1Score.py
+-rw-r--r--   0 mac        (501) staff       (20)      742 2024-06-02 20:34:35.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/metrics/MeanAbsoluteError.py
+-rw-r--r--   0 mac        (501) staff       (20)      736 2024-06-02 20:35:27.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/metrics/MeanSquaredError.py
+-rw-r--r--   0 mac        (501) staff       (20)      910 2024-06-02 20:35:39.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/metrics/Precision.py
+-rw-r--r--   0 mac        (501) staff       (20)      901 2024-06-02 20:36:41.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/metrics/RSquared.py
+-rw-r--r--   0 mac        (501) staff       (20)      888 2024-06-02 20:35:49.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/metrics/Recall.py
+-rw-r--r--   0 mac        (501) staff       (20)      805 2024-06-02 20:35:58.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/metrics/RootMeanSquaredError.py
+-rw-r--r--   0 mac        (501) staff       (20)      381 2024-06-02 18:18:52.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/metrics/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:31:44.016474 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/model_selection/
+-rw-r--r--   0 mac        (501) staff       (20)     4012 2024-06-02 21:49:06.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/model_selection/GridSearchCV.py
+-rw-r--r--   0 mac        (501) staff       (20)     2154 2024-06-02 21:28:12.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/model_selection/KFold.py
+-rw-r--r--   0 mac        (501) staff       (20)      967 2024-06-02 21:28:00.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/model_selection/ParameterGrid.py
+-rw-r--r--   0 mac        (501) staff       (20)      151 2024-06-02 18:19:39.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/model_selection/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     3797 2024-06-02 21:51:24.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/model_selection/train_test_split.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:31:44.021072 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/neural_networks/
+-rw-r--r--   0 mac        (501) staff       (20)     3875 2024-06-02 21:28:42.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/neural_networks/MLP.py
+-rw-r--r--   0 mac        (501) staff       (20)     7182 2024-06-02 21:29:49.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/neural_networks/MLPRegressor.py
+-rw-r--r--   0 mac        (501) staff       (20)     3025 2024-06-02 21:30:03.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/neural_networks/Perceptron.py
+-rw-r--r--   0 mac        (501) staff       (20)       60 2024-06-02 18:20:00.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/neural_networks/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:31:44.035900 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/preprocessing/
+-rw-r--r--   0 mac        (501) staff       (20)     2825 2024-06-02 21:31:50.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/preprocessing/LabelEncoder.py
+-rw-r--r--   0 mac        (501) staff       (20)     2317 2024-06-02 21:32:10.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/preprocessing/MinMaxScaler.py
+-rw-r--r--   0 mac        (501) staff       (20)     2468 2024-06-02 21:32:27.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/preprocessing/OneHotEncoder.py
+-rw-r--r--   0 mac        (501) staff       (20)     3041 2024-06-02 21:34:15.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/preprocessing/SimpleImputer.py
+-rw-r--r--   0 mac        (501) staff       (20)     2333 2024-06-02 21:34:44.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/preprocessing/StandardScaler.py
+-rw-r--r--   0 mac        (501) staff       (20)      202 2024-06-02 18:20:46.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/preprocessing/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:31:44.037583 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/supervised_learning/
+-rw-r--r--   0 mac        (501) staff       (20)     1810 2024-06-02 20:56:39.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/supervised_learning/BaseEstimator.py
+-rw-r--r--   0 mac        (501) staff       (20)       40 2024-06-02 18:23:05.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/supervised_learning/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:31:44.068617 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/supervised_learning/classification/
+-rw-r--r--   0 mac        (501) staff       (20)     6719 2024-06-02 21:17:12.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/supervised_learning/classification/DecisionTreeClassifier.py
+-rw-r--r--   0 mac        (501) staff       (20)     3339 2024-06-02 21:16:04.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/supervised_learning/classification/KNNClassifier.py
+-rw-r--r--   0 mac        (501) staff       (20)     5232 2024-06-02 21:14:23.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/supervised_learning/classification/LogisticRegression.py
+-rw-r--r--   0 mac        (501) staff       (20)     2722 2024-06-02 21:54:57.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/supervised_learning/classification/NaiveBayes.py
+-rw-r--r--   0 mac        (501) staff       (20)     2291 2024-06-02 21:04:16.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/supervised_learning/classification/SVM.py
+-rw-r--r--   0 mac        (501) staff       (20)      206 2024-06-02 20:58:44.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/supervised_learning/classification/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:31:44.082844 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/supervised_learning/regression/
+-rw-r--r--   0 mac        (501) staff       (20)     5598 2024-06-02 21:13:44.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/supervised_learning/regression/DecisionTreeRegressor.py
+-rw-r--r--   0 mac        (501) staff       (20)     2368 2024-06-02 21:05:04.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/supervised_learning/regression/LinearRegression.py
+-rw-r--r--   0 mac        (501) staff       (20)      104 2024-06-02 20:58:18.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/supervised_learning/regression/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:31:44.086867 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/utilities/
+-rw-r--r--   0 mac        (501) staff       (20)       94 2024-06-02 18:29:01.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/utilities/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)      825 2024-06-02 18:28:48.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/utilities/data_manipulation.py
+-rw-r--r--   0 mac        (501) staff       (20)      355 2024-06-02 18:26:21.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/utilities/file_handling.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 01:31:43.988092 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)     2715 2024-06-03 01:31:43.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     2957 2024-06-03 01:31:43.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2024-06-03 01:31:43.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)       38 2024-06-03 01:31:43.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)       24 2024-06-03 01:31:43.000000 cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn.egg-info/top_level.txt
+-rw-r--r--   0 mac        (501) staff       (20)       38 2024-06-03 01:31:44.101308 cs_ob_mini_scikit_learn-0.1.8/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)      625 2024-06-03 01:31:34.000000 cs_ob_mini_scikit_learn-0.1.8/setup.py
```

### Comparing `cs_ob_mini_scikit_learn-0.1.7/PKG-INFO` & `cs_ob_mini_scikit_learn-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs_ob_mini_scikit_learn
-Version: 0.1.7
+Version: 0.1.8
 Summary: A minimal implementation of scikit-learn like functionalities
 Home-page: https://github.com/Basma-Arnaoui/Mini-Scikit-Learn/tree/main
 Author: basma-arnaoui
 Author-email: basma.arnaoui@um6p.ma
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `cs_ob_mini_scikit_learn-0.1.7/README.md` & `cs_ob_mini_scikit_learn-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/__init__.py` & `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # mini-scikit-learn/__init__.py
 
 
 # Exposing high-level interfaces
-from .ensemble import AdaBoost, GradientBoostingClassifier, GradientBoostingRegressor, VotingClassifier
+from .ensemble import AdaBoost, GradientBoostingClassifier, GradientBoostingRegressor
 from .metrics import Accuracy, Precision, Recall, F1Score, MeanAbsoluteError, MeanSquaredError, RootMeanSquaredError, RSquared, BaseMetric, ConfusionMatrix
 from .model_selection import GridSearchCV, KFold, ParameterGrid, train_test_split
 from .neural_networks import MLP, MLPRegressor, Perceptron
 from .preprocessing import LabelEncoder, MinMaxScaler, OneHotEncoder, SimpleImputer, StandardScaler
 from .supervised_learning.classification import DecisionTreeClassifier, KNNClassifier, LogisticRegression, NaiveBayes, SVM
 from .supervised_learning.regression import DecisionTreeRegressor, LinearRegression
```

### Comparing `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/clone.py` & `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/clone.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/ensemble/AdaBoost.py` & `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/ensemble/AdaBoost.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/ensemble/GradientBoostingClassifier.py` & `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/ensemble/GradientBoostingClassifier.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/ensemble/GradientBoostingRegressor.py` & `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/ensemble/GradientBoostingRegressor.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/ensemble/RandomForestClassifier.py` & `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/ensemble/RandomForestClassifier.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/ensemble/RandomForestRegressor.py` & `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/ensemble/RandomForestRegressor.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/ensemble/VotingClassifier.py` & `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/neural_networks/Perceptron.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,93 +1,102 @@
 import numpy as np
-from sklearn.base import ClassifierMixin
-from supervised_learning.BaseEstimator import BaseEstimator
 
-class VotingClassifier(BaseEstimator, ClassifierMixin):
+class Perceptron:
     """
-    Voting Classifier implementation that allows for both hard and soft voting.
+    Perceptron classifier.
 
     Parameters
     ----------
-    estimators : list of (str, estimator) tuples
-        List of named base estimators. Each element of the list is a tuple containing
-        the name and the estimator instance.
+    learning_rate : float, default=0.01
+        Learning rate (between 0.0 and 1.0).
     
-    voting : {'hard', 'soft'}, default='hard'
-        If 'hard', uses predicted class labels for majority rule voting.
-        If 'soft', predicts the class label based on the argmax of the sums of the predicted probabilities.
-
-    Attributes
-    ----------
-    models_ : list
-        List of fitted base estimators.
+    n_iters : int, default=1000
+        The number of passes over the training dataset.
 
     Methods
     -------
     fit(X, y)
-        Fit the voting classifier to the training data.
+        Fit the Perceptron model to the training data.
     
     predict(X)
-        Predict classes for X.
+        Predict class labels for samples in X.
     """
 
-    def __init__(self, estimators, voting='hard'):
-        if not isinstance(estimators, list) or not estimators:
-            raise ValueError("estimators must be a non-empty list of (str, estimator) tuples.")
-        if voting not in ('hard', 'soft'):
-            raise ValueError("voting must be either 'hard' or 'soft'.")
+    def __init__(self, learning_rate=0.01, n_iters=1000):
+        if not isinstance(learning_rate, float) or learning_rate <= 0:
+            raise ValueError("learning_rate must be a positive float.")
+        if not isinstance(n_iters, int) or n_iters <= 0:
+            raise ValueError("n_iters must be a positive integer.")
+
+        self.learning_rate = learning_rate
+        self.n_iters = n_iters
+        self.activation_func = self._unit_step_func
+        self.weights = None
+        self.bias = None
 
-        self.estimators = estimators
-        self.voting = voting
-    
     def fit(self, X, y):
         """
-        Fit the voting classifier to the training data.
+        Fit the Perceptron model to the training data.
 
         Parameters
         ----------
         X : array-like of shape (n_samples, n_features)
             The training input samples.
         
         y : array-like of shape (n_samples,)
             The target values (class labels).
-
-        Returns
-        -------
-        self : object
-            Fitted estimator.
         """
         if not isinstance(X, np.ndarray) or not isinstance(y, np.ndarray):
             raise TypeError("X and y must be numpy arrays.")
         if X.shape[0] != y.shape[0]:
             raise ValueError("The number of samples in X and y must be equal.")
+        
+        n_samples, n_features = X.shape
+        self.weights = np.zeros(n_features)
+        self.bias = 0
+
+        y_ = np.array([1 if i > 0 else 0 for i in y])
+
+        for _ in range(self.n_iters):
+            for idx, x_i in enumerate(X):
+                linear_output = np.dot(x_i, self.weights) + self.bias
+                y_predicted = self.activation_func(linear_output)
+                update = self.learning_rate * (y_[idx] - y_predicted)
+                self.weights += update * x_i
+                self.bias += update
 
-        self.models_ = [clf.fit(X, y) for _, clf in self.estimators]
-        return self
-    
     def predict(self, X):
         """
-        Predict classes for X.
+        Predict class labels for samples in X.
 
         Parameters
         ----------
         X : array-like of shape (n_samples, n_features)
             The input samples.
 
         Returns
         -------
         y_pred : array-like of shape (n_samples,)
-            The predicted classes.
+            The predicted class labels.
         """
         if not isinstance(X, np.ndarray):
             raise TypeError("X must be a numpy array.")
-        if not self.models_:
-            raise RuntimeError("The model has not been fitted yet.")
+        
+        linear_output = np.dot(X, self.weights) + self.bias
+        y_predicted = self.activation_func(linear_output)
+        return y_predicted
 
-        if self.voting == 'hard':
-            predictions = np.asarray([clf.predict(X) for clf in self.models_]).T
-            maj_vote = np.apply_along_axis(lambda x: np.bincount(x).argmax(), axis=1, arr=predictions)
-            return maj_vote
-        else:
-            predictions = np.asarray([clf.predict_proba(X) for clf in self.models_])
-            avg_proba = np.average(predictions, axis=0)
-            return np.argmax(avg_proba, axis=1)
+    def _unit_step_func(self, x):
+        """
+        Unit step activation function.
+
+        Parameters
+        ----------
+        x : array-like
+            The input data.
+
+        Returns
+        -------
+        result : array-like
+            The output of the unit step function.
+        """
+        return np.where(x >= 0, 1, 0)
```

### Comparing `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/metrics/Accuracy.py` & `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/metrics/Accuracy.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/metrics/BaseMetric.py` & `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/metrics/BaseMetric.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/metrics/ConfusionMatrix.py` & `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/metrics/ConfusionMatrix.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/metrics/F1Score.py` & `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/metrics/F1Score.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/metrics/MeanAbsoluteError.py` & `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/metrics/MeanAbsoluteError.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/metrics/MeanSquaredError.py` & `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/metrics/MeanSquaredError.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/metrics/Precision.py` & `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/metrics/Precision.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/metrics/RSquared.py` & `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/metrics/RSquared.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/metrics/Recall.py` & `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/metrics/Recall.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/metrics/RootMeanSquaredError.py` & `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/metrics/RootMeanSquaredError.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/model_selection/GridSearchCV.py` & `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/model_selection/GridSearchCV.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/model_selection/KFold.py` & `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/model_selection/KFold.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/model_selection/ParameterGrid.py` & `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/model_selection/ParameterGrid.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/model_selection/train_test_split.py` & `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/model_selection/train_test_split.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/neural_networks/MLP.py` & `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/neural_networks/MLP.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/neural_networks/MLPRegressor.py` & `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/neural_networks/MLPRegressor.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/neural_networks/Perceptron.py` & `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/supervised_learning/classification/NaiveBayes.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,72 +1,54 @@
 import numpy as np
+from supervised_learning.BaseEstimator import BaseEstimator
 
-class Perceptron:
-    """
-    Perceptron classifier.
 
-    Parameters
-    ----------
-    learning_rate : float, default=0.01
-        Learning rate (between 0.0 and 1.0).
-    
-    n_iters : int, default=1000
-        The number of passes over the training dataset.
+class NaiveBayes(BaseEstimator):
+    """
+    Naive Bayes classifier.
 
     Methods
     -------
     fit(X, y)
-        Fit the Perceptron model to the training data.
+        Fit the Naive Bayes classifier to the training data.
     
     predict(X)
         Predict class labels for samples in X.
     """
 
-    def __init__(self, learning_rate=0.01, n_iters=1000):
-        if not isinstance(learning_rate, float) or learning_rate <= 0:
-            raise ValueError("learning_rate must be a positive float.")
-        if not isinstance(n_iters, int) or n_iters <= 0:
-            raise ValueError("n_iters must be a positive integer.")
-
-        self.learning_rate = learning_rate
-        self.n_iters = n_iters
-        self.activation_func = self._unit_step_func
-        self.weights = None
-        self.bias = None
-
     def fit(self, X, y):
         """
-        Fit the Perceptron model to the training data.
+        Fit the Naive Bayes classifier to the training data.
 
         Parameters
         ----------
         X : array-like of shape (n_samples, n_features)
             The training input samples.
         
         y : array-like of shape (n_samples,)
             The target values (class labels).
         """
         if not isinstance(X, np.ndarray) or not isinstance(y, np.ndarray):
             raise TypeError("X and y must be numpy arrays.")
         if X.shape[0] != y.shape[0]:
             raise ValueError("The number of samples in X and y must be equal.")
-        
-        n_samples, n_features = X.shape
-        self.weights = np.zeros(n_features)
-        self.bias = 0
 
-        y_ = np.array([1 if i > 0 else 0 for i in y])
+        n_samples, n_features = X.shape
+        self.classes_ = np.unique(y)
+        n_classes = len(self.classes_)
 
-        for _ in range(self.n_iters):
-            for idx, x_i in enumerate(X):
-                linear_output = np.dot(x_i, self.weights) + self.bias
-                y_predicted = self.activation_func(linear_output)
-                update = self.learning_rate * (y_[idx] - y_predicted)
-                self.weights += update * x_i
-                self.bias += update
+        self.mean_ = np.zeros((n_classes, n_features), dtype=np.float64)
+        self.var_ = np.zeros((n_classes, n_features), dtype=np.float64)
+        self.priors_ = np.zeros(n_classes, dtype=np.float64)
+
+        for idx, class_ in enumerate(self.classes_):
+            X_class = X[y == class_]
+            self.mean_[idx, :] = X_class.mean(axis=0)
+            self.var_[idx, :] = X_class.var(axis=0)
+            self.priors_[idx] = X_class.shape[0] / float(n_samples)
 
     def predict(self, X):
         """
         Predict class labels for samples in X.
 
         Parameters
         ----------
@@ -77,26 +59,26 @@
         -------
         y_pred : array-like of shape (n_samples,)
             The predicted class labels.
         """
         if not isinstance(X, np.ndarray):
             raise TypeError("X must be a numpy array.")
         
-        linear_output = np.dot(X, self.weights) + self.bias
-        y_predicted = self.activation_func(linear_output)
-        return y_predicted
+        return np.array([self._predict(x) for x in X])
 
-    def _unit_step_func(self, x):
-        """
-        Unit step activation function.
-
-        Parameters
-        ----------
-        x : array-like
-            The input data.
-
-        Returns
-        -------
-        result : array-like
-            The output of the unit step function.
-        """
-        return np.where(x >= 0, 1, 0)
+    def _predict(self, x):
+        posteriors = []
+        for idx, class_ in enumerate(self.classes_):
+            prior = np.log(self.priors_[idx])
+            posterior = np.sum(np.log(self._pdf(idx, x)))
+            posterior = prior + posterior
+            posteriors.append(posterior)
+        return self.classes_[np.argmax(posteriors)]
+
+    def _pdf(self, class_idx, x):
+        mean = self.mean_[class_idx]
+        var = self.var_[class_idx]
+        if np.any(var == 0):
+            raise RuntimeError("One or more features have zero variance.")
+        numerator = np.exp(-((x - mean) ** 2) / (2 * var))
+        denominator = np.sqrt(2 * np.pi * var)
+        return numerator / denominator
```

### Comparing `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/preprocessing/LabelEncoder.py` & `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/preprocessing/LabelEncoder.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/preprocessing/MinMaxScaler.py` & `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/preprocessing/MinMaxScaler.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/preprocessing/OneHotEncoder.py` & `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/preprocessing/OneHotEncoder.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/preprocessing/SimpleImputer.py` & `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/preprocessing/SimpleImputer.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/preprocessing/StandardScaler.py` & `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/preprocessing/StandardScaler.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/supervised_learning/BaseEstimator.py` & `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/supervised_learning/BaseEstimator.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/supervised_learning/classification/DecisionTreeClassifier.py` & `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/supervised_learning/classification/DecisionTreeClassifier.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/supervised_learning/classification/KNNClassifier.py` & `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/supervised_learning/classification/KNNClassifier.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/supervised_learning/classification/LogisticRegression.py` & `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/supervised_learning/classification/LogisticRegression.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/supervised_learning/classification/SVM.py` & `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/supervised_learning/classification/SVM.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/supervised_learning/regression/DecisionTreeRegressor.py` & `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/supervised_learning/regression/DecisionTreeRegressor.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/supervised_learning/regression/LinearRegression.py` & `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/supervised_learning/regression/LinearRegression.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn/utilities/data_manipulation.py` & `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn/utilities/data_manipulation.py`

 * *Files identical despite different names*

### Comparing `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn.egg-info/PKG-INFO` & `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs-ob-mini-scikit-learn
-Version: 0.1.7
+Version: 0.1.8
 Summary: A minimal implementation of scikit-learn like functionalities
 Home-page: https://github.com/Basma-Arnaoui/Mini-Scikit-Learn/tree/main
 Author: basma-arnaoui
 Author-email: basma.arnaoui@um6p.ma
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `cs_ob_mini_scikit_learn-0.1.7/cs_ob_mini_scikit_learn.egg-info/SOURCES.txt` & `cs_ob_mini_scikit_learn-0.1.8/cs_ob_mini_scikit_learn.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 cs_ob_mini_scikit_learn.egg-info/requires.txt
 cs_ob_mini_scikit_learn.egg-info/top_level.txt
 cs_ob_mini_scikit_learn/ensemble/AdaBoost.py
 cs_ob_mini_scikit_learn/ensemble/GradientBoostingClassifier.py
 cs_ob_mini_scikit_learn/ensemble/GradientBoostingRegressor.py
 cs_ob_mini_scikit_learn/ensemble/RandomForestClassifier.py
 cs_ob_mini_scikit_learn/ensemble/RandomForestRegressor.py
-cs_ob_mini_scikit_learn/ensemble/VotingClassifier.py
 cs_ob_mini_scikit_learn/ensemble/__init__.py
 cs_ob_mini_scikit_learn/metrics/Accuracy.py
 cs_ob_mini_scikit_learn/metrics/BaseMetric.py
 cs_ob_mini_scikit_learn/metrics/ConfusionMatrix.py
 cs_ob_mini_scikit_learn/metrics/F1Score.py
 cs_ob_mini_scikit_learn/metrics/MeanAbsoluteError.py
 cs_ob_mini_scikit_learn/metrics/MeanSquaredError.py
```

### Comparing `cs_ob_mini_scikit_learn-0.1.7/setup.py` & `cs_ob_mini_scikit_learn-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cs_ob_mini_scikit_learn',
-    version='0.1.7',
+    version='0.1.8',
     author='basma-arnaoui',
     author_email='basma.arnaoui@um6p.ma',
     packages=find_packages(),
     install_requires=[
         'numpy',
         'scipy',
         'scikit-learn',
```

