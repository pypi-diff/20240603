# Comparing `tmp/copernicusmarine-1.2.3.tar.gz` & `tmp/copernicusmarine-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copernicusmarine-1.2.3.tar", max compression
+gzip compressed data, was "copernicusmarine-1.2.4.tar", max compression
```

## Comparing `copernicusmarine-1.2.3.tar` & `copernicusmarine-1.2.4.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0    13827 2024-05-15 09:48:13.578567 copernicusmarine-1.2.3/LICENSE.txt
--rw-r--r--   0        0        0    31604 2024-05-16 13:14:26.413146 copernicusmarine-1.2.3/README.md
--rw-r--r--   0        0        0      972 2024-05-15 09:48:13.578567 copernicusmarine-1.2.3/copernicusmarine/__init__.py
--rw-r--r--   0        0        0     1070 2024-05-15 09:48:13.578567 copernicusmarine-1.2.3/copernicusmarine/aioretry/LICENSE
--rw-r--r--   0        0        0      225 2024-05-15 09:48:13.578567 copernicusmarine-1.2.3/copernicusmarine/aioretry/__init__.py
--rw-r--r--   0        0        0     4152 2024-05-15 09:48:13.578567 copernicusmarine-1.2.3/copernicusmarine/aioretry/retry.py
--rw-r--r--   0        0        0       10 2024-05-15 09:48:13.578567 copernicusmarine-1.2.3/copernicusmarine/catalogue_parser/__init__.py
--rw-r--r--   0        0        0    32637 2024-05-16 16:38:54.241675 copernicusmarine-1.2.3/copernicusmarine/catalogue_parser/catalogue_parser.py
--rw-r--r--   0        0        0    11593 2024-05-16 15:20:18.074366 copernicusmarine-1.2.3/copernicusmarine/catalogue_parser/request_structure.py
--rw-r--r--   0        0        0       10 2024-05-15 09:48:13.578567 copernicusmarine-1.2.3/copernicusmarine/command_line_interface/__init__.py
--rw-r--r--   0        0        0      868 2024-05-15 09:48:13.578567 copernicusmarine-1.2.3/copernicusmarine/command_line_interface/copernicus_marine.py
--rw-r--r--   0        0        0     1766 2024-05-15 09:48:13.578567 copernicusmarine-1.2.3/copernicusmarine/command_line_interface/exception_handler.py
--rw-r--r--   0        0        0     4043 2024-05-21 14:48:04.042753 copernicusmarine-1.2.3/copernicusmarine/command_line_interface/group_describe.py
--rw-r--r--   0        0        0     9849 2024-05-15 09:48:13.578567 copernicusmarine-1.2.3/copernicusmarine/command_line_interface/group_get.py
--rw-r--r--   0        0        0     3033 2024-05-15 09:48:13.582568 copernicusmarine-1.2.3/copernicusmarine/command_line_interface/group_login.py
--rw-r--r--   0        0        0    12730 2024-05-16 13:14:26.413146 copernicusmarine-1.2.3/copernicusmarine/command_line_interface/group_subset.py
--rw-r--r--   0        0        0     2339 2024-05-15 09:48:13.582568 copernicusmarine-1.2.3/copernicusmarine/command_line_interface/utils.py
--rw-r--r--   0        0        0    13437 2024-05-21 15:59:02.577682 copernicusmarine-1.2.3/copernicusmarine/core_functions/credentials_utils.py
--rw-r--r--   0        0        0     5312 2024-05-21 15:59:02.577682 copernicusmarine-1.2.3/copernicusmarine/core_functions/custom_zarr_store.py
--rw-r--r--   0        0        0     2806 2024-05-15 09:48:13.582568 copernicusmarine-1.2.3/copernicusmarine/core_functions/deprecated.py
--rw-r--r--   0        0        0     2385 2024-05-21 14:48:04.042753 copernicusmarine-1.2.3/copernicusmarine/core_functions/deprecated_options.py
--rw-r--r--   0        0        0     2174 2024-05-21 14:48:04.042753 copernicusmarine-1.2.3/copernicusmarine/core_functions/describe.py
--rw-r--r--   0        0        0     1233 2024-05-15 09:48:13.582568 copernicusmarine-1.2.3/copernicusmarine/core_functions/environment_variables.py
--rw-r--r--   0        0        0      742 2024-05-15 09:48:13.582568 copernicusmarine-1.2.3/copernicusmarine/core_functions/exceptions.py
--rw-r--r--   0        0        0     8123 2024-05-15 09:48:13.582568 copernicusmarine-1.2.3/copernicusmarine/core_functions/get.py
--rw-r--r--   0        0        0     1606 2024-05-15 09:48:13.582568 copernicusmarine-1.2.3/copernicusmarine/core_functions/login.py
--rw-r--r--   0        0        0      460 2024-05-16 13:14:26.413146 copernicusmarine-1.2.3/copernicusmarine/core_functions/models.py
--rw-r--r--   0        0        0    20227 2024-05-21 15:59:02.577682 copernicusmarine-1.2.3/copernicusmarine/core_functions/services_utils.py
--rw-r--r--   0        0        0     1984 2024-05-21 15:59:02.577682 copernicusmarine-1.2.3/copernicusmarine/core_functions/sessions.py
--rw-r--r--   0        0        0     9735 2024-05-16 15:20:18.074366 copernicusmarine-1.2.3/copernicusmarine/core_functions/subset.py
--rw-r--r--   0        0        0     6541 2024-05-21 15:59:02.577682 copernicusmarine-1.2.3/copernicusmarine/core_functions/utils.py
--rw-r--r--   0        0        0     2688 2024-05-21 15:59:02.577682 copernicusmarine-1.2.3/copernicusmarine/core_functions/versions_verifier.py
--rw-r--r--   0        0        0     2608 2024-05-21 14:48:04.042753 copernicusmarine-1.2.3/copernicusmarine/download_functions/common_download.py
--rw-r--r--   0        0        0     8027 2024-05-21 15:59:02.577682 copernicusmarine-1.2.3/copernicusmarine/download_functions/download_arco_series.py
--rw-r--r--   0        0        0     1706 2024-05-15 09:48:13.582568 copernicusmarine-1.2.3/copernicusmarine/download_functions/download_get.py
--rw-r--r--   0        0        0    20555 2024-05-21 15:59:02.577682 copernicusmarine-1.2.3/copernicusmarine/download_functions/download_original_files.py
--rw-r--r--   0        0        0      918 2024-05-15 09:48:13.582568 copernicusmarine-1.2.3/copernicusmarine/download_functions/subset_parameters.py
--rw-r--r--   0        0        0    19059 2024-05-21 15:59:02.581682 copernicusmarine-1.2.3/copernicusmarine/download_functions/subset_xarray.py
--rw-r--r--   0        0        0     5634 2024-05-15 09:48:13.582568 copernicusmarine-1.2.3/copernicusmarine/download_functions/utils.py
--rw-r--r--   0        0        0      863 2024-05-15 09:48:13.582568 copernicusmarine-1.2.3/copernicusmarine/logging_conf.json
--rw-r--r--   0        0        0     2143 2024-05-21 14:48:04.042753 copernicusmarine-1.2.3/copernicusmarine/python_interface/describe.py
--rw-r--r--   0        0        0      447 2024-05-15 09:48:13.582568 copernicusmarine-1.2.3/copernicusmarine/python_interface/exception_handler.py
--rw-r--r--   0        0        0     5817 2024-05-15 09:48:13.582568 copernicusmarine-1.2.3/copernicusmarine/python_interface/get.py
--rw-r--r--   0        0        0     3545 2024-05-16 15:20:18.074366 copernicusmarine-1.2.3/copernicusmarine/python_interface/load_utils.py
--rw-r--r--   0        0        0     1464 2024-05-15 09:48:13.582568 copernicusmarine-1.2.3/copernicusmarine/python_interface/login.py
--rw-r--r--   0        0        0     6469 2024-05-16 13:14:26.413146 copernicusmarine-1.2.3/copernicusmarine/python_interface/open_dataset.py
--rw-r--r--   0        0        0     6150 2024-05-16 13:14:26.413146 copernicusmarine-1.2.3/copernicusmarine/python_interface/read_dataframe.py
--rw-r--r--   0        0        0     6620 2024-05-16 13:14:26.413146 copernicusmarine-1.2.3/copernicusmarine/python_interface/subset.py
--rw-r--r--   0        0        0      348 2024-05-15 09:48:13.582568 copernicusmarine-1.2.3/copernicusmarine/python_interface/utils.py
--rw-r--r--   0        0        0      901 2024-05-23 07:19:40.465487 copernicusmarine-1.2.3/pyproject.toml
--rw-r--r--   0        0        0    32677 1970-01-01 00:00:00.000000 copernicusmarine-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0    13827 2024-05-15 09:48:12.382978 copernicusmarine-1.2.4/LICENSE.txt
+-rw-r--r--   0        0        0    31604 2024-05-15 11:11:24.040466 copernicusmarine-1.2.4/README.md
+-rw-r--r--   0        0        0      972 2024-05-15 09:48:12.382978 copernicusmarine-1.2.4/copernicusmarine/__init__.py
+-rw-r--r--   0        0        0     1070 2024-05-15 09:48:12.382978 copernicusmarine-1.2.4/copernicusmarine/aioretry/LICENSE
+-rw-r--r--   0        0        0      225 2024-05-15 09:48:12.382978 copernicusmarine-1.2.4/copernicusmarine/aioretry/__init__.py
+-rw-r--r--   0        0        0     4152 2024-05-15 09:48:12.382978 copernicusmarine-1.2.4/copernicusmarine/aioretry/retry.py
+-rw-r--r--   0        0        0       10 2024-05-15 09:48:12.382978 copernicusmarine-1.2.4/copernicusmarine/catalogue_parser/__init__.py
+-rw-r--r--   0        0        0    32940 2024-06-03 09:03:59.054783 copernicusmarine-1.2.4/copernicusmarine/catalogue_parser/catalogue_parser.py
+-rw-r--r--   0        0        0    11593 2024-05-16 15:20:15.365969 copernicusmarine-1.2.4/copernicusmarine/catalogue_parser/request_structure.py
+-rw-r--r--   0        0        0       10 2024-05-15 09:48:12.382978 copernicusmarine-1.2.4/copernicusmarine/command_line_interface/__init__.py
+-rw-r--r--   0        0        0      868 2024-05-15 09:48:12.382978 copernicusmarine-1.2.4/copernicusmarine/command_line_interface/copernicus_marine.py
+-rw-r--r--   0        0        0     1766 2024-05-15 09:48:12.382978 copernicusmarine-1.2.4/copernicusmarine/command_line_interface/exception_handler.py
+-rw-r--r--   0        0        0     4043 2024-06-03 13:22:42.857486 copernicusmarine-1.2.4/copernicusmarine/command_line_interface/group_describe.py
+-rw-r--r--   0        0        0     9849 2024-05-15 09:48:12.382978 copernicusmarine-1.2.4/copernicusmarine/command_line_interface/group_get.py
+-rw-r--r--   0        0        0     3033 2024-05-15 09:48:12.382978 copernicusmarine-1.2.4/copernicusmarine/command_line_interface/group_login.py
+-rw-r--r--   0        0        0    12730 2024-05-15 11:11:24.040466 copernicusmarine-1.2.4/copernicusmarine/command_line_interface/group_subset.py
+-rw-r--r--   0        0        0     2339 2024-05-15 09:48:12.382978 copernicusmarine-1.2.4/copernicusmarine/command_line_interface/utils.py
+-rw-r--r--   0        0        0    13437 2024-05-31 08:17:48.012476 copernicusmarine-1.2.4/copernicusmarine/core_functions/credentials_utils.py
+-rw-r--r--   0        0        0     5312 2024-05-31 08:17:48.012476 copernicusmarine-1.2.4/copernicusmarine/core_functions/custom_zarr_store.py
+-rw-r--r--   0        0        0     2806 2024-05-15 09:48:12.382978 copernicusmarine-1.2.4/copernicusmarine/core_functions/deprecated.py
+-rw-r--r--   0        0        0     2385 2024-06-03 13:22:42.857486 copernicusmarine-1.2.4/copernicusmarine/core_functions/deprecated_options.py
+-rw-r--r--   0        0        0     2174 2024-06-03 13:22:42.857486 copernicusmarine-1.2.4/copernicusmarine/core_functions/describe.py
+-rw-r--r--   0        0        0     1233 2024-05-15 09:48:12.382978 copernicusmarine-1.2.4/copernicusmarine/core_functions/environment_variables.py
+-rw-r--r--   0        0        0      742 2024-05-15 09:48:12.382978 copernicusmarine-1.2.4/copernicusmarine/core_functions/exceptions.py
+-rw-r--r--   0        0        0     8123 2024-05-30 15:07:26.318194 copernicusmarine-1.2.4/copernicusmarine/core_functions/get.py
+-rw-r--r--   0        0        0     1606 2024-05-15 09:48:12.382978 copernicusmarine-1.2.4/copernicusmarine/core_functions/login.py
+-rw-r--r--   0        0        0      460 2024-05-15 11:11:24.040466 copernicusmarine-1.2.4/copernicusmarine/core_functions/models.py
+-rw-r--r--   0        0        0    20227 2024-05-31 08:17:48.012476 copernicusmarine-1.2.4/copernicusmarine/core_functions/services_utils.py
+-rw-r--r--   0        0        0     1984 2024-05-31 08:17:48.012476 copernicusmarine-1.2.4/copernicusmarine/core_functions/sessions.py
+-rw-r--r--   0        0        0     9735 2024-05-30 15:07:26.318194 copernicusmarine-1.2.4/copernicusmarine/core_functions/subset.py
+-rw-r--r--   0        0        0     6541 2024-05-27 12:57:52.812257 copernicusmarine-1.2.4/copernicusmarine/core_functions/utils.py
+-rw-r--r--   0        0        0     2688 2024-05-31 08:17:48.012476 copernicusmarine-1.2.4/copernicusmarine/core_functions/versions_verifier.py
+-rw-r--r--   0        0        0     2608 2024-05-27 12:57:52.816258 copernicusmarine-1.2.4/copernicusmarine/download_functions/common_download.py
+-rw-r--r--   0        0        0     8027 2024-05-31 08:17:48.012476 copernicusmarine-1.2.4/copernicusmarine/download_functions/download_arco_series.py
+-rw-r--r--   0        0        0     1706 2024-05-15 09:48:12.382978 copernicusmarine-1.2.4/copernicusmarine/download_functions/download_get.py
+-rw-r--r--   0        0        0    20555 2024-05-31 08:17:48.012476 copernicusmarine-1.2.4/copernicusmarine/download_functions/download_original_files.py
+-rw-r--r--   0        0        0      918 2024-05-15 09:48:12.382978 copernicusmarine-1.2.4/copernicusmarine/download_functions/subset_parameters.py
+-rw-r--r--   0        0        0    19059 2024-05-31 08:17:48.012476 copernicusmarine-1.2.4/copernicusmarine/download_functions/subset_xarray.py
+-rw-r--r--   0        0        0     5634 2024-05-15 09:48:12.382978 copernicusmarine-1.2.4/copernicusmarine/download_functions/utils.py
+-rw-r--r--   0        0        0      863 2024-05-15 09:48:12.382978 copernicusmarine-1.2.4/copernicusmarine/logging_conf.json
+-rw-r--r--   0        0        0     2143 2024-06-03 13:22:42.857486 copernicusmarine-1.2.4/copernicusmarine/python_interface/describe.py
+-rw-r--r--   0        0        0      447 2024-05-15 09:48:12.382978 copernicusmarine-1.2.4/copernicusmarine/python_interface/exception_handler.py
+-rw-r--r--   0        0        0     5817 2024-05-15 09:48:12.382978 copernicusmarine-1.2.4/copernicusmarine/python_interface/get.py
+-rw-r--r--   0        0        0     3545 2024-05-16 15:20:15.369969 copernicusmarine-1.2.4/copernicusmarine/python_interface/load_utils.py
+-rw-r--r--   0        0        0     1464 2024-05-15 09:48:12.382978 copernicusmarine-1.2.4/copernicusmarine/python_interface/login.py
+-rw-r--r--   0        0        0     6469 2024-05-15 11:11:24.040466 copernicusmarine-1.2.4/copernicusmarine/python_interface/open_dataset.py
+-rw-r--r--   0        0        0     6150 2024-05-15 11:11:24.040466 copernicusmarine-1.2.4/copernicusmarine/python_interface/read_dataframe.py
+-rw-r--r--   0        0        0     6620 2024-05-15 11:11:24.040466 copernicusmarine-1.2.4/copernicusmarine/python_interface/subset.py
+-rw-r--r--   0        0        0      348 2024-05-15 09:48:12.382978 copernicusmarine-1.2.4/copernicusmarine/python_interface/utils.py
+-rw-r--r--   0        0        0      901 2024-06-03 14:37:45.388241 copernicusmarine-1.2.4/pyproject.toml
+-rw-r--r--   0        0        0    32677 1970-01-01 00:00:00.000000 copernicusmarine-1.2.4/PKG-INFO
```

### Comparing `copernicusmarine-1.2.3/LICENSE.txt` & `copernicusmarine-1.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.3/README.md` & `copernicusmarine-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.3/copernicusmarine/__init__.py` & `copernicusmarine-1.2.4/copernicusmarine/__init__.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.3/copernicusmarine/aioretry/LICENSE` & `copernicusmarine-1.2.4/copernicusmarine/aioretry/LICENSE`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.3/copernicusmarine/aioretry/retry.py` & `copernicusmarine-1.2.4/copernicusmarine/aioretry/retry.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.3/copernicusmarine/catalogue_parser/catalogue_parser.py` & `copernicusmarine-1.2.4/copernicusmarine/catalogue_parser/catalogue_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -488,26 +488,34 @@
 def _construct_copernicus_marine_service(
     stac_service_name, stac_asset, datacube
 ) -> Optional[CopernicusMarineService]:
     try:
         service_uri = stac_asset.get_absolute_href()
         service_type = _service_type_from_web_api_string(stac_service_name)
         service_format = None
+        admp_in_preparation = datacube.properties.get("admp_in_preparation")
         if stac_asset.media_type and "zarr" in stac_asset.media_type:
             service_format = CopernicusMarineServiceFormat.ZARR
         elif stac_asset.media_type and "sqlite3" in stac_asset.media_type:
             service_format = CopernicusMarineServiceFormat.SQLITE
 
         if not service_uri.endswith("/"):
-            return CopernicusMarineService(
-                service_type=service_type,
-                uri=service_uri,
-                variables=_get_variables(datacube, stac_asset),
-                service_format=service_format,
-            )
+            if admp_in_preparation and (
+                service_type == CopernicusMarineDatasetServiceType.GEOSERIES
+                or service_type
+                == CopernicusMarineDatasetServiceType.TIMESERIES
+            ):
+                return None
+            else:
+                return CopernicusMarineService(
+                    service_type=service_type,
+                    uri=service_uri,
+                    variables=_get_variables(datacube, stac_asset),
+                    service_format=service_format,
+                )
         return None
     except ServiceNotHandled as service_not_handled:
         log_exception_debug(service_not_handled)
         return None
 
 
 def _get_versions_from_marine_datastore(
@@ -551,15 +559,15 @@
         services = _get_services(datacube)
         _, _, part = get_version_and_part_from_full_dataset_id(datacube.id)
 
         if services:
             parts.append(
                 CopernicusMarineVersionPart(
                     name=part,
-                    services=_get_services(datacube),
+                    services=services,
                     retired_date=retired_date,
                     released_date=released_date,
                 )
             )
 
     if parts:
         return parts
@@ -569,15 +577,14 @@
 def _get_services(
     datacube: pystac.Item,
 ) -> list[CopernicusMarineService]:
     stac_assets_dict = datacube.get_assets()
     return [
         dataset_service
         for stac_service_name, stac_asset in stac_assets_dict.items()
-        if stac_asset.roles and "data" in stac_asset.roles
         if (
             dataset_service := _construct_copernicus_marine_service(
                 stac_service_name, stac_asset, datacube
             )
         )
         is not None
     ]
```

