# Comparing `tmp/mini_scikit_learn-0.1.5.tar.gz` & `tmp/mini_scikit_learn-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mini_scikit_learn-0.1.5.tar", last modified: Sun Jun  2 23:22:50 2024, max compression
+gzip compressed data, was "mini_scikit_learn-0.1.6.tar", last modified: Sun Jun  2 23:53:47 2024, max compression
```

## Comparing `mini_scikit_learn-0.1.5.tar` & `mini_scikit_learn-0.1.6.tar`

### file list

```diff
@@ -1,46 +1,62 @@
-drwxrwxrwx   0        0        0        0 2024-06-02 23:22:50.124792 mini_scikit_learn-0.1.5/
--rw-rw-rw-   0        0        0     6155 2024-06-02 23:22:50.123782 mini_scikit_learn-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     4754 2024-06-02 22:00:40.000000 mini_scikit_learn-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2024-06-02 23:22:50.007863 mini_scikit_learn-0.1.5/mini_scikit_learn/
--rw-rw-rw-   0        0        0     4984 2024-06-02 23:15:29.000000 mini_scikit_learn-0.1.5/mini_scikit_learn/AdaBoost.py
--rw-rw-rw-   0        0        0    12707 2024-06-02 23:15:29.000000 mini_scikit_learn-0.1.5/mini_scikit_learn/DecisionTree.py
--rw-rw-rw-   0        0        0     1865 2024-06-02 23:15:29.000000 mini_scikit_learn-0.1.5/mini_scikit_learn/Estimator.py
--rw-rw-rw-   0        0        0     2265 2024-06-02 23:15:49.000000 mini_scikit_learn-0.1.5/mini_scikit_learn/KnnEstimator.py
--rw-rw-rw-   0        0        0     9832 2024-06-02 23:15:29.000000 mini_scikit_learn-0.1.5/mini_scikit_learn/LinearModel.py
--rw-rw-rw-   0        0        0     4952 2024-06-02 22:49:10.000000 mini_scikit_learn-0.1.5/mini_scikit_learn/LogisticRegression.py
--rw-rw-rw-   0        0        0     8512 2024-06-02 23:21:51.000000 mini_scikit_learn-0.1.5/mini_scikit_learn/ModelEnsembler.py
--rw-rw-rw-   0        0        0     3817 2024-06-02 22:49:10.000000 mini_scikit_learn-0.1.5/mini_scikit_learn/NBClassifier.py
--rw-rw-rw-   0        0        0     5092 2024-06-02 23:15:29.000000 mini_scikit_learn-0.1.5/mini_scikit_learn/NN.py
--rw-rw-rw-   0        0        0     1679 2024-06-02 23:15:57.000000 mini_scikit_learn-0.1.5/mini_scikit_learn/Predictor.py
--rw-rw-rw-   0        0        0    10782 2024-06-02 23:15:29.000000 mini_scikit_learn-0.1.5/mini_scikit_learn/RandomForest.py
--rw-rw-rw-   0        0        0     1542 2024-06-02 23:16:32.000000 mini_scikit_learn-0.1.5/mini_scikit_learn/SVM.py
--rw-rw-rw-   0        0        0      819 2024-05-01 21:00:46.000000 mini_scikit_learn-0.1.5/mini_scikit_learn/main.py
-drwxrwxrwx   0        0        0        0 2024-06-02 23:22:50.112215 mini_scikit_learn-0.1.5/mini_scikit_learn/metrics/
--rw-rw-rw-   0        0        0     4575 2024-06-02 22:49:10.000000 mini_scikit_learn-0.1.5/mini_scikit_learn/metrics/metric.py
--rw-rw-rw-   0        0        0     1768 2024-05-08 19:11:07.000000 mini_scikit_learn-0.1.5/mini_scikit_learn/test1.py
--rw-rw-rw-   0        0        0     1735 2024-06-02 23:15:29.000000 mini_scikit_learn-0.1.5/mini_scikit_learn/test2.py
--rw-rw-rw-   0        0        0      771 2024-05-22 19:35:27.000000 mini_scikit_learn-0.1.5/mini_scikit_learn/test_ada.py
--rw-rw-rw-   0        0        0      732 2024-05-22 18:05:25.000000 mini_scikit_learn-0.1.5/mini_scikit_learn/test_cv.py
--rw-rw-rw-   0        0        0     2024 2024-05-22 18:24:36.000000 mini_scikit_learn-0.1.5/mini_scikit_learn/test_dt.py
--rw-rw-rw-   0        0        0     1242 2024-05-14 16:27:56.000000 mini_scikit_learn-0.1.5/mini_scikit_learn/test_dtr.py
--rw-rw-rw-   0        0        0     1805 2024-06-02 23:15:29.000000 mini_scikit_learn-0.1.5/mini_scikit_learn/test_knn.py
--rw-rw-rw-   0        0        0     1197 2024-05-14 23:37:28.000000 mini_scikit_learn-0.1.5/mini_scikit_learn/test_lg.py
--rw-rw-rw-   0        0        0     2249 2024-05-15 08:54:45.000000 mini_scikit_learn-0.1.5/mini_scikit_learn/test_lgr.py
--rw-rw-rw-   0        0        0     3100 2024-05-05 19:11:00.000000 mini_scikit_learn-0.1.5/mini_scikit_learn/test_nb.py
--rw-rw-rw-   0        0        0     4047 2024-05-07 15:17:35.000000 mini_scikit_learn-0.1.5/mini_scikit_learn/test_nn.py
--rw-rw-rw-   0        0        0     1981 2024-05-07 15:29:08.000000 mini_scikit_learn-0.1.5/mini_scikit_learn/test_nn2.py
--rw-rw-rw-   0        0        0     3939 2024-05-14 17:29:42.000000 mini_scikit_learn-0.1.5/mini_scikit_learn/test_rf.py
--rw-rw-rw-   0        0        0     2046 2024-05-15 09:12:06.000000 mini_scikit_learn-0.1.5/mini_scikit_learn/test_stacking.py
--rw-rw-rw-   0        0        0     2364 2024-05-15 09:18:44.000000 mini_scikit_learn-0.1.5/mini_scikit_learn/test_voting.py
-drwxrwxrwx   0        0        0        0 2024-06-02 23:22:50.120793 mini_scikit_learn-0.1.5/mini_scikit_learn/utils/
--rw-rw-rw-   0        0        0     5149 2024-05-08 08:28:46.000000 mini_scikit_learn-0.1.5/mini_scikit_learn/utils/NeuralNetwork.py
--rw-rw-rw-   0        0        0     1380 2024-06-02 23:15:29.000000 mini_scikit_learn-0.1.5/mini_scikit_learn/utils/cross_validation.py
--rw-rw-rw-   0        0        0     1769 2024-06-02 23:15:29.000000 mini_scikit_learn-0.1.5/mini_scikit_learn/utils/train_test_split.py
-drwxrwxrwx   0        0        0        0 2024-06-02 23:22:50.108208 mini_scikit_learn-0.1.5/mini_scikit_learn.egg-info/
--rw-rw-rw-   0        0        0     6155 2024-06-02 23:22:49.000000 mini_scikit_learn-0.1.5/mini_scikit_learn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1245 2024-06-02 23:22:49.000000 mini_scikit_learn-0.1.5/mini_scikit_learn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 23:22:49.000000 mini_scikit_learn-0.1.5/mini_scikit_learn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-06-02 23:22:49.000000 mini_scikit_learn-0.1.5/mini_scikit_learn.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 23:22:49.000000 mini_scikit_learn-0.1.5/mini_scikit_learn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-06-02 23:22:50.125788 mini_scikit_learn-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      719 2024-06-02 23:22:42.000000 mini_scikit_learn-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 23:53:47.342755 mini_scikit_learn-0.1.6/
+-rw-rw-rw-   0        0        0     6155 2024-06-02 23:53:47.340766 mini_scikit_learn-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4754 2024-06-02 22:00:40.000000 mini_scikit_learn-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-06-02 23:53:46.851424 mini_scikit_learn-0.1.6/mini_scikit_learn/
+-rw-rw-rw-   0        0        0     4031 2024-06-02 23:49:58.000000 mini_scikit_learn-0.1.6/mini_scikit_learn/AdaBoost.py
+-rw-rw-rw-   0        0        0    12699 2024-06-02 23:49:58.000000 mini_scikit_learn-0.1.6/mini_scikit_learn/DecisionTree.py
+-rw-rw-rw-   0        0        0     1871 2024-06-02 23:49:58.000000 mini_scikit_learn-0.1.6/mini_scikit_learn/Estimator.py
+-rw-rw-rw-   0        0        0     2966 2024-06-02 23:49:58.000000 mini_scikit_learn-0.1.6/mini_scikit_learn/KnnEstimator.py
+-rw-rw-rw-   0        0        0     9872 2024-06-02 23:49:58.000000 mini_scikit_learn-0.1.6/mini_scikit_learn/LinearModel.py
+-rw-rw-rw-   0        0        0     4952 2024-06-02 23:49:58.000000 mini_scikit_learn-0.1.6/mini_scikit_learn/LogisticRegression.py
+-rw-rw-rw-   0        0        0     9009 2024-06-02 23:53:13.000000 mini_scikit_learn-0.1.6/mini_scikit_learn/ModelEnsembler.py
+-rw-rw-rw-   0        0        0     3817 2024-06-02 23:49:58.000000 mini_scikit_learn-0.1.6/mini_scikit_learn/NBClassifier.py
+-rw-rw-rw-   0        0        0     5098 2024-06-02 23:49:58.000000 mini_scikit_learn-0.1.6/mini_scikit_learn/NN.py
+-rw-rw-rw-   0        0        0     1689 2024-06-02 23:49:58.000000 mini_scikit_learn-0.1.6/mini_scikit_learn/Predictor.py
+-rw-rw-rw-   0        0        0    10836 2024-06-02 23:49:58.000000 mini_scikit_learn-0.1.6/mini_scikit_learn/RandomForest.py
+-rw-rw-rw-   0        0        0     2315 2024-06-02 23:49:58.000000 mini_scikit_learn-0.1.6/mini_scikit_learn/SVM.py
+-rw-rw-rw-   0        0        0      649 2024-06-02 23:49:58.000000 mini_scikit_learn-0.1.6/mini_scikit_learn/__init__.py
+-rw-rw-rw-   0        0        0      819 2024-06-02 23:49:58.000000 mini_scikit_learn-0.1.6/mini_scikit_learn/main.py
+drwxrwxrwx   0        0        0        0 2024-06-02 23:53:47.207356 mini_scikit_learn-0.1.6/mini_scikit_learn/metrics/
+-rw-rw-rw-   0        0        0      201 2024-06-02 23:49:58.000000 mini_scikit_learn-0.1.6/mini_scikit_learn/metrics/__init__.py
+-rw-rw-rw-   0        0        0     4575 2024-06-02 23:49:58.000000 mini_scikit_learn-0.1.6/mini_scikit_learn/metrics/metric.py
+drwxrwxrwx   0        0        0        0 2024-06-02 23:53:47.290427 mini_scikit_learn-0.1.6/mini_scikit_learn/model_selection/
+-rw-rw-rw-   0        0        0     2724 2024-06-02 23:49:58.000000 mini_scikit_learn-0.1.6/mini_scikit_learn/model_selection/GridSearch.py
+-rw-rw-rw-   0        0        0     3325 2024-06-02 23:49:58.000000 mini_scikit_learn-0.1.6/mini_scikit_learn/model_selection/RandomSearch.py
+-rw-rw-rw-   0        0        0       74 2024-06-02 23:49:58.000000 mini_scikit_learn-0.1.6/mini_scikit_learn/model_selection/__init__.py
+-rw-rw-rw-   0        0        0     1768 2024-06-02 23:49:58.000000 mini_scikit_learn-0.1.6/mini_scikit_learn/test1.py
+-rw-rw-rw-   0        0        0     1674 2024-06-02 23:49:58.000000 mini_scikit_learn-0.1.6/mini_scikit_learn/test2.py
+-rw-rw-rw-   0        0        0      771 2024-06-02 23:49:58.000000 mini_scikit_learn-0.1.6/mini_scikit_learn/test_ada.py
+-rw-rw-rw-   0        0        0      732 2024-06-02 23:49:58.000000 mini_scikit_learn-0.1.6/mini_scikit_learn/test_cv.py
+-rw-rw-rw-   0        0        0     2024 2024-06-02 23:49:58.000000 mini_scikit_learn-0.1.6/mini_scikit_learn/test_dt.py
+-rw-rw-rw-   0        0        0     1242 2024-06-02 23:49:58.000000 mini_scikit_learn-0.1.6/mini_scikit_learn/test_dtr.py
+-rw-rw-rw-   0        0        0     1804 2024-06-02 23:49:58.000000 mini_scikit_learn-0.1.6/mini_scikit_learn/test_knn.py
+-rw-rw-rw-   0        0        0     1197 2024-06-02 23:49:58.000000 mini_scikit_learn-0.1.6/mini_scikit_learn/test_lg.py
+-rw-rw-rw-   0        0        0     2249 2024-06-02 23:49:58.000000 mini_scikit_learn-0.1.6/mini_scikit_learn/test_lgr.py
+-rw-rw-rw-   0        0        0     3100 2024-06-02 23:49:58.000000 mini_scikit_learn-0.1.6/mini_scikit_learn/test_nb.py
+-rw-rw-rw-   0        0        0     4047 2024-06-02 23:49:58.000000 mini_scikit_learn-0.1.6/mini_scikit_learn/test_nn.py
+-rw-rw-rw-   0        0        0     1981 2024-06-02 23:49:58.000000 mini_scikit_learn-0.1.6/mini_scikit_learn/test_nn2.py
+-rw-rw-rw-   0        0        0     2257 2024-06-02 23:49:58.000000 mini_scikit_learn-0.1.6/mini_scikit_learn/test_nn_digits.py
+-rw-rw-rw-   0        0        0     2339 2024-06-02 23:49:58.000000 mini_scikit_learn-0.1.6/mini_scikit_learn/test_nn_iris.py
+-rw-rw-rw-   0        0        0     3939 2024-06-02 23:49:58.000000 mini_scikit_learn-0.1.6/mini_scikit_learn/test_rf.py
+-rw-rw-rw-   0        0        0     2046 2024-06-02 23:49:58.000000 mini_scikit_learn-0.1.6/mini_scikit_learn/test_stacking.py
+-rw-rw-rw-   0        0        0     2364 2024-06-02 23:49:58.000000 mini_scikit_learn-0.1.6/mini_scikit_learn/test_voting.py
+drwxrwxrwx   0        0        0        0 2024-06-02 23:53:47.308630 mini_scikit_learn-0.1.6/mini_scikit_learn/transformers/
+-rw-rw-rw-   0        0        0     4537 2024-06-02 23:49:58.000000 mini_scikit_learn-0.1.6/mini_scikit_learn/transformers/Encoders.py
+-rw-rw-rw-   0        0        0     3399 2024-06-02 23:49:58.000000 mini_scikit_learn-0.1.6/mini_scikit_learn/transformers/Imputers.py
+-rw-rw-rw-   0        0        0     1131 2024-06-02 23:49:58.000000 mini_scikit_learn-0.1.6/mini_scikit_learn/transformers/Transfomer.py
+-rw-rw-rw-   0        0        0      229 2024-06-02 23:49:58.000000 mini_scikit_learn-0.1.6/mini_scikit_learn/transformers/__init__.py
+-rw-rw-rw-   0        0        0     1175 2024-06-02 23:49:58.000000 mini_scikit_learn-0.1.6/mini_scikit_learn/transformers/encoderTest.py
+drwxrwxrwx   0        0        0        0 2024-06-02 23:53:47.337318 mini_scikit_learn-0.1.6/mini_scikit_learn/utils/
+-rw-rw-rw-   0        0        0     2670 2024-06-02 23:49:58.000000 mini_scikit_learn-0.1.6/mini_scikit_learn/utils/Kfolds.py
+-rw-rw-rw-   0        0        0     5149 2024-06-02 23:49:58.000000 mini_scikit_learn-0.1.6/mini_scikit_learn/utils/NeuralNetwork.py
+-rw-rw-rw-   0        0        0      126 2024-06-02 23:49:58.000000 mini_scikit_learn-0.1.6/mini_scikit_learn/utils/__init__.py
+-rw-rw-rw-   0        0        0     1947 2024-06-02 23:49:58.000000 mini_scikit_learn-0.1.6/mini_scikit_learn/utils/cross_validation.py
+-rw-rw-rw-   0        0        0     3146 2024-06-02 23:49:58.000000 mini_scikit_learn-0.1.6/mini_scikit_learn/utils/train_test_split.py
+drwxrwxrwx   0        0        0        0 2024-06-02 23:53:47.163399 mini_scikit_learn-0.1.6/mini_scikit_learn.egg-info/
+-rw-rw-rw-   0        0        0     6155 2024-06-02 23:53:46.000000 mini_scikit_learn-0.1.6/mini_scikit_learn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1817 2024-06-02 23:53:46.000000 mini_scikit_learn-0.1.6/mini_scikit_learn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 23:53:46.000000 mini_scikit_learn-0.1.6/mini_scikit_learn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-06-02 23:53:46.000000 mini_scikit_learn-0.1.6/mini_scikit_learn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-06-02 23:53:46.000000 mini_scikit_learn-0.1.6/mini_scikit_learn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-02 23:53:47.343761 mini_scikit_learn-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      719 2024-06-02 23:51:43.000000 mini_scikit_learn-0.1.6/setup.py
```

### Comparing `mini_scikit_learn-0.1.5/PKG-INFO` & `mini_scikit_learn-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mini_scikit_learn
-Version: 0.1.5
+Version: 0.1.6
 Summary: A brief description of your package
 Home-page: https://github.com/YASSIRFRI/mini_scikit_learn.git
 Author: Yassir Fri
 Author-email: your.email@example.com
 License: UNKNOWN
 Description: # mini_scikit_learn
