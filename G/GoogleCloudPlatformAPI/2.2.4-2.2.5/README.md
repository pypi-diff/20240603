# Comparing `tmp/googlecloudplatformapi-2.2.4.tar.gz` & `tmp/googlecloudplatformapi-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "googlecloudplatformapi-2.2.4.tar", last modified: Thu May 30 15:05:01 2024, max compression
+gzip compressed data, was "googlecloudplatformapi-2.2.5.tar", last modified: Mon Jun  3 09:52:58 2024, max compression
```

## Comparing `googlecloudplatformapi-2.2.4.tar` & `googlecloudplatformapi-2.2.5.tar`

### file list

```diff
@@ -1,20 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:05:01.191957 googlecloudplatformapi-2.2.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:05:01.187957 googlecloudplatformapi-2.2.4/GoogleCloudPlatformAPI/
--rw-r--r--   0 runner    (1001) docker     (127)    35674 2024-05-30 15:04:56.000000 googlecloudplatformapi-2.2.4/GoogleCloudPlatformAPI/AdManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4688 2024-05-30 15:04:56.000000 googlecloudplatformapi-2.2.4/GoogleCloudPlatformAPI/Analytics.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    22712 2024-05-30 15:04:56.000000 googlecloudplatformapi-2.2.4/GoogleCloudPlatformAPI/BigQuery.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7227 2024-05-30 15:04:56.000000 googlecloudplatformapi-2.2.4/GoogleCloudPlatformAPI/CloudStorage.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2641 2024-05-30 15:04:56.000000 googlecloudplatformapi-2.2.4/GoogleCloudPlatformAPI/ServiceAccount.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2276 2024-05-30 15:04:56.000000 googlecloudplatformapi-2.2.4/GoogleCloudPlatformAPI/Utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-30 15:04:56.000000 googlecloudplatformapi-2.2.4/GoogleCloudPlatformAPI/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:05:01.187957 googlecloudplatformapi-2.2.4/GoogleCloudPlatformAPI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-30 15:05:01.000000 googlecloudplatformapi-2.2.4/GoogleCloudPlatformAPI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-30 15:05:01.000000 googlecloudplatformapi-2.2.4/GoogleCloudPlatformAPI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 15:05:01.000000 googlecloudplatformapi-2.2.4/GoogleCloudPlatformAPI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-30 15:05:01.000000 googlecloudplatformapi-2.2.4/GoogleCloudPlatformAPI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-30 15:05:01.000000 googlecloudplatformapi-2.2.4/GoogleCloudPlatformAPI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-30 15:04:56.000000 googlecloudplatformapi-2.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-30 15:05:01.187957 googlecloudplatformapi-2.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-30 15:04:56.000000 googlecloudplatformapi-2.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-30 15:04:56.000000 googlecloudplatformapi-2.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 15:05:01.191957 googlecloudplatformapi-2.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:52:58.505121 googlecloudplatformapi-2.2.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:52:58.501121 googlecloudplatformapi-2.2.5/GoogleCloudPlatformAPI/
+-rw-r--r--   0 runner    (1001) docker     (127)    36220 2024-06-03 09:52:51.000000 googlecloudplatformapi-2.2.5/GoogleCloudPlatformAPI/AdManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-06-03 09:52:51.000000 googlecloudplatformapi-2.2.5/GoogleCloudPlatformAPI/Analytics.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19849 2024-06-03 09:52:51.000000 googlecloudplatformapi-2.2.5/GoogleCloudPlatformAPI/BigQuery.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7213 2024-06-03 09:52:51.000000 googlecloudplatformapi-2.2.5/GoogleCloudPlatformAPI/CloudStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-06-03 09:52:51.000000 googlecloudplatformapi-2.2.5/GoogleCloudPlatformAPI/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:52:58.501121 googlecloudplatformapi-2.2.5/GoogleCloudPlatformAPI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-06-03 09:52:58.000000 googlecloudplatformapi-2.2.5/GoogleCloudPlatformAPI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-06-03 09:52:58.000000 googlecloudplatformapi-2.2.5/GoogleCloudPlatformAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 09:52:58.000000 googlecloudplatformapi-2.2.5/GoogleCloudPlatformAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-06-03 09:52:58.000000 googlecloudplatformapi-2.2.5/GoogleCloudPlatformAPI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-06-03 09:52:58.000000 googlecloudplatformapi-2.2.5/GoogleCloudPlatformAPI.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-06-03 09:52:51.000000 googlecloudplatformapi-2.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-06-03 09:52:58.505121 googlecloudplatformapi-2.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-06-03 09:52:51.000000 googlecloudplatformapi-2.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-06-03 09:52:51.000000 googlecloudplatformapi-2.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 09:52:58.505121 googlecloudplatformapi-2.2.5/setup.cfg
```

### Comparing `googlecloudplatformapi-2.2.4/GoogleCloudPlatformAPI/AdManager.py` & `googlecloudplatformapi-2.2.5/GoogleCloudPlatformAPI/AdManager.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,31 +7,31 @@
 import tempfile
 from typing import Dict, List, Literal, Optional, TypedDict, Union
 
 import pandas as pd
 import pytz
 from googleads import ad_manager, errors
 
