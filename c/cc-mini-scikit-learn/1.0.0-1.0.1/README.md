# Comparing `tmp/cc-mini-scikit-learn-1.0.0.tar.gz` & `tmp/cc-mini-scikit-learn-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cc-mini-scikit-learn-1.0.0.tar", last modified: Mon Jun  3 03:19:38 2024, max compression
+gzip compressed data, was "cc-mini-scikit-learn-1.0.1.tar", last modified: Mon Jun  3 03:27:24 2024, max compression
```

## Comparing `cc-mini-scikit-learn-1.0.0.tar` & `cc-mini-scikit-learn-1.0.1.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 03:19:38.003897 cc-mini-scikit-learn-1.0.0/
--rw-r--r--   0 mac        (501) staff       (20)     2812 2024-06-03 03:19:38.003334 cc-mini-scikit-learn-1.0.0/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     2346 2024-06-03 01:54:09.000000 cc-mini-scikit-learn-1.0.0/README.md
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 03:19:37.671797 cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/
--rw-r--r--   0 mac        (501) staff       (20)        0 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)      632 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/clone.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 03:19:37.701949 cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/ensemble/
--rw-r--r--   0 mac        (501) staff       (20)     4327 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/ensemble/AdaBoost.py
--rw-r--r--   0 mac        (501) staff       (20)     4689 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/ensemble/GradientBoostingClassifier.py
--rw-r--r--   0 mac        (501) staff       (20)     3705 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/ensemble/GradientBoostingRegressor.py
--rw-r--r--   0 mac        (501) staff       (20)     5053 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/ensemble/RandomForestClassifier.py
--rw-r--r--   0 mac        (501) staff       (20)     4000 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/ensemble/RandomForestRegressor.py
--rw-r--r--   0 mac        (501) staff       (20)     3882 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/ensemble/StackingClassifier.py
--rw-r--r--   0 mac        (501) staff       (20)     3094 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/ensemble/VotingClassifier.py
--rw-r--r--   0 mac        (501) staff       (20)      245 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/ensemble/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 03:19:37.743609 cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/metrics/
--rw-r--r--   0 mac        (501) staff       (20)      846 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/metrics/Accuracy.py
--rw-r--r--   0 mac        (501) staff       (20)      657 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/metrics/BaseMetric.py
--rw-r--r--   0 mac        (501) staff       (20)     1127 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/metrics/ConfusionMatrix.py
--rw-r--r--   0 mac        (501) staff       (20)      937 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/metrics/F1Score.py
--rw-r--r--   0 mac        (501) staff       (20)      742 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/metrics/MeanAbsoluteError.py
--rw-r--r--   0 mac        (501) staff       (20)      736 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/metrics/MeanSquaredError.py
--rw-r--r--   0 mac        (501) staff       (20)      910 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/metrics/Precision.py
--rw-r--r--   0 mac        (501) staff       (20)      901 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/metrics/RSquared.py
--rw-r--r--   0 mac        (501) staff       (20)      888 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/metrics/Recall.py
--rw-r--r--   0 mac        (501) staff       (20)      805 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/metrics/RootMeanSquaredError.py
--rw-r--r--   0 mac        (501) staff       (20)      381 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/metrics/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 03:19:37.862664 cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/model_selection/
--rw-r--r--   0 mac        (501) staff       (20)     3981 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/model_selection/GridSearchCV.py
--rw-r--r--   0 mac        (501) staff       (20)     2154 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/model_selection/KFold.py
--rw-r--r--   0 mac        (501) staff       (20)      967 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/model_selection/ParameterGrid.py
--rw-r--r--   0 mac        (501) staff       (20)      151 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/model_selection/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     3726 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/model_selection/train_test_split.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 03:19:37.913451 cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/neural_networks/
--rw-r--r--   0 mac        (501) staff       (20)     3875 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/neural_networks/MLP.py
--rw-r--r--   0 mac        (501) staff       (20)     7182 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/neural_networks/MLPRegressor.py
--rw-r--r--   0 mac        (501) staff       (20)     3025 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/neural_networks/Perceptron.py
--rw-r--r--   0 mac        (501) staff       (20)       60 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/neural_networks/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 03:19:37.941872 cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/preprocessing/
--rw-r--r--   0 mac        (501) staff       (20)     2825 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/preprocessing/LabelEncoder.py
--rw-r--r--   0 mac        (501) staff       (20)     2317 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/preprocessing/MinMaxScaler.py
--rw-r--r--   0 mac        (501) staff       (20)     2468 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/preprocessing/OneHotEncoder.py
--rw-r--r--   0 mac        (501) staff       (20)     3041 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/preprocessing/SimpleImputer.py
--rw-r--r--   0 mac        (501) staff       (20)     2333 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/preprocessing/StandardScaler.py
--rw-r--r--   0 mac        (501) staff       (20)      202 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/preprocessing/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 03:19:37.957931 cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/supervised_learning/
--rw-r--r--   0 mac        (501) staff       (20)     1810 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/supervised_learning/BaseEstimator.py
--rw-r--r--   0 mac        (501) staff       (20)       40 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/supervised_learning/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 03:19:37.979543 cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/supervised_learning/classification/
--rw-r--r--   0 mac        (501) staff       (20)     6719 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/supervised_learning/classification/DecisionTreeClassifier.py
--rw-r--r--   0 mac        (501) staff       (20)     3339 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/supervised_learning/classification/KNNClassifier.py
--rw-r--r--   0 mac        (501) staff       (20)     5232 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/supervised_learning/classification/LogisticRegression.py
--rw-r--r--   0 mac        (501) staff       (20)     2690 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/supervised_learning/classification/NaiveBayes.py
--rw-r--r--   0 mac        (501) staff       (20)     2291 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/supervised_learning/classification/SVM.py
--rw-r--r--   0 mac        (501) staff       (20)      206 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/supervised_learning/classification/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 03:19:37.991600 cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/supervised_learning/regression/
--rw-r--r--   0 mac        (501) staff       (20)     5598 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/supervised_learning/regression/DecisionTreeRegressor.py
--rw-r--r--   0 mac        (501) staff       (20)     2368 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/supervised_learning/regression/LinearRegression.py
--rw-r--r--   0 mac        (501) staff       (20)      104 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/supervised_learning/regression/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 03:19:38.000379 cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/utilities/
--rw-r--r--   0 mac        (501) staff       (20)       94 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/utilities/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)      825 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/utilities/data_manipulation.py
--rw-r--r--   0 mac        (501) staff       (20)      355 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/utilities/file_handling.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 03:19:37.676729 cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)     2812 2024-06-03 03:19:37.000000 cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     2866 2024-06-03 03:19:37.000000 cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2024-06-03 03:19:37.000000 cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)       66 2024-06-03 03:19:37.000000 cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)       21 2024-06-03 03:19:37.000000 cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn.egg-info/top_level.txt
--rw-r--r--   0 mac        (501) staff       (20)       38 2024-06-03 03:19:38.004049 cc-mini-scikit-learn-1.0.0/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)      823 2024-06-03 03:19:33.000000 cc-mini-scikit-learn-1.0.0/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 03:27:24.075399 cc-mini-scikit-learn-1.0.1/
+-rw-r--r--   0 mac        (501) staff       (20)     4549 2024-06-03 03:27:24.074488 cc-mini-scikit-learn-1.0.1/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     4083 2024-06-03 03:24:30.000000 cc-mini-scikit-learn-1.0.1/README.md
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 03:27:23.826016 cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)      632 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/clone.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 03:27:23.844559 cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/ensemble/
+-rw-r--r--   0 mac        (501) staff       (20)     4327 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/ensemble/AdaBoost.py
+-rw-r--r--   0 mac        (501) staff       (20)     4689 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/ensemble/GradientBoostingClassifier.py
+-rw-r--r--   0 mac        (501) staff       (20)     3705 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/ensemble/GradientBoostingRegressor.py
+-rw-r--r--   0 mac        (501) staff       (20)     5053 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/ensemble/RandomForestClassifier.py
+-rw-r--r--   0 mac        (501) staff       (20)     4000 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/ensemble/RandomForestRegressor.py
+-rw-r--r--   0 mac        (501) staff       (20)     3882 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/ensemble/StackingClassifier.py
+-rw-r--r--   0 mac        (501) staff       (20)     3094 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/ensemble/VotingClassifier.py
+-rw-r--r--   0 mac        (501) staff       (20)      245 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/ensemble/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 03:27:23.870003 cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/metrics/
+-rw-r--r--   0 mac        (501) staff       (20)      846 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/metrics/Accuracy.py
+-rw-r--r--   0 mac        (501) staff       (20)      657 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/metrics/BaseMetric.py
+-rw-r--r--   0 mac        (501) staff       (20)     1127 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/metrics/ConfusionMatrix.py
+-rw-r--r--   0 mac        (501) staff       (20)      937 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/metrics/F1Score.py
+-rw-r--r--   0 mac        (501) staff       (20)      742 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/metrics/MeanAbsoluteError.py
+-rw-r--r--   0 mac        (501) staff       (20)      736 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/metrics/MeanSquaredError.py
+-rw-r--r--   0 mac        (501) staff       (20)      910 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/metrics/Precision.py
+-rw-r--r--   0 mac        (501) staff       (20)      901 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/metrics/RSquared.py
+-rw-r--r--   0 mac        (501) staff       (20)      888 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/metrics/Recall.py
+-rw-r--r--   0 mac        (501) staff       (20)      805 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/metrics/RootMeanSquaredError.py
+-rw-r--r--   0 mac        (501) staff       (20)      381 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/metrics/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 03:27:23.911606 cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/model_selection/
+-rw-r--r--   0 mac        (501) staff       (20)     3981 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/model_selection/GridSearchCV.py
+-rw-r--r--   0 mac        (501) staff       (20)     2154 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/model_selection/KFold.py
+-rw-r--r--   0 mac        (501) staff       (20)      967 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/model_selection/ParameterGrid.py
+-rw-r--r--   0 mac        (501) staff       (20)      151 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/model_selection/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     3726 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/model_selection/train_test_split.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 03:27:23.934341 cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/neural_networks/
+-rw-r--r--   0 mac        (501) staff       (20)     3875 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/neural_networks/MLP.py
+-rw-r--r--   0 mac        (501) staff       (20)     7182 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/neural_networks/MLPRegressor.py
+-rw-r--r--   0 mac        (501) staff       (20)     3025 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/neural_networks/Perceptron.py
+-rw-r--r--   0 mac        (501) staff       (20)       60 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/neural_networks/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 03:27:23.975219 cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/preprocessing/
+-rw-r--r--   0 mac        (501) staff       (20)     2825 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/preprocessing/LabelEncoder.py
+-rw-r--r--   0 mac        (501) staff       (20)     2317 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/preprocessing/MinMaxScaler.py
+-rw-r--r--   0 mac        (501) staff       (20)     2468 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/preprocessing/OneHotEncoder.py
+-rw-r--r--   0 mac        (501) staff       (20)     3041 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/preprocessing/SimpleImputer.py
+-rw-r--r--   0 mac        (501) staff       (20)     2333 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/preprocessing/StandardScaler.py
+-rw-r--r--   0 mac        (501) staff       (20)      202 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/preprocessing/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 03:27:23.980102 cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/supervised_learning/
+-rw-r--r--   0 mac        (501) staff       (20)     1810 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/supervised_learning/BaseEstimator.py
+-rw-r--r--   0 mac        (501) staff       (20)       40 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/supervised_learning/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 03:27:24.032144 cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/supervised_learning/classification/
+-rw-r--r--   0 mac        (501) staff       (20)     6719 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/supervised_learning/classification/DecisionTreeClassifier.py
+-rw-r--r--   0 mac        (501) staff       (20)     3339 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/supervised_learning/classification/KNNClassifier.py
+-rw-r--r--   0 mac        (501) staff       (20)     5232 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/supervised_learning/classification/LogisticRegression.py
+-rw-r--r--   0 mac        (501) staff       (20)     2690 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/supervised_learning/classification/NaiveBayes.py
+-rw-r--r--   0 mac        (501) staff       (20)     2291 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/supervised_learning/classification/SVM.py
+-rw-r--r--   0 mac        (501) staff       (20)      206 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/supervised_learning/classification/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 03:27:24.056970 cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/supervised_learning/regression/
+-rw-r--r--   0 mac        (501) staff       (20)     5598 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/supervised_learning/regression/DecisionTreeRegressor.py
+-rw-r--r--   0 mac        (501) staff       (20)     2368 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/supervised_learning/regression/LinearRegression.py
+-rw-r--r--   0 mac        (501) staff       (20)      104 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/supervised_learning/regression/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 03:27:24.070601 cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/utilities/
+-rw-r--r--   0 mac        (501) staff       (20)       94 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/utilities/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)      825 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/utilities/data_manipulation.py
+-rw-r--r--   0 mac        (501) staff       (20)      355 2024-06-03 01:54:10.000000 cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/utilities/file_handling.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-06-03 03:27:23.830302 cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)     4549 2024-06-03 03:27:23.000000 cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     2866 2024-06-03 03:27:23.000000 cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2024-06-03 03:27:23.000000 cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)       66 2024-06-03 03:27:23.000000 cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)       21 2024-06-03 03:27:23.000000 cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn.egg-info/top_level.txt
+-rw-r--r--   0 mac        (501) staff       (20)       38 2024-06-03 03:27:24.075660 cc-mini-scikit-learn-1.0.1/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)      823 2024-06-03 03:24:34.000000 cc-mini-scikit-learn-1.0.1/setup.py
```

### Comparing `cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/clone.py` & `cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/clone.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/ensemble/AdaBoost.py` & `cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/ensemble/AdaBoost.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/ensemble/GradientBoostingClassifier.py` & `cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/ensemble/GradientBoostingClassifier.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/ensemble/GradientBoostingRegressor.py` & `cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/ensemble/GradientBoostingRegressor.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/ensemble/RandomForestClassifier.py` & `cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/ensemble/RandomForestClassifier.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/ensemble/RandomForestRegressor.py` & `cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/ensemble/RandomForestRegressor.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/ensemble/StackingClassifier.py` & `cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/ensemble/StackingClassifier.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/ensemble/VotingClassifier.py` & `cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/ensemble/VotingClassifier.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/metrics/Accuracy.py` & `cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/metrics/Accuracy.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/metrics/BaseMetric.py` & `cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/metrics/BaseMetric.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/metrics/ConfusionMatrix.py` & `cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/metrics/ConfusionMatrix.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/metrics/F1Score.py` & `cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/metrics/F1Score.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/metrics/MeanAbsoluteError.py` & `cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/metrics/MeanAbsoluteError.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/metrics/MeanSquaredError.py` & `cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/metrics/MeanSquaredError.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/metrics/Precision.py` & `cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/metrics/Precision.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/metrics/RSquared.py` & `cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/metrics/RSquared.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/metrics/Recall.py` & `cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/metrics/Recall.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/metrics/RootMeanSquaredError.py` & `cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/metrics/RootMeanSquaredError.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/model_selection/GridSearchCV.py` & `cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/model_selection/GridSearchCV.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/model_selection/KFold.py` & `cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/model_selection/KFold.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/model_selection/ParameterGrid.py` & `cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/model_selection/ParameterGrid.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/model_selection/train_test_split.py` & `cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/model_selection/train_test_split.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/neural_networks/MLP.py` & `cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/neural_networks/MLP.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/neural_networks/MLPRegressor.py` & `cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/neural_networks/MLPRegressor.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/neural_networks/Perceptron.py` & `cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/neural_networks/Perceptron.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/preprocessing/LabelEncoder.py` & `cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/preprocessing/LabelEncoder.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/preprocessing/MinMaxScaler.py` & `cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/preprocessing/MinMaxScaler.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/preprocessing/OneHotEncoder.py` & `cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/preprocessing/OneHotEncoder.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/preprocessing/SimpleImputer.py` & `cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/preprocessing/SimpleImputer.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/preprocessing/StandardScaler.py` & `cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/preprocessing/StandardScaler.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/supervised_learning/BaseEstimator.py` & `cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/supervised_learning/BaseEstimator.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/supervised_learning/classification/DecisionTreeClassifier.py` & `cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/supervised_learning/classification/DecisionTreeClassifier.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/supervised_learning/classification/KNNClassifier.py` & `cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/supervised_learning/classification/KNNClassifier.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/supervised_learning/classification/LogisticRegression.py` & `cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/supervised_learning/classification/LogisticRegression.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/supervised_learning/classification/NaiveBayes.py` & `cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/supervised_learning/classification/NaiveBayes.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/supervised_learning/classification/SVM.py` & `cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/supervised_learning/classification/SVM.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/supervised_learning/regression/DecisionTreeRegressor.py` & `cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/supervised_learning/regression/DecisionTreeRegressor.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/supervised_learning/regression/LinearRegression.py` & `cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/supervised_learning/regression/LinearRegression.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn/utilities/data_manipulation.py` & `cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn/utilities/data_manipulation.py`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-1.0.0/cc_mini_scikit_learn.egg-info/SOURCES.txt` & `cc-mini-scikit-learn-1.0.1/cc_mini_scikit_learn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cc-mini-scikit-learn-1.0.0/setup.py` & `cc-mini-scikit-learn-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cc-mini-scikit-learn',
-    version='1.0.0',
+    version='1.0.1',
     author='basma-arnaoui',
     author_email='basma.arnaoui@um6p.ma',
     description='A mini implementation of Scikit-Learn with custom models and metrics',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
     classifiers=[
```

