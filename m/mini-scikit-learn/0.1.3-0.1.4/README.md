# Comparing `tmp/mini_scikit_learn-0.1.3.tar.gz` & `tmp/mini_scikit_learn-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mini_scikit_learn-0.1.3.tar", last modified: Sun Jun  2 22:20:17 2024, max compression
+gzip compressed data, was "mini_scikit_learn-0.1.4.tar", last modified: Sun Jun  2 23:18:21 2024, max compression
```

## Comparing `mini_scikit_learn-0.1.3.tar` & `mini_scikit_learn-0.1.4.tar`

### file list

```diff
@@ -1,60 +1,46 @@
-drwxrwxrwx   0        0        0        0 2024-06-02 22:20:17.168066 mini_scikit_learn-0.1.3/
--rw-rw-rw-   0        0        0     6155 2024-06-02 22:20:17.164481 mini_scikit_learn-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     4754 2024-06-02 22:00:40.000000 mini_scikit_learn-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-06-02 22:20:17.051660 mini_scikit_learn-0.1.3/mini_scikit_learn/
--rw-rw-rw-   0        0        0     2692 2024-05-22 21:00:24.000000 mini_scikit_learn-0.1.3/mini_scikit_learn/AdaBoost.py
--rw-rw-rw-   0        0        0     8408 2024-06-01 13:34:18.000000 mini_scikit_learn-0.1.3/mini_scikit_learn/DecisionTree.py
--rw-rw-rw-   0        0        0     1170 2024-06-02 22:19:48.000000 mini_scikit_learn-0.1.3/mini_scikit_learn/Estimator.py
--rw-rw-rw-   0        0        0     2220 2024-06-02 22:16:13.000000 mini_scikit_learn-0.1.3/mini_scikit_learn/KnnEstimator.py
--rw-rw-rw-   0        0        0    10995 2024-06-02 22:18:53.000000 mini_scikit_learn-0.1.3/mini_scikit_learn/LinearModel.py
--rw-rw-rw-   0        0        0     2688 2024-05-14 23:36:33.000000 mini_scikit_learn-0.1.3/mini_scikit_learn/LogisticRegression.py
--rw-rw-rw-   0        0        0     5094 2024-06-02 22:02:02.000000 mini_scikit_learn-0.1.3/mini_scikit_learn/ModelEnsembler.py
--rw-rw-rw-   0        0        0     2616 2024-05-14 18:06:27.000000 mini_scikit_learn-0.1.3/mini_scikit_learn/NBClassifier.py
--rw-rw-rw-   0        0        0     2291 2024-06-02 16:05:01.000000 mini_scikit_learn-0.1.3/mini_scikit_learn/NN.py
--rw-rw-rw-   0        0        0     1458 2024-06-02 22:19:40.000000 mini_scikit_learn-0.1.3/mini_scikit_learn/Predictor.py
--rw-rw-rw-   0        0        0     9950 2024-06-02 22:18:29.000000 mini_scikit_learn-0.1.3/mini_scikit_learn/RandomForest.py
--rw-rw-rw-   0        0        0     1076 2024-06-02 22:02:46.000000 mini_scikit_learn-0.1.3/mini_scikit_learn/SVM.py
--rw-rw-rw-   0        0        0      649 2024-06-02 19:45:21.000000 mini_scikit_learn-0.1.3/mini_scikit_learn/__init__.py
--rw-rw-rw-   0        0        0      819 2024-05-01 21:00:46.000000 mini_scikit_learn-0.1.3/mini_scikit_learn/main.py
-drwxrwxrwx   0        0        0        0 2024-06-02 22:20:17.129850 mini_scikit_learn-0.1.3/mini_scikit_learn/metrics/
--rw-rw-rw-   0        0        0      201 2024-06-02 21:58:01.000000 mini_scikit_learn-0.1.3/mini_scikit_learn/metrics/__init__.py
--rw-rw-rw-   0        0        0     1511 2024-05-14 17:21:27.000000 mini_scikit_learn-0.1.3/mini_scikit_learn/metrics/metric.py
-drwxrwxrwx   0        0        0        0 2024-06-02 22:20:17.137872 mini_scikit_learn-0.1.3/mini_scikit_learn/model_selection/
--rw-rw-rw-   0        0        0     2724 2024-06-02 18:52:51.000000 mini_scikit_learn-0.1.3/mini_scikit_learn/model_selection/GridSearch.py
--rw-rw-rw-   0        0        0     3325 2024-06-02 19:17:55.000000 mini_scikit_learn-0.1.3/mini_scikit_learn/model_selection/RandomSearch.py
--rw-rw-rw-   0        0        0       74 2024-06-02 18:58:49.000000 mini_scikit_learn-0.1.3/mini_scikit_learn/model_selection/__init__.py
--rw-rw-rw-   0        0        0     1768 2024-05-08 19:11:07.000000 mini_scikit_learn-0.1.3/mini_scikit_learn/test1.py
--rw-rw-rw-   0        0        0     1674 2024-06-02 16:42:36.000000 mini_scikit_learn-0.1.3/mini_scikit_learn/test2.py
--rw-rw-rw-   0        0        0      771 2024-05-22 19:35:27.000000 mini_scikit_learn-0.1.3/mini_scikit_learn/test_ada.py
--rw-rw-rw-   0        0        0      732 2024-05-22 18:05:25.000000 mini_scikit_learn-0.1.3/mini_scikit_learn/test_cv.py
--rw-rw-rw-   0        0        0     2024 2024-05-22 18:24:36.000000 mini_scikit_learn-0.1.3/mini_scikit_learn/test_dt.py
--rw-rw-rw-   0        0        0     1242 2024-05-14 16:27:56.000000 mini_scikit_learn-0.1.3/mini_scikit_learn/test_dtr.py
--rw-rw-rw-   0        0        0     1804 2024-06-02 19:38:30.000000 mini_scikit_learn-0.1.3/mini_scikit_learn/test_knn.py
--rw-rw-rw-   0        0        0     1197 2024-05-14 23:37:28.000000 mini_scikit_learn-0.1.3/mini_scikit_learn/test_lg.py
--rw-rw-rw-   0        0        0     2249 2024-05-15 08:54:45.000000 mini_scikit_learn-0.1.3/mini_scikit_learn/test_lgr.py
--rw-rw-rw-   0        0        0     3100 2024-05-05 19:11:00.000000 mini_scikit_learn-0.1.3/mini_scikit_learn/test_nb.py
--rw-rw-rw-   0        0        0     4047 2024-05-07 15:17:35.000000 mini_scikit_learn-0.1.3/mini_scikit_learn/test_nn.py
--rw-rw-rw-   0        0        0     1981 2024-05-07 15:29:08.000000 mini_scikit_learn-0.1.3/mini_scikit_learn/test_nn2.py
--rw-rw-rw-   0        0        0     3939 2024-05-14 17:29:42.000000 mini_scikit_learn-0.1.3/mini_scikit_learn/test_rf.py
--rw-rw-rw-   0        0        0     2046 2024-05-15 09:12:06.000000 mini_scikit_learn-0.1.3/mini_scikit_learn/test_stacking.py
--rw-rw-rw-   0        0        0     2364 2024-05-15 09:18:44.000000 mini_scikit_learn-0.1.3/mini_scikit_learn/test_voting.py
-drwxrwxrwx   0        0        0        0 2024-06-02 22:20:17.148929 mini_scikit_learn-0.1.3/mini_scikit_learn/transformers/
--rw-rw-rw-   0        0        0     2149 2024-06-02 13:09:30.000000 mini_scikit_learn-0.1.3/mini_scikit_learn/transformers/Encoders.py
--rw-rw-rw-   0        0        0     1550 2024-06-01 13:45:18.000000 mini_scikit_learn-0.1.3/mini_scikit_learn/transformers/Imputers.py
--rw-rw-rw-   0        0        0     1131 2024-06-02 16:44:55.000000 mini_scikit_learn-0.1.3/mini_scikit_learn/transformers/Transfomer.py
--rw-rw-rw-   0        0        0      229 2024-06-02 17:33:02.000000 mini_scikit_learn-0.1.3/mini_scikit_learn/transformers/__init__.py
--rw-rw-rw-   0        0        0      621 2024-05-14 08:53:30.000000 mini_scikit_learn-0.1.3/mini_scikit_learn/transformers/encoderTest.py
-drwxrwxrwx   0        0        0        0 2024-06-02 22:20:17.164481 mini_scikit_learn-0.1.3/mini_scikit_learn/utils/
--rw-rw-rw-   0        0        0     2670 2024-06-02 21:53:25.000000 mini_scikit_learn-0.1.3/mini_scikit_learn/utils/Kfolds.py
--rw-rw-rw-   0        0        0     5149 2024-05-08 08:28:46.000000 mini_scikit_learn-0.1.3/mini_scikit_learn/utils/NeuralNetwork.py
--rw-rw-rw-   0        0        0      126 2024-06-02 21:53:44.000000 mini_scikit_learn-0.1.3/mini_scikit_learn/utils/__init__.py
--rw-rw-rw-   0        0        0     1947 2024-06-02 13:52:22.000000 mini_scikit_learn-0.1.3/mini_scikit_learn/utils/cross_validation.py
--rw-rw-rw-   0        0        0     3146 2024-06-02 14:04:24.000000 mini_scikit_learn-0.1.3/mini_scikit_learn/utils/train_test_split.py
-drwxrwxrwx   0        0        0        0 2024-06-02 22:20:17.125344 mini_scikit_learn-0.1.3/mini_scikit_learn.egg-info/
--rw-rw-rw-   0        0        0     6155 2024-06-02 22:20:16.000000 mini_scikit_learn-0.1.3/mini_scikit_learn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1747 2024-06-02 22:20:16.000000 mini_scikit_learn-0.1.3/mini_scikit_learn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 22:20:16.000000 mini_scikit_learn-0.1.3/mini_scikit_learn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-06-02 22:20:16.000000 mini_scikit_learn-0.1.3/mini_scikit_learn.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-06-02 22:20:16.000000 mini_scikit_learn-0.1.3/mini_scikit_learn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-06-02 22:20:17.169699 mini_scikit_learn-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      787 2024-06-02 22:20:05.000000 mini_scikit_learn-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 23:18:21.987858 mini_scikit_learn-0.1.4/
+-rw-rw-rw-   0        0        0     6155 2024-06-02 23:18:21.985819 mini_scikit_learn-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4754 2024-06-02 22:00:40.000000 mini_scikit_learn-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-06-02 23:18:21.873468 mini_scikit_learn-0.1.4/mini_scikit_learn/
+-rw-rw-rw-   0        0        0     4984 2024-06-02 23:15:29.000000 mini_scikit_learn-0.1.4/mini_scikit_learn/AdaBoost.py
+-rw-rw-rw-   0        0        0    12707 2024-06-02 23:15:29.000000 mini_scikit_learn-0.1.4/mini_scikit_learn/DecisionTree.py
+-rw-rw-rw-   0        0        0     1865 2024-06-02 23:15:29.000000 mini_scikit_learn-0.1.4/mini_scikit_learn/Estimator.py
+-rw-rw-rw-   0        0        0     2265 2024-06-02 23:15:49.000000 mini_scikit_learn-0.1.4/mini_scikit_learn/KnnEstimator.py
+-rw-rw-rw-   0        0        0     9832 2024-06-02 23:15:29.000000 mini_scikit_learn-0.1.4/mini_scikit_learn/LinearModel.py
+-rw-rw-rw-   0        0        0     4952 2024-06-02 22:49:10.000000 mini_scikit_learn-0.1.4/mini_scikit_learn/LogisticRegression.py
+-rw-rw-rw-   0        0        0     8572 2024-06-02 23:15:29.000000 mini_scikit_learn-0.1.4/mini_scikit_learn/ModelEnsembler.py
+-rw-rw-rw-   0        0        0     3817 2024-06-02 22:49:10.000000 mini_scikit_learn-0.1.4/mini_scikit_learn/NBClassifier.py
+-rw-rw-rw-   0        0        0     5092 2024-06-02 23:15:29.000000 mini_scikit_learn-0.1.4/mini_scikit_learn/NN.py
+-rw-rw-rw-   0        0        0     1679 2024-06-02 23:15:57.000000 mini_scikit_learn-0.1.4/mini_scikit_learn/Predictor.py
+-rw-rw-rw-   0        0        0    10782 2024-06-02 23:15:29.000000 mini_scikit_learn-0.1.4/mini_scikit_learn/RandomForest.py
+-rw-rw-rw-   0        0        0     1542 2024-06-02 23:16:32.000000 mini_scikit_learn-0.1.4/mini_scikit_learn/SVM.py
+-rw-rw-rw-   0        0        0      819 2024-05-01 21:00:46.000000 mini_scikit_learn-0.1.4/mini_scikit_learn/main.py
+drwxrwxrwx   0        0        0        0 2024-06-02 23:18:21.923771 mini_scikit_learn-0.1.4/mini_scikit_learn/metrics/
+-rw-rw-rw-   0        0        0     4575 2024-06-02 22:49:10.000000 mini_scikit_learn-0.1.4/mini_scikit_learn/metrics/metric.py
+-rw-rw-rw-   0        0        0     1768 2024-05-08 19:11:07.000000 mini_scikit_learn-0.1.4/mini_scikit_learn/test1.py
+-rw-rw-rw-   0        0        0     1735 2024-06-02 23:15:29.000000 mini_scikit_learn-0.1.4/mini_scikit_learn/test2.py
+-rw-rw-rw-   0        0        0      771 2024-05-22 19:35:27.000000 mini_scikit_learn-0.1.4/mini_scikit_learn/test_ada.py
+-rw-rw-rw-   0        0        0      732 2024-05-22 18:05:25.000000 mini_scikit_learn-0.1.4/mini_scikit_learn/test_cv.py
+-rw-rw-rw-   0        0        0     2024 2024-05-22 18:24:36.000000 mini_scikit_learn-0.1.4/mini_scikit_learn/test_dt.py
+-rw-rw-rw-   0        0        0     1242 2024-05-14 16:27:56.000000 mini_scikit_learn-0.1.4/mini_scikit_learn/test_dtr.py
+-rw-rw-rw-   0        0        0     1805 2024-06-02 23:15:29.000000 mini_scikit_learn-0.1.4/mini_scikit_learn/test_knn.py
+-rw-rw-rw-   0        0        0     1197 2024-05-14 23:37:28.000000 mini_scikit_learn-0.1.4/mini_scikit_learn/test_lg.py
+-rw-rw-rw-   0        0        0     2249 2024-05-15 08:54:45.000000 mini_scikit_learn-0.1.4/mini_scikit_learn/test_lgr.py
+-rw-rw-rw-   0        0        0     3100 2024-05-05 19:11:00.000000 mini_scikit_learn-0.1.4/mini_scikit_learn/test_nb.py
+-rw-rw-rw-   0        0        0     4047 2024-05-07 15:17:35.000000 mini_scikit_learn-0.1.4/mini_scikit_learn/test_nn.py
+-rw-rw-rw-   0        0        0     1981 2024-05-07 15:29:08.000000 mini_scikit_learn-0.1.4/mini_scikit_learn/test_nn2.py
+-rw-rw-rw-   0        0        0     3939 2024-05-14 17:29:42.000000 mini_scikit_learn-0.1.4/mini_scikit_learn/test_rf.py
+-rw-rw-rw-   0        0        0     2046 2024-05-15 09:12:06.000000 mini_scikit_learn-0.1.4/mini_scikit_learn/test_stacking.py
+-rw-rw-rw-   0        0        0     2364 2024-05-15 09:18:44.000000 mini_scikit_learn-0.1.4/mini_scikit_learn/test_voting.py
+drwxrwxrwx   0        0        0        0 2024-06-02 23:18:21.944188 mini_scikit_learn-0.1.4/mini_scikit_learn/utils/
+-rw-rw-rw-   0        0        0     5149 2024-05-08 08:28:46.000000 mini_scikit_learn-0.1.4/mini_scikit_learn/utils/NeuralNetwork.py
+-rw-rw-rw-   0        0        0     1380 2024-06-02 23:15:29.000000 mini_scikit_learn-0.1.4/mini_scikit_learn/utils/cross_validation.py
+-rw-rw-rw-   0        0        0     1769 2024-06-02 23:15:29.000000 mini_scikit_learn-0.1.4/mini_scikit_learn/utils/train_test_split.py
+drwxrwxrwx   0        0        0        0 2024-06-02 23:18:21.913461 mini_scikit_learn-0.1.4/mini_scikit_learn.egg-info/
+-rw-rw-rw-   0        0        0     6155 2024-06-02 23:18:21.000000 mini_scikit_learn-0.1.4/mini_scikit_learn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1245 2024-06-02 23:18:21.000000 mini_scikit_learn-0.1.4/mini_scikit_learn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 23:18:21.000000 mini_scikit_learn-0.1.4/mini_scikit_learn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-06-02 23:18:21.000000 mini_scikit_learn-0.1.4/mini_scikit_learn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 23:18:21.000000 mini_scikit_learn-0.1.4/mini_scikit_learn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-02 23:18:21.987858 mini_scikit_learn-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      787 2024-06-02 23:16:50.000000 mini_scikit_learn-0.1.4/setup.py
```

### Comparing `mini_scikit_learn-0.1.3/PKG-INFO` & `mini_scikit_learn-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mini_scikit_learn
-Version: 0.1.3
+Version: 0.1.4
 Summary: A brief description of your package
 Home-page: https://github.com/YASSIRFRI/mini_scikit_learn.git
 Author: Yassir Fri
 Author-email: your.email@example.com
 License: UNKNOWN
 Description: # mini_scikit_learn