+from .. import ListHelper
+from . import ServiceAccount
 
-from .ServiceAccount import ServiceAccount
-from .Utils import ListHelper
 
-PYTZ_TIMEZONE='UTC'
+PYTZ_TIMEZONE = 'UTC'
 AD_UNIT_VIEW = 'TOP_LEVEL'
 METRICS = ['TOTAL_CODE_SERVED_COUNT',
            'AD_SERVER_IMPRESSIONS',
            'AD_SERVER_CLICKS',
            'ADSENSE_LINE_ITEM_LEVEL_IMPRESSIONS',
            'ADSENSE_LINE_ITEM_LEVEL_CLICKS',
            'TOTAL_LINE_ITEM_LEVEL_IMPRESSIONS',
            'TOTAL_LINE_ITEM_LEVEL_CPM_AND_CPC_REVENUE']
 
 DIMENSIONS = ['DATE', 'AD_UNIT_NAME', 'CUSTOM_TARGETING_VALUE_ID']
 
-GAM_VERSION = "v202305"
+GAM_VERSION = "v202405"
 NETWORK_CODE = '5574'
 APP_NAME = 'AdManagerAPIClient'
 
 # region objects
 gam_adUnit = Dict[int, bool]
 
 gam_adUnits = List[gam_adUnit]
@@ -107,40 +107,53 @@
     name: str
     targeting: targeting
 # endregion
 
 
 class GamClient(ad_manager.AdManagerClient):
     def __init__(self,
-                 app_name: Optional[str] = APP_NAME,
-                 network_code:  Optional[str] = NETWORK_CODE):
+                 app_name: str = APP_NAME,
+                 network_code:  str = NETWORK_CODE):
+        logging.debug(f'GamClient::__init__::{network_code}')
         oauth2_client = ServiceAccount.get_service_account_client()
         super().__init__(oauth2_client, app_name, network_code=network_code)
 
     def get_service(self, service_name: str, gam_version: str):
+        logging.debug(f'GamClient::get_service::{service_name}::{gam_version}')
         return self.GetService(service_name=service_name,
                                version=gam_version)
 
     def get_data_downloader(self, gam_version: str):
+        logging.debug(f'GamClient::get_data_downloader:{gam_version}')
         return self.GetDataDownloader(version=gam_version)
 
 
 class Audience(GamClient):
     __service_name = 'AudienceSegmentService'
 
     def __init__(self,
                  app_name: str = APP_NAME,
                  network_code:  str = NETWORK_CODE,
                  gam_version: str = GAM_VERSION):