```

### Comparing `mini_scikit_learn-0.1.5/README.md` & `mini_scikit_learn-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.5/mini_scikit_learn/AdaBoost.py` & `mini_scikit_learn-0.1.6/mini_scikit_learn/AdaBoost.py`

 * *Files 17% similar despite different names*

```diff
@@ -53,57 +53,41 @@
         -----------
         X : numpy.ndarray
             The input features of shape (n_samples, n_features).
         y : numpy.ndarray
             The target values of shape (n_samples,).
         """
         n_samples, n_features = np.shape(X)
-
-        # Initialize weights to 1/N
         w = np.full(n_samples, (1 / n_samples))
-        
         self.clfs = []
-        # Iterate through classifiers
         for _ in range(self.n_clf):
             clf = DecisionStump()
             min_error = float('inf')
             for feature_i in range(n_features):
                 feature_values = np.expand_dims(X[:, feature_i], axis=1)
                 unique_values = np.unique(feature_values)
                 for threshold in unique_values:
                     p = 1
-                    # Set all predictions to '1' initially
                     prediction = np.ones(np.shape(y))
-                    # Label the samples whose values are below threshold as '-1'
                     prediction[X[:, feature_i] < threshold] = -1
-                    # Error = sum of weights of misclassified samples
                     error = sum(w[y != prediction])
                     if error > 0.5:
                         error = 1 - error
                         p = -1
-                    # configuration
                     if error < min_error:
                         clf.polarity = p
                         clf.threshold = threshold
                         clf.feature_index = feature_i
                         min_error = error
             clf.alpha = 0.5 * math.log((1.0 - min_error) / (min_error + 1e-10))
-            # Set all predictions to '1' initially
             predictions = np.ones(np.shape(y))
-            # The indexes where the sample values are below threshold
             negative_idx = (clf.polarity * X[:, clf.feature_index] < clf.polarity * clf.threshold)
-            # Label those as '-1'
             predictions[negative_idx] = -1
-            # Calculate new weights 
-            # Missclassified samples gets larger weights and correctly classified samples smaller
             w *= np.exp(-clf.alpha * y * predictions)
-            # Normalize to one
             w /= np.sum(w)
-
-            # Save classifier
             self.clfs.append(clf)
 
     def predict(self, X):
         """
         Predict the class labels for the input data.
 
         Parameters:
