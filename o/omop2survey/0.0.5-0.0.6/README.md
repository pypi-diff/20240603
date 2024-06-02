# Comparing `tmp/omop2survey-0.0.5.tar.gz` & `tmp/omop2survey-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omop2survey-0.0.5.tar", max compression
+gzip compressed data, was "omop2survey-0.0.6.tar", max compression
```

## Comparing `omop2survey-0.0.5.tar` & `omop2survey-0.0.6.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     5464 2024-05-19 23:44:34.164594 omop2survey-0.0.5/README.md
--rw-r--r--   0        0        0     6148 2024-05-17 04:16:32.815544 omop2survey-0.0.5/omop2survey/.DS_Store
--rw-r--r--   0        0        0      323 2024-05-17 04:52:20.337967 omop2survey-0.0.5/omop2survey/__init__.py
--rw-r--r--   0        0        0     6058 2024-05-17 04:52:20.338391 omop2survey-0.0.5/omop2survey/codebooks.py
--rw-r--r--   0        0        0      571 2024-05-17 04:52:20.338656 omop2survey-0.0.5/omop2survey/hash_csv.py
--rw-r--r--   0        0        0     2800 2024-05-17 04:52:20.338900 omop2survey-0.0.5/omop2survey/pivot_data.py
--rw-r--r--   0        0        0      872 2024-05-17 03:49:20.928260 omop2survey-0.0.5/omop2survey/recode_missing.py
--rw-r--r--   0        0        0    10229 2024-05-20 00:05:36.987436 omop2survey-0.0.5/omop2survey/response_set.py
--rw-r--r--   0        0        0  1172489 2024-05-10 03:42:23.460428 omop2survey-0.0.5/omop2survey/survey_key.csv
--rw-r--r--   0        0        0       64 2024-05-17 04:52:20.339780 omop2survey-0.0.5/omop2survey/survey_key_hash.txt
--rw-r--r--   0        0        0      828 2024-05-19 23:32:17.602826 omop2survey-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     6483 1970-01-01 00:00:00.000000 omop2survey-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     5367 2024-05-31 02:06:28.786619 omop2survey-0.0.6/README.md
+-rw-r--r--   0        0        0     6148 2024-05-17 04:16:32.815544 omop2survey-0.0.6/omop2survey/.DS_Store
+-rw-r--r--   0        0        0      323 2024-05-17 04:52:20.337967 omop2survey-0.0.6/omop2survey/__init__.py
+-rw-r--r--   0        0        0     6058 2024-05-17 04:52:20.338391 omop2survey-0.0.6/omop2survey/codebooks.py
+-rw-r--r--   0        0        0      571 2024-05-17 04:52:20.338656 omop2survey-0.0.6/omop2survey/hash_csv.py
+-rw-r--r--   0        0        0     2800 2024-05-17 04:52:20.338900 omop2survey-0.0.6/omop2survey/pivot_data.py
+-rw-r--r--   0        0        0     1877 2024-06-02 15:33:38.256012 omop2survey-0.0.6/omop2survey/recode_missing.py
+-rw-r--r--   0        0        0    11055 2024-06-02 18:53:45.616670 omop2survey-0.0.6/omop2survey/response_set.py
+-rw-r--r--   0        0        0     2068 2024-06-02 17:24:13.641687 omop2survey-0.0.6/omop2survey/subset.py
+-rw-r--r--   0        0        0  1172489 2024-05-10 03:42:23.460428 omop2survey-0.0.6/omop2survey/survey_key.csv
+-rw-r--r--   0        0        0       64 2024-05-17 04:52:20.339780 omop2survey-0.0.6/omop2survey/survey_key_hash.txt
+-rw-r--r--   0        0        0      851 2024-06-02 17:21:33.397460 omop2survey-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     6431 1970-01-01 00:00:00.000000 omop2survey-0.0.6/PKG-INFO
```

### Comparing `omop2survey-0.0.5/README.md` & `omop2survey-0.0.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 The **'omop2survey'** Python package offers a comprehensive solution for transforming standardized response codes from the Observational Medical Outcomes Partnership (OMOP) Common Data Model (CDM) survey variables into numeric values, streamlining the data preparation process. By automating the mapping and conversion of response codes, as well as the handling of missing data, it makes data analysis more accessible and reliable. The package provides a range of functions designed to help researchers and data analysts efficiently work through OMOP CDM survey data, ensuring accurate mappings of responses and effective management of data discrepancies. This package is a helpful tool for those working with OMOP CDM survey data, offering a path to more profound and accurate analyses by dramatically lowering the burden of data preprocessing.
 