+        logging.debug(
+            f'Audience::__init__:{self.__service_name}::{network_code}::{gam_version}')
         gam_client = GamClient(app_name=app_name,
                                network_code=network_code)
         self.__gam_service = gam_client.get_service(service_name=self.__service_name,
                                                     gam_version=gam_version)
 
-    def create(self, name, description, custom_targeting, pageviews: int = 1, recencydays: int = 1, membershipexpirationdays: int = 90, network_code=NETWORK_CODE):
+    def create(self,
+               name,
+                 description,
+                 custom_targeting,
+                 pageviews: int = 1,
+                 recencydays: int = 1,
+                 membershipexpirationdays: int = 90,
+                 network_code=NETWORK_CODE):
+        logging.debug(f'Audience::create:{name}')
         # Initialize appropriate services.
         network_service = Network(
             app_name=APP_NAME, network_code=network_code)
         # Get the root ad unit ID used to target the entire network.
         root_ad_unit_id = network_service.effectiveRootAdUnitId()
 
         # Create inventory targeting (pointed at root ad unit i.e. the whole network)
@@ -172,14 +185,15 @@
         for created_audience_segment in audience_segments:
             logging.debug('An audience segment with ID "%s", name "%s", and type "%s" '
                          'was created.' % (created_audience_segment['id'],
                                            created_audience_segment['name'],
                                            created_audience_segment['type']))
 
     def list(self):
+        logging.debug( f'Audience::list:{self.__service_name}::{self.network_code}::list')
         # Create a statement to select audience segments.
         statement = (ad_manager.StatementBuilder(version=GAM_VERSION)
                      .Where('Type = :type')
                      .WithBindVariable('type', 'FIRST_PARTY'))
         results = []
         # Retrieve a small amount of audience segments at a time, paging
         # through until all audience segments have been retrieved.
```

### Comparing `googlecloudplatformapi-2.2.4/GoogleCloudPlatformAPI/Analytics.py` & `googlecloudplatformapi-2.2.5/GoogleCloudPlatformAPI/Analytics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import List, Optional
 import logging
 import os
 import pandas as pd
 from googleapiclient.discovery import build
 import datetime
-from .ServiceAccount import ServiceAccount
+from . import ServiceAccount
 
 
 class Analytics():
     SCOPES = ['https://www.googleapis.com/auth/analytics.readonly']
 
     def __init__(self, credentials: Optional[str] = None):
         logging.debug(f"Analytics::__init__")
```

### Comparing `googlecloudplatformapi-2.2.4/GoogleCloudPlatformAPI/BigQuery.py` & `googlecloudplatformapi-2.2.5/GoogleCloudPlatformAPI/BigQuery.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 # python
 import datetime
 import json
 import logging
 import os
 import shutil
 from dataclasses import dataclass
-from typing import List, Optional,Union
+from typing import List, Optional, Union
 import decimal
 
 import pandas as pd
 from google.cloud import bigquery
 from google.cloud.bigquery import (QueryJobConfig,
                                    ScalarQueryParameter)
 from google.cloud.exceptions import NotFound
 
+
+from .. import FileHelper
+from . import ServiceAccount
 from .CloudStorage import CloudStorage
-from .ServiceAccount import ServiceAccount
-from .Utils import FileHelper
 