@@ -114,23 +98,18 @@
         Returns:
         --------
         y_pred : numpy.ndarray
             The predicted class labels of shape (n_samples,).
         """
         n_samples = np.shape(X)[0]
         y_pred = np.zeros((n_samples, 1))
-        # For each classifier => label the samples
         for clf in self.clfs:
             # Set all predictions to '1' initially
             predictions = np.ones(np.shape(y_pred))
             # The indexes where the sample values are below threshold
             negative_idx = (clf.polarity * X[:, clf.feature_index] < clf.polarity * clf.threshold)
-            # Label those as '-1'
             predictions[negative_idx] = -1
-            # Add predictions weighted by the classifiers alpha
-            # (alpha indicative of classifier's proficiency)
             y_pred += clf.alpha * predictions
 
-        # Return sign of prediction sum
         y_pred = np.sign(y_pred).flatten()
 
         return y_pred
```

### Comparing `mini_scikit_learn-0.1.5/mini_scikit_learn/DecisionTree.py` & `mini_scikit_learn-0.1.6/mini_scikit_learn/DecisionTree.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
-import Estimator
-import Predictor
+from .Estimator import Estimator
+from .Predictor import Predictor
 
 
-class DecisionTreeClassifier(Predictor.Predictor, Estimator.Estimator):
+class DecisionTreeClassifier(Predictor, Estimator):
     
     def __init__(self, max_depth=1000):
         """Initialize the classifier."""
         self.max_depth = max_depth
         self.tree = None
         self.is_fitted = False
         super().__init__(self)
@@ -202,15 +202,15 @@
         else:  # Decision node
             feature_index, threshold, left_subtree, right_subtree = tree
             if x[feature_index] < threshold:
                 return self._predict_tree(x, left_subtree)
             else:
                 return self._predict_tree(x, right_subtree)
 
-class DecisionTreeRegressor(Predictor.Predictor, Estimator.Estimator):
+class DecisionTreeRegressor(Predictor, Estimator):
     
     def __init__(self, max_depth=1000):
         """Initialize the regressor."""
         self.max_depth = max_depth
         self.tree = None
         self.is_fitted = False
         super().__init__(self)
```

### Comparing `mini_scikit_learn-0.1.5/mini_scikit_learn/Estimator.py` & `mini_scikit_learn-0.1.6/mini_scikit_learn/Estimator.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,10 +63,11 @@
         **params : dict
             The parameters of the model.
         Raises:
         -------
         NotImplementedError
             If the method is not implemented.
         """