### Comparing `copernicusmarine-1.2.3/copernicusmarine/catalogue_parser/request_structure.py` & `copernicusmarine-1.2.4/copernicusmarine/catalogue_parser/request_structure.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.3/copernicusmarine/command_line_interface/copernicus_marine.py` & `copernicusmarine-1.2.4/copernicusmarine/command_line_interface/copernicus_marine.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.3/copernicusmarine/command_line_interface/exception_handler.py` & `copernicusmarine-1.2.4/copernicusmarine/command_line_interface/exception_handler.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.3/copernicusmarine/command_line_interface/group_describe.py` & `copernicusmarine-1.2.4/copernicusmarine/command_line_interface/group_describe.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.3/copernicusmarine/command_line_interface/group_get.py` & `copernicusmarine-1.2.4/copernicusmarine/command_line_interface/group_get.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.3/copernicusmarine/command_line_interface/group_login.py` & `copernicusmarine-1.2.4/copernicusmarine/command_line_interface/group_login.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.3/copernicusmarine/command_line_interface/group_subset.py` & `copernicusmarine-1.2.4/copernicusmarine/command_line_interface/group_subset.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.3/copernicusmarine/command_line_interface/utils.py` & `copernicusmarine-1.2.4/copernicusmarine/command_line_interface/utils.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.3/copernicusmarine/core_functions/credentials_utils.py` & `copernicusmarine-1.2.4/copernicusmarine/core_functions/credentials_utils.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.3/copernicusmarine/core_functions/custom_zarr_store.py` & `copernicusmarine-1.2.4/copernicusmarine/core_functions/custom_zarr_store.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.3/copernicusmarine/core_functions/deprecated.py` & `copernicusmarine-1.2.4/copernicusmarine/core_functions/deprecated.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.3/copernicusmarine/core_functions/deprecated_options.py` & `copernicusmarine-1.2.4/copernicusmarine/core_functions/deprecated_options.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.3/copernicusmarine/core_functions/describe.py` & `copernicusmarine-1.2.4/copernicusmarine/core_functions/describe.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.3/copernicusmarine/core_functions/environment_variables.py` & `copernicusmarine-1.2.4/copernicusmarine/core_functions/environment_variables.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.3/copernicusmarine/core_functions/exceptions.py` & `copernicusmarine-1.2.4/copernicusmarine/core_functions/exceptions.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.3/copernicusmarine/core_functions/get.py` & `copernicusmarine-1.2.4/copernicusmarine/core_functions/get.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.3/copernicusmarine/core_functions/login.py` & `copernicusmarine-1.2.4/copernicusmarine/core_functions/login.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.3/copernicusmarine/core_functions/services_utils.py` & `copernicusmarine-1.2.4/copernicusmarine/core_functions/services_utils.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.3/copernicusmarine/core_functions/sessions.py` & `copernicusmarine-1.2.4/copernicusmarine/core_functions/sessions.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.3/copernicusmarine/core_functions/subset.py` & `copernicusmarine-1.2.4/copernicusmarine/core_functions/subset.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.3/copernicusmarine/core_functions/utils.py` & `copernicusmarine-1.2.4/copernicusmarine/core_functions/utils.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.3/copernicusmarine/core_functions/versions_verifier.py` & `copernicusmarine-1.2.4/copernicusmarine/core_functions/versions_verifier.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.3/copernicusmarine/download_functions/common_download.py` & `copernicusmarine-1.2.4/copernicusmarine/download_functions/common_download.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.3/copernicusmarine/download_functions/download_arco_series.py` & `copernicusmarine-1.2.4/copernicusmarine/download_functions/download_arco_series.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.3/copernicusmarine/download_functions/download_get.py` & `copernicusmarine-1.2.4/copernicusmarine/download_functions/download_get.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.3/copernicusmarine/download_functions/download_original_files.py` & `copernicusmarine-1.2.4/copernicusmarine/download_functions/download_original_files.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.3/copernicusmarine/download_functions/subset_parameters.py` & `copernicusmarine-1.2.4/copernicusmarine/download_functions/subset_parameters.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.3/copernicusmarine/download_functions/subset_xarray.py` & `copernicusmarine-1.2.4/copernicusmarine/download_functions/subset_xarray.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.3/copernicusmarine/download_functions/utils.py` & `copernicusmarine-1.2.4/copernicusmarine/download_functions/utils.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.3/copernicusmarine/logging_conf.json` & `copernicusmarine-1.2.4/copernicusmarine/logging_conf.json`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.3/copernicusmarine/python_interface/describe.py` & `copernicusmarine-1.2.4/copernicusmarine/python_interface/describe.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.3/copernicusmarine/python_interface/get.py` & `copernicusmarine-1.2.4/copernicusmarine/python_interface/get.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.3/copernicusmarine/python_interface/load_utils.py` & `copernicusmarine-1.2.4/copernicusmarine/python_interface/load_utils.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.3/copernicusmarine/python_interface/login.py` & `copernicusmarine-1.2.4/copernicusmarine/python_interface/login.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.3/copernicusmarine/python_interface/open_dataset.py` & `copernicusmarine-1.2.4/copernicusmarine/python_interface/open_dataset.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.3/copernicusmarine/python_interface/read_dataframe.py` & `copernicusmarine-1.2.4/copernicusmarine/python_interface/read_dataframe.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.3/copernicusmarine/python_interface/subset.py` & `copernicusmarine-1.2.4/copernicusmarine/python_interface/subset.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.3/pyproject.toml` & `copernicusmarine-1.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "copernicusmarine"
-version = "1.2.3"
+version = "1.2.4"
 description = ""
 authors = ["Copernicus Marine User Support <servicedesk.cmems@mercator-ocean.eu>"]
 readme = "README.md"
 packages = [{include = "copernicusmarine"}]
 license = "EUPL-1.2"
 
 [tool.poetry.dependencies]
```

### Comparing `copernicusmarine-1.2.3/PKG-INFO` & `copernicusmarine-1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copernicusmarine
-Version: 1.2.3
+Version: 1.2.4
 Summary: 
 License: EUPL-1.2
 Author: Copernicus Marine User Support
 Author-email: servicedesk.cmems@mercator-ocean.eu
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: copernicusmarine Version: 1.2.3 Summary: License:
+Metadata-Version: 2.1 Name: copernicusmarine Version: 1.2.4 Summary: License:
 EUPL-1.2 Author: Copernicus Marine User Support Author-email:
 servicedesk.cmems@mercator-ocean.eu Requires-Python: >=3.9,<3.13 Classifier:
 License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Requires-Dist: aiohttp (>=3.9.4) Requires-Dist:
```

