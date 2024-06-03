# Comparing `tmp/chasta-0.1.3.tar.gz` & `tmp/chasta-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chasta-0.1.3.tar", max compression
+gzip compressed data, was "chasta-0.1.4.tar", max compression
```

## Comparing `chasta-0.1.3.tar` & `chasta-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      439 2024-01-22 01:47:55.313229 chasta-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-07-16 02:58:42.192702 chasta-0.1.3/chasta/__init__.py
--rw-r--r--   0        0        0     6862 2024-01-22 04:21:57.829055 chasta-0.1.3/chasta/chasta.py
--rw-r--r--   0        0        0      447 2024-01-22 04:14:53.625555 chasta-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      946 1970-01-01 00:00:00.000000 chasta-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      663 2024-03-10 22:17:25.729493 chasta-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-07-16 02:58:42.192702 chasta-0.1.4/chasta/__init__.py
+-rw-r--r--   0        0        0     7554 2024-06-03 01:46:47.690911 chasta-0.1.4/chasta/chasta.py
+-rw-r--r--   0        0        0      447 2024-06-03 02:31:27.705292 chasta-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1170 1970-01-01 00:00:00.000000 chasta-0.1.4/PKG-INFO
```

### Comparing `chasta-0.1.3/chasta/chasta.py` & `chasta-0.1.4/chasta/chasta.py`

 * *Files 8% similar despite different names*

```diff
@@ -92,21 +92,46 @@
             df_to_chart = df[[*selected_column_names, chart_column_name]]
         else:
             df_to_chart = df_to_stats
 
     return df_to_stats, df_to_chart
 
 
+def determine_decimals(series):
+    max_val = abs(series.max())
+
+    if max_val >= 1000:
+        return 0
+    elif max_val >= 100:
+        return 1
+    elif max_val >= 10:
+        return 2
+    else:
+        return 3
+
+
+def format_stats(stats: Union[Series, DataFrame])-> Union[Series, DataFrame]:
+    # Determine the maximum number of decimal places needed across all columns
+    decimals = 0
+    for column in stats.columns:
+        col_decimals = determine_decimals(stats[column])
+        if col_decimals > decimals:
+            decimals = col_decimals
+    formatted_stats = stats.applymap(lambda x: f"{x:,.{decimals}f}")
+
+    return formatted_stats
+
 def get_stats_from_df(df_to_stats: pd.DataFrame, do_instance_count: bool) -> Union[Series, DataFrame]:
     if do_instance_count:
         stats = df_to_stats.value_counts()
     else:
         stats = df_to_stats.describe(percentiles=[.25, .50, .75, .90, .95, .99, .999], include='all')
         if '50%' in stats.index:
             stats.loc['median'] = stats.loc['50%']
+            stats = format_stats(stats)
 
     return stats
 
 
 def analyze_file(file_path: str, do_instance_count: bool = False, chart: Union[None, str] = None, delimiter: str = ',',
                  columns_str: str = '0') -> Tuple[Union[None, pd.DataFrame], Union[pd.DataFrame, pd.Series, None]]:
     try:
```

### Comparing `chasta-0.1.3/PKG-INFO` & `chasta-0.1.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chasta
-Version: 0.1.3
+Version: 0.1.4
 Summary: CHArt and run STAtitics on CSV data
 Author: Jerome Provensal
 Author-email: jeromegit@provensal.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -18,8 +18,12 @@
  * if data columns have different scale/range, use multiple Y-axis or left/right
  * use timeseries for x-axis
  * use "steps" in charts
  * store both data/html into a file that that can be "served"
  * allow to upload the chartable data to "the cloud" or at known file/data repo
  * store the data compressed
  * use a bit.ly type of short/random URL to access to saved data
- * 
+ * along with the normal describe stats add sum()
+ * when a delimiter is specified such as |, assume \s*|\s*
+ * combine the output of describe() and info()
+ * look for Exploratory Data Analysis (EDA) techniques
+ * Missing data?
```

