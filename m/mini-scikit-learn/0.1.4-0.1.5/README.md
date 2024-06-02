# Comparing `tmp/mini_scikit_learn-0.1.4.tar.gz` & `tmp/mini_scikit_learn-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mini_scikit_learn-0.1.4.tar", last modified: Sun Jun  2 23:18:21 2024, max compression
+gzip compressed data, was "mini_scikit_learn-0.1.5.tar", last modified: Sun Jun  2 23:22:50 2024, max compression
```

## Comparing `mini_scikit_learn-0.1.4.tar` & `mini_scikit_learn-0.1.5.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2024-06-02 23:18:21.987858 mini_scikit_learn-0.1.4/
--rw-rw-rw-   0        0        0     6155 2024-06-02 23:18:21.985819 mini_scikit_learn-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     4754 2024-06-02 22:00:40.000000 mini_scikit_learn-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-06-02 23:18:21.873468 mini_scikit_learn-0.1.4/mini_scikit_learn/
--rw-rw-rw-   0        0        0     4984 2024-06-02 23:15:29.000000 mini_scikit_learn-0.1.4/mini_scikit_learn/AdaBoost.py
--rw-rw-rw-   0        0        0    12707 2024-06-02 23:15:29.000000 mini_scikit_learn-0.1.4/mini_scikit_learn/DecisionTree.py
--rw-rw-rw-   0        0        0     1865 2024-06-02 23:15:29.000000 mini_scikit_learn-0.1.4/mini_scikit_learn/Estimator.py
--rw-rw-rw-   0        0        0     2265 2024-06-02 23:15:49.000000 mini_scikit_learn-0.1.4/mini_scikit_learn/KnnEstimator.py
--rw-rw-rw-   0        0        0     9832 2024-06-02 23:15:29.000000 mini_scikit_learn-0.1.4/mini_scikit_learn/LinearModel.py
--rw-rw-rw-   0        0        0     4952 2024-06-02 22:49:10.000000 mini_scikit_learn-0.1.4/mini_scikit_learn/LogisticRegression.py
--rw-rw-rw-   0        0        0     8572 2024-06-02 23:15:29.000000 mini_scikit_learn-0.1.4/mini_scikit_learn/ModelEnsembler.py
--rw-rw-rw-   0        0        0     3817 2024-06-02 22:49:10.000000 mini_scikit_learn-0.1.4/mini_scikit_learn/NBClassifier.py
--rw-rw-rw-   0        0        0     5092 2024-06-02 23:15:29.000000 mini_scikit_learn-0.1.4/mini_scikit_learn/NN.py
--rw-rw-rw-   0        0        0     1679 2024-06-02 23:15:57.000000 mini_scikit_learn-0.1.4/mini_scikit_learn/Predictor.py
--rw-rw-rw-   0        0        0    10782 2024-06-02 23:15:29.000000 mini_scikit_learn-0.1.4/mini_scikit_learn/RandomForest.py
--rw-rw-rw-   0        0        0     1542 2024-06-02 23:16:32.000000 mini_scikit_learn-0.1.4/mini_scikit_learn/SVM.py
--rw-rw-rw-   0        0        0      819 2024-05-01 21:00:46.000000 mini_scikit_learn-0.1.4/mini_scikit_learn/main.py
-drwxrwxrwx   0        0        0        0 2024-06-02 23:18:21.923771 mini_scikit_learn-0.1.4/mini_scikit_learn/metrics/
--rw-rw-rw-   0        0        0     4575 2024-06-02 22:49:10.000000 mini_scikit_learn-0.1.4/mini_scikit_learn/metrics/metric.py
--rw-rw-rw-   0        0        0     1768 2024-05-08 19:11:07.000000 mini_scikit_learn-0.1.4/mini_scikit_learn/test1.py
--rw-rw-rw-   0        0        0     1735 2024-06-02 23:15:29.000000 mini_scikit_learn-0.1.4/mini_scikit_learn/test2.py
--rw-rw-rw-   0        0        0      771 2024-05-22 19:35:27.000000 mini_scikit_learn-0.1.4/mini_scikit_learn/test_ada.py
--rw-rw-rw-   0        0        0      732 2024-05-22 18:05:25.000000 mini_scikit_learn-0.1.4/mini_scikit_learn/test_cv.py
--rw-rw-rw-   0        0        0     2024 2024-05-22 18:24:36.000000 mini_scikit_learn-0.1.4/mini_scikit_learn/test_dt.py
--rw-rw-rw-   0        0        0     1242 2024-05-14 16:27:56.000000 mini_scikit_learn-0.1.4/mini_scikit_learn/test_dtr.py
--rw-rw-rw-   0        0        0     1805 2024-06-02 23:15:29.000000 mini_scikit_learn-0.1.4/mini_scikit_learn/test_knn.py
--rw-rw-rw-   0        0        0     1197 2024-05-14 23:37:28.000000 mini_scikit_learn-0.1.4/mini_scikit_learn/test_lg.py
--rw-rw-rw-   0        0        0     2249 2024-05-15 08:54:45.000000 mini_scikit_learn-0.1.4/mini_scikit_learn/test_lgr.py
--rw-rw-rw-   0        0        0     3100 2024-05-05 19:11:00.000000 mini_scikit_learn-0.1.4/mini_scikit_learn/test_nb.py
--rw-rw-rw-   0        0        0     4047 2024-05-07 15:17:35.000000 mini_scikit_learn-0.1.4/mini_scikit_learn/test_nn.py
--rw-rw-rw-   0        0        0     1981 2024-05-07 15:29:08.000000 mini_scikit_learn-0.1.4/mini_scikit_learn/test_nn2.py
--rw-rw-rw-   0        0        0     3939 2024-05-14 17:29:42.000000 mini_scikit_learn-0.1.4/mini_scikit_learn/test_rf.py
--rw-rw-rw-   0        0        0     2046 2024-05-15 09:12:06.000000 mini_scikit_learn-0.1.4/mini_scikit_learn/test_stacking.py
--rw-rw-rw-   0        0        0     2364 2024-05-15 09:18:44.000000 mini_scikit_learn-0.1.4/mini_scikit_learn/test_voting.py
-drwxrwxrwx   0        0        0        0 2024-06-02 23:18:21.944188 mini_scikit_learn-0.1.4/mini_scikit_learn/utils/
--rw-rw-rw-   0        0        0     5149 2024-05-08 08:28:46.000000 mini_scikit_learn-0.1.4/mini_scikit_learn/utils/NeuralNetwork.py
--rw-rw-rw-   0        0        0     1380 2024-06-02 23:15:29.000000 mini_scikit_learn-0.1.4/mini_scikit_learn/utils/cross_validation.py
--rw-rw-rw-   0        0        0     1769 2024-06-02 23:15:29.000000 mini_scikit_learn-0.1.4/mini_scikit_learn/utils/train_test_split.py
-drwxrwxrwx   0        0        0        0 2024-06-02 23:18:21.913461 mini_scikit_learn-0.1.4/mini_scikit_learn.egg-info/
--rw-rw-rw-   0        0        0     6155 2024-06-02 23:18:21.000000 mini_scikit_learn-0.1.4/mini_scikit_learn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1245 2024-06-02 23:18:21.000000 mini_scikit_learn-0.1.4/mini_scikit_learn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 23:18:21.000000 mini_scikit_learn-0.1.4/mini_scikit_learn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-06-02 23:18:21.000000 mini_scikit_learn-0.1.4/mini_scikit_learn.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 23:18:21.000000 mini_scikit_learn-0.1.4/mini_scikit_learn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-06-02 23:18:21.987858 mini_scikit_learn-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      787 2024-06-02 23:16:50.000000 mini_scikit_learn-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 23:22:50.124792 mini_scikit_learn-0.1.5/
+-rw-rw-rw-   0        0        0     6155 2024-06-02 23:22:50.123782 mini_scikit_learn-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4754 2024-06-02 22:00:40.000000 mini_scikit_learn-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-06-02 23:22:50.007863 mini_scikit_learn-0.1.5/mini_scikit_learn/
+-rw-rw-rw-   0        0        0     4984 2024-06-02 23:15:29.000000 mini_scikit_learn-0.1.5/mini_scikit_learn/AdaBoost.py
+-rw-rw-rw-   0        0        0    12707 2024-06-02 23:15:29.000000 mini_scikit_learn-0.1.5/mini_scikit_learn/DecisionTree.py
+-rw-rw-rw-   0        0        0     1865 2024-06-02 23:15:29.000000 mini_scikit_learn-0.1.5/mini_scikit_learn/Estimator.py
+-rw-rw-rw-   0        0        0     2265 2024-06-02 23:15:49.000000 mini_scikit_learn-0.1.5/mini_scikit_learn/KnnEstimator.py
+-rw-rw-rw-   0        0        0     9832 2024-06-02 23:15:29.000000 mini_scikit_learn-0.1.5/mini_scikit_learn/LinearModel.py
+-rw-rw-rw-   0        0        0     4952 2024-06-02 22:49:10.000000 mini_scikit_learn-0.1.5/mini_scikit_learn/LogisticRegression.py
+-rw-rw-rw-   0        0        0     8512 2024-06-02 23:21:51.000000 mini_scikit_learn-0.1.5/mini_scikit_learn/ModelEnsembler.py
+-rw-rw-rw-   0        0        0     3817 2024-06-02 22:49:10.000000 mini_scikit_learn-0.1.5/mini_scikit_learn/NBClassifier.py
+-rw-rw-rw-   0        0        0     5092 2024-06-02 23:15:29.000000 mini_scikit_learn-0.1.5/mini_scikit_learn/NN.py
+-rw-rw-rw-   0        0        0     1679 2024-06-02 23:15:57.000000 mini_scikit_learn-0.1.5/mini_scikit_learn/Predictor.py
+-rw-rw-rw-   0        0        0    10782 2024-06-02 23:15:29.000000 mini_scikit_learn-0.1.5/mini_scikit_learn/RandomForest.py
+-rw-rw-rw-   0        0        0     1542 2024-06-02 23:16:32.000000 mini_scikit_learn-0.1.5/mini_scikit_learn/SVM.py
+-rw-rw-rw-   0        0        0      819 2024-05-01 21:00:46.000000 mini_scikit_learn-0.1.5/mini_scikit_learn/main.py
+drwxrwxrwx   0        0        0        0 2024-06-02 23:22:50.112215 mini_scikit_learn-0.1.5/mini_scikit_learn/metrics/
+-rw-rw-rw-   0        0        0     4575 2024-06-02 22:49:10.000000 mini_scikit_learn-0.1.5/mini_scikit_learn/metrics/metric.py
+-rw-rw-rw-   0        0        0     1768 2024-05-08 19:11:07.000000 mini_scikit_learn-0.1.5/mini_scikit_learn/test1.py
+-rw-rw-rw-   0        0        0     1735 2024-06-02 23:15:29.000000 mini_scikit_learn-0.1.5/mini_scikit_learn/test2.py
+-rw-rw-rw-   0        0        0      771 2024-05-22 19:35:27.000000 mini_scikit_learn-0.1.5/mini_scikit_learn/test_ada.py
+-rw-rw-rw-   0        0        0      732 2024-05-22 18:05:25.000000 mini_scikit_learn-0.1.5/mini_scikit_learn/test_cv.py
+-rw-rw-rw-   0        0        0     2024 2024-05-22 18:24:36.000000 mini_scikit_learn-0.1.5/mini_scikit_learn/test_dt.py
+-rw-rw-rw-   0        0        0     1242 2024-05-14 16:27:56.000000 mini_scikit_learn-0.1.5/mini_scikit_learn/test_dtr.py
+-rw-rw-rw-   0        0        0     1805 2024-06-02 23:15:29.000000 mini_scikit_learn-0.1.5/mini_scikit_learn/test_knn.py
+-rw-rw-rw-   0        0        0     1197 2024-05-14 23:37:28.000000 mini_scikit_learn-0.1.5/mini_scikit_learn/test_lg.py
+-rw-rw-rw-   0        0        0     2249 2024-05-15 08:54:45.000000 mini_scikit_learn-0.1.5/mini_scikit_learn/test_lgr.py
+-rw-rw-rw-   0        0        0     3100 2024-05-05 19:11:00.000000 mini_scikit_learn-0.1.5/mini_scikit_learn/test_nb.py
+-rw-rw-rw-   0        0        0     4047 2024-05-07 15:17:35.000000 mini_scikit_learn-0.1.5/mini_scikit_learn/test_nn.py
+-rw-rw-rw-   0        0        0     1981 2024-05-07 15:29:08.000000 mini_scikit_learn-0.1.5/mini_scikit_learn/test_nn2.py
+-rw-rw-rw-   0        0        0     3939 2024-05-14 17:29:42.000000 mini_scikit_learn-0.1.5/mini_scikit_learn/test_rf.py
+-rw-rw-rw-   0        0        0     2046 2024-05-15 09:12:06.000000 mini_scikit_learn-0.1.5/mini_scikit_learn/test_stacking.py
+-rw-rw-rw-   0        0        0     2364 2024-05-15 09:18:44.000000 mini_scikit_learn-0.1.5/mini_scikit_learn/test_voting.py
+drwxrwxrwx   0        0        0        0 2024-06-02 23:22:50.120793 mini_scikit_learn-0.1.5/mini_scikit_learn/utils/
+-rw-rw-rw-   0        0        0     5149 2024-05-08 08:28:46.000000 mini_scikit_learn-0.1.5/mini_scikit_learn/utils/NeuralNetwork.py
+-rw-rw-rw-   0        0        0     1380 2024-06-02 23:15:29.000000 mini_scikit_learn-0.1.5/mini_scikit_learn/utils/cross_validation.py
+-rw-rw-rw-   0        0        0     1769 2024-06-02 23:15:29.000000 mini_scikit_learn-0.1.5/mini_scikit_learn/utils/train_test_split.py
+drwxrwxrwx   0        0        0        0 2024-06-02 23:22:50.108208 mini_scikit_learn-0.1.5/mini_scikit_learn.egg-info/
+-rw-rw-rw-   0        0        0     6155 2024-06-02 23:22:49.000000 mini_scikit_learn-0.1.5/mini_scikit_learn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1245 2024-06-02 23:22:49.000000 mini_scikit_learn-0.1.5/mini_scikit_learn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 23:22:49.000000 mini_scikit_learn-0.1.5/mini_scikit_learn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-06-02 23:22:49.000000 mini_scikit_learn-0.1.5/mini_scikit_learn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 23:22:49.000000 mini_scikit_learn-0.1.5/mini_scikit_learn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-02 23:22:50.125788 mini_scikit_learn-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      719 2024-06-02 23:22:42.000000 mini_scikit_learn-0.1.5/setup.py
```

### Comparing `mini_scikit_learn-0.1.4/PKG-INFO` & `mini_scikit_learn-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mini_scikit_learn
-Version: 0.1.4
+Version: 0.1.5
 Summary: A brief description of your package
 Home-page: https://github.com/YASSIRFRI/mini_scikit_learn.git
 Author: Yassir Fri
 Author-email: your.email@example.com
 License: UNKNOWN
 Description: # mini_scikit_learn
