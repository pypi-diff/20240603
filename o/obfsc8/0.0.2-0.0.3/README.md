# Comparing `tmp/obfsc8-0.0.2.tar.gz` & `tmp/obfsc8-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "obfsc8-0.0.2.tar", last modified: Wed May 22 19:53:08 2024, max compression
+gzip compressed data, was "obfsc8-0.0.3.tar", last modified: Mon Jun  3 09:39:02 2024, max compression
```

## Comparing `obfsc8-0.0.2.tar` & `obfsc8-0.0.3.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 jwbennett  (1000) jwbennett  (1000)        0 2024-05-22 19:53:08.671898 obfsc8-0.0.2/
--rw-r--r--   0 jwbennett  (1000) jwbennett  (1000)     1070 2024-05-22 13:38:11.000000 obfsc8-0.0.2/LICENSE
--rw-r--r--   0 jwbennett  (1000) jwbennett  (1000)      997 2024-05-22 19:53:08.671898 obfsc8-0.0.2/PKG-INFO
--rw-r--r--   0 jwbennett  (1000) jwbennett  (1000)      465 2024-05-22 15:59:14.000000 obfsc8-0.0.2/README.md
--rw-r--r--   0 jwbennett  (1000) jwbennett  (1000)      569 2024-05-22 19:52:45.000000 obfsc8-0.0.2/pyproject.toml
--rw-r--r--   0 jwbennett  (1000) jwbennett  (1000)       38 2024-05-22 19:53:08.671898 obfsc8-0.0.2/setup.cfg
-drwxr-xr-x   0 jwbennett  (1000) jwbennett  (1000)        0 2024-05-22 19:53:08.661898 obfsc8-0.0.2/src/
-drwxr-xr-x   0 jwbennett  (1000) jwbennett  (1000)        0 2024-05-22 19:53:08.661898 obfsc8-0.0.2/src/obfsc8/
--rw-r--r--   0 jwbennett  (1000) jwbennett  (1000)       32 2024-05-22 18:43:04.000000 obfsc8-0.0.2/src/obfsc8/__init__.py
--rw-r--r--   0 jwbennett  (1000) jwbennett  (1000)      545 2024-05-22 13:38:11.000000 obfsc8-0.0.2/src/obfsc8/get_columns_to_be_obfuscated.py
--rw-r--r--   0 jwbennett  (1000) jwbennett  (1000)      537 2024-05-22 13:38:11.000000 obfsc8-0.0.2/src/obfsc8/get_file_object_from_s3_bucket.py
--rw-r--r--   0 jwbennett  (1000) jwbennett  (1000)      893 2024-05-22 13:38:11.000000 obfsc8-0.0.2/src/obfsc8/get_filetype.py
--rw-r--r--   0 jwbennett  (1000) jwbennett  (1000)      766 2024-05-22 13:38:11.000000 obfsc8-0.0.2/src/obfsc8/get_s3_bucket_and_key_names.py
--rw-r--r--   0 jwbennett  (1000) jwbennett  (1000)     1651 2024-05-22 18:43:43.000000 obfsc8-0.0.2/src/obfsc8/obfuscate.py
--rw-r--r--   0 jwbennett  (1000) jwbennett  (1000)     1143 2024-05-22 13:38:11.000000 obfsc8-0.0.2/src/obfsc8/obfuscate_csv_file.py
-drwxr-xr-x   0 jwbennett  (1000) jwbennett  (1000)        0 2024-05-22 19:53:08.671898 obfsc8-0.0.2/src/obfsc8.egg-info/
--rw-r--r--   0 jwbennett  (1000) jwbennett  (1000)      997 2024-05-22 19:53:08.000000 obfsc8-0.0.2/src/obfsc8.egg-info/PKG-INFO
--rw-r--r--   0 jwbennett  (1000) jwbennett  (1000)      623 2024-05-22 19:53:08.000000 obfsc8-0.0.2/src/obfsc8.egg-info/SOURCES.txt
--rw-r--r--   0 jwbennett  (1000) jwbennett  (1000)        1 2024-05-22 19:53:08.000000 obfsc8-0.0.2/src/obfsc8.egg-info/dependency_links.txt
--rw-r--r--   0 jwbennett  (1000) jwbennett  (1000)       13 2024-05-22 19:53:08.000000 obfsc8-0.0.2/src/obfsc8.egg-info/requires.txt
--rw-r--r--   0 jwbennett  (1000) jwbennett  (1000)        7 2024-05-22 19:53:08.000000 obfsc8-0.0.2/src/obfsc8.egg-info/top_level.txt
-drwxr-xr-x   0 jwbennett  (1000) jwbennett  (1000)        0 2024-05-22 19:53:08.671898 obfsc8-0.0.2/test/
--rw-r--r--   0 jwbennett  (1000) jwbennett  (1000)      407 2024-05-22 19:39:04.000000 obfsc8-0.0.2/test/test_get_columns_to_be_obfuscated.py
--rw-r--r--   0 jwbennett  (1000) jwbennett  (1000)      939 2024-05-22 19:39:04.000000 obfsc8-0.0.2/test/test_get_file_object_from_s3_bucket.py
--rw-r--r--   0 jwbennett  (1000) jwbennett  (1000)      820 2024-05-22 19:39:04.000000 obfsc8-0.0.2/test/test_get_filetype.py
--rw-r--r--   0 jwbennett  (1000) jwbennett  (1000)      703 2024-05-22 19:39:04.000000 obfsc8-0.0.2/test/test_get_s3_bucket_and_key_names.py
--rw-r--r--   0 jwbennett  (1000) jwbennett  (1000)     3777 2024-05-22 19:39:04.000000 obfsc8-0.0.2/test/test_obfuscate_csv_file.py
+drwxr-xr-x   0 jwbennett  (1000) jwbennett  (1000)        0 2024-06-03 09:39:02.095473 obfsc8-0.0.3/
+-rw-r--r--   0 jwbennett  (1000) jwbennett  (1000)     1070 2024-05-30 18:53:02.000000 obfsc8-0.0.3/LICENSE
+-rw-r--r--   0 jwbennett  (1000) jwbennett  (1000)     4656 2024-06-03 09:39:02.095473 obfsc8-0.0.3/PKG-INFO
+-rw-r--r--   0 jwbennett  (1000) jwbennett  (1000)     4117 2024-05-30 18:53:02.000000 obfsc8-0.0.3/README.md
+-rw-r--r--   0 jwbennett  (1000) jwbennett  (1000)      576 2024-06-03 09:38:38.000000 obfsc8-0.0.3/pyproject.toml
+-rw-r--r--   0 jwbennett  (1000) jwbennett  (1000)       38 2024-06-03 09:39:02.095473 obfsc8-0.0.3/setup.cfg
+drwxr-xr-x   0 jwbennett  (1000) jwbennett  (1000)        0 2024-06-03 09:39:02.095473 obfsc8-0.0.3/src/
+drwxr-xr-x   0 jwbennett  (1000) jwbennett  (1000)        0 2024-06-03 09:39:02.095473 obfsc8-0.0.3/src/obfsc8/
+-rw-r--r--   0 jwbennett  (1000) jwbennett  (1000)       33 2024-05-30 18:53:02.000000 obfsc8-0.0.3/src/obfsc8/__init__.py
+-rw-r--r--   0 jwbennett  (1000) jwbennett  (1000)      893 2024-05-30 18:53:02.000000 obfsc8-0.0.3/src/obfsc8/get_columns_to_be_obfuscated.py
+-rw-r--r--   0 jwbennett  (1000) jwbennett  (1000)      537 2024-05-30 18:53:02.000000 obfsc8-0.0.3/src/obfsc8/get_file_object_from_s3_bucket.py
+-rw-r--r--   0 jwbennett  (1000) jwbennett  (1000)      938 2024-05-30 18:53:02.000000 obfsc8-0.0.3/src/obfsc8/get_filetype.py
+-rw-r--r--   0 jwbennett  (1000) jwbennett  (1000)      766 2024-05-30 18:53:02.000000 obfsc8-0.0.3/src/obfsc8/get_s3_bucket_and_key_names.py
+-rw-r--r--   0 jwbennett  (1000) jwbennett  (1000)     2211 2024-05-30 18:53:02.000000 obfsc8-0.0.3/src/obfsc8/obfuscate.py
+-rw-r--r--   0 jwbennett  (1000) jwbennett  (1000)     1143 2024-05-30 18:53:02.000000 obfsc8-0.0.3/src/obfsc8/obfuscate_csv_file.py
+-rw-r--r--   0 jwbennett  (1000) jwbennett  (1000)     1207 2024-05-30 18:53:02.000000 obfsc8-0.0.3/src/obfsc8/obfuscate_parquet_file.py
+drwxr-xr-x   0 jwbennett  (1000) jwbennett  (1000)        0 2024-06-03 09:39:02.095473 obfsc8-0.0.3/src/obfsc8.egg-info/
+-rw-r--r--   0 jwbennett  (1000) jwbennett  (1000)     4656 2024-06-03 09:39:02.000000 obfsc8-0.0.3/src/obfsc8.egg-info/PKG-INFO
+-rw-r--r--   0 jwbennett  (1000) jwbennett  (1000)      696 2024-06-03 09:39:02.000000 obfsc8-0.0.3/src/obfsc8.egg-info/SOURCES.txt
+-rw-r--r--   0 jwbennett  (1000) jwbennett  (1000)        1 2024-06-03 09:39:02.000000 obfsc8-0.0.3/src/obfsc8.egg-info/dependency_links.txt
+-rw-r--r--   0 jwbennett  (1000) jwbennett  (1000)       13 2024-06-03 09:39:02.000000 obfsc8-0.0.3/src/obfsc8.egg-info/requires.txt
+-rw-r--r--   0 jwbennett  (1000) jwbennett  (1000)        7 2024-06-03 09:39:02.000000 obfsc8-0.0.3/src/obfsc8.egg-info/top_level.txt
+drwxr-xr-x   0 jwbennett  (1000) jwbennett  (1000)        0 2024-06-03 09:39:02.095473 obfsc8-0.0.3/test/
+-rw-r--r--   0 jwbennett  (1000) jwbennett  (1000)     1072 2024-05-30 18:53:02.000000 obfsc8-0.0.3/test/test_get_columns_to_be_obfuscated.py
+-rw-r--r--   0 jwbennett  (1000) jwbennett  (1000)      302 2024-05-30 18:53:02.000000 obfsc8-0.0.3/test/test_get_file_object_from_s3_bucket.py
+-rw-r--r--   0 jwbennett  (1000) jwbennett  (1000)     1080 2024-05-30 18:53:02.000000 obfsc8-0.0.3/test/test_get_filetype.py
+-rw-r--r--   0 jwbennett  (1000) jwbennett  (1000)      710 2024-05-30 18:53:02.000000 obfsc8-0.0.3/test/test_get_s3_bucket_and_key_names.py
+-rw-r--r--   0 jwbennett  (1000) jwbennett  (1000)     3660 2024-05-30 18:53:02.000000 obfsc8-0.0.3/test/test_obfuscate_csv_file.py
+-rw-r--r--   0 jwbennett  (1000) jwbennett  (1000)     2001 2024-05-30 18:53:02.000000 obfsc8-0.0.3/test/test_obfuscate_parquet_file.py
```

### Comparing `obfsc8-0.0.2/LICENSE` & `obfsc8-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `obfsc8-0.0.2/pyproject.toml` & `obfsc8-0.0.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "obfsc8"
-version = "0.0.2"
-description = "Easy obfuscation of Personally Identifiable Information (PII) within CSV files"
+version = "0.0.3"
+description = "Easy obfuscation of Personally Identifiable Information (PII) within Amazon S3 files"
 classifiers = ["License :: OSI Approved :: MIT License"]
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.10"
 dependencies = [
     "boto3",
     "polars",
 ]
 
 [project.urls]
 Homepage = "https://github.com/jambent/gdpr_obfuscator"
```