-        raise NotImplementedError("The set_params method is not implemented.")
+        for param, value in params.items():
+            setattr(self, param, value)
```

### Comparing `mini_scikit_learn-0.1.5/mini_scikit_learn/KnnEstimator.py` & `mini_scikit_learn-0.1.6/mini_scikit_learn/KnnEstimator.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,35 @@
 import numpy as np
-import Estimator
-import Predictor
+from  .Estimator import Estimator
+from .Predictor import Predictor
 
 class KnnEstimator(Predictor.Predictor, Estimator.Estimator):
+    """
+    K-Nearest Neighbors Estimator.
+
+    Parameters:
+    -----------
+    n_neighbors : int, optional (default=5)
+        The number of neighbors to consider for prediction.
+    p : int, optional (default=2)
+        The order of the Minkowski distance.
+
+    Attributes:
+    -----------
+    n_neighbors : int
+        The number of neighbors to consider for prediction.
+    p : int
+        The order of the Minkowski distance.
+    X_train : numpy.ndarray or None
+        The training data.
+    y_train : numpy.ndarray or None
+        The target values.
+    is_fitted : bool
+        Indicates whether the model has been fitted.
+    """
     
     def __init__(self, n_neighbors=5, p=2):
         """Initialize the KNN estimator."""
         self.n_neighbors = n_neighbors
         self.p = p
         self.X_train = None
         self.y_train = None