```

### Comparing `mini_scikit_learn-0.1.4/README.md` & `mini_scikit_learn-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.4/mini_scikit_learn/AdaBoost.py` & `mini_scikit_learn-0.1.5/mini_scikit_learn/AdaBoost.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.4/mini_scikit_learn/DecisionTree.py` & `mini_scikit_learn-0.1.5/mini_scikit_learn/DecisionTree.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.4/mini_scikit_learn/Estimator.py` & `mini_scikit_learn-0.1.5/mini_scikit_learn/Estimator.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.4/mini_scikit_learn/KnnEstimator.py` & `mini_scikit_learn-0.1.5/mini_scikit_learn/KnnEstimator.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.4/mini_scikit_learn/LinearModel.py` & `mini_scikit_learn-0.1.5/mini_scikit_learn/LinearModel.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.4/mini_scikit_learn/LogisticRegression.py` & `mini_scikit_learn-0.1.5/mini_scikit_learn/LogisticRegression.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.4/mini_scikit_learn/ModelEnsembler.py` & `mini_scikit_learn-0.1.5/mini_scikit_learn/ModelEnsembler.py`

 * *Files 0% similar despite different names*

```diff
@@ -285,16 +285,14 @@
         super().__init__(self)
 
     def fit(self, X, y):
         for model in self.base_models:
             model.fit(X, y)
             print(model.score(X, y))
         X_meta = np.array([model.predict(X) for model in self.base_models]).T