### Comparing `obfsc8-0.0.2/src/obfsc8/get_file_object_from_s3_bucket.py` & `obfsc8-0.0.3/src/obfsc8/get_file_object_from_s3_bucket.py`

 * *Files identical despite different names*

### Comparing `obfsc8-0.0.2/src/obfsc8/get_filetype.py` & `obfsc8-0.0.3/src/obfsc8/get_filetype.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,26 +5,26 @@
     Args:
         filename: target filename
     Returns:
         String of filetype
     Raises:
         TypeError if filename is not a string
         ValueError if filename does not contain a period
-        ValueError if determined filetype is not CSV
+        ValueError if determined filetype is not CSV or Parquet
     """
     if not isinstance(filename, str):
         raise TypeError('Input filename must be a string')
     if '.' not in filename:
         raise ValueError('Input filename must contain a period')
 
     try:
         filename_split_on_period = filename.split('.')
         filetype = filename_split_on_period[-1]
 
     except Exception as e:
         print(f'Failed to extract filetype from filename: {e}')
 
-    if filetype not in ['csv']:
-        raise ValueError(
-            f'Filetype {filetype} not recognised.  Filetype must be CSV.')
+    if filetype not in ['csv', 'parquet']:
+        raise ValueError(f'''Filetype {filetype} not recognised.  \
+                   Filetype must be CSV or Parquet.''')
 
     return filetype
```

### Comparing `obfsc8-0.0.2/src/obfsc8/get_s3_bucket_and_key_names.py` & `obfsc8-0.0.3/src/obfsc8/get_s3_bucket_and_key_names.py`

 * *Files identical despite different names*

### Comparing `obfsc8-0.0.2/src/obfsc8/obfuscate.py` & `obfsc8-0.0.3/src/obfsc8/obfuscate.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,41 +2,55 @@
     import get_s3_bucket_and_key_names
 from .get_file_object_from_s3_bucket \
     import get_file_object_from_s3_bucket
 from .get_filetype import get_filetype
 from .get_columns_to_be_obfuscated \
     import get_columns_to_be_obfuscated
 from .obfuscate_csv_file import obfuscate_csv_file
+from .obfuscate_parquet_file import obfuscate_parquet_file
 
 
-def obfuscate(input_json, replacement_string="***"):
+def obfuscate(input_json, restricted_fields=[], replacement_string="***"):
     """