@@ -81,7 +104,10 @@
         Returns:
         --------
         score : float
             The score of the model.
         """
         y_pred = self.predict(X)
         return np.mean(y == y_pred)
+
+
+
```

### Comparing `mini_scikit_learn-0.1.5/mini_scikit_learn/LinearModel.py` & `mini_scikit_learn-0.1.6/mini_scikit_learn/LinearModel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
-import Predictor
-import Estimator
+from . import Estimator
+from . import Predictor
 from numpy import log, dot, exp, shape
 import matplotlib.pyplot as plt
 from sklearn.datasets import make_classification
 from sklearn.model_selection import train_test_split
 
 class LinearModel(Predictor.Predictor, Estimator.Estimator):
     """
@@ -96,15 +96,16 @@
         return super().get_params()
     
     def set_params(self, **params):
         """This method is used to set the parameters of the model.
         Parameters:
         **params: The parameters of the model.
         """
-        self.model.fit_intercept = params["fit_intercept"]
+        for param, value in params.items():
+            setattr(self, param, value)
         return self
 
 class LogisticRegression:
     """
     Logistic Regression Classifier.
 
     Parameters:
```

### Comparing `mini_scikit_learn-0.1.5/mini_scikit_learn/LogisticRegression.py` & `mini_scikit_learn-0.1.6/mini_scikit_learn/LogisticRegression.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.5/mini_scikit_learn/ModelEnsembler.py` & `mini_scikit_learn-0.1.6/mini_scikit_learn/ModelEnsembler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-import Estimator
 import numpy as np
-import Predictor
+from . import Estimator
+from . import Predictor
 
 
 class ModelEnsembler(Predictor.Predictor, Estimator.Estimator):
     """
     Model Ensembler for averaging predictions.
 
     Parameters:
@@ -280,34 +280,49 @@
     def __init__(self, base_models, meta_model):
         """Initialize the Stacking Ensembler."""
         self.base_models = base_models
         self.meta_model = meta_model
         self.is_fitted = False
         super().__init__(self)
 
-    def fit(self, X, y):
+    def fit(self, X, y, n_iterations=1000):
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
+            print("Accuracy of Model: ",self.base_models.index(model))
             print(model.score(X, y))
         X_meta = np.array([model.predict(X) for model in self.base_models]).T
-        self.meta_model.fit(X_meta, y,lr=0.001)
+        self.meta_model.fit(X_meta, y)
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
-        print("Answer shape")
-        print(answer.shape)
-        print("Answer")
-        print(answer)
         return answer
 
     def score(self, X, y):
         """
         Evaluate the ensembled model.
 
         Parameters:
```

### Comparing `mini_scikit_learn-0.1.5/mini_scikit_learn/NBClassifier.py` & `mini_scikit_learn-0.1.6/mini_scikit_learn/NBClassifier.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.5/mini_scikit_learn/NN.py` & `mini_scikit_learn-0.1.6/mini_scikit_learn/NN.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
             The upcoming error to be propagated to the previous layer.
         """
         delta = (targets - self.output) * self.output * (1 - self.output) if previous_errors is None else previous_errors * self.output * (1 - self.output)
         upcoming_error = np.dot(delta, self.weights.T)
         self.weights += learning_rate * np.outer(self.input, delta)
         return upcoming_error
 
-class Network:
+class NeuralNetwork:
     def __init__(self):
         self.layers = []
 
     def add(self, layer):
         """
         Add a layer to the neural network.
         Parameters:
```

### Comparing `mini_scikit_learn-0.1.5/mini_scikit_learn/Predictor.py` & `mini_scikit_learn-0.1.6/mini_scikit_learn/Predictor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-import Estimator
-
-class Predictor(Estimator.Estimator):
+from .Estimator import Estimator
+class Predictor(Estimator):
     
     def __init__(self, model=None):
         """Initialize the Predictor with a given model."""
         self.model = model
         
     def predict(self, X):
         """
@@ -61,7 +60,8 @@
         self.model.fit(X_train, y_train)
         return self.predict(X_test)
     
     
     
     
     