```

### Comparing `mini_scikit_learn-0.1.3/README.md` & `mini_scikit_learn-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.3/mini_scikit_learn/DecisionTree.py` & `mini_scikit_learn-0.1.4/mini_scikit_learn/LinearModel.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,230 +1,343 @@
 import numpy as np
-from .Estimator import Estimator
-from .Predictor import Predictor
-
-
-class DecisionTreeClassifier(Predictor, Estimator):
+import Predictor
+import Estimator
+from numpy import log, dot, exp, shape
+import matplotlib.pyplot as plt
+from sklearn.datasets import make_classification
+from sklearn.model_selection import train_test_split
+
+class LinearModel(Predictor.Predictor, Estimator.Estimator):
+    """
+    A linear model for regression or classification.
+
+    Parameters:
+    -----------
+    fit_intercept : bool, optional (default=True)
+        Whether to fit an intercept term in the model.
+
+    Attributes:
+    -----------
+    fit_intercept : bool
+        Whether to fit an intercept term in the model.
+    beta : numpy.ndarray or None
+        The coefficients of the linear model.
+    is_fitted : bool
+        Indicates whether the model has been fitted.
+    """
     
-    def __init__(self, max_depth=1000):
-        """This is the constructor of the class.
-        Parameters:
-        max_depth (int): The maximum depth of the tree.
-        """
-        self.max_depth = max_depth
-        self.tree = None
+    def __init__(self, fit_intercept=True):
+        """Initialize the linear model."""
+        self.fit_intercept = fit_intercept
+        self.beta = None
         self.is_fitted = False
