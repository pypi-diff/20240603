# Comparing `tmp/scores-0.8.3.tar.gz` & `tmp/scores-0.8.4.tar.gz`

## Comparing `scores-0.8.3.tar` & `scores-0.8.4.tar`

### file list

```diff
@@ -1,52 +1,51 @@
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 scores-0.8.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0     5484 2020-02-02 00:00:00.000000 scores-0.8.3/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 scores-0.8.3/environment.yml
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 scores-0.8.3/mkdocs.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scores-0.8.3/py.typed
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 scores-0.8.3/readthedocs.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scores-0.8.3/setup.cfg
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 scores-0.8.3/.binder/postBuild
--rw-r--r--   0        0        0     7409 2020-02-02 00:00:00.000000 scores-0.8.3/.binder/requirements.txt
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 scores-0.8.3/.github/pull_request_template.md
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 scores-0.8.3/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 scores-0.8.3/.github/ISSUE_TEMPLATE/new_score.md
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 scores-0.8.3/.github/workflows/python-app.yml
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 scores-0.8.3/.github/workflows/run-pre-commit.yml
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 scores-0.8.3/src/scores/__init__.py
--rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 scores-0.8.3/src/scores/functions.py
--rw-r--r--   0        0        0     4521 2020-02-02 00:00:00.000000 scores-0.8.3/src/scores/sample_data.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 scores-0.8.3/src/scores/typing.py
--rw-r--r--   0        0        0    12725 2020-02-02 00:00:00.000000 scores-0.8.3/src/scores/utils.py
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 scores-0.8.3/src/scores/categorical/__init__.py
--rw-r--r--   0        0        0     6646 2020-02-02 00:00:00.000000 scores-0.8.3/src/scores/categorical/binary_impl.py
--rw-r--r--   0        0        0    21558 2020-02-02 00:00:00.000000 scores-0.8.3/src/scores/categorical/contingency_impl.py
--rw-r--r--   0        0        0    11009 2020-02-02 00:00:00.000000 scores-0.8.3/src/scores/categorical/multicategorical_impl.py
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 scores-0.8.3/src/scores/continuous/__init__.py
--rw-r--r--   0        0        0    18015 2020-02-02 00:00:00.000000 scores-0.8.3/src/scores/continuous/flip_flop_impl.py
--rw-r--r--   0        0        0    12571 2020-02-02 00:00:00.000000 scores-0.8.3/src/scores/continuous/murphy_impl.py
--rw-r--r--   0        0        0     4008 2020-02-02 00:00:00.000000 scores-0.8.3/src/scores/continuous/quantile_loss_impl.py
--rw-r--r--   0        0        0    16768 2020-02-02 00:00:00.000000 scores-0.8.3/src/scores/continuous/standard_impl.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 scores-0.8.3/src/scores/emerging/__init__.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 scores-0.8.3/src/scores/pandas/__init__.py
--rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 scores-0.8.3/src/scores/pandas/continuous.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 scores-0.8.3/src/scores/pandas/typing.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 scores-0.8.3/src/scores/probability/__init__.py
--rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 scores-0.8.3/src/scores/probability/brier_impl.py
--rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 scores-0.8.3/src/scores/probability/checks.py
--rw-r--r--   0        0        0    37967 2020-02-02 00:00:00.000000 scores-0.8.3/src/scores/probability/crps_impl.py
--rw-r--r--   0        0        0     6092 2020-02-02 00:00:00.000000 scores-0.8.3/src/scores/probability/roc_impl.py
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 scores-0.8.3/src/scores/processing/__init__.py
--rw-r--r--   0        0        0    12438 2020-02-02 00:00:00.000000 scores-0.8.3/src/scores/processing/discretise.py
--rw-r--r--   0        0        0    29482 2020-02-02 00:00:00.000000 scores-0.8.3/src/scores/processing/isoreg_impl.py
--rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 scores-0.8.3/src/scores/processing/matching.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 scores-0.8.3/src/scores/processing/cdf/__init__.py
--rw-r--r--   0        0        0    16430 2020-02-02 00:00:00.000000 scores-0.8.3/src/scores/processing/cdf/cdf_functions.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 scores-0.8.3/src/scores/stats/__init__.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 scores-0.8.3/src/scores/stats/statistical_tests/__init__.py
--rw-r--r--   0        0        0     4145 2020-02-02 00:00:00.000000 scores-0.8.3/src/scores/stats/statistical_tests/acovf.py
--rw-r--r--   0        0        0    17540 2020-02-02 00:00:00.000000 scores-0.8.3/src/scores/stats/statistical_tests/diebold_mariano_impl.py
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 scores-0.8.3/.gitignore
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 scores-0.8.3/LICENSE
--rw-r--r--   0        0        0     6381 2020-02-02 00:00:00.000000 scores-0.8.3/README.md
--rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 scores-0.8.3/pyproject.toml
--rw-r--r--   0        0        0     9187 2020-02-02 00:00:00.000000 scores-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 scores-0.8.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     5484 2020-02-02 00:00:00.000000 scores-0.8.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 scores-0.8.4/environment.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scores-0.8.4/py.typed
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 scores-0.8.4/readthedocs.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scores-0.8.4/setup.cfg
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 scores-0.8.4/.binder/postBuild
+-rw-r--r--   0        0        0     7409 2020-02-02 00:00:00.000000 scores-0.8.4/.binder/requirements.txt
+-rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 scores-0.8.4/.github/pull_request_template.md
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 scores-0.8.4/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 scores-0.8.4/.github/ISSUE_TEMPLATE/new_score.md
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 scores-0.8.4/.github/workflows/python-app.yml
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 scores-0.8.4/.github/workflows/run-pre-commit.yml
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 scores-0.8.4/src/scores/__init__.py
+-rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 scores-0.8.4/src/scores/functions.py
+-rw-r--r--   0        0        0     4521 2020-02-02 00:00:00.000000 scores-0.8.4/src/scores/sample_data.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 scores-0.8.4/src/scores/typing.py
+-rw-r--r--   0        0        0    12725 2020-02-02 00:00:00.000000 scores-0.8.4/src/scores/utils.py
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 scores-0.8.4/src/scores/categorical/__init__.py
+-rw-r--r--   0        0        0     6646 2020-02-02 00:00:00.000000 scores-0.8.4/src/scores/categorical/binary_impl.py
+-rw-r--r--   0        0        0    32483 2020-02-02 00:00:00.000000 scores-0.8.4/src/scores/categorical/contingency_impl.py
+-rw-r--r--   0        0        0    11009 2020-02-02 00:00:00.000000 scores-0.8.4/src/scores/categorical/multicategorical_impl.py
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 scores-0.8.4/src/scores/continuous/__init__.py
+-rw-r--r--   0        0        0    18015 2020-02-02 00:00:00.000000 scores-0.8.4/src/scores/continuous/flip_flop_impl.py
+-rw-r--r--   0        0        0    12571 2020-02-02 00:00:00.000000 scores-0.8.4/src/scores/continuous/murphy_impl.py
+-rw-r--r--   0        0        0     4008 2020-02-02 00:00:00.000000 scores-0.8.4/src/scores/continuous/quantile_loss_impl.py
+-rw-r--r--   0        0        0    16768 2020-02-02 00:00:00.000000 scores-0.8.4/src/scores/continuous/standard_impl.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 scores-0.8.4/src/scores/emerging/__init__.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 scores-0.8.4/src/scores/pandas/__init__.py
+-rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 scores-0.8.4/src/scores/pandas/continuous.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 scores-0.8.4/src/scores/pandas/typing.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 scores-0.8.4/src/scores/probability/__init__.py
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 scores-0.8.4/src/scores/probability/brier_impl.py
+-rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 scores-0.8.4/src/scores/probability/checks.py
+-rw-r--r--   0        0        0    37967 2020-02-02 00:00:00.000000 scores-0.8.4/src/scores/probability/crps_impl.py
+-rw-r--r--   0        0        0     6092 2020-02-02 00:00:00.000000 scores-0.8.4/src/scores/probability/roc_impl.py
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 scores-0.8.4/src/scores/processing/__init__.py
+-rw-r--r--   0        0        0    12338 2020-02-02 00:00:00.000000 scores-0.8.4/src/scores/processing/discretise.py
+-rw-r--r--   0        0        0    29482 2020-02-02 00:00:00.000000 scores-0.8.4/src/scores/processing/isoreg_impl.py
+-rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 scores-0.8.4/src/scores/processing/matching.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 scores-0.8.4/src/scores/processing/cdf/__init__.py
+-rw-r--r--   0        0        0    16430 2020-02-02 00:00:00.000000 scores-0.8.4/src/scores/processing/cdf/cdf_functions.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 scores-0.8.4/src/scores/stats/__init__.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 scores-0.8.4/src/scores/stats/statistical_tests/__init__.py
+-rw-r--r--   0        0        0     4145 2020-02-02 00:00:00.000000 scores-0.8.4/src/scores/stats/statistical_tests/acovf.py
+-rw-r--r--   0        0        0    17540 2020-02-02 00:00:00.000000 scores-0.8.4/src/scores/stats/statistical_tests/diebold_mariano_impl.py
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 scores-0.8.4/.gitignore
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 scores-0.8.4/LICENSE
+-rw-r--r--   0        0        0     6508 2020-02-02 00:00:00.000000 scores-0.8.4/README.md
+-rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 scores-0.8.4/pyproject.toml
+-rw-r--r--   0        0        0     9314 2020-02-02 00:00:00.000000 scores-0.8.4/PKG-INFO
```

