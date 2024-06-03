# Comparing `tmp/m_o_mini_scikit_learn_ai_project-0.1.0.tar.gz` & `tmp/m_o_mini_scikit_learn_ai_project-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m_o_mini_scikit_learn_ai_project-0.1.0.tar", last modified: Sun Jun  2 23:30:41 2024, max compression
+gzip compressed data, was "m_o_mini_scikit_learn_ai_project-0.1.1.tar", last modified: Mon Jun  3 00:17:22 2024, max compression
```

## Comparing `m_o_mini_scikit_learn_ai_project-0.1.0.tar` & `m_o_mini_scikit_learn_ai_project-0.1.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-06-02 23:30:41.985608 m_o_mini_scikit_learn_ai_project-0.1.0/
-drwxrwxrwx   0        0        0        0 2024-06-02 23:30:41.782092 m_o_mini_scikit_learn_ai_project-0.1.0/Mini-Scikit-Learn/
--rw-rw-rw-   0        0        0        0 2024-06-02 23:11:21.000000 m_o_mini_scikit_learn_ai_project-0.1.0/Mini-Scikit-Learn/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-02 23:30:41.790208 m_o_mini_scikit_learn_ai_project-0.1.0/Mini-Scikit-Learn/base/
--rw-rw-rw-   0        0        0        0 2024-05-06 10:54:58.000000 m_o_mini_scikit_learn_ai_project-0.1.0/Mini-Scikit-Learn/base/__init__.py
--rw-rw-rw-   0        0        0     2778 2024-06-02 22:11:28.000000 m_o_mini_scikit_learn_ai_project-0.1.0/Mini-Scikit-Learn/base/estimator.py
--rw-rw-rw-   0        0        0     4291 2024-06-02 22:11:28.000000 m_o_mini_scikit_learn_ai_project-0.1.0/Mini-Scikit-Learn/base/predictor.py
--rw-rw-rw-   0        0        0     3295 2024-06-02 22:11:28.000000 m_o_mini_scikit_learn_ai_project-0.1.0/Mini-Scikit-Learn/base/transformer.py
-drwxrwxrwx   0        0        0        0 2024-06-02 23:30:41.807602 m_o_mini_scikit_learn_ai_project-0.1.0/Mini-Scikit-Learn/model_selection_and_evaluation/
--rw-rw-rw-   0        0        0        0 2024-05-06 10:54:58.000000 m_o_mini_scikit_learn_ai_project-0.1.0/Mini-Scikit-Learn/model_selection_and_evaluation/__init__.py
--rw-rw-rw-   0        0        0     4483 2024-06-02 22:11:28.000000 m_o_mini_scikit_learn_ai_project-0.1.0/Mini-Scikit-Learn/model_selection_and_evaluation/cross_validation.py
--rw-rw-rw-   0        0        0     4493 2024-06-02 22:11:28.000000 m_o_mini_scikit_learn_ai_project-0.1.0/Mini-Scikit-Learn/model_selection_and_evaluation/grid_search.py
--rw-rw-rw-   0        0        0     3745 2024-06-02 22:11:28.000000 m_o_mini_scikit_learn_ai_project-0.1.0/Mini-Scikit-Learn/model_selection_and_evaluation/performance_metrics.py
--rw-rw-rw-   0        0        0     1116 2024-05-13 14:04:21.000000 m_o_mini_scikit_learn_ai_project-0.1.0/Mini-Scikit-Learn/model_selection_and_evaluation/train_test_split.py
-drwxrwxrwx   0        0        0        0 2024-06-02 23:30:41.816846 m_o_mini_scikit_learn_ai_project-0.1.0/Mini-Scikit-Learn/neural_networks/
--rw-rw-rw-   0        0        0        0 2024-05-06 10:54:58.000000 m_o_mini_scikit_learn_ai_project-0.1.0/Mini-Scikit-Learn/neural_networks/__init__.py
--rw-rw-rw-   0        0        0     2259 2024-06-02 22:11:28.000000 m_o_mini_scikit_learn_ai_project-0.1.0/Mini-Scikit-Learn/neural_networks/baseNeu.py
--rw-rw-rw-   0        0        0     6891 2024-06-02 22:11:28.000000 m_o_mini_scikit_learn_ai_project-0.1.0/Mini-Scikit-Learn/neural_networks/convolutional_neural_networks.py
--rw-rw-rw-   0        0        0     3192 2024-06-02 22:11:28.000000 m_o_mini_scikit_learn_ai_project-0.1.0/Mini-Scikit-Learn/neural_networks/perceptron.py
-drwxrwxrwx   0        0        0        0 2024-06-02 23:30:41.833519 m_o_mini_scikit_learn_ai_project-0.1.0/Mini-Scikit-Learn/supervised_learning/
--rw-rw-rw-   0        0        0        0 2024-05-09 14:15:32.000000 m_o_mini_scikit_learn_ai_project-0.1.0/Mini-Scikit-Learn/supervised_learning/__init__.py
--rw-rw-rw-   0        0        0     7356 2024-06-02 22:11:28.000000 m_o_mini_scikit_learn_ai_project-0.1.0/Mini-Scikit-Learn/supervised_learning/decision_trees.py
--rw-rw-rw-   0        0        0     4715 2024-06-02 22:11:28.000000 m_o_mini_scikit_learn_ai_project-0.1.0/Mini-Scikit-Learn/supervised_learning/linear_models.py
--rw-rw-rw-   0        0        0     2547 2024-06-02 22:11:28.000000 m_o_mini_scikit_learn_ai_project-0.1.0/Mini-Scikit-Learn/supervised_learning/naive_bayes.py
--rw-rw-rw-   0        0        0     4513 2024-06-02 22:11:28.000000 m_o_mini_scikit_learn_ai_project-0.1.0/Mini-Scikit-Learn/supervised_learning/neighbors.py
--rw-rw-rw-   0        0        0     2708 2024-06-02 22:11:28.000000 m_o_mini_scikit_learn_ai_project-0.1.0/Mini-Scikit-Learn/supervised_learning/svm.py
-drwxrwxrwx   0        0        0        0 2024-06-02 23:30:41.923146 m_o_mini_scikit_learn_ai_project-0.1.0/Mini-Scikit-Learn/utilities/
--rw-rw-rw-   0        0        0        0 2024-05-06 10:54:58.000000 m_o_mini_scikit_learn_ai_project-0.1.0/Mini-Scikit-Learn/utilities/__init__.py
--rw-rw-rw-   0        0        0      815 2024-06-02 22:11:28.000000 m_o_mini_scikit_learn_ai_project-0.1.0/Mini-Scikit-Learn/utilities/data_loading.py
--rw-rw-rw-   0        0        0      809 2024-06-02 22:11:28.000000 m_o_mini_scikit_learn_ai_project-0.1.0/Mini-Scikit-Learn/utilities/helpers.py
--rw-rw-rw-   0        0        0     6109 2024-06-02 22:11:28.000000 m_o_mini_scikit_learn_ai_project-0.1.0/Mini-Scikit-Learn/utilities/visualization.py
--rw-rw-rw-   0        0        0     2206 2024-06-02 23:30:41.983948 m_o_mini_scikit_learn_ai_project-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1826 2024-05-06 10:56:06.000000 m_o_mini_scikit_learn_ai_project-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-06-02 23:30:41.982091 m_o_mini_scikit_learn_ai_project-0.1.0/m_o_mini_scikit_learn_ai_project.egg-info/
--rw-rw-rw-   0        0        0     2206 2024-06-02 23:30:40.000000 m_o_mini_scikit_learn_ai_project-0.1.0/m_o_mini_scikit_learn_ai_project.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1491 2024-06-02 23:30:41.000000 m_o_mini_scikit_learn_ai_project-0.1.0/m_o_mini_scikit_learn_ai_project.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 23:30:40.000000 m_o_mini_scikit_learn_ai_project-0.1.0/m_o_mini_scikit_learn_ai_project.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-06-02 23:30:41.000000 m_o_mini_scikit_learn_ai_project-0.1.0/m_o_mini_scikit_learn_ai_project.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-06-02 23:30:41.000000 m_o_mini_scikit_learn_ai_project-0.1.0/m_o_mini_scikit_learn_ai_project.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-06-02 23:30:41.986454 m_o_mini_scikit_learn_ai_project-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      621 2024-06-02 23:28:25.000000 m_o_mini_scikit_learn_ai_project-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 00:17:22.729069 m_o_mini_scikit_learn_ai_project-0.1.1/
+-rw-rw-rw-   0        0        0     2216 2024-06-03 00:17:22.724633 m_o_mini_scikit_learn_ai_project-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1826 2024-05-06 10:56:06.000000 m_o_mini_scikit_learn_ai_project-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-06-03 00:17:22.603927 m_o_mini_scikit_learn_ai_project-0.1.1/m-o-mini-scikit-learn-ai-project/
+-rw-rw-rw-   0        0        0        0 2024-06-02 23:11:21.000000 m_o_mini_scikit_learn_ai_project-0.1.1/m-o-mini-scikit-learn-ai-project/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 00:17:22.613448 m_o_mini_scikit_learn_ai_project-0.1.1/m-o-mini-scikit-learn-ai-project/base/
+-rw-rw-rw-   0        0        0        0 2024-05-06 10:54:58.000000 m_o_mini_scikit_learn_ai_project-0.1.1/m-o-mini-scikit-learn-ai-project/base/__init__.py
+-rw-rw-rw-   0        0        0     2778 2024-06-02 22:11:28.000000 m_o_mini_scikit_learn_ai_project-0.1.1/m-o-mini-scikit-learn-ai-project/base/estimator.py
+-rw-rw-rw-   0        0        0     4291 2024-06-02 22:11:28.000000 m_o_mini_scikit_learn_ai_project-0.1.1/m-o-mini-scikit-learn-ai-project/base/predictor.py
+-rw-rw-rw-   0        0        0     3295 2024-06-02 22:11:28.000000 m_o_mini_scikit_learn_ai_project-0.1.1/m-o-mini-scikit-learn-ai-project/base/transformer.py
+drwxrwxrwx   0        0        0        0 2024-06-03 00:17:22.629682 m_o_mini_scikit_learn_ai_project-0.1.1/m-o-mini-scikit-learn-ai-project/model_selection_and_evaluation/
+-rw-rw-rw-   0        0        0        0 2024-05-06 10:54:58.000000 m_o_mini_scikit_learn_ai_project-0.1.1/m-o-mini-scikit-learn-ai-project/model_selection_and_evaluation/__init__.py
+-rw-rw-rw-   0        0        0     4483 2024-06-02 22:11:28.000000 m_o_mini_scikit_learn_ai_project-0.1.1/m-o-mini-scikit-learn-ai-project/model_selection_and_evaluation/cross_validation.py
+-rw-rw-rw-   0        0        0     4493 2024-06-02 22:11:28.000000 m_o_mini_scikit_learn_ai_project-0.1.1/m-o-mini-scikit-learn-ai-project/model_selection_and_evaluation/grid_search.py
+-rw-rw-rw-   0        0        0     3745 2024-06-02 22:11:28.000000 m_o_mini_scikit_learn_ai_project-0.1.1/m-o-mini-scikit-learn-ai-project/model_selection_and_evaluation/performance_metrics.py
+-rw-rw-rw-   0        0        0     1116 2024-05-13 14:04:21.000000 m_o_mini_scikit_learn_ai_project-0.1.1/m-o-mini-scikit-learn-ai-project/model_selection_and_evaluation/train_test_split.py
+drwxrwxrwx   0        0        0        0 2024-06-03 00:17:22.645130 m_o_mini_scikit_learn_ai_project-0.1.1/m-o-mini-scikit-learn-ai-project/neural_networks/
+-rw-rw-rw-   0        0        0        0 2024-05-06 10:54:58.000000 m_o_mini_scikit_learn_ai_project-0.1.1/m-o-mini-scikit-learn-ai-project/neural_networks/__init__.py
+-rw-rw-rw-   0        0        0     2259 2024-06-02 22:11:28.000000 m_o_mini_scikit_learn_ai_project-0.1.1/m-o-mini-scikit-learn-ai-project/neural_networks/baseNeu.py
+-rw-rw-rw-   0        0        0     6891 2024-06-02 22:11:28.000000 m_o_mini_scikit_learn_ai_project-0.1.1/m-o-mini-scikit-learn-ai-project/neural_networks/convolutional_neural_networks.py
+-rw-rw-rw-   0        0        0     3192 2024-06-02 22:11:28.000000 m_o_mini_scikit_learn_ai_project-0.1.1/m-o-mini-scikit-learn-ai-project/neural_networks/perceptron.py
+drwxrwxrwx   0        0        0        0 2024-06-03 00:17:22.662572 m_o_mini_scikit_learn_ai_project-0.1.1/m-o-mini-scikit-learn-ai-project/supervised_learning/
+-rw-rw-rw-   0        0        0        0 2024-05-09 14:15:32.000000 m_o_mini_scikit_learn_ai_project-0.1.1/m-o-mini-scikit-learn-ai-project/supervised_learning/__init__.py
+-rw-rw-rw-   0        0        0     7356 2024-06-02 22:11:28.000000 m_o_mini_scikit_learn_ai_project-0.1.1/m-o-mini-scikit-learn-ai-project/supervised_learning/decision_trees.py
+-rw-rw-rw-   0        0        0     4715 2024-06-02 22:11:28.000000 m_o_mini_scikit_learn_ai_project-0.1.1/m-o-mini-scikit-learn-ai-project/supervised_learning/linear_models.py
+-rw-rw-rw-   0        0        0     2547 2024-06-02 22:11:28.000000 m_o_mini_scikit_learn_ai_project-0.1.1/m-o-mini-scikit-learn-ai-project/supervised_learning/naive_bayes.py
+-rw-rw-rw-   0        0        0     4513 2024-06-02 22:11:28.000000 m_o_mini_scikit_learn_ai_project-0.1.1/m-o-mini-scikit-learn-ai-project/supervised_learning/neighbors.py
+-rw-rw-rw-   0        0        0     2708 2024-06-02 22:11:28.000000 m_o_mini_scikit_learn_ai_project-0.1.1/m-o-mini-scikit-learn-ai-project/supervised_learning/svm.py
+drwxrwxrwx   0        0        0        0 2024-06-03 00:17:22.675774 m_o_mini_scikit_learn_ai_project-0.1.1/m-o-mini-scikit-learn-ai-project/utilities/
+-rw-rw-rw-   0        0        0        0 2024-05-06 10:54:58.000000 m_o_mini_scikit_learn_ai_project-0.1.1/m-o-mini-scikit-learn-ai-project/utilities/__init__.py
+-rw-rw-rw-   0        0        0      815 2024-06-02 22:11:28.000000 m_o_mini_scikit_learn_ai_project-0.1.1/m-o-mini-scikit-learn-ai-project/utilities/data_loading.py
+-rw-rw-rw-   0        0        0      809 2024-06-02 22:11:28.000000 m_o_mini_scikit_learn_ai_project-0.1.1/m-o-mini-scikit-learn-ai-project/utilities/helpers.py
+-rw-rw-rw-   0        0        0     6109 2024-06-02 22:11:28.000000 m_o_mini_scikit_learn_ai_project-0.1.1/m-o-mini-scikit-learn-ai-project/utilities/visualization.py
+drwxrwxrwx   0        0        0        0 2024-06-03 00:17:22.722656 m_o_mini_scikit_learn_ai_project-0.1.1/m_o_mini_scikit_learn_ai_project.egg-info/
+-rw-rw-rw-   0        0        0     2216 2024-06-03 00:17:22.000000 m_o_mini_scikit_learn_ai_project-0.1.1/m_o_mini_scikit_learn_ai_project.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1851 2024-06-03 00:17:22.000000 m_o_mini_scikit_learn_ai_project-0.1.1/m_o_mini_scikit_learn_ai_project.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 00:17:22.000000 m_o_mini_scikit_learn_ai_project-0.1.1/m_o_mini_scikit_learn_ai_project.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-06-03 00:17:22.000000 m_o_mini_scikit_learn_ai_project-0.1.1/m_o_mini_scikit_learn_ai_project.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       33 2024-06-03 00:17:22.000000 m_o_mini_scikit_learn_ai_project-0.1.1/m_o_mini_scikit_learn_ai_project.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-03 00:17:22.729444 m_o_mini_scikit_learn_ai_project-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      621 2024-06-03 00:16:52.000000 m_o_mini_scikit_learn_ai_project-0.1.1/setup.py
```

### Comparing `m_o_mini_scikit_learn_ai_project-0.1.0/Mini-Scikit-Learn/base/estimator.py` & `m_o_mini_scikit_learn_ai_project-0.1.1/m-o-mini-scikit-learn-ai-project/base/estimator.py`

 * *Files identical despite different names*

### Comparing `m_o_mini_scikit_learn_ai_project-0.1.0/Mini-Scikit-Learn/base/predictor.py` & `m_o_mini_scikit_learn_ai_project-0.1.1/m-o-mini-scikit-learn-ai-project/base/predictor.py`

 * *Files identical despite different names*

### Comparing `m_o_mini_scikit_learn_ai_project-0.1.0/Mini-Scikit-Learn/base/transformer.py` & `m_o_mini_scikit_learn_ai_project-0.1.1/m-o-mini-scikit-learn-ai-project/base/transformer.py`

 * *Files identical despite different names*

### Comparing `m_o_mini_scikit_learn_ai_project-0.1.0/Mini-Scikit-Learn/model_selection_and_evaluation/cross_validation.py` & `m_o_mini_scikit_learn_ai_project-0.1.1/m-o-mini-scikit-learn-ai-project/model_selection_and_evaluation/cross_validation.py`

 * *Files identical despite different names*

### Comparing `m_o_mini_scikit_learn_ai_project-0.1.0/Mini-Scikit-Learn/model_selection_and_evaluation/grid_search.py` & `m_o_mini_scikit_learn_ai_project-0.1.1/m-o-mini-scikit-learn-ai-project/model_selection_and_evaluation/grid_search.py`

 * *Files identical despite different names*

### Comparing `m_o_mini_scikit_learn_ai_project-0.1.0/Mini-Scikit-Learn/model_selection_and_evaluation/performance_metrics.py` & `m_o_mini_scikit_learn_ai_project-0.1.1/m-o-mini-scikit-learn-ai-project/model_selection_and_evaluation/performance_metrics.py`

 * *Files identical despite different names*

### Comparing `m_o_mini_scikit_learn_ai_project-0.1.0/Mini-Scikit-Learn/model_selection_and_evaluation/train_test_split.py` & `m_o_mini_scikit_learn_ai_project-0.1.1/m-o-mini-scikit-learn-ai-project/model_selection_and_evaluation/train_test_split.py`

 * *Files identical despite different names*

### Comparing `m_o_mini_scikit_learn_ai_project-0.1.0/Mini-Scikit-Learn/neural_networks/baseNeu.py` & `m_o_mini_scikit_learn_ai_project-0.1.1/m-o-mini-scikit-learn-ai-project/neural_networks/baseNeu.py`

 * *Files identical despite different names*

### Comparing `m_o_mini_scikit_learn_ai_project-0.1.0/Mini-Scikit-Learn/neural_networks/convolutional_neural_networks.py` & `m_o_mini_scikit_learn_ai_project-0.1.1/m-o-mini-scikit-learn-ai-project/neural_networks/convolutional_neural_networks.py`

 * *Files identical despite different names*

### Comparing `m_o_mini_scikit_learn_ai_project-0.1.0/Mini-Scikit-Learn/neural_networks/perceptron.py` & `m_o_mini_scikit_learn_ai_project-0.1.1/m-o-mini-scikit-learn-ai-project/neural_networks/perceptron.py`

 * *Files identical despite different names*

### Comparing `m_o_mini_scikit_learn_ai_project-0.1.0/Mini-Scikit-Learn/supervised_learning/decision_trees.py` & `m_o_mini_scikit_learn_ai_project-0.1.1/m-o-mini-scikit-learn-ai-project/supervised_learning/decision_trees.py`

 * *Files identical despite different names*

### Comparing `m_o_mini_scikit_learn_ai_project-0.1.0/Mini-Scikit-Learn/supervised_learning/linear_models.py` & `m_o_mini_scikit_learn_ai_project-0.1.1/m-o-mini-scikit-learn-ai-project/supervised_learning/linear_models.py`

 * *Files identical despite different names*

### Comparing `m_o_mini_scikit_learn_ai_project-0.1.0/Mini-Scikit-Learn/supervised_learning/naive_bayes.py` & `m_o_mini_scikit_learn_ai_project-0.1.1/m-o-mini-scikit-learn-ai-project/supervised_learning/naive_bayes.py`

 * *Files identical despite different names*

### Comparing `m_o_mini_scikit_learn_ai_project-0.1.0/Mini-Scikit-Learn/supervised_learning/neighbors.py` & `m_o_mini_scikit_learn_ai_project-0.1.1/m-o-mini-scikit-learn-ai-project/supervised_learning/neighbors.py`

 * *Files identical despite different names*

### Comparing `m_o_mini_scikit_learn_ai_project-0.1.0/Mini-Scikit-Learn/supervised_learning/svm.py` & `m_o_mini_scikit_learn_ai_project-0.1.1/m-o-mini-scikit-learn-ai-project/supervised_learning/svm.py`

 * *Files identical despite different names*

### Comparing `m_o_mini_scikit_learn_ai_project-0.1.0/Mini-Scikit-Learn/utilities/data_loading.py` & `m_o_mini_scikit_learn_ai_project-0.1.1/m-o-mini-scikit-learn-ai-project/utilities/data_loading.py`

 * *Files identical despite different names*

### Comparing `m_o_mini_scikit_learn_ai_project-0.1.0/Mini-Scikit-Learn/utilities/helpers.py` & `m_o_mini_scikit_learn_ai_project-0.1.1/m-o-mini-scikit-learn-ai-project/utilities/helpers.py`

 * *Files identical despite different names*

### Comparing `m_o_mini_scikit_learn_ai_project-0.1.0/Mini-Scikit-Learn/utilities/visualization.py` & `m_o_mini_scikit_learn_ai_project-0.1.1/m-o-mini-scikit-learn-ai-project/utilities/visualization.py`

 * *Files identical despite different names*

### Comparing `m_o_mini_scikit_learn_ai_project-0.1.0/PKG-INFO` & `m_o_mini_scikit_learn_ai_project-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: m_o_mini_scikit_learn_ai_project
-Version: 0.1.0
-Summary: A mini implementation of scikit-learn with various machine learning models and utilities.
-Home-page: https://github.com/mahatun/Mini-Scikit-Learn.git
-Author: Maha,Oumaima
-Author-email: maha.hanif@um6p.ma
-License: UNKNOWN
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-
 # Lightweight Machine Learning Library
 
 ## Overview
 
 This project aims to create a lightweight machine learning library inspired by the architecture of scikit-learn. The library provides users with powerful and easy-to-use tools for building machine learning models and analyzing data. It emphasizes modularity, ease of use, and efficient implementation.
 
 ## Features