-        super().__init__(self)
     
     def fit(self, X, y):
-        self.tree = self._build_tree(X, y, depth=0)
+        """
+        Train the model on the training data.
+
+        Parameters:
+        -----------
+        X : numpy.ndarray
+            The training data.
+        y : numpy.ndarray
+            The target values.
+
+        Returns:
+        --------
+        self : object
+            The trained model.
+        """
         self.is_fitted = True
+        if self.fit_intercept:
+            X = np.hstack((np.ones((X.shape[0], 1)), X))
+        self.beta = np.linalg.inv(X.T @ X) @ X.T @ y
         return self
-
+    
     def get_params(self):
-        return {"max_depth": self.max_depth}
+        """
+        Get the parameters of the model.
 
+        Returns:
+        --------
+        params : dict
+            The parameters of the model.
+        """
+        return {"fit_intercept": self.fit_intercept}
+    
     def predict(self, X):
+        """
+        Make predictions on the test data.
+        """
         if not self.is_fitted:
             raise ValueError("The model has not been fitted yet.")
-        return np.array([self._predict_tree(x, self.tree) for x in X])
+        if self.fit_intercept:
+            X = np.hstack((np.ones((X.shape[0], 1)), X))
+        return X @ self.beta
+
+class LinearRegression(LinearModel):
+    """
+    A linear regression model.
+
+    Parameters:
+    -----------
+    fit_intercept : bool, optional (default=True)
+        Whether to fit an intercept term in the model.
+    """
+    
+    def __init__(self, fit_intercept=True):
+        """Initialize the linear regression model."""
+        super().__init__(fit_intercept)
     
     def score(self, X, y):
-        """This method is used to evaluate the model on the test data."""
         y_pred = self.predict(X)
-        return np.mean(y == y_pred)
-
-    def _build_tree(self, X, y, depth):
-        # Check termination conditions
-        if depth >= self.max_depth or len(np.unique(y)) == 1:
-            return np.argmax(np.bincount(y))  # Return the majority class index
-
-        # Find the best split
-        best_split = self._find_best_split(X, y)
-
-        if best_split is None:
-            return np.argmax(np.bincount(y))  # Return the majority class index if no split found
-
-        feature_index, threshold = best_split
-
-        # Split the data
-        left_indices = X[:, feature_index] < threshold
-        X_left, y_left = X[left_indices], y[left_indices]
-        X_right, y_right = X[~left_indices], y[~left_indices]
-
-        # Recursively build subtrees
-        left_subtree = self._build_tree(X_left, y_left, depth + 1)
-        right_subtree = self._build_tree(X_right, y_right, depth + 1)
-
-        return (feature_index, threshold, left_subtree, right_subtree)
-
-    def _find_best_split(self, X, y):
-        best_entropy_gain = float('-inf')
-        best_split = None
-        n_features = X.shape[1]
-        parent_entropy = self._entropy(y)
-
-        for feature_index in range(n_features):
-            thresholds = np.unique(X[:, feature_index])
-            for threshold in thresholds:
-                left_indices = X[:, feature_index] < threshold
-                left_labels = y[left_indices]
-                right_labels = y[~left_indices]
-
-                if len(left_labels) == 0 or len(right_labels) == 0:
-                    continue  # Skip if one of the child nodes is empty
-
-                # Calculate entropy for the child nodes
-                entropy_left = self._entropy(left_labels)
-                entropy_right = self._entropy(right_labels)
-
-                # Calculate weighted average entropy
-                weight_left = len(left_labels) / len(y)
-                weight_right = len(right_labels) / len(y)
-                weighted_avg_entropy = weight_left * entropy_left + weight_right * entropy_right
-
-                # Calculate entropy gain
-                entropy_gain = parent_entropy - weighted_avg_entropy
-
-                if entropy_gain > best_entropy_gain:
-                    best_entropy_gain = entropy_gain
-                    best_split = (feature_index, threshold)
-
-        return best_split
-
-    def _entropy(self, labels):
-        class_probabilities = [len(labels[labels == c]) / len(labels) for c in np.unique(labels)]
-        entropy = -np.sum(p * np.log2(p) for p in class_probabilities if p > 0)
-        return entropy
-
-    def _gini_impurity(self, left_labels, right_labels):
-        total_samples = len(left_labels) + len(right_labels)
-        p_left = len(left_labels) / total_samples
-        p_right = len(right_labels) / total_samples
-        gini_left = 1 - sum((np.mean(left_labels == c) ** 2 for c in set(left_labels)))
-        gini_right = 1 - sum((np.mean(right_labels == c) ** 2 for c in set(right_labels)))
+        return 1 - np.sum((y - y_pred) ** 2) / np.sum((y - np.mean(y)) ** 2)
+    
+    def get_params(self):
+        return super().get_params()
+    
+    def set_params(self, **params):
+        """This method is used to set the parameters of the model.
+        Parameters:
+        **params: The parameters of the model.
+        """
+        self.model.fit_intercept = params["fit_intercept"]
+        return self
 