### Comparing `scores-0.8.3/.pre-commit-config.yaml` & `scores-0.8.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `scores-0.8.3/CODE_OF_CONDUCT.md` & `scores-0.8.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `scores-0.8.3/readthedocs.yaml` & `scores-0.8.4/readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `scores-0.8.3/.binder/requirements.txt` & `scores-0.8.4/.binder/requirements.txt`

 * *Files 0% similar despite different names*

```diff
@@ -277,15 +277,15 @@
     #   rioxarray
     #   scores (pyproject.toml)
 referencing==0.34.0
     # via
     #   jsonschema
     #   jsonschema-specifications
     #   jupyter-events
-requests==2.31.0
+requests==2.32.2
     # via jupyterlab-server
 rfc3339-validator==0.1.4
     # via
     #   jsonschema
     #   jupyter-events
 rfc3986-validator==0.1.1
     # via
```

### Comparing `scores-0.8.3/.github/pull_request_template.md` & `scores-0.8.4/.github/pull_request_template.md`

 * *Files 11% similar despite different names*

```diff
@@ -16,13 +16,13 @@
 - [ ] Test that errors are raised as expected
 - [ ] Test that it works with both `xr.Dataarrays` and `xr.Datasets`
 
 ## Tutorial notebook 
 - [ ] Short introduction to why you would use that metric and what it tells you
 - [ ] A link to a reference
 - [ ] A "things to try next" section at the end
-- [ ] Add notebook to [Explanation.ipynb](https://github.com/nci/scores/blob/develop/tutorials/Explanation.ipynb)
+- [ ] Add notebook to [Tutorial_Gallery.ipynb](https://github.com/nci/scores/blob/develop/tutorials/Tutorial_Gallery.ipynb)
 - [ ] Optional - a detailed discussion of how the metric works at the end of the notebook
 
 ## Documentation
 - [ ] Add the score to the [API documentation](https://github.com/nci/scores/blob/develop/docs/api.md)
 - [ ] Add the score to the [included list of metrics and tools](https://github.com/nci/scores/blob/develop/docs/included.md)
```

### Comparing `scores-0.8.3/.github/ISSUE_TEMPLATE/feature_request.md` & `scores-0.8.4/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `scores-0.8.3/.github/ISSUE_TEMPLATE/new_score.md` & `scores-0.8.4/.github/ISSUE_TEMPLATE/new_score.md`

 * *Files identical despite different names*

### Comparing `scores-0.8.3/.github/workflows/python-app.yml` & `scores-0.8.4/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `scores-0.8.3/.github/workflows/run-pre-commit.yml` & `scores-0.8.4/.github/workflows/run-pre-commit.yml`

 * *Files identical despite different names*

### Comparing `scores-0.8.3/src/scores/__init__.py` & `scores-0.8.4/src/scores/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import scores.functions
 import scores.pandas
 import scores.probability
 import scores.processing
 import scores.sample_data
 import scores.stats.statistical_tests  # noqa: F401
 
