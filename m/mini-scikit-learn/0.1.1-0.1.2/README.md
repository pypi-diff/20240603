# Comparing `tmp/mini_scikit_learn-0.1.1.tar.gz` & `tmp/mini_scikit_learn-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mini_scikit_learn-0.1.1.tar", last modified: Sun Jun  2 20:22:51 2024, max compression
+gzip compressed data, was "mini_scikit_learn-0.1.2.tar", last modified: Sun Jun  2 22:04:31 2024, max compression
```

## Comparing `mini_scikit_learn-0.1.1.tar` & `mini_scikit_learn-0.1.2.tar`

### file list

```diff
@@ -1,59 +1,60 @@
-drwxrwxrwx   0        0        0        0 2024-06-02 20:22:51.318957 mini_scikit_learn-0.1.1/
--rw-rw-rw-   0        0        0     5396 2024-06-02 20:22:51.317955 mini_scikit_learn-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     4102 2024-06-02 20:15:08.000000 mini_scikit_learn-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-06-02 20:22:51.245818 mini_scikit_learn-0.1.1/mini_scikit_learn/
--rw-rw-rw-   0        0        0     2692 2024-05-22 21:00:24.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/AdaBoost.py
--rw-rw-rw-   0        0        0     8408 2024-06-01 13:34:18.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/DecisionTree.py
--rw-rw-rw-   0        0        0     1164 2024-05-01 19:19:40.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/Estimator.py
--rw-rw-rw-   0        0        0     2214 2024-06-02 19:51:34.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/KnnEstimator.py
--rw-rw-rw-   0        0        0    10969 2024-06-01 13:38:26.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/LinearModel.py
--rw-rw-rw-   0        0        0     2688 2024-05-14 23:36:33.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/LogisticRegression.py
--rw-rw-rw-   0        0        0     4585 2024-06-02 20:03:48.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/ModelEnsembler.py
--rw-rw-rw-   0        0        0     2616 2024-05-14 18:06:27.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/NBClassifier.py
--rw-rw-rw-   0        0        0     2291 2024-06-02 16:05:01.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/NN.py
--rw-rw-rw-   0        0        0     1452 2024-06-01 13:36:15.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/Predictor.py
--rw-rw-rw-   0        0        0     9746 2024-06-01 13:41:13.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/RandomForest.py
--rw-rw-rw-   0        0        0     1001 2024-05-22 18:57:48.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/SVM.py
--rw-rw-rw-   0        0        0      649 2024-06-02 19:45:21.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/__init__.py
--rw-rw-rw-   0        0        0      819 2024-05-01 21:00:46.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/main.py
-drwxrwxrwx   0        0        0        0 2024-06-02 20:22:51.283961 mini_scikit_learn-0.1.1/mini_scikit_learn/metrics/
--rw-rw-rw-   0        0        0      104 2024-06-02 13:28:04.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/metrics/__init__.py
--rw-rw-rw-   0        0        0     1511 2024-05-14 17:21:27.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/metrics/metric.py
-drwxrwxrwx   0        0        0        0 2024-06-02 20:22:51.292930 mini_scikit_learn-0.1.1/mini_scikit_learn/model_selection/
--rw-rw-rw-   0        0        0     2724 2024-06-02 18:52:51.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/model_selection/GridSearch.py
--rw-rw-rw-   0        0        0     3325 2024-06-02 19:17:55.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/model_selection/RandomSearch.py
--rw-rw-rw-   0        0        0       74 2024-06-02 18:58:49.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/model_selection/__init__.py
--rw-rw-rw-   0        0        0     1768 2024-05-08 19:11:07.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/test1.py
--rw-rw-rw-   0        0        0     1674 2024-06-02 16:42:36.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/test2.py
--rw-rw-rw-   0        0        0      771 2024-05-22 19:35:27.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/test_ada.py
--rw-rw-rw-   0        0        0      732 2024-05-22 18:05:25.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/test_cv.py
--rw-rw-rw-   0        0        0     2024 2024-05-22 18:24:36.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/test_dt.py
--rw-rw-rw-   0        0        0     1242 2024-05-14 16:27:56.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/test_dtr.py
--rw-rw-rw-   0        0        0     1804 2024-06-02 19:38:30.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/test_knn.py
--rw-rw-rw-   0        0        0     1197 2024-05-14 23:37:28.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/test_lg.py
--rw-rw-rw-   0        0        0     2249 2024-05-15 08:54:45.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/test_lgr.py
--rw-rw-rw-   0        0        0     3100 2024-05-05 19:11:00.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/test_nb.py
--rw-rw-rw-   0        0        0     4047 2024-05-07 15:17:35.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/test_nn.py
--rw-rw-rw-   0        0        0     1981 2024-05-07 15:29:08.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/test_nn2.py
--rw-rw-rw-   0        0        0     3939 2024-05-14 17:29:42.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/test_rf.py
--rw-rw-rw-   0        0        0     2046 2024-05-15 09:12:06.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/test_stacking.py
--rw-rw-rw-   0        0        0     2364 2024-05-15 09:18:44.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/test_voting.py
-drwxrwxrwx   0        0        0        0 2024-06-02 20:22:51.304025 mini_scikit_learn-0.1.1/mini_scikit_learn/transformers/
--rw-rw-rw-   0        0        0     2149 2024-06-02 13:09:30.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/transformers/Encoders.py
--rw-rw-rw-   0        0        0     1550 2024-06-01 13:45:18.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/transformers/Imputers.py
--rw-rw-rw-   0        0        0     1131 2024-06-02 16:44:55.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/transformers/Transfomer.py
--rw-rw-rw-   0        0        0      229 2024-06-02 17:33:02.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/transformers/__init__.py
--rw-rw-rw-   0        0        0      621 2024-05-14 08:53:30.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/transformers/encoderTest.py
-drwxrwxrwx   0        0        0        0 2024-06-02 20:22:51.311853 mini_scikit_learn-0.1.1/mini_scikit_learn/utils/
--rw-rw-rw-   0        0        0     5149 2024-05-08 08:28:46.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/utils/NeuralNetwork.py
--rw-rw-rw-   0        0        0       99 2024-06-02 18:55:11.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/utils/__init__.py
--rw-rw-rw-   0        0        0     1947 2024-06-02 13:52:22.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/utils/cross_validation.py
--rw-rw-rw-   0        0        0     3146 2024-06-02 14:04:24.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/utils/train_test_split.py
-drwxrwxrwx   0        0        0        0 2024-06-02 20:22:51.278887 mini_scikit_learn-0.1.1/mini_scikit_learn.egg-info/
--rw-rw-rw-   0        0        0     5396 2024-06-02 20:22:51.000000 mini_scikit_learn-0.1.1/mini_scikit_learn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1713 2024-06-02 20:22:51.000000 mini_scikit_learn-0.1.1/mini_scikit_learn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 20:22:51.000000 mini_scikit_learn-0.1.1/mini_scikit_learn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-06-02 20:22:51.000000 mini_scikit_learn-0.1.1/mini_scikit_learn.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-06-02 20:22:51.000000 mini_scikit_learn-0.1.1/mini_scikit_learn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-06-02 20:22:51.319956 mini_scikit_learn-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      873 2024-06-02 20:22:43.000000 mini_scikit_learn-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 22:04:31.706373 mini_scikit_learn-0.1.2/
+-rw-rw-rw-   0        0        0     6155 2024-06-02 22:04:31.706373 mini_scikit_learn-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4754 2024-06-02 22:00:40.000000 mini_scikit_learn-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-06-02 22:04:31.630182 mini_scikit_learn-0.1.2/mini_scikit_learn/
+-rw-rw-rw-   0        0        0     2692 2024-05-22 21:00:24.000000 mini_scikit_learn-0.1.2/mini_scikit_learn/AdaBoost.py
+-rw-rw-rw-   0        0        0     8408 2024-06-01 13:34:18.000000 mini_scikit_learn-0.1.2/mini_scikit_learn/DecisionTree.py
+-rw-rw-rw-   0        0        0     1164 2024-05-01 19:19:40.000000 mini_scikit_learn-0.1.2/mini_scikit_learn/Estimator.py
+-rw-rw-rw-   0        0        0     2214 2024-06-02 19:51:34.000000 mini_scikit_learn-0.1.2/mini_scikit_learn/KnnEstimator.py
+-rw-rw-rw-   0        0        0    10969 2024-06-01 13:38:26.000000 mini_scikit_learn-0.1.2/mini_scikit_learn/LinearModel.py
+-rw-rw-rw-   0        0        0     2688 2024-05-14 23:36:33.000000 mini_scikit_learn-0.1.2/mini_scikit_learn/LogisticRegression.py
+-rw-rw-rw-   0        0        0     5094 2024-06-02 22:02:02.000000 mini_scikit_learn-0.1.2/mini_scikit_learn/ModelEnsembler.py
+-rw-rw-rw-   0        0        0     2616 2024-05-14 18:06:27.000000 mini_scikit_learn-0.1.2/mini_scikit_learn/NBClassifier.py
+-rw-rw-rw-   0        0        0     2291 2024-06-02 16:05:01.000000 mini_scikit_learn-0.1.2/mini_scikit_learn/NN.py
+-rw-rw-rw-   0        0        0     1452 2024-06-01 13:36:15.000000 mini_scikit_learn-0.1.2/mini_scikit_learn/Predictor.py
+-rw-rw-rw-   0        0        0     9746 2024-06-01 13:41:13.000000 mini_scikit_learn-0.1.2/mini_scikit_learn/RandomForest.py
+-rw-rw-rw-   0        0        0     1076 2024-06-02 22:02:46.000000 mini_scikit_learn-0.1.2/mini_scikit_learn/SVM.py
+-rw-rw-rw-   0        0        0      649 2024-06-02 19:45:21.000000 mini_scikit_learn-0.1.2/mini_scikit_learn/__init__.py
+-rw-rw-rw-   0        0        0      819 2024-05-01 21:00:46.000000 mini_scikit_learn-0.1.2/mini_scikit_learn/main.py
+drwxrwxrwx   0        0        0        0 2024-06-02 22:04:31.672716 mini_scikit_learn-0.1.2/mini_scikit_learn/metrics/
+-rw-rw-rw-   0        0        0      201 2024-06-02 21:58:01.000000 mini_scikit_learn-0.1.2/mini_scikit_learn/metrics/__init__.py
+-rw-rw-rw-   0        0        0     1511 2024-05-14 17:21:27.000000 mini_scikit_learn-0.1.2/mini_scikit_learn/metrics/metric.py
+drwxrwxrwx   0        0        0        0 2024-06-02 22:04:31.677951 mini_scikit_learn-0.1.2/mini_scikit_learn/model_selection/
+-rw-rw-rw-   0        0        0     2724 2024-06-02 18:52:51.000000 mini_scikit_learn-0.1.2/mini_scikit_learn/model_selection/GridSearch.py
+-rw-rw-rw-   0        0        0     3325 2024-06-02 19:17:55.000000 mini_scikit_learn-0.1.2/mini_scikit_learn/model_selection/RandomSearch.py
+-rw-rw-rw-   0        0        0       74 2024-06-02 18:58:49.000000 mini_scikit_learn-0.1.2/mini_scikit_learn/model_selection/__init__.py
+-rw-rw-rw-   0        0        0     1768 2024-05-08 19:11:07.000000 mini_scikit_learn-0.1.2/mini_scikit_learn/test1.py
+-rw-rw-rw-   0        0        0     1674 2024-06-02 16:42:36.000000 mini_scikit_learn-0.1.2/mini_scikit_learn/test2.py
+-rw-rw-rw-   0        0        0      771 2024-05-22 19:35:27.000000 mini_scikit_learn-0.1.2/mini_scikit_learn/test_ada.py
+-rw-rw-rw-   0        0        0      732 2024-05-22 18:05:25.000000 mini_scikit_learn-0.1.2/mini_scikit_learn/test_cv.py
+-rw-rw-rw-   0        0        0     2024 2024-05-22 18:24:36.000000 mini_scikit_learn-0.1.2/mini_scikit_learn/test_dt.py
+-rw-rw-rw-   0        0        0     1242 2024-05-14 16:27:56.000000 mini_scikit_learn-0.1.2/mini_scikit_learn/test_dtr.py
+-rw-rw-rw-   0        0        0     1804 2024-06-02 19:38:30.000000 mini_scikit_learn-0.1.2/mini_scikit_learn/test_knn.py
+-rw-rw-rw-   0        0        0     1197 2024-05-14 23:37:28.000000 mini_scikit_learn-0.1.2/mini_scikit_learn/test_lg.py
+-rw-rw-rw-   0        0        0     2249 2024-05-15 08:54:45.000000 mini_scikit_learn-0.1.2/mini_scikit_learn/test_lgr.py
+-rw-rw-rw-   0        0        0     3100 2024-05-05 19:11:00.000000 mini_scikit_learn-0.1.2/mini_scikit_learn/test_nb.py
+-rw-rw-rw-   0        0        0     4047 2024-05-07 15:17:35.000000 mini_scikit_learn-0.1.2/mini_scikit_learn/test_nn.py
+-rw-rw-rw-   0        0        0     1981 2024-05-07 15:29:08.000000 mini_scikit_learn-0.1.2/mini_scikit_learn/test_nn2.py
+-rw-rw-rw-   0        0        0     3939 2024-05-14 17:29:42.000000 mini_scikit_learn-0.1.2/mini_scikit_learn/test_rf.py
+-rw-rw-rw-   0        0        0     2046 2024-05-15 09:12:06.000000 mini_scikit_learn-0.1.2/mini_scikit_learn/test_stacking.py
+-rw-rw-rw-   0        0        0     2364 2024-05-15 09:18:44.000000 mini_scikit_learn-0.1.2/mini_scikit_learn/test_voting.py
+drwxrwxrwx   0        0        0        0 2024-06-02 22:04:31.691421 mini_scikit_learn-0.1.2/mini_scikit_learn/transformers/
+-rw-rw-rw-   0        0        0     2149 2024-06-02 13:09:30.000000 mini_scikit_learn-0.1.2/mini_scikit_learn/transformers/Encoders.py
+-rw-rw-rw-   0        0        0     1550 2024-06-01 13:45:18.000000 mini_scikit_learn-0.1.2/mini_scikit_learn/transformers/Imputers.py
+-rw-rw-rw-   0        0        0     1131 2024-06-02 16:44:55.000000 mini_scikit_learn-0.1.2/mini_scikit_learn/transformers/Transfomer.py
+-rw-rw-rw-   0        0        0      229 2024-06-02 17:33:02.000000 mini_scikit_learn-0.1.2/mini_scikit_learn/transformers/__init__.py
+-rw-rw-rw-   0        0        0      621 2024-05-14 08:53:30.000000 mini_scikit_learn-0.1.2/mini_scikit_learn/transformers/encoderTest.py
+drwxrwxrwx   0        0        0        0 2024-06-02 22:04:31.705639 mini_scikit_learn-0.1.2/mini_scikit_learn/utils/
+-rw-rw-rw-   0        0        0     2670 2024-06-02 21:53:25.000000 mini_scikit_learn-0.1.2/mini_scikit_learn/utils/Kfolds.py
+-rw-rw-rw-   0        0        0     5149 2024-05-08 08:28:46.000000 mini_scikit_learn-0.1.2/mini_scikit_learn/utils/NeuralNetwork.py
+-rw-rw-rw-   0        0        0      126 2024-06-02 21:53:44.000000 mini_scikit_learn-0.1.2/mini_scikit_learn/utils/__init__.py
+-rw-rw-rw-   0        0        0     1947 2024-06-02 13:52:22.000000 mini_scikit_learn-0.1.2/mini_scikit_learn/utils/cross_validation.py
+-rw-rw-rw-   0        0        0     3146 2024-06-02 14:04:24.000000 mini_scikit_learn-0.1.2/mini_scikit_learn/utils/train_test_split.py
+drwxrwxrwx   0        0        0        0 2024-06-02 22:04:31.667413 mini_scikit_learn-0.1.2/mini_scikit_learn.egg-info/
+-rw-rw-rw-   0        0        0     6155 2024-06-02 22:04:31.000000 mini_scikit_learn-0.1.2/mini_scikit_learn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1747 2024-06-02 22:04:31.000000 mini_scikit_learn-0.1.2/mini_scikit_learn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 22:04:31.000000 mini_scikit_learn-0.1.2/mini_scikit_learn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-06-02 22:04:31.000000 mini_scikit_learn-0.1.2/mini_scikit_learn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-06-02 22:04:31.000000 mini_scikit_learn-0.1.2/mini_scikit_learn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-02 22:04:31.706373 mini_scikit_learn-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      787 2024-06-02 22:04:29.000000 mini_scikit_learn-0.1.2/setup.py
```

### Comparing `mini_scikit_learn-0.1.1/PKG-INFO` & `mini_scikit_learn-0.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,41 +1,49 @@
 Metadata-Version: 2.1
 Name: mini_scikit_learn