-The content of Python files in the package can be found below. For examples of how to use the package, see **example.py** for Python and **exampleR.Rmd** for R.
+The content of Python files in the package can be found below. 
 
 ### response_set.py
 
 >
 >**map_answers(input_data)**: Maps survey responses to corresponding numeric and text values, and handles survey responses that fall outside the predefined cases.
 > 
 > Parameters:
```

### Comparing `omop2survey-0.0.5/omop2survey/.DS_Store` & `omop2survey-0.0.6/omop2survey/.DS_Store`

 * *Files identical despite different names*

### Comparing `omop2survey-0.0.5/omop2survey/codebooks.py` & `omop2survey-0.0.6/omop2survey/codebooks.py`

 * *Files identical despite different names*

### Comparing `omop2survey-0.0.5/omop2survey/hash_csv.py` & `omop2survey-0.0.6/omop2survey/hash_csv.py`

 * *Files identical despite different names*

### Comparing `omop2survey-0.0.5/omop2survey/pivot_data.py` & `omop2survey-0.0.6/omop2survey/pivot_data.py`

 * *Files identical despite different names*

### Comparing `omop2survey-0.0.5/omop2survey/response_set.py` & `omop2survey-0.0.6/omop2survey/response_set.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,14 +62,15 @@
         if pd.isna(answer_id) and pd.notna(row['answer']) and str(row['answer']).isdigit():
             input_data.at[idx, 'answer_numeric'] = int(row['answer'])
             input_data.at[idx, 'answer_text'] = str(row['answer'])
 
         if isinstance(input_data.at[idx, 'answer_text'], (int, float)):
             input_data.at[idx, 'answer_text'] = str(input_data.at[idx, 'answer_text'])
 
+    print(f"The number of unique person_ids in the dataset: {input_data['person_id'].nunique()}")
     return input_data
 
 
 def create_dummies(user_data):
     question_key = load_survey_data()
 
     select_all_questions = question_key[question_key['select_all'] == 1]['question_concept_id'].unique()
@@ -177,14 +178,15 @@
     result = input_data.apply(apply_mappings, axis=1, result_type='expand')
     input_data[['answer_numeric', 'answer_text']] = result
 
     numeric_mask = pd.isna(input_data['answer_concept_id']) & input_data['answer'].apply(lambda x: str(x).isdigit())
     input_data.loc[numeric_mask, 'answer_numeric'] = input_data.loc[numeric_mask, 'answer'].astype(int)
     input_data.loc[numeric_mask, 'answer_text'] = input_data.loc[numeric_mask, 'answer'].astype(str)
 
+    print(f"The number of unique person_ids in the dataset: {input_data['person_id'].nunique()}")
     return input_data
 
 
 def map_items(input_data):
     special_cases = {
         903087: (-999, "Don't Know"),
         903096: (-998, "Skip"),
@@ -210,23 +212,32 @@
         43529089: (-997, "No Blood Related Daughters"),
         43529086: (-997, "No Blood Related Siblings"),
         43529092: (-997, "No Blood Related Sons"),
         43529090: (-997, "No Daughters Related")
     }
 
     survey_data = load_survey_data()
+    survey_data['question_concept_id_copy'] = survey_data['question_concept_id']
 