-        gini_impurity = p_left * gini_left + p_right * gini_right
-        return gini_impurity
+class LogisticRegression:
+    """
+    Logistic Regression Classifier.
+
+    Parameters:
+    -----------
+    max_iter : int, optional (default=10000)
+        Maximum number of iterations for the optimization loop.
+    thres : float, optional (default=1e-3)
+        Threshold for the optimization convergence.
+
+    Attributes:
+    -----------
+    max_iter : int
+        Maximum number of iterations for the optimization loop.
+    thres : float
+        Threshold for the optimization convergence.
+    weights : numpy.ndarray or None
+        The weights of the logistic regression model.
+    classes : numpy.ndarray
+        The unique class labels.
+    class_labels : dict
+        Dictionary mapping class labels to indices.
+    loss : list
+        List to store the loss values during training.
+    """
+    
+    def __init__(self, max_iter=10000, thres=1e-3):
+        self.max_iter = max_iter
+        self.thres = thres
+    
+    def fit(self, X, y, batch_size=64, lr=0.001, rand_seed=4, verbose=False): 
+        """
+        Fit the logistic regression model to the training set.
 
-    def _predict_tree(self, x, tree):
-        if isinstance(tree, np.int64):  
-            return tree
-        else:  
-            feature_index, threshold, left_subtree, right_subtree = tree
-            if x[feature_index] < threshold:
-                return self._predict_tree(x, left_subtree)
-            else:
-                return self._predict_tree(x, right_subtree)
-            
+        Parameters:
+        -----------
+        X : numpy.ndarray
+            Training data.
+        y : numpy.ndarray
+            Training labels.
+        batch_size : int, optional (default=64)
+            Batch size for training.
+        lr : float, optional (default=0.001)
+            Learning rate for gradient descent.
+        rand_seed : int, optional (default=4)
+            Random seed for reproducibility.
+        verbose : bool, optional (default=False)
+            Whether to print training progress.
+
+        Returns:
+        --------
+        self : object
+            Fitted logistic regression model.
+        """
+        np.random.seed(rand_seed) 
+        self.classes = np.unique(y)
+        self.class_labels = {c: i for i, c in enumerate(self.classes)}
+        X = self.add_bias(X)
+        y = self.one_hot(y)
+        self.loss = []
+        self.weights = np.zeros(shape=(len(self.classes), X.shape[1]))
+        self.fit_data(X, y, batch_size, lr, verbose)
+        return self
 
+    def fit_data(self, X, y, batch_size, lr, verbose):
+        """
+        Train the logistic regression model using batch gradient descent.
 
+        Parameters:
+        -----------
+        X : numpy.ndarray
+            Training data.
+        y : numpy.ndarray
+            Training labels.
+        batch_size : int
+            Batch size for training.
+        lr : float
+            Learning rate for gradient descent.
+        verbose : bool
+            Whether to print training progress.
+        """
+        i = 0
+        while (not self.max_iter or i < self.max_iter):
+            self.loss.append(self.cross_entropy(y, self.predict_(X)))
+            idx = np.random.choice(X.shape[0], batch_size)
+            X_batch, y_batch = X[idx], y[idx]
+            error = y_batch - self.predict_(X_batch)
+            update = (lr * np.dot(error.T, X_batch))
+            self.weights += update
+            if np.abs(update).max() < self.thres:
+                break
+            if i % 1000 == 0 and verbose: 
+                print(f'Training Accuracy at {i} iterations is {self.evaluate_(X, y)}')
+            i += 1
+    
+    def predict_probs(self, X):
+        """
+        Predict probabilities for given data using the logistic regression model.
 
+        Parameters:
+        -----------
+        X : numpy.ndarray
+            Data to predict.
+
+        Returns:
+        --------
+        probs : numpy.ndarray
+            Predicted probabilities.
+        """
+        return self.predict_(self.add_bias(X))
+    
+    def predict_(self, X):
+        """Predict probabilities for given data.
+        """
+        pre_vals = np.dot(X, self.weights.T).reshape(-1, len(self.classes))
+        return self.softmax(pre_vals)
+    
+    def softmax(self, z):
+        """
+        Compute the softmax of a set of values..
+        """
+        return np.exp(z) / np.sum(np.exp(z), axis=1).reshape(-1, 1)
 
+    def predict(self, X):
+        """
+        Predict class labels for given data.
+        """
+        self.probs_ = self.predict_probs(X)
+        return np.vectorize(lambda c: self.classes[c])(np.argmax(self.probs_, axis=1))
+  
+    def add_bias(self, X):
+        """
+        Add bias term to the data.
 
+        Parameters:
+        -----------
+        X : numpy.ndarray
+            Data to add bias term.
+
+        Returns:
+        --------
+        X_with_bias : numpy.ndarray
+            Data with bias term added.
+        """
+        return np.insert(X, 0, 1, axis=1)
+  
+    def get_random_weights(self, row, col):
+        """
+        Get random weights for initialization.
 
+        Parameters:
+        -----------
+        row : int
+            Number of rows.
+        col : int
+            Number of columns.
+
+        Returns:
+        --------
+        weights : numpy.ndarray
+            Random weights.
+        """
+        return np.zeros(shape=(row, col))
 
+    def one_hot(self, y):
+        """
+        Convert class labels to one-hot encoding.
 
+        Parameters:
+        -----------
+        y : numpy.ndarray
+            Class labels.
+
+        Returns:
+        --------
+        y_one_hot : numpy.ndarray
+            One-hot encoded labels.
+        """
+        return np.eye(len(self.classes))[np.vectorize(lambda c: self.class_labels[c])(y).reshape(-1)]
+    
+    def score(self, X, y):
+        """
+        Compute the accuracy of the model.
 
-class DecisionTreeRegressor(Predictor, Estimator):
+        Parameters:
+        -----------
+        X : numpy.ndarray
+            Test data.
+        y : numpy.ndarray
+            True labels.
+
+        Returns:
+        --------
+        accuracy : float
+            Accuracy of the model.
+        """
+        return np.mean(self.predict(X) == y)
     
-    def __init__(self, max_depth=1000):
-        """This is the constructor of the class.
+    def evaluate_(self, X, y):
+        """
+        Evaluate the model during training.
+
         Parameters:
-        max_depth (int): The maximum depth of the tree.
+        -----------
+        X : numpy.ndarray
+            Training data.
+        y : numpy.ndarray
+            Training labels.
+
+        Returns:
+        --------
+        accuracy : float
+            Accuracy of the model.
         """
-        self.max_depth = max_depth
-        self.tree = None
-        self.is_fitted = False
-        super().__init__(self)
+        return np.mean(np.argmax(self.predict_(X), axis=1) == np.argmax(y, axis=1))
     
-    def fit(self, X, y):
-        self.tree = self._build_tree(X, y, depth=0)
-        self.is_fitted = True
-        return self
+    def cross_entropy(self, y, probs):
+        """
+        Compute the cross-entropy loss.
 
-    def get_params(self):
-        return {"max_depth": self.max_depth}
+        Parameters:
+        -----------
+        y : numpy.ndarray
+            True labels.
+        probs : numpy.ndarray
+            Predicted probabilities.
+
+        Returns:
+        --------
+        loss : float
+            Cross-entropy loss.
+        """
+        return -1 * np.mean(y * np.log(probs))
 
-    def predict(self, X):
-        if not self.is_fitted:
-            raise ValueError("The model has not been fitted yet.")
-        return np.array([self._predict_tree(x, self.tree) for x in X])
     
     def score(self, X, y):
-        """This method is used to evaluate the model on the test data."""
-        y_pred = self.predict(X)
-        return np.mean((y - y_pred) ** 2)  # Mean Squared Error
-
-    def _build_tree(self, X, y, depth):
-        # Check termination conditions
-        if depth >= self.max_depth or len(y) <= 1:
-            return np.mean(y)  # Return the mean value of y
-
-        # Find the best split
-        best_split = self._find_best_split(X, y)
-
-        if best_split is None:
-            return np.mean(y)  # Return the mean value of y if no split found
-
-        feature_index, threshold = best_split
-
-        # Split the data
-        left_indices = X[:, feature_index] < threshold
-        X_left, y_left = X[left_indices], y[left_indices]
-        X_right, y_right = X[~left_indices], y[~left_indices]
-
-        # Recursively build subtrees
-        left_subtree = self._build_tree(X_left, y_left, depth + 1)
-        right_subtree = self._build_tree(X_right, y_right, depth + 1)
-
-        return (feature_index, threshold, left_subtree, right_subtree)
-
-    def _find_best_split(self, X, y):
-        best_mse_gain = float('-inf')
-        best_split = None
-        n_features = X.shape[1]
-        parent_mse = self._mean_squared_error(y)
-
-        for feature_index in range(n_features):
-            thresholds = np.unique(X[:, feature_index])
-            for threshold in thresholds:
-                left_indices = X[:, feature_index] < threshold
-                left_labels = y[left_indices]
-                right_labels = y[~left_indices]
-
-                if len(left_labels) == 0 or len(right_labels) == 0:
-                    continue  # Skip if one of the child nodes is empty
-
-                # Calculate mean squared error for the child nodes
-                mse_left = self._mean_squared_error(left_labels)
-                mse_right = self._mean_squared_error(right_labels)
-
-                # Calculate weighted average mean squared error
-                weight_left = len(left_labels) / len(y)
-                weight_right = len(right_labels) / len(y)
-                weighted_avg_mse = weight_left * mse_left + weight_right * mse_right
-
-                # Calculate mse gain
-                mse_gain = parent_mse - weighted_avg_mse
-
-                if mse_gain > best_mse_gain:
-                    best_mse_gain = mse_gain
-                    best_split = (feature_index, threshold)
-
-        return best_split
-
-    def _mean_squared_error(self, labels):
-        mean = np.mean(labels)
-        mse = np.mean((labels - mean) ** 2)
-        return mse
-
-    def _predict_tree(self, x, tree):
-        if isinstance(tree, float):  # Leaf node
-            return tree
-        else:  # Decision node
-            feature_index, threshold, left_subtree, right_subtree = tree
-            if x[feature_index] < threshold:
-                return self._predict_tree(x, left_subtree)
-            else:
-                return self._predict_tree(x, right_subtree)
-
+        return np.mean(self.predict(X) == y)
```

### Comparing `mini_scikit_learn-0.1.3/mini_scikit_learn/Estimator.py` & `mini_scikit_learn-0.1.4/mini_scikit_learn/Estimator.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,72 @@
+class Estimator:
+    """
+    Base class for all estimators in the package. It provides the basic structure for all estimators.
 
-
-class Estimator: 
-    """This is the base class for all estimators in the package. It provides the basic structure for all estimators.
+    Methods:
+    --------
+    fit(X, y=None)
+        Train the model on the training data.
+    get_params()
+        Get the parameters of the model.
+    set_params(**params)
+        Set the parameters of the model.
     """
     
     def __init__(self):
-        """This is the constructor of the class.
+        """
+        Initialize the estimator.
         """
         pass
     
     def fit(self, X, y=None):
-        """This method is used to train the model on the training data.
+        """
+        Train the model on the training data.
         Parameters:
-        X (numpy.ndarray): The training data.
-        y (numpy.ndarray): The target values.
+        -----------
+        X : numpy.ndarray
+            The training data.
+        y : numpy.ndarray, optional
+            The target values. Default is None.
+
         Returns:
-        self: The trained model.
+        --------
+        self : object
+            The trained model.
+
+        Raises:
+        -------
+        NotImplementedError
+            If the method is not implemented.
         """
         raise NotImplementedError("The fit method is not implemented.")
     
     def get_params(self):
-        """This method is used to get the parameters of the model.
+        """
+        Get the parameters of the model.
         Returns:
-        dict: The parameters of the model.
+        --------
+        params : dict
+            The parameters of the model.
+
+        Raises:
+        -------
+        NotImplementedError
+            If the method is not implemented.
         """
         raise NotImplementedError("The get_params method is not implemented.")
     
     def set_params(self, **params):
-        """This method is used to set the parameters of the model.
+        """
+        Set the parameters of the model.
         Parameters:
-        **params: The parameters of the model.
+        -----------
+        **params : dict
+            The parameters of the model.
+        Raises:
+        -------
+        NotImplementedError
+            If the method is not implemented.
         """
-        for param, value in params.items():
-            setattr(self, param, value)
+        raise NotImplementedError("The set_params method is not implemented.")
     
-        
+
```

### Comparing `mini_scikit_learn-0.1.3/mini_scikit_learn/Predictor.py` & `mini_scikit_learn-0.1.4/mini_scikit_learn/Predictor.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,47 +1,67 @@
-from .Estimator import Estimator
-class Predictor(Estimator):
+import Estimator
+
+class Predictor(Estimator.Estimator):
     
     def __init__(self, model=None):
-        """This is the constructor of the class.
-        Parameters:
-        model: The model to be used for prediction.
-        """
+        """Initialize the Predictor with a given model."""
         self.model = model
         
     def predict(self, X):
-        """This method is used to make predictions on the test data.
+        """
+        Make predictions on the test data.
         Parameters:
-        X (numpy.ndarray): The test data.
+        -----------
+        X : numpy.ndarray
+            The test data.
         Returns:
-        numpy.ndarray: The predictions.
+        --------
+        numpy.ndarray
+            The predictions.
         """
         return self.model.predict(X)
     
-    
     def score(self, X, y):
-        """This method is used to evaluate the model on the test data.
+        """
+        Evaluate the model on the test data.
         Parameters:
-        X (numpy.ndarray): The test data.
-        y (numpy.ndarray): The target values.
+        -----------
+        X : numpy.ndarray
+            The test data.
+        y : numpy.ndarray
+            The target values.
+
         Returns:
-        float: The score of the model.
+        --------
+        float
+            The score of the model.
+        Raises:
+        -------
+        NotImplementedError
+            If the score method has not been implemented.
         """
         raise NotImplementedError("The score method has not been implemented.")
     
     def fit_predict(self, X_train, y_train, X_test):