-Version: 0.1.1
+Version: 0.1.2
 Summary: A brief description of your package
-Home-page: UNKNOWN
+Home-page: https://github.com/YASSIRFRI/mini_scikit_learn.git
 Author: Yassir Fri
 Author-email: your.email@example.com
 License: UNKNOWN
 Description: # mini_scikit_learn
         
         **mini_scikit_learn** is a minimalistic clone of scikit-learn, designed to provide essential machine learning functionalities with minimal overhead. It only depends on numpy and offers a variety of basic and advanced models, utility functions, metrics, data transformers, and model selection tools. 
         
         ## Features
         
         ### Models
         - **Linear Models**: Implementations of linear regression, logistic regression, etc.
         - **Tree-Based Models**: Decision trees for classification and regression.
+        - **K-Nearest Neighbors**: KNN for classification and regression.
+        - **Random Forest**: Ensemble method for classification and regression.
+        - **SVM**: Support Vector Machines for classification and regression.(Under Testing)
         - **Naive Bayes**: Various naive Bayes classifiers.
-        - **Ensembling Techniques**: Advanced techniques such as voting, stacking, and boosting.
+        - **Neural Networks**: Basic feedforward and backpropagation neural networks, with customizable layers and activation functions.
+        - **Ensembling Techniques**: Advanced techniques such as voting, stacking, and boosting (AdaBoost, Gradient Boosting).
+        
         
         ### Utility Functions
         - **Cross Validation**: Functions for k-fold cross-validation, train-test splitting, etc.
         - **Train-Test Split**: Simple utility to split datasets into training and testing sets.
         - **K-Folds**: Functionality to split data into k folds for cross-validation.
         
         ### Metrics
         - **Accuracy**: Measure the accuracy of predictions.