-DATA_TYPE_MAPPING = {'object': bigquery.enums.SqlTypeNames.STRING, 'int64': bigquery.enums.SqlTypeNames.INT64,
-                     'float64': bigquery.enums.SqlTypeNames.FLOAT, 'bool': bigquery.enums.SqlTypeNames.BOOL}
+DATA_TYPE_MAPPING = {'object': bigquery.enums.SqlTypeNames.STRING,
+                     'int64': bigquery.enums.SqlTypeNames.INT64,
+                     'float64': bigquery.enums.SqlTypeNames.FLOAT,
+                     'bool': bigquery.enums.SqlTypeNames.BOOL}
 
 
 class BigQuery():
     __client: bigquery.Client
     SCOPES = ["https://www.googleapis.com/auth/cloud-platform"]
 
     def __init__(self,
@@ -55,37 +58,39 @@
             return [row for row in self.__client.query(query, job_config=job_config).result()]
         else:
             return [row for row in self.__client.query(query).result()]
 
     @dataclass
     class oSpParam():
         name: str
-        value: Union[str, int, float, decimal.Decimal, bool, datetime.datetime, datetime.date]
+        value: Union[str, int, float, decimal.Decimal,
+                     bool, datetime.datetime, datetime.date]
         type: str
 
     def execute_stored_procedure(self, sp_name: str, sp_params: List[oSpParam]) -> pd.DataFrame:
         logging.debug(f"BigQuery::execute_sp::{sp_name}")
         sp_instruction_params = "@" + ",@".join(
             [sp_param.name for sp_param in sp_params])
 
         query = f"CALL `{sp_name}`({sp_instruction_params})"
         query_parameters = []
         for sp_param in sp_params:
             query_parameters.append(
-                ScalarQueryParameter(sp_param.name, sp_param.type, sp_param.value))  
+                ScalarQueryParameter(sp_param.name, sp_param.type, sp_param.value))
 
         job_config = QueryJobConfig(query_parameters=query_parameters)
         query_results = self.execute_query(query, job_config)
         result_list = []
         for result in query_results:
             t = dict(**result)
             result_list.append(t)
         return pd.DataFrame(result_list)
 
     def table_exists(self, table_id: str) -> bool:
+        logging.debug(f"BigQuery::table_exists::{table_id}")
         try:
             self.__client.get_table(table_id)
             return True
         except NotFound:
             return False
 
     def create_schema_from_table(self, folder: str, dataset: Optional[str] = None) -> Optional[dict]:
@@ -117,19 +122,22 @@
                     schema), destination_blob_name=f"{folder}/schema.json")
             return schema
 
     def create_external_table(self,
                               dataset_name: str,
                               table_name: str,
                               table_schema: dict,
-                              source_uris=List[str]):
+                              source_uris=List[str],
+                              partition_field: str = 'date',
+                              time_partioning: bool = False):
+        logging.debug(f"BigQuery::create_external_table::{table_name}")
         # Configuring the external data source
+
         schema = []
-        partition_field = 'date'
-        time_partioning = False
+
         for field in table_schema['table_schema']:
             bq_field = bigquery.SchemaField(name=field['name'],
                                             field_type=field['type'],
                                             mode=field['mode'])
             if field['name'] == 'report_date':
                 partition_field = 'report_date'
             if field['name'] == partition_field:
@@ -192,16 +200,17 @@
         return False
 
     def load_from_query(self, query: str,
                         table_id: str,
                         write_disposition: bigquery.WriteDisposition = bigquery.WriteDisposition.WRITE_TRUNCATE  # type: ignore
                         ):
         logging.debug(f"BigQuery::load_from_query")
-        job_config = bigquery.QueryJobConfig(
-            destination=table_id, allow_large_results=True, write_disposition=write_disposition)
+        job_config = bigquery.QueryJobConfig(destination=table_id,
+                                             allow_large_results=True,
+                                             write_disposition=write_disposition)
         query_job = self.__client.query(query=query, job_config=job_config)
         query_job.result()  # Wait for the job to complete.
 
         logging.debug("Query results loaded to the table {}".format(table_id))
 
     def delete_partition(self, table_id: str,
                          partition_date: datetime.date,
@@ -287,84 +296,24 @@
                                     local_folder=local_folder,
                                     remote_folder=remote_folder,
                                     partition_date=partition_date,
                                     partition_name=partition_name,
                                     file_mask=file_mask,
                                     override=override)
 