@@ -27,9 +16,7 @@
 
 ## Installation
 
 You can install the library using pip:
 
 ```bash
 pip install lightweight-ml
-
-
```

### Comparing `m_o_mini_scikit_learn_ai_project-0.1.0/README.md` & `m_o_mini_scikit_learn_ai_project-0.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: m-o-mini-scikit-learn-ai-project
+Version: 0.1.1
+Summary: A mini implementation of scikit-learn with various machine learning models and utilities.
+Home-page: https://github.com/mahatun/Mini-Scikit-Learn.git
+Author: Maha,Oumaima
+Author-email: maha.hanif@um6p.ma
+Description-Content-Type: text/markdown
+Requires-Dist: numpy
+Requires-Dist: scikit-learn
+
 # Lightweight Machine Learning Library
 
 ## Overview
 
 This project aims to create a lightweight machine learning library inspired by the architecture of scikit-learn. The library provides users with powerful and easy-to-use tools for building machine learning models and analyzing data. It emphasizes modularity, ease of use, and efficient implementation.
 
 ## Features
```

### Comparing `m_o_mini_scikit_learn_ai_project-0.1.0/m_o_mini_scikit_learn_ai_project.egg-info/PKG-INFO` & `m_o_mini_scikit_learn_ai_project-0.1.1/m_o_mini_scikit_learn_ai_project.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: m-o-mini-scikit-learn-ai-project
-Version: 0.1.0
+Version: 0.1.1
 Summary: A mini implementation of scikit-learn with various machine learning models and utilities.
 Home-page: https://github.com/mahatun/Mini-Scikit-Learn.git
 Author: Maha,Oumaima
 Author-email: maha.hanif@um6p.ma
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+Requires-Dist: numpy
+Requires-Dist: scikit-learn
 
 # Lightweight Machine Learning Library
 
 ## Overview
 
 This project aims to create a lightweight machine learning library inspired by the architecture of scikit-learn. The library provides users with powerful and easy-to-use tools for building machine learning models and analyzing data. It emphasizes modularity, ease of use, and efficient implementation.
 
@@ -27,9 +27,7 @@
 
 ## Installation
 
 You can install the library using pip:
 
 ```bash
 pip install lightweight-ml
-
-
```

### Comparing `m_o_mini_scikit_learn_ai_project-0.1.0/setup.py` & `m_o_mini_scikit_learn_ai_project-0.1.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
-    name='m_o_mini_scikit_learn_ai_project', 
-    version='0.1.0',
+    name='m-o-mini-scikit-learn-ai-project', 
+    version='0.1.1',
     packages=find_packages(),
     install_requires=[
         'numpy',
         'scikit-learn',
         # Add any other dependencies here
     ],
     author='Maha,Oumaima',
```

