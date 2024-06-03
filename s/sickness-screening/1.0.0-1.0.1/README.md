# Comparing `tmp/sickness_screening-1.0.0.tar.gz` & `tmp/sickness_screening-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sickness_screening-1.0.0.tar", last modified: Sat Jun  1 17:40:00 2024, max compression
+gzip compressed data, was "dist/sickness_screening-1.0.1.tar", last modified: Mon Jun  3 12:59:28 2024, max compression
```

## Comparing `sickness_screening-1.0.0.tar` & `sickness_screening-1.0.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 artemij    (501) staff       (20)        0 2024-06-01 17:40:00.000000 sickness_screening-1.0.0/
--rw-r--r--   0 artemij    (501) staff       (20)     8300 2024-06-01 17:40:00.000000 sickness_screening-1.0.0/PKG-INFO
--rw-r--r--   0 artemij    (501) staff       (20)     6136 2024-06-01 15:49:46.000000 sickness_screening-1.0.0/README.md
-drwxr-xr-x   0 artemij    (501) staff       (20)        0 2024-06-01 17:40:00.000000 sickness_screening-1.0.0/sickness_screening.egg-info/
--rw-r--r--   0 artemij    (501) staff       (20)     8300 2024-06-01 17:40:00.000000 sickness_screening-1.0.0/sickness_screening.egg-info/PKG-INFO
--rw-r--r--   0 artemij    (501) staff       (20)      669 2024-06-01 17:40:00.000000 sickness_screening-1.0.0/sickness_screening.egg-info/SOURCES.txt
--rw-r--r--   0 artemij    (501) staff       (20)      150 2024-06-01 17:40:00.000000 sickness_screening-1.0.0/sickness_screening.egg-info/requires.txt
--rw-r--r--   0 artemij    (501) staff       (20)       19 2024-06-01 17:40:00.000000 sickness_screening-1.0.0/sickness_screening.egg-info/top_level.txt
--rw-r--r--   0 artemij    (501) staff       (20)        1 2024-06-01 17:40:00.000000 sickness_screening-1.0.0/sickness_screening.egg-info/dependency_links.txt
--rw-r--r--   0 artemij    (501) staff       (20)     1019 2024-06-01 17:39:15.000000 sickness_screening-1.0.0/setup.py
--rw-r--r--   0 artemij    (501) staff       (20)       38 2024-06-01 17:40:00.000000 sickness_screening-1.0.0/setup.cfg
-drwxr-xr-x   0 artemij    (501) staff       (20)        0 2024-06-01 17:40:00.000000 sickness_screening-1.0.0/sickness_screening/
--rw-r--r--   0 artemij    (501) staff       (20)     2849 2024-06-01 17:39:15.000000 sickness_screening-1.0.0/sickness_screening/get_analasys_data.py
--rw-r--r--   0 artemij    (501) staff       (20)     1774 2024-05-31 14:27:13.000000 sickness_screening-1.0.0/sickness_screening/choose.py
--rw-r--r--   0 artemij    (501) staff       (20)     3694 2024-05-31 13:59:27.000000 sickness_screening-1.0.0/sickness_screening/balance_on_patients.py
--rw-r--r--   0 artemij    (501) staff       (20)     4197 2024-05-31 15:34:40.000000 sickness_screening-1.0.0/sickness_screening/train_model.py
--rw-r--r--   0 artemij    (501) staff       (20)     8414 2024-05-31 12:51:29.000000 sickness_screening-1.0.0/sickness_screening/transformers.py
--rw-r--r--   0 artemij    (501) staff       (20)     1464 2024-05-31 15:05:36.000000 sickness_screening-1.0.0/sickness_screening/fill_values.py
--rw-r--r--   0 artemij    (501) staff       (20)     1870 2024-05-31 12:49:20.000000 sickness_screening-1.0.0/sickness_screening/get_disease_info.py
--rw-r--r--   0 artemij    (501) staff       (20)      846 2024-06-01 17:39:15.000000 sickness_screening-1.0.0/sickness_screening/__init__.py
--rw-r--r--   0 artemij    (501) staff       (20)     4533 2024-06-01 17:39:15.000000 sickness_screening-1.0.0/sickness_screening/combine_data.py
--rw-r--r--   0 artemij    (501) staff       (20)     1710 2024-06-01 17:39:14.000000 sickness_screening-1.0.0/sickness_screening/get_diagnoses_data.py
--rw-r--r--   0 artemij    (501) staff       (20)     7265 2024-05-31 12:49:20.000000 sickness_screening-1.0.0/sickness_screening/merge_and_get_data.py
--rw-r--r--   0 artemij    (501) staff       (20)     1026 2024-05-31 14:16:45.000000 sickness_screening-1.0.0/sickness_screening/compress.py
+drwxr-xr-x   0 artemij    (501) staff       (20)        0 2024-06-03 12:59:28.000000 sickness_screening-1.0.1/
+-rw-r--r--   0 artemij    (501) staff       (20)    11275 2024-06-03 12:59:28.000000 sickness_screening-1.0.1/PKG-INFO
+-rw-r--r--   0 artemij    (501) staff       (20)     8679 2024-06-03 12:58:05.000000 sickness_screening-1.0.1/README.md
+drwxr-xr-x   0 artemij    (501) staff       (20)        0 2024-06-03 12:59:28.000000 sickness_screening-1.0.1/sickness_screening.egg-info/
+-rw-r--r--   0 artemij    (501) staff       (20)    11275 2024-06-03 12:59:28.000000 sickness_screening-1.0.1/sickness_screening.egg-info/PKG-INFO
+-rw-r--r--   0 artemij    (501) staff       (20)      669 2024-06-03 12:59:28.000000 sickness_screening-1.0.1/sickness_screening.egg-info/SOURCES.txt
+-rw-r--r--   0 artemij    (501) staff       (20)      150 2024-06-03 12:59:28.000000 sickness_screening-1.0.1/sickness_screening.egg-info/requires.txt
+-rw-r--r--   0 artemij    (501) staff       (20)       19 2024-06-03 12:59:28.000000 sickness_screening-1.0.1/sickness_screening.egg-info/top_level.txt
+-rw-r--r--   0 artemij    (501) staff       (20)        1 2024-06-03 12:59:28.000000 sickness_screening-1.0.1/sickness_screening.egg-info/dependency_links.txt
+-rw-r--r--   0 artemij    (501) staff       (20)     1019 2024-06-03 12:59:20.000000 sickness_screening-1.0.1/setup.py
+-rw-r--r--   0 artemij    (501) staff       (20)       38 2024-06-03 12:59:28.000000 sickness_screening-1.0.1/setup.cfg
+drwxr-xr-x   0 artemij    (501) staff       (20)        0 2024-06-03 12:59:28.000000 sickness_screening-1.0.1/sickness_screening/
+-rw-r--r--   0 artemij    (501) staff       (20)     1778 2024-06-03 12:56:17.000000 sickness_screening-1.0.1/sickness_screening/choose.py
+-rw-r--r--   0 artemij    (501) staff       (20)     3694 2024-06-03 12:29:09.000000 sickness_screening-1.0.1/sickness_screening/balance_on_patients.py
+-rw-r--r--   0 artemij    (501) staff       (20)     4197 2024-06-03 12:29:09.000000 sickness_screening-1.0.1/sickness_screening/train_model.py
+-rw-r--r--   0 artemij    (501) staff       (20)     8414 2024-06-03 12:29:09.000000 sickness_screening-1.0.1/sickness_screening/transformers.py
+-rw-r--r--   0 artemij    (501) staff       (20)     1464 2024-06-03 12:29:09.000000 sickness_screening-1.0.1/sickness_screening/fill_values.py
+-rw-r--r--   0 artemij    (501) staff       (20)     1870 2024-06-03 12:29:09.000000 sickness_screening-1.0.1/sickness_screening/get_disease_info.py
+-rw-r--r--   0 artemij    (501) staff       (20)      829 2024-06-03 12:56:17.000000 sickness_screening-1.0.1/sickness_screening/__init__.py
+-rw-r--r--   0 artemij    (501) staff       (20)     4617 2024-06-03 12:56:17.000000 sickness_screening-1.0.1/sickness_screening/combine_data.py
+-rw-r--r--   0 artemij    (501) staff       (20)     1710 2024-06-03 12:29:09.000000 sickness_screening-1.0.1/sickness_screening/get_diagnoses_data.py
+-rw-r--r--   0 artemij    (501) staff       (20)     6981 2024-06-03 12:57:35.000000 sickness_screening-1.0.1/sickness_screening/merge_and_get_data.py
+-rw-r--r--   0 artemij    (501) staff       (20)     1026 2024-06-03 12:29:09.000000 sickness_screening-1.0.1/sickness_screening/compress.py
+-rw-r--r--   0 artemij    (501) staff       (20)     2840 2024-06-03 12:56:17.000000 sickness_screening-1.0.1/sickness_screening/get_analyzes_data.py
```

### Comparing `sickness_screening-1.0.0/sickness_screening.egg-info/SOURCES.txt` & `sickness_screening-1.0.1/sickness_screening.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 setup.py
 sickness_screening/__init__.py
 sickness_screening/balance_on_patients.py
 sickness_screening/choose.py
 sickness_screening/combine_data.py
 sickness_screening/compress.py
 sickness_screening/fill_values.py