-__version__ = "0.8.3"
+__version__ = "0.8.4"
 
 __all__ = [
     "scores.categorical",
     "scores.contingency",
     "scores.continuous",
     "scores.functions",
     "scores.pandas",
```

### Comparing `scores-0.8.3/src/scores/functions.py` & `scores-0.8.4/src/scores/functions.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.3/src/scores/sample_data.py` & `scores-0.8.4/src/scores/sample_data.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.3/src/scores/typing.py` & `scores-0.8.4/src/scores/typing.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.3/src/scores/utils.py` & `scores-0.8.4/src/scores/utils.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.3/src/scores/categorical/__init__.py` & `scores-0.8.4/src/scores/categorical/__init__.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.3/src/scores/categorical/binary_impl.py` & `scores-0.8.4/src/scores/categorical/binary_impl.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.3/src/scores/categorical/contingency_impl.py` & `scores-0.8.4/src/scores/categorical/contingency_impl.py`

 * *Files 25% similar despite different names*

```diff
@@ -35,16 +35,16 @@
     """
     A BasicContingencyManager is produced when a BinaryContingencyManager is transformed.
 
     A basic contingency table is built only from the event counts, losing the connection
     to the actual event tables in their full dimensionality.
 
     The event count data is much smaller than the full event tables, particularly when
-    considering very large data sets like NWP data, which could be terabytes to petabytes
-    in size.
+    considering very large data sets like Numerical Weather Prediction (NWP) data, which
+    could be terabytes to petabytes in size.
     """
 
     def __init__(self, counts: dict):
         """
         Compute any arrays required and store the resulting counts.
         """
         for key, arr in counts.items():
@@ -86,208 +86,493 @@
 
     def get_table(self):
         """
         Return the contingency table as an xarray object
         """
         return self.xr_table
 
-    def accuracy(self):
+    def accuracy(self) -> xr.DataArray:
         """
-        The proportion of forecasts which are true
+        Identical to fraction correct.
 
-        https://www.cawcr.gov.au/projects/verification/#ACC
+        Accuracy calculates the proportion of forecasts which are correct.
+
+        Returns:
+            xr.DataArray: A DataArray containing the accuracy score
+
+        .. math::
+            \\text{accuracy} = \\frac{\\text{true positives} + \\text{true negatives}}{\\text{total count}}
+
+        Notes:
+
+            - Range: 0 to 1, where 1 indicates a perfect score.
+            - "True positives" is the same at "hits".
+            - "False negatives" is the same as "misses".
+
+        References:
+            https://www.cawcr.gov.au/projects/verification/#ACC
         """
         count_dictionary = self.counts
         correct_count = count_dictionary["tp_count"] + count_dictionary["tn_count"]
         ratio = correct_count / count_dictionary["total_count"]
         return ratio
 
-    def frequency_bias(self):
+    def fraction_correct(self) -> xr.DataArray:
+        """
+        Identical to accuracy.
+
+        Fraction correct calculates the proportion of forecasts which are correct.
+
+        Returns:
+            xr.DataArray: An xarray object containing the fraction correct.
+
+        .. math::
+            \\text{fraction correct} = \\frac{\\text{true positives} + \\text{true negatives}}{\\text{total count}}
+
+        Notes:
+
+            - Range: 0 to 1, where 1 indicates a perfect score.
+            - "True positives" is the same as "hits".
+            - "False negatives" is the same as "misses".
+
+        References:
+            https://www.cawcr.gov.au/projects/verification/#ACC
+        """
+        return self.accuracy()
+
+    def frequency_bias(self) -> xr.DataArray:
         """
         How did the forecast frequency of "yes" events compare to the observed frequency of "yes" events?
 
-        https://www.cawcr.gov.au/projects/verification/#BIAS
+        Returns:
+            xr.DataAray: An xarray object containing the frequency bias
+
+        .. math::
+            \\text{frequency bias} = \\frac{\\text{true positives} + \\text{false positives}}{\\text{true positives} + \\text{false negatives}}
+
+        Notes:
+
+            - Range: 0 to ∞ (infinity), where 1 indicates a perfect score
+            - "True positives" is the same as "hits"
+            - "False positives" is the same as "false alarms"
+            - "False negatives" is the same as "misses"
+
+        References:
+            https://www.cawcr.gov.au/projects/verification/#BIAS
         """
         # Note - bias_score calls this method
         cd = self.counts
         freq_bias = (cd["tp_count"] + cd["fp_count"]) / (cd["tp_count"] + cd["fn_count"])
 
         return freq_bias
 
-    def bias_score(self):
+    def bias_score(self) -> xr.DataArray:
         """
         How did the forecast frequency of "yes" events compare to the observed frequency of "yes" events?
 
-        https://www.cawcr.gov.au/projects/verification/#BIAS
+        Returns:
+            xr.DataArray: An xarray object containing the bias score
+
+        .. math::
+            \\text{frequency bias} = \\frac{\\text{true positives} + \\text{false positives}}{\\text{true positives} + \\text{false negatives}}
+
+        Notes:
+
+            - Range: 0 to ∞ (infinity), where 1 indicates a perfect score
+            - "True positives" is the same as "hits"
+            - "False positives" is the same as "false alarms"
+            - "False negatives" is the same as "misses"
+
+        References:
+            https://www.cawcr.gov.au/projects/verification/#BIAS
         """
         return self.frequency_bias()
 
-    def hit_rate(self):
+    def hit_rate(self) -> xr.DataArray:
         """
-        What proportion of the observed events where correctly forecast?
         Identical to probability_of_detection
-        Range: 0 to 1.  Perfect score: 1.
 
-        https://www.cawcr.gov.au/projects/verification/#POD
+        Calculates the proportion of the observed events that were correctly forecast.
+
+        Returns:
+            xr.DataArray: An xarray object containing the hit rate
+
+        .. math::
+            \\text{true positives} = \\frac{\\text{true positives}}{\\text{true positives} + \\text{false negatives}}
+
+        Notes:
+
+            - Range: 0 to 1.  Perfect score: 1.
+            - "True positives" is the same as "hits"
+            - "False negatives" is the same as "misses"
+
+        References:
+            https://www.cawcr.gov.au/projects/verification/#POD
         """
         return self.probability_of_detection()
 
-    def probability_of_detection(self):
+    def probability_of_detection(self) -> xr.DataArray:
         """
-        What proportion of the observed events where correctly forecast?
-        Identical to hit_rate
-        Range: 0 to 1.  Perfect score: 1.
+        Identical to hit rate
+
+        Calculates the proportion of the observed events that were correctly forecast.
+
+        Returns:
+            xr.DataArray: An xarray object containing the probability of detection
+
+        .. math::
+            \\text{hit rate} = \\frac{\\text{true positives}}{\\text{true positives} + \\text{false negatives}}
 
-        https://www.cawcr.gov.au/projects/verification/#POD
+        Notes:
+            - Range: 0 to 1.  Perfect score: 1.
+            - "True positives" is the same as "hits"
+            - "False negatives" is the same as "misses"
+
+        References:
+            https://www.cawcr.gov.au/projects/verification/#POD
         """
         # Note - hit_rate and sensitiviy call this function
         cd = self.counts
         pod = cd["tp_count"] / (cd["tp_count"] + cd["fn_count"])
 
         return pod
 
-    def true_positive_rate(self):
+    def true_positive_rate(self) -> xr.DataArray:
         """
-        What proportion of the observed events where correctly forecast?
         Identical to probability_of_detection
-        Range: 0 to 1.  Perfect score: 1.
 
-        https://www.cawcr.gov.au/projects/verification/#POD
+        What proportion of the observed events where correctly forecast?
+
+        Returns:
+            An xarray object containing the true positive rate
+
+        .. math::
+            \\text{true positive rate} = \\frac{\\text{true positives}}{\\text{true positives} + \\text{false negatives}}
+
+        Notes:
+            - Range: 0 to 1.  Perfect score: 1.
+            - "True positives" is the same as "hits"
+            - "False negatives" is the same as "misses"
+
+        References:
+            https://www.cawcr.gov.au/projects/verification/#POD
         """
         return self.probability_of_detection()
 
-    def false_alarm_ratio(self):
+    def false_alarm_ratio(self) -> xr.DataArray:
         """
         What fraction of the predicted "yes" events actually did not occur (i.e.,
         were false alarms)?
-        Range: 0 to 1. Perfect score: 0.
 
-        https://www.cawcr.gov.au/projects/verification/#FAR
+        Returns:
+            xr.DataArray: An xarray object containing the false alarm ratio
+
+        .. math::
+            \\text{false alarm ratio} = \\frac{\\text{false positives}}{\\text{true positives} + \\text{false positives}}
+
+        Notes:
+            - Range: 0 to 1. Perfect score: 0.
+            - Not to be confused with the False Alarm Rate
+            - "False positives" is the same as "false alarms"
+            - "True positives" is the same as "hits"
+
+        References:
+            https://www.cawcr.gov.au/projects/verification/#FAR
         """
         cd = self.counts
         far = cd["fp_count"] / (cd["tp_count"] + cd["fp_count"])
 
         return far
 
-    def false_alarm_rate(self):
+    def false_alarm_rate(self) -> xr.DataArray:
         """
-        What fraction of the non-events were incorrectly predicted?
         Identical to probability_of_false_detection
-        Range: 0 to 1.  Perfect score: 0.
 
-        https://www.cawcr.gov.au/projects/verification/#POFD
+        What fraction of the non-events were incorrectly predicted?
+
+        Returns:
+            xr.DataArray: An xarray object containing the false alarm rate
+
+        .. math::
+            \\text{false alarm rate} = \\frac{\\text{false positives}}{\\text{true negatives} + \\text{false positives}}
+
+        Notes:
+            - Range: 0 to 1.  Perfect score: 0.
+            - Not to be confused with the false alarm ratio
+            - "False positives" is the same as "false alarms"
+            - "True negatives" is the same as "correct negatives"
+
+        References:
+            https://www.cawcr.gov.au/projects/verification/#POFD
         """
         # Note - probability of false detection calls this function
         cd = self.counts
         far = cd["fp_count"] / (cd["tn_count"] + cd["fp_count"])
 
         return far
 
-    def probability_of_false_detection(self):
+    def probability_of_false_detection(self) -> xr.DataArray:
         """
-        What fraction of the non-events were incorrectly predicted?
         Identical to false_alarm_rate
-        Range: 0 to 1.  Perfect score: 0.
 
-        https://www.cawcr.gov.au/projects/verification/#POFD
+        What fraction of the non-events were incorrectly predicted?
+
+        Returns:
+            An xarray object containing the probability of false detection
+
+        .. math::
+            \\text{probability of false detection} = \\frac{\\text{false positives}}{\\text{true negatives} + \\text{false positives}}
+
+        Notes:
+            - Range: 0 to 1.  Perfect score: 0.
+            - "False positives" is the same as "false alarms"
+            - "True negatives" is the same as "correct negatives"
+
+        References:
+            https://www.cawcr.gov.au/projects/verification/#POFD
         """
 
         return self.false_alarm_rate()
 
-    def success_ratio(self):
+    def success_ratio(self) -> xr.DataArray:
         """
         What proportion of the forecast events actually eventuated?
-        Range: 0 to 1.  Perfect score: 1.
 
-        https://www.cawcr.gov.au/projects/verification/#SR
+        Returns:
+            An xarray object containing the success ratio
+
+        .. math::
+            \\text{success ratio} = \\frac{\\text{true positives}}{\\text{true positives} + \\text{false positives}}
+
+        Notes:
+            - Range: 0 to 1.  Perfect score: 1.
+            - "True positives" is the same as "hits"
+            - "False positives" is the same as "misses"
+
+        References:
+            https://www.cawcr.gov.au/projects/verification/#SR
         """
         cd = self.counts
         sr = cd["tp_count"] / (cd["tp_count"] + cd["fp_count"])
 
         return sr
 
-    def threat_score(self):
+    def threat_score(self) -> xr.DataArray:
         """
-        How well did the forecast "yes" events correspond to the observed "yes" events?
         Identical to critical_success_index
-        Range: 0 to 1, 0 indicates no skill. Perfect score: 1.
 
-        https://www.cawcr.gov.au/projects/verification/#CSI
+        Returns:
+            xr.DataArray: An xarray object containing the threat score
+
+        .. math::
+            \\text{threat score} = \\frac{\\text{true positives}}{\\text{true positives} + \\text{false positives} + \\text{false negatives}}
+
+        Notes:
+            - Range: 0 to 1, 0 indicates no skill. Perfect score: 1.
+            - "True positives" is the same as "hits"
+            - "False positives" is the same as "false alarms"
+            - "True negatives" is the same as "correct negatives"
+
+        References:
+            https://www.cawcr.gov.au/projects/verification/#CSI
         """
         # Note - critical success index just calls this method
 
         cd = self.counts
-        ts = cd["tp_count"] / (cd["tp_count"] + cd["fp_count"] + cd["tn_count"])
+        ts = cd["tp_count"] / (cd["tp_count"] + cd["fp_count"] + cd["fn_count"])
         return ts
 
-    def critical_success_index(self):
+    def critical_success_index(self) -> xr.DataArray:
         """
-        Often known as CSI.
-
-        How well did the forecast "yes" events correspond to the observed "yes" events?
         Identical to threat_score
-        Range: 0 to 1, 0 indicates no skill. Perfect score: 1.
 
-        https://www.cawcr.gov.au/projects/verification/#CSI
+        .. math::
+            \\text{threat score} = \\frac{\\text{true positives}}{\\text{true positives} + \\text{false positives} + \\text{false negatives}}
+
+        Returns:
+            An xarray object containing the critical success index
+
+        Notes:
+            - Range: 0 to 1, 0 indicates no skill. Perfect score: 1.
+            - Often known as CSI.
+            - "True positives" is the same as "hits"
+            - "False positives" is the same as "false alarms"
+            - "True negatives" is the same as "correct negatives"
+
+        References:
+            https://www.cawcr.gov.au/projects/verification/#CSI
         """
         return self.threat_score()
 
-    def peirce_skill_score(self):
+    def peirce_skill_score(self) -> xr.DataArray:
         """
-        Hanssen and Kuipers discriminant (true skill statistic, Peirce's skill score)
+        Identical to Hanssen and Kuipers discriminant and the true skill statistic
+
         How well did the forecast separate the "yes" events from the "no" events?
-        Range: -1 to 1, 0 indicates no skill. Perfect score: 1.
 
-        https://www.cawcr.gov.au/projects/verification/#HK
+        Returns:
+            An xarray object containing the Peirce Skill Score
+
+        .. math::
+            \\text{Peirce skill score} = \\frac{\\text{true positives}}{\\text{true positives} + \\text{false negatives}} - \\frac{\\text{false positives}}{\\text{false positives} + \\text{true negatives}}
+
+        Notes:
+            - Range: -1 to 1, 0 indicates no skill. Perfect score: 1.
+            - "True positives" is the same as "hits"
+            - "False negatives" is the same as "misses"
+            - "False positives" is the same as "false alarms"
+            - "True negatives" is the same as "correct negatives"
+
+        References:
+            https://www.cawcr.gov.au/projects/verification/#HK
         """
         cd = self.counts
         component_a = cd["tp_count"] / (cd["tp_count"] + cd["fn_count"])
         component_b = cd["fp_count"] / (cd["fp_count"] + cd["tn_count"])
         skill_score = component_a - component_b
         return skill_score
 
-    def true_skill_statistic(self):
+    def true_skill_statistic(self) -> xr.DataArray:
         """
         Identical to Peirce's skill score and to Hanssen and Kuipers discriminant
+
         How well did the forecast separate the "yes" events from the "no" events?
-        Range: -1 to 1, 0 indicates no skill. Perfect score: 1.
 
-        https://www.cawcr.gov.au/projects/verification/#HK
+        Returns:
+            xr.DataArray: An xarray object containing the true skill statistic
+
+        .. math::
+            \\text{true skill statistic} = \\frac{\\text{true positives}}{\\text{true positives} + \\text{false negatives}} - \\frac{\\text{false positives}}{\\text{false positives} + \\text{true negatives}}
+
+        Notes:
+            - Range: -1 to 1, 0 indicates no skill. Perfect score: 1.
+            - "True positives" is the same as "hits"
+            - "False negatives" is the same as "misses"
+            - "False positives" is the same as "false alarms"
+            - "True negatives" is the same as "correct negatives"
+
+        References:
+            https://www.cawcr.gov.au/projects/verification/#HK
         """
         return self.peirce_skill_score()
 
-    def hanssen_and_kuipers_discriminant(self):
+    def hanssen_and_kuipers_discriminant(self) -> xr.DataArray:
         """
         Identical to Peirce's skill score and to true skill statistic
+
         How well did the forecast separate the "yes" events from the "no" events?
-        Range: -1 to 1, 0 indicates no skill. Perfect score: 1.
 
-        https://www.cawcr.gov.au/projects/verification/#HK
+        Returns:
+            xr.DataArray: An xarray object containing Hanssen and Kuipers' Discriminant
+
+        .. math::
+            \\text{HK} = \\frac{\\text{true positives}}{\\text{true positives} + \\text{false negatives}} - \\frac{\\text{false positives}}{\\text{false positives} + \\text{true negatives}}
+
+        Where :math:`\\text{HK}` is Hansen and Kuipers Discriminant
+
+        Notes:
+            - Range: -1 to 1, 0 indicates no skill. Perfect score: 1.
+            - "True positives" is the same as "hits"
+            - "False negatives" is the same as "misses"
+            - "False positives" is the same as "false alarms"
+            - "True negatives" is the same as "correct negatives"
+
+        References:
+            https://www.cawcr.gov.au/projects/verification/#HK
         """
         return self.peirce_skill_score()
 
-    def sensitivity(self):
+    def sensitivity(self) -> xr.DataArray:
         """
-        https://en.wikipedia.org/wiki/Sensitivity_and_specificity
+        Identical to probability of detection and hit_rate
+
+        Calculates the proportion of the observed events that were correctly forecast.
+
+        Returns:
+            An xarray object containing the probability of detection
+
+        .. math::
+            \\text{sensitivity} = \\frac{\\text{true positives}}{\\text{true positives} + \\text{false negatives}}
+
+        Notes:
+            - Range: 0 to 1.  Perfect score: 1.
+            - "True positives" is the same as "hits"
+            - "False negatives" is the same as "misses"
+
+        References:
+            - https://www.cawcr.gov.au/projects/verification/#POD
+            - https://en.wikipedia.org/wiki/Sensitivity_and_specificity
+
         """
         return self.probability_of_detection()
 
-    def specificity(self):
+    def specificity(self) -> xr.DataArray:
         """
-        https://en.wikipedia.org/wiki/Sensitivity_and_specificity
+        Identical to true negative rate.
+
+        The probability that an observed non-event will be correctly predicted.
+
+        Returns:
+            xr.DataArray: An xarray object containing the true negative rate (specificity).
+
+        .. math::
+            \\text{specificity} = \\frac{\\text{true negatives}}{\\text{true negatives} + \\text{false positives}}
+
+        Notes:
+            - "True negatives" is the same as "correct negatives".
+            - "False positives" is the same as "false alarms".
+
+        Reference:
+            https://en.wikipedia.org/wiki/Sensitivity_and_specificity
         """
         cd = self.counts
         s = cd["tn_count"] / (cd["tn_count"] + cd["fp_count"])
         return s
 
-    def recall(self):
+    def true_negative_rate(self) -> xr.DataArray:
+        """
+        Identical to specificity.
+
+        The probability that an observed non-event will be correctly predicted.
+
+        Returns:
+            xr.DataArray: An xarray object containing the true negative rate.
+
+        .. math::
+            \\text{true negative rate} = \\frac{\\text{true negatives}}{\\text{true negatives} + \\text{false positives}}
+
+        Notes:
+            - "True negatives" is the same as "correct negatives".
+            - "False positives" is the same as "false alarms".
+
+        Reference:
+            https://en.wikipedia.org/wiki/Sensitivity_and_specificity
+        """
+        return self.specificity()
+
+    def recall(self) -> xr.DataArray:
         """
         Identical to probability of detection.
 
-        https://en.wikipedia.org/wiki/Precision_and_recall
+        Calculates the proportion of the observed events that were correctly forecast.
+
+        Returns:
+            An xarray object containing the probability of detection
+
+        .. math::
+            \\text{recall} = \\frac{\\text{true positives}}{\\text{true positives} + \\text{false negatives}}
+
+        Notes:
+            - Range: 0 to 1.  Perfect score: 1.
+            - "True positives" is the same as "hits"
+            - "False negatives" is the same as "misses"
+
+        References:
+            - https://www.cawcr.gov.au/projects/verification/#POD
+            - https://en.wikipedia.org/wiki/Precision_and_recall
         """
         return self.probability_of_detection()
 
     def precision(self):
         """
         Identical to the Success Ratio.
 
@@ -309,17 +594,22 @@
         Calculates the Equitable threat score (also known as the Gilbert skill score).
 
         How well did the forecast "yes" events correspond to the observed "yes"
         events (accounting for hits due to chance)?
 
         Range: -1/3 to 1, 0 indicates no skill. Perfect score: 1.
 
+
+        References:
+
+        Gilbert, G.K., 1884. Finley’s tornado predictions. American Meteorological Journal, 1(5), pp.166–172.
+
         Hogan, R.J., Ferro, C.A., Jolliffe, I.T. and Stephenson, D.B., 2010.
         Equitability revisited: Why the “equitable threat score” is not equitable.
-        Weather and Forecasting, 25(2), pp.710-726.
+        Weather and Forecasting, 25(2), pp.710-726. https://doi.org/10.1175/2009WAF2222350.1
         """
         cd = self.counts
         hits_random = (cd["tp_count"] + cd["fn_count"]) * (cd["tp_count"] + cd["fp_count"]) / cd["total_count"]
         ets = (cd["tp_count"] - hits_random) / (cd["tp_count"] + cd["fn_count"] + cd["fp_count"] - hits_random)
 
         return ets
 
@@ -328,17 +618,21 @@
         Calculates the Gilbert skill score (also known as the Equitable threat score).
 
         How well did the forecast "yes" events correspond to the observed "yes"
         events (accounting for hits due to chance)?
 
         Range: -1/3 to 1, 0 indicates no skill. Perfect score: 1.
 
+        References:
+
+        Gilbert, G.K., 1884. Finley’s tornado predictions. American Meteorological Journal, 1(5), pp.166–172.
+
         Hogan, R.J., Ferro, C.A., Jolliffe, I.T. and Stephenson, D.B., 2010.
         Equitability revisited: Why the “equitable threat score” is not equitable.
-        Weather and Forecasting, 25(2), pp.710-726.
+        Weather and Forecasting, 25(2), pp.710-726. https://doi.org/10.1175/2009WAF2222350.1
         """
         return self.equitable_threat_score()
 
     def heidke_skill_score(self):
         """
         Calculates the Heidke skill score (also known as Cohen's kappa).
 
@@ -413,26 +707,29 @@
         Weather and Forecasting, 15(2), pp.221-232.
         """
         return self.odds_ratio_skill_score()
 
 
 class BinaryContingencyManager(BasicContingencyManager):
     """
+
     At each location, the value will either be:
-     - A true positive (hit)
-     - A false positive (false alarm)
-     - A true negative (correct negative)
-     - A false negative (miss)
+
+    - A true positive (hit)
+    - A false positive (false alarm)
+    - A true negative (correct negative)
+    - A false negative (miss)
+
 
     It will be common to want to operate on masks of these values,
     such as:
-     - Plotting these attributes on a map
-     - Calculating the total number of these attributes
-     - Calculating various ratios of these attributes, potentially
-       masked by geographical area (e.g. accuracy in a region)
+
+    - Plotting these attributes on a map
+    - Calculating the total number of these attributes
+    - Calculating various ratios of these attributes, potentially masked by geographical area (e.g. accuracy in a region)
 
     As such, the per-pixel information is useful as well as the overall
     ratios involved.
 
     BinaryContingencyManager utilises the BasicContingencyManager class to provide
     most functionality.
     """
```

### Comparing `scores-0.8.3/src/scores/categorical/multicategorical_impl.py` & `scores-0.8.4/src/scores/categorical/multicategorical_impl.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.3/src/scores/continuous/__init__.py` & `scores-0.8.4/src/scores/continuous/__init__.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.3/src/scores/continuous/flip_flop_impl.py` & `scores-0.8.4/src/scores/continuous/flip_flop_impl.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.3/src/scores/continuous/murphy_impl.py` & `scores-0.8.4/src/scores/continuous/murphy_impl.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.3/src/scores/continuous/quantile_loss_impl.py` & `scores-0.8.4/src/scores/continuous/quantile_loss_impl.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.3/src/scores/continuous/standard_impl.py` & `scores-0.8.4/src/scores/continuous/standard_impl.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.3/src/scores/pandas/continuous.py` & `scores-0.8.4/src/scores/pandas/continuous.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.3/src/scores/probability/__init__.py` & `scores-0.8.4/src/scores/probability/__init__.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.3/src/scores/probability/brier_impl.py` & `scores-0.8.4/src/scores/probability/brier_impl.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.3/src/scores/probability/checks.py` & `scores-0.8.4/src/scores/probability/checks.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.3/src/scores/probability/crps_impl.py` & `scores-0.8.4/src/scores/probability/crps_impl.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.3/src/scores/probability/roc_impl.py` & `scores-0.8.4/src/scores/probability/roc_impl.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.3/src/scores/processing/__init__.py` & `scores-0.8.4/src/scores/processing/__init__.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.3/src/scores/processing/discretise.py` & `scores-0.8.4/src/scores/processing/discretise.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,17 +184,16 @@
 ):
     """
     Calculates the proportion of `data` equal to or exceeding `thresholds`.
 
     Args:
         data (xarray.Dataset or xarray.DataArray): The data from which
             to calculate the proportion exceeding `thresholds`
-        thresholds (iterable): The proportion of Flip-Flop Index results
+        thresholds (iterable): The proportion of values
             equal to or exceeding these thresholds will be calculated.
-            the Flip-Flop Index.
         reduce_dims: Dimensions to reduce.
         preserve_dims: Dimensions to preserve.
 
     Returns:
         An xarray data object with the type of `data` and dimensions
         `dims` + 'threshold'. The values are the proportion of `data`
         that are greater than or equal to the corresponding threshold.
@@ -218,17 +217,16 @@
     defined by the relationship of data to threshold as specified by
     the operation `mode`.
 
     Args:
         data: The data to convert
            into 0 and 1 according the thresholds before calculating the
            proportion.
-        thresholds: The proportion of Flip-Flop Index results
+        thresholds: The proportion of values
             equal to or exceeding these thresholds will be calculated.
-            the Flip-Flop Index.
         mode: Specifies the required relation of `data` to `thresholds`
             for a value to fall in the 'event' category (i.e. assigned to 1).
             Allowed modes are:
 
             - '>=' values in `data` greater than or equal to the
               corresponding threshold are assigned as 1.
             - '>' values in `data` greater than the corresponding threshold
```

### Comparing `scores-0.8.3/src/scores/processing/isoreg_impl.py` & `scores-0.8.4/src/scores/processing/isoreg_impl.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.3/src/scores/processing/matching.py` & `scores-0.8.4/src/scores/processing/matching.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.3/src/scores/processing/cdf/cdf_functions.py` & `scores-0.8.4/src/scores/processing/cdf/cdf_functions.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.3/src/scores/stats/statistical_tests/acovf.py` & `scores-0.8.4/src/scores/stats/statistical_tests/acovf.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.3/src/scores/stats/statistical_tests/diebold_mariano_impl.py` & `scores-0.8.4/src/scores/stats/statistical_tests/diebold_mariano_impl.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.3/.gitignore` & `scores-0.8.4/.gitignore`

 * *Files identical despite different names*

### Comparing `scores-0.8.3/LICENSE` & `scores-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `scores-0.8.3/README.md` & `scores-0.8.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 # Scores: Verification and Evaluation for Forecasts and Models
+
+> **Notice:**
+> **`scores` is undergoing final testing and review. When this is completed, this notice will be removed.**
+
 > 
 > **A list of over 50 metrics, statistical techniques and data processing tools contained in `scores` is [available here](https://scores.readthedocs.io/en/latest/included.html).**
 
 `scores` is a Python package containing mathematical functions for the verification, evaluation, and optimisation of forecasts, predictions or models. It primarily supports the meteorological, climatological and geoscience communities. In addition to supporting the Earth system science communities, it also has wide potential application in machine learning and other domains.
 
 Documentation is hosted at [scores.readthedocs.io](https://scores.readthedocs.io).  
 Source code is hosted at [github.com/nci/scores](https://github.com/nci/scores).  
-The tutorial gallery is hosted at [as part of the documentation, here](https://scores.readthedocs.io/en/latest/tutorials/Explanation.html).
+The tutorial gallery is hosted at [as part of the documentation, here](https://scores.readthedocs.io/en/latest/tutorials/Tutorial_Gallery.html). 
 
 ## Overview
 Here is a **curated selection** of the metrics, tools and statistical tests included in `scores`:
 
 |                       	| **Description** 	| **Selection of Included Functions** 	|
 |-----------------------	|-----------------	|--------------	|
 | **[Continuous](https://scores.readthedocs.io/en/latest/included.html#continuous)**        	|Scores for evaluating single-valued continuous forecasts.                  	|Mean Absolute Error (MAE), Mean Squared Error (MSE), Root Mean Squared Error (RMSE), Additive Bias, Multiplicative Bias, Pearson's Correlation Coefficient, Flip-Flop Index, Quantile loss, Murphy score.              	|
 | **[Probability](https://scores.readthedocs.io/en/latest/included.html#probability)**       	|Scores for evaluating forecasts that are expressed as predictive distributions, ensembles, and probabilities of binary events.                 	|Brier Score, Continuous Ranked Probability Score (CRPS) for Cumulative Density Function (CDF), Threshold weighted CRPS for CDF, CRPS for ensembles, Receiver Operating Characteristic (ROC), Isotonic Regression (reliability diagrams).              	|
-| **[Categorical](https://scores.readthedocs.io/en/latest/included.html#categorical)**       	|Scores for evaluating forecasts based on categories.                	|Probability of Detection (POD), False Alarm Rate (FAR), Probability of False Detection (POFD), Success Ratio, Accuracy, Peirce's Skill Score, Critical Success Index (CSI), Gilbert Skill Score, Heidke Skill Score, Odds Ratio, Odds Ratio Skill Score, F1 score, FIxed Risk Multicategorical (FIRM) Score.               	|
+| **[Categorical](https://scores.readthedocs.io/en/latest/included.html#categorical)**       	|Scores for evaluating forecasts based on categories.                	|Probability of Detection (POD), False Alarm Ratio (FAR), Probability of False Detection (POFD), Success Ratio, Accuracy, Peirce's Skill Score, Critical Success Index (CSI), Gilbert Skill Score, Heidke Skill Score, Odds Ratio, Odds Ratio Skill Score, F1 score, FIxed Risk Multicategorical (FIRM) Score.               	|
 | **[Statistical Tests](https://scores.readthedocs.io/en/latest/included.html#statistical-tests)** 	|Tools to conduct statistical tests and generate confidence intervals.                 	|Diebold Mariano.              	|
 | **[Processing Tools](https://scores.readthedocs.io/en/latest/included.html#processing-tools-for-preparing-data)**        	|Tools to pre-process data.                 	|Data matching, Discretisation, Cumulative Density Function Manipulation.              	|
 
 
 `scores` not only includes common scores (e.g. MAE, RMSE), it includes novel scores not commonly found elsewhere (e.g. FIRM, Flip-Flop Index), complex scores (e.g. threshold weighted CRPS), and statistical tests (such as the Diebold Mariano test). Additionally, it provides pre-processing tools for preparing data for scores in a variety of formats including cumulative distribution functions (CDF). `scores` provides its own implementations where relevant to avoid extensive dependencies.
 
-`scores` primarily supports xarray datatypes for Earth system data allowing it to work with NetCDF4, hdf5, Zarr and GRIB data sources among others. `scores` uses Dask for scaling and performance. Some metrics work with pandas and we will aim to expand this capability. 
+`scores` primarily supports xarray datatypes for Earth system data allowing it to work with NetCDF4, HDF5, Zarr and GRIB data sources among others. `scores` uses Dask for scaling and performance. Some metrics work with pandas and we will aim to expand this capability. 
 
 All of the scores and metrics in this package have undergone a thorough scientific review. Every score has a companion Jupyter Notebook tutorial that demonstrates its use in practice.
 
 ## Contributing
-To find out more about contributing, see our [contributor's guide](https://github.com/nci/scores/blob/main/docs/contributing.md).
+To find out more about contributing, see our [Contributing Guide](https://scores.readthedocs.io/en/latest/contributing.html).
 
 All interactions in discussions, issues, emails and code (e.g. merge requests, code comments) will be managed according to the expectations outlined in the [ code of conduct ](https://github.com/nci/scores/blob/main/CODE_OF_CONDUCT.md) and in accordance with all relevant laws and obligations. This project is an inclusive, respectful and open project with high standards for respectful behaviour and language. The code of conduct is the Contributor Covenant, adopted by over 40,000 open source projects. Any concerns will be dealt with fairly and respectfully, with the processes described in the code of conduct.
 
 ## Using This Package
 
 The [installation guide](https://scores.readthedocs.io/en/latest/installation.html) describes four different use cases for installing, using and working with this package.
```

### Comparing `scores-0.8.3/pyproject.toml` & `scores-0.8.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scores-0.8.3/PKG-INFO` & `scores-0.8.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: scores
-Version: 0.8.3
+Version: 0.8.4
 Summary: Scores is a package containing mathematical functions for the verification, evaluation and optimisation of forecasts, predictions or models.
 Project-URL: Repository, https://github.com/nci/scores
 Project-URL: Documentation, https://scores.readthedocs.io/en/latest/
 Author-email: Tennessee Leeuwenburg <tennessee.leeuwenburg@bom.gov.au>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -63,43 +63,47 @@
 Requires-Dist: matplotlib; extra == 'tutorial'
 Requires-Dist: plotly; extra == 'tutorial'
 Requires-Dist: rasterio; extra == 'tutorial'
 Requires-Dist: rioxarray; extra == 'tutorial'
 Description-Content-Type: text/markdown
 
 # Scores: Verification and Evaluation for Forecasts and Models
+
+> **Notice:**
+> **`scores` is undergoing final testing and review. When this is completed, this notice will be removed.**
+
 > 
 > **A list of over 50 metrics, statistical techniques and data processing tools contained in `scores` is [available here](https://scores.readthedocs.io/en/latest/included.html).**
 
 `scores` is a Python package containing mathematical functions for the verification, evaluation, and optimisation of forecasts, predictions or models. It primarily supports the meteorological, climatological and geoscience communities. In addition to supporting the Earth system science communities, it also has wide potential application in machine learning and other domains.
 
 Documentation is hosted at [scores.readthedocs.io](https://scores.readthedocs.io).  
 Source code is hosted at [github.com/nci/scores](https://github.com/nci/scores).  
-The tutorial gallery is hosted at [as part of the documentation, here](https://scores.readthedocs.io/en/latest/tutorials/Explanation.html).
+The tutorial gallery is hosted at [as part of the documentation, here](https://scores.readthedocs.io/en/latest/tutorials/Tutorial_Gallery.html). 
 
 ## Overview
 Here is a **curated selection** of the metrics, tools and statistical tests included in `scores`:
 
 |                       	| **Description** 	| **Selection of Included Functions** 	|
 |-----------------------	|-----------------	|--------------	|
 | **[Continuous](https://scores.readthedocs.io/en/latest/included.html#continuous)**        	|Scores for evaluating single-valued continuous forecasts.                  	|Mean Absolute Error (MAE), Mean Squared Error (MSE), Root Mean Squared Error (RMSE), Additive Bias, Multiplicative Bias, Pearson's Correlation Coefficient, Flip-Flop Index, Quantile loss, Murphy score.              	|
 | **[Probability](https://scores.readthedocs.io/en/latest/included.html#probability)**       	|Scores for evaluating forecasts that are expressed as predictive distributions, ensembles, and probabilities of binary events.                 	|Brier Score, Continuous Ranked Probability Score (CRPS) for Cumulative Density Function (CDF), Threshold weighted CRPS for CDF, CRPS for ensembles, Receiver Operating Characteristic (ROC), Isotonic Regression (reliability diagrams).              	|
-| **[Categorical](https://scores.readthedocs.io/en/latest/included.html#categorical)**       	|Scores for evaluating forecasts based on categories.                	|Probability of Detection (POD), False Alarm Rate (FAR), Probability of False Detection (POFD), Success Ratio, Accuracy, Peirce's Skill Score, Critical Success Index (CSI), Gilbert Skill Score, Heidke Skill Score, Odds Ratio, Odds Ratio Skill Score, F1 score, FIxed Risk Multicategorical (FIRM) Score.               	|
+| **[Categorical](https://scores.readthedocs.io/en/latest/included.html#categorical)**       	|Scores for evaluating forecasts based on categories.                	|Probability of Detection (POD), False Alarm Ratio (FAR), Probability of False Detection (POFD), Success Ratio, Accuracy, Peirce's Skill Score, Critical Success Index (CSI), Gilbert Skill Score, Heidke Skill Score, Odds Ratio, Odds Ratio Skill Score, F1 score, FIxed Risk Multicategorical (FIRM) Score.               	|
 | **[Statistical Tests](https://scores.readthedocs.io/en/latest/included.html#statistical-tests)** 	|Tools to conduct statistical tests and generate confidence intervals.                 	|Diebold Mariano.              	|
 | **[Processing Tools](https://scores.readthedocs.io/en/latest/included.html#processing-tools-for-preparing-data)**        	|Tools to pre-process data.                 	|Data matching, Discretisation, Cumulative Density Function Manipulation.              	|
 
 
 `scores` not only includes common scores (e.g. MAE, RMSE), it includes novel scores not commonly found elsewhere (e.g. FIRM, Flip-Flop Index), complex scores (e.g. threshold weighted CRPS), and statistical tests (such as the Diebold Mariano test). Additionally, it provides pre-processing tools for preparing data for scores in a variety of formats including cumulative distribution functions (CDF). `scores` provides its own implementations where relevant to avoid extensive dependencies.
 
-`scores` primarily supports xarray datatypes for Earth system data allowing it to work with NetCDF4, hdf5, Zarr and GRIB data sources among others. `scores` uses Dask for scaling and performance. Some metrics work with pandas and we will aim to expand this capability. 
+`scores` primarily supports xarray datatypes for Earth system data allowing it to work with NetCDF4, HDF5, Zarr and GRIB data sources among others. `scores` uses Dask for scaling and performance. Some metrics work with pandas and we will aim to expand this capability. 
 
 All of the scores and metrics in this package have undergone a thorough scientific review. Every score has a companion Jupyter Notebook tutorial that demonstrates its use in practice.
 
 ## Contributing
-To find out more about contributing, see our [contributor's guide](https://github.com/nci/scores/blob/main/docs/contributing.md).
+To find out more about contributing, see our [Contributing Guide](https://scores.readthedocs.io/en/latest/contributing.html).
 
 All interactions in discussions, issues, emails and code (e.g. merge requests, code comments) will be managed according to the expectations outlined in the [ code of conduct ](https://github.com/nci/scores/blob/main/CODE_OF_CONDUCT.md) and in accordance with all relevant laws and obligations. This project is an inclusive, respectful and open project with high standards for respectful behaviour and language. The code of conduct is the Contributor Covenant, adopted by over 40,000 open source projects. Any concerns will be dealt with fairly and respectfully, with the processes described in the code of conduct.
 
 ## Using This Package
 
 The [installation guide](https://scores.readthedocs.io/en/latest/installation.html) describes four different use cases for installing, using and working with this package.
```

