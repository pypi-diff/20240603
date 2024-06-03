# Comparing `tmp/mambular-0.1.2.tar.gz` & `tmp/mambular-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mambular-0.1.2.tar", last modified: Sat May 25 18:55:30 2024, max compression
+gzip compressed data, was "mambular-0.1.3.tar", last modified: Mon Jun  3 13:27:18 2024, max compression
```

## Comparing `mambular-0.1.2.tar` & `mambular-0.1.3.tar`

### file list

```diff
@@ -1,42 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-05-25 18:55:30.454741 mambular-0.1.2/
--rw-rw-rw-   0        0        0      472 2024-05-25 18:55:30.454741 mambular-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     9597 2024-05-25 09:48:17.000000 mambular-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-25 18:55:30.326325 mambular-0.1.2/mambular/
--rw-rw-rw-   0        0        0      158 2024-05-25 18:41:38.000000 mambular-0.1.2/mambular/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-25 18:55:30.384445 mambular-0.1.2/mambular/base_models/
--rw-rw-rw-   0        0        0        0 2024-05-25 18:42:36.000000 mambular-0.1.2/mambular/base_models/__init__.py
--rw-rw-rw-   0        0        0    14504 2024-05-25 09:48:18.000000 mambular-0.1.2/mambular/base_models/classifier.py
--rw-rw-rw-   0        0        0    12529 2024-05-25 09:48:18.000000 mambular-0.1.2/mambular/base_models/distributional.py
--rw-rw-rw-   0        0        0    16034 2024-05-25 09:48:18.000000 mambular-0.1.2/mambular/base_models/embedding_classifier.py
--rw-rw-rw-   0        0        0    14066 2024-05-25 18:41:38.000000 mambular-0.1.2/mambular/base_models/embedding_regressor.py
--rw-rw-rw-   0        0        0    11172 2024-05-25 09:48:18.000000 mambular-0.1.2/mambular/base_models/regressor.py
-drwxrwxrwx   0        0        0        0 2024-05-25 18:55:30.408720 mambular-0.1.2/mambular/models/
--rw-rw-rw-   0        0        0      291 2024-05-25 18:41:38.000000 mambular-0.1.2/mambular/models/__init__.py
--rw-rw-rw-   0        0        0    22513 2024-05-25 09:48:18.000000 mambular-0.1.2/mambular/models/sklearn_classifier.py
--rw-rw-rw-   0        0        0    21208 2024-05-25 09:48:18.000000 mambular-0.1.2/mambular/models/sklearn_distributional.py
--rw-rw-rw-   0        0        0    22109 2024-05-25 09:48:18.000000 mambular-0.1.2/mambular/models/sklearn_embedding_classifier.py
--rw-rw-rw-   0        0        0    20043 2024-05-25 09:48:18.000000 mambular-0.1.2/mambular/models/sklearn_embedding_regressor.py
--rw-rw-rw-   0        0        0    19287 2024-05-25 09:48:18.000000 mambular-0.1.2/mambular/models/sklearn_regressor.py
-drwxrwxrwx   0        0        0        0 2024-05-25 18:55:30.435336 mambular-0.1.2/mambular/utils/
--rw-rw-rw-   0        0        0        0 2024-05-06 13:10:41.000000 mambular-0.1.2/mambular/utils/__init__.py
--rw-rw-rw-   0        0        0     6041 2024-05-06 13:10:41.000000 mambular-0.1.2/mambular/utils/config.py
--rw-rw-rw-   0        0        0     5081 2024-05-06 13:10:41.000000 mambular-0.1.2/mambular/utils/dataset.py
--rw-rw-rw-   0        0        0     1556 2024-05-06 13:10:41.000000 mambular-0.1.2/mambular/utils/distributional_metrics.py
--rw-rw-rw-   0        0        0    20476 2024-05-06 13:10:41.000000 mambular-0.1.2/mambular/utils/distributions.py
--rw-rw-rw-   0        0        0     5199 2024-05-06 13:10:41.000000 mambular-0.1.2/mambular/utils/mamba_arch.py
--rw-rw-rw-   0        0        0     5230 2024-05-06 13:10:41.000000 mambular-0.1.2/mambular/utils/normalization_layers.py
--rw-rw-rw-   0        0        0    23099 2024-05-06 13:10:41.000000 mambular-0.1.2/mambular/utils/preprocessor.py
-drwxrwxrwx   0        0        0        0 2024-05-25 18:55:30.364507 mambular-0.1.2/mambular.egg-info/
--rw-rw-rw-   0        0        0      472 2024-05-25 18:55:30.000000 mambular-0.1.2/mambular.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1040 2024-05-25 18:55:30.000000 mambular-0.1.2/mambular.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-25 18:55:30.000000 mambular-0.1.2/mambular.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      105 2024-05-25 18:55:30.000000 mambular-0.1.2/mambular.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-25 18:55:30.000000 mambular-0.1.2/mambular.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-25 18:55:30.456115 mambular-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      991 2024-05-25 18:54:46.000000 mambular-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-25 18:55:30.451340 mambular-0.1.2/tests/
--rw-rw-rw-   0        0        0     4750 2024-05-06 13:10:41.000000 mambular-0.1.2/tests/test_classifier.py
--rw-rw-rw-   0        0        0    15165 2024-05-06 13:10:41.000000 mambular-0.1.2/tests/test_distributions.py
--rw-rw-rw-   0        0        0     4988 2024-05-06 13:10:41.000000 mambular-0.1.2/tests/test_lss.py
--rw-rw-rw-   0        0        0     3044 2024-05-06 13:10:41.000000 mambular-0.1.2/tests/test_preprocessor.py
--rw-rw-rw-   0        0        0     4079 2024-05-06 13:10:41.000000 mambular-0.1.2/tests/test_regressor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:27:18.746329 mambular-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-06-03 13:26:58.000000 mambular-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11681 2024-06-03 13:27:18.746329 mambular-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9737 2024-06-03 13:26:58.000000 mambular-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:27:18.742329 mambular-0.1.3/mambular/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-06-03 13:26:58.000000 mambular-0.1.3/mambular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-06-03 13:26:58.000000 mambular-0.1.3/mambular/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:27:18.742329 mambular-0.1.3/mambular/base_models/
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-06-03 13:26:58.000000 mambular-0.1.3/mambular/base_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15918 2024-06-03 13:26:58.000000 mambular-0.1.3/mambular/base_models/classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14669 2024-06-03 13:26:58.000000 mambular-0.1.3/mambular/base_models/distributional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18836 2024-06-03 13:26:58.000000 mambular-0.1.3/mambular/base_models/embedding_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16010 2024-06-03 13:26:58.000000 mambular-0.1.3/mambular/base_models/embedding_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12748 2024-06-03 13:26:58.000000 mambular-0.1.3/mambular/base_models/regressor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:27:18.746329 mambular-0.1.3/mambular/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-06-03 13:26:58.000000 mambular-0.1.3/mambular/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26795 2024-06-03 13:26:58.000000 mambular-0.1.3/mambular/models/sklearn_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25150 2024-06-03 13:26:58.000000 mambular-0.1.3/mambular/models/sklearn_distributional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26701 2024-06-03 13:26:58.000000 mambular-0.1.3/mambular/models/sklearn_embedding_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24375 2024-06-03 13:26:58.000000 mambular-0.1.3/mambular/models/sklearn_embedding_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23181 2024-06-03 13:26:58.000000 mambular-0.1.3/mambular/models/sklearn_regressor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:27:18.746329 mambular-0.1.3/mambular/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-06-03 13:26:58.000000 mambular-0.1.3/mambular/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-06-03 13:26:58.000000 mambular-0.1.3/mambular/utils/configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5299 2024-06-03 13:26:58.000000 mambular-0.1.3/mambular/utils/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-06-03 13:26:58.000000 mambular-0.1.3/mambular/utils/distributional_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21258 2024-06-03 13:26:58.000000 mambular-0.1.3/mambular/utils/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8137 2024-06-03 13:26:58.000000 mambular-0.1.3/mambular/utils/mamba_arch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7689 2024-06-03 13:26:58.000000 mambular-0.1.3/mambular/utils/mlp_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5228 2024-06-03 13:26:58.000000 mambular-0.1.3/mambular/utils/normalization_layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5386 2024-06-03 13:26:58.000000 mambular-0.1.3/mambular/utils/ple_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6723 2024-06-03 13:26:58.000000 mambular-0.1.3/mambular/utils/prepro_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21917 2024-06-03 13:26:58.000000 mambular-0.1.3/mambular/utils/preprocessor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:27:18.742329 mambular-0.1.3/mambular.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11681 2024-06-03 13:27:16.000000 mambular-0.1.3/mambular.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-06-03 13:27:18.000000 mambular-0.1.3/mambular.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 13:27:16.000000 mambular-0.1.3/mambular.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-06-03 13:27:16.000000 mambular-0.1.3/mambular.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-06-03 13:27:16.000000 mambular-0.1.3/mambular.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 13:27:18.746329 mambular-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-06-03 13:26:58.000000 mambular-0.1.3/setup.py
```

### Comparing `mambular-0.1.2/README.md` & `mambular-0.1.3/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,142 +1,159 @@
-# Mambular: Tabular Deep Learning with Mamba Architectures
-
-Mambular is a Python package that brings the power of Mamba architectures to tabular data, offering a suite of deep learning models for regression, classification, and distributional regression tasks. Designed with ease of use in mind, Mambular models adhere to scikit-learn's `BaseEstimator` interface, making them highly compatible with the familiar scikit-learn ecosystem. This means you can fit, predict, and transform using Mambular models just as you would with any traditional scikit-learn model, but with the added performance and flexibility of deep learning.
-
-<img src="https://github.com/basf/mamba-tabular/blob/documentation/Mamba_Tabular_Converted.jpg" alt="Mamba Tabular" width="400"/>
-
-## Features
-
-- **Comprehensive Model Suite**: Includes modules for regression (`MambularRegressor`), classification (`MambularClassifier`), and distributional regression (`MambularLSS`), catering to a wide range of tabular data tasks.
-- **State-of-the-Art Architectures**: Leverages the Mamba architecture, known for its effectiveness in handling sequential and time-series data within a state-space modeling framework, adapted here for tabular data.
-- **Seamless Integration**: Designed to work effortlessly with scikit-learn, allowing for easy inclusion in existing machine learning pipelines, cross-validation, and hyperparameter tuning workflows.
-- **Extensive Preprocessing**: Comes with a powerful preprocessing module that supports a broad array of data transformation techniques, ensuring that your data is optimally prepared for model training.
-- **Sklearn-like API**: The familiar scikit-learn `fit`, `predict`, and `predict_proba` methods mean minimal learning curve for those already accustomed to scikit-learn.
-- **PyTorch Lightning Under the Hood**: Built on top of PyTorch Lightning, Mambular models benefit from streamlined training processes, easy customization, and advanced features like distributed training and 16-bit precision.
-
-## Documentation
-
-You can find the Mamba-Tabular API documentation [here](https://mamba-tabular.readthedocs.io/en/latest/index.html).
-
-## Installation
-
-Install Mambular using pip:
-```sh
-pip install mambular
-```
-
-## Advanced Preprocessing for Optimal Performance
-
-Mambular elevates the preprocessing stage of model development, employing a sophisticated suite of techniques to ensure your data is in the best shape for the Mamba architectures. Our preprocessing module is designed to be both powerful and intuitive, offering a range of options to transform your tabular data efficiently.
-
-### Intelligent Data Type Detection and Transformation
-
-Mambular automatically identifies the type of each feature in your dataset, applying the most suitable transformations to numerical and categorical variables. This includes:
-
-- **Ordinal Encoding**: Categorical features are seamlessly transformed into numerical values, preserving their inherent order and making them model-ready.
-- **One-Hot Encoding**: For nominal data, Mambular employs one-hot encoding to capture the presence or absence of categories without imposing ordinality.
-- **Binning**: Numerical features can be discretized into bins, a useful technique for handling continuous variables in certain modeling contexts.
-- **Decision Tree Binning**: Optionally, Mambular can use decision trees to find the optimal binning strategy for numerical features, enhancing model interpretability and performance.
-- **Normalization**: Mambular can easily handle numerical features without specifically turning them into categorical features. Standard preprocessing steps such as normalization per feature are possible
-- **Standardization**: Similarly, Standardization instead of Normalization can be used.
-
-
-### Handling Missing Values
-
-Our preprocessing pipeline gracefully handles missing data, employing strategies like mean imputation for numerical features and mode imputation for categorical ones, ensuring that your models receive complete data inputs without manual intervention.
-
-### Flexible and Customizable
-
-While Mambular excels in automating the preprocessing workflow, it also offers flexibility. You can customize the preprocessing steps to fit the unique needs of your dataset, ensuring that you're not locked into a one-size-fits-all approach.
-
-By integrating Mambular's preprocessing module into your workflow, you're not just preparing your data for deep learning; you're optimizing it for excellence. This commitment to data quality is what sets Mambular apart, making it an indispensable tool in your machine learning arsenal.
-
-
-## Fit a Model
-Fitting a model in mambular is as simple as it gets. All models in mambular are sklearn BaseEstimators. Thus the `.fit` method is implemented for all of them. Additionally, this allows for using all other sklearn inherent methods such as their built in hyperparameter optimization tools.
-
-```python
-from mambular.models import MambularClassifier
-# Initialize and fit your model
-model = MambularClassifier(
-    dropout=0.01,
-    d_model=128,
-    n_layers=6,
-    numerical_preprocessing="normalization",
-)
-
-# X can be a dataframe or something that can be easily transformed into a pd.DataFrame as a np.array
-model.fit(X, y, max_epochs=500, lr=1e-03, patience=25)
-```
-
-Predictions are also easily obtained:
-```python
-# simple predictions
-preds = model.predict(X)
-
-# Predict probabilities
-preds = model.predict_proba(X)
-```
-
-
-## Distributional Regression with MambularLSS
-
-Mambular introduces a cutting-edge approach to distributional regression through its `MambularLSS` module, empowering users to model the full distribution of a response variable, not just its mean. This method is particularly valuable in scenarios where understanding the variability, skewness, or kurtosis of the response distribution is as crucial as predicting its central tendency.
-
-### Key Features of MambularLSS:
-
-- **Full Distribution Modeling**: Unlike traditional regression models that predict a single value (e.g., the mean), `MambularLSS` models the entire distribution of the response variable. This allows for more informative predictions, including quantiles, variance, and higher moments.
-- **Customizable Distribution Types**: `MambularLSS` supports a variety of distribution families (e.g., Gaussian, Poisson, Binomial), making it adaptable to different types of response variables, from continuous to count data.
-- **Location, Scale, Shape Parameters**: The model predicts parameters corresponding to the location, scale, and shape of the distribution, offering a nuanced understanding of the data's underlying distributional characteristics.
-- **Enhanced Predictive Uncertainty**: By modeling the full distribution, `MambularLSS` provides richer information on predictive uncertainty, enabling more robust decision-making processes in uncertain environments.
-
-
-### Available Distribution Classes:
-
-`MambularLSS` offers a wide range of distribution classes to cater to various statistical modeling needs. The available distribution classes include:
-
-- `normal`: Normal Distribution for modeling continuous data with a symmetric distribution around the mean.
-- `poisson`: Poisson Distribution for modeling count data that for instance represent the number of events occurring within a fixed interval.
-- `gamma`: Gamma Distribution for modeling continuous data that is skewed and bounded at zero, often used for waiting times.
-- `beta`: Beta Distribution for modeling data that is bounded between 0 and 1, useful for proportions and percentages.
-- `dirichlet`: Dirichlet Distribution for modeling multivariate data where individual components are correlated, and the sum is constrained to 1.
-- `studentt`: Student's T-Distribution for modeling data with heavier tails than the normal distribution, useful when the sample size is small.
-- `negativebinom`: Negative Binomial Distribution for modeling count data with over-dispersion relative to the Poisson distribution.
-- `inversegamma`: Inverse Gamma Distribution, often used as a prior distribution in Bayesian inference for scale parameters.
-- `categorical`: Categorical Distribution for modeling categorical data with more than two categories.
-
-These distribution classes allow `MambularLSS` to flexibly model a wide variety of data types and distributions, providing users with the tools needed to capture the full complexity of their data.
-
-
-### Use Cases for MambularLSS:
-
-- **Risk Assessment**: In finance or insurance, understanding the range and likelihood of potential losses is as important as predicting average outcomes.
-- **Demand Forecasting**: For inventory management, capturing the variability in product demand helps in optimizing stock levels.
-- **Personalized Medicine**: In healthcare, distributional regression can predict a range of possible patient responses to a treatment, aiding in personalized therapy planning.
-
-### Getting Started with MambularLSS:
-
-To integrate distributional regression into your workflow with `MambularLSS`, start by initializing the model with your desired configuration, similar to other Mambular models:
-
-```python
-from mambular.models import MambularLSS
-
-# Initialize the MambularLSS model
-model = MambularLSS(
-    dropout=0.2,
-    d_model=256,
-    n_layers=4,
- 
-)
-
-# Fit the model to your data
-model.fit(
-    X, 
-    y, 
-    max_epochs=300, 
-    lr=1e-03, 
-    patience=10,     
-    family="normal" # define your distribution
-    )
-
-```
-
+<div align="center">
+  <img src="./docs/images/logo/mamba_tabular.jpg" width="400"/>
+
+
+[![PyPI](https://img.shields.io/pypi/v/mambular)](https://pypi.org/project/mambular)
+![PyPI - Downloads](https://img.shields.io/pypi/dw/mambular)
+[![docs build](https://readthedocs.org/projects/mambular/badge/?version=latest)](https://mambular.readthedocs.io/en/latest/?badge=latest)
+[![docs](https://img.shields.io/badge/docs-latest-blue)](https://mambular.readthedocs.io/en/latest/)
+[![open issues](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/basf/mamba-tabular/issues)
+
+
+[📘Documentation](https://mambular.readthedocs.io/en/latest/index.html) |
+[🛠️Installation](https://mambular.readthedocs.io/en/latest/installation.html) |
+[Models](https://mambular.readthedocs.io/en/latest/api/models/index.html) |
+[🤔Report Issues](https://github.com/basf/mamba-tabular/issues)
+</div>
+
+# Mambular: Tabular Deep Learning with Mamba Architectures
+
+Mambular is a Python package that brings the power of Mamba architectures to tabular data, offering a suite of deep learning models for regression, classification, and distributional regression tasks. Designed with ease of use in mind, Mambular models adhere to scikit-learn's `BaseEstimator` interface, making them highly compatible with the familiar scikit-learn ecosystem. This means you can fit, predict, and evaluate using Mambular models just as you would with any traditional scikit-learn model, but with the added performance and flexibility of deep learning.
+
+## Features
+
+- **Comprehensive Model Suite**: Includes modules for regression (`MambularRegressor`), classification (`MambularClassifier`), and distributional regression (`MambularLSS`), catering to a wide range of tabular data tasks.
+- **State-of-the-Art Architectures**: Leverages the Mamba architecture, known for its effectiveness in handling sequential and time-series data within a state-space modeling framework, adapted here for tabular data.
+- **Seamless Integration**: Designed to work effortlessly with scikit-learn, allowing for easy inclusion in existing machine learning pipelines, cross-validation, and hyperparameter tuning workflows.
+- **Extensive Preprocessing**: Comes with a powerful preprocessing module that supports a broad array of data transformation techniques, ensuring that your data is optimally prepared for model training.
+- **Sklearn-like API**: The familiar scikit-learn `fit`, `predict`, and `predict_proba` methods mean minimal learning curve for those already accustomed to scikit-learn.
+- **PyTorch Lightning Under the Hood**: Built on top of PyTorch Lightning, Mambular models benefit from streamlined training processes, easy customization, and advanced features like distributed training and 16-bit precision.
+
+## Documentation
+
+You can find the Mamba-Tabular API documentation [here](https://mamba-tabular.readthedocs.io/en/latest/index.html).
+
+## Installation
+
+Install Mambular using pip:
+```sh
+pip install mambular
+```
+
+## Preprocessing
+
+Mambular simplifies the preprocessing stage of model development with a comprehensive set of techniques to prepare your data for Mamba architectures. Our preprocessing module is designed to be both powerful and easy to use, offering a variety of options to efficiently transform your tabular data.
+
+### Data Type Detection and Transformation
+
+Mambular automatically identifies the type of each feature in your dataset and applies the most appropriate transformations for numerical and categorical variables. This includes:
+- **Ordinal Encoding**: Categorical features are seamlessly transformed into numerical values, preserving their inherent order and making them model-ready.
+- **One-Hot Encoding**: For nominal data, Mambular employs one-hot encoding to capture the presence or absence of categories without imposing ordinality.
+- **Binning**: Numerical features can be discretized into bins, a useful technique for handling continuous variables in certain modeling contexts.
+- **Decision Tree Binning**: Optionally, Mambular can use decision trees to find the optimal binning strategy for numerical features, enhancing model interpretability and performance.
+- **Normalization**: Mambular can easily handle numerical features without specifically turning them into categorical features. Standard preprocessing steps such as normalization per feature are possible
+- **Standardization**: Similarly, Standardization instead of Normalization can be used.
+- **PLE**: Periodic Linear Encodings for numerical features can enhance performance for tabular DL methods.
+
+
+### Handling Missing Values
+
+Our preprocessing pipeline effectively handles missing data by using mean imputation for numerical features and mode imputation for categorical features. This ensures that your models receive complete data inputs without needing manual intervention.
+Additionally, Mambular can manage unknown categorical values during inference by incorporating classical <UNK> tokens in categorical preprocessing.
+
+
+## Fit a Model
+Fitting a model in mambular is as simple as it gets. All models in mambular are sklearn BaseEstimators. Thus the `.fit` method is implemented for all of them. Additionally, this allows for using all other sklearn inherent methods such as their built in hyperparameter optimization tools.
+
+```python
+from mambular.models import MambularClassifier
+# Initialize and fit your model
+model = MambularClassifier(
+    d_model=64,
+    n_layers=8,
+    numerical_preprocessing="ple",
+    n_bins=50
+)
+
+# X can be a dataframe or something that can be easily transformed into a pd.DataFrame as a np.array
+model.fit(X, y, max_epochs=150, lr=1e-04)
+```
+
+Predictions are also easily obtained:
+```python
+# simple predictions
+preds = model.predict(X)
+
+# Predict probabilities
+preds = model.predict_proba(X)
+```
+
+
+## Distributional Regression with MambularLSS
+
+Mambular introduces a cutting-edge approach to distributional regression through its `MambularLSS` module, empowering users to model the full distribution of a response variable, not just its mean. This method is particularly valuable in scenarios where understanding the variability, skewness, or kurtosis of the response distribution is as crucial as predicting its central tendency.
+
+### Key Features of MambularLSS:
+
+- **Full Distribution Modeling**: Unlike traditional regression models that predict a single value (e.g., the mean), `MambularLSS` models the entire distribution of the response variable. This allows for more informative predictions, including quantiles, variance, and higher moments.
+- **Customizable Distribution Types**: `MambularLSS` supports a variety of distribution families (e.g., Gaussian, Poisson, Binomial), making it adaptable to different types of response variables, from continuous to count data.
+- **Location, Scale, Shape Parameters**: The model predicts parameters corresponding to the location, scale, and shape of the distribution, offering a nuanced understanding of the data's underlying distributional characteristics.
+- **Enhanced Predictive Uncertainty**: By modeling the full distribution, `MambularLSS` provides richer information on predictive uncertainty, enabling more robust decision-making processes in uncertain environments.
+
+
+### Available Distribution Classes:
+
+`MambularLSS` offers a wide range of distribution classes to cater to various statistical modeling needs. The available distribution classes include:
+
+- `normal`: Normal Distribution for modeling continuous data with a symmetric distribution around the mean.
+- `poisson`: Poisson Distribution for modeling count data that for instance represent the number of events occurring within a fixed interval.
+- `gamma`: Gamma Distribution for modeling continuous data that is skewed and bounded at zero, often used for waiting times.
+- `beta`: Beta Distribution for modeling data that is bounded between 0 and 1, useful for proportions and percentages.
+- `dirichlet`: Dirichlet Distribution for modeling multivariate data where individual components are correlated, and the sum is constrained to 1.
+- `studentt`: Student's T-Distribution for modeling data with heavier tails than the normal distribution, useful when the sample size is small.
+- `negativebinom`: Negative Binomial Distribution for modeling count data with over-dispersion relative to the Poisson distribution.
+- `inversegamma`: Inverse Gamma Distribution, often used as a prior distribution in Bayesian inference for scale parameters.
+- `categorical`: Categorical Distribution for modeling categorical data with more than two categories.
+
+These distribution classes allow `MambularLSS` to flexibly model a wide variety of data types and distributions, providing users with the tools needed to capture the full complexity of their data.
+
+
+### Getting Started with MambularLSS:
+
+To integrate distributional regression into your workflow with `MambularLSS`, start by initializing the model with your desired configuration, similar to other Mambular models:
+
+```python
+from mambular.models import MambularLSS
+
+# Initialize the MambularLSS model
+model = MambularLSS(
+    dropout=0.2,
+    d_model=64,
+    n_layers=8,
+ 
+)
+
+# Fit the model to your data
+model.fit(
+    X, 
+    y, 
+    max_epochs=150, 
+    lr=1e-04, 
+    patience=10,     
+    family="normal" # define your distribution
+    )
+
+```
+
+## Citation
+
+If you find this project useful in your research, please consider cite:
+```BibTeX
+@misc{2024,
+    title={Mambular: Tabular Deep Learning with Mamba Architectures},
+    author={Anton Frederik Thielmann, Manish Kumar, Christoph Weisser, Benjamin Saefken, Soheila Samiee},
+    howpublished = {\url{https://github.com/basf/mamba-tabular}},
+    year={2024}
+}
+```
+
+## License
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mambular-0.1.2/mambular/base_models/classifier.py` & `mambular-0.1.3/mambular/base_models/classifier.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,172 +1,205 @@
+import lightning as pl
 import torch
 import torch.nn as nn
 import torchmetrics
 from ..utils.mamba_arch import Mamba
-from ..utils.config import MambularConfig
-import pytorch_lightning as pl
+from ..utils.mlp_utils import MLP
+from ..utils.normalization_layers import (
+    RMSNorm,
+    LayerNorm,
+    LearnableLayerScaling,
+    BatchNorm,
+    InstanceNorm,
+    GroupNorm,
+)
+from ..utils.configs import DefaultMambularConfig
 
 
 class BaseMambularClassifier(pl.LightningModule):
     """
     A base class for building classification models using the Mambular architecture within the PyTorch Lightning framework.
 
     This class integrates various components such as embeddings for categorical and numerical features, the Mambular model
     for processing sequences of embeddings, and a classification head for prediction. It supports multi-class and binary classification tasks.
 
     Parameters
     ----------
     num_classes : int
-        The number of classes in the classification task. For binary classification, this should be 2.
-    config : MambularConfig
-        An instance of MambularConfig containing configuration parameters for the Mambular model.
-    cat_feature_info : dict, optional
-        A dictionary mapping the names of categorical features to their number of unique categories.
-        This information is used to configure embedding layers for categorical features. Defaults to None.
-    num_feature_info : dict, optional
-        A dictionary mapping the names of numerical features to the size of their input dimensions.
-        This information is used to configure embedding layers for numerical features. Defaults to None.
-    lr : float, optional
-        The learning rate for the optimizer. Defaults to 1e-03.
-    lr_patience : int, optional
-        The number of epochs with no improvement after which learning rate will be reduced. Defaults to 10.
-    weight_decay : float, optional
-        Weight decay (L2 penalty) parameter for the optimizer. Defaults to 0.025.
-    lr_factor : float, optional
-        Factor by which the learning rate will be reduced. Defaults to 0.75.
+        number of classes for classification.
+    cat_feature_info : dict
+        Dictionary containing information about categorical features.
+    num_feature_info : dict
+        Dictionary containing information about numerical features.
+    config : DefaultMambularConfig, optional
+        Configuration object containing default hyperparameters for the model (default is DefaultMambularConfig()).
+    **kwargs : dict
+        Additional keyword arguments.
+
 
     Attributes
     ----------
-    embedding_activation : nn.Module
-        The activation function to be applied after the linear transformation of numerical features.
-    num_embeddings : nn.ModuleList
-        A list of sequential modules, each corresponding to an embedding layer for a numerical feature.
-    cat_embeddings : nn.ModuleList
-        A list of embedding layers, each corresponding to a categorical feature.
+    lr : float
+        Learning rate.
+    lr_patience : int
+        Patience for learning rate scheduler.
+    weight_decay : float
+        Weight decay for optimizer.
+    lr_factor : float
+        Factor by which the learning rate will be reduced.
+    pooling_method : str
+        Method to pool the features.
+    cat_feature_info : dict
+        Dictionary containing information about categorical features.
+    num_feature_info : dict
+        Dictionary containing information about numerical features.
+    embedding_activation : callable
+        Activation function for embeddings.
     mamba : Mamba
-        The Mambular model for processing sequences of embeddings.
+        Mamba architecture component.
     norm_f : nn.Module
-        A normalization layer applied after the Mambular model.
-    tabular_head : nn.Linear
-        A linear layer for predicting the class labels from the aggregated embedding representation.
-    pooling_method : str
-        The method used to aggregate embeddings across features. Supported methods are 'avg', 'max', and 'sum'.
+        Normalization layer.
+    num_embeddings : nn.ModuleList
+        Module list for numerical feature embeddings.
+    cat_embeddings : nn.ModuleList
+        Module list for categorical feature embeddings.
+    tabular_head : MLP
+        Multi-layer perceptron head for tabular data.
+    cls_token : nn.Parameter
+        Class token parameter.
+    embedding_norm : nn.Module, optional
+        Layer normalization applied after embedding if specified.
     loss_fct : nn.Module
         The loss function used for training the model, configured based on the number of classes.
     acc : torchmetrics.Accuracy
         A metric for computing the accuracy of predictions.
     auroc : torchmetrics.AUROC
         A metric for computing the Area Under the Receiver Operating Characteristic curve.
     precision : torchmetrics.Precision
         A metric for computing the precision of predictions.
 
-    Methods
-    -------
-    forward(cat_features, num_features)
-        Defines the forward pass of the model, processing both categorical and numerical features, aggregating embeddings,
-        and producing predictions.
-    training_step(batch, batch_idx)
-        Performs a single training step, computing the loss and logging metrics for the training set.
-    validation_step(batch, batch_idx)
-        Performs a single validation step, computing the loss and logging metrics for the validation set.
-    configure_optimizers()
-        Configures the model's optimizers and learning rate schedulers.
     """
 
-
-
-
-
-
     def __init__(
         self,
         num_classes,
-        config: MambularConfig,
-        cat_feature_info: dict = None,
-        num_feature_info: dict = None,
-        lr=1e-03,
-        lr_patience=10,
-        weight_decay=0.025,
-        lr_factor=0.75,
+        cat_feature_info,
+        num_feature_info,
+        config: DefaultMambularConfig = DefaultMambularConfig(),
+        **kwargs,
     ):
         super().__init__()
 
-        self.config = config
         self.num_classes = 1 if num_classes == 2 else num_classes
-        self.lr = lr
-        self.lr_patience = lr_patience
-        self.weight_decay = weight_decay
-        self.lr_factor = lr_factor
+        # Save all hyperparameters
+        self.save_hyperparameters(ignore=["cat_feature_info", "num_feature_info"])
+
+        # Assigning values from hyperparameters
+        self.lr = self.hparams.get("lr", config.lr)
+        self.lr_patience = self.hparams.get("lr_patience", config.lr_patience)
+        self.weight_decay = self.hparams.get("weight_decay", config.weight_decay)
+        self.lr_factor = self.hparams.get("lr_factor", config.lr_factor)
+        self.pooling_method = self.hparams.get("pooling_method", config.pooling_method)
         self.cat_feature_info = cat_feature_info
         self.num_feature_info = num_feature_info
 
-        activations = {
-            "relu": nn.ReLU(),
-            "tanh": nn.Tanh(),
-            "sigmoid": nn.Sigmoid(),
-            "leaky_relu": nn.LeakyReLU(),
-            "elu": nn.ELU(),
-            "selu": nn.SELU(),
-            "gelu": nn.GELU(),
-            "softplus": nn.Softplus(),
-            "leakyrelu": nn.LeakyReLU(),
-            "linear": nn.Identity(),
-        }
-
-        self.embedding_activation = activations.get(
-            self.config.num_embedding_activation.lower()
-        )
-        if self.embedding_activation is None:
-            raise ValueError(
-                f"Unsupported activation function: {self.config.num_embedding_activation}"
+        self.embedding_activation = self.hparams.get(
+            "num_embedding_activation", config.num_embedding_activation
+        )
+
+        # Additional layers and components initialization based on hyperparameters
+        self.mamba = Mamba(
+            d_model=self.hparams.get("d_model", config.d_model),
+            n_layers=self.hparams.get("n_layers", config.n_layers),
+            expand_factor=self.hparams.get("expand_factor", config.expand_factor),
+            bias=self.hparams.get("bias", config.bias),
+            d_conv=self.hparams.get("d_conv", config.d_conv),
+            conv_bias=self.hparams.get("conv_bias", config.conv_bias),
+            dropout=self.hparams.get("dropout", config.dropout),
+            dt_rank=self.hparams.get("dt_rank", config.dt_rank),
+            d_state=self.hparams.get("d_state", config.d_state),
+            dt_scale=self.hparams.get("dt_scale", config.dt_scale),
+            dt_init=self.hparams.get("dt_init", config.dt_init),
+            dt_max=self.hparams.get("dt_max", config.dt_max),
+            dt_min=self.hparams.get("dt_min", config.dt_min),
+            dt_init_floor=self.hparams.get("dt_init_floor", config.dt_init_floor),
+            norm=globals()[self.hparams.get("norm", config.norm)],
+            activation=self.hparams.get("activation", config.activation),
+        )
+
+        # Set the normalization layer dynamically
+        norm_layer = self.hparams.get("norm", config.norm)
+        if norm_layer == "RMSNorm":
+            self.norm_f = RMSNorm(self.hparams.get("d_model", config.d_model))
+        elif norm_layer == "LayerNorm":
+            self.norm_f = LayerNorm(self.hparams.get("d_model", config.d_model))
+        elif norm_layer == "BatchNorm":
+            self.norm_f = BatchNorm(self.hparams.get("d_model", config.d_model))
+        elif norm_layer == "InstanceNorm":
+            self.norm_f = InstanceNorm(self.hparams.get("d_model", config.d_model))
+        elif norm_layer == "GroupNorm":
+            self.norm_f = GroupNorm(1, self.hparams.get("d_model", config.d_model))
+        elif norm_layer == "LearnableLayerScaling":
+            self.norm_f = LearnableLayerScaling(
+                self.hparams.get("d_model", config.d_model)
             )
+        else:
+            raise ValueError(f"Unsupported normalization layer: {norm_layer}")
 
         self.num_embeddings = nn.ModuleList(
             [
                 nn.Sequential(
-                    nn.Linear(input_shape, self.config.d_model, bias=False),
-                    nn.BatchNorm1d(self.config.d_model),
-                    self.embedding_activation,  # Example using ReLU as the activation function, change as needed
+                    nn.Linear(
+                        input_shape,
+                        self.hparams.get("d_model", config.d_model),
+                        bias=False,
+                    ),
+                    self.embedding_activation,
                 )
                 for feature_name, input_shape in num_feature_info.items()
             ]
         )
 
-        # Create embedding layers for categorical features based on cat_feature_info
         self.cat_embeddings = nn.ModuleList(
             [
-                nn.Embedding(num_categories + 1, self.config.d_model)
+                nn.Embedding(
+                    num_categories + 1, self.hparams.get("d_model", config.d_model)
+                )
                 for feature_name, num_categories in cat_feature_info.items()
             ]
         )
 
-        self.mamba = Mamba(self.config)
-        self.norm_f = self.config.norm(self.config.d_model)
-
-        mlp_activation_fn = activations.get(
-            self.config.tabular_head_activation.lower(), nn.Identity()
-        )
-        mlp_layers = []
-        input_dim = self.config.d_model  # Initial input dimension
-
-        # Iterate over the specified units for each layer in the MLP
-        for units in self.config.tabular_head_units:
-            mlp_layers.append(nn.Linear(input_dim, units))
-            mlp_layers.append(mlp_activation_fn)
-            mlp_layers.append(nn.Dropout(self.config.tabular_head_dropout))
-            input_dim = units
-
-        # Add the final linear layer to map to a single output value
-        mlp_layers.append(nn.Linear(input_dim, self.num_classes))
-
-        # Combine all layers into a Sequential module
-        self.tabular_head = nn.Sequential(*mlp_layers)
+        head_activation = self.hparams.get("head_activation", config.head_activation)
 
-        self.pooling_method = self.config.pooling_method
-        self.cls_token = nn.Parameter(torch.zeros(1, 1, self.config.d_model))
+        self.tabular_head = MLP(
+            self.hparams.get("d_model", config.d_model),
+            hidden_units_list=self.hparams.get(
+                "head_layer_sizes", config.head_layer_sizes
+            ),
+            dropout_rate=self.hparams.get("head_dropout", config.head_dropout),
+            use_skip_layers=self.hparams.get(
+                "head_skip_layers", config.head_skip_layers
+            ),
+            activation_fn=head_activation,
+            use_batch_norm=self.hparams.get(
+                "head_use_batch_norm", config.head_use_batch_norm
+            ),
+            n_output_units=self.num_classes,
+        )
+
+        self.cls_token = nn.Parameter(
+            torch.zeros(1, 1, self.hparams.get("d_model", config.d_model))
+        )
+
+        self.loss_fct = nn.MSELoss()
+
+        if self.hparams.get("layer_norm_after_embedding"):
+            self.embedding_norm = nn.LayerNorm(
+                self.hparams.get("d_model", config.d_model)
+            )
 
         if self.num_classes > 2:
             self.loss_fct = nn.CrossEntropyLoss()
             self.acc = torchmetrics.Accuracy(
                 task="multiclass", num_classes=self.num_classes
             )
             self.auroc = torchmetrics.AUROC(
@@ -177,53 +210,56 @@
             )
         else:
             self.loss_fct = torch.nn.BCEWithLogitsLoss()
             self.acc = torchmetrics.Accuracy(task="binary")
             self.auroc = torchmetrics.AUROC(task="binary")
             self.precision = torchmetrics.Precision(task="binary")
 
-    def forward(self, cat_features, num_features):
+    def forward(self, num_features, cat_features):
         """
         Defines the forward pass of the classifier.
 
         Parameters
         ----------
         cat_features : Tensor
             Tensor containing the categorical features.
         num_features : Tensor
             Tensor containing the numerical features.
 
+
         Returns
         -------
         Tensor
             The output predictions of the model.
         """
         batch_size = (
-            cat_features[0].size(0)
-            if cat_features is not None
-            else num_features[0].size(0)
+            cat_features[0].size(0) if cat_features != [] else num_features[0].size(0)
         )
         cls_tokens = self.cls_token.expand(batch_size, -1, -1)
 
         # Process categorical features if present
         if len(self.cat_embeddings) > 0 and cat_features:
             cat_embeddings = [
                 emb(cat_features[i]) for i, emb in enumerate(self.cat_embeddings)
             ]
             cat_embeddings = torch.stack(cat_embeddings, dim=1)
             cat_embeddings = torch.squeeze(cat_embeddings, dim=2)
+            if self.hparams.get("layer_norm_after_embedding"):
+                cat_embeddings = self.embedding_norm(cat_embeddings)
         else:
             cat_embeddings = None
 
         # Process numerical features if present
         if len(self.num_embeddings) > 0 and num_features:
             num_embeddings = [
                 emb(num_features[i]) for i, emb in enumerate(self.num_embeddings)
             ]
             num_embeddings = torch.stack(num_embeddings, dim=1)
+            if self.hparams.get("layer_norm_after_embedding"):
+                num_embeddings = self.embedding_norm(num_embeddings)
         else:
             num_embeddings = None
 
         # Combine embeddings if both types are present, otherwise use whichever is available
         if cat_embeddings is not None and num_embeddings is not None:
             x = torch.cat([cls_tokens, cat_embeddings, num_embeddings], dim=1)
         elif cat_embeddings is not None:
@@ -245,36 +281,35 @@
         elif self.pooling_method == "cls":
             x = x[:, 0]
         else:
             raise ValueError(f"Invalid pooling method: {self.pooling_method}")
 
         x = self.norm_f(x)
         preds = self.tabular_head(x)
-
         return preds
 
     def training_step(self, batch, batch_idx):
         """
         Processes a single batch during training, computes the loss and logs training metrics.
 
         Parameters
         ----------
         batch : tuple
             A batch of data from the DataLoader, containing numerical features, categorical features, and labels.
         batch_idx : int
             The index of the batch within the epoch.
         """
-        
-        num_features, cat_features, labels = batch
-        preds = self(num_features, cat_features)
+
+        cat_features, num_features, labels = batch
+        preds = self(num_features=num_features, cat_features=cat_features)
 
         if self.num_classes == 1:
-            labels = labels.unsqueeze(
-                1
-            ).float()  # Reshape for binary classification loss calculation
+            labels = torch.float(
+                labels.unsqueeze(1), dtype=torch.float32
+            )  # Reshape for binary classification loss calculation
 
         loss = self.loss_fct(preds, labels)
         self.log("train_loss", loss)
         # Calculate and log training accuracy
 
         acc = self.acc(preds, labels.int())
         self.log(
@@ -306,28 +341,27 @@
             on_epoch=True,
             prog_bar=True,
             logger=True,
         )
 
         return loss
 
-    def validation_step(self, batch, batch_idx):     
+    def validation_step(self, batch, batch_idx):
         """
         Processes a single batch during validation, computes the loss and logs validation metrics.
 
         Parameters
         ----------
         batch : tuple
             A batch of data from the DataLoader, containing numerical features, categorical features, and labels.
         batch_idx : int
             The index of the batch within the epoch.
         """
-        
-        num_features, cat_features, labels = batch
-        preds = self(num_features, cat_features)
+        cat_features, num_features, labels = batch
+        preds = self(num_features=num_features, cat_features=cat_features)
 
         if self.num_classes == 1:
             labels = labels.unsqueeze(
                 1
             ).float()  # Reshape for binary classification loss calculation
 
         loss = self.loss_fct(preds, labels)
@@ -366,15 +400,15 @@
 
         Returns
         -------
         dict
             A dictionary containing the optimizer and lr_scheduler configurations.
         """
         optimizer = torch.optim.Adam(
-            self.parameters(), lr=self.lr, weight_decay=self.config.weight_decay
+            self.parameters(), lr=self.lr, weight_decay=self.weight_decay
         )
         scheduler = {
             "scheduler": torch.optim.lr_scheduler.ReduceLROnPlateau(
                 optimizer,
                 mode="min",
                 factor=self.lr_factor,
                 patience=self.lr_patience,
```

### Comparing `mambular-0.1.2/mambular/base_models/embedding_classifier.py` & `mambular-0.1.3/mambular/base_models/distributional.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,259 +1,278 @@
+import lightning as pl
 import torch
 import torch.nn as nn
+
+from ..utils.configs import DefaultMambularConfig
+from ..utils.mlp_utils import MLP
+from ..utils.distributions import (
+    BetaDistribution,
+    CategoricalDistribution,
+    DirichletDistribution,
+    GammaDistribution,
+    InverseGammaDistribution,
+    NegativeBinomialDistribution,
+    NormalDistribution,
+    PoissonDistribution,
+    StudentTDistribution,
+)
+from ..utils.normalization_layers import (
+    RMSNorm,
+    LayerNorm,
+    LearnableLayerScaling,
+    BatchNorm,
+    InstanceNorm,
+    GroupNorm,
+)
 from ..utils.mamba_arch import Mamba
-from ..utils.config import MambularConfig
-import pytorch_lightning as pl
-import torchmetrics
 
 
-class BaseEmbeddingMambularClassifier(pl.LightningModule):
+class BaseMambularLSS(pl.LightningModule):
     """
-    A specialized classification module for protein data, built on PyTorch Lightning and integrating the Mamba architecture.
-    It supports embeddings for categorical features and can process raw or embedded numerical features, making it suitable
-    for complex protein sequence data.
+    A base module for likelihood-based statistical learning (LSS) models built on PyTorch Lightning,
+    integrating the Mamba architecture for tabular data. This module is designed to accommodate various
+    statistical distribution families for different types of regression and classification tasks.
+
 
     Parameters
     ----------
-    config : MambularConfig
-        Configuration parameters for the model architecture.
-    cat_feature_info : dict, optional
-        Information about categorical features, mapping feature names to the number of unique categories.
-    num_feature_info : dict, optional
-        Information about numerical features, mapping feature names to their number of dimensions after embedding.
-    lr : float, optional
-        Learning rate for the optimizer. Defaults to 1e-03.
-    lr_patience : int, optional
-        Number of epochs with no improvement after which learning rate will be reduced. Defaults to 10.
-    weight_decay : float, optional
-        Weight decay coefficient for regularization in the optimizer. Defaults to 0.025.
-    lr_factor : float, optional
-        Factor by which the learning rate will be reduced by the scheduler. Defaults to 0.75.
-    seq_size : int, optional
-        Size of sequence chunks for processing numerical features. Relevant when `raw_embeddings` is False.
-    raw_embeddings : bool, optional
-        Indicates whether to use raw numerical features directly or to process them into embeddings. Defaults to False.
+    family : str
+        The name of the statistical distribution family to be used for modeling. Supported families include
+        'normal', 'poisson', 'gamma', 'beta', 'dirichlet', 'studentt', 'negativebinom', 'inversegamma', and 'categorical'.
+    cat_feature_info : dict
+        Dictionary containing information about categorical features.
+    num_feature_info : dict
+        Dictionary containing information about numerical features.
+    config : DefaultMambularConfig, optional
+        Configuration object containing default hyperparameters for the model (default is DefaultMambularConfig()).
+    **kwargs : dict
+        Additional keyword arguments.
+
 
     Attributes
     ----------
+    lr : float
+        Learning rate.
+    lr_patience : int
+        Patience for learning rate scheduler.
+    weight_decay : float
+        Weight decay for optimizer.
+    lr_factor : float
+        Factor by which the learning rate will be reduced.
+    pooling_method : str
+        Method to pool the features.
+    cat_feature_info : dict
+        Dictionary containing information about categorical features.
+    num_feature_info : dict
+        Dictionary containing information about numerical features.
+    embedding_activation : callable
+        Activation function for embeddings.
     mamba : Mamba
-        The core neural network module implementing the Mamba architecture.
+        Mamba architecture component.
     norm_f : nn.Module
-        Normalization layer applied after the Mamba block.
-    tabular_head : nn.Linear
-        Final linear layer mapping the features to the target.
-
-    Methods
-    -------
-    forward(cat_features, num_features)
-        Defines the forward pass of the model.
-    training_step(batch, batch_idx)
-        Processes a single batch during training.
-    validation_step(batch, batch_idx)
-        Processes a single batch during validation.
-    configure_optimizers()
-        Sets up the model's optimizer and learning rate scheduler.
+        Normalization layer.
+    num_embeddings : nn.ModuleList
+        Module list for numerical feature embeddings.
+    cat_embeddings : nn.ModuleList
+        Module list for categorical feature embeddings.
+    tabular_head : MLP
+        Multi-layer perceptron head for tabular data.
+    cls_token : nn.Parameter
+        Class token parameter.
+    embedding_norm : nn.Module, optional
+        Layer normalization applied after embedding if specified.
     """
 
     def __init__(
         self,
-        num_classes,
-        config: MambularConfig,
-        cat_feature_info: dict = None,
-        num_feature_info: dict = None,
-        lr=1e-03,
-        lr_patience=10,
-        weight_decay=0.025,
-        lr_factor=0.75,
-        seq_size: int = 20,
-        raw_embeddings=False,
+        family,
+        cat_feature_info,
+        num_feature_info,
+        config: DefaultMambularConfig = DefaultMambularConfig(),
+        distributional_kwargs=None,
+        **kwargs,
     ):
         super().__init__()
 
-        self.config = config
-        self.num_classes = 1 if num_classes == 2 else num_classes
-        self.lr = lr
-        self.lr_patience = lr_patience
-        self.weight_decay = weight_decay
-        self.lr_factor = lr_factor
+        # Save all hyperparameters
+        self.save_hyperparameters(ignore=["cat_feature_info", "num_feature_info"])
+
+        # Assigning values from hyperparameters
+        self.lr = self.hparams.get("lr", config.lr)
+        self.lr_patience = self.hparams.get("lr_patience", config.lr_patience)
+        self.weight_decay = self.hparams.get("weight_decay", config.weight_decay)
+        self.lr_factor = self.hparams.get("lr_factor", config.lr_factor)
+        self.pooling_method = self.hparams.get("pooling_method", config.pooling_method)
         self.cat_feature_info = cat_feature_info
         self.num_feature_info = num_feature_info
-        self.seq_size = seq_size
-        self.raw_embeddings = raw_embeddings
 
-        activations = {
-            "relu": nn.ReLU(),
-            "tanh": nn.Tanh(),
-            "sigmoid": nn.Sigmoid(),
-            "leaky_relu": nn.LeakyReLU(),
-            "elu": nn.ELU(),
-            "selu": nn.SELU(),
-            "gelu": nn.GELU(),
-            "softplus": nn.Softplus(),
-            "leakyrelu": nn.LeakyReLU(),
-            "linear": nn.Identity(),
+        self.embedding_activation = self.hparams.get(
+            "num_embedding_activation", config.num_embedding_activation
+        )
+
+        distribution_classes = {
+            "normal": NormalDistribution,
+            "poisson": PoissonDistribution,
+            "gamma": GammaDistribution,
+            "beta": BetaDistribution,
+            "dirichlet": DirichletDistribution,
+            "studentt": StudentTDistribution,
+            "negativebinom": NegativeBinomialDistribution,
+            "inversegamma": InverseGammaDistribution,
+            "categorical": CategoricalDistribution,
         }
 
-        if not self.raw_embeddings:
-            data_size = len(num_feature_info.items())
-            num_embedding_modules = data_size // self.seq_size
-            self.num_embeddings = nn.ModuleList(
-                [
-                    nn.Sequential(
-                        nn.Linear(self.seq_size, self.config.d_model, bias=False),
-                        self.embedding_activation,  # Example using ReLU as the activation function, change as needed
-                    )
-                    for _ in range(num_embedding_modules)
-                ]
-            )
+        if distributional_kwargs is None:
+            distributional_kwargs = {}
+
+        if family in distribution_classes:
+            self.family = distribution_classes[family](**distributional_kwargs)
         else:
-            data_size = len(num_feature_info.items())
-            num_embedding_modules = data_size
-            self.num_embeddings = nn.ModuleList(
-                [
-                    nn.Sequential(
-                        nn.Linear(1, self.config.d_model, bias=False),
-                        self.embedding_activation,  # Example using ReLU as the activation function, change as needed
-                    )
-                    for _ in range(num_embedding_modules)
-                ]
+            raise ValueError("Unsupported family: {}".format(family))
+
+        # Set the normalization layer dynamically
+        norm_layer = self.hparams.get("norm", config.norm)
+        if norm_layer == "RMSNorm":
+            self.norm_f = RMSNorm(self.hparams.get("d_model", config.d_model))
+        elif norm_layer == "LayerNorm":
+            self.norm_f = LayerNorm(self.hparams.get("d_model", config.d_model))
+        elif norm_layer == "BatchNorm":
+            self.norm_f = BatchNorm(self.hparams.get("d_model", config.d_model))
+        elif norm_layer == "InstanceNorm":
+            self.norm_f = InstanceNorm(self.hparams.get("d_model", config.d_model))
+        elif norm_layer == "GroupNorm":
+            self.norm_f = GroupNorm(1, self.hparams.get("d_model", config.d_model))
+        elif norm_layer == "LearnableLayerScaling":
+            self.norm_f = LearnableLayerScaling(
+                self.hparams.get("d_model", config.d_model)
             )
+        else:
+            raise ValueError(f"Unsupported normalization layer: {norm_layer}")
+
+        # Additional layers and components initialization based on hyperparameters
+        self.mamba = Mamba(
+            d_model=self.hparams.get("d_model", config.d_model),
+            n_layers=self.hparams.get("n_layers", config.n_layers),
+            expand_factor=self.hparams.get("expand_factor", config.expand_factor),
+            bias=self.hparams.get("bias", config.bias),
+            d_conv=self.hparams.get("d_conv", config.d_conv),
+            conv_bias=self.hparams.get("conv_bias", config.conv_bias),
+            dropout=self.hparams.get("dropout", config.dropout),
+            dt_rank=self.hparams.get("dt_rank", config.dt_rank),
+            d_state=self.hparams.get("d_state", config.d_state),
+            dt_scale=self.hparams.get("dt_scale", config.dt_scale),
+            dt_init=self.hparams.get("dt_init", config.dt_init),
+            dt_max=self.hparams.get("dt_max", config.dt_max),
+            dt_min=self.hparams.get("dt_min", config.dt_min),
+            dt_init_floor=self.hparams.get("dt_init_floor", config.dt_init_floor),
+            norm=globals()[self.hparams.get("norm", config.norm)],
+            activation=self.hparams.get("activation", config.activation),
+        )
+
+        self.num_embeddings = nn.ModuleList(
+            [
+                nn.Sequential(
+                    nn.Linear(
+                        input_shape,
+                        self.hparams.get("d_model", config.d_model),
+                        bias=False,
+                    ),
+                    self.embedding_activation,
+                )
+                for feature_name, input_shape in num_feature_info.items()
+            ]
+        )
 
         self.cat_embeddings = nn.ModuleList(
             [
-                nn.Embedding(num_categories + 1, self.config.d_model)
+                nn.Embedding(
+                    num_categories + 1, self.hparams.get("d_model", config.d_model)
+                )
                 for feature_name, num_categories in cat_feature_info.items()
             ]
         )
 
-        self.mamba = Mamba(self.config)
-        self.norm_f = self.config.norm(self.config.d_model)
-        mlp_activation_fn = activations.get(
-            self.config.tabular_head_activation.lower(), nn.Identity()
+        head_activation = self.hparams.get("head_activation", config.head_activation)
+
+        self.tabular_head = MLP(
+            self.hparams.get("d_model", config.d_model),
+            hidden_units_list=self.hparams.get(
+                "head_layer_sizes", config.head_layer_sizes
+            ),
+            dropout_rate=self.hparams.get("head_dropout", config.head_dropout),
+            use_skip_layers=self.hparams.get(
+                "head_skip_layers", config.head_skip_layers
+            ),
+            activation_fn=head_activation,
+            use_batch_norm=self.hparams.get(
+                "head_use_batch_norm", config.head_use_batch_norm
+            ),
+            n_output_units=self.family.param_count,
         )
 
-        # Dynamically create MLP layers based on config.tabular_units
-        mlp_layers = []
-        input_dim = self.config.d_model  # Initial input dimension
-
-        # Iterate over the specified units for each layer in the MLP
-        for units in self.config.tabular_head_units:
-            mlp_layers.append(nn.Linear(input_dim, units))
-            mlp_layers.append(mlp_activation_fn)
-            mlp_layers.append(nn.Dropout(self.config.tabular_head_dropout))
-            input_dim = units
-
-        # Add the final linear layer to map to a single output value
-        mlp_layers.append(nn.Linear(input_dim, self.num_classes))
-
-        # Combine all layers into a Sequential module
-        self.tabular_head = nn.Sequential(*mlp_layers)
-
-        self.pooling_method = self.config.pooling_method
-        self.cls_token = nn.Parameter(torch.zeros(1, 1, self.config.d_model))
-
-        if self.config.layer_norm_after_embedding:
-            self.embedding_norm = nn.LayerNorm(self.config.d_model)
-
-        if self.num_classes > 2:
-            self.loss_fct = nn.CrossEntropyLoss()
-            self.acc = torchmetrics.Accuracy(
-                task="multiclass", num_classes=self.num_classes
-            )
-            self.auroc = torchmetrics.AUROC(
-                task="multiclass", num_classes=self.num_classes
-            )
-            self.precision = torchmetrics.Precision(
-                task="multiclass", num_classes=self.num_classes
+        self.cls_token = nn.Parameter(
+            torch.zeros(1, 1, self.hparams.get("d_model", config.d_model))
+        )
+
+        self.loss_fct = nn.MSELoss()
+
+        if self.hparams.get("layer_norm_after_embedding"):
+            self.embedding_norm = nn.LayerNorm(
+                self.hparams.get("d_model", config.d_model)
             )
-        else:
-            self.loss_fct = torch.nn.BCEWithLogitsLoss()
-            self.acc = torchmetrics.Accuracy(task="binary")
-            self.auroc = torchmetrics.AUROC(task="binary")
-            self.precision = torchmetrics.Precision(task="binary")
 
-    def forward(self, cat_features, num_features):      
+    def compute_loss(self, predictions, y_true):
+        return self.family.compute_loss(predictions, y_true)
+
+    def forward(self, cat_features, num_features):
         """
         Defines the forward pass of the model, processing both categorical and numerical features,
-        and returning regression predictions.
+        and returning predictions based on the configured statistical distribution.
 
         Parameters
         ----------
         cat_features : Tensor
             Tensor containing the categorical features.
         num_features : Tensor
-            Tensor containing the numerical features or raw sequence data, depending on `raw_embeddings`.
+            Tensor containing the numerical features.
+
 
         Returns
         -------
         Tensor
-            The output predictions of the model for regression tasks.
+            The predictions of the model, typically the parameters of the chosen statistical distribution.
         """
+
         batch_size = (
             cat_features[0].size(0) if cat_features != [] else num_features[0].size(0)
         )
         cls_tokens = self.cls_token.expand(batch_size, -1, -1)
+
         # Process categorical features if present
-        if not self.raw_embeddings:
-            if len(self.cat_embeddings) > 0 and cat_features:
-                cat_embeddings = [
-                    emb(cat_features[i]) for i, emb in enumerate(self.cat_embeddings)
-                ]
-                cat_embeddings = torch.stack(cat_embeddings, dim=1)
-                cat_embeddings = torch.squeeze(cat_embeddings, dim=2)
-            else:
-                cat_embeddings = None
-
-            if len(self.num_embeddings) > 0 and num_features:
-                num_embeddings = []
-                # Iterate through the num_embeddings, taking slices of num_features for each
-                for i, emb in enumerate(self.num_embeddings):
-                    # Calculate start and end indices for slicing the list
-                    start_idx = i * self.seq_size
-                    end_idx = start_idx + self.seq_size
-
-                    # Slice the num_features list to get the current chunk
-                    current_chunk = num_features[start_idx:end_idx]
-
-                    # If the current_chunk is not empty, process it
-                    if current_chunk:
-                        # Concatenate tensors in the current chunk along dimension 1
-                        chunk_tensor = torch.cat(current_chunk, dim=1)
-                        # Apply the embedding layer to the chunk_tensor
-                        num_embeddings.append(emb(chunk_tensor))
-
-                # Stack the resulting embeddings along the second dimension if num_embeddings is not empty
-                if num_embeddings:
-                    num_embeddings = torch.stack(num_embeddings, dim=1)
-            else:
-                num_embeddings = None
+        if len(self.cat_embeddings) > 0 and cat_features:
+            cat_embeddings = [
+                emb(cat_features[i]) for i, emb in enumerate(self.cat_embeddings)
+            ]
+            cat_embeddings = torch.stack(cat_embeddings, dim=1)
+            cat_embeddings = torch.squeeze(cat_embeddings, dim=2)
+            if self.hparams.get("layer_norm_after_embedding"):
+                cat_embeddings = self.embedding_norm(cat_embeddings)
+        else:
+            cat_embeddings = None
 
+        # Process numerical features if present
+        if len(self.num_embeddings) > 0 and num_features:
+            num_embeddings = [
+                emb(num_features[i]) for i, emb in enumerate(self.num_embeddings)
+            ]
+            num_embeddings = torch.stack(num_embeddings, dim=1)
+            if self.hparams.get("layer_norm_after_embedding"):
+                num_embeddings = self.embedding_norm(num_embeddings)
         else:
-            # Process categorical features if present
-            if len(self.cat_embeddings) > 0 and cat_features:
-                cat_embeddings = [
-                    emb(cat_features[i]) for i, emb in enumerate(self.cat_embeddings)
-                ]
-                cat_embeddings = torch.stack(cat_embeddings, dim=1)
-                cat_embeddings = torch.squeeze(cat_embeddings, dim=2)
-                if self.config.layer_norm_after_embedding:
-                    cat_embeddings = self.embedding_norm(cat_embeddings)
-            else:
-                cat_embeddings = None
-
-            # Process numerical features if present
-            if len(self.num_embeddings) > 0 and num_features:
-                num_embeddings = [
-                    emb(num_features[i]) for i, emb in enumerate(self.num_embeddings)
-                ]
-                num_embeddings = torch.stack(num_embeddings, dim=1)
-                if self.config.layer_norm_after_embedding:
-                    num_embeddings = self.embedding_norm(num_embeddings)
-            else:
-                num_embeddings = None
+            num_embeddings = None
 
         # Combine embeddings if both types are present, otherwise use whichever is available
         if cat_embeddings is not None and num_embeddings is not None:
             x = torch.cat([cls_tokens, cat_embeddings, num_embeddings], dim=1)
         elif cat_embeddings is not None:
             x = torch.cat([cls_tokens, cat_embeddings], dim=1)
         elif num_embeddings is not None:
@@ -266,146 +285,91 @@
         # Apply pooling based on the specified method
         if self.pooling_method == "avg":
             x = torch.mean(x, dim=1)
         elif self.pooling_method == "max":
             x, _ = torch.max(x, dim=1)
         elif self.pooling_method == "sum":
             x = torch.sum(x, dim=1)
-        elif self.pooling_method == "cls_token":
+        elif self.pooling_method == "cls":
             x = x[:, 0]
         else:
             raise ValueError(f"Invalid pooling method: {self.pooling_method}")
 
         x = self.norm_f(x)
         preds = self.tabular_head(x)
 
         return preds
 
     def training_step(self, batch, batch_idx):
         """
-        Processes a single batch during training, computes the loss, and logs training metrics.
+        Processes a single batch during training, computes the loss using the distribution-specific loss function,
+        and logs training metrics.
 
         Parameters
         ----------
         batch : tuple
             A batch of data from the DataLoader, containing numerical features, categorical features, and labels.
         batch_idx : int
             The index of the batch within the epoch.
 
         Returns
         -------
         Tensor
             The computed loss for the batch.
         """
-        num_features, cat_features, labels = batch
-        preds = self(num_features, cat_features)
-
-        if self.num_classes == 1:
-            labels = labels.unsqueeze(
-                1
-            ).float()  # Reshape for binary classification loss calculation
-
-        loss = self.loss_fct(preds, labels)
-        self.log("train_loss", loss)
-        # Calculate and log training accuracy
-
-        acc = self.acc(preds, labels.int())
-        self.log(
-            "train_acc",
-            acc,
-            on_step=False,
-            on_epoch=True,
-            prog_bar=True,
-            logger=True,
-        )
+        cat_features, num_features, labels = batch
+        preds = self(num_features=num_features, cat_features=cat_features)
 
-        # Calculate and log AUROC
-        auroc = self.auroc(preds, labels.int())
+        loss = self.compute_loss(preds, labels)
         self.log(
-            "train_auroc",
-            auroc,
-            on_step=False,
+            "train_loss",
+            loss,
             on_epoch=True,
             prog_bar=True,
             logger=True,
         )
-
-        # Calculate and log precision
-        precision = self.precision(preds, labels.int())
-        self.log(
-            "train_precision",
-            precision,
-            on_step=False,
-            on_epoch=True,
-            prog_bar=True,
-            logger=True,
-        )
-
         return loss
 
     def validation_step(self, batch, batch_idx):
         """
-        Processes a single batch during validation, computes the loss, and logs validation metrics.
+        Processes a single batch during validation, computes the loss using the distribution-specific loss function,
+        and logs validation metrics.
 
         Parameters
         ----------
         batch : tuple
             A batch of data from the DataLoader, containing numerical features, categorical features, and labels.
         batch_idx : int
             The index of the batch within the epoch.
         """
-        num_features, cat_features, labels = batch
-        preds = self(num_features, cat_features)
 
-        if self.num_classes == 1:
-            labels = labels.unsqueeze(
-                1
-            ).float()  # Reshape for binary classification loss calculation
-
-        loss = self.loss_fct(preds, labels)
-        self.log("val_loss", loss)
-        # Calculate and log training accuracy
+        cat_features, num_features, labels = batch
+        preds = self(num_features=num_features, cat_features=cat_features)
 
-        acc = self.acc(preds, labels.int())
+        loss = self.compute_loss(preds, labels)
         self.log(
-            "val_acc",
-            acc,
-            on_step=False,
-            on_epoch=True,
-            prog_bar=True,
-            logger=True,
-        )
-
-        auroc = self.auroc(preds, labels.int())
-        self.log(
-            "val_auroc", auroc, on_step=False, on_epoch=True, prog_bar=True, logger=True
-        )
-
-        # Calculate and log precision
-        precision = self.precision(preds, labels.int())
-        self.log(
-            "val_precision",
-            precision,
-            on_step=False,
+            "val_loss",
+            loss,
             on_epoch=True,
             prog_bar=True,
             logger=True,
         )
+        return loss
 
     def configure_optimizers(self):
         """
         Sets up the model's optimizer and learning rate scheduler based on the configurations provided.
 
         Returns
         -------
         dict
             A dictionary containing the optimizer and lr_scheduler configurations.
         """
         optimizer = torch.optim.Adam(
-            self.parameters(), lr=self.lr, weight_decay=self.config.weight_decay
+            self.parameters(), lr=self.lr, weight_decay=self.weight_decay
         )
         scheduler = {
             "scheduler": torch.optim.lr_scheduler.ReduceLROnPlateau(
                 optimizer,
                 mode="min",
                 factor=self.lr_factor,
                 patience=self.lr_patience,
```

### Comparing `mambular-0.1.2/mambular/base_models/embedding_regressor.py` & `mambular-0.1.3/mambular/base_models/regressor.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,253 +1,237 @@
+import lightning as pl
 import torch
 import torch.nn as nn
 from ..utils.mamba_arch import Mamba
-from ..utils.config import MambularConfig
-import pytorch_lightning as pl
+from ..utils.mlp_utils import MLP
+from ..utils.normalization_layers import (
+    RMSNorm,
+    LayerNorm,
+    LearnableLayerScaling,
+    BatchNorm,
+    InstanceNorm,
+    GroupNorm,
+)
+from ..utils.configs import DefaultMambularConfig
 
 
-class BaseEmbeddingMambularRegressor(pl.LightningModule):   
+class BaseMambularRegressor(pl.LightningModule):
     """
-    A specialized regression module for protein data, built on PyTorch Lightning and integrating the Mamba architecture.
-    It supports embeddings for categorical features and can process raw or embedded numerical features, making it suitable
-    for complex protein sequence data.
+    A PyTorch Lightning Module for regression tasks utilizing the Mamba architecture and various normalization techniques.
 
     Parameters
     ----------
-    config : MambularConfig
-        Configuration parameters for the model architecture.
-    cat_feature_info : dict, optional
-        Information about categorical features, mapping feature names to the number of unique categories. Defaults to None.
-    num_feature_info : dict, optional
-        Information about numerical features, mapping feature names to their number of dimensions after embedding. Defaults to None.
-    lr : float, optional
-        Learning rate for the optimizer. Defaults to 1e-03.
-    lr_patience : int, optional
-        Number of epochs with no improvement after which learning rate will be reduced. Defaults to 10.
-    weight_decay : float, optional
-        Weight decay coefficient for regularization in the optimizer. Defaults to 0.025.
-    lr_factor : float, optional
-        Factor by which the learning rate will be reduced by the scheduler. Defaults to 0.75.
-    seq_size : int, optional
-        Size of sequence chunks for processing numerical features. Relevant when `raw_embeddings` is False.
-    raw_embeddings : bool, optional
-        Indicates whether to use raw numerical features directly or to process them into embeddings. Defaults to False.
+    cat_feature_info : dict
+        Dictionary containing information about categorical features.
+    num_feature_info : dict
+        Dictionary containing information about numerical features.
+    config : DefaultMambularConfig, optional
+        Configuration object containing default hyperparameters for the model (default is DefaultMambularConfig()).
+    **kwargs : dict
+        Additional keyword arguments.
 
     Attributes
     ----------
+    lr : float
+        Learning rate.
+    lr_patience : int
+        Patience for learning rate scheduler.
+    weight_decay : float
+        Weight decay for optimizer.
+    lr_factor : float
+        Factor by which the learning rate will be reduced.
+    pooling_method : str
+        Method to pool the features.
+    cat_feature_info : dict
+        Dictionary containing information about categorical features.
+    num_feature_info : dict
+        Dictionary containing information about numerical features.
+    embedding_activation : callable
+        Activation function for embeddings.
     mamba : Mamba
-        The core neural network module implementing the Mamba architecture.
+        Mamba architecture component.
     norm_f : nn.Module
-        Normalization layer applied after the Mamba block.
-    tabular_head : nn.Linear
-        Final linear layer mapping the features to the regression target.
-    loss_fct : nn.MSELoss
-        The loss function for regression tasks.
-
-    Methods
-    -------
-    forward(cat_features, num_features)
-        Defines the forward pass of the model.
-    training_step(batch, batch_idx)
-        Processes a single batch during training.
-    validation_step(batch, batch_idx)
-        Processes a single batch during validation.
-    configure_optimizers()
-        Sets up the model's optimizer and learning rate scheduler.
+        Normalization layer.
+    num_embeddings : nn.ModuleList
+        Module list for numerical feature embeddings.
+    cat_embeddings : nn.ModuleList
+        Module list for categorical feature embeddings.
+    tabular_head : MLP
+        Multi-layer perceptron head for tabular data.
+    cls_token : nn.Parameter
+        Class token parameter.
+    loss_fct : nn.Module
+        Loss function.
+    embedding_norm : nn.Module, optional
+        Layer normalization applied after embedding if specified.
     """
-    
+
     def __init__(
         self,
-        config: MambularConfig,
-        cat_feature_info: dict = None,
-        num_feature_info: dict = None,
-        lr=1e-03,
-        lr_patience=10,
-        weight_decay=0.025,
-        lr_factor=0.75,
-        seq_size: int = 20,
-        raw_embeddings=False,
+        cat_feature_info,
+        num_feature_info,
+        config: DefaultMambularConfig = DefaultMambularConfig(),
+        **kwargs,
     ):
         super().__init__()
 
-        self.config = config
-        self.lr = lr
-        self.lr_patience = lr_patience
-        self.weight_decay = weight_decay
-        self.lr_factor = lr_factor
+        # Save all hyperparameters
+        self.save_hyperparameters(ignore=["cat_feature_info", "num_feature_info"])
+
+        # Assigning values from hyperparameters
+        self.lr = self.hparams.get("lr", config.lr)
+        self.lr_patience = self.hparams.get("lr_patience", config.lr_patience)
+        self.weight_decay = self.hparams.get("weight_decay", config.weight_decay)
+        self.lr_factor = self.hparams.get("lr_factor", config.lr_factor)
+        self.pooling_method = self.hparams.get("pooling_method", config.pooling_method)
         self.cat_feature_info = cat_feature_info
         self.num_feature_info = num_feature_info
-        self.seq_size = seq_size
-        self.raw_embeddings = raw_embeddings
 
-        activations = {
-            "relu": nn.ReLU(),
-            "tanh": nn.Tanh(),
-            "sigmoid": nn.Sigmoid(),
-            "leaky_relu": nn.LeakyReLU(),
-            "elu": nn.ELU(),
-            "selu": nn.SELU(),
-            "gelu": nn.GELU(),
-            "softplus": nn.Softplus(),
-            "leakyrelu": nn.LeakyReLU(),
-            "linear": nn.Identity(),
-        }
+        self.embedding_activation = self.hparams.get(
+            "num_embedding_activation", config.num_embedding_activation
+        )
 
-        self.embedding_activation = activations.get(
-            self.config.num_embedding_activation.lower()
+        # Additional layers and components initialization based on hyperparameters
+        self.mamba = Mamba(
+            d_model=self.hparams.get("d_model", config.d_model),
+            n_layers=self.hparams.get("n_layers", config.n_layers),
+            expand_factor=self.hparams.get("expand_factor", config.expand_factor),
+            bias=self.hparams.get("bias", config.bias),
+            d_conv=self.hparams.get("d_conv", config.d_conv),
+            conv_bias=self.hparams.get("conv_bias", config.conv_bias),
+            dropout=self.hparams.get("dropout", config.dropout),
+            dt_rank=self.hparams.get("dt_rank", config.dt_rank),
+            d_state=self.hparams.get("d_state", config.d_state),
+            dt_scale=self.hparams.get("dt_scale", config.dt_scale),
+            dt_init=self.hparams.get("dt_init", config.dt_init),
+            dt_max=self.hparams.get("dt_max", config.dt_max),
+            dt_min=self.hparams.get("dt_min", config.dt_min),
+            dt_init_floor=self.hparams.get("dt_init_floor", config.dt_init_floor),
+            norm=globals()[self.hparams.get("norm", config.norm)],
+            activation=self.hparams.get("activation", config.activation),
         )
-        if self.embedding_activation is None:
-            raise ValueError(
-                f"Unsupported activation function: {self.config.num_embedding_activation}"
-            )
 
-        if not self.raw_embeddings:
-            data_size = len(num_feature_info.items())
-            num_embedding_modules = data_size // self.seq_size
-            self.num_embeddings = nn.ModuleList(
-                [
-                    nn.Sequential(
-                        nn.Linear(self.seq_size, self.config.d_model, bias=False),
-                        self.embedding_activation,  # Example using ReLU as the activation function, change as needed
-                    )
-                    for _ in range(num_embedding_modules)
-                ]
+        # Set the normalization layer dynamically
+        norm_layer = self.hparams.get("norm", config.norm)
+        if norm_layer == "RMSNorm":
+            self.norm_f = RMSNorm(self.hparams.get("d_model", config.d_model))
+        elif norm_layer == "LayerNorm":
+            self.norm_f = LayerNorm(self.hparams.get("d_model", config.d_model))
+        elif norm_layer == "BatchNorm":
+            self.norm_f = BatchNorm(self.hparams.get("d_model", config.d_model))
+        elif norm_layer == "InstanceNorm":
+            self.norm_f = InstanceNorm(self.hparams.get("d_model", config.d_model))
+        elif norm_layer == "GroupNorm":
+            self.norm_f = GroupNorm(1, self.hparams.get("d_model", config.d_model))
+        elif norm_layer == "LearnableLayerScaling":
+            self.norm_f = LearnableLayerScaling(
+                self.hparams.get("d_model", config.d_model)
             )
         else:
-            data_size = len(num_feature_info.items())
-            num_embedding_modules = data_size
-            self.num_embeddings = nn.ModuleList(
-                [
-                    nn.Sequential(
-                        nn.Linear(1, self.config.d_model, bias=False),
-                        self.embedding_activation,  # Example using ReLU as the activation function, change as needed
-                    )
-                    for _ in range(num_embedding_modules)
-                ]
-            )
+            raise ValueError(f"Unsupported normalization layer: {norm_layer}")
 
-        self.cat_embeddings = nn.ModuleList(
+        self.num_embeddings = nn.ModuleList(
             [
-                nn.Embedding(num_categories + 1, self.config.d_model)
-                for feature_name, num_categories in cat_feature_info.items()
+                nn.Sequential(
+                    nn.Linear(
+                        input_shape,
+                        self.hparams.get("d_model", config.d_model),
+                        bias=False,
+                    ),
+                    self.embedding_activation,
+                )
+                for feature_name, input_shape in num_feature_info.items()
             ]
         )
 
-        self.mamba = Mamba(self.config)
-        self.norm_f = self.config.norm(self.config.d_model)
-        mlp_activation_fn = activations.get(
-            self.config.tabular_head_activation.lower(), nn.Identity()
+        self.cat_embeddings = nn.ModuleList(
+            [
+                nn.Embedding(
+                    num_categories + 1, self.hparams.get("d_model", config.d_model)
+                )
+                for feature_name, num_categories in cat_feature_info.items()
+            ]
         )
 
-        # Dynamically create MLP layers based on config.tabular_units
-        mlp_layers = []
-        input_dim = self.config.d_model  # Initial input dimension
-
-        # Iterate over the specified units for each layer in the MLP
-        for units in self.config.tabular_head_units:
-            mlp_layers.append(nn.Linear(input_dim, units))
-            mlp_layers.append(mlp_activation_fn)
-            mlp_layers.append(nn.Dropout(self.config.tabular_head_dropout))
-            input_dim = units
-
-        # Add the final linear layer to map to a single output value
-        mlp_layers.append(nn.Linear(input_dim, 1))
+        head_activation = self.hparams.get("head_activation", config.head_activation)
 
-        # Combine all layers into a Sequential module
-        self.tabular_head = nn.Sequential(*mlp_layers)
-
-        self.pooling_method = self.config.pooling_method
-        self.cls_token = nn.Parameter(torch.zeros(1, 1, self.config.d_model))
+        self.tabular_head = MLP(
+            self.hparams.get("d_model", config.d_model),
+            hidden_units_list=self.hparams.get(
+                "head_layer_sizes", config.head_layer_sizes
+            ),
+            dropout_rate=self.hparams.get("head_dropout", config.head_dropout),
+            use_skip_layers=self.hparams.get(
+                "head_skip_layers", config.head_skip_layers
+            ),
+            activation_fn=head_activation,
+            use_batch_norm=self.hparams.get(
+                "head_use_batch_norm", config.head_use_batch_norm
+            ),
+        )
 
-        if self.config.layer_norm_after_embedding:
-            self.embedding_norm = nn.LayerNorm(self.config.d_model)
+        self.cls_token = nn.Parameter(
+            torch.zeros(1, 1, self.hparams.get("d_model", config.d_model))
+        )
 
         self.loss_fct = nn.MSELoss()
 
-    def forward(self, cat_features, num_features):
+        if self.hparams.get("layer_norm_after_embedding"):
+            self.embedding_norm = nn.LayerNorm(
+                self.hparams.get("d_model", config.d_model)
+            )
+
+    def forward(self, num_features, cat_features):
         """
-        Defines the forward pass of the model, processing both categorical and numerical features,
-        and returning regression predictions.
+        Defines the forward pass of the regressor.
 
         Parameters
         ----------
         cat_features : Tensor
             Tensor containing the categorical features.
         num_features : Tensor
-            Tensor containing the numerical features or raw sequence data, depending on `raw_embeddings`.
+            Tensor containing the numerical features.
+
 
         Returns
         -------
         Tensor
             The output predictions of the model for regression tasks.
         """
+
         batch_size = (
             cat_features[0].size(0) if cat_features != [] else num_features[0].size(0)
         )
         cls_tokens = self.cls_token.expand(batch_size, -1, -1)
+
         # Process categorical features if present
-        if not self.raw_embeddings:
-            if len(self.cat_embeddings) > 0 and cat_features:
-                cat_embeddings = [
-                    emb(cat_features[i]) for i, emb in enumerate(self.cat_embeddings)
-                ]
-                cat_embeddings = torch.stack(cat_embeddings, dim=1)
-                cat_embeddings = torch.squeeze(cat_embeddings, dim=2)
-            else:
-                cat_embeddings = None
-
-            if len(self.num_embeddings) > 0 and num_features:
-                num_embeddings = []
-                # Iterate through the num_embeddings, taking slices of num_features for each
-                for i, emb in enumerate(self.num_embeddings):
-                    # Calculate start and end indices for slicing the list
-                    start_idx = i * self.seq_size
-                    end_idx = start_idx + self.seq_size
-
-                    # Slice the num_features list to get the current chunk
-                    current_chunk = num_features[start_idx:end_idx]
-
-                    # If the current_chunk is not empty, process it
-                    if current_chunk:
-                        # Concatenate tensors in the current chunk along dimension 1
-                        chunk_tensor = torch.cat(current_chunk, dim=1)
-                        # Apply the embedding layer to the chunk_tensor
-                        num_embeddings.append(emb(chunk_tensor))
-
-                # Stack the resulting embeddings along the second dimension if num_embeddings is not empty
-                if num_embeddings:
-                    num_embeddings = torch.stack(num_embeddings, dim=1)
-            else:
-                num_embeddings = None
+        if len(self.cat_embeddings) > 0 and cat_features:
+            cat_embeddings = [
+                emb(cat_features[i]) for i, emb in enumerate(self.cat_embeddings)
+            ]
+            cat_embeddings = torch.stack(cat_embeddings, dim=1)
+            cat_embeddings = torch.squeeze(cat_embeddings, dim=2)
+            if self.hparams.get("layer_norm_after_embedding"):
+                cat_embeddings = self.embedding_norm(cat_embeddings)
+        else:
+            cat_embeddings = None
 
+        # Process numerical features if present
+        if len(self.num_embeddings) > 0 and num_features:
+            num_embeddings = [
+                emb(num_features[i]) for i, emb in enumerate(self.num_embeddings)
+            ]
+            num_embeddings = torch.stack(num_embeddings, dim=1)
+            if self.hparams.get("layer_norm_after_embedding"):
+                num_embeddings = self.embedding_norm(num_embeddings)
         else:
-            # Process categorical features if present
-            if len(self.cat_embeddings) > 0 and cat_features:
-                cat_embeddings = [
-                    emb(cat_features[i]) for i, emb in enumerate(self.cat_embeddings)
-                ]
-                cat_embeddings = torch.stack(cat_embeddings, dim=1)
-                cat_embeddings = torch.squeeze(cat_embeddings, dim=2)
-                if self.config.layer_norm_after_embedding:
-                    cat_embeddings = self.embedding_norm(cat_embeddings)
-            else:
-                cat_embeddings = None
-
-            # Process numerical features if present
-            if len(self.num_embeddings) > 0 and num_features:
-                num_embeddings = [
-                    emb(num_features[i]) for i, emb in enumerate(self.num_embeddings)
-                ]
-                num_embeddings = torch.stack(num_embeddings, dim=1)
-                if self.config.layer_norm_after_embedding:
-                    num_embeddings = self.embedding_norm(num_embeddings)
-            else:
-                num_embeddings = None
+            num_embeddings = None
 
         # Combine embeddings if both types are present, otherwise use whichever is available
+
         if cat_embeddings is not None and num_embeddings is not None:
             x = torch.cat([cls_tokens, cat_embeddings, num_embeddings], dim=1)
         elif cat_embeddings is not None:
             x = torch.cat([cls_tokens, cat_embeddings], dim=1)
         elif num_embeddings is not None:
             x = torch.cat([cls_tokens, num_embeddings], dim=1)
         else:
@@ -270,30 +254,31 @@
         x = self.norm_f(x)
         preds = self.tabular_head(x)
 
         return preds
 
     def training_step(self, batch, batch_idx):
         """
-        Processes a single batch during training, computes the loss, and logs training metrics.
+        Defines the forward pass of the regressor.
 
         Parameters
         ----------
-        batch : tuple
-            A batch of data from the DataLoader, containing numerical features, categorical features, and labels.
-        batch_idx : int
-            The index of the batch within the epoch.
+        cat_features : Tensor
+            Tensor containing the categorical features.
+        num_features : Tensor
+            Tensor containing the numerical features.
+
 
         Returns
         -------
         Tensor
-            The computed loss for the batch.
-        """    
-        num_features, cat_features, labels = batch
-        preds = self(num_features, cat_features)
+            The output predictions of the model for regression tasks.
+        """
+        cat_features, num_features, labels = batch
+        preds = self(num_features=num_features, cat_features=cat_features)
 
         loss = self.loss_fct(preds.squeeze(), labels.float())
         self.log(
             "train_loss",
             loss,
             on_step=True,
             on_epoch=True,
@@ -309,16 +294,16 @@
         Parameters
         ----------
         batch : tuple
             A batch of data from the DataLoader, containing numerical features, categorical features, and labels.
         batch_idx : int
             The index of the batch within the epoch.
         """
-        num_features, cat_features, labels = batch
-        preds = self(num_features, cat_features)
+        cat_features, num_features, labels = batch
+        preds = self(num_features=num_features, cat_features=cat_features)
 
         loss = self.loss_fct(preds.squeeze(), labels.float())
         self.log(
             "val_loss",
             loss,
             on_step=True,
             on_epoch=True,
@@ -334,15 +319,15 @@
 
         Returns
         -------
         dict
             A dictionary containing the optimizer and lr_scheduler configurations.
         """
         optimizer = torch.optim.Adam(
-            self.parameters(), lr=self.lr, weight_decay=self.config.weight_decay
+            self.parameters(), lr=self.lr, weight_decay=self.weight_decay
         )
         scheduler = {
             "scheduler": torch.optim.lr_scheduler.ReduceLROnPlateau(
                 optimizer,
                 mode="min",
                 factor=self.lr_factor,
                 patience=self.lr_patience,
```

### Comparing `mambular-0.1.2/mambular/models/sklearn_classifier.py` & `mambular-0.1.3/mambular/models/sklearn_embedding_regressor.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,587 +1,666 @@
-from sklearn.model_selection import train_test_split
-import pytorch_lightning as pl
-import torch
-from torch.utils.data import DataLoader
-import numpy as np
-from pytorch_lightning.callbacks import ModelCheckpoint, EarlyStopping
-from ..base_models.classifier import BaseMambularClassifier
-from ..utils.config import MambularConfig
-from ..utils.preprocessor import Preprocessor
-from ..utils.dataset import MambularDataModule, MambularDataset
-from sklearn.base import BaseEstimator
-import pandas as pd
-from sklearn.metrics import accuracy_score
-
-
-class MambularClassifier(BaseEstimator):  
-    """
-    A classifier that mimics scikit-learn's API using PyTorch Lightning and a custom architecture.
-    
-    This classifier is designed to work with tabular data and provides a flexible interface for specifying model
-    configurations and preprocessing steps. It integrates smoothly with scikit-learn's utilities, such as cross-validation
-    and grid search.
-
-    Parameters
-    ----------
-    **kwargs : Various
-        Accepts any number of keyword arguments that are passed to the MambularConfig and Preprocessor classes.
-        Known configuration arguments for the model are extracted based on a predefined list, and the rest are
-        passed to the Preprocessor.
-
-    Attributes
-    ----------
-    config : MambularConfig
-        Configuration object that holds model-specific settings.
-    preprocessor : Preprocessor
-        Preprocessor object for handling feature preprocessing like normalization and encoding.
-    model : BaseMambularClassifier or None
-        The underlying PyTorch Lightning model, instantiated upon calling the `fit` method.
-    """
-    
-    def __init__(self, **kwargs):
-        # Known config arguments
-        print("Received kwargs:", kwargs)
-        config_arg_names = [
-            "d_model",
-            "n_layers",
-            "dt_rank",
-            "output_dimension",
-            "pooling_method",
-            "norm",
-            "cls",
-            "dt_min",
-            "dt_max",
-            "dropout",
-            "bias",
-            "weight_decay",
-            "conv_bias",
-            "d_state",
-            "expand_factor",
-            "d_conv",
-            "dt_init",
-            "dt_scale",
-            "dt_init_floor",
-            "tabular_head_units",
-            "tabular_head_activation",
-            "tabular_head_dropout",
-            "num_emebedding_activation",
-            "layer_norm_after_embedding",
-        ]
-        self.config_kwargs = {k: v for k, v in kwargs.items() if k in config_arg_names}
-        self.config = MambularConfig(**self.config_kwargs)
-
-        # The rest are assumed to be preprocessor arguments
-        preprocessor_kwargs = {
-            k: v for k, v in kwargs.items() if k not in config_arg_names
-        }
-        self.preprocessor = Preprocessor(**preprocessor_kwargs)
-        self.model = None
-
-    def get_params(self, deep=True):    
-        """
-        Get parameters for this estimator.
-
-        Parameters
-        ----------
-        deep : bool, default=True
-            If True, will return the parameters for this estimator and contained subobjects that are estimators.
-
-        Returns
-        -------
-        params : dict
-            Parameter names mapped to their values.
-        """
-        
-        params = self.config_kwargs  # Parameters used to initialize MambularConfig
-
-        # If deep=True, include parameters from nested components like preprocessor
-        if deep:
-            # Assuming Preprocessor has a get_params method
-            preprocessor_params = {
-                "preprocessor__" + key: value
-                for key, value in self.preprocessor.get_params().items()
-            }
-            params.update(preprocessor_params)
-
-        return params
-
-    def set_params(self, **parameters):
-        """
-        Set the parameters of this estimator.
-
-        Parameters
-        ----------
-        **parameters : dict
-            Estimator parameters.
-
-        Returns
-        -------
-        self : object
-            Estimator instance.
-        """
-        # Update config_kwargs with provided parameters
-        valid_config_keys = self.config_kwargs.keys()
-        config_updates = {k: v for k, v in parameters.items() if k in valid_config_keys}
-        self.config_kwargs.update(config_updates)
-
-        # Update the config object
-        for key, value in config_updates.items():
-            setattr(self.config, key, value)
-
-        # Handle preprocessor parameters (prefixed with 'preprocessor__')
-        preprocessor_params = {
-            k.split("__")[1]: v
-            for k, v in parameters.items()
-            if k.startswith("preprocessor__")
-        }
-        if preprocessor_params:
-            # Assuming Preprocessor has a set_params method
-            self.preprocessor.set_params(**preprocessor_params)
-
-        return self
-
-    def split_data(self, X, y, val_size, random_state):
-        """
-        Split the dataset into training and validation sets.
-
-        Parameters
-        ----------
-        X : array-like of shape (n_samples, n_features)
-            The input samples.
-        y : array-like of shape (n_samples,)
-            The target values.
-        val_size : float
-            The proportion of the dataset to include in the validation split.
-        random_state : int
-            Controls the shuffling applied to the data before applying the split.
-
-        Returns
-        -------
-        X_train, X_val, y_train, y_val : arrays
-            The split datasets.
-        """
-        X_train, X_val, y_train, y_val = train_test_split(
-            X, y, test_size=val_size, random_state=random_state
-        )
-
-        return X_train, X_val, y_train, y_val
-
-    def preprocess_data(self, X_train, y_train, X_val, y_val, batch_size, shuffle):
-        """
-        Preprocess the training and validation data and create corresponding DataLoaders.
-
-        Parameters
-        ----------
-        X_train : array-like of shape (n_samples, n_features)
-            The training input samples.
-        y_train : array-like of shape (n_samples,)
-            The training target values.
-        X_val : array-like of shape (n_samples, n_features)
-            The validation input samples.
-        y_val : array-like of shape (n_samples,)
-            The validation target values.
-        batch_size : int
-            Size of mini-batches for the DataLoader.
-        shuffle : bool
-            Whether to shuffle the training data before splitting into batches.
-
-        Returns
-        -------
-        data_module : MambularDataModule
-            An instance of MambularDataModule containing training and validation DataLoaders.
-        """
-
-        train_preprocessed_data = self.preprocessor.fit_transform(X_train, y_train)
-        val_preprocessed_data = self.preprocessor.transform(X_val)
-
-        # Update feature info based on the actual processed data
-        (
-            self.cat_feature_info,
-            self.num_feature_info,
-        ) = self.preprocessor.get_feature_info()
-
-        # Initialize lists for tensors
-        train_cat_tensors = []
-        train_num_tensors = []
-        val_cat_tensors = []
-        val_num_tensors = []
-
-        # Populate tensors for categorical features, if present in processed data
-        for key in self.cat_feature_info:
-            cat_key = "cat_" + key  # Assuming categorical keys are prefixed with 'cat_'
-            if cat_key in train_preprocessed_data:
-                train_cat_tensors.append(
-                    torch.tensor(train_preprocessed_data[cat_key], dtype=torch.long)
-                )
-            if cat_key in val_preprocessed_data:
-                val_cat_tensors.append(
-                    torch.tensor(val_preprocessed_data[cat_key], dtype=torch.long)
-                )
-
-            binned_key = "num_" + key  # for binned features
-            if binned_key in train_preprocessed_data:
-                train_cat_tensors.append(
-                    torch.tensor(train_preprocessed_data[binned_key], dtype=torch.long)
-                )
-
-            if binned_key in val_preprocessed_data:
-                val_cat_tensors.append(
-                    torch.tensor(val_preprocessed_data[binned_key], dtype=torch.long)
-                )
-
-        # Populate tensors for numerical features, if present in processed data
-        for key in self.num_feature_info:
-            num_key = "num_" + key  # Assuming numerical keys are prefixed with 'num_'
-            if num_key in train_preprocessed_data:
-                train_num_tensors.append(
-                    torch.tensor(train_preprocessed_data[num_key], dtype=torch.float)
-                )
-            if num_key in val_preprocessed_data:
-                val_num_tensors.append(
-                    torch.tensor(val_preprocessed_data[num_key], dtype=torch.float)
-                )
-
-        train_labels = torch.tensor(y_train, dtype=torch.long)
-        val_labels = torch.tensor(y_val, dtype=torch.long)
-
-        # Create datasets
-        train_dataset = MambularDataset(
-            train_cat_tensors, train_num_tensors, train_labels, regression=False
-        )
-        val_dataset = MambularDataset(
-            val_cat_tensors, val_num_tensors, val_labels, regression=False
-        )
-
-        # Create dataloaders
-        train_dataloader = DataLoader(
-            train_dataset, batch_size=batch_size, shuffle=shuffle
-        )
-        val_dataloader = DataLoader(val_dataset, batch_size=batch_size)
-
-        return MambularDataModule(train_dataloader, val_dataloader)
-
-    def preprocess_test_data(self, X):
-        """
-        Preprocesses the test data and creates tensors for categorical and numerical features.
-
-        Parameters
-        ----------
-        X : DataFrame or array-like, shape (n_samples, n_features)
-            Test feature set.
-
-        Returns
-        -------
-        cat_tensors : list of Tensors
-            List of tensors for each categorical feature.
-        num_tensors : list of Tensors
-            List of tensors for each numerical feature.
-        """
-        processed_data = self.preprocessor.transform(X)
-
-        # Initialize lists for tensors
-        cat_tensors = []
-        num_tensors = []
-
-        # Populate tensors for categorical features
-        for key in self.cat_feature_info:
-            cat_key = "cat_" + key  # Assuming categorical keys are prefixed with 'cat_'
-            if cat_key in processed_data:
-                cat_tensors.append(
-                    torch.tensor(processed_data[cat_key], dtype=torch.long)
-                )
-
-            binned_key = "num_" + key  # for binned features
-            if binned_key in processed_data:
-                cat_tensors.append(
-                    torch.tensor(processed_data[binned_key], dtype=torch.long)
-                )
-
-        # Populate tensors for numerical features
-        for key in self.num_feature_info:
-            num_key = "num_" + key  # Assuming numerical keys are prefixed with 'num_'
-            if num_key in processed_data:
-                num_tensors.append(
-                    torch.tensor(processed_data[num_key], dtype=torch.float)
-                )
-
-        return cat_tensors, num_tensors
-
-    def fit(
-        self,
-        X,
-        y,
-        val_size=0.2,
-        X_val=None,
-        y_val=None,
-        max_epochs=100,
-        random_state=101,
-        batch_size=64,
-        shuffle=True,
-        patience=10,
-        monitor="val_loss",
-        mode="min",
-        lr=1e-3,
-        lr_patience=10,
-        factor=0.75,
-        weight_decay=0.025,
-        **trainer_kwargs
-    ):
-        """
-        Fit the model to the given training data, optionally using a separate validation set.
-
-        Parameters
-        ----------
-        X : array-like or pd.DataFrame of shape (n_samples, n_features)
-            The training input samples.
-        y : array-like of shape (n_samples,) or (n_samples, n_outputs)
-            The target values (class labels in classification, real numbers in regression).
-        val_size : float, default=0.2
-            The proportion of the dataset to include in the validation split if `X_val` is None. Ignored if `X_val` is provided.
-        X_val : array-like or pd.DataFrame of shape (n_samples, n_features), optional
-            The validation input samples. If provided, `X` and `y` are not split and this data is used for validation.
-        y_val : array-like of shape (n_samples,) or (n_samples, n_outputs), optional
-            The validation target values. Required if `X_val` is provided.
-        max_epochs : int, default=100
-            Maximum number of epochs for training.
-        random_state : int, default=101
-            Seed used by the random number generator for shuffling the data if `X_val` is not provided.
-        batch_size : int, default=64
-            Number of samples per gradient update.
-        shuffle : bool, default=True
-            Whether to shuffle the training data before each epoch if `X_val` is not provided.
-        patience : int, default=10
-            Number of epochs with no improvement after which training will be stopped if using early stopping.
-        monitor : str, default="val_loss"
-            Quantity to be monitored for early stopping.
-        mode : str, default="min"
-            One of {"min", "max"}. In "min" mode, training will stop when the quantity monitored has stopped decreasing; in "max" mode, it will stop when the quantity monitored has stopped increasing.
-        lr : float, default=1e-3
-            Learning rate for the optimizer.
-        lr_patience : int, default=10
-            Number of epochs with no improvement after which the learning rate will be reduced.
-        factor : float, default=0.75
-            Factor by which the learning rate will be reduced. new_lr = lr * factor.
-        weight_decay : float, default=0.025
-            Weight decay (L2 penalty) parameter.
-        **trainer_kwargs : dict
-            Additional keyword arguments to be passed to the PyTorch Lightning Trainer constructor.
-
-        Returns
-        -------
-        self : object
-            The fitted estimator.
-        """
-
-        if not isinstance(X, pd.DataFrame):
-            X = pd.DataFrame(X)
-        if X_val:
-            if not isinstance(X_val, pd.DataFrame):
-                X_val = pd.DataFrame(X_val)
-
-        num_classes = len(np.unique(y))
-
-        if not X_val:
-            X_train, X_val, y_train, y_val = self.split_data(
-                X, y, val_size, random_state
-            )
-
-        data_module = self.preprocess_data(
-            X_train, y_train, X_val, y_val, batch_size, shuffle
-        )
-
-        self.model = BaseMambularClassifier(
-            num_classes=num_classes,
-            config=self.config,
-            cat_feature_info=self.cat_feature_info,
-            num_feature_info=self.num_feature_info,
-            lr=lr,
-            lr_patience=lr_patience,
-            lr_factor=factor,
-            weight_decay=weight_decay,
-        )
-
-        early_stop_callback = EarlyStopping(
-            monitor=monitor, min_delta=0.00, patience=patience, verbose=False, mode=mode
-        )
-
-        checkpoint_callback = ModelCheckpoint(
-            monitor="val_loss",  # Adjust according to your validation metric
-            mode="min",
-            save_top_k=1,
-            dirpath="model_checkpoints",  # Specify the directory to save checkpoints
-            filename="best_model",
-        )
-
-        # Initialize the trainer and train the model
-        trainer = pl.Trainer(
-            max_epochs=max_epochs,
-            callbacks=[early_stop_callback, checkpoint_callback],
-            **trainer_kwargs
-        )
-        trainer.fit(self.model, data_module)
-
-        best_model_path = checkpoint_callback.best_model_path
-        if best_model_path:
-            checkpoint = torch.load(best_model_path)
-            self.model.load_state_dict(checkpoint["state_dict"])
-
-        return self
-
-    def predict(self, X):
-        """
-        Predict the class labels for the given input samples.
-
-        Parameters
-        ----------
-        X : array-like or pd.DataFrame of shape (n_samples, n_features)
-            The input samples to predict.
-
-        Returns
-        -------
-        predictions : ndarray of shape (n_samples,)
-            Predicted class labels for each input sample.
-
-        Notes
-        -----
-        The method preprocesses the input data using the same preprocessor used during training,
-        sets the model to evaluation mode, and then performs inference to predict the class labels.
-        The predictions are converted from a PyTorch tensor to a NumPy array before being returned.
-        """
-        # Preprocess the data
-        if not isinstance(X, pd.DataFrame):
-            X = pd.DataFrame(X)
-        device = next(self.model.parameters()).device
-        cat_tensors, num_tensors = self.preprocess_test_data(X)
-        if isinstance(cat_tensors, list):
-            cat_tensors = [tensor.to(device) for tensor in cat_tensors]
-        else:
-            cat_tensors = cat_tensors.to(device)
-
-        if isinstance(num_tensors, list):
-            num_tensors = [tensor.to(device) for tensor in num_tensors]
-        else:
-            num_tensors = num_tensors.to(device)
-
-        # Set the model to evaluation mode
-        self.model.eval()
-
-        # Perform inference
-        with torch.no_grad():
-            logits = self.model(cat_tensors, num_tensors)
-            predictions = torch.argmax(logits, dim=1)
-
-        # Convert predictions to NumPy array and return
-        return predictions.cpu().numpy()
-
-    def predict_proba(self, X):
-        """
-        Predict class probabilities for the given input samples.
-
-        Example
-        -------
-            from sklearn.metrics import accuracy_score, precision_score, f1_score, roc_auc_score
-
-            # Define the metrics you want to evaluate
-            metrics = {
-                'Accuracy': (accuracy_score, False),
-                'Precision': (precision_score, False),
-                'F1 Score': (f1_score, False),
-                'AUC Score': (roc_auc_score, True)
-            }
-
-            # Assuming 'X_test' and 'y_test' are your test dataset and labels
-            # Evaluate using the specified metrics
-            results = classifier.evaluate(X_test, y_test, metrics=metrics)
-
-        Parameters
-        ----------
-        X : array-like or pd.DataFrame of shape (n_samples, n_features)
-            The input samples for which to predict class probabilities.
-
-        Returns
-        -------
-        probabilities : ndarray of shape (n_samples, n_classes)
-            Predicted class probabilities for each input sample.
-
-        Notes
-        -----
-        The method preprocesses the input data using the same preprocessor used during training,
-        sets the model to evaluation mode, and then performs inference to predict the class probabilities.
-        Softmax is applied to the logits to obtain probabilities, which are then converted from a PyTorch tensor
-        to a NumPy array before being returned.
-        """
-        # Preprocess the data
-        if not isinstance(X, pd.DataFrame):
-            X = pd.DataFrame(X)
-        device = next(self.model.parameters()).device
-        cat_tensors, num_tensors = self.preprocess_test_data(X)
-        if isinstance(cat_tensors, list):
-            cat_tensors = [tensor.to(device) for tensor in cat_tensors]
-        else:
-            cat_tensors = cat_tensors.to(device)
-
-        if isinstance(num_tensors, list):
-            num_tensors = [tensor.to(device) for tensor in num_tensors]
-        else:
-            num_tensors = num_tensors.to(device)
-
-        # Set the model to evaluation mode
-        self.model.eval()
-
-        # Perform inference
-        with torch.no_grad():
-            logits = self.model(cat_tensors, num_tensors)
-            probabilities = torch.softmax(logits, dim=1)
-
-        # Convert probabilities to NumPy array and return
-        return probabilities.cpu().numpy()
-
-    def evaluate(self, X, y_true, metrics=None):
-        """
-        Evaluate the model on the given data using specified metrics.
-
-        Parameters
-        ----------
-        X : array-like or pd.DataFrame of shape (n_samples, n_features)
-            The input samples to predict.
-        y_true : array-like of shape (n_samples,)
-            The true class labels against which to evaluate the predictions.
-        metrics : dict
-            A dictionary where keys are metric names and values are tuples containing the metric function
-            and a boolean indicating whether the metric requires probability scores (True) or class labels (False).
-
-        Returns
-        -------
-        scores : dict
-            A dictionary with metric names as keys and their corresponding scores as values.
-
-        Notes
-        -----
-        This method uses either the `predict` or `predict_proba` method depending on the metric requirements.
-        """
-        # Ensure input is in the correct format
-        if metrics is None:
-            metrics = {"Accuracy": (accuracy_score, False)}
-
-        if not isinstance(X, pd.DataFrame):
-            X = pd.DataFrame(X)
-
-        # Initialize dictionary to store results
-        scores = {}
-
-        # Generate class probabilities if any metric requires them
-        if any(use_proba for _, use_proba in metrics.values()):
-            probabilities = self.predict_proba(X)
-
-        # Generate class labels if any metric requires them
-        if any(not use_proba for _, use_proba in metrics.values()):
-            predictions = self.predict(X)
-
-        # Compute each metric
-        for metric_name, (metric_func, use_proba) in metrics.items():
-            if use_proba:
-                scores[metric_name] = metric_func(y_true, probabilities)
-            else:
-                scores[metric_name] = metric_func(y_true, predictions)
-
-        return scores
+import warnings
+
+import lightning as pl
+import numpy as np
+import pandas as pd
+import torch
+from lightning.pytorch.callbacks import EarlyStopping, ModelCheckpoint
+from sklearn.base import BaseEstimator
+from sklearn.decomposition import PCA
+from sklearn.metrics import mean_squared_error
+from sklearn.model_selection import train_test_split
+from torch.utils.data import DataLoader
+
+from ..base_models.embedding_regressor import BaseEmbeddingMambularRegressor
+from ..utils.configs import DefaultMambularConfig
+from ..utils.dataset import EmbeddingMambularDataset, MambularDataModule
+from ..utils.preprocessor import Preprocessor
+
+
+class EmbeddingMambularRegressor(BaseEstimator):
+    """
+    An sklearn-like interface for the ProteinMambularRegressor, making it compatible with sklearn's utilities
+    and workflows. This class wraps the PyTorch Lightning model and preprocessor, providing methods for fitting,
+    predicting, and setting/getting parameters in a way that mimics sklearn's API.
+
+    Parameters
+    ----------
+    # configuration parameters
+    lr : float, optional
+        Learning rate for the optimizer. Default is 1e-4.
+    lr_patience : int, optional
+        Number of epochs with no improvement on the validation loss to wait before reducing the learning rate. Default is 10.
+    weight_decay : float, optional
+        Weight decay (L2 penalty) coefficient. Default is 1e-6.
+    lr_factor : float, optional
+        Factor by which the learning rate will be reduced. Default is 0.1.
+    d_model : int, optional
+        Dimension of the model. Default is 64.
+    n_layers : int, optional
+        Number of layers. Default is 8.
+    expand_factor : int, optional
+        Expansion factor. Default is 2.
+    bias : bool, optional
+        Whether to use bias. Default is False.
+    d_conv : int, optional
+        Dimension of the convolution. Default is 16.
+    conv_bias : bool, optional
+        Whether to use bias in the convolution. Default is True.
+    dropout : float, optional
+        Dropout rate in the mamba blocks. Default is 0.05.
+    dt_rank : str, optional
+        Rank of the time dimension. Default is "auto".
+    d_state : int, optional
+        State dimension. Default is 16.
+    dt_scale : float, optional
+        Scale of the time dimension. Default is 1.0.
+    dt_init : str, optional
+        Initialization method for the time dimension. Default is "random".
+    dt_max : float, optional
+        Maximum value for the time dimension. Default is 0.1.
+    dt_min : float, optional
+        Minimum value for the time dimension. Default is 1e-3.
+    dt_init_floor : float, optional
+        Floor value for the time dimension initialization. Default is 1e-4.
+    norm : str, optional
+        Normalization method. Default is 'RMSNorm'.
+    activation : callable, optional
+        Activation function. Default is nn.SELU().
+    num_embedding_activation : callable, optional
+        Activation function for numerical embeddings. Default is nn.Identity().
+    head_layer_sizes : list, optional
+        Sizes of the layers in the head. Default is [64, 64, 32].
+    head_dropout : float, optional
+        Dropout rate for the head. Default is 0.5.
+    head_skip_layers : bool, optional
+        Whether to use skip layers in the head. Default is False.
+    head_activation : callable, optional
+        Activation function for the head. Default is nn.SELU().
+    head_use_batch_norm : bool, optional
+        Whether to use batch normalization in the head. Default is False.
+
+    # Preprocessor Parameters
+    n_bins : int, optional
+        The number of bins to use for numerical feature binning. Default is 50.
+    numerical_preprocessing : str, optional
+        The preprocessing strategy for numerical features. Default is 'ple'.
+    use_decision_tree_bins : bool, optional
+        If True, uses decision tree regression/classification to determine optimal bin edges for numerical feature binning. Default is False.
+    binning_strategy : str, optional
+        Defines the strategy for binning numerical features. Default is 'uniform'.
+    task : str, optional
+        Indicates the type of machine learning task ('regression' or 'classification'). Default is 'regression'.
+    cat_cutoff: float or int, optional
+        Indicates the cutoff after which integer values are treated as categorical. If float, it's treated as a percentage. If int, it's the maximum number of unique values for a column to be considered categorical. Default is 3%
+    treat_all_integers_as_numerical : bool, optional
+        If True, all integer columns will be treated as numerical, regardless of their unique value count or proportion. Default is False
+
+
+    Attributes
+    ----------
+    config : MambularConfig
+        Configuration object containing model-specific parameters.
+    preprocessor : Preprocessor
+        Preprocessor object for data preprocessing steps.
+    model : BaseEmbeddingMambularRegressor
+        The neural network model, initialized after the `fit` method is called.
+    """
+
+    def __init__(self, **kwargs):
+        # Known config arguments
+        config_arg_names = [
+            "lr",
+            "lr_patience",
+            "weight_decay",
+            "lr_factor",
+            "d_model",
+            "n_layers",
+            "expand_factor",
+            "bias",
+            "d_conv",
+            "conv_bias",
+            "dropout",
+            "dt_rank",
+            "d_state",
+            "dt_scale",
+            "dt_init",
+            "dt_max",
+            "dt_min",
+            "dt_init_floor",
+            "norm",
+            "activation",
+            "num_embedding_activation",
+            "head_layer_sizes",
+            "head_dropout",
+            "head_skip_layers",
+            "head_activation",
+            "head_use_batch_norm",
+        ]
+
+        preprocessor_arg_names = [
+            "n_bins",
+            "numerical_preprocessing",
+            "use_decision_tree_bins",
+            "binning_strategy",
+            "task",
+            "cat_cutoff",
+            "treat_all_integers_as_numerical",
+        ]
+
+        self.config_kwargs = {k: v for k,
+                              v in kwargs.items() if k in config_arg_names}
+        self.config = DefaultMambularConfig(**self.config_kwargs)
+
+        preprocessor_kwargs = {
+            k: v for k, v in kwargs.items() if k in preprocessor_arg_names
+        }
+        if "numerical_preprocessing" not in list(preprocessor_kwargs.keys()):
+            preprocessor_kwargs["numerical_preprocessing"] = "standardization"
+
+        self.preprocessor = Preprocessor(**preprocessor_kwargs)
+        self.model = None
+
+        # Raise a warning if task is set to 'classification'
+        if preprocessor_kwargs.get("task") == "classification":
+            warnings.warn(
+                "The task is set to 'classification'. MambularRegressor is designed for regression tasks.",
+                UserWarning,
+            )
+
+    def get_params(self, deep=True):
+        """
+        Get parameters for this estimator. Overrides the BaseEstimator method.
+
+        Parameters
+        ----------
+        deep : bool, default=True
+            If True, returns the parameters for this estimator and contained sub-objects that are estimators.
+
+        Returns
+        -------
+        params : dict
+            Parameter names mapped to their values.
+        """
+        params = self.config_kwargs  # Parameters used to initialize MambularConfig
+
+        # If deep=True, include parameters from nested components like preprocessor
+        if deep:
+            # Assuming Preprocessor has a get_params method
+            preprocessor_params = {
+                "preprocessor__" + key: value
+                for key, value in self.preprocessor.get_params().items()
+            }
+            params.update(preprocessor_params)
+
+        return params
+
+    def set_params(self, **parameters):
+        """
+        Set the parameters of this estimator. Overrides the BaseEstimator method.
+
+        Parameters
+        ----------
+        **parameters : dict
+            Estimator parameters to be set.
+
+
+        Returns
+        -------
+        self : object
+            The instance with updated parameters.
+        """
+        # Update config_kwargs with provided parameters
+        valid_config_keys = self.config_kwargs.keys()
+        config_updates = {k: v for k,
+                          v in parameters.items() if k in valid_config_keys}
+        self.config_kwargs.update(config_updates)
+
+        # Update the config object
+        for key, value in config_updates.items():
+            setattr(self.config, key, value)
+
+        # Handle preprocessor parameters (prefixed with 'preprocessor__')
+        preprocessor_params = {
+            k.split("__")[1]: v
+            for k, v in parameters.items()
+            if k.startswith("preprocessor__")
+        }
+        if preprocessor_params:
+            # Assuming Preprocessor has a set_params method
+            self.preprocessor.set_params(**preprocessor_params)
+
+        return self
+
+    def split_data(self, X, y, val_size, random_state):
+        """
+        Splits the dataset into training and validation sets.
+
+        Parameters
+        ----------
+        X : array-like or DataFrame, shape (n_samples, n_features)
+            Input features.
+        y : array-like, shape (n_samples,) or (n_samples, n_targets)
+            Target values.
+        val_size : float
+            The proportion of the dataset to include in the validation split.
+        random_state : int
+            Controls the shuffling applied to the data before applying the split.
+
+
+        Returns
+        -------
+        X_train, X_val, y_train, y_val : arrays
+            The split datasets.
+        """
+        X_train, X_val, y_train, y_val = train_test_split(
+            X, y, test_size=val_size, random_state=random_state
+        )
+
+        return X_train, X_val, y_train, y_val
+
+    def preprocess_data(self, X_train, y_train, X_val, y_val, batch_size, shuffle):
+        """
+        Preprocesses the training and validation data, and creates DataLoaders for them.
+
+        Parameters
+        ----------
+        X_train : DataFrame or array-like, shape (n_samples_train, n_features)
+            Training feature set.
+        y_train : array-like, shape (n_samples_train,)
+            Training target values.
+        X_val : DataFrame or array-like, shape (n_samples_val, n_features)
+            Validation feature set.
+        y_val : array-like, shape (n_samples_val,)
+            Validation target values.
+        batch_size : int
+            Size of batches for the DataLoader.
+        shuffle : bool
+            Whether to shuffle the training data in the DataLoader.
+
+
+        Returns
+        -------
+        data_module : MambularDataModule
+            An instance of MambularDataModule containing the training and validation DataLoaders.
+        """
+        self.preprocessor.fit(
+            pd.concat([X_train, X_val], axis=0).reset_index(drop=True),
+            np.concatenate((y_train, y_val), axis=0),
+        )
+        train_preprocessed_data = self.preprocessor.transform(X_train)
+        val_preprocessed_data = self.preprocessor.transform(X_val)
+
+        # Update feature info based on the actual processed data
+        (
+            self.cat_feature_info,
+            self.num_feature_info,
+        ) = self.preprocessor.get_feature_info()
+
+        # Initialize lists for tensors
+        train_cat_tensors = []
+        train_num_tensors = []
+        val_cat_tensors = []
+        val_num_tensors = []
+
+        # Populate tensors for categorical features, if present in processed data
+        for key in self.cat_feature_info:
+            cat_key = "cat_" + key  # Assuming categorical keys are prefixed with 'cat_'
+            if cat_key in train_preprocessed_data:
+                train_cat_tensors.append(
+                    torch.tensor(
+                        train_preprocessed_data[cat_key], dtype=torch.long)
+                )
+            if cat_key in val_preprocessed_data:
+                val_cat_tensors.append(
+                    torch.tensor(
+                        val_preprocessed_data[cat_key], dtype=torch.long)
+                )
+
+            binned_key = "num_" + key  # for binned features
+            if binned_key in train_preprocessed_data:
+                train_cat_tensors.append(
+                    torch.tensor(
+                        train_preprocessed_data[binned_key], dtype=torch.long)
+                )
+
+            if binned_key in val_preprocessed_data:
+                val_cat_tensors.append(
+                    torch.tensor(
+                        val_preprocessed_data[binned_key], dtype=torch.long)
+                )
+
+        # Populate tensors for numerical features, if present in processed data
+        for key in self.num_feature_info:
+            num_key = "num_" + str(
+                key
+            )  # Assuming numerical keys are prefixed with 'num_'
+            if num_key in train_preprocessed_data:
+                train_num_tensors.append(
+                    torch.tensor(
+                        train_preprocessed_data[num_key], dtype=torch.float32)
+                )
+            if num_key in val_preprocessed_data:
+                val_num_tensors.append(
+                    torch.tensor(
+                        val_preprocessed_data[num_key], dtype=torch.float32)
+                )
+
+        train_labels = torch.tensor(y_train, dtype=torch.float32)
+        val_labels = torch.tensor(y_val, dtype=torch.float32)
+
+        # Create datasets
+        train_dataset = EmbeddingMambularDataset(
+            train_cat_tensors, train_num_tensors, train_labels
+        )
+        val_dataset = EmbeddingMambularDataset(
+            val_cat_tensors, val_num_tensors, val_labels
+        )
+
+        # Create dataloaders
+        train_dataloader = DataLoader(
+            train_dataset, batch_size=batch_size, shuffle=shuffle
+        )
+        val_dataloader = DataLoader(val_dataset, batch_size=batch_size)
+
+        return MambularDataModule(train_dataloader, val_dataloader)
+
+    def preprocess_test_data(self, X):
+        """
+        Preprocesses the test data and creates tensors for categorical and numerical features.
+
+        Parameters
+        ----------
+        X : DataFrame or array-like, shape (n_samples, n_features)
+            Test feature set.
+
+
+        Returns
+        -------
+        cat_tensors : list of Tensors
+            List of tensors for each categorical feature.
+        num_tensors : list of Tensors
+            List of tensors for each numerical feature.
+        """
+        processed_data = self.preprocessor.transform(X)
+
+        # Initialize lists for tensors
+        cat_tensors = []
+        num_tensors = []
+
+        # Populate tensors for categorical features
+        for key in self.cat_feature_info:
+            cat_key = "cat_" + str(
+                key
+            )  # Assuming categorical keys are prefixed with 'cat_'
+            if cat_key in processed_data:
+                cat_tensors.append(
+                    torch.tensor(processed_data[cat_key], dtype=torch.long)
+                )
+
+            binned_key = "num_" + str(key)  # for binned features
+            if binned_key in processed_data:
+                cat_tensors.append(
+                    torch.tensor(processed_data[binned_key], dtype=torch.long)
+                )
+
+        # Populate tensors for numerical features
+        for key in self.num_feature_info:
+            num_key = "num_" + str(
+                key
+            )  # Assuming numerical keys are prefixed with 'num_'
+            if num_key in processed_data:
+                num_tensors.append(
+                    torch.tensor(processed_data[num_key], dtype=torch.float32)
+                )
+
+        return cat_tensors, num_tensors
+
+    def fit(
+        self,
+        X,
+        y,
+        val_size=0.2,
+        X_val=None,
+        y_val=None,
+        max_epochs=100,
+        random_state=101,
+        batch_size=64,
+        shuffle=True,
+        patience=10,
+        monitor="val_loss",
+        mode="min",
+        lr=1e-3,
+        lr_patience=10,
+        factor=0.75,
+        weight_decay=0.025,
+        raw_embeddings=False,
+        seq_size=20,
+        pca=False,
+        **trainer_kwargs
+    ):
+        """
+        Fits the ProteinMambularRegressor model to the training data.
+
+        Parameters
+        ----------
+        X : array-like or DataFrame
+            The training input samples.
+        y : array-like
+            The target values (class labels for classification, real numbers for regression).
+        val_size : float, optional
+            The proportion of the dataset to include in the validation split if `X_val` is not provided.
+        X_val : array-like or DataFrame, optional
+            The validation input samples.
+        y_val : array-like, optional
+            The validation target values.
+        max_epochs : int, optional
+            The maximum number of epochs for training.
+        random_state : int, optional
+            The seed used by the random number generator.
+        batch_size : int, optional
+            Size of the batches for training.
+        shuffle : bool, optional
+            Whether to shuffle the training data.
+        patience : int, optional
+            Patience for early stopping.
+        monitor : str, optional
+            Quantity to be monitored for early stopping.
+        mode : str, optional
+            One of {'auto', 'min', 'max'}. In 'min' mode, training will stop when the quantity monitored has stopped decreasing;
+            in 'max' mode, it will stop when the quantity monitored has stopped increasing.
+        lr : float, optional
+            Learning rate for the optimizer.
+        lr_patience : int, optional
+            Number of epochs with no improvement after which the learning rate will be reduced.
+        factor : float, optional
+            Factor by which the learning rate will be reduced.
+        weight_decay : float, optional
+            Weight decay coefficient for regularization in the optimizer.
+        raw_embeddings : bool, optional
+            Whether to use raw numerical features directly or to process them into embeddings.
+        seq_size : int, optional
+            The sequence size for processing numerical features when not using raw embeddings.
+        **trainer_kwargs : dict
+            Additional keyword arguments for the PyTorch Lightning Trainer.
+
+        Returns
+        -------
+        self : object
+            Returns an instance of self.
+        """
+
+        if not isinstance(X, pd.DataFrame):
+            X = pd.DataFrame(X)
+        if X_val:
+            if not isinstance(X_val, pd.DataFrame):
+                X_val = pd.DataFrame(X_val)
+
+        # Apply PCA if indicated
+        if pca:
+            self.pca_transformer = PCA(n_components=seq_size)
+            X = pd.DataFrame(
+                self.pca_transformer.fit_transform(X)
+            )  # Fit and transform the PCA on the complete dataset
+            if X_val is not None:
+                X_val = pd.DataFrame(
+                    self.pca_transformer.transform(X_val)
+                )  # Transform validation data with the same PCA model
+
+            raw_embeddings = True
+
+        if not X_val:
+            X_train, X_val, y_train, y_val = self.split_data(
+                X, y, val_size, random_state
+            )
+        else:
+            X_train = X
+            y_train = y
+
+        data_module = self.preprocess_data(
+            X_train, y_train, X_val, y_val, batch_size, shuffle
+        )
+
+        if raw_embeddings:
+            self.config.d_model = X.shape[1]
+
+        self.model = BaseEmbeddingMambularRegressor(
+            config=self.config,
+            cat_feature_info=self.cat_feature_info,
+            num_feature_info=self.num_feature_info,
+            lr=lr,
+            lr_patience=lr_patience,
+            lr_factor=factor,
+            weight_decay=weight_decay,
+            raw_embeddings=raw_embeddings,
+            seq_size=seq_size,
+        )
+
+        early_stop_callback = EarlyStopping(
+            monitor=monitor, min_delta=0.00, patience=patience, verbose=False, mode=mode
+        )
+
+        checkpoint_callback = ModelCheckpoint(
+            monitor="val_loss",  # Adjust according to your validation metric
+            mode="min",
+            save_top_k=1,
+            dirpath="model_checkpoints",  # Specify the directory to save checkpoints
+            filename="best_model",
+        )
+
+        # Initialize the trainer and train the model
+        trainer = pl.Trainer(
+            max_epochs=max_epochs,
+            callbacks=[early_stop_callback, checkpoint_callback],
+            **trainer_kwargs
+        )
+        trainer.fit(self.model, data_module)
+
+        best_model_path = checkpoint_callback.best_model_path
+        if best_model_path:
+            checkpoint = torch.load(best_model_path)
+            self.model.load_state_dict(checkpoint["state_dict"])
+
+        return self
+
+    def predict(self, X):
+        """
+        Predicts target values for the given input samples.
+
+        Parameters
+        ----------
+        X : DataFrame or array-like, shape (n_samples, n_features)
+            The input samples for which to predict target values.
+
+
+        Returns
+        -------
+        predictions : ndarray, shape (n_samples,) or (n_samples, n_outputs)
+            The predicted target values.
+        """
+        # Preprocess the data
+        if not isinstance(X, pd.DataFrame):
+            X = pd.DataFrame(X)
+
+        if hasattr(self, "pca_transformer"):
+            X = pd.DataFrame(self.pca_transformer.transform(X))
+
+        device = next(self.model.parameters()).device
+        cat_tensors, num_tensors = self.preprocess_test_data(X)
+        if isinstance(cat_tensors, list):
+            cat_tensors = [tensor.to(device) for tensor in cat_tensors]
+        else:
+            cat_tensors = cat_tensors.to(device)
+
+        if isinstance(num_tensors, list):
+            num_tensors = [tensor.to(device) for tensor in num_tensors]
+        else:
+            num_tensors = num_tensors.to(device)
+
+        # Set the model to evaluation mode
+        self.model.eval()
+
+        # Perform inference
+        with torch.no_grad():
+            predictions = self.model(
+                num_features=num_tensors, cat_features=cat_tensors)
+
+        # Convert predictions to NumPy array and return
+        return predictions.cpu().numpy()
+
+    def evaluate(self, X, y_true, metrics=None):
+        """
+        Evaluate the model on the given data using specified metrics.
+
+        Parameters
+        ----------
+        X : array-like or pd.DataFrame of shape (n_samples, n_features)
+            The input samples to predict.
+        y_true : array-like of shape (n_samples,) or (n_samples, n_outputs)
+            The true target values against which to evaluate the predictions.
+        metrics : dict
+            A dictionary where keys are metric names and values are the metric functions.
+
+
+        Notes
+        -----
+        This method uses the `predict` method to generate predictions and computes each metric.
+
+
+        Examples
+        --------
+        >>> from sklearn.metrics import mean_squared_error, r2_score
+        >>> regressor = EmbeddingMambularRegressor()
+        >>> regressor.fit(X_train, y_train)
+        >>> metrics = {
+        ...     'Mean Squared Error': mean_squared_error,
+        ...     'R2 Score': r2_score
+        ... }
+        >>> # Assuming 'X_test' and 'y_test' are your test dataset and labels
+        >>> # Evaluate using the specified metrics
+        >>> results = regressor.evaluate(X_test, y_test, metrics=metrics)
+
+
+        Returns
+        -------
+        scores : dict
+            A dictionary with metric names as keys and their corresponding scores as values.
+
+        """
+        if metrics is None:
+            metrics = {"Mean Squared Error": mean_squared_error}
+
+        # Ensure input is in the correct format
+        if not isinstance(X, pd.DataFrame):
+            X = pd.DataFrame(X)
+
+        # Generate predictions using the trained model
+        predictions = self.predict(X)
+
+        # Initialize dictionary to store results
+        scores = {}
+
+        # Compute each metric
+        for metric_name, metric_func in metrics.items():
+            scores[metric_name] = metric_func(y_true, predictions)
+
+        return scores
```

### Comparing `mambular-0.1.2/mambular/models/sklearn_distributional.py` & `mambular-0.1.3/mambular/models/sklearn_regressor.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,556 +1,610 @@
-from sklearn.model_selection import train_test_split
-import pytorch_lightning as pl
-import torch
-from torch.utils.data import DataLoader
-from pytorch_lightning.callbacks import ModelCheckpoint, EarlyStopping
-from ..base_models.distributional import BaseMambularLSS
-from ..utils.config import MambularConfig
-from ..utils.preprocessor import Preprocessor
-from ..utils.dataset import MambularDataModule, MambularDataset
-from sklearn.base import BaseEstimator
-import pandas as pd
-from ..utils.distributional_metrics import (
-    poisson_deviance,
-    gamma_deviance,
-    beta_brier_score,
-    dirichlet_error,
-    student_t_loss,
-    negative_binomial_deviance,
-    inverse_gamma_loss,
-)
-from sklearn.metrics import mean_squared_error, accuracy_score
-import numpy as np
-import properscoring as ps
-
-
-class MambularLSS(BaseEstimator):
-    """
-    MambularLSS is a machine learning estimator that is designed for structured data,
-    incorporating both preprocessing and a deep learning model. The estimator
-    integrates configurable components for data preprocessing and the neural network model,
-    facilitating end-to-end training and prediction workflows.
-
-    The initialization of this class separates configuration arguments for the model and
-    the preprocessor, allowing for flexible adjustment of parameters.
-
-    Attributes
-    ----------
-    config : MambularConfig
-        Configuration object containing model-specific parameters.
-    preprocessor : Preprocessor
-        Preprocessor object for data preprocessing steps.
-    model : torch.nn.Module
-        The neural network model, initialized based on 'config'.
-
-    Parameters
-    ----------
-    **kwargs : Arbitrary keyword arguments, divided into configuration for the model and
-        preprocessing. Recognized keys include model parameters such as 'd_model',
-        'n_layers', etc., and any additional keys are assumed to be preprocessor arguments.
-    """
-
-    def __init__(self, **kwargs):
-        # Known config arguments
-        config_arg_names = [
-            "d_model",
-            "n_layers",
-            "dt_rank",
-            "output_dimension",
-            "pooling_method",
-            "norm",
-            "cls",
-            "dt_min",
-            "dt_max",
-            "dropout",
-            "bias",
-            "weight_decay",
-            "conv_bias",
-            "d_state",
-            "expand_factor",
-            "d_conv",
-            "dt_init",
-            "dt_scale",
-            "dt_init_floor",
-            "tabular_head_units",
-            "tabular_head_activation",
-            "tabular_head_dropout",
-            "num_emebedding_activation",
-        ]
-        config_kwargs = {k: v for k, v in kwargs.items() if k in config_arg_names}
-        self.config = MambularConfig(**config_kwargs)
-
-        # The rest are assumed to be preprocessor arguments
-        preprocessor_kwargs = {
-            k: v for k, v in kwargs.items() if k not in config_arg_names
-        }
-        self.preprocessor = Preprocessor(**preprocessor_kwargs)
-        self.model = None
-
-    def get_params(self, deep=True): 
-        """
-        Get parameters for this estimator, optionally including parameters from nested components
-        like the preprocessor.
-
-        Parameters
-        ----------
-        deep : bool, default=True
-            If True, return parameters of nested components.
-
-        Returns
-        -------
-        dict
-            A dictionary mapping parameter names to their values. For nested components,
-            parameter names are prefixed accordingly (e.g., 'preprocessor__<param_name>').
-        """
-        
-        params = self.config_kwargs  # Parameters used to initialize MambularConfig
-
-        # If deep=True, include parameters from nested components like preprocessor
-        if deep:
-            # Assuming Preprocessor has a get_params method
-            preprocessor_params = {
-                "preprocessor__" + key: value
-                for key, value in self.preprocessor.get_params().items()
-            }
-            params.update(preprocessor_params)
-
-        return params
-
-    def set_params(self, **parameters):
-        """
-        Set the parameters of this estimator, allowing for modifications to both the configuration
-        and preprocessor parameters. Parameters not recognized as configuration arguments are
-        assumed to be preprocessor arguments.
-
-        Parameters
-        ----------
-            **parameters: Arbitrary keyword arguments where keys are parameter names and values
-                          are the new parameter values.
-
-        Returns
-        -------
-            self: This instance with updated parameters.
-        """
-        # Update config_kwargs with provided parameters
-        valid_config_keys = self.config_kwargs.keys()
-        config_updates = {k: v for k, v in parameters.items() if k in valid_config_keys}
-        self.config_kwargs.update(config_updates)
-
-        # Update the config object
-        for key, value in config_updates.items():
-            setattr(self.config, key, value)
-
-        # Handle preprocessor parameters (prefixed with 'preprocessor__')
-        preprocessor_params = {
-            k.split("__")[1]: v
-            for k, v in parameters.items()
-            if k.startswith("preprocessor__")
-        }
-        if preprocessor_params:
-            # Assuming Preprocessor has a set_params method
-            self.preprocessor.set_params(**preprocessor_params)
-
-        return self
-
-    def split_data(self, X, y, val_size, random_state): 
-        """
-        Split the dataset into training and validation sets.
-
-        Parameters
-        ----------
-        X : array-like
-            Features of the dataset.
-        y : array-like
-            Target values.
-        val_size : float
-            The proportion of the dataset to include in the validation split.
-        random_state : int, optional
-            The seed used by the random number generator for reproducibility.
-
-        Returns
-        -------
-        tuple
-            A tuple containing split datasets (X_train, X_val, y_train, y_val).
-        """
-        X_train, X_val, y_train, y_val = train_test_split(
-            X, y, test_size=val_size, random_state=random_state
-        )
-
-        return X_train, X_val, y_train, y_val
-
-    def preprocess_data(self, X_train, y_train, X_val, y_val, batch_size, shuffle):
-        """
-        Preprocess the training and validation data, fit the preprocessor on the training data,
-        and transform both training and validation data. This method also initializes tensors
-        for categorical and numerical features and labels, and prepares DataLoader objects for
-        both datasets.
-
-        Parameters
-        ----------
-        X_train : array-like
-            Training features.
-        y_train : array-like
-            Training target values.
-        X_val : array-like
-            Validation features.
-        y_val : array-like
-            Validation target values.
-        batch_size : int
-            Batch size for DataLoader objects.
-        shuffle : bool
-            Whether to shuffle the training data in the DataLoader.
-
-        Returns
-        -------
-        MambularDataModule
-            An object containing DataLoaders for training and validation datasets.
-        """
-        train_preprocessed_data = self.preprocessor.fit_transform(X_train, y_train)
-        val_preprocessed_data = self.preprocessor.transform(X_val)
-
-        # Update feature info based on the actual processed data
-        (
-            self.cat_feature_info,
-            self.num_feature_info,
-        ) = self.preprocessor.get_feature_info()
-
-        # Initialize lists for tensors
-        train_cat_tensors = []
-        train_num_tensors = []
-        val_cat_tensors = []
-        val_num_tensors = []
-
-        # Populate tensors for categorical features, if present in processed data
-        for key in self.cat_feature_info:
-            cat_key = "cat_" + key  # Assuming categorical keys are prefixed with 'cat_'
-            if cat_key in train_preprocessed_data:
-                train_cat_tensors.append(
-                    torch.tensor(train_preprocessed_data[cat_key], dtype=torch.long)
-                )
-            if cat_key in val_preprocessed_data:
-                val_cat_tensors.append(
-                    torch.tensor(val_preprocessed_data[cat_key], dtype=torch.long)
-                )
-
-            binned_key = "num_" + key  # for binned features
-            if binned_key in train_preprocessed_data:
-                train_cat_tensors.append(
-                    torch.tensor(train_preprocessed_data[binned_key], dtype=torch.long)
-                )
-
-            if binned_key in val_preprocessed_data:
-                val_cat_tensors.append(
-                    torch.tensor(val_preprocessed_data[binned_key], dtype=torch.long)
-                )
-
-        # Populate tensors for numerical features, if present in processed data
-        for key in self.num_feature_info:
-            num_key = "num_" + key  # Assuming numerical keys are prefixed with 'num_'
-            if num_key in train_preprocessed_data:
-                train_num_tensors.append(
-                    torch.tensor(train_preprocessed_data[num_key], dtype=torch.float)
-                )
-            if num_key in val_preprocessed_data:
-                val_num_tensors.append(
-                    torch.tensor(val_preprocessed_data[num_key], dtype=torch.float)
-                )
-
-        train_labels = torch.tensor(y_train, dtype=torch.float)
-        val_labels = torch.tensor(y_val, dtype=torch.float)
-
-        # Create datasets
-        train_dataset = MambularDataset(
-            train_cat_tensors, train_num_tensors, train_labels
-        )
-        val_dataset = MambularDataset(val_cat_tensors, val_num_tensors, val_labels)
-
-        # Create dataloaders
-        train_dataloader = DataLoader(
-            train_dataset, batch_size=batch_size, shuffle=shuffle
-        )
-        val_dataloader = DataLoader(val_dataset, batch_size=batch_size)
-
-        return MambularDataModule(train_dataloader, val_dataloader)
-
-    def preprocess_test_data(self, X):
-        """
-        Preprocess test data using the fitted preprocessor. This method prepares tensors for
-        categorical and numerical features based on the preprocessed test data.
-
-        Parameters
-        ----------
-        X : array-like
-            Test features to preprocess.
-
-        Returns
-        -------
-        tuple
-            A tuple containing lists of tensors for categorical and numerical features.
-        """
-        processed_data = self.preprocessor.transform(X)
-
-        # Initialize lists for tensors
-        cat_tensors = []
-        num_tensors = []
-
-        # Populate tensors for categorical features
-        for key in self.cat_feature_info:
-            cat_key = "cat_" + key  # Assuming categorical keys are prefixed with 'cat_'
-            if cat_key in processed_data:
-                cat_tensors.append(
-                    torch.tensor(processed_data[cat_key], dtype=torch.long)
-                )
-
-            binned_key = "num_" + key  # for binned features
-            if binned_key in processed_data:
-                cat_tensors.append(
-                    torch.tensor(processed_data[binned_key], dtype=torch.long)
-                )
-
-        # Populate tensors for numerical features
-        for key in self.num_feature_info:
-            num_key = "num_" + key  # Assuming numerical keys are prefixed with 'num_'
-            if num_key in processed_data:
-                num_tensors.append(
-                    torch.tensor(processed_data[num_key], dtype=torch.float)
-                )
-
-        return cat_tensors, num_tensors
-
-    def fit(
-        self,
-        X,
-        y,
-        family,
-        val_size=0.2,
-        X_val=None,
-        y_val=None,
-        max_epochs=100,
-        random_state=101,
-        batch_size=64,
-        shuffle=True,
-        patience=10,
-        monitor="val_loss",
-        mode="min",
-        lr=1e-3,
-        lr_patience=10,
-        factor=0.75,
-        weight_decay=0.025,
-        **trainer_kwargs,
-    ):    
-        """
-        Fits the model to the provided data, using the specified loss distribution family for the prediction task.
-
-        Parameters
-        ----------
-        X : DataFrame or array-like, shape (n_samples, n_features)
-            Training features.
-        y : array-like, shape (n_samples,) or (n_samples, n_targets)
-            Target values for training.
-        family : str
-            The name of the distribution family to use for the loss function. Examples include 'normal' for regression tasks.
-        val_size : float, default=0.2
-            Proportion of the dataset to include in the validation split if `X_val` is None.
-        X_val : DataFrame or array-like, shape (n_samples, n_features), optional
-            Validation features. If provided, `X` and `y` are not split.
-        y_val : array-like, shape (n_samples,) or (n_samples, n_targets), optional
-            Validation target values. Required if `X_val` is provided.
-        max_epochs : int, default=100
-            Maximum number of epochs for training.
-        random_state : int, default=101
-            Seed used by the random number generator for shuffling the data.
-        batch_size : int, default=64
-            Number of samples per gradient update.
-        shuffle : bool, default=True
-            Whether to shuffle the training data before each epoch.
-        patience : int, default=10
-            Number of epochs with no improvement on the validation metric to wait before early stopping.
-        monitor : str, default="val_loss"
-            The metric to monitor for early stopping.
-        mode : str, default="min"
-            In 'min' mode, training will stop when the quantity monitored has stopped decreasing;
-            in 'max' mode, it will stop when the quantity monitored has stopped increasing.
-        lr : float, default=1e-3
-            Learning rate for the optimizer.
-        lr_patience : int, default=10
-            Number of epochs with no improvement on the validation metric to wait before reducing the learning rate.
-        factor : float, default=0.75
-            Factor by which the learning rate will be reduced.
-        weight_decay : float, default=0.025
-            Weight decay (L2 penalty) parameter.
-        **trainer_kwargs : dict
-            Additional keyword arguments for PyTorch Lightning's Trainer class.
-
-        Returns
-        -------
-        self : object
-            The fitted estimator.
-        """
-        if not isinstance(X, pd.DataFrame):
-            X = pd.DataFrame(X)
-        if X_val:
-            if not isinstance(X_val, pd.DataFrame):
-                X_val = pd.DataFrame(X_val)
-
-        if not X_val:
-            X_train, X_val, y_train, y_val = self.split_data(
-                X, y, val_size, random_state
-            )
-
-        data_module = self.preprocess_data(
-            X_train, y_train, X_val, y_val, batch_size, shuffle
-        )
-
-        self.model = BaseMambularLSS(
-            family=family,
-            config=self.config,
-            cat_feature_info=self.cat_feature_info,
-            num_feature_info=self.num_feature_info,
-            lr=lr,
-            lr_patience=lr_patience,
-            lr_factor=factor,
-            weight_decay=weight_decay,
-        )
-
-        early_stop_callback = EarlyStopping(
-            monitor=monitor, min_delta=0.00, patience=patience, verbose=False, mode=mode
-        )
-
-        checkpoint_callback = ModelCheckpoint(
-            monitor="val_loss",
-            mode="min",
-            save_top_k=1,
-            dirpath="model_checkpoints",
-            filename="best_model",
-        )
-
-        # Initialize the trainer and train the model
-        trainer = pl.Trainer(
-            max_epochs=max_epochs,
-            callbacks=[early_stop_callback, checkpoint_callback],
-            **trainer_kwargs,
-        )
-        trainer.fit(self.model, data_module)
-
-        best_model_path = checkpoint_callback.best_model_path
-        if best_model_path:
-            checkpoint = torch.load(best_model_path)
-            self.model.load_state_dict(checkpoint["state_dict"])
-
-        return self
-
-    def predict(self, X):
-        """
-        Predicts target values for the given input samples using the fitted model.
-
-        Parameters
-        ----------
-        X : DataFrame or array-like, shape (n_samples, n_features)
-            The input samples for which to predict target values.
-
-        Returns
-        -------
-        predictions : ndarray, shape (n_samples,) or (n_samples, n_distributional_parameters)
-            The predicted target values.
-        """
-        # Preprocess the data
-        if not isinstance(X, pd.DataFrame):
-            X = pd.DataFrame(X)
-        device = next(self.model.parameters()).device
-        cat_tensors, num_tensors = self.preprocess_test_data(X)
-        if isinstance(cat_tensors, list):
-            cat_tensors = [tensor.to(device) for tensor in cat_tensors]
-        else:
-            cat_tensors = cat_tensors.to(device)
-
-        if isinstance(num_tensors, list):
-            num_tensors = [tensor.to(device) for tensor in num_tensors]
-        else:
-            num_tensors = num_tensors.to(device)
-
-        # Set the model to evaluation mode
-        self.model.eval()
-
-        # Perform inference
-        with torch.no_grad():
-            predictions = self.model(cat_tensors, num_tensors)
-
-        # Convert predictions to NumPy array and return
-        return predictions.cpu().numpy()
-
-    def evaluate(self, X, y_true, metrics=None, distribution_family=None):
-        """
-        Evaluate the model on the given data using specified metrics tailored to the distribution type.
-
-        Parameters
-        ----------
-        X : DataFrame or array-like, shape (n_samples, n_features)
-            Input samples.
-        y_true : DataFrame or array-like, shape (n_samples,) or (n_samples, n_outputs)
-            True target values.
-        metrics : dict, optional
-            A dictionary where keys are metric names and values are the metric functions.
-            If None, default metrics based on the detected or specified distribution_family are used.
-        distribution_family : str, optional
-            Specifies the distribution family the model is predicting for. If None, it will attempt to infer based
-            on the model's settings.
-
-        Returns
-        -------
-        scores : dict
-            A dictionary with metric names as keys and their corresponding scores as values.
-        """
-        # Infer distribution family from model settings if not provided
-        if distribution_family is None:
-            distribution_family = getattr(self.model, "distribution_family", "normal")
-
-        # Setup default metrics if none are provided
-        if metrics is None:
-            metrics = self.get_default_metrics(distribution_family)
-
-        # Make predictions
-        predictions = self.predict(X)
-
-        # Initialize dictionary to store results
-        scores = {}
-
-        # Compute each metric
-        for metric_name, metric_func in metrics.items():
-            scores[metric_name] = metric_func(y_true, predictions)
-
-        return scores
-
-    def get_default_metrics(self, distribution_family):
-        """
-        Provides default metrics based on the distribution family.
-
-        Parameters
-        ----------
-        distribution_family : str
-            The distribution family for which to provide default metrics.
-
-        Returns
-        -------
-        metrics : dict
-            A dictionary of default metric functions.
-        """
-        default_metrics = {
-            "normal": {
-                "MSE": lambda y, pred: mean_squared_error(y, pred[:, 0]),
-                "CRPS": lambda y, pred: np.mean(
-                    [
-                        ps.crps_gaussian(y[i], mu=pred[i, 0], sig=np.sqrt(pred[i, 1]))
-                        for i in range(len(y))
-                    ]
-                ),
-            },
-            "poisson": {"Poisson Deviance": poisson_deviance},
-            "gamma": {"Gamma Deviance": gamma_deviance},
-            "beta": {"Brier Score": beta_brier_score},
-            "dirichlet": {"Dirichlet Error": dirichlet_error},
-            "studentt": {"Student-T Loss": student_t_loss},
-            "negativebinom": {"Negative Binomial Deviance": negative_binomial_deviance},
-            "inversegamma": {"Inverse Gamma Loss": inverse_gamma_loss},
-            "categorical": {"Accuracy": accuracy_score},
-        }
-        return default_metrics.get(distribution_family, {})
+import lightning as pl
+import pandas as pd
+import torch
+from lightning.pytorch.callbacks import EarlyStopping, ModelCheckpoint
+from sklearn.base import BaseEstimator
+from sklearn.metrics import mean_squared_error
+from sklearn.model_selection import train_test_split
+from torch.utils.data import DataLoader
+import warnings
+import numpy as np
+from ..base_models.regressor import BaseMambularRegressor
+from ..utils.dataset import MambularDataModule, MambularDataset
+from ..utils.preprocessor import Preprocessor
+from ..utils.configs import DefaultMambularConfig
+
+
+class MambularRegressor(BaseEstimator):
+    """
+    A regressor implemented using PyTorch Lightning that follows the scikit-learn API conventions.
+    This class is designed to work with tabular data, offering a straightforward way to specify
+    model configurations and preprocessing steps. It integrates seamlessly with scikit-learn's tools
+    such as cross-validation and grid search.
+
+    Parameters
+    ----------
+    # configuration parameters
+    lr : float, optional
+        Learning rate for the optimizer. Default is 1e-4.
+    lr_patience : int, optional
+        Number of epochs with no improvement on the validation loss to wait before reducing the learning rate. Default is 10.
+    weight_decay : float, optional
+        Weight decay (L2 penalty) coefficient. Default is 1e-6.
+    lr_factor : float, optional
+        Factor by which the learning rate will be reduced. Default is 0.1.
+    d_model : int, optional
+        Dimension of the model. Default is 64.
+    n_layers : int, optional
+        Number of layers. Default is 8.
+    expand_factor : int, optional
+        Expansion factor. Default is 2.
+    bias : bool, optional
+        Whether to use bias. Default is False.
+    d_conv : int, optional
+        Dimension of the convolution. Default is 16.
+    conv_bias : bool, optional
+        Whether to use bias in the convolution. Default is True.
+    dropout : float, optional
+        Dropout rate in the mamba blocks. Default is 0.05.
+    dt_rank : str, optional
+        Rank of the time dimension. Default is "auto".
+    d_state : int, optional
+        State dimension. Default is 16.
+    dt_scale : float, optional
+        Scale of the time dimension. Default is 1.0.
+    dt_init : str, optional
+        Initialization method for the time dimension. Default is "random".
+    dt_max : float, optional
+        Maximum value for the time dimension. Default is 0.1.
+    dt_min : float, optional
+        Minimum value for the time dimension. Default is 1e-3.
+    dt_init_floor : float, optional
+        Floor value for the time dimension initialization. Default is 1e-4.
+    norm : str, optional
+        Normalization method. Default is 'RMSNorm'.
+    activation : callable, optional
+        Activation function. Default is nn.SELU().
+    num_embedding_activation : callable, optional
+        Activation function for numerical embeddings. Default is nn.Identity().
+    head_layer_sizes : list, optional
+        Sizes of the layers in the head. Default is [64, 64, 32].
+    head_dropout : float, optional
+        Dropout rate for the head. Default is 0.5.
+    head_skip_layers : bool, optional
+        Whether to use skip layers in the head. Default is False.
+    head_activation : callable, optional
+        Activation function for the head. Default is nn.SELU().
+    head_use_batch_norm : bool, optional
+        Whether to use batch normalization in the head. Default is False.
+
+    # Preprocessor Parameters
+    n_bins : int, optional
+        The number of bins to use for numerical feature binning. Default is 50.
+    numerical_preprocessing : str, optional
+        The preprocessing strategy for numerical features. Default is 'ple'.
+    use_decision_tree_bins : bool, optional
+        If True, uses decision tree regression/classification to determine optimal bin edges for numerical feature binning. Default is False.
+    binning_strategy : str, optional
+        Defines the strategy for binning numerical features. Default is 'uniform'.
+    task : str, optional
+        Indicates the type of machine learning task ('regression' or 'classification'). Default is 'regression'.
+    cat_cutoff: float or int, optional
+        Indicates the cutoff after which integer values are treated as categorical. If float, it's treated as a percentage. If int, it's the maximum number of unique values for a column to be considered categorical. Default is 3%
+    treat_all_integers_as_numerical : bool, optional
+        If True, all integer columns will be treated as numerical, regardless of their unique value count or proportion. Default is False
+
+
+
+    Attributes
+    ----------
+    config : DefaultConfig
+        An object storing the configuration settings for the model.
+    preprocessor : Preprocessor
+        An object responsible for preprocessing the input data, such as encoding categorical variables and scaling numerical features.
+    model : BaseMambularRegressor or None
+        The underlying regression model, which is a PyTorch Lightning module. It is instantiated when the `fit` method is called.
+    """
+
+    def __init__(self, **kwargs):
+        # Known config arguments
+        config_arg_names = [
+            "lr",
+            "lr_patience",
+            "weight_decay",
+            "lr_factor",
+            "d_model",
+            "n_layers",
+            "expand_factor",
+            "bias",
+            "d_conv",
+            "conv_bias",
+            "dropout",
+            "dt_rank",
+            "d_state",
+            "dt_scale",
+            "dt_init",
+            "dt_max",
+            "dt_min",
+            "dt_init_floor",
+            "norm",
+            "activation",
+            "num_embedding_activation",
+            "head_layer_sizes",
+            "head_dropout",
+            "head_skip_layers",
+            "head_activation",
+            "head_use_batch_norm",
+        ]
+
+        preprocessor_arg_names = [
+            "n_bins",
+            "numerical_preprocessing",
+            "use_decision_tree_bins",
+            "binning_strategy",
+            "task",
+            "cat_cutoff",
+            "treat_all_integers_as_numerical",
+        ]
+
+        self.config_kwargs = {k: v for k, v in kwargs.items() if k in config_arg_names}
+        self.config = DefaultMambularConfig(**self.config_kwargs)
+
+        preprocessor_kwargs = {
+            k: v for k, v in kwargs.items() if k in preprocessor_arg_names
+        }
+
+        self.preprocessor = Preprocessor(**preprocessor_kwargs)
+        self.model = None
+
+        # Raise a warning if task is set to 'classification'
+        if preprocessor_kwargs.get("task") == "classification":
+            warnings.warn(
+                "The task is set to 'classification'. MambularRegressor is designed for regression tasks.",
+                UserWarning,
+            )
+
+    def get_params(self, deep=True):
+        """
+        Get parameters for this estimator. Overrides the BaseEstimator method.
+
+        Parameters
+        ----------
+        deep : bool, default=True
+            If True, returns the parameters for this estimator and contained sub-objects that are estimators.
+
+        Returns
+        -------
+        params : dict
+            Parameter names mapped to their values.
+        """
+        params = self.config_kwargs  # Parameters used to initialize DefaultConfig
+
+        # If deep=True, include parameters from nested components like preprocessor
+        if deep:
+            # Assuming Preprocessor has a get_params method
+            preprocessor_params = {
+                "preprocessor__" + key: value
+                for key, value in self.preprocessor.get_params().items()
+            }
+            params.update(preprocessor_params)
+
+        return params
+
+    def set_params(self, **parameters):
+        """
+        Set the parameters of this estimator. Overrides the BaseEstimator method.
+
+        Parameters
+        ----------
+        **parameters : dict
+            Estimator parameters to be set.
+
+        Returns
+        -------
+        self : object
+            The instance with updated parameters.
+        """
+        # Update config_kwargs with provided parameters
+        valid_config_keys = self.config_kwargs.keys()
+        config_updates = {k: v for k, v in parameters.items() if k in valid_config_keys}
+        self.config_kwargs.update(config_updates)
+
+        # Update the config object
+        for key, value in config_updates.items():
+            setattr(self.config, key, value)
+
+        # Handle preprocessor parameters (prefixed with 'preprocessor__')
+        preprocessor_params = {
+            k.split("__")[1]: v
+            for k, v in parameters.items()
+            if k.startswith("preprocessor__")
+        }
+        if preprocessor_params:
+            # Assuming Preprocessor has a set_params method
+            self.preprocessor.set_params(**preprocessor_params)
+
+        return self
+
+    def split_data(self, X, y, val_size, random_state):
+        """
+        Splits the dataset into training and validation sets.
+
+        Parameters
+        ----------
+        X : array-like or DataFrame, shape (n_samples, n_features)
+            Input features.
+        y : array-like, shape (n_samples,) or (n_samples, n_targets)
+            Target values.
+        val_size : float
+            The proportion of the dataset to include in the validation split.
+        random_state : int
+            Controls the shuffling applied to the data before applying the split.
+
+
+        Returns
+        -------
+        X_train, X_val, y_train, y_val : arrays
+            The split datasets.
+        """
+        X_train, X_val, y_train, y_val = train_test_split(
+            X, y, test_size=val_size, random_state=random_state
+        )
+
+        return X_train, X_val, y_train, y_val
+
+    def preprocess_data(self, X_train, y_train, X_val, y_val, batch_size, shuffle):
+        """
+        Preprocesses the training and validation data, and creates DataLoaders for them.
+
+        Parameters
+        ----------
+        X_train : DataFrame or array-like, shape (n_samples_train, n_features)
+            Training feature set.
+        y_train : array-like, shape (n_samples_train,)
+            Training target values.
+        X_val : DataFrame or array-like, shape (n_samples_val, n_features)
+            Validation feature set.
+        y_val : array-like, shape (n_samples_val,)
+            Validation target values.
+        batch_size : int
+            Size of batches for the DataLoader.
+        shuffle : bool
+            Whether to shuffle the training data in the DataLoader.
+
+
+        Returns
+        -------
+        data_module : MambularDataModule
+            An instance of MambularDataModule containing the training and validation DataLoaders.
+        """
+        self.preprocessor.fit(
+            pd.concat([X_train, X_val], axis=0).reset_index(drop=True),
+            np.concatenate((y_train, y_val), axis=0),
+        )
+        train_preprocessed_data = self.preprocessor.transform(X_train)
+        val_preprocessed_data = self.preprocessor.transform(X_val)
+
+        # Update feature info based on the actual processed data
+        (
+            self.cat_feature_info,
+            self.num_feature_info,
+        ) = self.preprocessor.get_feature_info()
+
+        # Initialize lists for tensors
+        train_cat_tensors = []
+        train_num_tensors = []
+        val_cat_tensors = []
+        val_num_tensors = []
+
+        # Populate tensors for categorical features, if present in processed data
+        for key in self.cat_feature_info:
+            cat_key = "cat_" + key  # Assuming categorical keys are prefixed with 'cat_'
+            if cat_key in train_preprocessed_data:
+                train_cat_tensors.append(
+                    torch.tensor(train_preprocessed_data[cat_key], dtype=torch.long)
+                )
+            if cat_key in val_preprocessed_data:
+                val_cat_tensors.append(
+                    torch.tensor(val_preprocessed_data[cat_key], dtype=torch.long)
+                )
+
+            binned_key = "num_" + key  # for binned features
+            if binned_key in train_preprocessed_data:
+                train_cat_tensors.append(
+                    torch.tensor(train_preprocessed_data[binned_key], dtype=torch.long)
+                )
+
+            if binned_key in val_preprocessed_data:
+                val_cat_tensors.append(
+                    torch.tensor(val_preprocessed_data[binned_key], dtype=torch.long)
+                )
+
+        # Populate tensors for numerical features, if present in processed data
+        for key in self.num_feature_info:
+            num_key = "num_" + key  # Assuming numerical keys are prefixed with 'num_'
+            if num_key in train_preprocessed_data:
+                train_num_tensors.append(
+                    torch.tensor(train_preprocessed_data[num_key], dtype=torch.float32)
+                )
+            if num_key in val_preprocessed_data:
+                val_num_tensors.append(
+                    torch.tensor(val_preprocessed_data[num_key], dtype=torch.float32)
+                )
+
+        train_labels = torch.tensor(y_train, dtype=torch.float32)
+        val_labels = torch.tensor(y_val, dtype=torch.float32)
+
+        # Create datasets
+        train_dataset = MambularDataset(
+            train_cat_tensors, train_num_tensors, train_labels
+        )
+        val_dataset = MambularDataset(val_cat_tensors, val_num_tensors, val_labels)
+
+        # Create dataloaders
+        train_dataloader = DataLoader(
+            train_dataset, batch_size=batch_size, shuffle=shuffle
+        )
+        val_dataloader = DataLoader(val_dataset, batch_size=batch_size)
+
+        return MambularDataModule(train_dataloader, val_dataloader)
+
+    def preprocess_test_data(self, X):
+        """
+        Preprocesses the test data and creates tensors for categorical and numerical features.
+
+        Parameters
+        ----------
+        X : DataFrame or array-like, shape (n_samples, n_features)
+            Test feature set.
+
+
+        Returns
+        -------
+        cat_tensors : list of Tensors
+            List of tensors for each categorical feature.
+        num_tensors : list of Tensors
+            List of tensors for each numerical feature.
+        """
+        processed_data = self.preprocessor.transform(X)
+
+        # Initialize lists for tensors
+        cat_tensors = []
+        num_tensors = []
+
+        # Populate tensors for categorical features
+        for key in self.cat_feature_info:
+            cat_key = "cat_" + key  # Assuming categorical keys are prefixed with 'cat_'
+            if cat_key in processed_data:
+                cat_tensors.append(
+                    torch.tensor(processed_data[cat_key], dtype=torch.long)
+                )
+
+            binned_key = "num_" + key  # for binned features
+            if binned_key in processed_data:
+                cat_tensors.append(
+                    torch.tensor(processed_data[binned_key], dtype=torch.long)
+                )
+
+        # Populate tensors for numerical features
+        for key in self.num_feature_info:
+            num_key = "num_" + key  # Assuming numerical keys are prefixed with 'num_'
+            if num_key in processed_data:
+                num_tensors.append(
+                    torch.tensor(processed_data[num_key], dtype=torch.float32)
+                )
+
+        return cat_tensors, num_tensors
+
+    def fit(
+        self,
+        X,
+        y,
+        val_size: float = 0.2,
+        X_val=None,
+        y_val=None,
+        max_epochs: int = 100,
+        random_state: int = 101,
+        batch_size: int = 128,
+        shuffle: bool = True,
+        patience: int = 15,
+        monitor: str = "val_loss",
+        mode: str = "min",
+        lr: float = 1e-4,
+        lr_patience: int = 10,
+        factor: float = 0.1,
+        weight_decay: float = 1e-06,
+        **trainer_kwargs
+    ):
+        """
+        Trains the regression model using the provided training data. Optionally, a separate validation set can be used.
+
+        Parameters
+        ----------
+        X : DataFrame or array-like, shape (n_samples, n_features)
+            The training input samples.
+        y : array-like, shape (n_samples,) or (n_samples, n_targets)
+            The target values (real numbers).
+        val_size : float, default=0.2
+            The proportion of the dataset to include in the validation split if `X_val` is None. Ignored if `X_val` is provided.
+        X_val : DataFrame or array-like, shape (n_samples, n_features), optional
+            The validation input samples. If provided, `X` and `y` are not split and this data is used for validation.
+        y_val : array-like, shape (n_samples,) or (n_samples, n_targets), optional
+            The validation target values. Required if `X_val` is provided.
+        max_epochs : int, default=100
+            Maximum number of epochs for training.
+        random_state : int, default=101
+            Controls the shuffling applied to the data before applying the split.
+        batch_size : int, default=64
+            Number of samples per gradient update.
+        shuffle : bool, default=True
+            Whether to shuffle the training data before each epoch.
+        patience : int, default=10
+            Number of epochs with no improvement on the validation loss to wait before early stopping.
+        monitor : str, default="val_loss"
+            The metric to monitor for early stopping.
+        mode : str, default="min"
+            Whether the monitored metric should be minimized (`min`) or maximized (`max`).
+        lr : float, default=1e-3
+            Learning rate for the optimizer.
+        lr_patience : int, default=10
+            Number of epochs with no improvement on the validation loss to wait before reducing the learning rate.
+        factor : float, default=0.1
+            Factor by which the learning rate will be reduced.
+        weight_decay : float, default=0.025
+            Weight decay (L2 penalty) coefficient.
+        **trainer_kwargs : Additional keyword arguments for PyTorch Lightning's Trainer class.
+
+
+        Returns
+        -------
+        self : object
+            The fitted regressor.
+        """
+        if not isinstance(X, pd.DataFrame):
+            X = pd.DataFrame(X)
+        if X_val:
+            if not isinstance(X_val, pd.DataFrame):
+                X_val = pd.DataFrame(X_val)
+
+        if not X_val:
+            X_train, X_val, y_train, y_val = self.split_data(
+                X, y, val_size, random_state
+            )
+
+        self.data_module = self.preprocess_data(
+            X_train, y_train, X_val, y_val, batch_size, shuffle
+        )
+
+        self.model = BaseMambularRegressor(
+            config=self.config,
+            cat_feature_info=self.cat_feature_info,
+            num_feature_info=self.num_feature_info,
+            lr=lr,
+            lr_patience=lr_patience,
+            lr_factor=factor,
+            weight_decay=weight_decay,
+        )
+
+        early_stop_callback = EarlyStopping(
+            monitor=monitor, min_delta=0.00, patience=patience, verbose=False, mode=mode
+        )
+
+        checkpoint_callback = ModelCheckpoint(
+            monitor="val_loss",  # Adjust according to your validation metric
+            mode="min",
+            save_top_k=1,
+            dirpath="model_checkpoints",  # Specify the directory to save checkpoints
+            filename="best_model",
+        )
+
+        # Initialize the trainer and train the model
+        trainer = pl.Trainer(
+            max_epochs=max_epochs,
+            callbacks=[early_stop_callback, checkpoint_callback],
+            **trainer_kwargs
+        )
+        trainer.fit(self.model, self.data_module)
+
+        best_model_path = checkpoint_callback.best_model_path
+        if best_model_path:
+            checkpoint = torch.load(best_model_path)
+            self.model.load_state_dict(checkpoint["state_dict"])
+
+        return self
+
+    def predict(self, X):
+        """
+        Predicts target values for the given input samples.
+
+        Parameters
+        ----------
+        X : DataFrame or array-like, shape (n_samples, n_features)
+            The input samples for which to predict target values.
+
+
+        Returns
+        -------
+        predictions : ndarray, shape (n_samples,) or (n_samples, n_outputs)
+            The predicted target values.
+        """
+        # Preprocess the data
+        if not isinstance(X, pd.DataFrame):
+            X = pd.DataFrame(X)
+        device = next(self.model.parameters()).device
+        cat_tensors, num_tensors = self.preprocess_test_data(X)
+        if isinstance(cat_tensors, list):
+            cat_tensors = [tensor.to(device) for tensor in cat_tensors]
+        else:
+            cat_tensors = cat_tensors.to(device)
+
+        if isinstance(num_tensors, list):
+            num_tensors = [tensor.to(device) for tensor in num_tensors]
+        else:
+            num_tensors = num_tensors.to(device)
+
+        # Set the model to evaluation mode
+        self.model.eval()
+
+        # Perform inference
+        with torch.no_grad():
+            predictions = self.model(num_features=num_tensors, cat_features=cat_tensors)
+
+        # Convert predictions to NumPy array and return
+        return predictions.cpu().numpy()
+
+    def evaluate(self, X, y_true, metrics=None):
+        """
+        Evaluate the model on the given data using specified metrics.
+
+        Parameters
+        ----------
+        X : array-like or pd.DataFrame of shape (n_samples, n_features)
+            The input samples to predict.
+        y_true : array-like of shape (n_samples,) or (n_samples, n_outputs)
+            The true target values against which to evaluate the predictions.
+        metrics : dict
+            A dictionary where keys are metric names and values are the metric functions.
+
+
+        Notes
+        -----
+        This method uses the `predict` method to generate predictions and computes each metric.
+
+
+        Examples
+        --------
+        >>> from sklearn.metrics import mean_squared_error, r2_score
+        >>> from sklearn.model_selection import train_test_split
+        >>> from mambular.models import MambularRegressor
+        >>> metrics = {
+        ...     'Mean Squared Error': mean_squared_error,
+        ...     'R2 Score': r2_score
+        ... }
+        >>> # Assuming 'X_test' and 'y_test' are your test dataset and labels
+        >>> # Evaluate using the specified metrics
+        >>> results = regressor.evaluate(X_test, y_test, metrics=metrics)
+
+
+        Returns
+        -------
+        scores : dict
+            A dictionary with metric names as keys and their corresponding scores as values.
+        """
+        if metrics is None:
+            metrics = {"Mean Squared Error": mean_squared_error}
+
+        # Ensure input is in the correct format
+        if not isinstance(X, pd.DataFrame):
+            X = pd.DataFrame(X)
+
+        # Generate predictions using the trained model
+        predictions = self.predict(X)
+
+        # Initialize dictionary to store results
+        scores = {}
+
+        # Compute each metric
+        for metric_name, metric_func in metrics.items():
+            scores[metric_name] = metric_func(y_true, predictions)
+
+        return scores
```

### Comparing `mambular-0.1.2/mambular/models/sklearn_embedding_classifier.py` & `mambular-0.1.3/mambular/models/sklearn_distributional.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,601 +1,663 @@
-from sklearn.model_selection import train_test_split
-import pytorch_lightning as pl
-import torch
-from torch.utils.data import DataLoader
-from pytorch_lightning.callbacks import ModelCheckpoint, EarlyStopping
-from ..base_models.embedding_classifier import BaseEmbeddingMambularClassifier
-from ..utils.config import MambularConfig
-from ..utils.preprocessor import Preprocessor
-from ..utils.dataset import MambularDataModule, EmbeddingMambularDataset
-from sklearn.base import BaseEstimator
-import pandas as pd
-from sklearn.decomposition import PCA
-import numpy as np
-from sklearn.metrics import accuracy_score
-
-
-class EmbeddingMambularClassifier(BaseEstimator):
-    """
-    Provides an scikit-learn-like interface for the ProteinMambularClassifier, making it compatible with
-    scikit-learn's utilities and workflow. This class encapsulates the PyTorch Lightning model, preprocessing,
-    and data loading, offering methods for fitting, predicting, and probability estimation in a manner akin
-    to scikit-learn's API.
-
-    Parameters
-    ----------
-    **kwargs : Configuration parameters that can include both MambularConfig settings and preprocessing
-        options. Any unrecognized parameters are passed to the preprocessor.
-
-    Attributes
-    ----------
-    config : MambularConfig
-        Configuration object for the model, storing architecture-specific parameters.
-    preprocessor : Preprocessor
-        Object handling data preprocessing steps such as feature encoding and normalization.
-    model : ProteinMambularClassifier
-        The underlying neural network model, instantiated during the `fit` method.
-    """
-       
-    def __init__(self, **kwargs):
-        # Known config arguments
-        config_arg_names = [
-            "d_model",
-            "n_layers",
-            "dt_rank",
-            "output_dimension",
-            "pooling_method",
-            "norm",
-            "cls",
-            "dt_min",
-            "dt_max",
-            "dropout",
-            "bias",
-            "weight_decay",
-            "conv_bias",
-            "d_state",
-            "expand_factor",
-            "d_conv",
-            "dt_init",
-            "dt_scale",
-            "dt_init_floor",
-        ]
-        config_kwargs = {k: v for k, v in kwargs.items() if k in config_arg_names}
-        self.config = MambularConfig(**config_kwargs)
-
-        # The rest are assumed to be preprocessor arguments
-        preprocessor_kwargs = {
-            k: v for k, v in kwargs.items() if k not in config_arg_names
-        }
-        self.preprocessor = Preprocessor(**preprocessor_kwargs)
-        self.model = None
-
-    def get_params(self, deep=True):
-        """
-        Get parameters for this estimator.
-
-        Parameters
-        ----------
-        deep : bool, default=True
-            If True, will return the parameters for this estimator and contained subobjects that are estimators.
-
-        Returns
-        -------
-        params : dict
-            Parameter names mapped to their values.
-        """
-        params = self.config_kwargs  # Parameters used to initialize MambularConfig
-
-        # If deep=True, include parameters from nested components like preprocessor
-        if deep:
-            # Assuming Preprocessor has a get_params method
-            preprocessor_params = {
-                "preprocessor__" + key: value
-                for key, value in self.preprocessor.get_params().items()
-            }
-            params.update(preprocessor_params)
-
-        return params
-
-    def set_params(self, **parameters):
-        """
-        Set the parameters of this estimator.
-
-        Parameters
-        ----------
-        **parameters : dict
-            Estimator parameters.
-
-        Returns
-        -------
-        self : object
-            Estimator instance.
-        """
-        # Update config_kwargs with provided parameters
-        valid_config_keys = self.config_kwargs.keys()
-        config_updates = {k: v for k, v in parameters.items() if k in valid_config_keys}
-        self.config_kwargs.update(config_updates)
-
-        # Update the config object
-        for key, value in config_updates.items():
-            setattr(self.config, key, value)
-
-        # Handle preprocessor parameters (prefixed with 'preprocessor__')
-        preprocessor_params = {
-            k.split("__")[1]: v
-            for k, v in parameters.items()
-            if k.startswith("preprocessor__")
-        }
-        if preprocessor_params:
-            # Assuming Preprocessor has a set_params method
-            self.preprocessor.set_params(**preprocessor_params)
-
-        return self
-
-    def split_data(self, X, y, val_size, random_state):
-        """
-        Split the dataset into training and validation sets.
-
-        Parameters
-        ----------
-        X : array-like of shape (n_samples, n_features)
-            The input samples.
-        y : array-like of shape (n_samples,)
-            The target values.
-        val_size : float
-            The proportion of the dataset to include in the validation split.
-        random_state : int
-            Controls the shuffling applied to the data before applying the split.
-
-        Returns
-        -------
-        X_train, X_val, y_train, y_val : arrays
-            The split datasets.
-        """
-        X_train, X_val, y_train, y_val = train_test_split(
-            X, y, test_size=val_size, random_state=random_state
-        )
-
-        return X_train, X_val, y_train, y_val
-
-    def preprocess_data(self, X_train, y_train, X_val, y_val, batch_size, shuffle):
-        """
-        Preprocess the training and validation data and create corresponding DataLoaders.
-
-        Parameters
-        ----------
-        X_train : array-like of shape (n_samples, n_features)
-            The training input samples.
-        y_train : array-like of shape (n_samples,)
-            The training target values.
-        X_val : array-like of shape (n_samples, n_features)
-            The validation input samples.
-        y_val : array-like of shape (n_samples,)
-            The validation target values.
-        batch_size : int
-            Size of mini-batches for the DataLoader.
-        shuffle : bool
-            Whether to shuffle the training data before splitting into batches.
-
-        Returns
-        -------
-        data_module : MambularDataModule
-            An instance of MambularDataModule containing training and validation DataLoaders.
-        """
-        train_preprocessed_data = self.preprocessor.fit_transform(X_train, y_train)
-        val_preprocessed_data = self.preprocessor.transform(X_val)
-
-        # Update feature info based on the actual processed data
-        (
-            self.cat_feature_info,
-            self.num_feature_info,
-        ) = self.preprocessor.get_feature_info()
-
-        # Initialize lists for tensors
-        train_cat_tensors = []
-        train_num_tensors = []
-        val_cat_tensors = []
-        val_num_tensors = []
-
-        # Populate tensors for categorical features, if present in processed data
-        for key in self.cat_feature_info:
-            cat_key = "cat_" + key  # Assuming categorical keys are prefixed with 'cat_'
-            if cat_key in train_preprocessed_data:
-                train_cat_tensors.append(
-                    torch.tensor(train_preprocessed_data[cat_key], dtype=torch.long)
-                )
-            if cat_key in val_preprocessed_data:
-                val_cat_tensors.append(
-                    torch.tensor(val_preprocessed_data[cat_key], dtype=torch.long)
-                )
-
-            binned_key = "num_" + key  # for binned features
-            if binned_key in train_preprocessed_data:
-                train_cat_tensors.append(
-                    torch.tensor(train_preprocessed_data[binned_key], dtype=torch.long)
-                )
-
-            if binned_key in val_preprocessed_data:
-                val_cat_tensors.append(
-                    torch.tensor(val_preprocessed_data[binned_key], dtype=torch.long)
-                )
-
-        # Populate tensors for numerical features, if present in processed data
-        for key in self.num_feature_info:
-            num_key = "num_" + str(
-                key
-            )  # Assuming numerical keys are prefixed with 'num_'
-            if num_key in train_preprocessed_data:
-                train_num_tensors.append(
-                    torch.tensor(train_preprocessed_data[num_key], dtype=torch.float)
-                )
-            if num_key in val_preprocessed_data:
-                val_num_tensors.append(
-                    torch.tensor(val_preprocessed_data[num_key], dtype=torch.float)
-                )
-
-        train_labels = torch.tensor(y_train, dtype=torch.long)
-        val_labels = torch.tensor(y_val, dtype=torch.long)
-
-        # Create datasets
-        train_dataset = EmbeddingMambularDataset(
-            train_cat_tensors, train_num_tensors, train_labels, regression=False
-        )
-        val_dataset = EmbeddingMambularDataset(
-            val_cat_tensors, val_num_tensors, val_labels, regression=False
-        )
-
-        # Create dataloaders
-        train_dataloader = DataLoader(
-            train_dataset, batch_size=batch_size, shuffle=shuffle
-        )
-        val_dataloader = DataLoader(val_dataset, batch_size=batch_size)
-
-        return MambularDataModule(train_dataloader, val_dataloader)
-
-    def preprocess_test_data(self, X):
-        """
-        Preprocesses the test data and creates tensors for categorical and numerical features.
-
-        Parameters
-        ----------
-        X : DataFrame or array-like, shape (n_samples, n_features)
-            Test feature set.
-
-        Returns
-        -------
-        cat_tensors : list of Tensors
-            List of tensors for each categorical feature.
-        num_tensors : list of Tensors
-            List of tensors for each numerical feature.
-        """
-        processed_data = self.preprocessor.transform(X)
-
-        # Initialize lists for tensors
-        cat_tensors = []
-        num_tensors = []
-
-        # Populate tensors for categorical features
-        for key in self.cat_feature_info:
-            cat_key = "cat_" + str(
-                key
-            )  # Assuming categorical keys are prefixed with 'cat_'
-            if cat_key in processed_data:
-                cat_tensors.append(
-                    torch.tensor(processed_data[cat_key], dtype=torch.long)
-                )
-
-            binned_key = "num_" + str(key)  # for binned features
-            if binned_key in processed_data:
-                cat_tensors.append(
-                    torch.tensor(processed_data[binned_key], dtype=torch.long)
-                )
-
-        # Populate tensors for numerical features
-        for key in self.num_feature_info:
-            num_key = "num_" + str(
-                key
-            )  # Assuming numerical keys are prefixed with 'num_'
-            if num_key in processed_data:
-                num_tensors.append(
-                    torch.tensor(processed_data[num_key], dtype=torch.float)
-                )
-
-        return cat_tensors, num_tensors
-
-    def fit(
-        self,
-        X,
-        y,
-        val_size=0.2,
-        X_val=None,
-        y_val=None,
-        max_epochs=100,
-        random_state=101,
-        batch_size=64,
-        shuffle=True,
-        patience=10,
-        monitor="val_loss",
-        mode="min",
-        lr=1e-3,
-        lr_patience=10,
-        factor=0.75,
-        weight_decay=0.025,
-        raw_embeddings=False,
-        seq_size=20,
-        pca=False,
-        reduced_dims=16,
-        **trainer_kwargs
-    ):   
-        """
-        Fits the model to the given dataset.
-
-        Parameters
-        ----------
-        X : pandas DataFrame or array-like
-            Feature matrix for training.
-        y : array-like
-            Target vector.
-        val_size : float, optional
-            Fraction of the data to use for validation if X_val is None.
-        X_val : pandas DataFrame or array-like, optional
-            Feature matrix for validation.
-        y_val : array-like, optional
-            Target vector for validation.
-        max_epochs : int, default=100
-            Maximum number of epochs for training.
-        random_state : int, optional
-            Seed for random number generators.
-        batch_size : int, default=32
-            Size of batches for training and validation.
-        shuffle : bool, default=True
-            Whether to shuffle training data before each epoch.
-        patience : int, default=10
-            Patience for early stopping based on val_loss.
-        monitor : str, default='val_loss'
-            Metric to monitor for early stopping.
-        mode : str, default='min'
-            Mode for early stopping ('min' or 'max').
-        lr : float, default=0.001
-            Learning rate for the optimizer.
-        lr_patience : int, default=5
-            Patience for learning rate reduction.
-        factor : float, default=0.1
-            Factor for learning rate reduction.
-        weight_decay : float, default=0.0
-            Weight decay for the optimizer.
-        raw_embeddings : bool, default=False
-            Whether to use raw features or embeddings.
-        seq_size : int, optional
-            Sequence size for embeddings, relevant if raw_embeddings is False.
-        **trainer_kwargs : dict
-            Additional arguments for the PyTorch Lightning Trainer.
-
-        Returns
-        -------
-        self : object
-            The fitted estimator.
-        """
-        if not isinstance(X, pd.DataFrame):
-            X = pd.DataFrame(X)
-        if X_val:
-            if not isinstance(X_val, pd.DataFrame):
-                X_val = pd.DataFrame(X_val)
-
-        # Apply PCA if indicated
-        if pca:
-            pca_transformer = PCA(n_components=reduced_dims)
-            X = pca_transformer.fit_transform(
-                X
-            )  # Fit and transform the PCA on the complete dataset
-            if X_val is not None:
-                X_val = pca_transformer.transform(
-                    X_val
-                )  # Transform validation data with the same PCA model
-
-            raw_embeddings = True
-
-        if not X_val:
-            X_train, X_val, y_train, y_val = self.split_data(
-                X, y, val_size, random_state
-            )
-        else:
-            X_train = X
-            y_train = y
-
-        data_module = self.preprocess_data(
-            X_train, y_train, X_val, y_val, batch_size, shuffle
-        )
-
-        if raw_embeddings:
-            self.config.d_model = X.shape[1]
-
-        num_classes = len(np.unique(y))
-
-        self.model = BaseEmbeddingMambularClassifier(
-            num_classes=num_classes,
-            config=self.config,
-            cat_feature_info=self.cat_feature_info,
-            num_feature_info=self.num_feature_info,
-            lr=lr,
-            lr_patience=lr_patience,
-            lr_factor=factor,
-            weight_decay=weight_decay,
-            raw_embeddings=raw_embeddings,
-            seq_size=seq_size,
-        )
-
-        early_stop_callback = EarlyStopping(
-            monitor=monitor, min_delta=0.00, patience=patience, verbose=False, mode=mode
-        )
-
-        checkpoint_callback = ModelCheckpoint(
-            monitor="val_loss",  # Adjust according to your validation metric
-            mode="min",
-            save_top_k=1,
-            dirpath="model_checkpoints",  # Specify the directory to save checkpoints
-            filename="best_model",
-        )
-
-        # Initialize the trainer and train the model
-        trainer = pl.Trainer(
-            max_epochs=max_epochs,
-            callbacks=[early_stop_callback, checkpoint_callback],
-            **trainer_kwargs
-        )
-        trainer.fit(self.model, data_module)
-
-        best_model_path = checkpoint_callback.best_model_path
-        if best_model_path:
-            checkpoint = torch.load(best_model_path)
-            self.model.load_state_dict(checkpoint["state_dict"])
-
-        return self
-
-    def predict(self, X):
-        """
-        Predict the class labels for the given input samples.
-
-        Parameters
-        ----------
-        X : array-like or pd.DataFrame of shape (n_samples, n_features)
-            The input samples to predict.
-
-        Returns
-        -------
-        predictions : ndarray of shape (n_samples,)
-            Predicted class labels for each input sample.
-
-        Notes
-        -----
-        The method preprocesses the input data using the same preprocessor used during training,
-        sets the model to evaluation mode, and then performs inference to predict the class labels.
-        The predictions are converted from a PyTorch tensor to a NumPy array before being returned.
-        """
-        # Preprocess the data
-        if not isinstance(X, pd.DataFrame):
-            X = pd.DataFrame(X)
-
-        if hasattr(self, "pca_transformer"):
-            X = pd.DataFrame(self.pca_transformer.transform(X))
-
-        cat_tensors, num_tensors = self.preprocess_test_data(X)
-        device = next(self.model.parameters()).device
-        cat_tensors, num_tensors = self.preprocess_test_data(X)
-        if isinstance(cat_tensors, list):
-            cat_tensors = [tensor.to(device) for tensor in cat_tensors]
-        else:
-            cat_tensors = cat_tensors.to(device)
-
-        if isinstance(num_tensors, list):
-            num_tensors = [tensor.to(device) for tensor in num_tensors]
-        else:
-            num_tensors = num_tensors.to(device)
-
-        # Set the model to evaluation mode
-        self.model.eval()
-
-        # Perform inference
-        with torch.no_grad():
-            logits = self.model(cat_tensors, num_tensors)
-            predictions = torch.argmax(logits, dim=1)
-
-        # Convert predictions to NumPy array and return
-        return predictions.cpu().numpy()
-
-    def predict_proba(self, X):
-        """
-        Predict class probabilities for the given input samples.
-
-        Parameters
-        ----------
-        X : array-like or pd.DataFrame of shape (n_samples, n_features)
-            The input samples for which to predict class probabilities.
-
-        Returns
-        -------
-        probabilities : ndarray of shape (n_samples, n_classes)
-            Predicted class probabilities for each input sample.
-
-        Notes
-        -----
-        The method preprocesses the input data using the same preprocessor used during training,
-        sets the model to evaluation mode, and then performs inference to predict the class probabilities.
-        Softmax is applied to the logits to obtain probabilities, which are then converted from a PyTorch tensor
-        to a NumPy array before being returned.
-        """
-        # Preprocess the data
-        if not isinstance(X, pd.DataFrame):
-            X = pd.DataFrame(X)
-        cat_tensors, num_tensors = self.preprocess_test_data(X)
-        device = next(self.model.parameters()).device
-        cat_tensors, num_tensors = self.preprocess_test_data(X)
-        if isinstance(cat_tensors, list):
-            cat_tensors = [tensor.to(device) for tensor in cat_tensors]
-        else:
-            cat_tensors = cat_tensors.to(device)
-
-        if isinstance(num_tensors, list):
-            num_tensors = [tensor.to(device) for tensor in num_tensors]
-        else:
-            num_tensors = num_tensors.to(device)
-
-        # Set the model to evaluation mode
-        self.model.eval()
-
-        # Perform inference
-        with torch.no_grad():
-            logits = self.model(cat_tensors, num_tensors)
-            probabilities = torch.softmax(logits, dim=1)
-
-        # Convert probabilities to NumPy array and return
-        return probabilities.cpu().numpy()
-
-    def evaluate(self, X, y_true, metrics=None):
-        """
-        Evaluate the model on the given data using specified metrics.
-
-        Parameters
-        ----------
-        X : array-like or pd.DataFrame of shape (n_samples, n_features)
-            The input samples to predict.
-        y_true : array-like of shape (n_samples,)
-            The true class labels against which to evaluate the predictions.
-        metrics : dict
-            A dictionary where keys are metric names and values are tuples containing the metric function
-            and a boolean indicating whether the metric requires probability scores (True) or class labels (False).
-
-        Returns
-        -------
-        scores : dict
-            A dictionary with metric names as keys and their corresponding scores as values.
-
-        Notes
-        -----
-        This method uses either the `predict` or `predict_proba` method depending on the metric requirements.
-        """
-        # Ensure input is in the correct format
-        if metrics is None:
-            metrics = {"Accuracy": (accuracy_score, False)}
-
-        if not isinstance(X, pd.DataFrame):
-            X = pd.DataFrame(X)
-
-        # Initialize dictionary to store results
-        scores = {}
-
-        # Generate class probabilities if any metric requires them
-        if any(use_proba for _, use_proba in metrics.values()):
-            probabilities = self.predict_proba(X)
-
-        # Generate class labels if any metric requires them
-        if any(not use_proba for _, use_proba in metrics.values()):
-            predictions = self.predict(X)
-
-        # Compute each metric
-        for metric_name, (metric_func, use_proba) in metrics.items():
-            if use_proba:
-                scores[metric_name] = metric_func(y_true, probabilities)
-            else:
-                scores[metric_name] = metric_func(y_true, predictions)
-
-        return scores
+import lightning as pl
+import numpy as np
+import warnings
+import pandas as pd
+import properscoring as ps
+import torch
+from lightning.pytorch.callbacks import EarlyStopping, ModelCheckpoint
+from sklearn.base import BaseEstimator
+from sklearn.metrics import accuracy_score, mean_squared_error
+from sklearn.model_selection import train_test_split
+from torch.utils.data import DataLoader
+
+from ..base_models.distributional import BaseMambularLSS
+from ..utils.configs import DefaultMambularConfig
+from ..utils.dataset import MambularDataModule, MambularDataset
+from ..utils.distributional_metrics import (
+    beta_brier_score,
+    dirichlet_error,
+    gamma_deviance,
+    inverse_gamma_loss,
+    negative_binomial_deviance,
+    poisson_deviance,
+    student_t_loss,
+)
+from ..utils.preprocessor import Preprocessor
+
+
+class MambularLSS(BaseEstimator):
+    """
+    MambularLSS is a machine learning estimator that is designed for structured data,
+    incorporating both preprocessing and a deep learning model. The estimator
+    integrates configurable components for data preprocessing and the neural network model,
+    facilitating end-to-end training and prediction workflows.
+
+    The initialization of this class separates configuration arguments for the model and
+    the preprocessor, allowing for flexible adjustment of parameters.
+
+    Parameters
+    ----------
+    # configuration parameters
+    lr : float, optional
+        Learning rate for the optimizer. Default is 1e-4.
+    lr_patience : int, optional
+        Number of epochs with no improvement on the validation loss to wait before reducing the learning rate. Default is 10.
+    weight_decay : float, optional
+        Weight decay (L2 penalty) coefficient. Default is 1e-6.
+    lr_factor : float, optional
+        Factor by which the learning rate will be reduced. Default is 0.1.
+    d_model : int, optional
+        Dimension of the model. Default is 64.
+    n_layers : int, optional
+        Number of layers. Default is 8.
+    expand_factor : int, optional
+        Expansion factor. Default is 2.
+    bias : bool, optional
+        Whether to use bias. Default is False.
+    d_conv : int, optional
+        Dimension of the convolution. Default is 16.
+    conv_bias : bool, optional
+        Whether to use bias in the convolution. Default is True.
+    dropout : float, optional
+        Dropout rate in the mamba blocks. Default is 0.05.
+    dt_rank : str, optional
+        Rank of the time dimension. Default is "auto".
+    d_state : int, optional
+        State dimension. Default is 16.
+    dt_scale : float, optional
+        Scale of the time dimension. Default is 1.0.
+    dt_init : str, optional
+        Initialization method for the time dimension. Default is "random".
+    dt_max : float, optional
+        Maximum value for the time dimension. Default is 0.1.
+    dt_min : float, optional
+        Minimum value for the time dimension. Default is 1e-3.
+    dt_init_floor : float, optional
+        Floor value for the time dimension initialization. Default is 1e-4.
+    norm : str, optional
+        Normalization method. Default is 'RMSNorm'.
+    activation : callable, optional
+        Activation function. Default is nn.SELU().
+    num_embedding_activation : callable, optional
+        Activation function for numerical embeddings. Default is nn.Identity().
+    head_layer_sizes : list, optional
+        Sizes of the layers in the head. Default is [64, 64, 32].
+    head_dropout : float, optional
+        Dropout rate for the head. Default is 0.5.
+    head_skip_layers : bool, optional
+        Whether to use skip layers in the head. Default is False.
+    head_activation : callable, optional
+        Activation function for the head. Default is nn.SELU().
+    head_use_batch_norm : bool, optional
+        Whether to use batch normalization in the head. Default is False.
+
+    # Preprocessor Parameters
+    n_bins : int, optional
+        The number of bins to use for numerical feature binning. Default is 50.
+    numerical_preprocessing : str, optional
+        The preprocessing strategy for numerical features. Default is 'ple'.
+    use_decision_tree_bins : bool, optional
+        If True, uses decision tree regression/classification to determine optimal bin edges for numerical feature binning. Default is False.
+    binning_strategy : str, optional
+        Defines the strategy for binning numerical features. Default is 'uniform'.
+    task : str, optional
+        Indicates the type of machine learning task ('regression' or 'classification'). Default is 'regression'.
+    cat_cutoff: float or int, optional
+        Indicates the cutoff after which integer values are treated as categorical. If float, it's treated as a percentage. If int, it's the maximum number of unique values for a column to be considered categorical. Default is 3%
+    treat_all_integers_as_numerical : bool, optional
+        If True, all integer columns will be treated as numerical, regardless of their unique value count or proportion. Default is False
+
+
+
+    Attributes
+    ----------
+    config : MambularConfig
+        Configuration object that holds model-specific settings.
+    preprocessor : Preprocessor
+        Preprocessor object for handling feature preprocessing like normalization and encoding.
+    model : BaseMambularClassifier or None
+        The underlying PyTorch Lightning model, instantiated upon calling the `fit` method.
+    """
+
+    def __init__(self, **kwargs):
+        # Known config arguments
+        config_arg_names = [
+            "lr",
+            "lr_patience",
+            "weight_decay",
+            "lr_factor",
+            "d_model",
+            "n_layers",
+            "expand_factor",
+            "bias",
+            "d_conv",
+            "conv_bias",
+            "dropout",
+            "dt_rank",
+            "d_state",
+            "dt_scale",
+            "dt_init",
+            "dt_max",
+            "dt_min",
+            "dt_init_floor",
+            "norm",
+            "activation",
+            "num_embedding_activation",
+            "head_layer_sizes",
+            "head_dropout",
+            "head_skip_layers",
+            "head_activation",
+            "head_use_batch_norm",
+        ]
+
+        preprocessor_arg_names = [
+            "n_bins",
+            "numerical_preprocessing",
+            "use_decision_tree_bins",
+            "binning_strategy",
+            "task",
+            "cat_cutoff",
+            "treat_all_integers_as_numerical",
+        ]
+
+        self.config_kwargs = {k: v for k, v in kwargs.items() if k in config_arg_names}
+        self.config = DefaultMambularConfig(**self.config_kwargs)
+
+        preprocessor_kwargs = {
+            k: v for k, v in kwargs.items() if k in preprocessor_arg_names
+        }
+        # Raise a warning if task is set to 'classification'
+        if preprocessor_kwargs.get("task") == "regression":
+            warnings.warn(
+                "The task in preprocessing binning is set to 'regression'. Make sure that this is correct for your distributional family ",
+                UserWarning,
+            )
+
+        self.preprocessor = Preprocessor(**preprocessor_kwargs)
+        self.model = None
+
+    def get_params(self, deep=True):
+        """
+        Get parameters for this estimator, optionally including parameters from nested components
+        like the preprocessor.
+
+        Parameters
+        ----------
+        deep : bool, default=True
+            If True, return parameters of nested components.
+
+
+        Returns
+        -------
+        dict
+            A dictionary mapping parameter names to their values. For nested components,
+            parameter names are prefixed accordingly (e.g., 'preprocessor__<param_name>').
+        """
+
+        params = self.config_kwargs  # Parameters used to initialize MambularConfig
+
+        # If deep=True, include parameters from nested components like preprocessor
+        if deep:
+            # Assuming Preprocessor has a get_params method
+            preprocessor_params = {
+                "preprocessor__" + key: value
+                for key, value in self.preprocessor.get_params().items()
+            }
+            params.update(preprocessor_params)
+
+        return params
+
+    def set_params(self, **parameters):
+        """
+        Set the parameters of this estimator, allowing for modifications to both the configuration
+        and preprocessor parameters. Parameters not recognized as configuration arguments are
+        assumed to be preprocessor arguments.
+
+        Parameters
+        ----------
+            **parameters: Arbitrary keyword arguments where keys are parameter names and values
+                          are the new parameter values.
+
+
+        Returns
+        -------
+            self: This instance with updated parameters.
+        """
+        # Update config_kwargs with provided parameters
+        valid_config_keys = self.config_kwargs.keys()
+        config_updates = {k: v for k, v in parameters.items() if k in valid_config_keys}
+        self.config_kwargs.update(config_updates)
+
+        # Update the config object
+        for key, value in config_updates.items():
+            setattr(self.config, key, value)
+
+        # Handle preprocessor parameters (prefixed with 'preprocessor__')
+        preprocessor_params = {
+            k.split("__")[1]: v
+            for k, v in parameters.items()
+            if k.startswith("preprocessor__")
+        }
+        if preprocessor_params:
+            # Assuming Preprocessor has a set_params method
+            self.preprocessor.set_params(**preprocessor_params)
+
+        return self
+
+    def split_data(self, X, y, val_size, random_state):
+        """
+        Split the dataset into training and validation sets.
+
+        Parameters
+        ----------
+        X : array-like
+            Features of the dataset.
+        y : array-like
+            Target values.
+        val_size : float
+            The proportion of the dataset to include in the validation split.
+        random_state : int, optional
+            The seed used by the random number generator for reproducibility.
+
+
+        Returns
+        -------
+        tuple
+            A tuple containing split datasets (X_train, X_val, y_train, y_val).
+        """
+        X_train, X_val, y_train, y_val = train_test_split(
+            X, y, test_size=val_size, random_state=random_state
+        )
+
+        return X_train, X_val, y_train, y_val
+
+    def preprocess_data(self, X_train, y_train, X_val, y_val, batch_size, shuffle):
+        """
+        Preprocess the training and validation data, fit the preprocessor on the training data,
+        and transform both training and validation data. This method also initializes tensors
+        for categorical and numerical features and labels, and prepares DataLoader objects for
+        both datasets.
+
+        Parameters
+        ----------
+        X_train : array-like
+            Training features.
+        y_train : array-like
+            Training target values.
+        X_val : array-like
+            Validation features.
+        y_val : array-like
+            Validation target values.
+        batch_size : int
+            Batch size for DataLoader objects.
+        shuffle : bool
+            Whether to shuffle the training data in the DataLoader.
+
+
+        Returns
+        -------
+        MambularDataModule
+            An object containing DataLoaders for training and validation datasets.
+        """
+        self.preprocessor.fit(
+            pd.concat([X_train, X_val], axis=0).reset_index(drop=True),
+            np.concatenate((y_train, y_val), axis=0),
+        )
+        train_preprocessed_data = self.preprocessor.transform(X_train)
+        val_preprocessed_data = self.preprocessor.transform(X_val)
+
+        # Update feature info based on the actual processed data
+        (
+            self.cat_feature_info,
+            self.num_feature_info,
+        ) = self.preprocessor.get_feature_info()
+
+        # Initialize lists for tensors
+        train_cat_tensors = []
+        train_num_tensors = []
+        val_cat_tensors = []
+        val_num_tensors = []
+
+        # Populate tensors for categorical features, if present in processed data
+        for key in self.cat_feature_info:
+            cat_key = "cat_" + key  # Assuming categorical keys are prefixed with 'cat_'
+            if cat_key in train_preprocessed_data:
+                train_cat_tensors.append(
+                    torch.tensor(train_preprocessed_data[cat_key], dtype=torch.long)
+                )
+            if cat_key in val_preprocessed_data:
+                val_cat_tensors.append(
+                    torch.tensor(val_preprocessed_data[cat_key], dtype=torch.long)
+                )
+
+            binned_key = "num_" + key  # for binned features
+            if binned_key in train_preprocessed_data:
+                train_cat_tensors.append(
+                    torch.tensor(train_preprocessed_data[binned_key], dtype=torch.long)
+                )
+
+            if binned_key in val_preprocessed_data:
+                val_cat_tensors.append(
+                    torch.tensor(val_preprocessed_data[binned_key], dtype=torch.long)
+                )
+
+        # Populate tensors for numerical features, if present in processed data
+        for key in self.num_feature_info:
+            num_key = "num_" + key  # Assuming numerical keys are prefixed with 'num_'
+            if num_key in train_preprocessed_data:
+                train_num_tensors.append(
+                    torch.tensor(train_preprocessed_data[num_key], dtype=torch.float32)
+                )
+            if num_key in val_preprocessed_data:
+                val_num_tensors.append(
+                    torch.tensor(val_preprocessed_data[num_key], dtype=torch.float32)
+                )
+
+        train_labels = torch.tensor(y_train, dtype=torch.float32)
+        val_labels = torch.tensor(y_val, dtype=torch.float32)
+
+        # Create datasets
+        train_dataset = MambularDataset(
+            train_cat_tensors, train_num_tensors, train_labels
+        )
+        val_dataset = MambularDataset(val_cat_tensors, val_num_tensors, val_labels)
+
+        # Create dataloaders
+        train_dataloader = DataLoader(
+            train_dataset, batch_size=batch_size, shuffle=shuffle
+        )
+        val_dataloader = DataLoader(val_dataset, batch_size=batch_size)
+
+        return MambularDataModule(train_dataloader, val_dataloader)
+
+    def preprocess_test_data(self, X):
+        """
+        Preprocess test data using the fitted preprocessor. This method prepares tensors for
+        categorical and numerical features based on the preprocessed test data.
+
+        Parameters
+        ----------
+        X : array-like
+            Test features to preprocess.
+
+
+        Returns
+        -------
+        tuple
+            A tuple containing lists of tensors for categorical and numerical features.
+        """
+        processed_data = self.preprocessor.transform(X)
+
+        # Initialize lists for tensors
+        cat_tensors = []
+        num_tensors = []
+
+        # Populate tensors for categorical features
+        for key in self.cat_feature_info:
+            cat_key = "cat_" + key  # Assuming categorical keys are prefixed with 'cat_'
+            if cat_key in processed_data:
+                cat_tensors.append(
+                    torch.tensor(processed_data[cat_key], dtype=torch.long)
+                )
+
+            binned_key = "num_" + key  # for binned features
+            if binned_key in processed_data:
+                cat_tensors.append(
+                    torch.tensor(processed_data[binned_key], dtype=torch.long)
+                )
+
+        # Populate tensors for numerical features
+        for key in self.num_feature_info:
+            num_key = "num_" + key  # Assuming numerical keys are prefixed with 'num_'
+            if num_key in processed_data:
+                num_tensors.append(
+                    torch.tensor(processed_data[num_key], dtype=torch.float32)
+                )
+
+        return cat_tensors, num_tensors
+
+    def fit(
+        self,
+        X,
+        y,
+        family,
+        val_size: float = 0.2,
+        X_val=None,
+        y_val=None,
+        max_epochs: int = 100,
+        random_state: int = 101,
+        batch_size: int = 128,
+        shuffle: bool = True,
+        patience: int = 15,
+        monitor: str = "val_loss",
+        mode: str = "min",
+        lr: float = 1e-4,
+        lr_patience: int = 10,
+        factor: float = 0.1,
+        weight_decay: float = 1e-06,
+        **trainer_kwargs
+    ):
+        """
+        Fits the model to the provided data, using the specified loss distribution family for the prediction task.
+
+        Parameters
+        ----------
+        X : DataFrame or array-like, shape (n_samples, n_features)
+            Training features.
+        y : array-like, shape (n_samples,) or (n_samples, n_targets)
+            Target values for training.
+        family : str
+            The name of the distribution family to use for the loss function. Examples include 'normal' for regression tasks.
+        val_size : float, default=0.2
+            Proportion of the dataset to include in the validation split if `X_val` is None.
+        X_val : DataFrame or array-like, shape (n_samples, n_features), optional
+            Validation features. If provided, `X` and `y` are not split.
+        y_val : array-like, shape (n_samples,) or (n_samples, n_targets), optional
+            Validation target values. Required if `X_val` is provided.
+        max_epochs : int, default=100
+            Maximum number of epochs for training.
+        random_state : int, default=101
+            Seed used by the random number generator for shuffling the data.
+        batch_size : int, default=64
+            Number of samples per gradient update.
+        shuffle : bool, default=True
+            Whether to shuffle the training data before each epoch.
+        patience : int, default=10
+            Number of epochs with no improvement on the validation metric to wait before early stopping.
+        monitor : str, default="val_loss"
+            The metric to monitor for early stopping.
+        mode : str, default="min"
+            In 'min' mode, training will stop when the quantity monitored has stopped decreasing;
+            in 'max' mode, it will stop when the quantity monitored has stopped increasing.
+        lr : float, default=1e-3
+            Learning rate for the optimizer.
+        lr_patience : int, default=10
+            Number of epochs with no improvement on the validation metric to wait before reducing the learning rate.
+        factor : float, default=0.75
+            Factor by which the learning rate will be reduced.
+        weight_decay : float, default=0.025
+            Weight decay (L2 penalty) parameter.
+        **trainer_kwargs : dict
+            Additional keyword arguments for PyTorch Lightning's Trainer class.
+
+
+        Returns
+        -------
+        self : object
+            The fitted estimator.
+        """
+        if not isinstance(X, pd.DataFrame):
+            X = pd.DataFrame(X)
+        if X_val:
+            if not isinstance(X_val, pd.DataFrame):
+                X_val = pd.DataFrame(X_val)
+
+        if not X_val:
+            X_train, X_val, y_train, y_val = self.split_data(
+                X, y, val_size, random_state
+            )
+
+        data_module = self.preprocess_data(
+            X_train, y_train, X_val, y_val, batch_size, shuffle
+        )
+
+        self.model = BaseMambularLSS(
+            family=family,
+            config=self.config,
+            cat_feature_info=self.cat_feature_info,
+            num_feature_info=self.num_feature_info,
+            lr=lr,
+            lr_patience=lr_patience,
+            lr_factor=factor,
+            weight_decay=weight_decay,
+        )
+
+        early_stop_callback = EarlyStopping(
+            monitor=monitor, min_delta=0.00, patience=patience, verbose=False, mode=mode
+        )
+
+        checkpoint_callback = ModelCheckpoint(
+            monitor="val_loss",
+            mode="min",
+            save_top_k=1,
+            dirpath="model_checkpoints",
+            filename="best_model",
+        )
+
+        # Initialize the trainer and train the model
+        trainer = pl.Trainer(
+            max_epochs=max_epochs,
+            callbacks=[early_stop_callback, checkpoint_callback],
+            **trainer_kwargs,
+        )
+        trainer.fit(self.model, data_module)
+
+        best_model_path = checkpoint_callback.best_model_path
+        if best_model_path:
+            checkpoint = torch.load(best_model_path)
+            self.model.load_state_dict(checkpoint["state_dict"])
+
+        return self
+
+    def predict(self, X, raw=False):
+        """
+        Predicts target values for the given input samples using the fitted model.
+
+        Parameters
+        ----------
+        X : DataFrame or array-like, shape (n_samples, n_features)
+            The input samples for which to predict target values.
+
+
+        Returns
+        -------
+        predictions : ndarray, shape (n_samples,) or (n_samples, n_distributional_parameters)
+            The predicted target values.
+        """
+        # Preprocess the data
+        if not isinstance(X, pd.DataFrame):
+            X = pd.DataFrame(X)
+        device = next(self.model.parameters()).device
+        cat_tensors, num_tensors = self.preprocess_test_data(X)
+        if isinstance(cat_tensors, list):
+            cat_tensors = [tensor.to(device) for tensor in cat_tensors]
+        else:
+            cat_tensors = cat_tensors.to(device)
+
+        if isinstance(num_tensors, list):
+            num_tensors = [tensor.to(device) for tensor in num_tensors]
+        else:
+            num_tensors = num_tensors.to(device)
+
+        # Set the model to evaluation mode
+        self.model.eval()
+
+        # Perform inference
+        with torch.no_grad():
+            predictions = self.model(num_features=num_tensors, cat_features=cat_tensors)
+
+        if not raw:
+            return self.model.family(predictions).cpu().numpy()
+
+        # Convert predictions to NumPy array and return
+        else:
+            return predictions.cpu().numpy()
+
+    def evaluate(self, X, y_true, metrics=None, distribution_family=None):
+        """
+        Evaluate the model on the given data using specified metrics tailored to the distribution type.
+
+        Parameters
+        ----------
+        X : DataFrame or array-like, shape (n_samples, n_features)
+            Input samples.
+        y_true : DataFrame or array-like, shape (n_samples,) or (n_samples, n_outputs)
+            True target values.
+        metrics : dict, optional
+            A dictionary where keys are metric names and values are the metric functions.
+            If None, default metrics based on the detected or specified distribution_family are used.
+        distribution_family : str, optional
+            Specifies the distribution family the model is predicting for. If None, it will attempt to infer based
+            on the model's settings.
+
+
+        Returns
+        -------
+        scores : dict
+            A dictionary with metric names as keys and their corresponding scores as values.
+        """
+        # Infer distribution family from model settings if not provided
+        if distribution_family is None:
+            distribution_family = getattr(self.model, "distribution_family", "normal")
+
+        # Setup default metrics if none are provided
+        if metrics is None:
+            metrics = self.get_default_metrics(distribution_family)
+
+        # Make predictions
+        predictions = self.predict(X, raw=False)
+
+        # Initialize dictionary to store results
+        scores = {}
+
+        # Compute each metric
+        for metric_name, metric_func in metrics.items():
+            scores[metric_name] = metric_func(y_true, predictions)
+
+        return scores
+
+    def get_default_metrics(self, distribution_family):
+        """
+        Provides default metrics based on the distribution family.
+
+        Parameters
+        ----------
+        distribution_family : str
+            The distribution family for which to provide default metrics.
+
+
+        Returns
+        -------
+        metrics : dict
+            A dictionary of default metric functions.
+        """
+        default_metrics = {
+            "normal": {
+                "MSE": lambda y, pred: mean_squared_error(y, pred[:, 0]),
+                "CRPS": lambda y, pred: np.mean(
+                    [
+                        ps.crps_gaussian(y[i], mu=pred[i, 0], sig=np.sqrt(pred[i, 1]))
+                        for i in range(len(y))
+                    ]
+                ),
+            },
+            "poisson": {"Poisson Deviance": poisson_deviance},
+            "gamma": {"Gamma Deviance": gamma_deviance},
+            "beta": {"Brier Score": beta_brier_score},
+            "dirichlet": {"Dirichlet Error": dirichlet_error},
+            "studentt": {"Student-T Loss": student_t_loss},
+            "negativebinom": {"Negative Binomial Deviance": negative_binomial_deviance},
+            "inversegamma": {"Inverse Gamma Loss": inverse_gamma_loss},
+            "categorical": {"Accuracy": accuracy_score},
+        }
+        return default_metrics.get(distribution_family, {})
```

### Comparing `mambular-0.1.2/mambular/models/sklearn_embedding_regressor.py` & `mambular-0.1.3/mambular/models/sklearn_classifier.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,545 +1,706 @@
-from sklearn.model_selection import train_test_split
-import pytorch_lightning as pl
-import torch
-from torch.utils.data import DataLoader
-from pytorch_lightning.callbacks import ModelCheckpoint, EarlyStopping
-from ..base_models.embedding_regressor import BaseEmbeddingMambularRegressor
-from ..utils.config import MambularConfig
-from ..utils.preprocessor import Preprocessor
-from ..utils.dataset import MambularDataModule, EmbeddingMambularDataset
-from sklearn.base import BaseEstimator
-import pandas as pd
-from sklearn.decomposition import PCA
-from sklearn.metrics import mean_squared_error
-
-
-class EmbeddingMambularRegressor(BaseEstimator):
-    """
-    An sklearn-like interface for the ProteinMambularRegressor, making it compatible with sklearn's utilities
-    and workflows. This class wraps the PyTorch Lightning model and preprocessor, providing methods for fitting,
-    predicting, and setting/getting parameters in a way that mimics sklearn's API.
-
-    Parameters
-    ----------
-    **kwargs : Keyword arguments that can include both configuration parameters for the MambularConfig and
-        parameters for the preprocessor.
-
-    Attributes
-    ----------
-    config : MambularConfig
-        Configuration object containing model-specific parameters.
-    preprocessor : Preprocessor
-        Preprocessor object for data preprocessing steps.
-    model : ProteinMambularRegressor
-        The neural network model, initialized after the `fit` method is called.
-    """
-    
-    def __init__(self, **kwargs):
-        # Known config arguments
-        config_arg_names = [
-            "d_model",
-            "n_layers",
-            "dt_rank",
-            "output_dimension",
-            "pooling_method",
-            "norm",
-            "cls",
-            "dt_min",
-            "dt_max",
-            "dropout",
-            "bias",
-            "weight_decay",
-            "conv_bias",
-            "d_state",
-            "expand_factor",
-            "d_conv",
-            "dt_init",
-            "dt_scale",
-            "dt_init_floor",
-        ]
-        config_kwargs = {k: v for k, v in kwargs.items() if k in config_arg_names}
-        self.config = MambularConfig(**config_kwargs)
-
-        # The rest are assumed to be preprocessor arguments
-        preprocessor_kwargs = {
-            k: v for k, v in kwargs.items() if k not in config_arg_names
-        }
-
-        if not "numerical_preprocessing" in preprocessor_kwargs.keys():
-            preprocessor_kwargs["numerical_preprocessing"] = "normalization"
-        self.preprocessor = Preprocessor(**preprocessor_kwargs)
-        self.model = None
-
-    def get_params(self, deep=True):
-        """
-        Get parameters for this estimator. Overrides the BaseEstimator method.
-
-        Parameters
-        ----------
-        deep : bool, default=True
-            If True, returns the parameters for this estimator and contained sub-objects that are estimators.
-
-        Returns
-        -------
-        params : dict
-            Parameter names mapped to their values.
-        """
-        params = self.config_kwargs  # Parameters used to initialize MambularConfig
-
-        # If deep=True, include parameters from nested components like preprocessor
-        if deep:
-            # Assuming Preprocessor has a get_params method
-            preprocessor_params = {
-                "preprocessor__" + key: value
-                for key, value in self.preprocessor.get_params().items()
-            }
-            params.update(preprocessor_params)
-
-        return params
-
-    def set_params(self, **parameters):
-        """
-        Set the parameters of this estimator. Overrides the BaseEstimator method.
-
-        Parameters
-        ----------
-        **parameters : dict
-            Estimator parameters to be set.
-
-        Returns
-        -------
-        self : object
-            The instance with updated parameters.
-        """
-        # Update config_kwargs with provided parameters
-        valid_config_keys = self.config_kwargs.keys()
-        config_updates = {k: v for k, v in parameters.items() if k in valid_config_keys}
-        self.config_kwargs.update(config_updates)
-
-        # Update the config object
-        for key, value in config_updates.items():
-            setattr(self.config, key, value)
-
-        # Handle preprocessor parameters (prefixed with 'preprocessor__')
-        preprocessor_params = {
-            k.split("__")[1]: v
-            for k, v in parameters.items()
-            if k.startswith("preprocessor__")
-        }
-        if preprocessor_params:
-            # Assuming Preprocessor has a set_params method
-            self.preprocessor.set_params(**preprocessor_params)
-
-        return self
-
-    def split_data(self, X, y, val_size, random_state):
-        """
-        Splits the dataset into training and validation sets.
-
-        Parameters
-        ----------
-        X : array-like or DataFrame, shape (n_samples, n_features)
-            Input features.
-        y : array-like, shape (n_samples,) or (n_samples, n_targets)
-            Target values.
-        val_size : float
-            The proportion of the dataset to include in the validation split.
-        random_state : int
-            Controls the shuffling applied to the data before applying the split.
-
-        Returns
-        -------
-        X_train, X_val, y_train, y_val : arrays
-            The split datasets.
-        """
-        X_train, X_val, y_train, y_val = train_test_split(
-            X, y, test_size=val_size, random_state=random_state
-        )
-
-        return X_train, X_val, y_train, y_val
-
-    def preprocess_data(self, X_train, y_train, X_val, y_val, batch_size, shuffle):
-        """
-        Preprocesses the training and validation data, and creates DataLoaders for them.
-
-        Parameters
-        ----------
-        X_train : DataFrame or array-like, shape (n_samples_train, n_features)
-            Training feature set.
-        y_train : array-like, shape (n_samples_train,)
-            Training target values.
-        X_val : DataFrame or array-like, shape (n_samples_val, n_features)
-            Validation feature set.
-        y_val : array-like, shape (n_samples_val,)
-            Validation target values.
-        batch_size : int
-            Size of batches for the DataLoader.
-        shuffle : bool
-            Whether to shuffle the training data in the DataLoader.
-
-        Returns
-        -------
-        data_module : MambularDataModule
-            An instance of MambularDataModule containing the training and validation DataLoaders.
-        """
-        train_preprocessed_data = self.preprocessor.fit_transform(X_train, y_train)
-        val_preprocessed_data = self.preprocessor.transform(X_val)
-
-        # Update feature info based on the actual processed data
-        (
-            self.cat_feature_info,
-            self.num_feature_info,
-        ) = self.preprocessor.get_feature_info()
-
-        # Initialize lists for tensors
-        train_cat_tensors = []
-        train_num_tensors = []
-        val_cat_tensors = []
-        val_num_tensors = []
-
-        # Populate tensors for categorical features, if present in processed data
-        for key in self.cat_feature_info:
-            cat_key = "cat_" + key  # Assuming categorical keys are prefixed with 'cat_'
-            if cat_key in train_preprocessed_data:
-                train_cat_tensors.append(
-                    torch.tensor(train_preprocessed_data[cat_key], dtype=torch.long)
-                )
-            if cat_key in val_preprocessed_data:
-                val_cat_tensors.append(
-                    torch.tensor(val_preprocessed_data[cat_key], dtype=torch.long)
-                )
-
-            binned_key = "num_" + key  # for binned features
-            if binned_key in train_preprocessed_data:
-                train_cat_tensors.append(
-                    torch.tensor(train_preprocessed_data[binned_key], dtype=torch.long)
-                )
-
-            if binned_key in val_preprocessed_data:
-                val_cat_tensors.append(
-                    torch.tensor(val_preprocessed_data[binned_key], dtype=torch.long)
-                )
-
-        # Populate tensors for numerical features, if present in processed data
-        for key in self.num_feature_info:
-            num_key = "num_" + str(
-                key
-            )  # Assuming numerical keys are prefixed with 'num_'
-            if num_key in train_preprocessed_data:
-                train_num_tensors.append(
-                    torch.tensor(train_preprocessed_data[num_key], dtype=torch.float)
-                )
-            if num_key in val_preprocessed_data:
-                val_num_tensors.append(
-                    torch.tensor(val_preprocessed_data[num_key], dtype=torch.float)
-                )
-
-        train_labels = torch.tensor(y_train, dtype=torch.float)
-        val_labels = torch.tensor(y_val, dtype=torch.float)
-
-        # Create datasets
-        train_dataset = EmbeddingMambularDataset(
-            train_cat_tensors, train_num_tensors, train_labels
-        )
-        val_dataset = EmbeddingMambularDataset(
-            val_cat_tensors, val_num_tensors, val_labels
-        )
-
-        # Create dataloaders
-        train_dataloader = DataLoader(
-            train_dataset, batch_size=batch_size, shuffle=shuffle
-        )
-        val_dataloader = DataLoader(val_dataset, batch_size=batch_size)
-
-        return MambularDataModule(train_dataloader, val_dataloader)
-
-    def preprocess_test_data(self, X):
-        """
-        Preprocesses the test data and creates tensors for categorical and numerical features.
-
-        Parameters
-        ----------
-        X : DataFrame or array-like, shape (n_samples, n_features)
-            Test feature set.
-
-        Returns
-        -------
-        cat_tensors : list of Tensors
-            List of tensors for each categorical feature.
-        num_tensors : list of Tensors
-            List of tensors for each numerical feature.
-        """
-        processed_data = self.preprocessor.transform(X)
-
-        # Initialize lists for tensors
-        cat_tensors = []
-        num_tensors = []
-
-        # Populate tensors for categorical features
-        for key in self.cat_feature_info:
-            cat_key = "cat_" + str(
-                key
-            )  # Assuming categorical keys are prefixed with 'cat_'
-            if cat_key in processed_data:
-                cat_tensors.append(
-                    torch.tensor(processed_data[cat_key], dtype=torch.long)
-                )
-
-            binned_key = "num_" + str(key)  # for binned features
-            if binned_key in processed_data:
-                cat_tensors.append(
-                    torch.tensor(processed_data[binned_key], dtype=torch.long)
-                )
-
-        # Populate tensors for numerical features
-        for key in self.num_feature_info:
-            num_key = "num_" + str(
-                key
-            )  # Assuming numerical keys are prefixed with 'num_'
-            if num_key in processed_data:
-                num_tensors.append(
-                    torch.tensor(processed_data[num_key], dtype=torch.float)
-                )
-
-        return cat_tensors, num_tensors
-
-    def fit(
-        self,
-        X,
-        y,
-        val_size=0.2,
-        X_val=None,
-        y_val=None,
-        max_epochs=100,
-        random_state=101,
-        batch_size=64,
-        shuffle=True,
-        patience=10,
-        monitor="val_loss",
-        mode="min",
-        lr=1e-3,
-        lr_patience=10,
-        factor=0.75,
-        weight_decay=0.025,
-        raw_embeddings=False,
-        seq_size=20,
-        pca=False,
-        **trainer_kwargs
-    ):
-        """
-        Fits the ProteinMambularRegressor model to the training data.
-
-        Parameters
-        ----------
-        X : array-like or DataFrame
-            The training input samples.
-        y : array-like
-            The target values (class labels for classification, real numbers for regression).
-        val_size : float, optional
-            The proportion of the dataset to include in the validation split if `X_val` is not provided.
-        X_val : array-like or DataFrame, optional
-            The validation input samples.
-        y_val : array-like, optional
-            The validation target values.
-        max_epochs : int, optional
-            The maximum number of epochs for training.
-        random_state : int, optional
-            The seed used by the random number generator.
-        batch_size : int, optional
-            Size of the batches for training.
-        shuffle : bool, optional
-            Whether to shuffle the training data.
-        patience : int, optional
-            Patience for early stopping.
-        monitor : str, optional
-            Quantity to be monitored for early stopping.
-        mode : str, optional
-            One of {'auto', 'min', 'max'}. In 'min' mode, training will stop when the quantity monitored has stopped decreasing;
-            in 'max' mode, it will stop when the quantity monitored has stopped increasing.
-        lr : float, optional
-            Learning rate for the optimizer.
-        lr_patience : int, optional
-            Number of epochs with no improvement after which the learning rate will be reduced.
-        factor : float, optional
-            Factor by which the learning rate will be reduced.
-        weight_decay : float, optional
-            Weight decay coefficient for regularization in the optimizer.
-        raw_embeddings : bool, optional
-            Whether to use raw numerical features directly or to process them into embeddings.
-        seq_size : int, optional
-            The sequence size for processing numerical features when not using raw embeddings.
-        **trainer_kwargs : dict
-            Additional keyword arguments for the PyTorch Lightning Trainer.
-
-        Returns
-        -------
-        self : object
-            Returns an instance of self.
-        """
-            
-        if not isinstance(X, pd.DataFrame):
-            X = pd.DataFrame(X)
-        if X_val:
-            if not isinstance(X_val, pd.DataFrame):
-                X_val = pd.DataFrame(X_val)
-
-        # Apply PCA if indicated
-        if pca:
-            self.pca_transformer = PCA(n_components=seq_size)
-            X = pd.DataFrame(
-                self.pca_transformer.fit_transform(X)
-            )  # Fit and transform the PCA on the complete dataset
-            if X_val is not None:
-                X_val = pd.DataFrame(
-                    self.pca_transformer.transform(X_val)
-                )  # Transform validation data with the same PCA model
-
-            raw_embeddings = True
-
-        if not X_val:
-            X_train, X_val, y_train, y_val = self.split_data(
-                X, y, val_size, random_state
-            )
-        else:
-            X_train = X
-            y_train = y
-
-        data_module = self.preprocess_data(
-            X_train, y_train, X_val, y_val, batch_size, shuffle
-        )
-
-        if raw_embeddings:
-            self.config.d_model = X.shape[1]
-
-        self.model = BaseEmbeddingMambularRegressor(
-            config=self.config,
-            cat_feature_info=self.cat_feature_info,
-            num_feature_info=self.num_feature_info,
-            lr=lr,
-            lr_patience=lr_patience,
-            lr_factor=factor,
-            weight_decay=weight_decay,
-            raw_embeddings=raw_embeddings,
-            seq_size=seq_size,
-        )
-
-        early_stop_callback = EarlyStopping(
-            monitor=monitor, min_delta=0.00, patience=patience, verbose=False, mode=mode
-        )
-
-        checkpoint_callback = ModelCheckpoint(
-            monitor="val_loss",  # Adjust according to your validation metric
-            mode="min",
-            save_top_k=1,
-            dirpath="model_checkpoints",  # Specify the directory to save checkpoints
-            filename="best_model",
-        )
-
-        # Initialize the trainer and train the model
-        trainer = pl.Trainer(
-            max_epochs=max_epochs,
-            callbacks=[early_stop_callback, checkpoint_callback],
-            **trainer_kwargs
-        )
-        trainer.fit(self.model, data_module)
-
-        best_model_path = checkpoint_callback.best_model_path
-        if best_model_path:
-            checkpoint = torch.load(best_model_path)
-            self.model.load_state_dict(checkpoint["state_dict"])
-
-        return self
-
-    def predict(self, X):
-        """
-        Predicts target values for the given input samples.
-
-        Parameters
-        ----------
-        X : DataFrame or array-like, shape (n_samples, n_features)
-            The input samples for which to predict target values.
-
-        Returns
-        -------
-        predictions : ndarray, shape (n_samples,) or (n_samples, n_outputs)
-            The predicted target values.
-        """
-        # Preprocess the data
-        if not isinstance(X, pd.DataFrame):
-            X = pd.DataFrame(X)
-
-        if hasattr(self, "pca_transformer"):
-            X = pd.DataFrame(self.pca_transformer.transform(X))
-
-        device = next(self.model.parameters()).device
-        cat_tensors, num_tensors = self.preprocess_test_data(X)
-        if isinstance(cat_tensors, list):
-            cat_tensors = [tensor.to(device) for tensor in cat_tensors]
-        else:
-            cat_tensors = cat_tensors.to(device)
-
-        if isinstance(num_tensors, list):
-            num_tensors = [tensor.to(device) for tensor in num_tensors]
-        else:
-            num_tensors = num_tensors.to(device)
-
-        # Set the model to evaluation mode
-        self.model.eval()
-
-        # Perform inference
-        with torch.no_grad():
-            predictions = self.model(cat_tensors, num_tensors)
-
-        # Convert predictions to NumPy array and return
-        return predictions.cpu().numpy()
-
-    def evaluate(self, X, y_true, metrics=None):
-        """
-        Evaluate the model on the given data using specified metrics.
-
-        Example:
-            metrics = {
-                'Mean Squared Error': mean_squared_error,
-                'R2 Score': r2_score
-            }
-
-            # Assuming 'X_test' and 'y_test' are your test dataset and labels
-            # Evaluate using the specified metrics
-            results = regressor.evaluate(X_test, y_test, metrics=metrics)
-
-        Parameters
-        ----------
-        X : array-like or pd.DataFrame of shape (n_samples, n_features)
-            The input samples to predict.
-        y_true : array-like of shape (n_samples,) or (n_samples, n_outputs)
-            The true target values against which to evaluate the predictions.
-        metrics : dict
-            A dictionary where keys are metric names and values are the metric functions.
-
-        Returns
-        -------
-        scores : dict
-            A dictionary with metric names as keys and their corresponding scores as values.
-
-        Notes
-        -----
-        This method uses the `predict` method to generate predictions and computes each metric.
-        """
-        if metrics is None:
-            metrics = {"Mean Squared Error": mean_squared_error}
-
-        # Ensure input is in the correct format
-        if not isinstance(X, pd.DataFrame):
-            X = pd.DataFrame(X)
-
-        # Generate predictions using the trained model
-        predictions = self.predict(X)
-
-        # Initialize dictionary to store results
-        scores = {}
-
-        # Compute each metric
-        for metric_name, metric_func in metrics.items():
-            scores[metric_name] = metric_func(y_true, predictions)
-
-        return scores
+import lightning as pl
+import numpy as np
+import warnings
+import pandas as pd
+import torch
+from lightning.pytorch.callbacks import EarlyStopping, ModelCheckpoint
+from sklearn.base import BaseEstimator
+from sklearn.metrics import accuracy_score
+from sklearn.model_selection import train_test_split
+from torch.utils.data import DataLoader
+
+from ..base_models.classifier import BaseMambularClassifier
+from ..utils.configs import DefaultMambularConfig
+from ..utils.dataset import MambularDataModule, MambularDataset
+from ..utils.preprocessor import Preprocessor
+
+
+class MambularClassifier(BaseEstimator):
+    """
+    A classifier that mimics scikit-learn's API using PyTorch Lightning and a custom architecture.
+
+    This classifier is designed to work with tabular data and provides a flexible interface for specifying model
+    configurations and preprocessing steps. It integrates smoothly with scikit-learn's utilities, such as cross-validation
+    and grid search.
+
+    Parameters
+    ----------
+    # configuration parameters
+    lr : float, optional
+        Learning rate for the optimizer. Default is 1e-4.
+    lr_patience : int, optional
+        Number of epochs with no improvement on the validation loss to wait before reducing the learning rate. Default is 10.
+    weight_decay : float, optional
+        Weight decay (L2 penalty) coefficient. Default is 1e-6.
+    lr_factor : float, optional
+        Factor by which the learning rate will be reduced. Default is 0.1.
+    d_model : int, optional
+        Dimension of the model. Default is 64.
+    n_layers : int, optional
+        Number of layers. Default is 8.
+    expand_factor : int, optional
+        Expansion factor. Default is 2.
+    bias : bool, optional
+        Whether to use bias. Default is False.
+    d_conv : int, optional
+        Dimension of the convolution. Default is 16.
+    conv_bias : bool, optional
+        Whether to use bias in the convolution. Default is True.
+    dropout : float, optional
+        Dropout rate in the mamba blocks. Default is 0.05.
+    dt_rank : str, optional
+        Rank of the time dimension. Default is "auto".
+    d_state : int, optional
+        State dimension. Default is 16.
+    dt_scale : float, optional
+        Scale of the time dimension. Default is 1.0.
+    dt_init : str, optional
+        Initialization method for the time dimension. Default is "random".
+    dt_max : float, optional
+        Maximum value for the time dimension. Default is 0.1.
+    dt_min : float, optional
+        Minimum value for the time dimension. Default is 1e-3.
+    dt_init_floor : float, optional
+        Floor value for the time dimension initialization. Default is 1e-4.
+    norm : str, optional
+        Normalization method. Default is 'RMSNorm'.
+    activation : callable, optional
+        Activation function. Default is nn.SELU().
+    num_embedding_activation : callable, optional
+        Activation function for numerical embeddings. Default is nn.Identity().
+    head_layer_sizes : list, optional
+        Sizes of the layers in the head. Default is [64, 64, 32].
+    head_dropout : float, optional
+        Dropout rate for the head. Default is 0.5.
+    head_skip_layers : bool, optional
+        Whether to use skip layers in the head. Default is False.
+    head_activation : callable, optional
+        Activation function for the head. Default is nn.SELU().
+    head_use_batch_norm : bool, optional
+        Whether to use batch normalization in the head. Default is False.
+
+    # Preprocessor Parameters
+    n_bins : int, optional
+        The number of bins to use for numerical feature binning. Default is 50.
+    numerical_preprocessing : str, optional
+        The preprocessing strategy for numerical features. Default is 'ple'.
+    use_decision_tree_bins : bool, optional
+        If True, uses decision tree regression/classification to determine optimal bin edges for numerical feature binning. Default is False.
+    binning_strategy : str, optional
+        Defines the strategy for binning numerical features. Default is 'uniform'.
+    task : str, optional
+        Indicates the type of machine learning task ('regression' or 'classification'). Default is 'regression'.
+    cat_cutoff: float or int, optional
+        Indicates the cutoff after which integer values are treated as categorical. If float, it's treated as a percentage. If int, it's the maximum number of unique values for a column to be considered categorical. Default is 3%
+    treat_all_integers_as_numerical : bool, optional
+        If True, all integer columns will be treated as numerical, regardless of their unique value count or proportion. Default is False
+
+
+
+    Attributes
+    ----------
+    config : MambularConfig
+        Configuration object that holds model-specific settings.
+    preprocessor : Preprocessor
+        Preprocessor object for handling feature preprocessing like normalization and encoding.
+    model : BaseMambularClassifier or None
+        The underlying PyTorch Lightning model, instantiated upon calling the `fit` method.
+    """
+
+    def __init__(self, **kwargs):
+        # Known config arguments
+        config_arg_names = [
+            "lr",
+            "lr_patience",
+            "weight_decay",
+            "lr_factor",
+            "d_model",
+            "n_layers",
+            "expand_factor",
+            "bias",
+            "d_conv",
+            "conv_bias",
+            "dropout",
+            "dt_rank",
+            "d_state",
+            "dt_scale",
+            "dt_init",
+            "dt_max",
+            "dt_min",
+            "dt_init_floor",
+            "norm",
+            "activation",
+            "num_embedding_activation",
+            "head_layer_sizes",
+            "head_dropout",
+            "head_skip_layers",
+            "head_activation",
+            "head_use_batch_norm",
+        ]
+
+        preprocessor_arg_names = [
+            "n_bins",
+            "numerical_preprocessing",
+            "use_decision_tree_bins",
+            "binning_strategy",
+            "task",
+            "cat_cutoff",
+            "treat_all_integers_as_numerical",
+        ]
+
+        self.config_kwargs = {k: v for k, v in kwargs.items() if k in config_arg_names}
+        self.config = DefaultMambularConfig(**self.config_kwargs)
+
+        preprocessor_kwargs = {
+            k: v for k, v in kwargs.items() if k in preprocessor_arg_names
+        }
+        # Raise a warning if task is set to 'classification'
+        if preprocessor_kwargs.get("task") == "regression":
+            warnings.warn(
+                "The task in preprocessing binning is set to 'regression'. MambularClassifier is designed for classification tasks.",
+                UserWarning,
+            )
+
+        if "task" not in list(preprocessor_kwargs.keys()):
+            preprocessor_kwargs["task"] = "classification"
+
+        self.preprocessor = Preprocessor(**preprocessor_kwargs)
+        self.model = None
+
+    def get_params(self, deep=True):
+        """
+        Get parameters for this estimator.
+
+        Parameters
+        ----------
+        deep : bool, default=True
+            If True, will return the parameters for this estimator and contained subobjects that are estimators.
+
+
+        Returns
+        -------
+        params : dict
+            Parameter names mapped to their values.
+        """
+
+        params = self.config_kwargs  # Parameters used to initialize MambularConfig
+
+        # If deep=True, include parameters from nested components like preprocessor
+        if deep:
+            # Assuming Preprocessor has a get_params method
+            preprocessor_params = {
+                "preprocessor__" + key: value
+                for key, value in self.preprocessor.get_params().items()
+            }
+            params.update(preprocessor_params)
+
+        return params
+
+    def set_params(self, **parameters):
+        """
+        Set the parameters of this estimator.
+
+        Parameters
+        ----------
+        **parameters : dict
+            Estimator parameters.
+
+
+        Returns
+        -------
+        self : object
+            Estimator instance.
+        """
+        # Update config_kwargs with provided parameters
+        valid_config_keys = self.config_kwargs.keys()
+        config_updates = {k: v for k, v in parameters.items() if k in valid_config_keys}
+        self.config_kwargs.update(config_updates)
+
+        # Update the config object
+        for key, value in config_updates.items():
+            setattr(self.config, key, value)
+
+        # Handle preprocessor parameters (prefixed with 'preprocessor__')
+        preprocessor_params = {
+            k.split("__")[1]: v
+            for k, v in parameters.items()
+            if k.startswith("preprocessor__")
+        }
+        if preprocessor_params:
+            # Assuming Preprocessor has a set_params method
+            self.preprocessor.set_params(**preprocessor_params)
+
+        return self
+
+    def split_data(self, X, y, val_size, random_state):
+        """
+        Split the dataset into training and validation sets.
+
+        Parameters
+        ----------
+        X : array-like of shape (n_samples, n_features)
+            The input samples.
+        y : array-like of shape (n_samples,)
+            The target values.
+        val_size : float
+            The proportion of the dataset to include in the validation split.
+        random_state : int
+            Controls the shuffling applied to the data before applying the split.
+
+
+        Returns
+        -------
+        X_train, X_val, y_train, y_val : arrays
+            The split datasets.
+        """
+        X_train, X_val, y_train, y_val = train_test_split(
+            X, y, test_size=val_size, random_state=random_state
+        )
+
+        return X_train, X_val, y_train, y_val
+
+    def preprocess_data(self, X_train, y_train, X_val, y_val, batch_size, shuffle):
+        """
+        Preprocess the training and validation data and create corresponding DataLoaders.
+
+        Parameters
+        ----------
+        X_train : array-like of shape (n_samples, n_features)
+            The training input samples.
+        y_train : array-like of shape (n_samples,)
+            The training target values.
+        X_val : array-like of shape (n_samples, n_features)
+            The validation input samples.
+        y_val : array-like of shape (n_samples,)
+            The validation target values.
+        batch_size : int
+            Size of mini-batches for the DataLoader.
+        shuffle : bool
+            Whether to shuffle the training data before splitting into batches.
+
+
+        Returns
+        -------
+        data_module : MambularDataModule
+            An instance of MambularDataModule containing training and validation DataLoaders.
+        """
+        self.preprocessor.fit(
+            pd.concat([X_train, X_val], axis=0).reset_index(drop=True),
+            np.concatenate((y_train, y_val), axis=0),
+        )
+        train_preprocessed_data = self.preprocessor.transform(X_train)
+        val_preprocessed_data = self.preprocessor.transform(X_val)
+
+        # Update feature info based on the actual processed data
+        (
+            self.cat_feature_info,
+            self.num_feature_info,
+        ) = self.preprocessor.get_feature_info()
+
+        # Initialize lists for tensors
+        train_cat_tensors = []
+        train_num_tensors = []
+        val_cat_tensors = []
+        val_num_tensors = []
+
+        # Populate tensors for categorical features, if present in processed data
+        for key in self.cat_feature_info:
+            cat_key = "cat_" + key  # Assuming categorical keys are prefixed with 'cat_'
+            if cat_key in train_preprocessed_data:
+                train_cat_tensors.append(
+                    torch.tensor(train_preprocessed_data[cat_key], dtype=torch.long)
+                )
+            if cat_key in val_preprocessed_data:
+                val_cat_tensors.append(
+                    torch.tensor(val_preprocessed_data[cat_key], dtype=torch.long)
+                )
+
+            binned_key = "num_" + key  # for binned features
+            if binned_key in train_preprocessed_data:
+                train_cat_tensors.append(
+                    torch.tensor(train_preprocessed_data[binned_key], dtype=torch.long)
+                )
+
+            if binned_key in val_preprocessed_data:
+                val_cat_tensors.append(
+                    torch.tensor(val_preprocessed_data[binned_key], dtype=torch.long)
+                )
+
+        # Populate tensors for numerical features, if present in processed data
+        for key in self.num_feature_info:
+            num_key = "num_" + key  # Assuming numerical keys are prefixed with 'num_'
+            if num_key in train_preprocessed_data:
+                train_num_tensors.append(
+                    torch.tensor(train_preprocessed_data[num_key], dtype=torch.float32)
+                )
+            if num_key in val_preprocessed_data:
+                val_num_tensors.append(
+                    torch.tensor(val_preprocessed_data[num_key], dtype=torch.float32)
+                )
+
+        train_labels = torch.tensor(y_train, dtype=torch.long)
+        val_labels = torch.tensor(y_val, dtype=torch.long)
+
+        # Create datasets
+        train_dataset = MambularDataset(
+            train_cat_tensors, train_num_tensors, train_labels, regression=False
+        )
+        val_dataset = MambularDataset(
+            val_cat_tensors, val_num_tensors, val_labels, regression=False
+        )
+
+        # Create dataloaders
+        train_dataloader = DataLoader(
+            train_dataset, batch_size=batch_size, shuffle=shuffle
+        )
+        val_dataloader = DataLoader(val_dataset, batch_size=batch_size)
+
+        return MambularDataModule(train_dataloader, val_dataloader)
+
+    def preprocess_test_data(self, X):
+        """
+        Preprocesses the test data and creates tensors for categorical and numerical features.
+
+        Parameters
+        ----------
+        X : DataFrame or array-like, shape (n_samples, n_features)
+            Test feature set.
+
+
+        Returns
+        -------
+        cat_tensors : list of Tensors
+            List of tensors for each categorical feature.
+        num_tensors : list of Tensors
+            List of tensors for each numerical feature.
+        """
+        processed_data = self.preprocessor.transform(X)
+
+        # Initialize lists for tensors
+        cat_tensors = []
+        num_tensors = []
+
+        # Populate tensors for categorical features
+        for key in self.cat_feature_info:
+            cat_key = "cat_" + key  # Assuming categorical keys are prefixed with 'cat_'
+            if cat_key in processed_data:
+                cat_tensors.append(
+                    torch.tensor(processed_data[cat_key], dtype=torch.long)
+                )
+
+            binned_key = "num_" + key  # for binned features
+            if binned_key in processed_data:
+                cat_tensors.append(
+                    torch.tensor(processed_data[binned_key], dtype=torch.long)
+                )
+
+        # Populate tensors for numerical features
+        for key in self.num_feature_info:
+            num_key = "num_" + key  # Assuming numerical keys are prefixed with 'num_'
+            if num_key in processed_data:
+                num_tensors.append(
+                    torch.tensor(processed_data[num_key], dtype=torch.float32)
+                )
+
+        return cat_tensors, num_tensors
+
+    def fit(
+        self,
+        X,
+        y,
+        val_size: float = 0.2,
+        X_val=None,
+        y_val=None,
+        max_epochs: int = 100,
+        random_state: int = 101,
+        batch_size: int = 128,
+        shuffle: bool = True,
+        patience: int = 15,
+        monitor: str = "val_loss",
+        mode: str = "min",
+        lr: float = 1e-4,
+        lr_patience: int = 10,
+        factor: float = 0.1,
+        weight_decay: float = 1e-06,
+        **trainer_kwargs
+    ):
+        """
+        Fit the model to the given training data, optionally using a separate validation set.
+
+        Parameters
+        ----------
+        X : array-like or pd.DataFrame of shape (n_samples, n_features)
+            The training input samples.
+        y : array-like of shape (n_samples,) or (n_samples, n_outputs)
+            The target values (class labels in classification, real numbers in regression).
+        val_size : float, default=0.2
+            The proportion of the dataset to include in the validation split if `X_val` is None. Ignored if `X_val` is provided.
+        X_val : array-like or pd.DataFrame of shape (n_samples, n_features), optional
+            The validation input samples. If provided, `X` and `y` are not split and this data is used for validation.
+        y_val : array-like of shape (n_samples,) or (n_samples, n_outputs), optional
+            The validation target values. Required if `X_val` is provided.
+        max_epochs : int, default=100
+            Maximum number of epochs for training.
+        random_state : int, default=101
+            Seed used by the random number generator for shuffling the data if `X_val` is not provided.
+        batch_size : int, default=64
+            Number of samples per gradient update.
+        shuffle : bool, default=True
+            Whether to shuffle the training data before each epoch if `X_val` is not provided.
+        patience : int, default=10
+            Number of epochs with no improvement after which training will be stopped if using early stopping.
+        monitor : str, default="val_loss"
+            Quantity to be monitored for early stopping.
+        mode : str, default="min"
+            One of {"min", "max"}. In "min" mode, training will stop when the quantity monitored has stopped decreasing; in "max" mode, it will stop when the quantity monitored has stopped increasing.
+        lr : float, default=1e-3
+            Learning rate for the optimizer.
+        lr_patience : int, default=10
+            Number of epochs with no improvement after which the learning rate will be reduced.
+        factor : float, default=0.75
+            Factor by which the learning rate will be reduced. new_lr = lr * factor.
+        weight_decay : float, default=0.025
+            Weight decay (L2 penalty) parameter.
+        **trainer_kwargs : dict
+            Additional keyword arguments to be passed to the PyTorch Lightning Trainer constructor.
+
+
+        Returns
+        -------
+        self : object
+            The fitted estimator.
+        """
+
+        if not isinstance(X, pd.DataFrame):
+            X = pd.DataFrame(X)
+        if X_val:
+            if not isinstance(X_val, pd.DataFrame):
+                X_val = pd.DataFrame(X_val)
+
+        num_classes = len(np.unique(y))
+
+        if not X_val:
+            X_train, X_val, y_train, y_val = self.split_data(
+                X, y, val_size, random_state
+            )
+
+        self.data_module = self.preprocess_data(
+            X_train, y_train, X_val, y_val, batch_size, shuffle
+        )
+
+        self.model = BaseMambularClassifier(
+            num_classes=num_classes,
+            config=self.config,
+            cat_feature_info=self.cat_feature_info,
+            num_feature_info=self.num_feature_info,
+            lr=lr,
+            lr_patience=lr_patience,
+            lr_factor=factor,
+            weight_decay=weight_decay,
+        )
+
+        early_stop_callback = EarlyStopping(
+            monitor=monitor, min_delta=0.00, patience=patience, verbose=False, mode=mode
+        )
+
+        checkpoint_callback = ModelCheckpoint(
+            monitor="val_loss",  # Adjust according to your validation metric
+            mode="min",
+            save_top_k=1,
+            dirpath="model_checkpoints",  # Specify the directory to save checkpoints
+            filename="best_model",
+        )
+
+        # Initialize the trainer and train the model
+        trainer = pl.Trainer(
+            max_epochs=max_epochs,
+            callbacks=[early_stop_callback, checkpoint_callback],
+            **trainer_kwargs
+        )
+        trainer.fit(self.model, self.data_module)
+
+        best_model_path = checkpoint_callback.best_model_path
+        if best_model_path:
+            checkpoint = torch.load(best_model_path)
+            self.model.load_state_dict(checkpoint["state_dict"])
+
+        return self
+
+    def predict(self, X):
+        """
+        Predict the class labels for the given input samples.
+
+        Parameters
+        ----------
+        X : array-like or pd.DataFrame of shape (n_samples, n_features)
+            The input samples to predict.
+
+
+        Returns
+        -------
+        predictions : ndarray of shape (n_samples,)
+            Predicted class labels for each input sample.
+
+
+        Notes
+        -----
+        The method preprocesses the input data using the same preprocessor used during training,
+        sets the model to evaluation mode, and then performs inference to predict the class labels.
+        The predictions are converted from a PyTorch tensor to a NumPy array before being returned.
+
+        """
+
+        # Preprocess the data
+        if not isinstance(X, pd.DataFrame):
+            X = pd.DataFrame(X)
+        device = next(self.model.parameters()).device
+        cat_tensors, num_tensors = self.preprocess_test_data(X)
+        if isinstance(cat_tensors, list):
+            cat_tensors = [tensor.to(device) for tensor in cat_tensors]
+        else:
+            cat_tensors = cat_tensors.to(device)
+
+        if isinstance(num_tensors, list):
+            num_tensors = [tensor.to(device) for tensor in num_tensors]
+        else:
+            num_tensors = num_tensors.to(device)
+
+        # Set the model to evaluation mode
+        self.model.eval()
+
+        # Perform inference
+        with torch.no_grad():
+            logits = self.model(num_features=num_tensors, cat_features=cat_tensors)
+
+            # Check the shape of the logits to determine binary or multi-class classification
+            if logits.shape[1] == 1:
+                # Binary classification
+                probabilities = torch.sigmoid(logits)
+                predictions = (probabilities > 0.5).long().squeeze()
+            else:
+                # Multi-class classification
+                probabilities = torch.softmax(logits, dim=1)
+                predictions = torch.argmax(probabilities, dim=1)
+
+        # Convert predictions to NumPy array and return
+        return predictions.cpu().numpy()
+
+    def predict_proba(self, X):
+        """
+        Predict class probabilities for the given input samples.
+
+        Parameters
+        ----------
+        X : array-like or pd.DataFrame of shape (n_samples, n_features)
+            The input samples for which to predict class probabilities.
+
+
+        Notes
+        -----
+        The method preprocesses the input data using the same preprocessor used during training,
+        sets the model to evaluation mode, and then performs inference to predict the class probabilities.
+        Softmax is applied to the logits to obtain probabilities, which are then converted from a PyTorch tensor
+        to a NumPy array before being returned.
+
+
+        Examples
+        --------
+        >>> from sklearn.metrics import accuracy_score, precision_score, f1_score, roc_auc_score
+        >>> # Define the metrics you want to evaluate
+        >>> metrics = {
+        ...     'Accuracy': (accuracy_score, False),
+        ...     'Precision': (precision_score, False),
+        ...     'F1 Score': (f1_score, False),
+        ...     'AUC Score': (roc_auc_score, True)
+        ... }
+        >>> # Assuming 'X_test' and 'y_test' are your test dataset and labels
+        >>> # Evaluate using the specified metrics
+        >>> results = classifier.evaluate(X_test, y_test, metrics=metrics)
+
+
+        Returns
+        -------
+        probabilities : ndarray of shape (n_samples, n_classes)
+            Predicted class probabilities for each input sample.
+
+        """
+        # Preprocess the data
+        if not isinstance(X, pd.DataFrame):
+            X = pd.DataFrame(X)
+        device = next(self.model.parameters()).device
+        cat_tensors, num_tensors = self.preprocess_test_data(X)
+        if isinstance(cat_tensors, list):
+            cat_tensors = [tensor.to(device) for tensor in cat_tensors]
+        else:
+            cat_tensors = cat_tensors.to(device)
+
+        if isinstance(num_tensors, list):
+            num_tensors = [tensor.to(device) for tensor in num_tensors]
+        else:
+            num_tensors = num_tensors.to(device)
+
+        # Set the model to evaluation mode
+        self.model.eval()
+
+        # Perform inference
+        with torch.no_grad():
+            logits = self.model(num_features=num_tensors, cat_features=cat_tensors)
+            if logits.shape[1] > 1:
+                probabilities = torch.softmax(logits, dim=1)
+            else:
+                probabilities = torch.sigmoid(logits)
+
+        # Convert probabilities to NumPy array and return
+        return probabilities.cpu().numpy()
+
+    def evaluate(self, X, y_true, metrics=None):
+        """
+        Evaluate the model on the given data using specified metrics.
+
+        Parameters
+        ----------
+        X : array-like or pd.DataFrame of shape (n_samples, n_features)
+            The input samples to predict.
+        y_true : array-like of shape (n_samples,)
+            The true class labels against which to evaluate the predictions.
+        metrics : dict
+            A dictionary where keys are metric names and values are tuples containing the metric function
+            and a boolean indicating whether the metric requires probability scores (True) or class labels (False).
+
+
+        Returns
+        -------
+        scores : dict
+            A dictionary with metric names as keys and their corresponding scores as values.
+
+
+        Notes
+        -----
+        This method uses either the `predict` or `predict_proba` method depending on the metric requirements.
+        """
+        # Ensure input is in the correct format
+        if metrics is None:
+            metrics = {"Accuracy": (accuracy_score, False)}
+
+        if not isinstance(X, pd.DataFrame):
+            X = pd.DataFrame(X)
+
+        # Initialize dictionary to store results
+        scores = {}
+
+        # Generate class probabilities if any metric requires them
+        if any(use_proba for _, use_proba in metrics.values()):
+            probabilities = self.predict_proba(X)
+
+        # Generate class labels if any metric requires them
+        if any(not use_proba for _, use_proba in metrics.values()):
+            predictions = self.predict(X)
+
+        # Compute each metric
+        for metric_name, (metric_func, use_proba) in metrics.items():
+            if use_proba:
+                scores[metric_name] = metric_func(y_true, probabilities)
+            else:
+                scores[metric_name] = metric_func(y_true, predictions)
+
+        return scores
```

### Comparing `mambular-0.1.2/mambular/models/sklearn_regressor.py` & `mambular-0.1.3/mambular/models/sklearn_embedding_classifier.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,506 +1,730 @@
-from sklearn.model_selection import train_test_split
-import pytorch_lightning as pl
-import torch
-from torch.utils.data import DataLoader
-from pytorch_lightning.callbacks import ModelCheckpoint, EarlyStopping
-from ..base_models.regressor import BaseMambularRegressor
-from ..utils.config import MambularConfig
-from ..utils.preprocessor import Preprocessor
-from ..utils.dataset import MambularDataModule, MambularDataset
-from sklearn.base import BaseEstimator
-import pandas as pd
-from sklearn.metrics import mean_squared_error
-
-
-class MambularRegressor(BaseEstimator):
-    """
-    A regressor implemented using PyTorch Lightning that follows the scikit-learn API conventions. This class is designed
-    to work with tabular data, offering a straightforward way to specify model configurations and preprocessing steps. It
-    integrates seamlessly with scikit-learn's tools such as cross-validation and grid search.
-
-    Parameters
-    ----------
-    **kwargs : Various
-        Accepts any number of keyword arguments. Arguments recognized as model configuration options are passed to the
-        MambularConfig constructor. Remaining arguments are assumed to be preprocessor options and passed to the
-        Preprocessor constructor.
-
-    Attributes
-    ----------
-    config : MambularConfig
-        An object storing the configuration settings for the model.
-    preprocessor : Preprocessor
-        An object responsible for preprocessing the input data, such as encoding categorical variables and scaling numerical features.
-    model : BaseMambularRegressor or None
-        The underlying regression model, which is a PyTorch Lightning module. It is instantiated when the `fit` method is called.
-    """
-
-    def __init__(self, **kwargs):
-        # Known config arguments
-        print("Received kwargs:", kwargs)
-        config_arg_names = [
-            "d_model",
-            "n_layers",
-            "dt_rank",
-            "output_dimension",
-            "pooling_method",
-            "norm",
-            "cls",
-            "dt_min",
-            "dt_max",
-            "dropout",
-            "bias",
-            "weight_decay",
-            "conv_bias",
-            "d_state",
-            "expand_factor",
-            "d_conv",
-            "dt_init",
-            "dt_scale",
-            "dt_init_floor",
-            "tabular_head_units",
-            "tabular_head_activation",
-            "tabular_head_dropout",
-            "num_emebedding_activation",
-            "layer_norm_after_embedding",
-        ]
-        self.config_kwargs = {k: v for k, v in kwargs.items() if k in config_arg_names}
-        self.config = MambularConfig(**self.config_kwargs)
-
-        # The rest are assumed to be preprocessor arguments
-        preprocessor_kwargs = {
-            k: v for k, v in kwargs.items() if k not in config_arg_names
-        }
-        self.preprocessor = Preprocessor(**preprocessor_kwargs)
-        self.model = None
-
-    def get_params(self, deep=True):
-        """
-        Get parameters for this estimator. Overrides the BaseEstimator method.
-
-        Parameters
-        ----------
-        deep : bool, default=True
-            If True, returns the parameters for this estimator and contained sub-objects that are estimators.
-
-        Returns
-        -------
-        params : dict
-            Parameter names mapped to their values.
-        """
-        params = self.config_kwargs  # Parameters used to initialize MambularConfig
-
-        # If deep=True, include parameters from nested components like preprocessor
-        if deep:
-            # Assuming Preprocessor has a get_params method
-            preprocessor_params = {
-                "preprocessor__" + key: value
-                for key, value in self.preprocessor.get_params().items()
-            }
-            params.update(preprocessor_params)
-
-        return params
-
-    def set_params(self, **parameters):
-        """
-        Set the parameters of this estimator. Overrides the BaseEstimator method.
-
-        Parameters
-        ----------
-        **parameters : dict
-            Estimator parameters to be set.
-
-        Returns
-        -------
-        self : object
-            The instance with updated parameters.
-        """
-        # Update config_kwargs with provided parameters
-        valid_config_keys = self.config_kwargs.keys()
-        config_updates = {k: v for k, v in parameters.items() if k in valid_config_keys}
-        self.config_kwargs.update(config_updates)
-
-        # Update the config object
-        for key, value in config_updates.items():
-            setattr(self.config, key, value)
-
-        # Handle preprocessor parameters (prefixed with 'preprocessor__')
-        preprocessor_params = {
-            k.split("__")[1]: v
-            for k, v in parameters.items()
-            if k.startswith("preprocessor__")
-        }
-        if preprocessor_params:
-            # Assuming Preprocessor has a set_params method
-            self.preprocessor.set_params(**preprocessor_params)
-
-        return self
-
-    def split_data(self, X, y, val_size, random_state):
-        """
-        Splits the dataset into training and validation sets.
-
-        Parameters
-        ----------
-        X : array-like or DataFrame, shape (n_samples, n_features)
-            Input features.
-        y : array-like, shape (n_samples,) or (n_samples, n_targets)
-            Target values.
-        val_size : float
-            The proportion of the dataset to include in the validation split.
-        random_state : int
-            Controls the shuffling applied to the data before applying the split.
-
-        Returns
-        -------
-        X_train, X_val, y_train, y_val : arrays
-            The split datasets.
-        """
-        X_train, X_val, y_train, y_val = train_test_split(
-            X, y, test_size=val_size, random_state=random_state
-        )
-
-        return X_train, X_val, y_train, y_val
-
-    def preprocess_data(self, X_train, y_train, X_val, y_val, batch_size, shuffle):
-        """
-        Preprocesses the training and validation data, and creates DataLoaders for them.
-
-        Parameters
-        ----------
-        X_train : DataFrame or array-like, shape (n_samples_train, n_features)
-            Training feature set.
-        y_train : array-like, shape (n_samples_train,)
-            Training target values.
-        X_val : DataFrame or array-like, shape (n_samples_val, n_features)
-            Validation feature set.
-        y_val : array-like, shape (n_samples_val,)
-            Validation target values.
-        batch_size : int
-            Size of batches for the DataLoader.
-        shuffle : bool
-            Whether to shuffle the training data in the DataLoader.
-
-        Returns
-        -------
-        data_module : MambularDataModule
-            An instance of MambularDataModule containing the training and validation DataLoaders.
-        """
-        train_preprocessed_data = self.preprocessor.fit_transform(X_train, y_train)
-        val_preprocessed_data = self.preprocessor.transform(X_val)
-
-        # Update feature info based on the actual processed data
-        (
-            self.cat_feature_info,
-            self.num_feature_info,
-        ) = self.preprocessor.get_feature_info()
-
-        # Initialize lists for tensors
-        train_cat_tensors = []
-        train_num_tensors = []
-        val_cat_tensors = []
-        val_num_tensors = []
-
-        # Populate tensors for categorical features, if present in processed data
-        for key in self.cat_feature_info:
-            cat_key = "cat_" + key  # Assuming categorical keys are prefixed with 'cat_'
-            if cat_key in train_preprocessed_data:
-                train_cat_tensors.append(
-                    torch.tensor(train_preprocessed_data[cat_key], dtype=torch.long)
-                )
-            if cat_key in val_preprocessed_data:
-                val_cat_tensors.append(
-                    torch.tensor(val_preprocessed_data[cat_key], dtype=torch.long)
-                )
-
-            binned_key = "num_" + key  # for binned features
-            if binned_key in train_preprocessed_data:
-                train_cat_tensors.append(
-                    torch.tensor(train_preprocessed_data[binned_key], dtype=torch.long)
-                )
-
-            if binned_key in val_preprocessed_data:
-                val_cat_tensors.append(
-                    torch.tensor(val_preprocessed_data[binned_key], dtype=torch.long)
-                )
-
-        # Populate tensors for numerical features, if present in processed data
-        for key in self.num_feature_info:
-            num_key = "num_" + key  # Assuming numerical keys are prefixed with 'num_'
-            if num_key in train_preprocessed_data:
-                train_num_tensors.append(
-                    torch.tensor(train_preprocessed_data[num_key], dtype=torch.float)
-                )
-            if num_key in val_preprocessed_data:
-                val_num_tensors.append(
-                    torch.tensor(val_preprocessed_data[num_key], dtype=torch.float)
-                )
-
-        train_labels = torch.tensor(y_train, dtype=torch.float)
-        val_labels = torch.tensor(y_val, dtype=torch.float)
-
-        # Create datasets
-        train_dataset = MambularDataset(
-            train_cat_tensors, train_num_tensors, train_labels
-        )
-        val_dataset = MambularDataset(val_cat_tensors, val_num_tensors, val_labels)
-
-        # Create dataloaders
-        train_dataloader = DataLoader(
-            train_dataset, batch_size=batch_size, shuffle=shuffle
-        )
-        val_dataloader = DataLoader(val_dataset, batch_size=batch_size)
-
-        return MambularDataModule(train_dataloader, val_dataloader)
-
-    def preprocess_test_data(self, X):
-        """
-        Preprocesses the test data and creates tensors for categorical and numerical features.
-
-        Parameters
-        ----------
-        X : DataFrame or array-like, shape (n_samples, n_features)
-            Test feature set.
-
-        Returns
-        -------
-        cat_tensors : list of Tensors
-            List of tensors for each categorical feature.
-        num_tensors : list of Tensors
-            List of tensors for each numerical feature.
-        """
-        processed_data = self.preprocessor.transform(X)
-
-        # Initialize lists for tensors
-        cat_tensors = []
-        num_tensors = []
-
-        # Populate tensors for categorical features
-        for key in self.cat_feature_info:
-            cat_key = "cat_" + key  # Assuming categorical keys are prefixed with 'cat_'
-            if cat_key in processed_data:
-                cat_tensors.append(
-                    torch.tensor(processed_data[cat_key], dtype=torch.long)
-                )
-
-            binned_key = "num_" + key  # for binned features
-            if binned_key in processed_data:
-                cat_tensors.append(
-                    torch.tensor(processed_data[binned_key], dtype=torch.long)
-                )
-
-        # Populate tensors for numerical features
-        for key in self.num_feature_info:
-            num_key = "num_" + key  # Assuming numerical keys are prefixed with 'num_'
-            if num_key in processed_data:
-                num_tensors.append(
-                    torch.tensor(processed_data[num_key], dtype=torch.float)
-                )
-
-        return cat_tensors, num_tensors
-
-    def fit(
-        self,
-        X,
-        y,
-        val_size=0.2,
-        X_val=None,
-        y_val=None,
-        max_epochs=100,
-        random_state=101,
-        batch_size=128,
-        shuffle=True,
-        patience=10,
-        monitor="val_loss",
-        mode="min",
-        lr=1e-3,
-        lr_patience=5,
-        factor=0.75,
-        weight_decay=1e-06,
-        **trainer_kwargs
-    ):
-        """
-        Trains the regression model using the provided training data. Optionally, a separate validation set can be used.
-
-        Parameters
-        ----------
-        X : DataFrame or array-like, shape (n_samples, n_features)
-            The training input samples.
-        y : array-like, shape (n_samples,) or (n_samples, n_targets)
-            The target values (real numbers).
-        val_size : float, default=0.2
-            The proportion of the dataset to include in the validation split if `X_val` is None. Ignored if `X_val` is provided.
-        X_val : DataFrame or array-like, shape (n_samples, n_features), optional
-            The validation input samples. If provided, `X` and `y` are not split and this data is used for validation.
-        y_val : array-like, shape (n_samples,) or (n_samples, n_targets), optional
-            The validation target values. Required if `X_val` is provided.
-        max_epochs : int, default=100
-            Maximum number of epochs for training.
-        random_state : int, default=101
-            Controls the shuffling applied to the data before applying the split.
-        batch_size : int, default=64
-            Number of samples per gradient update.
-        shuffle : bool, default=True
-            Whether to shuffle the training data before each epoch.
-        patience : int, default=10
-            Number of epochs with no improvement on the validation loss to wait before early stopping.
-        monitor : str, default="val_loss"
-            The metric to monitor for early stopping.
-        mode : str, default="min"
-            Whether the monitored metric should be minimized (`min`) or maximized (`max`).
-        lr : float, default=1e-3
-            Learning rate for the optimizer.
-        lr_patience : int, default=10
-            Number of epochs with no improvement on the validation loss to wait before reducing the learning rate.
-        factor : float, default=0.75
-            Factor by which the learning rate will be reduced.
-        weight_decay : float, default=0.025
-            Weight decay (L2 penalty) coefficient.
-        **trainer_kwargs : Additional keyword arguments for PyTorch Lightning's Trainer class.
-
-        Returns
-        -------
-        self : object
-            The fitted regressor.
-        """
-        if not isinstance(X, pd.DataFrame):
-            X = pd.DataFrame(X)
-        if X_val:
-            if not isinstance(X_val, pd.DataFrame):
-                X_val = pd.DataFrame(X_val)
-
-        if not X_val:
-            X_train, X_val, y_train, y_val = self.split_data(
-                X, y, val_size, random_state
-            )
-
-        data_module = self.preprocess_data(
-            X_train, y_train, X_val, y_val, batch_size, shuffle
-        )
-
-        self.model = BaseMambularRegressor(
-            config=self.config,
-            cat_feature_info=self.cat_feature_info,
-            num_feature_info=self.num_feature_info,
-            lr=lr,
-            lr_patience=lr_patience,
-            lr_factor=factor,
-            weight_decay=weight_decay,
-        )
-
-        early_stop_callback = EarlyStopping(
-            monitor=monitor, min_delta=0.00, patience=patience, verbose=False, mode=mode
-        )
-
-        checkpoint_callback = ModelCheckpoint(
-            monitor="val_loss",  # Adjust according to your validation metric
-            mode="min",
-            save_top_k=1,
-            dirpath="model_checkpoints",  # Specify the directory to save checkpoints
-            filename="best_model",
-        )
-
-        # Initialize the trainer and train the model
-        trainer = pl.Trainer(
-            max_epochs=max_epochs,
-            callbacks=[early_stop_callback, checkpoint_callback],
-            **trainer_kwargs
-        )
-        trainer.fit(self.model, data_module)
-
-        best_model_path = checkpoint_callback.best_model_path
-        if best_model_path:
-            checkpoint = torch.load(best_model_path)
-            self.model.load_state_dict(checkpoint["state_dict"])
-
-        return self
-
-    def predict(self, X):
-        """
-        Predicts target values for the given input samples.
-
-        Parameters
-        ----------
-        X : DataFrame or array-like, shape (n_samples, n_features)
-            The input samples for which to predict target values.
-
-        Returns
-        -------
-        predictions : ndarray, shape (n_samples,) or (n_samples, n_outputs)
-            The predicted target values.
-        """
-        # Preprocess the data
-        if not isinstance(X, pd.DataFrame):
-            X = pd.DataFrame(X)
-        device = next(self.model.parameters()).device
-        cat_tensors, num_tensors = self.preprocess_test_data(X)
-        if isinstance(cat_tensors, list):
-            cat_tensors = [tensor.to(device) for tensor in cat_tensors]
-        else:
-            cat_tensors = cat_tensors.to(device)
-
-        if isinstance(num_tensors, list):
-            num_tensors = [tensor.to(device) for tensor in num_tensors]
-        else:
-            num_tensors = num_tensors.to(device)
-
-        # Set the model to evaluation mode
-        self.model.eval()
-
-        # Perform inference
-        with torch.no_grad():
-            predictions = self.model(cat_tensors, num_tensors)
-
-        # Convert predictions to NumPy array and return
-        return predictions.cpu().numpy()
-
-    def evaluate(self, X, y_true, metrics=None):
-        """
-        Evaluate the model on the given data using specified metrics.
-
-        Example:
-            metrics = {
-                'Mean Squared Error': mean_squared_error,
-                'R2 Score': r2_score
-            }
-
-            # Assuming 'X_test' and 'y_test' are your test dataset and labels
-            # Evaluate using the specified metrics
-            results = regressor.evaluate(X_test, y_test, metrics=metrics)
-
-        Parameters
-        ----------
-        X : array-like or pd.DataFrame of shape (n_samples, n_features)
-            The input samples to predict.
-        y_true : array-like of shape (n_samples,) or (n_samples, n_outputs)
-            The true target values against which to evaluate the predictions.
-        metrics : dict
-            A dictionary where keys are metric names and values are the metric functions.
-
-        Returns
-        -------
-        scores : dict
-            A dictionary with metric names as keys and their corresponding scores as values.
-
-        Notes
-        -----
-        This method uses the `predict` method to generate predictions and computes each metric.
-        """
-        if metrics is None:
-            metrics = {"Mean Squared Error": mean_squared_error}
-
-        # Ensure input is in the correct format
-        if not isinstance(X, pd.DataFrame):
-            X = pd.DataFrame(X)
-
-        # Generate predictions using the trained model
-        predictions = self.predict(X)
-
-        # Initialize dictionary to store results
-        scores = {}
-
-        # Compute each metric
-        for metric_name, metric_func in metrics.items():
-            scores[metric_name] = metric_func(y_true, predictions)
-
-        return scores
+import lightning as pl
+import numpy as np
+import pandas as pd
+import warnings
+
+import torch
+from lightning.pytorch.callbacks import EarlyStopping, ModelCheckpoint
+from sklearn.base import BaseEstimator
+from sklearn.decomposition import PCA
+from sklearn.metrics import accuracy_score
+from sklearn.model_selection import train_test_split
+from torch.utils.data import DataLoader
+
+from ..base_models.embedding_classifier import BaseEmbeddingMambularClassifier
+from ..utils.configs import DefaultMambularConfig
+from ..utils.dataset import EmbeddingMambularDataset, MambularDataModule
+from ..utils.preprocessor import Preprocessor
+
+
+class EmbeddingMambularClassifier(BaseEstimator):
+    """
+    Provides an scikit-learn-like interface for the ProteinMambularClassifier, making it compatible with
+    scikit-learn's utilities and workflow. This class encapsulates the PyTorch Lightning model, preprocessing,
+    and data loading, offering methods for fitting, predicting, and probability estimation in a manner akin
+    to scikit-learn's API.
+
+    Parameters
+    ----------
+    # configuration parameters
+    lr : float, optional
+        Learning rate for the optimizer. Default is 1e-4.
+    lr_patience : int, optional
+        Number of epochs with no improvement on the validation loss to wait before reducing the learning rate. Default is 10.
+    weight_decay : float, optional
+        Weight decay (L2 penalty) coefficient. Default is 1e-6.
+    lr_factor : float, optional
+        Factor by which the learning rate will be reduced. Default is 0.1.
+    d_model : int, optional
+        Dimension of the model. Default is 64.
+    n_layers : int, optional
+        Number of layers. Default is 8.
+    expand_factor : int, optional
+        Expansion factor. Default is 2.
+    bias : bool, optional
+        Whether to use bias. Default is False.
+    d_conv : int, optional
+        Dimension of the convolution. Default is 16.
+    conv_bias : bool, optional
+        Whether to use bias in the convolution. Default is True.
+    dropout : float, optional
+        Dropout rate in the mamba blocks. Default is 0.05.
+    dt_rank : str, optional
+        Rank of the time dimension. Default is "auto".
+    d_state : int, optional
+        State dimension. Default is 16.
+    dt_scale : float, optional
+        Scale of the time dimension. Default is 1.0.
+    dt_init : str, optional
+        Initialization method for the time dimension. Default is "random".
+    dt_max : float, optional
+        Maximum value for the time dimension. Default is 0.1.
+    dt_min : float, optional
+        Minimum value for the time dimension. Default is 1e-3.
+    dt_init_floor : float, optional
+        Floor value for the time dimension initialization. Default is 1e-4.
+    norm : str, optional
+        Normalization method. Default is 'RMSNorm'.
+    activation : callable, optional
+        Activation function. Default is nn.SELU().
+    num_embedding_activation : callable, optional
+        Activation function for numerical embeddings. Default is nn.Identity().
+    head_layer_sizes : list, optional
+        Sizes of the layers in the head. Default is [64, 64, 32].
+    head_dropout : float, optional
+        Dropout rate for the head. Default is 0.5.
+    head_skip_layers : bool, optional
+        Whether to use skip layers in the head. Default is False.
+    head_activation : callable, optional
+        Activation function for the head. Default is nn.SELU().
+    head_use_batch_norm : bool, optional
+        Whether to use batch normalization in the head. Default is False.
+
+    # Preprocessor Parameters
+    n_bins : int, optional
+        The number of bins to use for numerical feature binning. Default is 50.
+    numerical_preprocessing : str, optional
+        The preprocessing strategy for numerical features. Default is 'ple'.
+    use_decision_tree_bins : bool, optional
+        If True, uses decision tree regression/classification to determine optimal bin edges for numerical feature binning. Default is False.
+    binning_strategy : str, optional
+        Defines the strategy for binning numerical features. Default is 'uniform'.
+    task : str, optional
+        Indicates the type of machine learning task ('regression' or 'classification'). Default is 'regression'.
+    cat_cutoff: float or int, optional
+        Indicates the cutoff after which integer values are treated as categorical. If float, it's treated as a percentage. If int, it's the maximum number of unique values for a column to be considered categorical. Default is 3%
+    treat_all_integers_as_numerical : bool, optional
+        If True, all integer columns will be treated as numerical, regardless of their unique value count or proportion. Default is False
+
+
+    Attributes
+    ----------
+    config : MambularConfig
+        Configuration object containing model-specific parameters.
+    preprocessor : Preprocessor
+        Preprocessor object for data preprocessing steps.
+    model : BaseEmbeddingMambularRegressor
+        The neural network model, initialized after the `fit` method is called.
+    """
+
+    def __init__(self, **kwargs):
+        # Known config arguments
+        config_arg_names = [
+            "lr",
+            "lr_patience",
+            "weight_decay",
+            "lr_factor",
+            "d_model",
+            "n_layers",
+            "expand_factor",
+            "bias",
+            "d_conv",
+            "conv_bias",
+            "dropout",
+            "dt_rank",
+            "d_state",
+            "dt_scale",
+            "dt_init",
+            "dt_max",
+            "dt_min",
+            "dt_init_floor",
+            "norm",
+            "activation",
+            "num_embedding_activation",
+            "head_layer_sizes",
+            "head_dropout",
+            "head_skip_layers",
+            "head_activation",
+            "head_use_batch_norm",
+        ]
+
+        preprocessor_arg_names = [
+            "n_bins",
+            "numerical_preprocessing",
+            "use_decision_tree_bins",
+            "binning_strategy",
+            "task",
+            "cat_cutoff",
+            "treat_all_integers_as_numerical",
+        ]
+
+        self.config_kwargs = {k: v for k, v in kwargs.items() if k in config_arg_names}
+        self.config = DefaultMambularConfig(**self.config_kwargs)
+
+        preprocessor_kwargs = {
+            k: v for k, v in kwargs.items() if k in preprocessor_arg_names
+        }
+        if "numerical_preprocessing" not in list(preprocessor_kwargs.keys()):
+            preprocessor_kwargs["numerical_preprocessing"] = "standardization"
+
+        # Raise a warning if task is set to 'classification'
+        if preprocessor_kwargs.get("task") == "regression":
+            warnings.warn(
+                "The task is set to 'regression'. This model is designed for classification tasks.",
+                UserWarning,
+            )
+
+        if "task" not in list(preprocessor_kwargs.keys()):
+            preprocessor_kwargs["task"] = "classification"
+
+        self.preprocessor = Preprocessor(**preprocessor_kwargs)
+        self.model = None
+
+    def get_params(self, deep=True):
+        """
+        Get parameters for this estimator.
+
+        Parameters
+        ----------
+        deep : bool, default=True
+            If True, will return the parameters for this estimator and contained subobjects that are estimators.
+
+
+        Returns
+        -------
+        params : dict
+            Parameter names mapped to their values.
+        """
+        params = self.config_kwargs  # Parameters used to initialize MambularConfig
+
+        # If deep=True, include parameters from nested components like preprocessor
+        if deep:
+            # Assuming Preprocessor has a get_params method
+            preprocessor_params = {
+                "preprocessor__" + key: value
+                for key, value in self.preprocessor.get_params().items()
+            }
+            params.update(preprocessor_params)
+
+        return params
+
+    def set_params(self, **parameters):
+        """
+        Set the parameters of this estimator.
+
+        Parameters
+        ----------
+        **parameters : dict
+            Estimator parameters.
+
+
+        Returns
+        -------
+        self : object
+            Estimator instance.
+        """
+        # Update config_kwargs with provided parameters
+        valid_config_keys = self.config_kwargs.keys()
+        config_updates = {k: v for k, v in parameters.items() if k in valid_config_keys}
+        self.config_kwargs.update(config_updates)
+
+        # Update the config object
+        for key, value in config_updates.items():
+            setattr(self.config, key, value)
+
+        # Handle preprocessor parameters (prefixed with 'preprocessor__')
+        preprocessor_params = {
+            k.split("__")[1]: v
+            for k, v in parameters.items()
+            if k.startswith("preprocessor__")
+        }
+        if preprocessor_params:
+            # Assuming Preprocessor has a set_params method
+            self.preprocessor.set_params(**preprocessor_params)
+
+        return self
+
+    def split_data(self, X, y, val_size, random_state):
+        """
+        Split the dataset into training and validation sets.
+
+        Parameters
+        ----------
+        X : array-like of shape (n_samples, n_features)
+            The input samples.
+        y : array-like of shape (n_samples,)
+            The target values.
+        val_size : float
+            The proportion of the dataset to include in the validation split.
+        random_state : int
+            Controls the shuffling applied to the data before applying the split.
+
+
+        Returns
+        -------
+        X_train, X_val, y_train, y_val : arrays
+            The split datasets.
+        """
+        X_train, X_val, y_train, y_val = train_test_split(
+            X, y, test_size=val_size, random_state=random_state
+        )
+
+        return X_train, X_val, y_train, y_val
+
+    def preprocess_data(self, X_train, y_train, X_val, y_val, batch_size, shuffle):
+        """
+        Preprocess the training and validation data and create corresponding DataLoaders.
+
+        Parameters
+        ----------
+        X_train : array-like of shape (n_samples, n_features)
+            The training input samples.
+        y_train : array-like of shape (n_samples,)
+            The training target values.
+        X_val : array-like of shape (n_samples, n_features)
+            The validation input samples.
+        y_val : array-like of shape (n_samples,)
+            The validation target values.
+        batch_size : int
+            Size of mini-batches for the DataLoader.
+        shuffle : bool
+            Whether to shuffle the training data before splitting into batches.
+
+
+        Returns
+        -------
+        data_module : MambularDataModule
+            An instance of MambularDataModule containing training and validation DataLoaders.
+        """
+        self.preprocessor.fit(
+            pd.concat([X_train, X_val], axis=0).reset_index(drop=True),
+            np.concatenate((y_train, y_val), axis=0),
+        )
+        train_preprocessed_data = self.preprocessor.transform(X_train)
+        val_preprocessed_data = self.preprocessor.transform(X_val)
+
+        # Update feature info based on the actual processed data
+        (
+            self.cat_feature_info,
+            self.num_feature_info,
+        ) = self.preprocessor.get_feature_info()
+
+        # Initialize lists for tensors
+        train_cat_tensors = []
+        train_num_tensors = []
+        val_cat_tensors = []
+        val_num_tensors = []
+
+        # Populate tensors for categorical features, if present in processed data
+        for key in self.cat_feature_info:
+            cat_key = "cat_" + key  # Assuming categorical keys are prefixed with 'cat_'
+            if cat_key in train_preprocessed_data:
+                train_cat_tensors.append(
+                    torch.tensor(train_preprocessed_data[cat_key], dtype=torch.long)
+                )
+            if cat_key in val_preprocessed_data:
+                val_cat_tensors.append(
+                    torch.tensor(val_preprocessed_data[cat_key], dtype=torch.long)
+                )
+
+            binned_key = "num_" + key  # for binned features
+            if binned_key in train_preprocessed_data:
+                train_cat_tensors.append(
+                    torch.tensor(train_preprocessed_data[binned_key], dtype=torch.long)
+                )
+
+            if binned_key in val_preprocessed_data:
+                val_cat_tensors.append(
+                    torch.tensor(val_preprocessed_data[binned_key], dtype=torch.long)
+                )
+
+        # Populate tensors for numerical features, if present in processed data
+        for key in self.num_feature_info:
+            num_key = "num_" + str(
+                key
+            )  # Assuming numerical keys are prefixed with 'num_'
+            if num_key in train_preprocessed_data:
+                train_num_tensors.append(
+                    torch.tensor(train_preprocessed_data[num_key], dtype=torch.float32)
+                )
+            if num_key in val_preprocessed_data:
+                val_num_tensors.append(
+                    torch.tensor(val_preprocessed_data[num_key], dtype=torch.float32)
+                )
+
+        train_labels = torch.tensor(y_train, dtype=torch.long)
+        val_labels = torch.tensor(y_val, dtype=torch.long)
+
+        # Create datasets
+        train_dataset = EmbeddingMambularDataset(
+            train_cat_tensors, train_num_tensors, train_labels, regression=False
+        )
+        val_dataset = EmbeddingMambularDataset(
+            val_cat_tensors, val_num_tensors, val_labels, regression=False
+        )
+
+        # Create dataloaders
+        train_dataloader = DataLoader(
+            train_dataset, batch_size=batch_size, shuffle=shuffle
+        )
+        val_dataloader = DataLoader(val_dataset, batch_size=batch_size)
+
+        return MambularDataModule(train_dataloader, val_dataloader)
+
+    def preprocess_test_data(self, X):
+        """
+        Preprocesses the test data and creates tensors for categorical and numerical features.
+
+        Parameters
+        ----------
+        X : DataFrame or array-like, shape (n_samples, n_features)
+            Test feature set.
+
+
+        Returns
+        -------
+        cat_tensors : list of Tensors
+            List of tensors for each categorical feature.
+        num_tensors : list of Tensors
+            List of tensors for each numerical feature.
+        """
+        processed_data = self.preprocessor.transform(X)
+
+        # Initialize lists for tensors
+        cat_tensors = []
+        num_tensors = []
+
+        # Populate tensors for categorical features
+        for key in self.cat_feature_info:
+            cat_key = "cat_" + str(
+                key
+            )  # Assuming categorical keys are prefixed with 'cat_'
+            if cat_key in processed_data:
+                cat_tensors.append(
+                    torch.tensor(processed_data[cat_key], dtype=torch.long)
+                )
+
+            binned_key = "num_" + str(key)  # for binned features
+            if binned_key in processed_data:
+                cat_tensors.append(
+                    torch.tensor(processed_data[binned_key], dtype=torch.long)
+                )
+
+        # Populate tensors for numerical features
+        for key in self.num_feature_info:
+            num_key = "num_" + str(
+                key
+            )  # Assuming numerical keys are prefixed with 'num_'
+            if num_key in processed_data:
+                num_tensors.append(
+                    torch.tensor(processed_data[num_key], dtype=torch.float32)
+                )
+
+        return cat_tensors, num_tensors
+
+    def fit(
+        self,
+        X,
+        y,
+        val_size=0.2,
+        X_val=None,
+        y_val=None,
+        max_epochs=100,
+        random_state=101,
+        batch_size=64,
+        shuffle=True,
+        patience=10,
+        monitor="val_loss",
+        mode="min",
+        lr=1e-3,
+        lr_patience=10,
+        factor=0.75,
+        weight_decay=0.025,
+        raw_embeddings=False,
+        seq_size=20,
+        pca=False,
+        reduced_dims=16,
+        **trainer_kwargs
+    ):
+        """
+        Fits the model to the given dataset.
+
+        Parameters
+        ----------
+        X : pandas DataFrame or array-like
+            Feature matrix for training.
+        y : array-like
+            Target vector.
+        val_size : float, optional
+            Fraction of the data to use for validation if X_val is None.
+        X_val : pandas DataFrame or array-like, optional
+            Feature matrix for validation.
+        y_val : array-like, optional
+            Target vector for validation.
+        max_epochs : int, default=100
+            Maximum number of epochs for training.
+        random_state : int, optional
+            Seed for random number generators.
+        batch_size : int, default=32
+            Size of batches for training and validation.
+        shuffle : bool, default=True
+            Whether to shuffle training data before each epoch.
+        patience : int, default=10
+            Patience for early stopping based on val_loss.
+        monitor : str, default='val_loss'
+            Metric to monitor for early stopping.
+        mode : str, default='min'
+            Mode for early stopping ('min' or 'max').
+        lr : float, default=0.001
+            Learning rate for the optimizer.
+        lr_patience : int, default=5
+            Patience for learning rate reduction.
+        factor : float, default=0.1
+            Factor for learning rate reduction.
+        weight_decay : float, default=0.0
+            Weight decay for the optimizer.
+        raw_embeddings : bool, default=False
+            Whether to use raw features or embeddings.
+        seq_size : int, optional
+            Sequence size for embeddings, relevant if raw_embeddings is False.
+        **trainer_kwargs : dict
+            Additional arguments for the PyTorch Lightning Trainer.
+
+
+        Returns
+        -------
+        self : object
+            The fitted estimator.
+        """
+        if not isinstance(X, pd.DataFrame):
+            X = pd.DataFrame(X)
+        if X_val:
+            if not isinstance(X_val, pd.DataFrame):
+                X_val = pd.DataFrame(X_val)
+
+        # Apply PCA if indicated
+        if pca:
+            pca_transformer = PCA(n_components=reduced_dims)
+            X = pca_transformer.fit_transform(
+                X
+            )  # Fit and transform the PCA on the complete dataset
+            if X_val is not None:
+                X_val = pca_transformer.transform(
+                    X_val
+                )  # Transform validation data with the same PCA model
+
+            raw_embeddings = True
+
+        if not X_val:
+            X_train, X_val, y_train, y_val = self.split_data(
+                X, y, val_size, random_state
+            )
+        else:
+            X_train = X
+            y_train = y
+
+        data_module = self.preprocess_data(
+            X_train, y_train, X_val, y_val, batch_size, shuffle
+        )
+
+        if raw_embeddings:
+            self.config.d_model = X.shape[1]
+
+        num_classes = len(np.unique(y))
+
+        self.model = BaseEmbeddingMambularClassifier(
+            num_classes=num_classes,
+            config=self.config,
+            cat_feature_info=self.cat_feature_info,
+            num_feature_info=self.num_feature_info,
+            lr=lr,
+            lr_patience=lr_patience,
+            lr_factor=factor,
+            weight_decay=weight_decay,
+            raw_embeddings=raw_embeddings,
+            seq_size=seq_size,
+        )
+
+        early_stop_callback = EarlyStopping(
+            monitor=monitor, min_delta=0.00, patience=patience, verbose=False, mode=mode
+        )
+
+        checkpoint_callback = ModelCheckpoint(
+            monitor="val_loss",  # Adjust according to your validation metric
+            mode="min",
+            save_top_k=1,
+            dirpath="model_checkpoints",  # Specify the directory to save checkpoints
+            filename="best_model",
+        )
+
+        # Initialize the trainer and train the model
+        trainer = pl.Trainer(
+            max_epochs=max_epochs,
+            callbacks=[early_stop_callback, checkpoint_callback],
+            **trainer_kwargs
+        )
+        trainer.fit(self.model, data_module)
+
+        best_model_path = checkpoint_callback.best_model_path
+        if best_model_path:
+            checkpoint = torch.load(best_model_path)
+            self.model.load_state_dict(checkpoint["state_dict"])
+
+        return self
+
+    def predict(self, X):
+        """
+        Predict the class labels for the given input samples.
+
+        Parameters
+        ----------
+        X : array-like or pd.DataFrame of shape (n_samples, n_features)
+            The input samples to predict.
+
+
+        Returns
+        -------
+        predictions : ndarray of shape (n_samples,)
+            Predicted class labels for each input sample.
+
+
+        Notes
+        -----
+        The method preprocesses the input data using the same preprocessor used during training,
+        sets the model to evaluation mode, and then performs inference to predict the class labels.
+        The predictions are converted from a PyTorch tensor to a NumPy array before being returned.
+        """
+        # Preprocess the data
+        if not isinstance(X, pd.DataFrame):
+            X = pd.DataFrame(X)
+
+        if hasattr(self, "pca_transformer"):
+            X = pd.DataFrame(self.pca_transformer.transform(X))
+
+        cat_tensors, num_tensors = self.preprocess_test_data(X)
+        device = next(self.model.parameters()).device
+        cat_tensors, num_tensors = self.preprocess_test_data(X)
+        if isinstance(cat_tensors, list):
+            cat_tensors = [tensor.to(device) for tensor in cat_tensors]
+        else:
+            cat_tensors = cat_tensors.to(device)
+
+        if isinstance(num_tensors, list):
+            num_tensors = [tensor.to(device) for tensor in num_tensors]
+        else:
+            num_tensors = num_tensors.to(device)
+
+        # Set the model to evaluation mode
+        self.model.eval()
+
+        # Perform inference
+        with torch.no_grad():
+            logits = self.model(num_features=num_tensors, cat_features=cat_tensors)
+
+            # Check the shape of the logits to determine binary or multi-class classification
+            if logits.shape[1] == 1:
+                # Binary classification
+                probabilities = torch.sigmoid(logits)
+                predictions = (probabilities > 0.5).long().squeeze()
+            else:
+                # Multi-class classification
+                probabilities = torch.softmax(logits, dim=1)
+                predictions = torch.argmax(probabilities, dim=1)
+
+        # Convert predictions to NumPy array and return
+        return predictions.cpu().numpy()
+
+    def predict_proba(self, X):
+        """
+        Predict class probabilities for the given input samples.
+
+        Parameters
+        ----------
+        X : array-like or pd.DataFrame of shape (n_samples, n_features)
+            The input samples for which to predict class probabilities.
+
+
+        Returns
+        -------
+        probabilities : ndarray of shape (n_samples, n_classes)
+            Predicted class probabilities for each input sample.
+
+
+        Notes
+        -----
+        The method preprocesses the input data using the same preprocessor used during training,
+        sets the model to evaluation mode, and then performs inference to predict the class probabilities.
+        Softmax is applied to the logits to obtain probabilities, which are then converted from a PyTorch tensor
+        to a NumPy array before being returned.
+        """
+        # Preprocess the data
+        if not isinstance(X, pd.DataFrame):
+            X = pd.DataFrame(X)
+        cat_tensors, num_tensors = self.preprocess_test_data(X)
+        device = next(self.model.parameters()).device
+        cat_tensors, num_tensors = self.preprocess_test_data(X)
+        if isinstance(cat_tensors, list):
+            cat_tensors = [tensor.to(device) for tensor in cat_tensors]
+        else:
+            cat_tensors = cat_tensors.to(device)
+
+        if isinstance(num_tensors, list):
+            num_tensors = [tensor.to(device) for tensor in num_tensors]
+        else:
+            num_tensors = num_tensors.to(device)
+
+        # Set the model to evaluation mode
+        self.model.eval()
+
+        # Perform inference
+        with torch.no_grad():
+            logits = self.model(num_features=num_tensors, cat_features=cat_tensors)
+            if logits.shape[1] > 1:
+                probabilities = torch.softmax(logits, dim=1)
+            else:
+                probabilities = torch.sigmoid(logits)
+
+        # Convert probabilities to NumPy array and return
+        return probabilities.cpu().numpy()
+
+    def evaluate(self, X, y_true, metrics=None):
+        """
+        Evaluate the model on the given data using specified metrics.
+
+        Parameters
+        ----------
+        X : array-like or pd.DataFrame of shape (n_samples, n_features)
+            The input samples to predict.
+        y_true : array-like of shape (n_samples,)
+            The true class labels against which to evaluate the predictions.
+        metrics : dict
+            A dictionary where keys are metric names and values are tuples containing the metric function
+            and a boolean indicating whether the metric requires probability scores (True) or class labels (False).
+
+
+        Returns
+        -------
+        scores : dict
+            A dictionary with metric names as keys and their corresponding scores as values.
+
+
+        Notes
+        -----
+        This method uses either the `predict` or `predict_proba` method depending on the metric requirements.
+        """
+        # Ensure input is in the correct format
+        if metrics is None:
+            metrics = {"Accuracy": (accuracy_score, False)}
+
+        if not isinstance(X, pd.DataFrame):
+            X = pd.DataFrame(X)
+
+        # Initialize dictionary to store results
+        scores = {}
+
+        # Generate class probabilities if any metric requires them
+        if any(use_proba for _, use_proba in metrics.values()):
+            probabilities = self.predict_proba(X)
+
+        # Generate class labels if any metric requires them
+        if any(not use_proba for _, use_proba in metrics.values()):
+            predictions = self.predict(X)
+
+        # Compute each metric
+        for metric_name, (metric_func, use_proba) in metrics.items():
+            if use_proba:
+                scores[metric_name] = metric_func(y_true, probabilities)
+            else:
+                scores[metric_name] = metric_func(y_true, predictions)
+
+        return scores
```

### Comparing `mambular-0.1.2/mambular/utils/distributional_metrics.py` & `mambular-0.1.3/mambular/utils/distributional_metrics.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-import numpy as np
-
-
-def poisson_deviance(y_true, y_pred):
-    # Ensure no zero to avoid log(0)
-    y_pred = np.clip(y_pred, 1e-9, None)
-    return 2 * np.sum(y_true * np.log(y_true / y_pred) - (y_true - y_pred))
-
-
-def gamma_deviance(y_true, y_pred):
-    # Avoid division by zero and log(0)
-    y_pred = np.clip(y_pred, 1e-9, None)
-    y_true = np.clip(y_true, 1e-9, None)
-    return 2 * np.sum(np.log(y_true / y_pred) + (y_true - y_pred) / y_pred)
-
-
-def beta_brier_score(y_true, y_pred):
-    return np.mean((y_pred - y_true) ** 2)
-
-
-def dirichlet_error(y_true, y_pred):
-    # Simple sum of squared differences as an example
-    return np.mean(np.sum((y_pred - y_true) ** 2, axis=1))
-
-
-def student_t_loss(y_true, y_pred, df=2):
-    # Assuming y_pred includes both location and scale
-    mu = y_pred[:, 0]
-    scale = np.clip(y_pred[:, 1], 1e-9, None)  # Avoid zero scale
-    return np.mean((df + 1) * np.log(1 + (y_true - mu) ** 2 / (df * scale)) / scale)
-
-
-def negative_binomial_deviance(y_true, y_pred, alpha):
-    # Here alpha is the overdispersion parameter
-    mu = y_pred
-    return 2 * np.sum(
-        y_true * np.log(y_true / mu + 1e-9)
-        + (y_true + alpha) * np.log((mu + alpha) / (y_true + alpha))
-    )
-
-
-def inverse_gamma_loss(y_true, y_pred):
-    # Assuming y_pred includes both shape and scale
-    shape = y_pred[:, 0]
-    scale = np.clip(y_pred[:, 1], 1e-9, None)  # Avoid zero scale
-    return np.mean(
-        (shape + 1) * np.log(y_true / scale) + np.log(scale**shape / y_true)
-    )
+import numpy as np
+
+
+def poisson_deviance(y_true, y_pred):
+    # Ensure no zero to avoid log(0)
+    y_pred = np.clip(y_pred, 1e-9, None)
+    return 2 * np.sum(y_true * np.log(y_true / y_pred) - (y_true - y_pred))
+
+
+def gamma_deviance(y_true, y_pred):
+    # Avoid division by zero and log(0)
+    y_pred = np.clip(y_pred, 1e-9, None)
+    y_true = np.clip(y_true, 1e-9, None)
+    return 2 * np.sum(np.log(y_true / y_pred) + (y_true - y_pred) / y_pred)
+
+
+def beta_brier_score(y_true, y_pred):
+    return np.mean((y_pred - y_true) ** 2)
+
+
+def dirichlet_error(y_true, y_pred):
+    # Simple sum of squared differences as an example
+    return np.mean(np.sum((y_pred - y_true) ** 2, axis=1))
+
+
+def student_t_loss(y_true, y_pred, df=2):
+    # Assuming y_pred includes both location and scale
+    mu = y_pred[:, 0]
+    scale = np.clip(y_pred[:, 1], 1e-9, None)  # Avoid zero scale
+    return np.mean((df + 1) * np.log(1 + (y_true - mu) ** 2 / (df * scale)) / scale)
+
+
+def negative_binomial_deviance(y_true, y_pred, alpha):
+    # Here alpha is the overdispersion parameter
+    mu = y_pred
+    return 2 * np.sum(
+        y_true * np.log(y_true / mu + 1e-9)
+        + (y_true + alpha) * np.log((mu + alpha) / (y_true + alpha))
+    )
+
+
+def inverse_gamma_loss(y_true, y_pred):
+    # Assuming y_pred includes both shape and scale
+    shape = y_pred[:, 0]
+    scale = np.clip(y_pred[:, 1], 1e-9, None)  # Avoid zero scale
+    return np.mean(
+        (shape + 1) * np.log(y_true / scale) + np.log(scale**shape / y_true)
+    )
```

### Comparing `mambular-0.1.2/mambular/utils/distributions.py` & `mambular-0.1.3/mambular/utils/distributions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import torch
 import torch.distributions as dist
 import numpy as np
 
 
-class BaseDistribution:
+class BaseDistribution(torch.nn.Module):
     """
     The base class for various statistical distributions, providing a common interface and utilities.
 
     This class defines the basic structure and methods that are inherited by specific distribution
     classes, allowing for the implementation of custom distributions with specific parameter transformations
     and loss computations.
 
@@ -19,14 +19,16 @@
 
     Parameters:
         name (str): The name of the distribution.
         param_names (list of str): A list of names for the parameters of the distribution.
     """
 
     def __init__(self, name, param_names):
+        super(BaseDistribution, self).__init__()
+
         self._name = name
         self.param_names = param_names
         self.param_count = len(param_names)
         # Predefined transformation functions accessible to all subclasses
         self.predefined_transforms = {
             "positive": torch.nn.functional.softplus,
             "none": lambda x: x,
@@ -93,14 +95,32 @@
         nll_loss_tensor = self.compute_loss(y_pred_tensor, y_true_tensor)
 
         # Convert the NLL loss tensor back to a numpy array and return
         return {
             "NLL": nll_loss_tensor.detach().numpy(),
         }
 
+    def forward(self, predictions):
+        """
+        Apply the appropriate transformations to the predicted parameters.
+
+        Parameters:
+            predictions (torch.Tensor): The predicted parameters of the distribution.
+
+        Returns:
+            torch.Tensor: A tensor with transformed parameters.
+        """
+        transformed_params = []
+        for idx, param_name in enumerate(self.param_names):
+            transform_func = self.get_transform(
+                getattr(self, f"{param_name}_transform", "none")
+            )
+            transformed_params.append(transform_func(predictions[:, idx]).unsqueeze(1))
+        return torch.cat(transformed_params, dim=1)
+
 
 class NormalDistribution(BaseDistribution):
     """
     Represents a Normal (Gaussian) distribution with parameters for mean and variance, including functionality
     for transforming these parameters and computing the loss.
 
     Inherits from BaseDistribution.
@@ -115,19 +135,19 @@
         param_names = [
             "mean",
             "variance",
         ]
         super().__init__(name, param_names)
 
         self.mean_transform = self.get_transform(mean_transform)
-        self.var_transform = self.get_transform(var_transform)
+        self.variance_transform = self.get_transform(var_transform)
 
     def compute_loss(self, predictions, y_true):
         mean = self.mean_transform(predictions[:, self.param_names.index("mean")])
-        variance = self.var_transform(
+        variance = self.variance_transform(
             predictions[:, self.param_names.index("variance")]
         )
 
         normal_dist = dist.Normal(mean, variance)
 
         nll = -normal_dist.log_prob(y_true).mean()
         return nll
```

### Comparing `mambular-0.1.2/mambular/utils/normalization_layers.py` & `mambular-0.1.3/mambular/utils/normalization_layers.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
         d_model (int): The dimensionality of the input and output tensors.
         eps (float): Small value to avoid division by zero.
         weight (nn.Parameter): Learnable parameter for scaling.
     """
 
     def __init__(self, d_model: int, eps: float = 1e-5):
         super().__init__()
-
         self.eps = eps
         self.weight = nn.Parameter(torch.ones(d_model))
 
     def forward(self, x):
         output = (
             x * torch.rsqrt(x.pow(2).mean(-1, keepdim=True) + self.eps) * self.weight
         )
```

### Comparing `mambular-0.1.2/mambular/utils/preprocessor.py` & `mambular-0.1.3/mambular/utils/preprocessor.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,275 +1,168 @@
-import pandas as pd
 import numpy as np
-from sklearn.base import TransformerMixin, BaseEstimator
-from sklearn.preprocessing import (
-    StandardScaler,
-    KBinsDiscretizer,
-    MinMaxScaler,
-)
-from sklearn.tree import DecisionTreeRegressor, DecisionTreeClassifier
+import pandas as pd
 from sklearn.compose import ColumnTransformer
-from sklearn.pipeline import Pipeline
-from sklearn.impute import SimpleImputer
 from sklearn.exceptions import NotFittedError
+from sklearn.impute import SimpleImputer
+from sklearn.pipeline import Pipeline
+from sklearn.preprocessing import KBinsDiscretizer, MinMaxScaler, StandardScaler
+from sklearn.tree import DecisionTreeClassifier, DecisionTreeRegressor
 
-
-class CustomBinner(TransformerMixin):
-    def __init__(self, bins):
-        # bins can be a scalar (number of bins) or array-like (bin edges)
-        self.bins = bins
-
-    def fit(self, X, y=None):
-        # Fit doesn't need to do anything as we are directly using provided bins
-        return self
-
-    def transform(self, X):
-        if isinstance(self.bins, int):
-            # Calculate equal width bins based on the range of the data and number of bins
-            _, bins = pd.cut(X.squeeze(), bins=self.bins, retbins=True)
-        else:
-            # Use predefined bins
-            bins = self.bins
-
-        # Apply the bins to the data
-        binned_data = pd.cut(
-            X.squeeze(),
-            bins=np.sort(np.unique(bins)),
-            labels=False,
-            include_lowest=True,
-        )
-        print(binned_data)
-        return np.expand_dims(np.array(binned_data), 1)
-
-
-class ContinuousOrdinalEncoder(BaseEstimator, TransformerMixin):
-    """
-    This encoder converts categorical features into continuous integer values. Each unique category within a feature
-    is assigned a unique integer based on its order of appearance in the dataset. This transformation is useful for
-    models that can only handle continuous data.
-
-    Attributes:
-        mapping_ (list of dicts): A list where each element is a dictionary mapping original categories to integers
-                                  for a single feature.
-
-    Methods:
-        fit(X, y=None): Learns the mapping from original categories to integers.
-        transform(X): Applies the learned mapping to the data.
-        get_feature_names_out(input_features=None): Returns the input features after transformation.
-    """
-
-    def fit(self, X, y=None):
-        """
-        Learns the mapping from original categories to integers for each feature.
-
-        Parameters:
-            X (array-like of shape (n_samples, n_features)): The input data to fit.
-            y (ignored): Not used, present for API consistency by convention.
-
-        Returns:
-            self: Returns the instance itself.
-        """
-        # Fit should determine the mapping from original categories to sequential integers starting from 0
-        self.mapping_ = [
-            {category: i for i, category in enumerate(np.unique(col))} for col in X.T
-        ]
-        return self
-
-    def transform(self, X):
-        """
-        Transforms the categories in X to their corresponding integer values based on the learned mapping.
-
-        Parameters:
-            X (array-like of shape (n_samples, n_features)): The input data to transform.
-
-        Returns:
-            X_transformed (ndarray of shape (n_samples, n_features)): The transformed data with integer values.
-        """
-        # Transform the categories to their mapped integer values
-        X_transformed = np.array(
-            [
-                [self.mapping_[col].get(value, -1) for col, value in enumerate(row)]
-                for row in X
-            ]
-        )
-        return X_transformed
-
-    def get_feature_names_out(self, input_features=None):
-        """
-        Returns the names of the transformed features.
-
-        Parameters:
-            input_features (list of str): The names of the input features.
-
-        Returns:
-            input_features (array of shape (n_features,)): The names of the output features after transformation.
-        """
-        if input_features is None:
-            raise ValueError("input_features must be specified")
-        return input_features
-
-
-class OneHotFromOrdinal(TransformerMixin, BaseEstimator):
-    """
-    A transformer that takes ordinal-encoded features and converts them into one-hot encoded format. This is useful
-    in scenarios where features have been pre-encoded with ordinal encoding and a one-hot representation is required
-    for model training.
-
-    Attributes:
-        max_bins_ (ndarray of shape (n_features,)): An array containing the maximum bin index for each feature,
-                                                    determining the size of the one-hot encoded array for that feature.
-
-    Methods:
-        fit(X, y=None): Learns the maximum bin index for each feature.
-        transform(X): Converts ordinal-encoded features into one-hot format.
-        get_feature_names_out(input_features=None): Returns the feature names after one-hot encoding.
-    """
-
-    def fit(self, X, y=None):
-        """
-        Learns the maximum bin index for each feature from the data.
-
-        Parameters:
-            X (array-like of shape (n_samples, n_features)): The input data to fit, containing ordinal-encoded features.
-            y (ignored): Not used, present for API consistency by convention.
-
-        Returns:
-            self: Returns the instance itself.
-        """
-        self.max_bins_ = (
-            np.max(X, axis=0).astype(int) + 1
-        )  # Find the maximum bin index for each feature
-        return self
-
-    def transform(self, X):
-        """
-        Transforms ordinal-encoded features into one-hot encoded format based on the `max_bins_` learned during fitting.
-
-        Parameters:
-            X (array-like of shape (n_samples, n_features)): The input data to transform, containing ordinal-encoded features.
-
-        Returns:
-            X_one_hot (ndarray of shape (n_samples, n_output_features)): The one-hot encoded features.
-        """
-        # Initialize an empty list to hold the one-hot encoded arrays
-        one_hot_encoded = []
-        for i, max_bins in enumerate(self.max_bins_):
-            # Convert each feature to one-hot using its max_bins
-            feature_one_hot = np.eye(max_bins)[X[:, i].astype(int)]
-            one_hot_encoded.append(feature_one_hot)
-        # Concatenate the one-hot encoded features horizontally
-        return np.hstack(one_hot_encoded)
-
-    def get_feature_names_out(self, input_features=None):
-        """
-        Generates feature names for the one-hot encoded features based on the input feature names and the number of bins.
-
-        Parameters:
-            input_features (list of str): The names of the input features that were ordinal-encoded.
-
-        Returns:
-            feature_names (array of shape (n_output_features,)): The names of the one-hot encoded features.
-        """
-        feature_names = []
-        for i, max_bins in enumerate(self.max_bins_):
-            feature_names.extend(
-                [f"{input_features[i]}_bin_{j}" for j in range(int(max_bins))]
-            )
-        return np.array(feature_names)
+from .ple_encoding import PLE
+from .prepro_utils import ContinuousOrdinalEncoder, CustomBinner, OneHotFromOrdinal
 
 
 class Preprocessor:
     """
     A comprehensive preprocessor for structured data, capable of handling both numerical and categorical features.
     It supports various preprocessing strategies for numerical data, including binning, one-hot encoding,
     standardization, and normalization. Categorical features can be transformed using continuous ordinal encoding.
     Additionally, it allows for the use of decision tree-derived bin edges for numerical feature binning.
 
     The class is designed to work seamlessly with pandas DataFrames, facilitating easy integration into
     machine learning pipelines.
 
-    Parameters:
+    Parameters
+    ----------
         n_bins (int): The number of bins to use for numerical feature binning. This parameter is relevant
                       only if `numerical_preprocessing` is set to 'binning' or 'one_hot'.
         numerical_preprocessing (str): The preprocessing strategy for numerical features. Valid options are
                                        'binning', 'one_hot', 'standardization', and 'normalization'.
         use_decision_tree_bins (bool): If True, uses decision tree regression/classification to determine
                                        optimal bin edges for numerical feature binning. This parameter is
                                        relevant only if `numerical_preprocessing` is set to 'binning' or 'one_hot'.
+        binning_strategy (str): Defines the strategy for binning numerical features. Options include 'uniform',
+                                'quantile', or other sklearn-compatible strategies.
+        task (str): Indicates the type of machine learning task ('regression' or 'classification'). This can
+                    influence certain preprocessing behaviors, especially when using decision tree-based binning.
+        binning_strategy (str): Defines the strategy for binning numerical features. Options include 'uniform',
+                                'quantile', or other sklearn-compatible strategies.
+        task (str): Indicates the type of machine learning task ('regression' or 'classification'). This can
+                    influence certain preprocessing behaviors, especially when using decision tree-based binning.
+        cat_cutoff (float or int): Indicates the cutoff after which integer values are treated as categorical.
+                                   If float, it's treated as a percentage. If int, it's the maximum number of
+                                   unique values for a column to be considered categorical.
+        treat_all_integers_as_numerical (bool): If True, all integer columns will be treated as numerical, regardless
+                                                of their unique value count or proportion.
+
+
+    Attributes
+    ----------
+        column_transformer (ColumnTransformer): An instance of sklearn's ColumnTransformer that holds the
+                                                configured preprocessing pipelines for different feature types.
+        fitted (bool): Indicates whether the preprocessor has been fitted to the data.
 
-    Attributes:
-        column_transformer (ColumnTransformer): A sklearn ColumnTransformer instance that holds the configured
-                                                preprocessing pipelines for the different feature types.
-
-    Methods:
-        fit(X, y=None): Fits the preprocessor to the data, identifying feature types and configuring the
-                        appropriate transformations.
-        transform(X): Transforms the data using the fitted preprocessing pipelines.
-        fit_transform(X, y=None): Fits the preprocessor to the data and then transforms the data.
-        get_feature_info(): Returns information about the processed features, including the number of bins for
-                            binned features and the dimensionality of encoded features.
     """
 
     def __init__(
         self,
-        n_bins=200,
-        numerical_preprocessing="binning",
+        n_bins=50,
+        numerical_preprocessing="ple",
         use_decision_tree_bins=False,
         binning_strategy="uniform",
+        task="regression",
+        cat_cutoff=0.03,
+        treat_all_integers_as_numerical=False,
     ):
         self.n_bins = n_bins
-        self.numerical_preprocessing = numerical_preprocessing
+        self.numerical_preprocessing = numerical_preprocessing.lower()
+        if self.numerical_preprocessing not in [
+            "ple",
+            "binning",
+            "one_hot",
+            "standardization",
+            "normalization",
+        ]:
+            raise ValueError(
+                "Invalid numerical_preprocessing value. Supported values are 'ple', 'binning', 'one_hot', 'standardization', and 'normalization'."
+            )
+        self.numerical_preprocessing = numerical_preprocessing.lower()
+        if self.numerical_preprocessing not in [
+            "ple",
+            "binning",
+            "one_hot",
+            "standardization",
+            "normalization",
+        ]:
+            raise ValueError(
+                "Invalid numerical_preprocessing value. Supported values are 'ple', 'binning', 'one_hot', 'standardization', and 'normalization'."
+            )
         self.use_decision_tree_bins = use_decision_tree_bins
         self.column_transformer = None
         self.fitted = False
         self.binning_strategy = binning_strategy
+        self.task = task
+        self.cat_cutoff = cat_cutoff
+        self.treat_all_integers_as_numerical = treat_all_integers_as_numerical
 
     def set_params(self, **params):
         for key, value in params.items():
             setattr(self, key, value)
         return self
 
     def _detect_column_types(self, X):
         """
         Identifies and separates the features in the dataset into numerical and categorical types based on the data type
         and the proportion of unique values.
 
-        Parameters:
+        Parameters
+        ----------
             X (DataFrame or dict): The input dataset, where the features are columns in a DataFrame or keys in a dict.
 
-        Returns:
+
+        Returns
+        -------
             tuple: A tuple containing two lists, the first with the names of numerical features and the second with the names of categorical features.
         """
         categorical_features = []
         numerical_features = []
 
         if isinstance(X, dict):
             X = pd.DataFrame(X)
 
         for col in X.columns:
             num_unique_values = X[col].nunique()
             total_samples = len(X[col])
-            if X[col].dtype.kind not in "iufc" or (
-                X[col].dtype.kind == "i" and (num_unique_values / total_samples) < 0.05
-            ):
-                categorical_features.append(col)
-            else:
+
+            if self.treat_all_integers_as_numerical and X[col].dtype.kind == "i":
                 numerical_features.append(col)
+            else:
+                if isinstance(self.cat_cutoff, float):
+                    cutoff_condition = (
+                        num_unique_values / total_samples
+                    ) < self.cat_cutoff
+                elif isinstance(self.cat_cutoff, int):
+                    cutoff_condition = num_unique_values < self.cat_cutoff
+                else:
+                    raise ValueError(
+                        "cat_cutoff should be either a float or an integer."
+                    )
+
+                if X[col].dtype.kind not in "iufc" or (
+                    X[col].dtype.kind == "i" and cutoff_condition
+                ):
+                    categorical_features.append(col)
+                else:
+                    numerical_features.append(col)
+
         return numerical_features, categorical_features
 
     def fit(self, X, y=None):
         """
         Fits the preprocessor to the data by identifying feature types and configuring the appropriate transformations for each feature.
         It sets up a column transformer with a pipeline of transformations for numerical and categorical features based on the specified preprocessing strategy.
 
-        Parameters:
+        Parameters
+        ----------
             X (DataFrame or dict): The input dataset to fit the preprocessor on.
             y (array-like, optional): The target variable. Required if `use_decision_tree_bins` is True for determining optimal bin edges using decision trees.
 
-        Returns:
+
+        Returns
+        -------
             self: The fitted Preprocessor instance.
         """
         if isinstance(X, dict):
             X = pd.DataFrame(X)
 
         numerical_features, categorical_features = self._detect_column_types(X)
         transformers = []
@@ -321,25 +214,40 @@
 
                 elif self.numerical_preprocessing == "standardization":
                     numeric_transformer_steps.append(("scaler", StandardScaler()))
 
                 elif self.numerical_preprocessing == "normalization":
                     numeric_transformer_steps.append(("normalizer", MinMaxScaler()))
 
+                elif self.numerical_preprocessing == "ple":
+                    numeric_transformer_steps.append(("normalizer", MinMaxScaler()))
+                    numeric_transformer_steps.append(
+                        ("ple", PLE(n_bins=self.n_bins, task=self.task))
+                    )
+
+                elif self.numerical_preprocessing == "ple":
+                    numeric_transformer_steps.append(("normalizer", MinMaxScaler()))
+                    numeric_transformer_steps.append(
+                        ("ple", PLE(n_bins=self.n_bins, task=self.task))
+                    )
+
                 numeric_transformer = Pipeline(numeric_transformer_steps)
 
                 transformers.append((f"num_{feature}", numeric_transformer, [feature]))
 
         if categorical_features:
             for feature in categorical_features:
                 # Create a pipeline for each categorical feature
                 categorical_transformer = Pipeline(
                     [
                         ("imputer", SimpleImputer(strategy="most_frequent")),
-                        ("continuous_ordinal", ContinuousOrdinalEncoder()),
+                        (
+                            "continuous_ordinal",
+                            ContinuousOrdinalEncoder(),
+                        ),
                     ]
                 )
                 # Append the transformer for the current categorical feature
                 transformers.append(
                     (f"cat_{feature}", categorical_transformer, [feature])
                 )
 
@@ -350,20 +258,23 @@
 
         self.fitted = True
 
     def _get_decision_tree_bins(self, X, y, numerical_features):
         """
         Uses decision tree models to determine optimal bin edges for numerical feature binning. This method is used when `use_decision_tree_bins` is True.
 
-        Parameters:
+        Parameters
+        ----------
             X (DataFrame): The input dataset containing only the numerical features for which the bin edges are to be determined.
             y (array-like): The target variable for training the decision tree models.
             numerical_features (list of str): The names of the numerical features for which the bin edges are to be determined.
 
-        Returns:
+
+        Returns
+        -------
             list: A list of arrays, where each array contains the bin edges determined by the decision tree for a numerical feature.
         """
         bins = []
         for feature in numerical_features:
             tree_model = (
                 DecisionTreeClassifier(max_depth=3)
                 if y.dtype.kind in "bi"
@@ -376,87 +287,122 @@
             bins.append(
                 np.concatenate(([X[feature].min()], bin_edges, [X[feature].max()]))
             )
         return bins
 
     def transform(self, X):
         """
-        Transforms the dataset using the fitted preprocessing pipelines. This method applies the transformations set up during the fitting process
-        to the input data and returns a dictionary with the transformed data.
+        Transforms the input data using the preconfigured column transformer and converts the output into a dictionary
+        format with keys corresponding to transformed feature names and values as arrays of transformed data.
 
-        Parameters:
-            X (DataFrame or dict): The input dataset to be transformed.
-
-        Returns:
-            dict: A dictionary where keys are the base feature names and values are the transformed features as arrays.
+        This method converts the sparse or dense matrix returned by the column transformer into a more accessible
+        dictionary format, where each key-value pair represents a feature and its transformed data.
+        Transforms the input data using the preconfigured column transformer and converts the output into a dictionary
+        format with keys corresponding to transformed feature names and values as arrays of transformed data.
+
+        This method converts the sparse or dense matrix returned by the column transformer into a more accessible
+        dictionary format, where each key-value pair represents a feature and its transformed data.
+
+        Parameters
+        ----------
+            X (DataFrame): The input data to be transformed.
+            X (DataFrame): The input data to be transformed.
+
+
+        Returns
+        -------
+            dict: A dictionary where keys are the names of the features (as per the transformations defined in the
+            column transformer) and the values are numpy arrays of the transformed data.
         """
         if not self.fitted:
             raise NotFittedError(
-                "This Preprocessor instance is not fitted yet. Call 'fit' with appropriate arguments before using this method."
+                "The preprocessor must be fitted before transforming new data. Use .fit or .fit_transform"
             )
+        transformed_X = self.column_transformer.transform(X)
 
-        if isinstance(X, dict):
-            X = pd.DataFrame(X)
+        # Now let's convert this into a dictionary of arrays, one per column
+        transformed_dict = self._split_transformed_output(X, transformed_X)
+        return transformed_dict
 
-        # Transform X using the column transformer
-        transformed_X = self.column_transformer.transform(
-            X
-        )  # To understand the shape of the transformed data
+    def _split_transformed_output(self, X, transformed_X):
+        """
+        Splits the transformed data array into a dictionary where keys correspond to the original column names or
+        feature groups and values are the transformed data for those columns.
 
-        # Initialize the transformed dictionary
-        transformed_dict = {}
+        This helper method is utilized within `transform` to segregate the transformed data based on the
+        specification in the column transformer, assigning each transformed section to its corresponding feature name.
 
-        # Retrieve output feature names from the column transformer
-        output_features = self.column_transformer.get_feature_names_out()
+        Parameters
+        ----------
+            X (DataFrame): The original input data, used for determining shapes and transformations.
+            transformed_X (numpy array): The transformed data as a numpy array, outputted by the column transformer.
 
-        # Iterate over each output feature name to populate the transformed_dict
-        for i, col in enumerate(output_features):
-            # Extract the base feature name (before any transformation)
-            base_feature = col.split("__")[0]
-
-            # If the base feature name already exists in the dictionary, append the new data
-            if base_feature in transformed_dict:
-                transformed_dict[base_feature] = np.vstack(
-                    [transformed_dict[base_feature], transformed_X[:, i]]
-                )
-            else:
-                # Otherwise, create a new entry in the dictionary
-                transformed_dict[base_feature] = transformed_X[:, i]
 
-        # Ensure all arrays in the dictionary are the correct shape
-        for key in transformed_dict.keys():
-            transformed_dict[key] = (
-                transformed_dict[key].reshape(-1, transformed_X.shape[0]).T
-            )
+        Returns
+        -------
+            dict: A dictionary mapping each transformation's name to its respective numpy array of transformed data.
+            The type of each array (int or float) is determined based on the type of transformation applied.
+        """
+        start = 0
+        transformed_dict = {}
+        for (
+            name,
+            transformer,
+            columns,
+        ) in self.column_transformer.transformers_:
+            if transformer != "drop":
+                end = start + transformer.transform(X[[columns[0]]]).shape[1]
+                dtype = int if "cat" in name else float
+                transformed_dict[name] = transformed_X[:, start:end].astype(dtype)
+                start = end
 
         return transformed_dict
 
     def fit_transform(self, X, y=None):
         """
         Fits the preprocessor to the data and then transforms the data using the fitted preprocessing pipelines. This is a convenience method that combines `fit` and `transform`.
 
-        Parameters:
+        Parameters
+        ----------
             X (DataFrame or dict): The input dataset to fit the preprocessor on and then transform.
             y (array-like, optional): The target variable. Required if `use_decision_tree_bins` is True.
 
-        Returns:
+
+        Returns
+        -------
             dict: A dictionary with the transformed data, where keys are the base feature names and values are the transformed features as arrays.
         """
         self.fit(X, y)
         self.fitted = True
         return self.transform(X)
 
     def get_feature_info(self):
         """
-        Returns detailed information about the processed features, including the number of bins for binned features
-        and the dimensionality of encoded features. This method is useful for understanding the transformations applied to each feature.
+        Retrieves information about how features are encoded within the model's preprocessor.
+        This method identifies the type of encoding applied to each feature, categorizing them into binned or ordinal
+        encodings and other types of encodings (e.g., one-hot encoding after discretization).
+
+        This method should only be called after the preprocessor has been fitted, as it relies on the structure and
+        configuration of the `column_transformer` attribute.
+
+
+        Raises
+        ------
+            RuntimeError: If the `column_transformer` is not yet fitted, indicating that the preprocessor must be
+            fitted before invoking this method.
+
+
+        Returns
+        -------
+            tuple of (dict, dict):
+                - The first dictionary maps feature names to their respective number of bins or categories if they are
+                  processed using discretization or ordinal encoding.
+                - The second dictionary includes feature names with other encoding details, such as the dimension of
+                  features after encoding transformations (e.g., one-hot encoding dimensions).
 
-        Returns:
-            tuple: A tuple containing two dictionaries, the first with information about binned or ordinal encoded features and
-                   the second with information about other encoded features.
         """
         binned_or_ordinal_info = {}
         other_encoding_info = {}
 
         if not self.column_transformer:
             raise RuntimeError("The preprocessor has not been fitted yet.")
 
@@ -503,13 +449,14 @@
                     last_step = transformer_pipeline.steps[-1][1]
                     if hasattr(last_step, "transform"):
                         transformed_feature = last_step.transform(
                             np.zeros((1, len(columns)))
                         )
                         other_encoding_info[feature_name] = transformed_feature.shape[1]
                         print(
-                            f"Feature: {feature_name} ({self.numerical_preprocessing}), Encoded feature dimension: {transformed_feature.shape[1]}"
+                            f"Feature: {feature_name} (Other Encoding), Encoded feature dimension: {transformed_feature.shape[1]}"
+                            f"Feature: {feature_name} (Other Encoding), Encoded feature dimension: {transformed_feature.shape[1]}"
                         )
 
                 print("-" * 50)
 
         return binned_or_ordinal_info, other_encoding_info
```