-sickness_screening/get_analasys_data.py
+sickness_screening/get_analyzes_data.py
 sickness_screening/get_diagnoses_data.py
 sickness_screening/get_disease_info.py
 sickness_screening/merge_and_get_data.py
 sickness_screening/train_model.py
 sickness_screening/transformers.py
 sickness_screening.egg-info/PKG-INFO
 sickness_screening.egg-info/SOURCES.txt
```

### Comparing `sickness_screening-1.0.0/setup.py` & `sickness_screening-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 setup(
     name='sickness_screening',
-    version='1.0.0',
+    version='1.0.1',
     author='@Margo78, @akp1n',
     author_email='timtimk30@yandex.ru',
     description='Module for sepsis predictions',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://github.com/sslavian812/sepsis-predictions.git',
     packages=find_packages(),
```

### Comparing `sickness_screening-1.0.0/sickness_screening/get_analasys_data.py` & `sickness_screening-1.0.1/sickness_screening/get_analyzes_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import pandas as pd
 
 
-def get_analasys_data(chartevents_csv='chartevents.csv', subject_id_col='subject_id', itemid_col='itemid',
+def get_analyzes_data(analyzes_csv='chartevents.csv', subject_id_col='subject_id', itemid_col='itemid',
                       charttime_col='charttime', value_col='value', valuenum_col='valuenum', valueuom_col='valueuom',
                       itemids=None, rest_columns=None, output_csv='ssir.csv'):
     """
         Extracts specific item IDs from chartevents data, pivots the table, and saves the result to a CSV file.
         This function reads chartevents data from a CSV file, filters it based on specified item IDs, pivots the table to
         have item IDs as columns, and saves the resulting data to a 'output_csv' file.
 
         Args:
-            chartevents_csv (str): Path to the CSV file containing chartevents data. Default is 'chartevents.csv'.
+            analyzes_csv (str): Path to the CSV file containing chartevents data. Default is 'chartevents.csv'.
             subject_id_col (str): Column name for subject IDs. Default is 'subject_id'.
             itemid_col (str): Column name for item IDs. Default is 'itemid'.
             charttime_col (str): Column name for chart times. Default is 'charttime'.
             value_col (str): Column name for values. Default is 'value'.
             valuenum_col (str): Column name for numeric values. Default is 'valuenum'.
             valueuom_col (str): Column name for units of measurement. Default is 'valueuom'.
             itemids (list of int, optional): List of item IDs to filter. Default is None, which uses [220045, 220210, 223762, 223761, 225651].
@@ -26,15 +26,15 @@
         """
     if rest_columns is None:
         rest_columns = ['Heart rate', 'Respiratory rate', 'Temperature Fahrenheit', 'Temperature Celsius',
                         'Direct Bilurubin', 'Heart rate_valueom', 'Respiratory rate_valueom',
                         'Temperature Fahrenheit_valueom', 'Temperature Celsius_valueom', 'Direct Bilurubin_valueom']
     if itemids is None:
         itemids = [220045, 220210, 223762, 223761, 225651]
-    chartevents_df = pd.read_csv(chartevents_csv,
+    chartevents_df = pd.read_csv(analyzes_csv,
                                  usecols=[subject_id_col, itemid_col, charttime_col, value_col, valuenum_col,
                                           valueuom_col])
 
     filtered_df = chartevents_df[chartevents_df['itemid'].isin(itemids)]
     pivot_df = filtered_df.pivot_table(index=[subject_id_col, charttime_col], columns=itemid_col,
                                        values=[value_col, valueuom_col], aggfunc='first').reset_index()
     pivot_df.columns = [subject_id_col, charttime_col] + rest_columns
```

### Comparing `sickness_screening-1.0.0/sickness_screening/balance_on_patients.py` & `sickness_screening-1.0.1/sickness_screening/balance_on_patients.py`

 * *Files identical despite different names*

### Comparing `sickness_screening-1.0.0/sickness_screening/train_model.py` & `sickness_screening-1.0.1/sickness_screening/train_model.py`

 * *Files identical despite different names*

### Comparing `sickness_screening-1.0.0/sickness_screening/transformers.py` & `sickness_screening-1.0.1/sickness_screening/transformers.py`

 * *Files identical despite different names*

### Comparing `sickness_screening-1.0.0/sickness_screening/fill_values.py` & `sickness_screening-1.0.1/sickness_screening/fill_values.py`

 * *Files identical despite different names*

### Comparing `sickness_screening-1.0.0/sickness_screening/get_disease_info.py` & `sickness_screening-1.0.1/sickness_screening/get_disease_info.py`

 * *Files identical despite different names*

### Comparing `sickness_screening-1.0.0/sickness_screening/__init__.py` & `sickness_screening-1.0.1/sickness_screening/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import pandas as pd
 from .get_diagnoses_data import get_diagnoses_data
-from .get_analasys_data import get_analasys_data
+from .get_analyzes_data import get_analyzes_data
 from .get_disease_info import get_diseas_info
 from .balance_on_patients import balance_on_patients
 from .choose import choose
 from .combine_data import combine_data
 from .compress import compress
 from .fill_values import fill_values
-from .merge_and_get_data import merge_diagnoses_and_ssir_with_blood
+from .merge_and_get_data import merge_and_get_data
 from .train_model import train_model
 from .transformers import process_chartevents
 from .transformers import add_diagnosis_column
 from .transformers import impute_data
 from .transformers import prepare_and_save_data
 from .transformers import resample_test_val_data
 from .transformers import train_tabnet_model
```

### Comparing `sickness_screening-1.0.0/sickness_screening/combine_data.py` & `sickness_screening-1.0.1/sickness_screening/combine_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,68 +1,68 @@
 import pandas as pd
 
 
 def fahrenheit_to_celsius(f):
     return (f - 32) * 5.0 / 9.0
 
 
-def combine_data(gotten_diagnoses_csv='gottenDiagnoses.csv', has_sepsis_column='has_sepsis',
-                 ssir_csv='ssir.csv', title_column='long_title', subject_id_column='subject_id',
-                 output_sepsis_information_df='sepsis_info_df.csv', disease_str='sepsis', has_temp=True,
-                 temp_col1='Temperature Fahrenheit', temp_col2='Temperature Celsius',
+def combine_data(first_data='gottenDiagnoses.csv', has_disease_column='has_sepsis',
+                 second_data='ssir.csv', title_column='long_title', subject_id_column='subject_id',
+                 output_information_df='sepsis_info_df.csv', disease_str='sepsis', has_temp=True,
+                 translate_data_from_col='Temperature Fahrenheit', translate_data_to_col='Temperature Celsius',
                  translate_function=fahrenheit_to_celsius, value_column='valueuom', log_stats=True,
                  output_file='diagnoses_and_ssir.csv'):
     """
     Combines diagnoses and SSIR data, translate temperature from Fahrenheit to Celsius (or any other value if needed),
     and log statistics about sepsis patients.
     Also, it could be possible to combine any other csv data frames as long as both of them have specified columns.
     First should have title_column and subject_id, second data_frame should have at least subject_id column.
     Output file will have boolean value about long_title containing disease_str value.
     Args:
-        gotten_diagnoses_csv (str): Path to the CSV file containing diagnoses data. Default is 'gottenDiagnoses.csv'.
-        has_sepsis_column (str): Column name to indicate sepsis presence. Default is 'has_sepsis'.
-        ssir_csv (str): Path to the CSV file containing SSIR data. Default is 'ssir.csv'.
+        first_data (str): Path to the CSV file containing diagnoses data. Default is 'gottenDiagnoses.csv'.
+        has_disease_column (str): Column name to indicate sepsis presence. Default is 'has_sepsis'.
+        second_data (str): Path to the CSV file containing SSIR data. Default is 'ssir.csv'.
         title_column (str): Column name for diagnosis titles. Default is 'long_title'.
         subject_id_column (str): Column name for subject IDs. Default is 'subject_id'.
-        output_sepsis_information_df (str): Path to the output CSV file for sepsis information. Default is 'sepsis_info_df.csv'.
+        output_information_df (str): Path to the output CSV file for sepsis information. Default is 'sepsis_info_df.csv'.
         disease_str (str): String to identify sepsis-related diagnoses. Default is 'sepsis'.
         has_temp (bool): Whether to process temperature data. Default is True.
-        temp_col1 (str): Column name for temperature in Fahrenheit. Default is 'Temperature Fahrenheit'.
-        temp_col2 (str): Column name for temperature in Celsius. Default is 'Temperature Celsius'.
+        translate_data_from_col (str): Column name for temperature in Fahrenheit. Default is 'Temperature Fahrenheit'.
+        translate_data_to_col (str): Column name for temperature in Celsius. Default is 'Temperature Celsius'.
         translate_function (function): Function to convert Fahrenheit to Celsius. Default is fahrenheit_to_celsius.
         value_column (str): Column name to be excluded from the merged data. Default is 'valueom'.
         log_stats (bool): Whether to log statistics about sepsis patients. Default is True.
         output_file (str): Path to the output CSV file for combined data. Default is 'diagnoses_and_ssir.csv'.
 
     Returns:
         None: Writes the combined and processed data to the specified output file.
     """
-    diagnoses = pd.read_csv(gotten_diagnoses_csv)
-    ssir = pd.read_csv(ssir_csv)
-    diagnoses[has_sepsis_column] = diagnoses[title_column].str.contains(disease_str, case=False, na=False)
-    sepsis_info_df = diagnoses.groupby(subject_id_column)[has_sepsis_column].any().reset_index()
-    sepsis_info_df.to_csv(output_sepsis_information_df)
+    diagnoses = pd.read_csv(first_data)
+    ssir = pd.read_csv(second_data)
+    diagnoses[has_disease_column] = diagnoses[title_column].str.contains(disease_str, case=False, na=False)
+    sepsis_info_df = diagnoses.groupby(subject_id_column)[has_disease_column].any().reset_index()
+    sepsis_info_df.to_csv(output_information_df)
     merged_df = pd.merge(ssir, sepsis_info_df, on=subject_id_column, how='left')
     merged_df.drop(columns=[col for col in merged_df.columns if value_column in col], inplace=True)
     if has_temp:
-        merged_df[temp_col2] = merged_df.apply(
-            lambda row: translate_function(row[temp_col1]) if pd.notnull(
-                row[temp_col1]) else
-            row[temp_col2],
+        merged_df[translate_data_to_col] = merged_df.apply(
+            lambda row: translate_function(row[translate_data_from_col]) if pd.notnull(
+                row[translate_data_from_col]) else
+            row[translate_data_to_col],
             axis=1
         )
-        merged_df.drop(columns=[temp_col1], inplace=True)
+        merged_df.drop(columns=[translate_data_from_col], inplace=True)
     merged_df.to_csv(output_file, index=False)
     if log_stats:
-        ans = sepsis_info_df[has_sepsis_column].sum()
-        unique_patients = merged_df[[subject_id_column, has_sepsis_column]].drop_duplicates()
-        sepsis_counts = unique_patients[has_sepsis_column].value_counts(normalize=False)
+        ans = sepsis_info_df[has_disease_column].sum()
+        unique_patients = merged_df[[subject_id_column, has_disease_column]].drop_duplicates()
+        sepsis_counts = unique_patients[has_disease_column].value_counts(normalize=False)
         count_with_sepsis = sepsis_counts.get(True, 0)
         count_without_sepsis = sepsis_counts.get(False, 0)
-        grouped_sepsis = unique_patients.groupby(subject_id_column)[has_sepsis_column].agg(['min', 'max'])
+        grouped_sepsis = unique_patients.groupby(subject_id_column)[has_disease_column].agg(['min', 'max'])
         ambiguous_sepsis_patients = grouped_sepsis[grouped_sepsis['min'] != grouped_sepsis['max']]
         count_ambiguous_sepsis = len(ambiguous_sepsis_patients)
         print(f'Correct number of patients with sepsis: {ans}')
         print(f'Unique patients with predictions_sepsis: {count_with_sepsis}')
         print(f'Unique patients without predictions_sepsis: {count_without_sepsis}')
         print(f'Patients with both predictions_sepsis and no predictions_sepsis records: {count_ambiguous_sepsis}')
         print(f'All unique patients: {len(grouped_sepsis)}')
```

### Comparing `sickness_screening-1.0.0/sickness_screening/get_diagnoses_data.py` & `sickness_screening-1.0.1/sickness_screening/get_diagnoses_data.py`

 * *Files identical despite different names*

### Comparing `sickness_screening-1.0.0/sickness_screening/merge_and_get_data.py` & `sickness_screening-1.0.1/sickness_screening/merge_and_get_data.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 import pandas as pd
 
 
-def merge_diagnoses_and_ssir_with_blood(analysis_names=None, diagnoses_and_ssir_csv='diagnoses_and_ssir.csv',
-                                        blood_csv='labevents.csv', chartevents_csv='chartevents.csv',
-                                        output_csv='diagnoses_and_ssir_and_blood_and_chartevents.csv',
-                                        subject_id_column='subject_id',
-                                        charttime_column='charttime',
-                                        itemid_column='itemid',
-                                        has_sepsis_column='has_sepsis',
-                                        log_stats=True,
-                                        sepsis_info_df='sepsis_info_df.csv',
-                                        valueuom_column='valueuom'
-                                        ):
+def merge_and_get_data(analyzes_names=None, merge_with='diagnoses_and_ssir.csv',
+                       blood_csv='labevents.csv', get_data_from='chartevents.csv',
+                       output_csv='diagnoses_and_ssir_and_blood_and_chartevents.csv',
+                       subject_id_column='subject_id',
+                       time_column='charttime',
+                       itemid_column='itemid',
+                       has_sepsis_column='has_sepsis',
+                       log_stats=True,
+                       sepsis_info_df='sepsis_info_df.csv',
+                       valueuom_column='valueuom'
+                       ):
     """
         Merges diagnoses and SSIR data with blood and chartevents data, and logs statistics about sepsis patients.
         It is recommended to get file diagnoses_and_ssir by get_diagnoses and merge_diagnoses_and_ssir. 'sepsis_info_df' is recommended to be a path
         to a .csv file after 'get_disease_info' function.
         Args:
-            analysis_names (dict, optional): Dictionary mapping item IDs to analysis names. Default is None, in which case a predefined dictionary is used.
-            diagnoses_and_ssir_csv (str): Path to the CSV file containing diagnoses and SSIR data. Default is 'diagnoses_and_ssir.csv'.
+            analyzes_names (dict, optional): Dictionary mapping item IDs to analysis names. Default is None, in which case a predefined dictionary is used.
+            merge_with (str): Path to the CSV file containing diagnoses and SSIR data. Default is 'diagnoses_and_ssir.csv'.
             blood_csv (str): Path to the CSV file containing blood analysis data. Default is 'labevents.csv'.
-            chartevents_csv (str): Path to the CSV file containing chartevents data. Default is 'chartevents.csv'.
+            get_data_from (str): Path to the CSV file containing chartevents data. Default is 'chartevents.csv'.
             output_csv (str): Path to the output CSV file for combined data. Default is 'diagnoses_and_ssir_and_blood_and_chartevents.csv'.
             subject_id_column (str): Column name for subject IDs. Default is 'subject_id'.
-            charttime_column (str): Column name for chart times. Default is 'charttime'.
+            time_column (str): Column name for chart times. Default is 'charttime'.
             itemid_column (str): Column name for item IDs. Default is 'itemid'.
             has_sepsis_column (str): Column name to indicate sepsis presence. Default is 'has_sepsis'.
             log_stats (bool): Whether to log statistics about sepsis patients. Default is True.
             sepsis_info_df (str): Path to the CSV file containing sepsis information. Default is 'sepsis_info_df.csv'.
             valueuom_column (str): Column name for value units of measurement. Default is 'valueom'.
         Returns:
             None: Writes the combined and processed data to the specified output file and logs statistics if required.
         """
-    if analysis_names is None:
-        analysis_names = {
+    if analyzes_names is None:
+        analyzes_names = {
             51222: "Hemoglobin",
             51279: "Red Blood Cell",
             51240: "Large Platelets",
             50861: "Alanine Aminotransferase (ALT)",
             50878: "Asparate Aminotransferase (AST)",
             225651: "Direct Bilirubin",
             50867: "Amylase",
@@ -54,45 +54,45 @@
             51265: "Platelet Count",
             51248: "MCH",
             51250: "MCV",
             51249: "MCHC",
             50912: "Creatinine",
             50920: "Estimated GFR (MDRD equation)"
         }
-    diagnoses_and_ssir = pd.read_csv(diagnoses_and_ssir_csv)
+    diagnoses_and_ssir = pd.read_csv(merge_with)
     blood = pd.read_csv(blood_csv)
-    chartevents = pd.read_csv(chartevents_csv)
+    chartevents = pd.read_csv(get_data_from)
 
-    blood['analysis_name'] = blood[itemid_column].map(analysis_names)
+    blood['analysis_name'] = blood[itemid_column].map(analyzes_names)
 
-    pivot_values_blood = blood.pivot_table(index=[subject_id_column, charttime_column], columns='analysis_name',
+    pivot_values_blood = blood.pivot_table(index=[subject_id_column, time_column], columns='analysis_name',
                                            values='value',
                                            aggfunc='first').reset_index()
-    pivot_uom_blood = blood.pivot_table(index=[subject_id_column, charttime_column], columns='analysis_name',
+    pivot_uom_blood = blood.pivot_table(index=[subject_id_column, time_column], columns='analysis_name',
                                         values= valueuom_column,
                                         aggfunc='first').reset_index()
-    chartevents_itemids = analysis_names
+    chartevents_itemids = analyzes_names
     chartevents['analysis_name'] = chartevents[itemid_column].map(chartevents_itemids)
 
-    pivot_values_chartevents = chartevents.pivot_table(index=[subject_id_column, charttime_column],
+    pivot_values_chartevents = chartevents.pivot_table(index=[subject_id_column, time_column],
                                                        columns='analysis_name',
                                                        values='value', aggfunc='first').reset_index()
-    pivot_uom_chartevents = chartevents.pivot_table(index=[subject_id_column, charttime_column],
+    pivot_uom_chartevents = chartevents.pivot_table(index=[subject_id_column, time_column],
                                                     columns='analysis_name',
                                                     values=valueuom_column, aggfunc='first').reset_index()
 
-    pivot_values = pd.merge(pivot_values_blood, pivot_values_chartevents, on=[subject_id_column, charttime_column],
+    pivot_values = pd.merge(pivot_values_blood, pivot_values_chartevents, on=[subject_id_column, time_column],
                             how='outer')
-    pivot_uom = pd.merge(pivot_uom_blood, pivot_uom_chartevents, on=[subject_id_column, charttime_column], how='outer')
+    pivot_uom = pd.merge(pivot_uom_blood, pivot_uom_chartevents, on=[subject_id_column, time_column], how='outer')
 
-    pivot_uom.columns = [f'{col}_{valueuom_column}' if col not in [subject_id_column, charttime_column] else col for col
+    pivot_uom.columns = [f'{col}_{valueuom_column}' if col not in [subject_id_column, time_column] else col for col
                          in
                          pivot_uom.columns]
-    pivot_df = pd.merge(pivot_values, pivot_uom, on=[subject_id_column, charttime_column], how='left')
-    merged_df = pd.merge(pivot_df, diagnoses_and_ssir, on=[subject_id_column, charttime_column], how='outer')
+    pivot_df = pd.merge(pivot_values, pivot_uom, on=[subject_id_column, time_column], how='left')
+    merged_df = pd.merge(pivot_df, diagnoses_and_ssir, on=[subject_id_column, time_column], how='outer')
     sepsis_info_df = pd.read_csv(sepsis_info_df)
     sepsis_map = sepsis_info_df.set_index(subject_id_column)[has_sepsis_column].to_dict()
     merged_df[has_sepsis_column] = merged_df[subject_id_column].map(sepsis_map)
     unique_patients = merged_df[[subject_id_column, has_sepsis_column]].drop_duplicates()
     grouped_sepsis = unique_patients.groupby(subject_id_column)[has_sepsis_column].agg(['min', 'max'])
     ambiguous_sepsis_patients = grouped_sepsis[grouped_sepsis['min'] != grouped_sepsis['max']].index
     merged_df.loc[merged_df[subject_id_column].isin(ambiguous_sepsis_patients), has_sepsis_column] = False
```

### Comparing `sickness_screening-1.0.0/sickness_screening/compress.py` & `sickness_screening-1.0.1/sickness_screening/compress.py`

 * *Files identical despite different names*

