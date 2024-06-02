# Comparing `tmp/mini_scikit_learn-0.1.0.tar.gz` & `tmp/mini_scikit_learn-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mini_scikit_learn-0.1.0.tar", last modified: Sun Jun  2 16:46:58 2024, max compression
+gzip compressed data, was "mini_scikit_learn-0.1.1.tar", last modified: Sun Jun  2 20:22:51 2024, max compression
```

## Comparing `mini_scikit_learn-0.1.0.tar` & `mini_scikit_learn-0.1.1.tar`

### file list

```diff
@@ -1,56 +1,59 @@
-drwxrwxrwx   0        0        0        0 2024-06-02 16:46:58.518849 mini_scikit_learn-0.1.0/
--rw-rw-rw-   0        0        0      580 2024-06-02 16:46:58.516829 mini_scikit_learn-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      126 2024-05-22 23:31:29.000000 mini_scikit_learn-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-06-02 16:46:58.450122 mini_scikit_learn-0.1.0/mini_scikit_learn/
--rw-rw-rw-   0        0        0     2692 2024-05-22 21:00:24.000000 mini_scikit_learn-0.1.0/mini_scikit_learn/AdaBoost.py
--rw-rw-rw-   0        0        0     8408 2024-06-01 13:34:18.000000 mini_scikit_learn-0.1.0/mini_scikit_learn/DecisionTree.py
--rw-rw-rw-   0        0        0     1164 2024-05-01 19:19:40.000000 mini_scikit_learn-0.1.0/mini_scikit_learn/Estimator.py
--rw-rw-rw-   0        0        0     2214 2024-06-01 13:37:03.000000 mini_scikit_learn-0.1.0/mini_scikit_learn/KnnEstimator.py
--rw-rw-rw-   0        0        0    10969 2024-06-01 13:38:26.000000 mini_scikit_learn-0.1.0/mini_scikit_learn/LinearModel.py
--rw-rw-rw-   0        0        0     2688 2024-05-14 23:36:33.000000 mini_scikit_learn-0.1.0/mini_scikit_learn/LogisticRegression.py
--rw-rw-rw-   0        0        0     4676 2024-06-01 13:42:54.000000 mini_scikit_learn-0.1.0/mini_scikit_learn/ModelEnsembler.py
--rw-rw-rw-   0        0        0     2616 2024-05-14 18:06:27.000000 mini_scikit_learn-0.1.0/mini_scikit_learn/NBClassifier.py
--rw-rw-rw-   0        0        0     2291 2024-06-02 16:05:01.000000 mini_scikit_learn-0.1.0/mini_scikit_learn/NN.py
--rw-rw-rw-   0        0        0     1452 2024-06-01 13:36:15.000000 mini_scikit_learn-0.1.0/mini_scikit_learn/Predictor.py
--rw-rw-rw-   0        0        0     9746 2024-06-01 13:41:13.000000 mini_scikit_learn-0.1.0/mini_scikit_learn/RandomForest.py
--rw-rw-rw-   0        0        0     1001 2024-05-22 18:57:48.000000 mini_scikit_learn-0.1.0/mini_scikit_learn/SVM.py
--rw-rw-rw-   0        0        0      535 2024-06-02 16:05:37.000000 mini_scikit_learn-0.1.0/mini_scikit_learn/__init__.py
--rw-rw-rw-   0        0        0      819 2024-05-01 21:00:46.000000 mini_scikit_learn-0.1.0/mini_scikit_learn/main.py
-drwxrwxrwx   0        0        0        0 2024-06-02 16:46:58.484954 mini_scikit_learn-0.1.0/mini_scikit_learn/metrics/
--rw-rw-rw-   0        0        0      104 2024-06-02 13:28:04.000000 mini_scikit_learn-0.1.0/mini_scikit_learn/metrics/__init__.py
--rw-rw-rw-   0        0        0     1511 2024-05-14 17:21:27.000000 mini_scikit_learn-0.1.0/mini_scikit_learn/metrics/metric.py
--rw-rw-rw-   0        0        0     1768 2024-05-08 19:11:07.000000 mini_scikit_learn-0.1.0/mini_scikit_learn/test1.py
--rw-rw-rw-   0        0        0     1674 2024-06-02 16:42:36.000000 mini_scikit_learn-0.1.0/mini_scikit_learn/test2.py
--rw-rw-rw-   0        0        0      771 2024-05-22 19:35:27.000000 mini_scikit_learn-0.1.0/mini_scikit_learn/test_ada.py
--rw-rw-rw-   0        0        0      732 2024-05-22 18:05:25.000000 mini_scikit_learn-0.1.0/mini_scikit_learn/test_cv.py
--rw-rw-rw-   0        0        0     2024 2024-05-22 18:24:36.000000 mini_scikit_learn-0.1.0/mini_scikit_learn/test_dt.py
--rw-rw-rw-   0        0        0     1242 2024-05-14 16:27:56.000000 mini_scikit_learn-0.1.0/mini_scikit_learn/test_dtr.py
--rw-rw-rw-   0        0        0     1805 2024-05-22 17:48:17.000000 mini_scikit_learn-0.1.0/mini_scikit_learn/test_knn.py
--rw-rw-rw-   0        0        0     1197 2024-05-14 23:37:28.000000 mini_scikit_learn-0.1.0/mini_scikit_learn/test_lg.py
--rw-rw-rw-   0        0        0     2249 2024-05-15 08:54:45.000000 mini_scikit_learn-0.1.0/mini_scikit_learn/test_lgr.py
--rw-rw-rw-   0        0        0     3100 2024-05-05 19:11:00.000000 mini_scikit_learn-0.1.0/mini_scikit_learn/test_nb.py
--rw-rw-rw-   0        0        0     4047 2024-05-07 15:17:35.000000 mini_scikit_learn-0.1.0/mini_scikit_learn/test_nn.py
--rw-rw-rw-   0        0        0     1981 2024-05-07 15:29:08.000000 mini_scikit_learn-0.1.0/mini_scikit_learn/test_nn2.py
--rw-rw-rw-   0        0        0     2228 2024-05-08 08:33:02.000000 mini_scikit_learn-0.1.0/mini_scikit_learn/test_nn_3.py
--rw-rw-rw-   0        0        0     3939 2024-05-14 17:29:42.000000 mini_scikit_learn-0.1.0/mini_scikit_learn/test_rf.py
--rw-rw-rw-   0        0        0     2046 2024-05-15 09:12:06.000000 mini_scikit_learn-0.1.0/mini_scikit_learn/test_stacking.py
--rw-rw-rw-   0        0        0     2364 2024-05-15 09:18:44.000000 mini_scikit_learn-0.1.0/mini_scikit_learn/test_voting.py
-drwxrwxrwx   0        0        0        0 2024-06-02 16:46:58.507472 mini_scikit_learn-0.1.0/mini_scikit_learn/transformers/
--rw-rw-rw-   0        0        0     2149 2024-06-02 13:09:30.000000 mini_scikit_learn-0.1.0/mini_scikit_learn/transformers/Encoders.py
--rw-rw-rw-   0        0        0     1550 2024-06-01 13:45:18.000000 mini_scikit_learn-0.1.0/mini_scikit_learn/transformers/Imputers.py
--rw-rw-rw-   0        0        0     1131 2024-06-02 16:44:55.000000 mini_scikit_learn-0.1.0/mini_scikit_learn/transformers/Transfomer.py
--rw-rw-rw-   0        0        0      423 2024-06-02 16:46:52.000000 mini_scikit_learn-0.1.0/mini_scikit_learn/transformers/__init__.py
--rw-rw-rw-   0        0        0      621 2024-05-14 08:53:30.000000 mini_scikit_learn-0.1.0/mini_scikit_learn/transformers/encoderTest.py
-drwxrwxrwx   0        0        0        0 2024-06-02 16:46:58.509946 mini_scikit_learn-0.1.0/mini_scikit_learn/utils/
--rw-rw-rw-   0        0        0     5149 2024-05-08 08:28:46.000000 mini_scikit_learn-0.1.0/mini_scikit_learn/utils/NeuralNetwork.py
--rw-rw-rw-   0        0        0       97 2024-06-01 12:46:30.000000 mini_scikit_learn-0.1.0/mini_scikit_learn/utils/__init__.py
--rw-rw-rw-   0        0        0     1947 2024-06-02 13:52:22.000000 mini_scikit_learn-0.1.0/mini_scikit_learn/utils/cross_validation.py
--rw-rw-rw-   0        0        0     3146 2024-06-02 14:04:24.000000 mini_scikit_learn-0.1.0/mini_scikit_learn/utils/train_test_split.py
-drwxrwxrwx   0        0        0        0 2024-06-02 16:46:58.479940 mini_scikit_learn-0.1.0/mini_scikit_learn.egg-info/
--rw-rw-rw-   0        0        0      580 2024-06-02 16:46:58.000000 mini_scikit_learn-0.1.0/mini_scikit_learn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1600 2024-06-02 16:46:58.000000 mini_scikit_learn-0.1.0/mini_scikit_learn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 16:46:58.000000 mini_scikit_learn-0.1.0/mini_scikit_learn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-06-02 16:46:58.000000 mini_scikit_learn-0.1.0/mini_scikit_learn.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-06-02 16:46:58.000000 mini_scikit_learn-0.1.0/mini_scikit_learn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-06-02 16:46:58.518849 mini_scikit_learn-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      873 2024-05-22 23:42:04.000000 mini_scikit_learn-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 20:22:51.318957 mini_scikit_learn-0.1.1/
+-rw-rw-rw-   0        0        0     5396 2024-06-02 20:22:51.317955 mini_scikit_learn-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4102 2024-06-02 20:15:08.000000 mini_scikit_learn-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-06-02 20:22:51.245818 mini_scikit_learn-0.1.1/mini_scikit_learn/
+-rw-rw-rw-   0        0        0     2692 2024-05-22 21:00:24.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/AdaBoost.py
+-rw-rw-rw-   0        0        0     8408 2024-06-01 13:34:18.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/DecisionTree.py
+-rw-rw-rw-   0        0        0     1164 2024-05-01 19:19:40.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/Estimator.py
+-rw-rw-rw-   0        0        0     2214 2024-06-02 19:51:34.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/KnnEstimator.py
+-rw-rw-rw-   0        0        0    10969 2024-06-01 13:38:26.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/LinearModel.py
+-rw-rw-rw-   0        0        0     2688 2024-05-14 23:36:33.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/LogisticRegression.py
+-rw-rw-rw-   0        0        0     4585 2024-06-02 20:03:48.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/ModelEnsembler.py
+-rw-rw-rw-   0        0        0     2616 2024-05-14 18:06:27.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/NBClassifier.py
+-rw-rw-rw-   0        0        0     2291 2024-06-02 16:05:01.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/NN.py
+-rw-rw-rw-   0        0        0     1452 2024-06-01 13:36:15.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/Predictor.py
+-rw-rw-rw-   0        0        0     9746 2024-06-01 13:41:13.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/RandomForest.py
+-rw-rw-rw-   0        0        0     1001 2024-05-22 18:57:48.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/SVM.py
+-rw-rw-rw-   0        0        0      649 2024-06-02 19:45:21.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/__init__.py
+-rw-rw-rw-   0        0        0      819 2024-05-01 21:00:46.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/main.py
+drwxrwxrwx   0        0        0        0 2024-06-02 20:22:51.283961 mini_scikit_learn-0.1.1/mini_scikit_learn/metrics/
+-rw-rw-rw-   0        0        0      104 2024-06-02 13:28:04.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/metrics/__init__.py
+-rw-rw-rw-   0        0        0     1511 2024-05-14 17:21:27.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/metrics/metric.py
+drwxrwxrwx   0        0        0        0 2024-06-02 20:22:51.292930 mini_scikit_learn-0.1.1/mini_scikit_learn/model_selection/
+-rw-rw-rw-   0        0        0     2724 2024-06-02 18:52:51.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/model_selection/GridSearch.py
+-rw-rw-rw-   0        0        0     3325 2024-06-02 19:17:55.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/model_selection/RandomSearch.py
+-rw-rw-rw-   0        0        0       74 2024-06-02 18:58:49.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/model_selection/__init__.py
+-rw-rw-rw-   0        0        0     1768 2024-05-08 19:11:07.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/test1.py
+-rw-rw-rw-   0        0        0     1674 2024-06-02 16:42:36.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/test2.py
+-rw-rw-rw-   0        0        0      771 2024-05-22 19:35:27.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/test_ada.py
+-rw-rw-rw-   0        0        0      732 2024-05-22 18:05:25.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/test_cv.py
+-rw-rw-rw-   0        0        0     2024 2024-05-22 18:24:36.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/test_dt.py
+-rw-rw-rw-   0        0        0     1242 2024-05-14 16:27:56.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/test_dtr.py
+-rw-rw-rw-   0        0        0     1804 2024-06-02 19:38:30.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/test_knn.py
+-rw-rw-rw-   0        0        0     1197 2024-05-14 23:37:28.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/test_lg.py
+-rw-rw-rw-   0        0        0     2249 2024-05-15 08:54:45.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/test_lgr.py
+-rw-rw-rw-   0        0        0     3100 2024-05-05 19:11:00.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/test_nb.py
+-rw-rw-rw-   0        0        0     4047 2024-05-07 15:17:35.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/test_nn.py
+-rw-rw-rw-   0        0        0     1981 2024-05-07 15:29:08.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/test_nn2.py
+-rw-rw-rw-   0        0        0     3939 2024-05-14 17:29:42.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/test_rf.py
+-rw-rw-rw-   0        0        0     2046 2024-05-15 09:12:06.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/test_stacking.py
+-rw-rw-rw-   0        0        0     2364 2024-05-15 09:18:44.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/test_voting.py
+drwxrwxrwx   0        0        0        0 2024-06-02 20:22:51.304025 mini_scikit_learn-0.1.1/mini_scikit_learn/transformers/
+-rw-rw-rw-   0        0        0     2149 2024-06-02 13:09:30.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/transformers/Encoders.py
+-rw-rw-rw-   0        0        0     1550 2024-06-01 13:45:18.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/transformers/Imputers.py
+-rw-rw-rw-   0        0        0     1131 2024-06-02 16:44:55.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/transformers/Transfomer.py
+-rw-rw-rw-   0        0        0      229 2024-06-02 17:33:02.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/transformers/__init__.py
+-rw-rw-rw-   0        0        0      621 2024-05-14 08:53:30.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/transformers/encoderTest.py
+drwxrwxrwx   0        0        0        0 2024-06-02 20:22:51.311853 mini_scikit_learn-0.1.1/mini_scikit_learn/utils/
+-rw-rw-rw-   0        0        0     5149 2024-05-08 08:28:46.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/utils/NeuralNetwork.py
+-rw-rw-rw-   0        0        0       99 2024-06-02 18:55:11.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/utils/__init__.py
+-rw-rw-rw-   0        0        0     1947 2024-06-02 13:52:22.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/utils/cross_validation.py
+-rw-rw-rw-   0        0        0     3146 2024-06-02 14:04:24.000000 mini_scikit_learn-0.1.1/mini_scikit_learn/utils/train_test_split.py
+drwxrwxrwx   0        0        0        0 2024-06-02 20:22:51.278887 mini_scikit_learn-0.1.1/mini_scikit_learn.egg-info/
+-rw-rw-rw-   0        0        0     5396 2024-06-02 20:22:51.000000 mini_scikit_learn-0.1.1/mini_scikit_learn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1713 2024-06-02 20:22:51.000000 mini_scikit_learn-0.1.1/mini_scikit_learn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 20:22:51.000000 mini_scikit_learn-0.1.1/mini_scikit_learn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-06-02 20:22:51.000000 mini_scikit_learn-0.1.1/mini_scikit_learn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-06-02 20:22:51.000000 mini_scikit_learn-0.1.1/mini_scikit_learn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-02 20:22:51.319956 mini_scikit_learn-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      873 2024-06-02 20:22:43.000000 mini_scikit_learn-0.1.1/setup.py
```

### Comparing `mini_scikit_learn-0.1.0/mini_scikit_learn/AdaBoost.py` & `mini_scikit_learn-0.1.1/mini_scikit_learn/AdaBoost.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.0/mini_scikit_learn/DecisionTree.py` & `mini_scikit_learn-0.1.1/mini_scikit_learn/DecisionTree.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.0/mini_scikit_learn/Estimator.py` & `mini_scikit_learn-0.1.1/mini_scikit_learn/Estimator.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.0/mini_scikit_learn/KnnEstimator.py` & `mini_scikit_learn-0.1.1/mini_scikit_learn/KnnEstimator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 from  .Estimator import Estimator
 from .Predictor import Predictor
 