-    mapping_numeric = survey_data.groupby('question_concept_id').apply(
-        lambda g: g.set_index('answer_concept_id')['answer_numeric'].to_dict()
+    mapping_numeric = survey_data.groupby('question_concept_id_copy', group_keys=False).apply(
+        lambda g: g.set_index('answer_concept_id')['answer_numeric'].to_dict(), include_groups= False
     ).to_dict()
 
-    mapping_text = survey_data.groupby('question_concept_id').apply(
-        lambda g: g.set_index('answer_concept_id')['answer_text'].str.strip().to_dict()
+    mapping_text = survey_data.groupby('question_concept_id_copy', group_keys=False).apply(
+        lambda g: g.set_index('answer_concept_id')['answer_text'].str.strip().to_dict(), include_groups= False
     ).to_dict()
 
+    # mapping_numeric = survey_data.groupby('question_concept_id').apply(
+    #     lambda g: g.set_index('answer_concept_id')['answer_numeric'].to_dict()
+    # ).to_dict()
+    #
+    # mapping_text = survey_data.groupby('question_concept_id').apply(
+    #     lambda g: g.set_index('answer_concept_id')['answer_text'].str.strip().to_dict()
+    # ).to_dict()
+
     input_data['answer_numeric'] = pd.NA
     input_data['answer_text'] = pd.NA
 
     for answer_id, (num, text) in special_cases.items():
         mask = input_data['answer_concept_id'] == answer_id
         input_data.loc[mask, 'answer_numeric'] = num
         input_data.loc[mask, 'answer_text'] = text
@@ -245,9 +256,10 @@
         lambda row: pd.Series(apply_mappings(row)), axis=1
     )
 
     numeric_mask = pd.isna(input_data['answer_concept_id']) & input_data['answer'].apply(lambda x: str(x).isdigit())
     input_data.loc[numeric_mask, 'answer_numeric'] = input_data.loc[numeric_mask, 'answer'].astype(int)
     input_data.loc[numeric_mask, 'answer_text'] = input_data.loc[numeric_mask, 'answer'].astype(str)
 
+    print(f"The number of unique person_ids in the dataset: {input_data['person_id'].nunique()}")
     return input_data
```

### Comparing `omop2survey-0.0.5/omop2survey/survey_key.csv` & `omop2survey-0.0.6/omop2survey/survey_key.csv`

 * *Files identical despite different names*

### Comparing `omop2survey-0.0.5/pyproject.toml` & `omop2survey-0.0.6/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [tool.poetry]
 name = "omop2survey"
-version = "0.0.5"
+version = "0.0.6"
 description = "The 'omop2survey' Python package transforms standardized response codes from the OMOP CDM survey variables into numeric values and simplifies data preparation by providing functionalities for mapping and converting response codes, as well as handling missing data, facilitating easier and more reliable data analysis."
 authors = ["Elif Dede Yildirim <elifdy@auburn.edu>"]
 repository = "https://github.com/elifdy/omop2survey.git"
 license = "MIT"
 readme = "README.md"
 include = ["omop2survey/survey_key.csv"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pandas = "^2.2.2"
 tabulate = "^0.9.0"
 openpyxl = "^3.1.2"
+pandas-gbq = "^0.17.9"
 
 
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `omop2survey-0.0.5/PKG-INFO` & `omop2survey-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: omop2survey
-Version: 0.0.5
+Version: 0.0.6
 Summary: The 'omop2survey' Python package transforms standardized response codes from the OMOP CDM survey variables into numeric values and simplifies data preparation by providing functionalities for mapping and converting response codes, as well as handling missing data, facilitating easier and more reliable data analysis.
 Home-page: https://github.com/elifdy/omop2survey.git
 License: MIT
 Author: Elif Dede Yildirim
 Author-email: elifdy@auburn.edu
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: pandas (>=2.2.2,<3.0.0)
+Requires-Dist: pandas-gbq (>=0.17.9,<0.18.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Project-URL: Repository, https://github.com/elifdy/omop2survey.git
 Description-Content-Type: text/markdown
 
 
 The **'omop2survey'** Python package offers a comprehensive solution for transforming standardized response codes from the Observational Medical Outcomes Partnership (OMOP) Common Data Model (CDM) survey variables into numeric values, streamlining the data preparation process. By automating the mapping and conversion of response codes, as well as the handling of missing data, it makes data analysis more accessible and reliable. The package provides a range of functions designed to help researchers and data analysts efficiently work through OMOP CDM survey data, ensuring accurate mappings of responses and effective management of data discrepancies. This package is a helpful tool for those working with OMOP CDM survey data, offering a path to more profound and accurate analyses by dramatically lowering the burden of data preprocessing.
 
-The content of Python files in the package can be found below. For examples of how to use the package, see **example.py** for Python and **exampleR.Rmd** for R.
+The content of Python files in the package can be found below. 
 
 ### response_set.py
 
 >
 >**map_answers(input_data)**: Maps survey responses to corresponding numeric and text values, and handles survey responses that fall outside the predefined cases.
 > 
 > Parameters:
```