-    Replaces all values within specified column/s, in file loaded from
-    S3 bucket, with single replacement string, and writes resulting file
-    in the same file format as a streamable object
+    Replaces all values within specified column/s, in CSV or Parquet file
+    loaded from S3 bucket, with single replacement string, and writes
+    resulting file in the same file format as a streamable object
 
     Args:
         input_json: JSON string detailing "file_to_obfuscate" and "pii_fields"
         , e.g.,
         '{
         "file_to_obfuscate": "s3://my_ingestion_bucket/new_data/file1.csv",
         "pii_fields": ["name", "email_address"]
         }'
 
+        restricted_fields: list of fields that cannot be overwritten,
+                            regardless of contents of input_json (default = [])
+
         replacement_string: string to be used to replace all values in the
                             specified PII fields (default = "***")
     Returns:
         BytesIO object containing obfuscated file data
     """
 
     s3_bucket_name, s3_key_name = get_s3_bucket_and_key_names(input_json)
     retrieved_file_object = (get_file_object_from_s3_bucket
                              (s3_bucket_name, s3_key_name))
     filetype = get_filetype(s3_key_name)
-    columns_to_be_obfuscated = get_columns_to_be_obfuscated(input_json)
+    columns_to_be_obfuscated = (get_columns_to_be_obfuscated
+                                (input_json, restricted_fields))
 
     if filetype == "csv":
         transformed_file_data = (obfuscate_csv_file(retrieved_file_object,
                                                     columns_to_be_obfuscated,
                                                     replacement_string))
 
         return transformed_file_data
+
+    elif filetype == 'parquet':
+        transformed_file_data = (
+            obfuscate_parquet_file(
+                retrieved_file_object,
+                columns_to_be_obfuscated,
+                replacement_string))
+
+        return transformed_file_data
```

### Comparing `obfsc8-0.0.2/src/obfsc8/obfuscate_csv_file.py` & `obfsc8-0.0.3/src/obfsc8/obfuscate_csv_file.py`

 * *Files identical despite different names*

### Comparing `obfsc8-0.0.2/src/obfsc8.egg-info/SOURCES.txt` & `obfsc8-0.0.3/src/obfsc8.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -4,17 +4,19 @@
 src/obfsc8/__init__.py
 src/obfsc8/get_columns_to_be_obfuscated.py
 src/obfsc8/get_file_object_from_s3_bucket.py
 src/obfsc8/get_filetype.py
 src/obfsc8/get_s3_bucket_and_key_names.py
 src/obfsc8/obfuscate.py
 src/obfsc8/obfuscate_csv_file.py
+src/obfsc8/obfuscate_parquet_file.py
 src/obfsc8.egg-info/PKG-INFO
 src/obfsc8.egg-info/SOURCES.txt
 src/obfsc8.egg-info/dependency_links.txt
 src/obfsc8.egg-info/requires.txt
 src/obfsc8.egg-info/top_level.txt
 test/test_get_columns_to_be_obfuscated.py
 test/test_get_file_object_from_s3_bucket.py
 test/test_get_filetype.py
 test/test_get_s3_bucket_and_key_names.py
-test/test_obfuscate_csv_file.py
+test/test_obfuscate_csv_file.py
+test/test_obfuscate_parquet_file.py
```

### Comparing `obfsc8-0.0.2/test/test_get_filetype.py` & `obfsc8-0.0.3/test/test_get_filetype.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,39 @@
 import pytest
 
-from src.obfsc8.get_filetype import get_filetype
-
-filename = "new_data/file1.csv"
+from obfsc8.src.obfsc8.get_filetype import get_filetype
 
 
 def test_that_string_returned():
+    filename = "new_data/file1.csv"
     result = get_filetype(filename)
 
     assert isinstance(result, str)
 
 
 def test_that_csv_returned_with_csv_file_input():
-    result = get_filetype(filename)
+    csv_filename = "new_data/file1.csv"
+    result = get_filetype(csv_filename)
 
     assert result == "csv"
 
 
+def test_that_parquet_returned_with_parquet_file_input():
+    parquet_filename = "new_data/file1.parquet"
+    result = get_filetype(parquet_filename)
+
+    assert result == "parquet"
+
+
 def test_that_type_error_raised_if_input_filename_not_a_string():
     with pytest.raises(TypeError, match="must be a string"):
         get_filetype(674)
 
 
 def test_that_value_error_raised_if_period_not_present_in_filename():
     with pytest.raises(ValueError, match="must contain a period"):
         get_filetype("new_data/file1")
 
 
-def test_that_value_error_raised_if_filetype_not_CSV():
-    with pytest.raises(ValueError, match="Filetype must be CSV"):
+def test_that_value_error_raised_if_filetype_not_CSV_or_Parquet():
+    with pytest.raises(ValueError, match="Filetype must be CSV or Parquet"):
         get_filetype("new_data/file1.jpg")
```

### Comparing `obfsc8-0.0.2/test/test_get_s3_bucket_and_key_names.py` & `obfsc8-0.0.3/test/test_get_s3_bucket_and_key_names.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from src.obfsc8.get_s3_bucket_and_key_names \
+from obfsc8.src.obfsc8.get_s3_bucket_and_key_names \
     import get_s3_bucket_and_key_names
 from test_data.test_json import test_json
 
 
 def test_that_2_strings_returned():
     s3_bucket, s3_key = get_s3_bucket_and_key_names(test_json)
```