+
```

### Comparing `mini_scikit_learn-0.1.5/mini_scikit_learn/RandomForest.py` & `mini_scikit_learn-0.1.6/mini_scikit_learn/RandomForest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
-import Estimator
-import Predictor
-from DecisionTree import DecisionTreeClassifier, DecisionTreeRegressor
+from . import Estimator
+from . import Predictor
+from .DecisionTree import DecisionTreeClassifier, DecisionTreeRegressor
 from sklearn.utils import resample
 
 class RandomForestClassifier(Predictor.Predictor, Estimator.Estimator):
     """
     Random Forest Classifier.
 
     Parameters:
@@ -90,24 +90,21 @@
                     left_indices = X[:, feature_index] < threshold
                     left_labels = y[left_indices]
                     right_labels = y[~left_indices]
                     
                     if len(left_labels) == 0 or len(right_labels) == 0:
                         continue
                     
-                    # Calculate entropy for the child nodes
                     entropy_left = self._entropy(left_labels)
                     entropy_right = self._entropy(right_labels)
                     
-                    # Calculate weighted average entropy
                     weight_left = len(left_labels) / len(y)
                     weight_right = len(right_labels) / len(y)
                     weighted_avg_entropy = weight_left * entropy_left + weight_right * entropy_right
                     
-                    # Calculate entropy gain
                     entropy_gain = parent_entropy - weighted_avg_entropy
                     
                     if entropy_gain > best_entropy_gain:
                         best_entropy_gain = entropy_gain
                         best_split = (feature_index, threshold)
             
             return best_split
@@ -301,7 +298,14 @@
         Returns:
         --------
         float
             Negative mean squared error.
         """
         y_pred = self.predict(X)
         return -mean_squared_error(y, y_pred)
+    
+    
+    def set_params(self, **params):
+        """Set the parameters of the model."""
+        for param, value in params.items():
+            setattr(self, param, value)
+        return self
```

### Comparing `mini_scikit_learn-0.1.5/mini_scikit_learn/main.py` & `mini_scikit_learn-0.1.6/mini_scikit_learn/main.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.5/mini_scikit_learn/metrics/metric.py` & `mini_scikit_learn-0.1.6/mini_scikit_learn/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.5/mini_scikit_learn/test1.py` & `mini_scikit_learn-0.1.6/mini_scikit_learn/test1.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.5/mini_scikit_learn/test2.py` & `mini_scikit_learn-0.1.6/mini_scikit_learn/test2.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from sklearn.datasets import load_digits
 from sklearn.preprocessing import StandardScaler, OneHotEncoder
 from sklearn.model_selection import train_test_split
-from NN import Network, Layer 
+from NN import NeuralNetwork, Layer 
 import numpy as np 
 # Load Digits data
 digits = load_digits()
 X = digits.data
 y = digits.target.reshape(-1, 1)
 
 # Select a subset of data for quicker training
@@ -19,40 +19,36 @@
 # Normalize features
 scaler = StandardScaler()
 X_scaled = scaler.fit_transform(X_subset)
 
 # One-hot encode labels
 encoder = OneHotEncoder()
 y_encoded = encoder.fit_transform(y_subset).toarray()
-print(y_encoded.shape)
 
 X_train, X_test, y_train, y_test = train_test_split(X_scaled, y_encoded, test_size=0.2, random_state=42)
 
-# Define your neural network structure
-network = Network()
-network.add(Layer(64, 64, 'sigmoid'))  # Hidden layer with 50 neurons
-network.add(Layer(64, 10, 'sigmoid'))  # Output layer with 10 neurons
+# Define your neural NeuralNetwork structure
+NeuralNetwork = NeuralNetwork()
+NeuralNetwork.add(Layer(64, 64, 'sigmoid'))  # Hidden layer with 50 neurons
+NeuralNetwork.add(Layer(64, 10, 'sigmoid'))  # Output layer with 10 neurons
 
-# Train the network
-network.fit(X_train, y_train, epochs=1000, learning_rate=0.01)
+# Train the NeuralNetwork
+NeuralNetwork.fit(X_train, y_train, epochs=10, learning_rate=0.01)
 
 # Predictions
-predictions = network.predict(X_test)
+predictions = NeuralNetwork.predict(X_test)
 
 # Convert predictions to class labels
 def convert_prob_to_class(probs):
     return np.argmax(probs, axis=1)
 
-predicted_classes = convert_prob_to_class(predictions)
 
 # Convert one-hot encoded test labels back to class labels
-actual_classes = np.argmax(y_test, axis=1)
-
-# Calculate accuracy
-accuracy = np.mean(predicted_classes == actual_classes)
+#actual_classes = np.argmax(y_test, axis=1)
+accuracy=NeuralNetwork.score(X_test,y_test)
 print("Accuracy:", accuracy)