-    def subject_access_request(self,
-                               user_id: str,
-                               dataset: str,
-                               override: bool = False,
-                               data_path: Optional[str] = os.environ.get(
-                                   "DATA_PATH"),
-                               span: int = 30) -> bool:
-        """
-
-        :return:
-        :rtype: bool
-        :param user_id: the user's unique identifier to search for
-        :param dataset: the data to search for.
-        :param override: Flag to override an existing table file.
-        :return: True if user's data has been found
-        :rtype: bool
-        """
-        logging.debug(f'user:{user_id}')
-        logging.debug(f'dataset:{dataset}')
-        user_has_data = False
-        try:
-            user_files_folder = f"{data_path}dsar/{user_id}/"
-            # list tables in the dataset
-            tables = self.__client.list_tables(dataset=dataset)
-            # Loop dataset's tables
-            for table in tables:
-                user_table_file_path = f"{user_files_folder}{table.table_id}.csv"
-                qualified_table_id = "{}.{}.{}".format(
-                    table.project, table.dataset_id, table.table_id)
-                logging.debug(qualified_table_id)
-                table = self.__client.get_table(qualified_table_id)
-                user_id_field = None
-                # Loop table's fields to check if it has a user identifier column
-                for schema_field in table.schema:
-                    if schema_field.name == 'user_id':
-                        user_id_field = schema_field.name
-                    elif schema_field.name == 'permutive_id':
-                        user_id_field = schema_field.name
-                # Query the table for the user's data if file does not already exist
-                if user_id_field is not None and (override or not os.path.exists(user_table_file_path)):
-                    # Reducing the scope to dates with user activity
-                    partitions_query = "SELECT DISTINCT _PARTITIONTIME as p_partition from {} where DATE_DIFF(CURRENT_DATE(),DATE(_PARTITIONTIME), DAY) <30 and {}=\'{}\'".format(
-                        qualified_table_id, user_id_field, user_id)
-                    logging.debug(partitions_query)
-                    partitions_df = self.bigquery_to_dataframe(
-                        partitions_query)
-                    if len(partitions_df) > 0:
-                        user_has_data = True
-                        df_list = []
-                        for _, row in partitions_df.iterrows():
-
-                            query = "SELECT * from {} where {}=\'{}\' AND _PARTITIONTIME=\'{}\'".format(
-                                qualified_table_id, user_id_field, user_id, row['p_partition'])
-                            logging.debug(query)
-                            df = self.bigquery_to_dataframe(query)
-                            logging.debug(qualified_table_id +
-                                          ':' + str(len(df)))
-                            df_list.append(df)
-                        # concat the partitioned dataframes and save to csv
-                        FileHelper.check_filepath(user_files_folder)
-                        new_df = pd.concat(df_list)
-                        new_df.to_csv(user_table_file_path, index=False)
-            return user_has_data
-        except NotFound:
-            return user_has_data
-
-    def load_from_uri(self, table_id, bucket_name, data_path, partition_date: datetime.date) -> bool:
+    def load_from_uri(self,
+                      table_id: str,
+                      bucket_name: str,
+                      data_path: str,
+                      partition_date: datetime.date) -> bool:
         logging.debug('BigQuery::load_from_uri')
-        job_config, uri = BigQuery.build_job_config(
-            table_name=table_id, partition_date=partition_date, bucket_name=bucket_name, data_path=data_path)
+        job_config, uri = BigQuery.build_job_config(table_name=table_id,
+                                                    partition_date=partition_date,
+                                                    bucket_name=bucket_name,
+                                                    data_path=data_path)
 
         self.__client.load_table_from_uri(
             source_uris=uri, destination=table_id, job_config=job_config).result()
         return True
 
     @staticmethod
     def build_job_config(table_name: str,
@@ -461,15 +410,16 @@
                            local_folder=local_folder,
                            prefix=prefix,
                            partition_date=partition_date,
                            partition_name=partition_name,
                            file_mask=file_mask,
                            override=override)
 