-class KnnEstimator(Predictor, Estimator):
+class KNNEstimator(Predictor, Estimator):
     
     def __init__(self, n_neighbors=5, p=2):
         """This is the constructor of the class.
         Parameters:
         n_neighbors (int): The number of neighbors to consider for prediction.
         p (int): The order of the Minkowski distance.
         """
```

### Comparing `mini_scikit_learn-0.1.0/mini_scikit_learn/LinearModel.py` & `mini_scikit_learn-0.1.1/mini_scikit_learn/LinearModel.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.0/mini_scikit_learn/LogisticRegression.py` & `mini_scikit_learn-0.1.1/mini_scikit_learn/LogisticRegression.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.0/mini_scikit_learn/ModelEnsembler.py` & `mini_scikit_learn-0.1.1/mini_scikit_learn/ModelEnsembler.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,36 +102,31 @@
         meta_model (Estimator): The meta model that combines the base models' predictions.
         """
         self.base_models = base_models
         self.meta_model = meta_model
         self.is_fitted = False
         super().__init__(self)
 
-    def fit(self, X, y):
+    def fit(self, X, y, n_iterations=1000):
         for model in self.base_models:
             model.fit(X, y)
+            print("Accuracy of Model: ",base_models.index(model))
             print(model.score(X, y))
         X_meta = np.array([model.predict(X) for model in self.base_models]).T
-        print("X_meta shape")
-        print(X_meta.shape)
-        self.meta_model.fit(X_meta, y,lr=0.001)
+        self.meta_model.fit(X_meta, y)
         print("Meta model score")
         print(self.meta_model.score(X_meta, y))
         self.is_fitted = True
         return self
 
     def predict(self, X):
         if not self.is_fitted:
             raise ValueError("The model has not been fitted yet.")
         X_meta = np.array([model.predict(X) for model in self.base_models]).T
         answer=self.meta_model.predict(X_meta)
-        print("Answer shape")
-        print(answer.shape)
-        print("Answer")
-        print(answer)
         return answer
 
     def score(self, X, y):
         """This method is used to evaluate the model on the test data."""
         y_pred = self.predict(X)
         return np.mean(y == y_pred)
```

### Comparing `mini_scikit_learn-0.1.0/mini_scikit_learn/NBClassifier.py` & `mini_scikit_learn-0.1.1/mini_scikit_learn/NBClassifier.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.0/mini_scikit_learn/NN.py` & `mini_scikit_learn-0.1.1/mini_scikit_learn/NN.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.0/mini_scikit_learn/Predictor.py` & `mini_scikit_learn-0.1.1/mini_scikit_learn/Predictor.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.0/mini_scikit_learn/RandomForest.py` & `mini_scikit_learn-0.1.1/mini_scikit_learn/RandomForest.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.0/mini_scikit_learn/SVM.py` & `mini_scikit_learn-0.1.1/mini_scikit_learn/SVM.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.0/mini_scikit_learn/main.py` & `mini_scikit_learn-0.1.1/mini_scikit_learn/main.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.0/mini_scikit_learn/metrics/metric.py` & `mini_scikit_learn-0.1.1/mini_scikit_learn/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.0/mini_scikit_learn/test1.py` & `mini_scikit_learn-0.1.1/mini_scikit_learn/test1.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.0/mini_scikit_learn/test2.py` & `mini_scikit_learn-0.1.1/mini_scikit_learn/test2.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.0/mini_scikit_learn/test_ada.py` & `mini_scikit_learn-0.1.1/mini_scikit_learn/test_ada.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.0/mini_scikit_learn/test_cv.py` & `mini_scikit_learn-0.1.1/mini_scikit_learn/test_cv.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.0/mini_scikit_learn/test_dt.py` & `mini_scikit_learn-0.1.1/mini_scikit_learn/test_dt.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.0/mini_scikit_learn/test_dtr.py` & `mini_scikit_learn-0.1.1/mini_scikit_learn/test_dtr.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.0/mini_scikit_learn/test_knn.py` & `mini_scikit_learn-0.1.1/mini_scikit_learn/test_knn.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from KnnEstimator import KnnEstimator
+from KnnEtimator import KNNEstimator
 from sklearn.datasets import load_digits, load_iris
 from sklearn.model_selection import train_test_split
 from sklearn.neighbors import KNeighborsClassifier as SklearnKNeighborsClassifier
 
 # Load the datasets
 digits = load_digits()
 X_digits, y_digits = digits.data, digits.target
@@ -11,23 +11,23 @@
 X_iris, y_iris = iris.data, iris.target
 
 # Split the data for digits dataset
 X_digits_train, X_digits_test, y_digits_train, y_digits_test = train_test_split(X_digits, y_digits, test_size=0.2, random_state=42)
 
 X_iris_train, X_iris_test, y_iris_train, y_iris_test = train_test_split(X_iris, y_iris, test_size=0.2, random_state=42)
 
-your_model_digits = KnnEstimator()  # Use k=5 as an example
+your_model_digits = KNNEstimator()  # Use k=5 as an example
 your_model_digits.fit(X_digits_train, y_digits_train)
 your_score_digits = your_model_digits.score(X_digits_test, y_digits_test)
-print("Your KnnEstimator Score (Digits):", your_score_digits)
+print("Your KNNEstimator Score (Digits):", your_score_digits)
 
-your_model_iris = KnnEstimator()  # Use k=5 as an example
+your_model_iris = KNNEstimator()  # Use k=5 as an example
 your_model_iris.fit(X_iris_train, y_iris_train)
 your_score_iris = your_model_iris.score(X_iris_test, y_iris_test)
-print("Your KnnEstimator Score (Iris):", your_score_iris)
+print("Your KNNEstimator Score (Iris):", your_score_iris)
 
 sklearn_model_digits = SklearnKNeighborsClassifier(n_neighbors=5)  # Use n_neighbors=5 as an example
 sklearn_model_digits.fit(X_digits_train, y_digits_train)
 sklearn_score_digits = sklearn_model_digits.score(X_digits_test, y_digits_test)
 print("Scikit-learn KNeighborsClassifier Score (Digits):", sklearn_score_digits)
 
 sklearn_model_iris = SklearnKNeighborsClassifier(n_neighbors=5)  # Use n_neighbors=5 as an example
```

### Comparing `mini_scikit_learn-0.1.0/mini_scikit_learn/test_lg.py` & `mini_scikit_learn-0.1.1/mini_scikit_learn/test_lg.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.0/mini_scikit_learn/test_lgr.py` & `mini_scikit_learn-0.1.1/mini_scikit_learn/test_lgr.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.0/mini_scikit_learn/test_nb.py` & `mini_scikit_learn-0.1.1/mini_scikit_learn/test_nb.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.0/mini_scikit_learn/test_nn.py` & `mini_scikit_learn-0.1.1/mini_scikit_learn/test_nn.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.0/mini_scikit_learn/test_nn2.py` & `mini_scikit_learn-0.1.1/mini_scikit_learn/test_nn2.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.0/mini_scikit_learn/test_rf.py` & `mini_scikit_learn-0.1.1/mini_scikit_learn/test_rf.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.0/mini_scikit_learn/test_stacking.py` & `mini_scikit_learn-0.1.1/mini_scikit_learn/test_stacking.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.0/mini_scikit_learn/test_voting.py` & `mini_scikit_learn-0.1.1/mini_scikit_learn/test_voting.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.0/mini_scikit_learn/transformers/Encoders.py` & `mini_scikit_learn-0.1.1/mini_scikit_learn/transformers/Encoders.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.0/mini_scikit_learn/transformers/Imputers.py` & `mini_scikit_learn-0.1.1/mini_scikit_learn/transformers/Imputers.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.0/mini_scikit_learn/transformers/Transfomer.py` & `mini_scikit_learn-0.1.1/mini_scikit_learn/transformers/Transfomer.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.0/mini_scikit_learn/transformers/encoderTest.py` & `mini_scikit_learn-0.1.1/mini_scikit_learn/transformers/encoderTest.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.0/mini_scikit_learn/utils/NeuralNetwork.py` & `mini_scikit_learn-0.1.1/mini_scikit_learn/utils/NeuralNetwork.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.0/mini_scikit_learn/utils/cross_validation.py` & `mini_scikit_learn-0.1.1/mini_scikit_learn/utils/cross_validation.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.0/mini_scikit_learn/utils/train_test_split.py` & `mini_scikit_learn-0.1.1/mini_scikit_learn/utils/train_test_split.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.0/mini_scikit_learn.egg-info/SOURCES.txt` & `mini_scikit_learn-0.1.1/mini_scikit_learn.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -22,25 +22,27 @@
 mini_scikit_learn/test_dtr.py
 mini_scikit_learn/test_knn.py
 mini_scikit_learn/test_lg.py
 mini_scikit_learn/test_lgr.py
 mini_scikit_learn/test_nb.py
 mini_scikit_learn/test_nn.py
 mini_scikit_learn/test_nn2.py
-mini_scikit_learn/test_nn_3.py
 mini_scikit_learn/test_rf.py
 mini_scikit_learn/test_stacking.py
 mini_scikit_learn/test_voting.py
 mini_scikit_learn.egg-info/PKG-INFO
 mini_scikit_learn.egg-info/SOURCES.txt
 mini_scikit_learn.egg-info/dependency_links.txt
 mini_scikit_learn.egg-info/requires.txt
 mini_scikit_learn.egg-info/top_level.txt
 mini_scikit_learn/metrics/__init__.py
 mini_scikit_learn/metrics/metric.py
+mini_scikit_learn/model_selection/GridSearch.py
+mini_scikit_learn/model_selection/RandomSearch.py
+mini_scikit_learn/model_selection/__init__.py
 mini_scikit_learn/transformers/Encoders.py
 mini_scikit_learn/transformers/Imputers.py
 mini_scikit_learn/transformers/Transfomer.py
 mini_scikit_learn/transformers/__init__.py
 mini_scikit_learn/transformers/encoderTest.py
 mini_scikit_learn/utils/NeuralNetwork.py
 mini_scikit_learn/utils/__init__.py
```

### Comparing `mini_scikit_learn-0.1.0/setup.py` & `mini_scikit_learn-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mini_scikit_learn',  # Replace with your package name
-    version='0.1.0',  # Initial version of your package
+    version='0.1.1',  # Initial version of your package
     author='Yassir Fri',
     author_email='your.email@example.com',
     description='A brief description of your package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     #url='https://github.com/yourusername/your-repo-name',  # Replace with your GitHub repository URL
     packages=find_packages(),  # Automatically find packages in the directory
```