-        print("X_meta shape")
-        print(X_meta.shape)
         self.meta_model.fit(X_meta, y,lr=0.001)
         print("Meta model score")
         print(self.meta_model.score(X_meta, y))
         self.is_fitted = True
         return self
 
     def predict(self, X):
```

### Comparing `mini_scikit_learn-0.1.4/mini_scikit_learn/NBClassifier.py` & `mini_scikit_learn-0.1.5/mini_scikit_learn/NBClassifier.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.4/mini_scikit_learn/NN.py` & `mini_scikit_learn-0.1.5/mini_scikit_learn/NN.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.4/mini_scikit_learn/Predictor.py` & `mini_scikit_learn-0.1.5/mini_scikit_learn/Predictor.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.4/mini_scikit_learn/RandomForest.py` & `mini_scikit_learn-0.1.5/mini_scikit_learn/RandomForest.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.4/mini_scikit_learn/SVM.py` & `mini_scikit_learn-0.1.5/mini_scikit_learn/SVM.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.4/mini_scikit_learn/main.py` & `mini_scikit_learn-0.1.5/mini_scikit_learn/main.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.4/mini_scikit_learn/metrics/metric.py` & `mini_scikit_learn-0.1.5/mini_scikit_learn/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.4/mini_scikit_learn/test1.py` & `mini_scikit_learn-0.1.5/mini_scikit_learn/test1.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.4/mini_scikit_learn/test2.py` & `mini_scikit_learn-0.1.5/mini_scikit_learn/test2.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.4/mini_scikit_learn/test_ada.py` & `mini_scikit_learn-0.1.5/mini_scikit_learn/test_ada.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.4/mini_scikit_learn/test_cv.py` & `mini_scikit_learn-0.1.5/mini_scikit_learn/test_cv.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.4/mini_scikit_learn/test_dt.py` & `mini_scikit_learn-0.1.5/mini_scikit_learn/test_dt.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.4/mini_scikit_learn/test_dtr.py` & `mini_scikit_learn-0.1.5/mini_scikit_learn/test_dtr.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.4/mini_scikit_learn/test_knn.py` & `mini_scikit_learn-0.1.5/mini_scikit_learn/test_knn.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.4/mini_scikit_learn/test_lg.py` & `mini_scikit_learn-0.1.5/mini_scikit_learn/test_lg.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.4/mini_scikit_learn/test_lgr.py` & `mini_scikit_learn-0.1.5/mini_scikit_learn/test_lgr.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.4/mini_scikit_learn/test_nb.py` & `mini_scikit_learn-0.1.5/mini_scikit_learn/test_nb.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.4/mini_scikit_learn/test_nn.py` & `mini_scikit_learn-0.1.5/mini_scikit_learn/test_nn.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.4/mini_scikit_learn/test_nn2.py` & `mini_scikit_learn-0.1.5/mini_scikit_learn/test_nn2.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.4/mini_scikit_learn/test_rf.py` & `mini_scikit_learn-0.1.5/mini_scikit_learn/test_rf.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.4/mini_scikit_learn/test_stacking.py` & `mini_scikit_learn-0.1.5/mini_scikit_learn/test_stacking.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.4/mini_scikit_learn/test_voting.py` & `mini_scikit_learn-0.1.5/mini_scikit_learn/test_voting.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.4/mini_scikit_learn/utils/NeuralNetwork.py` & `mini_scikit_learn-0.1.5/mini_scikit_learn/utils/NeuralNetwork.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.4/mini_scikit_learn/utils/cross_validation.py` & `mini_scikit_learn-0.1.5/mini_scikit_learn/utils/cross_validation.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.4/mini_scikit_learn/utils/train_test_split.py` & `mini_scikit_learn-0.1.5/mini_scikit_learn/utils/train_test_split.py`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.4/mini_scikit_learn.egg-info/PKG-INFO` & `mini_scikit_learn-0.1.5/mini_scikit_learn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mini-scikit-learn
-Version: 0.1.4
+Version: 0.1.5
 Summary: A brief description of your package
 Home-page: https://github.com/YASSIRFRI/mini_scikit_learn.git
 Author: Yassir Fri
 Author-email: your.email@example.com
 License: UNKNOWN
 Description: # mini_scikit_learn
```

### Comparing `mini_scikit_learn-0.1.4/mini_scikit_learn.egg-info/SOURCES.txt` & `mini_scikit_learn-0.1.5/mini_scikit_learn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mini_scikit_learn-0.1.4/setup.py` & `mini_scikit_learn-0.1.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
-    name='mini_scikit_learn',  # Replace with your package name
-    version='0.1.4',  # Initial version of your package
+    name='mini_scikit_learn', 
+    version='0.1.5',
     author='Yassir Fri',
     author_email='your.email@example.com',
     description='A brief description of your package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/YASSIRFRI/mini_scikit_learn.git",
     packages=find_packages(),
```