-        """This method is used to train the model on the training data and make predictions on the test data.
+        """
+        Train the model on the training data and make predictions on the test data.
         Parameters:
-        X_train (numpy.ndarray): The training data.
-        y_train (numpy.ndarray): The target values.
-        X_test (numpy.ndarray): The test data.
+        -----------
+        X_train : numpy.ndarray
+            The training data.
+        y_train : numpy.ndarray
+            The target values.
+        X_test : numpy.ndarray
+            The test data.
+
         Returns:
-        numpy.ndarray: The predictions.
+        --------
+        numpy.ndarray
+            The predictions.
         """
         self.model.fit(X_train, y_train)
         return self.predict(X_test)
     
     
     
     
     
-
```

### Comparing `mini_scikit_learn-0.1.3/mini_scikit_learn/RandomForest.py` & `mini_scikit_learn-0.1.4/mini_scikit_learn/RandomForest.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,55 +1,75 @@
 import numpy as np
-from . import Estimator
-from . import Predictor
-from .DecisionTree import DecisionTreeClassifier, DecisionTreeRegressor
+import Estimator
+import Predictor
+from DecisionTree import DecisionTreeClassifier, DecisionTreeRegressor
 from sklearn.utils import resample
 
 class RandomForestClassifier(Predictor.Predictor, Estimator.Estimator):
-    
+    """
+    Random Forest Classifier.
+
+    Parameters:
+    -----------
+    n_estimators : int, optional (default=100)
+        The number of trees in the forest.
+    max_depth : int, optional (default=1000)
+        The maximum depth of the trees.
+    max_features : str or int, optional (default='sqrt')
+        The number of features to consider when looking for the best split:
+        - If int, then consider `max_features` features at each split.
+        - If 'sqrt', then consider `sqrt(n_features)` features at each split.
+        - If 'log2', then consider `log2(n_features)` features at each split.
+
+    Attributes:
+    -----------
+    n_estimators : int
+        The number of trees in the forest.
+    max_depth : int
+        The maximum depth of the trees.
+    max_features : str or int
+        The number of features to consider when looking for the best split.
+    trees : list
+        List of decision trees in the forest.
+    is_fitted : bool
+        Indicates whether the model has been fitted.
+    """
+
     def __init__(self, n_estimators=100, max_depth=1000, max_features='sqrt'):
-        """Random Forest Classifier.
-        
-        Parameters:
-        n_estimators (int): The number of trees in the forest.
-        max_depth (int): The maximum depth of the trees.
-        max_features (str or int): The number of features to consider when looking for the best split:
-            - If int, then consider `max_features` features at each split.
-            - If 'sqrt', then consider `sqrt(n_features)` features at each split.
-            - If 'log2', then consider `log2(n_features)` features at each split.
-        """
+        """Initialize the Random Forest Classifier."""
         self.n_estimators = n_estimators
         self.max_depth = max_depth
         self.max_features = max_features
         self.trees = []
         self.is_fitted = False
         super().__init__(self)
 
     def fit(self, X, y):
-        """Fit the random forest model.
-        
+        """
+        Fit the random forest model.
+
         Parameters:
-        X (np.ndarray): Training data.
-        y (np.ndarray): Training labels.
+        -----------
+        X : np.ndarray
+            Training data.
+        y : np.ndarray
+            Training labels.
         """
         self.trees = []
         n_samples, n_features = X.shape
         
         if self.max_features == 'sqrt':
             max_features = int(np.sqrt(n_features))
         elif self.max_features == 'log2':
             max_features = int(np.log2(n_features))
         else:
             max_features = self.max_features
         
         for _ in range(self.n_estimators):
-            # Bootstrap sample
             X_sample, y_sample = resample(X, y)
-            
-            # Create and train a decision tree
             tree = DecisionTreeClassifier(max_depth=self.max_depth)
             tree._find_best_split = self._get_find_best_split(max_features)
             tree.fit(X_sample, y_sample)
             self.trees.append(tree)
         
         self.is_fitted = True
         return self
@@ -68,23 +88,26 @@
                 thresholds = np.unique(X[:, feature_index])
                 for threshold in thresholds:
                     left_indices = X[:, feature_index] < threshold
                     left_labels = y[left_indices]
                     right_labels = y[~left_indices]
                     
                     if len(left_labels) == 0 or len(right_labels) == 0:
-                        continue  # Skip if one of the child nodes is empty
+                        continue
                     
+                    # Calculate entropy for the child nodes
                     entropy_left = self._entropy(left_labels)
                     entropy_right = self._entropy(right_labels)
                     
+                    # Calculate weighted average entropy
                     weight_left = len(left_labels) / len(y)
                     weight_right = len(right_labels) / len(y)
                     weighted_avg_entropy = weight_left * entropy_left + weight_right * entropy_right
                     
+                    # Calculate entropy gain
                     entropy_gain = parent_entropy - weighted_avg_entropy
                     
                     if entropy_gain > best_entropy_gain:
                         best_entropy_gain = entropy_gain
                         best_split = (feature_index, threshold)
             
             return best_split
@@ -94,91 +117,114 @@
     def _entropy(self, labels):
         """Calculate the entropy of a set of labels."""
         class_probabilities = [len(labels[labels == c]) / len(labels) for c in np.unique(labels)]
         entropy = -np.sum(p * np.log2(p) for p in class_probabilities if p > 0)
         return entropy
 
     def predict(self, X):
-        """Predict class for X.
-        
+        """
+        Predict class for X.
+
         Parameters:
-        X (np.ndarray): Test data.
-        
+        -----------
+        X : np.ndarray
+            Test data.
+
         Returns:
-        np.ndarray: Predicted classes.
+        --------
+        np.ndarray
+            Predicted classes.
         """
         if not self.is_fitted:
             raise ValueError("The model has not been fitted yet.")
         
         tree_predictions = np.array([tree.predict(X) for tree in self.trees])
-        # Majority vote
         majority_vote = np.apply_along_axis(lambda x: np.bincount(x).argmax(), axis=0, arr=tree_predictions)
         return majority_vote
     
     def score(self, X, y):
-        """Evaluate the model on the test data.
-        
+        """
+        Evaluate the model on the test data.
+
         Parameters:
-        X (np.ndarray): Test data.
-        y (np.ndarray): True labels.
-        
+        -----------
+        X : np.ndarray
+            Test data.
+        y : np.ndarray
+            True labels.
+
         Returns:
-        float: Accuracy score.
+        --------
+        float
+            Accuracy score.
         """
         y_pred = self.predict(X)
         return np.mean(y == y_pred)
 
+class RandomForestRegressor:
+    """
+    Random Forest Regressor.
 
+    Parameters:
+    -----------
+    n_estimators : int, optional (default=100)
+        The number of trees in the forest.
+    max_depth : int, optional (default=1000)
+        The maximum depth of the trees.
+    max_features : str or int, optional (default='sqrt')
+        The number of features to consider when looking for the best split:
+        - If int, then consider `max_features` features at each split.
+        - If 'sqrt', then consider `sqrt(n_features)` features at each split.
+        - If 'log2', then consider `log2(n_features)` features at each split.
+
+    Attributes:
+    -----------
+    n_estimators : int
+        The number of trees in the forest.
+    max_depth : int
+        The maximum depth of the trees.
+    max_features : str or int
+        The number of features to consider when looking for the best split.
+    trees : list
+        List of decision trees in the forest.
+    is_fitted : bool
+        Indicates whether the model has been fitted.
+    """
 
