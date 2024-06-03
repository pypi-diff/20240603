# Comparing `tmp/ng_data_pipelines_sdk-1.7.1.tar.gz` & `tmp/ng_data_pipelines_sdk-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ng_data_pipelines_sdk-1.7.1.tar", max compression
+gzip compressed data, was "ng_data_pipelines_sdk-1.8.0.tar", max compression
```

## Comparing `ng_data_pipelines_sdk-1.7.1.tar` & `ng_data_pipelines_sdk-1.8.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      106 2024-05-27 11:34:39.711501 ng_data_pipelines_sdk-1.7.1/README.md
--rw-r--r--   0        0        0        0 2024-05-27 11:34:39.747501 ng_data_pipelines_sdk-1.7.1/ng_data_pipelines_sdk/__init__.py
--rw-r--r--   0        0        0     9155 2024-05-27 11:34:39.712501 ng_data_pipelines_sdk-1.7.1/ng_data_pipelines_sdk/aws_interface.py
--rw-r--r--   0        0        0      231 2024-05-27 11:34:39.712501 ng_data_pipelines_sdk-1.7.1/ng_data_pipelines_sdk/custom_logger.py
--rw-r--r--   0        0        0    28037 2024-05-27 11:34:39.712501 ng_data_pipelines_sdk-1.7.1/ng_data_pipelines_sdk/dataframe_manager.py
--rw-r--r--   0        0        0    22122 2024-05-27 11:34:39.712501 ng_data_pipelines_sdk-1.7.1/ng_data_pipelines_sdk/interfaces.py
--rw-r--r--   0        0        0     5406 2024-05-27 11:34:39.712501 ng_data_pipelines_sdk-1.7.1/ng_data_pipelines_sdk/spark_manager.py
--rw-r--r--   0        0        0     4780 2024-05-27 11:34:39.712501 ng_data_pipelines_sdk-1.7.1/ng_data_pipelines_sdk/utils.py
--rw-r--r--   0        0        0      838 2024-05-27 11:34:39.715501 ng_data_pipelines_sdk-1.7.1/pyproject.toml
--rw-r--r--   0        0        0      884 1970-01-01 00:00:00.000000 ng_data_pipelines_sdk-1.7.1/PKG-INFO
+-rw-r--r--   0        0        0      106 2024-06-03 13:34:21.295095 ng_data_pipelines_sdk-1.8.0/README.md
+-rw-r--r--   0        0        0        0 2024-06-03 13:34:21.330096 ng_data_pipelines_sdk-1.8.0/ng_data_pipelines_sdk/__init__.py
+-rw-r--r--   0        0        0     9155 2024-06-03 13:34:21.295095 ng_data_pipelines_sdk-1.8.0/ng_data_pipelines_sdk/aws_interface.py
+-rw-r--r--   0        0        0      231 2024-06-03 13:34:21.295095 ng_data_pipelines_sdk-1.8.0/ng_data_pipelines_sdk/custom_logger.py
+-rw-r--r--   0        0        0    28134 2024-06-03 13:34:21.295095 ng_data_pipelines_sdk-1.8.0/ng_data_pipelines_sdk/dataframe_manager.py
+-rw-r--r--   0        0        0    22122 2024-06-03 13:34:21.296095 ng_data_pipelines_sdk-1.8.0/ng_data_pipelines_sdk/interfaces.py
+-rw-r--r--   0        0        0     5406 2024-06-03 13:34:21.296095 ng_data_pipelines_sdk-1.8.0/ng_data_pipelines_sdk/spark_manager.py
+-rw-r--r--   0        0        0     4780 2024-06-03 13:34:21.296095 ng_data_pipelines_sdk-1.8.0/ng_data_pipelines_sdk/utils.py
+-rw-r--r--   0        0        0      838 2024-06-03 13:34:21.299095 ng_data_pipelines_sdk-1.8.0/pyproject.toml
+-rw-r--r--   0        0        0      884 1970-01-01 00:00:00.000000 ng_data_pipelines_sdk-1.8.0/PKG-INFO
```

### Comparing `ng_data_pipelines_sdk-1.7.1/ng_data_pipelines_sdk/aws_interface.py` & `ng_data_pipelines_sdk-1.8.0/ng_data_pipelines_sdk/aws_interface.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-1.7.1/ng_data_pipelines_sdk/dataframe_manager.py` & `ng_data_pipelines_sdk-1.8.0/ng_data_pipelines_sdk/dataframe_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -312,29 +312,27 @@
         Returns:
             None
         """
         bucket_url = self._get_bucket_url(output_df_params.dataframe_bucket_params)
         write_base_path_url = f"{bucket_url}/{output_df_params.dataframe_base_path}"
         logger.debug(f"Write base path: {write_base_path_url}")
 
-        write_info =  f"Writing DataFrame to base path {write_base_path_url}"
+        write_info = f"Writing DataFrame to base path {write_base_path_url}"
         if output_df_params.partition_by:
             write_info += f" with partitions {output_df_params.partition_by}"
         else:
             write_info += " without partitions"
 
         df_to_write = df
         if output_df_params.single_write_date_params:
             date_partition_path = ""
             for (
                 date_partition,
                 date_partition_name,
-            ) in (
-                output_df_params.single_write_date_params.single_write_date_partitions.items()
-            ):
+            ) in output_df_params.single_write_date_params.single_write_date_partitions.items():
                 formatted_date_part_value = DATE_FORMATTER[date_partition.value](
                     output_df_params.single_write_date_params.single_write_date
                 )
                 # Add the date partition column to the DataFrame
                 df_to_write = df_to_write.withColumn(
                     date_partition_name, lit(formatted_date_part_value)
                 )
@@ -525,30 +523,35 @@
         self, step_params: StepParams, processing_date: datetime
     ) -> None:
         for _, df_params in step_params.input_dataframes_params.items():
             if df_params.read_date_params:
                 df_params.read_date_params.was_offset_applied = False
 
                 if df_params.read_date_params.read_dates == "{{processing_date}}":
-                    df_params.read_date_params.read_dates = processing_date
-
                     offset = df_params.read_date_params.processing_date_offset_days
+
                     if offset and offset != 0:
-                        df_params.read_date_params.read_dates
-                        +timedelta(days=offset)
+                        df_params.read_date_params.read_dates = (
+                            processing_date + timedelta(days=offset)
+                        )
                         df_params.read_date_params.was_offset_applied = True
+                    else:
+                        df_params.read_date_params.read_dates = processing_date
+
 
         if step_params.output_dataframes_params:
             for _, df_params in step_params.output_dataframes_params.items():
                 if (
                     df_params.single_write_date_params
                     and df_params.single_write_date_params.single_write_date
                     == "{{processing_date}}"
                 ):
-                    df_params.single_write_date_params.single_write_date = processing_date
+                    df_params.single_write_date_params.single_write_date = (
+                        processing_date
+                    )
 
     def process_step(
         self,
         step_params_json_file_path: Optional[str] = None,
         step_params: Optional[StepParams] = None,
         processing_date: Optional[datetime] = None,
         write_output_dfs: bool = True,
```

### Comparing `ng_data_pipelines_sdk-1.7.1/ng_data_pipelines_sdk/interfaces.py` & `ng_data_pipelines_sdk-1.8.0/ng_data_pipelines_sdk/interfaces.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-1.7.1/ng_data_pipelines_sdk/spark_manager.py` & `ng_data_pipelines_sdk-1.8.0/ng_data_pipelines_sdk/spark_manager.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-1.7.1/ng_data_pipelines_sdk/utils.py` & `ng_data_pipelines_sdk-1.8.0/ng_data_pipelines_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-1.7.1/pyproject.toml` & `ng_data_pipelines_sdk-1.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ng-data-pipelines-sdk"
-version = "1.7.1"
+version = "1.8.0"
 description = "A library for interacting with data from Amazon S3 through PySpark. Read, write and tranform data using a powerful and intuitive API with strong consistency and type checking, thanks to Pydantic. Compatible with Amazon MWAA running Airflow 2.7.2 and 2.8.1."
 authors = ["ng.cash"]
 readme = "README.md"
 exclude = [".git/", ".gitignore", "tests/", "docs/", "*.yml", "__pycache__/", "*.pyc", "*.ipynb", "playground/", "poetry.lock", "dist/", "build/"]
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.12"
```

### Comparing `ng_data_pipelines_sdk-1.7.1/PKG-INFO` & `ng_data_pipelines_sdk-1.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ng-data-pipelines-sdk
-Version: 1.7.1
+Version: 1.8.0
 Summary: A library for interacting with data from Amazon S3 through PySpark. Read, write and tranform data using a powerful and intuitive API with strong consistency and type checking, thanks to Pydantic. Compatible with Amazon MWAA running Airflow 2.7.2 and 2.8.1.
 Author: ng.cash
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