+        - **Precision**: Calculate the precision for classification models.
+        - **Recall**: Compute the recall for classification models.
         - **F1 Score**: Calculate the F1 score for classification models.
         - **Mean Squared Error (MSE)**: Compute the mean squared error for regression models.
+        - **Mean Absolute Error (MAE)**: Compute the mean absolute error for regression models.
         - **Log Loss**: Calculate the logistic loss for classification models.
         
         ### Data Transformers
         - **Encoders**: Various encoding techniques for categorical data.
-        - **Imputers**: Different strategies for handling missing values.
+        - **Imputers**: Different strategies for handling missing values, SimpleImputer, IterativeImputer, KNNImputer.
         - **Scalers**: MinMaxScaler and StandardScaler for feature scaling.
         
         ### Model Selection
         - **Grid Search**: Exhaustive search over specified parameter values for an estimator.
         - **Random Search**: Random search over specified parameter values for an estimator.
         
         ## System Architecture
```

### Comparing `mini_scikit_learn-0.1.1/mini_scikit_learn/AdaBoost.py` & `mini_scikit_learn-0.1.2/mini_scikit_learn/AdaBoost.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.1/mini_scikit_learn/DecisionTree.py` & `mini_scikit_learn-0.1.2/mini_scikit_learn/DecisionTree.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.1/mini_scikit_learn/Estimator.py` & `mini_scikit_learn-0.1.2/mini_scikit_learn/Estimator.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.1/mini_scikit_learn/KnnEstimator.py` & `mini_scikit_learn-0.1.2/mini_scikit_learn/KnnEstimator.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.1/mini_scikit_learn/LinearModel.py` & `mini_scikit_learn-0.1.2/mini_scikit_learn/LinearModel.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.1/mini_scikit_learn/LogisticRegression.py` & `mini_scikit_learn-0.1.2/mini_scikit_learn/LogisticRegression.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.1/mini_scikit_learn/ModelEnsembler.py` & `mini_scikit_learn-0.1.2/mini_scikit_learn/ModelEnsembler.py`

 * *Files 12% similar despite different names*

```diff
@@ -103,26 +103,44 @@
         """
         self.base_models = base_models
         self.meta_model = meta_model
         self.is_fitted = False
         super().__init__(self)
 
     def fit(self, X, y, n_iterations=1000):
+        """
+        
+        This method is used to train the model on the training data.
+        Parameters:
+        X (numpy.ndarray): The training data.
+        y (numpy.ndarray): The target values.
+        Returns:
+        self: The trained model.
+        
+        """
         for model in self.base_models:
             model.fit(X, y)
             print("Accuracy of Model: ",base_models.index(model))
             print(model.score(X, y))
         X_meta = np.array([model.predict(X) for model in self.base_models]).T
         self.meta_model.fit(X_meta, y)
         print("Meta model score")
         print(self.meta_model.score(X_meta, y))
         self.is_fitted = True
         return self
 
     def predict(self, X):
+        """
+        This method is used to make predictions on the test data.
+        Parameters:
+        X (numpy.ndarray): The test data.
+        Returns:
+        numpy.ndarray: The predictions.
+        
+        """
         if not self.is_fitted:
             raise ValueError("The model has not been fitted yet.")
         X_meta = np.array([model.predict(X) for model in self.base_models]).T
         answer=self.meta_model.predict(X_meta)
         return answer
 
     def score(self, X, y):
```

### Comparing `mini_scikit_learn-0.1.1/mini_scikit_learn/NBClassifier.py` & `mini_scikit_learn-0.1.2/mini_scikit_learn/NBClassifier.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.1/mini_scikit_learn/NN.py` & `mini_scikit_learn-0.1.2/mini_scikit_learn/NN.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.1/mini_scikit_learn/Predictor.py` & `mini_scikit_learn-0.1.2/mini_scikit_learn/Predictor.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.1/mini_scikit_learn/RandomForest.py` & `mini_scikit_learn-0.1.2/mini_scikit_learn/RandomForest.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.1/mini_scikit_learn/SVM.py` & `mini_scikit_learn-0.1.2/mini_scikit_learn/SVM.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 import numpy as np 
 
 class SupportVectorMachine:
+    """
+    Implementation of the Support Vector Machine.
+    
+    """
 
     def __init__(self, learning_rate=0.001, lambda_param=0.01, n_iters=1000):
         self.lr = learning_rate
         self.lambda_param = lambda_param
         self.n_iters = n_iters
         self.w = None
         self.b = None
```

### Comparing `mini_scikit_learn-0.1.1/mini_scikit_learn/__init__.py` & `mini_scikit_learn-0.1.2/mini_scikit_learn/__init__.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.1/mini_scikit_learn/main.py` & `mini_scikit_learn-0.1.2/mini_scikit_learn/main.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.1/mini_scikit_learn/metrics/metric.py` & `mini_scikit_learn-0.1.2/mini_scikit_learn/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.1/mini_scikit_learn/model_selection/GridSearch.py` & `mini_scikit_learn-0.1.2/mini_scikit_learn/model_selection/GridSearch.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.1/mini_scikit_learn/model_selection/RandomSearch.py` & `mini_scikit_learn-0.1.2/mini_scikit_learn/model_selection/RandomSearch.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.1/mini_scikit_learn/test1.py` & `mini_scikit_learn-0.1.2/mini_scikit_learn/test1.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.1/mini_scikit_learn/test2.py` & `mini_scikit_learn-0.1.2/mini_scikit_learn/test2.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.1/mini_scikit_learn/test_ada.py` & `mini_scikit_learn-0.1.2/mini_scikit_learn/test_ada.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.1/mini_scikit_learn/test_cv.py` & `mini_scikit_learn-0.1.2/mini_scikit_learn/test_cv.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.1/mini_scikit_learn/test_dt.py` & `mini_scikit_learn-0.1.2/mini_scikit_learn/test_dt.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.1/mini_scikit_learn/test_dtr.py` & `mini_scikit_learn-0.1.2/mini_scikit_learn/test_dtr.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.1/mini_scikit_learn/test_knn.py` & `mini_scikit_learn-0.1.2/mini_scikit_learn/test_knn.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.1/mini_scikit_learn/test_lg.py` & `mini_scikit_learn-0.1.2/mini_scikit_learn/test_lg.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.1/mini_scikit_learn/test_lgr.py` & `mini_scikit_learn-0.1.2/mini_scikit_learn/test_lgr.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.1/mini_scikit_learn/test_nb.py` & `mini_scikit_learn-0.1.2/mini_scikit_learn/test_nb.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.1/mini_scikit_learn/test_nn.py` & `mini_scikit_learn-0.1.2/mini_scikit_learn/test_nn.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.1/mini_scikit_learn/test_nn2.py` & `mini_scikit_learn-0.1.2/mini_scikit_learn/test_nn2.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.1/mini_scikit_learn/test_rf.py` & `mini_scikit_learn-0.1.2/mini_scikit_learn/test_rf.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.1/mini_scikit_learn/test_stacking.py` & `mini_scikit_learn-0.1.2/mini_scikit_learn/test_stacking.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.1/mini_scikit_learn/test_voting.py` & `mini_scikit_learn-0.1.2/mini_scikit_learn/test_voting.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.1/mini_scikit_learn/transformers/Encoders.py` & `mini_scikit_learn-0.1.2/mini_scikit_learn/transformers/Encoders.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.1/mini_scikit_learn/transformers/Imputers.py` & `mini_scikit_learn-0.1.2/mini_scikit_learn/transformers/Imputers.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.1/mini_scikit_learn/transformers/Transfomer.py` & `mini_scikit_learn-0.1.2/mini_scikit_learn/transformers/Transfomer.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.1/mini_scikit_learn/transformers/encoderTest.py` & `mini_scikit_learn-0.1.2/mini_scikit_learn/transformers/encoderTest.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.1/mini_scikit_learn/utils/NeuralNetwork.py` & `mini_scikit_learn-0.1.2/mini_scikit_learn/utils/NeuralNetwork.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.1/mini_scikit_learn/utils/cross_validation.py` & `mini_scikit_learn-0.1.2/mini_scikit_learn/utils/cross_validation.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.1/mini_scikit_learn/utils/train_test_split.py` & `mini_scikit_learn-0.1.2/mini_scikit_learn/utils/train_test_split.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.1/mini_scikit_learn.egg-info/PKG-INFO` & `mini_scikit_learn-0.1.2/mini_scikit_learn.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,49 @@
 Metadata-Version: 2.1
 Name: mini-scikit-learn
-Version: 0.1.1
+Version: 0.1.2
 Summary: A brief description of your package
-Home-page: UNKNOWN
+Home-page: https://github.com/YASSIRFRI/mini_scikit_learn.git
 Author: Yassir Fri
 Author-email: your.email@example.com
 License: UNKNOWN
 Description: # mini_scikit_learn
         
         **mini_scikit_learn** is a minimalistic clone of scikit-learn, designed to provide essential machine learning functionalities with minimal overhead. It only depends on numpy and offers a variety of basic and advanced models, utility functions, metrics, data transformers, and model selection tools. 
         
         ## Features
         
         ### Models
         - **Linear Models**: Implementations of linear regression, logistic regression, etc.
         - **Tree-Based Models**: Decision trees for classification and regression.
+        - **K-Nearest Neighbors**: KNN for classification and regression.
+        - **Random Forest**: Ensemble method for classification and regression.
+        - **SVM**: Support Vector Machines for classification and regression.(Under Testing)
         - **Naive Bayes**: Various naive Bayes classifiers.
-        - **Ensembling Techniques**: Advanced techniques such as voting, stacking, and boosting.
+        - **Neural Networks**: Basic feedforward and backpropagation neural networks, with customizable layers and activation functions.
+        - **Ensembling Techniques**: Advanced techniques such as voting, stacking, and boosting (AdaBoost, Gradient Boosting).
+        
         
         ### Utility Functions
         - **Cross Validation**: Functions for k-fold cross-validation, train-test splitting, etc.
         - **Train-Test Split**: Simple utility to split datasets into training and testing sets.
         - **K-Folds**: Functionality to split data into k folds for cross-validation.
         
         ### Metrics
         - **Accuracy**: Measure the accuracy of predictions.
+        - **Precision**: Calculate the precision for classification models.
+        - **Recall**: Compute the recall for classification models.
         - **F1 Score**: Calculate the F1 score for classification models.
         - **Mean Squared Error (MSE)**: Compute the mean squared error for regression models.
+        - **Mean Absolute Error (MAE)**: Compute the mean absolute error for regression models.
         - **Log Loss**: Calculate the logistic loss for classification models.
         
         ### Data Transformers
         - **Encoders**: Various encoding techniques for categorical data.
-        - **Imputers**: Different strategies for handling missing values.
+        - **Imputers**: Different strategies for handling missing values, SimpleImputer, IterativeImputer, KNNImputer.
         - **Scalers**: MinMaxScaler and StandardScaler for feature scaling.
         
         ### Model Selection
         - **Grid Search**: Exhaustive search over specified parameter values for an estimator.
         - **Random Search**: Random search over specified parameter values for an estimator.
         
         ## System Architecture
```

### Comparing `mini_scikit_learn-0.1.1/mini_scikit_learn.egg-info/SOURCES.txt` & `mini_scikit_learn-0.1.2/mini_scikit_learn.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -40,11 +40,12 @@
 mini_scikit_learn/model_selection/RandomSearch.py
 mini_scikit_learn/model_selection/__init__.py
 mini_scikit_learn/transformers/Encoders.py
 mini_scikit_learn/transformers/Imputers.py
 mini_scikit_learn/transformers/Transfomer.py
 mini_scikit_learn/transformers/__init__.py
 mini_scikit_learn/transformers/encoderTest.py
+mini_scikit_learn/utils/Kfolds.py
 mini_scikit_learn/utils/NeuralNetwork.py
 mini_scikit_learn/utils/__init__.py
 mini_scikit_learn/utils/cross_validation.py
 mini_scikit_learn/utils/train_test_split.py
```