-
-
-
-from sklearn.utils import resample
-
-class RandomForestRegressor:
-    
     def __init__(self, n_estimators=100, max_depth=1000, max_features='sqrt'):
-        """Random Forest Regressor.
-        
-        Parameters:
-        n_estimators (int): The number of trees in the forest.
-        max_depth (int): The maximum depth of the trees.
-        max_features (str or int): The number of features to consider when looking for the best split:
-            - If int, then consider `max_features` features at each split.
-            - If 'sqrt', then consider `sqrt(n_features)` features at each split.
-            - If 'log2', then consider `log2(n_features)` features at each split.
-        """
+        """Initialize the Random Forest Regressor."""
         self.n_estimators = n_estimators
         self.max_depth = max_depth
         self.max_features = max_features
         self.trees = []
         self.is_fitted = False
 
     def fit(self, X, y):
-        """Fit the random forest model.
-        
+        """
+        Fit the random forest model.
+
         Parameters:
-        X (np.ndarray): Training data.
-        y (np.ndarray): Training labels.
+        -----------
+        X : np.ndarray
+            Training data.
+        y : np.ndarray
+            Training labels.
         """
         self.trees = []
         n_samples, n_features = X.shape
         
         if self.max_features == 'sqrt':
             max_features = int(np.sqrt(n_features))
         elif self.max_features == 'log2':
             max_features = int(np.log2(n_features))
         else:
             max_features = self.max_features
         
         for _ in range(self.n_estimators):
-            # Bootstrap sample
             X_sample, y_sample = resample(X, y)
-            
-            # Create and train a decision tree
             tree = DecisionTreeRegressor(max_depth=self.max_depth)
             tree._find_best_split = self._get_find_best_split(max_features)
             tree.fit(X_sample, y_sample)
             self.trees.append(tree)
         
         self.is_fitted = True
         return self
@@ -197,65 +243,65 @@
                 thresholds = np.unique(X[:, feature_index])
                 for threshold in thresholds:
                     left_indices = X[:, feature_index] < threshold
                     left_labels = y[left_indices]
                     right_labels = y[~left_indices]
                     
                     if len(left_labels) == 0 or len(right_labels) == 0:
-                        continue  # Skip if one of the child nodes is empty
+                        continue
                     
-                    # Calculate variance for the child nodes
                     variance_left = np.var(left_labels)
                     variance_right = np.var(right_labels)
                     
-                    # Calculate weighted average variance
                     weight_left = len(left_labels) / len(y)
                     weight_right = len(right_labels) / len(y)
                     weighted_avg_variance = weight_left * variance_left + weight_right * variance_right
                     
-                    # Calculate variance reduction
                     variance_reduction = parent_variance - weighted_avg_variance
                     
                     if variance_reduction > best_variance_reduction:
                         best_variance_reduction = variance_reduction
                         best_split = (feature_index, threshold)
             
             return best_split
         
         return _find_best_split
 
     def predict(self, X):
-        """Predict values for X.
-        
+        """
+        Predict values for X.
+
         Parameters:
-        X (np.ndarray): Test data.
-        
+        -----------
+        X : np.ndarray
+            Test data.
+
         Returns:
-        np.ndarray: Predicted values.
+        --------
+        np.ndarray
+            Predicted values.
         """
         if not self.is_fitted:
             raise ValueError("The model has not been fitted yet.")
         
         tree_predictions = np.array([tree.predict(X) for tree in self.trees])
-        # Mean of predictions
         mean_predictions = np.mean(tree_predictions, axis=0)
         return mean_predictions
     
     def score(self, X, y):
-        """Evaluate the model on the test data.
-        
+        """
+        Evaluate the model on the test data.
+
         Parameters:
-        X (np.ndarray): Test data.
-        y (np.ndarray): True values.
-        
+        -----------
+        X : np.ndarray
+            Test data.
+        y : np.ndarray
+            True values.
+
         Returns:
-        float: Negative mean squared error.
+        --------
+        float
+            Negative mean squared error.
         """
         y_pred = self.predict(X)
         return -mean_squared_error(y, y_pred)
-    
-    
-    def set_params(self, **params):
-        """Set the parameters of the model."""
-        for param, value in params.items():
-            setattr(self, param, value)
-        return self
```

### Comparing `mini_scikit_learn-0.1.3/mini_scikit_learn/SVM.py` & `mini_scikit_learn-0.1.4/mini_scikit_learn/SVM.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,30 @@
-import numpy as np 
+import numpy as np
 
 class SupportVectorMachine:
-    """
-    Implementation of the Support Vector Machine.
-    
-    """
 
     def __init__(self, learning_rate=0.001, lambda_param=0.01, n_iters=1000):
+        """Initialize the Support Vector Machine."""
         self.lr = learning_rate
         self.lambda_param = lambda_param
         self.n_iters = n_iters
         self.w = None
         self.b = None
 
-
     def fit(self, X, y):
+        """
+        Fit the SVM model to the training data.
+
+        Parameters:
+        -----------
+        X : numpy.ndarray
+            Training data.
+        y : numpy.ndarray
+            Target labels.
+        """
         n_samples, n_features = X.shape
 
         y_ = np.where(y <= 0, -1, 1)
 
         self.w = np.zeros(n_features)
         self.b = 0
 
@@ -27,12 +33,22 @@
                 condition = y_[idx] * (np.dot(x_i, self.w) - self.b) >= 1
                 if condition:
                     self.w -= self.lr * (2 * self.lambda_param * self.w)
                 else:
                     self.w -= self.lr * (2 * self.lambda_param * self.w - np.dot(x_i, y_[idx]))
                     self.b -= self.lr * y_[idx]
 
-
     def predict(self, X):
+        """
+        Predict class labels for samples in X.
+        Parameters:
+        -----------
+        X : numpy.ndarray
+            Test data.
+
+        Returns:
+        --------
+        numpy.ndarray
+            Predicted class labels.
+        """
         approx = np.dot(X, self.w) - self.b
         return np.sign(approx)
-
```

### Comparing `mini_scikit_learn-0.1.3/mini_scikit_learn/main.py` & `mini_scikit_learn-0.1.4/mini_scikit_learn/main.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.3/mini_scikit_learn/test1.py` & `mini_scikit_learn-0.1.4/mini_scikit_learn/test1.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.3/mini_scikit_learn/test2.py` & `mini_scikit_learn-0.1.4/mini_scikit_learn/test2.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from sklearn.datasets import load_digits
 from sklearn.preprocessing import StandardScaler, OneHotEncoder
 from sklearn.model_selection import train_test_split
-from NN import NeuralNetwork, Layer 
+from NN import Network, Layer 
 import numpy as np 
 # Load Digits data
 digits = load_digits()
 X = digits.data
 y = digits.target.reshape(-1, 1)
 
 # Select a subset of data for quicker training
@@ -19,36 +19,40 @@
 # Normalize features
 scaler = StandardScaler()
 X_scaled = scaler.fit_transform(X_subset)
 
 # One-hot encode labels
 encoder = OneHotEncoder()
 y_encoded = encoder.fit_transform(y_subset).toarray()
+print(y_encoded.shape)
 
 X_train, X_test, y_train, y_test = train_test_split(X_scaled, y_encoded, test_size=0.2, random_state=42)
 
-# Define your neural NeuralNetwork structure
-NeuralNetwork = NeuralNetwork()
-NeuralNetwork.add(Layer(64, 64, 'sigmoid'))  # Hidden layer with 50 neurons
-NeuralNetwork.add(Layer(64, 10, 'sigmoid'))  # Output layer with 10 neurons
+# Define your neural network structure
+network = Network()
+network.add(Layer(64, 64, 'sigmoid'))  # Hidden layer with 50 neurons
+network.add(Layer(64, 10, 'sigmoid'))  # Output layer with 10 neurons
 
-# Train the NeuralNetwork
-NeuralNetwork.fit(X_train, y_train, epochs=10, learning_rate=0.01)
+# Train the network
+network.fit(X_train, y_train, epochs=1000, learning_rate=0.01)
 
 # Predictions
-predictions = NeuralNetwork.predict(X_test)
+predictions = network.predict(X_test)
 
 # Convert predictions to class labels
 def convert_prob_to_class(probs):
     return np.argmax(probs, axis=1)
 
+predicted_classes = convert_prob_to_class(predictions)
 
 # Convert one-hot encoded test labels back to class labels
-#actual_classes = np.argmax(y_test, axis=1)
-accuracy=NeuralNetwork.score(X_test,y_test)
+actual_classes = np.argmax(y_test, axis=1)
+
+# Calculate accuracy
+accuracy = np.mean(predicted_classes == actual_classes)
 print("Accuracy:", accuracy)
-#print("Predicted classes:", predicted_classes)
-#print("Actual classes:", actual_classes)
+print("Predicted classes:", predicted_classes)
+print("Actual classes:", actual_classes)
```

### Comparing `mini_scikit_learn-0.1.3/mini_scikit_learn/test_ada.py` & `mini_scikit_learn-0.1.4/mini_scikit_learn/test_ada.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.3/mini_scikit_learn/test_cv.py` & `mini_scikit_learn-0.1.4/mini_scikit_learn/test_cv.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.3/mini_scikit_learn/test_dt.py` & `mini_scikit_learn-0.1.4/mini_scikit_learn/test_dt.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.3/mini_scikit_learn/test_dtr.py` & `mini_scikit_learn-0.1.4/mini_scikit_learn/test_dtr.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.3/mini_scikit_learn/test_knn.py` & `mini_scikit_learn-0.1.4/mini_scikit_learn/test_knn.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from KnnEtimator import KNNEstimator
+from KnnEstimator import KnnEstimator
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
 
-your_model_digits = KNNEstimator()  # Use k=5 as an example
+your_model_digits = KnnEstimator()  # Use k=5 as an example
 your_model_digits.fit(X_digits_train, y_digits_train)
 your_score_digits = your_model_digits.score(X_digits_test, y_digits_test)
-print("Your KNNEstimator Score (Digits):", your_score_digits)
+print("Your KnnEstimator Score (Digits):", your_score_digits)
 
-your_model_iris = KNNEstimator()  # Use k=5 as an example
+your_model_iris = KnnEstimator()  # Use k=5 as an example
 your_model_iris.fit(X_iris_train, y_iris_train)
 your_score_iris = your_model_iris.score(X_iris_test, y_iris_test)
-print("Your KNNEstimator Score (Iris):", your_score_iris)
+print("Your KnnEstimator Score (Iris):", your_score_iris)
 
 sklearn_model_digits = SklearnKNeighborsClassifier(n_neighbors=5)  # Use n_neighbors=5 as an example
 sklearn_model_digits.fit(X_digits_train, y_digits_train)
 sklearn_score_digits = sklearn_model_digits.score(X_digits_test, y_digits_test)
 print("Scikit-learn KNeighborsClassifier Score (Digits):", sklearn_score_digits)
 
 sklearn_model_iris = SklearnKNeighborsClassifier(n_neighbors=5)  # Use n_neighbors=5 as an example
```

### Comparing `mini_scikit_learn-0.1.3/mini_scikit_learn/test_lg.py` & `mini_scikit_learn-0.1.4/mini_scikit_learn/test_lg.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.3/mini_scikit_learn/test_lgr.py` & `mini_scikit_learn-0.1.4/mini_scikit_learn/test_lgr.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.3/mini_scikit_learn/test_nb.py` & `mini_scikit_learn-0.1.4/mini_scikit_learn/test_nb.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.3/mini_scikit_learn/test_nn.py` & `mini_scikit_learn-0.1.4/mini_scikit_learn/test_nn.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.3/mini_scikit_learn/test_nn2.py` & `mini_scikit_learn-0.1.4/mini_scikit_learn/test_nn2.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.3/mini_scikit_learn/test_rf.py` & `mini_scikit_learn-0.1.4/mini_scikit_learn/test_rf.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.3/mini_scikit_learn/test_stacking.py` & `mini_scikit_learn-0.1.4/mini_scikit_learn/test_stacking.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.3/mini_scikit_learn/test_voting.py` & `mini_scikit_learn-0.1.4/mini_scikit_learn/test_voting.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.3/mini_scikit_learn/utils/NeuralNetwork.py` & `mini_scikit_learn-0.1.4/mini_scikit_learn/utils/NeuralNetwork.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.3/mini_scikit_learn.egg-info/PKG-INFO` & `mini_scikit_learn-0.1.4/mini_scikit_learn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mini-scikit-learn
-Version: 0.1.3
+Version: 0.1.4
 Summary: A brief description of your package
 Home-page: https://github.com/YASSIRFRI/mini_scikit_learn.git
 Author: Yassir Fri
 Author-email: your.email@example.com
 License: UNKNOWN
 Description: # mini_scikit_learn
```

### Comparing `mini_scikit_learn-0.1.3/mini_scikit_learn.egg-info/SOURCES.txt` & `mini_scikit_learn-0.1.4/mini_scikit_learn.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 mini_scikit_learn/LogisticRegression.py
 mini_scikit_learn/ModelEnsembler.py
 mini_scikit_learn/NBClassifier.py
 mini_scikit_learn/NN.py
 mini_scikit_learn/Predictor.py
 mini_scikit_learn/RandomForest.py
 mini_scikit_learn/SVM.py
-mini_scikit_learn/__init__.py
 mini_scikit_learn/main.py
 mini_scikit_learn/test1.py
 mini_scikit_learn/test2.py
 mini_scikit_learn/test_ada.py
 mini_scikit_learn/test_cv.py
 mini_scikit_learn/test_dt.py
 mini_scikit_learn/test_dtr.py
@@ -30,22 +29,11 @@
 mini_scikit_learn/test_stacking.py
 mini_scikit_learn/test_voting.py
 mini_scikit_learn.egg-info/PKG-INFO
 mini_scikit_learn.egg-info/SOURCES.txt
 mini_scikit_learn.egg-info/dependency_links.txt
 mini_scikit_learn.egg-info/requires.txt
 mini_scikit_learn.egg-info/top_level.txt
-mini_scikit_learn/metrics/__init__.py
 mini_scikit_learn/metrics/metric.py
-mini_scikit_learn/model_selection/GridSearch.py
-mini_scikit_learn/model_selection/RandomSearch.py
-mini_scikit_learn/model_selection/__init__.py
-mini_scikit_learn/transformers/Encoders.py
-mini_scikit_learn/transformers/Imputers.py
-mini_scikit_learn/transformers/Transfomer.py
-mini_scikit_learn/transformers/__init__.py
-mini_scikit_learn/transformers/encoderTest.py
-mini_scikit_learn/utils/Kfolds.py
 mini_scikit_learn/utils/NeuralNetwork.py
-mini_scikit_learn/utils/__init__.py
 mini_scikit_learn/utils/cross_validation.py
 mini_scikit_learn/utils/train_test_split.py
```

### Comparing `mini_scikit_learn-0.1.3/setup.py` & `mini_scikit_learn-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mini_scikit_learn',  # Replace with your package name
-    version='0.1.3',  # Initial version of your package
+    version='0.1.4',  # Initial version of your package
     author='Yassir Fri',
     author_email='your.email@example.com',
     description='A brief description of your package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/YASSIRFRI/mini_scikit_learn.git",
     packages=find_packages(),
```