-print("Predicted classes:", predicted_classes)
-print("Actual classes:", actual_classes)
+#print("Predicted classes:", predicted_classes)
+#print("Actual classes:", actual_classes)
```

### Comparing `mini_scikit_learn-0.1.5/mini_scikit_learn/test_ada.py` & `mini_scikit_learn-0.1.6/mini_scikit_learn/test_ada.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.5/mini_scikit_learn/test_cv.py` & `mini_scikit_learn-0.1.6/mini_scikit_learn/test_cv.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.5/mini_scikit_learn/test_dt.py` & `mini_scikit_learn-0.1.6/mini_scikit_learn/test_dt.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.5/mini_scikit_learn/test_dtr.py` & `mini_scikit_learn-0.1.6/mini_scikit_learn/test_dtr.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.5/mini_scikit_learn/test_knn.py` & `mini_scikit_learn-0.1.6/mini_scikit_learn/test_knn.py`

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

### Comparing `mini_scikit_learn-0.1.5/mini_scikit_learn/test_lg.py` & `mini_scikit_learn-0.1.6/mini_scikit_learn/test_lg.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.5/mini_scikit_learn/test_lgr.py` & `mini_scikit_learn-0.1.6/mini_scikit_learn/test_lgr.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.5/mini_scikit_learn/test_nb.py` & `mini_scikit_learn-0.1.6/mini_scikit_learn/test_nb.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.5/mini_scikit_learn/test_nn.py` & `mini_scikit_learn-0.1.6/mini_scikit_learn/test_nn.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.5/mini_scikit_learn/test_nn2.py` & `mini_scikit_learn-0.1.6/mini_scikit_learn/test_nn2.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.5/mini_scikit_learn/test_rf.py` & `mini_scikit_learn-0.1.6/mini_scikit_learn/test_rf.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.5/mini_scikit_learn/test_stacking.py` & `mini_scikit_learn-0.1.6/mini_scikit_learn/test_stacking.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.5/mini_scikit_learn/test_voting.py` & `mini_scikit_learn-0.1.6/mini_scikit_learn/test_voting.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.5/mini_scikit_learn/utils/NeuralNetwork.py` & `mini_scikit_learn-0.1.6/mini_scikit_learn/utils/NeuralNetwork.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.5/mini_scikit_learn.egg-info/PKG-INFO` & `mini_scikit_learn-0.1.6/mini_scikit_learn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mini-scikit-learn
-Version: 0.1.5
+Version: 0.1.6
 Summary: A brief description of your package
 Home-page: https://github.com/YASSIRFRI/mini_scikit_learn.git
 Author: Yassir Fri
 Author-email: your.email@example.com
 License: UNKNOWN
 Description: # mini_scikit_learn
```

### Comparing `mini_scikit_learn-0.1.5/mini_scikit_learn.egg-info/SOURCES.txt` & `mini_scikit_learn-0.1.6/mini_scikit_learn.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -8,32 +8,46 @@
 mini_scikit_learn/LogisticRegression.py
 mini_scikit_learn/ModelEnsembler.py
 mini_scikit_learn/NBClassifier.py
 mini_scikit_learn/NN.py
 mini_scikit_learn/Predictor.py
 mini_scikit_learn/RandomForest.py
 mini_scikit_learn/SVM.py
+mini_scikit_learn/__init__.py
 mini_scikit_learn/main.py
 mini_scikit_learn/test1.py
 mini_scikit_learn/test2.py
 mini_scikit_learn/test_ada.py
 mini_scikit_learn/test_cv.py
 mini_scikit_learn/test_dt.py
 mini_scikit_learn/test_dtr.py
 mini_scikit_learn/test_knn.py
 mini_scikit_learn/test_lg.py
 mini_scikit_learn/test_lgr.py
 mini_scikit_learn/test_nb.py
 mini_scikit_learn/test_nn.py
 mini_scikit_learn/test_nn2.py
+mini_scikit_learn/test_nn_digits.py
+mini_scikit_learn/test_nn_iris.py
 mini_scikit_learn/test_rf.py
 mini_scikit_learn/test_stacking.py
 mini_scikit_learn/test_voting.py
 mini_scikit_learn.egg-info/PKG-INFO
 mini_scikit_learn.egg-info/SOURCES.txt
 mini_scikit_learn.egg-info/dependency_links.txt
 mini_scikit_learn.egg-info/requires.txt
 mini_scikit_learn.egg-info/top_level.txt
+mini_scikit_learn/metrics/__init__.py
 mini_scikit_learn/metrics/metric.py
+mini_scikit_learn/model_selection/GridSearch.py
+mini_scikit_learn/model_selection/RandomSearch.py
+mini_scikit_learn/model_selection/__init__.py
+mini_scikit_learn/transformers/Encoders.py
+mini_scikit_learn/transformers/Imputers.py
+mini_scikit_learn/transformers/Transfomer.py
+mini_scikit_learn/transformers/__init__.py
+mini_scikit_learn/transformers/encoderTest.py
+mini_scikit_learn/utils/Kfolds.py
 mini_scikit_learn/utils/NeuralNetwork.py
+mini_scikit_learn/utils/__init__.py
 mini_scikit_learn/utils/cross_validation.py
 mini_scikit_learn/utils/train_test_split.py
```

### Comparing `mini_scikit_learn-0.1.5/setup.py` & `mini_scikit_learn-0.1.6/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mini_scikit_learn', 
-    version='0.1.5',
+    version='0.1.6',
     author='Yassir Fri',
     author_email='your.email@example.com',
     description='A brief description of your package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/YASSIRFRI/mini_scikit_learn.git",
     packages=find_packages(),
```