-    def bigquery_to_dataframe(self, query_string: str) -> pd.DataFrame:
+    def bigquery_to_dataframe(self,
+                              query_string: str) -> pd.DataFrame:
         logging.debug("bigquery_to_dataframe")
         return self.__client.query(query_string).result().to_dataframe(create_bqstorage_client=True)
 
     def dataframe_to_bigquery(self,
                               dataframe: pd.DataFrame,
                               table_id: str,
                               write_disposition: bigquery.WriteDisposition = bigquery.WriteDisposition.WRITE_TRUNCATE  # type: ignore
@@ -485,23 +435,21 @@
         df_schema = dict(dataframe.dtypes)
 
         for item in df_schema.items():
             # Specify the type of columns whose type cannot be auto-detected.
             # For example  pandas dtype "object", so its data type is ambiguous.
 
             if item[1].name == 'object':
-                bq_field = bigquery.SchemaField(
-                    item[0], DATA_TYPE_MAPPING[item[1].name])  # type: ignore
+                bq_field = bigquery.SchemaField(item[0],
+                                                DATA_TYPE_MAPPING[item[1].name])
                 bq_schema.append(bq_field)
 
-        job_config = bigquery.LoadJobConfig(
-            schema=bq_schema,
-            write_disposition=write_disposition,
-        )
+        job_config = bigquery.LoadJobConfig(schema=bq_schema,
+                                            write_disposition=write_disposition)
 
-        job = self.__client.load_table_from_dataframe(
-            dataframe, table_id, job_config=job_config
-        )  # Make an API request.
-        job.result()  # Wait for the job to complete.
-        table = self.__client.get_table(table_id)  # Make an API request.
+        job = self.__client.load_table_from_dataframe(dataframe,
+                                                      table_id,
+                                                      job_config=job_config)
+        job.result()
+        table = self.__client.get_table(table_id)
         logging.debug("Loaded {} rows and {} columns to {}".format(
             table.num_rows, len(table.schema), table_id))
```

### Comparing `googlecloudplatformapi-2.2.4/GoogleCloudPlatformAPI/CloudStorage.py` & `googlecloudplatformapi-2.2.5/GoogleCloudPlatformAPI/CloudStorage.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import logging
 import os
 import json
 from typing import List, Optional, Union
 
 from google.cloud import storage
 
-from .ServiceAccount import ServiceAccount
+from . import ServiceAccount
 
 
 class CloudStorage:
     __client: storage.Client
 
     def __init__(self,
                  credentials: Optional[str] = None,
```

### Comparing `googlecloudplatformapi-2.2.4/GoogleCloudPlatformAPI/ServiceAccount.py` & `googlecloudplatformapi-2.2.5/GoogleCloudPlatformAPI/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,20 @@
+
 import logging
 from typing import List, Optional
 from google.oauth2 import service_account, credentials
 from googleads import oauth2
 import os
 
+from .AdManager import Audience,Network,Report,TargetingPreset,Traffic,Forecast
+from .Analytics import Analytics
+from .BigQuery import BigQuery
+from .CloudStorage import CloudStorage
+
+
 
 class ClientCredentials:
     def __init__(self):
         self.credentials_path = os.environ.get(
             "GOOGLE_APPLICATION_CREDENTIALS")
 
     @property
@@ -51,7 +58,18 @@
     @staticmethod
     def get_service_account_client(credentials: Optional[str] = None,
                                    scope: Optional[str] = "ad_manager"):
         if credentials is None:
             credentials = os.environ.get("GOOGLE_APPLICATION_CREDENTIALS")
         return oauth2.GoogleServiceAccountClient(key_file=credentials,
                                                  scope=oauth2.GetAPIScope(scope))
+
+
+__all__ = ["Audience",
+           "Network",
+           "Report",
+           "TargetingPreset",
+           "Traffic",
+           "Forecast",
+           "Analytics",
+           "BigQuery",
+           "CloudStorage"]
```

### Comparing `googlecloudplatformapi-2.2.4/LICENSE` & `googlecloudplatformapi-2.2.5/LICENSE`

 * *Files identical despite different names*

