# Comparing `tmp/redbacktechpy-2024.5.1b7.tar.gz` & `tmp/redbacktechpy-2024.5.1b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redbacktechpy-2024.5.1b7.tar", last modified: Sun Jun  2 19:55:16 2024, max compression
+gzip compressed data, was "redbacktechpy-2024.5.1b8.tar", last modified: Mon Jun  3 03:10:04 2024, max compression
```

## Comparing `redbacktechpy-2024.5.1b7.tar` & `redbacktechpy-2024.5.1b8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:55:16.008871 redbacktechpy-2024.5.1b7/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-02 19:55:11.000000 redbacktechpy-2024.5.1b7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-06-02 19:55:16.008871 redbacktechpy-2024.5.1b7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-06-02 19:55:11.000000 redbacktechpy-2024.5.1b7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 19:55:16.008871 redbacktechpy-2024.5.1b7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:55:16.004871 redbacktechpy-2024.5.1b7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:55:16.008871 redbacktechpy-2024.5.1b7/src/redbacktechpy/
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-06-02 19:55:11.000000 redbacktechpy-2024.5.1b7/src/redbacktechpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-06-02 19:55:11.000000 redbacktechpy-2024.5.1b7/src/redbacktechpy/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-06-02 19:55:11.000000 redbacktechpy-2024.5.1b7/src/redbacktechpy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-06-02 19:55:11.000000 redbacktechpy-2024.5.1b7/src/redbacktechpy/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    51810 2024-06-02 19:55:11.000000 redbacktechpy-2024.5.1b7/src/redbacktechpy/redbacktech_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-06-02 19:55:11.000000 redbacktechpy-2024.5.1b7/src/redbacktechpy/str_enum.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:55:16.008871 redbacktechpy-2024.5.1b7/src/redbacktechpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-06-02 19:55:16.000000 redbacktechpy-2024.5.1b7/src/redbacktechpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-06-02 19:55:16.000000 redbacktechpy-2024.5.1b7/src/redbacktechpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 19:55:16.000000 redbacktechpy-2024.5.1b7/src/redbacktechpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-06-02 19:55:16.000000 redbacktechpy-2024.5.1b7/src/redbacktechpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-06-02 19:55:16.000000 redbacktechpy-2024.5.1b7/src/redbacktechpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 03:10:04.901004 redbacktechpy-2024.5.1b8/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-03 03:09:55.000000 redbacktechpy-2024.5.1b8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-06-03 03:10:04.901004 redbacktechpy-2024.5.1b8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-06-03 03:09:55.000000 redbacktechpy-2024.5.1b8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 03:10:04.901004 redbacktechpy-2024.5.1b8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 03:10:04.897004 redbacktechpy-2024.5.1b8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 03:10:04.901004 redbacktechpy-2024.5.1b8/src/redbacktechpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-06-03 03:09:55.000000 redbacktechpy-2024.5.1b8/src/redbacktechpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-06-03 03:09:55.000000 redbacktechpy-2024.5.1b8/src/redbacktechpy/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-06-03 03:09:55.000000 redbacktechpy-2024.5.1b8/src/redbacktechpy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-06-03 03:09:55.000000 redbacktechpy-2024.5.1b8/src/redbacktechpy/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55598 2024-06-03 03:09:55.000000 redbacktechpy-2024.5.1b8/src/redbacktechpy/redbacktech_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-06-03 03:09:55.000000 redbacktechpy-2024.5.1b8/src/redbacktechpy/str_enum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 03:10:04.901004 redbacktechpy-2024.5.1b8/src/redbacktechpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-06-03 03:10:04.000000 redbacktechpy-2024.5.1b8/src/redbacktechpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-06-03 03:10:04.000000 redbacktechpy-2024.5.1b8/src/redbacktechpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 03:10:04.000000 redbacktechpy-2024.5.1b8/src/redbacktechpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-06-03 03:10:04.000000 redbacktechpy-2024.5.1b8/src/redbacktechpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-06-03 03:10:04.000000 redbacktechpy-2024.5.1b8/src/redbacktechpy.egg-info/top_level.txt
```

### Comparing `redbacktechpy-2024.5.1b7/LICENSE` & `redbacktechpy-2024.5.1b8/LICENSE`

 * *Files identical despite different names*

### Comparing `redbacktechpy-2024.5.1b7/PKG-INFO` & `redbacktechpy-2024.5.1b8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redbacktechpy
-Version: 2024.5.1b7
+Version: 2024.5.1b8
 Summary: Python Module to support Home Asssistant integration with Redback Technologies Smart Hybrid Inverter
 Author-email: Chris Abberley <unlisted@gmail.com>
 Project-URL: Homepage, https://github.com/cabberley/redbacktechpy
 Project-URL: Issues, https://github.com/cabberley/redbacktechpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `redbacktechpy-2024.5.1b7/pyproject.toml` & `redbacktechpy-2024.5.1b8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "redbacktechpy"
-version = "2024.05.1b7"
+version = "2024.05.1b8"
 authors = [
   { name="Chris Abberley", email="unlisted@gmail.com" },
 ]
 description = "Python Module to support Home Asssistant integration with Redback Technologies Smart Hybrid Inverter"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE.txt"}
```

### Comparing `redbacktechpy-2024.5.1b7/src/redbacktechpy/__init__.py` & `redbacktechpy-2024.5.1b8/src/redbacktechpy/__init__.py`

 * *Files identical despite different names*

### Comparing `redbacktechpy-2024.5.1b7/src/redbacktechpy/constants.py` & `redbacktechpy-2024.5.1b8/src/redbacktechpy/constants.py`

 * *Files identical despite different names*

### Comparing `redbacktechpy-2024.5.1b7/src/redbacktechpy/model.py` & `redbacktechpy-2024.5.1b8/src/redbacktechpy/model.py`

 * *Files identical despite different names*

### Comparing `redbacktechpy-2024.5.1b7/src/redbacktechpy/redbacktech_client.py` & `redbacktechpy-2024.5.1b8/src/redbacktechpy/redbacktech_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Python API for Redback Tech Systems"""
 from __future__ import annotations
 from aiohttp import ClientResponse, ClientSession
 from typing import Any
+from math import sqrt
 import asyncio
 from datetime import datetime, timedelta, timezone
 from bs4 import BeautifulSoup
 import logging
 
 from .constants import (
     BaseUrl, 
@@ -49,14 +50,15 @@
         self._GAFToken: str | None = None
         self._device_info_refresh_time: datetime | None = None
         self._flatInverters = []
         self._flatBatterys = []
         self._redback_devices = []
         self._redback_entities = []
         self._redback_device_info = []
+        self._redback_site_load = 0
     
     async def get_redback_data(self):
         """Get Redback Data."""
         #Check if we need to get a new device list
         await self.create_device_info()
         
         inverter_data: dict[str, Inverters] = {}
@@ -307,14 +309,16 @@
             #response = await self.create_dynamic_info()
             if response1['Data']['Nodes'][0]['StaticData']['BatteryCount'] > 0:
                 soc_data = await self.get_config_by_serial(response1['Data']['Nodes'][0]['StaticData']['Id'])
                 #self._flatBatterys = await self._convert_static_by_serial_to_battery_list(response1, response2, soc_data)
                 await self._convert_responses_to_battery_entities(response1, response2, soc_data)
                 await self._create_device_info_battery(response1)
                 #self._redback_devices.append(self._flatBatterys)
+            await self._add_site_load_to_entities(self._redback_site_load, response1)
+            await self._create_device_info_inverter(response1)
         self._device_info_refresh_time = datetime.now() + timedelta(seconds=DEVICEINFOREFRESH)
         return 
     
     async def create_dynamic_info(self) -> None:
 
         self._serial_numbers = await self.get_inverter_list()
         self._dynamic_data = []
@@ -659,19 +663,19 @@
         #entity_name
         dataDict = {'value': data['Data']['Nodes'][0]['StaticData']['ModelName'], 'entity_name': 'model_name', 'device_id': id_temp, 'device_type': 'inverter', 'type_set': 'sensor.string' }
         self._redback_entities.append(dataDict)
         dataDict = {'value': data['Data']['Nodes'][0]['StaticData']['Id'], 'entity_name': 'serial_number', 'device_id': id_temp, 'device_type': 'inverter', 'type_set': 'sensor.string' }
         self._redback_entities.append(dataDict)
         dataDict = {'value': data['Data']['StaticData']['Location']['Latitude'], 'entity_name': 'latitude', 'device_id': id_temp, 'device_type': 'inverter', 'type_set': 'sensor.string' }
         self._redback_entities.append(dataDict)
-        dataDict = { 'value': data['Data']['StaticData']['Location']['Latitude'], 'entity_name': 'latitude', 'device_id': id_temp, 'device_type': 'inverter', 'type_set': 'sensor.string' }
+        dataDict = { 'value': data['Data']['StaticData']['Location']['Longitude'], 'entity_name': 'longitude', 'device_id': id_temp, 'device_type': 'inverter', 'type_set': 'sensor.string' }
         self._redback_entities.append(dataDict)
         dataDict = {'value': data['Data']['StaticData']['RemoteAccessConnection']['Type'],'entity_name': 'network_connection', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data['Data']['StaticData']['ApprovedCapacityW'],'entity_name': 'approved_capacity', 'device_id': id_temp, 'device_type': 'inverter'}
+        dataDict = {'value': data['Data']['StaticData']['ApprovedCapacityW'],'entity_name': 'approved_capacity_w', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
         dataDict = {'value': data['Data']['StaticData']['SiteDetails']['GenerationHardLimitVA'],'entity_name': 'generation_hard_limit_va', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
         dataDict = {'value': data['Data']['StaticData']['SiteDetails']['GenerationSoftLimitVA'],'entity_name': 'generation_soft_limit_va', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
         dataDict = {'value': data['Data']['StaticData']['SiteDetails']['ExportHardLimitkW'],'entity_name': 'export_hard_limit_kw', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
@@ -711,15 +715,18 @@
         self._redback_entities.append(dataDict)
         dataDict = {'value': data2['Data']['FrequencyInstantaneousHz'],'entity_name': 'frequency_instantaneous', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
         dataDict = {'value': data2['Data']['PvPowerInstantaneouskW'],'entity_name': 'pv_power_instantaneous_kw', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
         dataDict = {'value': data2['Data']['InverterTemperatureC'],'entity_name': 'inverter_temperature_c', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data2['Data']['PvAllTimeEnergykWh'],'entity_name': 'pv_all_time_energy_kwh', 'device_id': id_temp, 'device_type': 'inverter'}
+        if data2['Data']['PvAllTimeEnergykWh'] != None:
+            dataDict = {'value': (data2['Data']['PvAllTimeEnergykWh'])/1000,'entity_name': 'pv_all_time_energy_mwh', 'device_id': id_temp, 'device_type': 'inverter'}
+        else:
+            dataDict = {'value': data2['Data']['PvAllTimeEnergykWh'],'entity_name': 'pv_all_time_energy_mwh', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
         if data2['Data']['ExportAllTimeEnergykWh'] != None:
             dataDict = {'value': (data2['Data']['ExportAllTimeEnergykWh'])/1000,'entity_name': 'export_all_time_energy_mwh', 'device_id': id_temp, 'device_type': 'inverter'}
         else:
             dataDict = {'value': data2['Data']['ExportAllTimeEnergykWh'],'entity_name': 'export_all_time_energy_mwh', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
         if data2['Data']['ImportAllTimeEnergykWh'] != None:
@@ -734,43 +741,75 @@
         self._redback_entities.append(dataDict)
         dataDict = {'value': data2['Data']['Status'],'entity_name': 'status', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
         dataDict = {'value': data2['Data']['Inverters'][0]['PowerMode']['InverterMode'],'entity_name': 'power_mode_inverter_mode', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
         dataDict = {'value': data2['Data']['Inverters'][0]['PowerMode']['PowerW'],'entity_name': 'power_mode_power_w', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
+
+        
         for pv in data2['Data']['PVs']:
+            
             entity_name_temp = f'mppt_{pvId}_current_a'
             dataDict = {'value': pv['CurrentA'],'entity_name': entity_name_temp, 'device_id': id_temp, 'device_type': 'inverter'}
             self._redback_entities.append(dataDict)
             entity_name_temp = f'mppt_{pvId}_voltage_v'
             dataDict = {'value': pv['VoltageV'],'entity_name': entity_name_temp, 'device_id': id_temp, 'device_type': 'inverter'}
             self._redback_entities.append(dataDict)
             entity_name_temp = f'mppt_{pvId}_power_kw'
             dataDict = {'value': pv['PowerkW'],'entity_name': entity_name_temp, 'device_id': id_temp, 'device_type': 'inverter'}
             self._redback_entities.append(dataDict)
             pvId += 1
+        phase_count = 0
+        phase_voltage_sum = 0
+        phase_Current_sum = 0
+        phase_power_exported_sum = 0
+        phase_power_imported_sum = 0
+        phase_power_net_sum = 0
         for phase in data2['Data']['Phases']:  
-            phaseAlpha=phase['Id']
+            if phase['VoltageInstantaneousV'] != None:
+                phase_count += 1
+                phase_voltage_sum += phase['VoltageInstantaneousV']
+                phase_Current_sum += phase['CurrentInstantaneousA']
+                phase_power_exported_sum += phase['ActiveExportedPowerInstantaneouskW']
+                phase_power_imported_sum += phase['ActiveImportedPowerInstantaneouskW'] 
+                phase_power_net_sum += phase['ActiveImportedPowerInstantaneouskW'] - phase['ActiveExportedPowerInstantaneouskW']
+            phaseAlpha=phase['Id'].lower()
             entity_name_temp = f'inverter_phase_{phaseAlpha}_active_exported_power_instantaneous_kw'
             dataDict = {'value': phase['ActiveExportedPowerInstantaneouskW'],'entity_name': entity_name_temp, 'device_id': id_temp, 'device_type': 'inverter'}
             self._redback_entities.append(dataDict)
             entity_name_temp = f'inverter_phase_{phaseAlpha}_active_imported_power_instantaneous_kw'
             dataDict = {'value': phase['ActiveImportedPowerInstantaneouskW'],'entity_name': entity_name_temp, 'device_id': id_temp, 'device_type': 'inverter'}
             self._redback_entities.append(dataDict)
+            entity_name_temp = f'inverter_phase_{phaseAlpha}_active_net_power_instantaneous_kw'
+            dataDict = {'value': phase['ActiveImportedPowerInstantaneouskW'] - phase['ActiveExportedPowerInstantaneouskW'],'entity_name': entity_name_temp, 'device_id': id_temp, 'device_type': 'inverter'}
+            self._redback_entities.append(dataDict)
             entity_name_temp = f'inverter_phase_{phaseAlpha}_voltage_instantaneous_v'
             dataDict = {'value': phase['VoltageInstantaneousV'],'entity_name': entity_name_temp, 'device_id': id_temp, 'device_type': 'inverter'}
             self._redback_entities.append(dataDict)
             entity_name_temp = f'inverter_phase_{phaseAlpha}_current_instantaneous_a'
             dataDict = {'value': phase['CurrentInstantaneousA'],'entity_name': entity_name_temp, 'device_id': id_temp, 'device_type': 'inverter'}
             self._redback_entities.append(dataDict)
             entity_name_temp = f'inverter_phase_{phaseAlpha}_power_factor_instantaneous_minus_1to1'
             dataDict = {'value': phase['PowerFactorInstantaneousMinus1to1'],'entity_name': entity_name_temp, 'device_id': id_temp, 'device_type': 'inverter'}
             self._redback_entities.append(dataDict)
-
+        dataDict = {'value': round( phase_voltage_sum / phase_count * sqrt(phase_count), 1), 'entity_name': 'inverter_phase_total_voltage_instantaneous_v', 'device_id': id_temp, 'device_type': 'inverter'}
+        self._redback_entities.append(dataDict)
+        dataDict = {'value': phase_Current_sum, 'entity_name': 'inverter_phase_total_current_instantaneous_a', 'device_id': id_temp, 'device_type': 'inverter'}
+        self._redback_entities.append(dataDict)
+        dataDict = {'value': phase_power_exported_sum, 'entity_name': 'inverter_phase_total_active_exported_power_instantaneous_kw', 'device_id': id_temp, 'device_type': 'inverter'} 
+        self._redback_entities.append(dataDict)
+        dataDict = {'value': phase_power_imported_sum, 'entity_name': 'inverter_phase_total_active_imported_power_instantaneous_kw', 'device_id': id_temp, 'device_type': 'inverter'}
+        self._redback_entities.append(dataDict)
+        dataDict = {'value': round(phase_power_net_sum,3), 'entity_name': 'inverter_phase_total_active_net_power_instantaneous_kw', 'device_id': id_temp, 'device_type': 'inverter'}
+        self._redback_entities.append(dataDict)
+        
+        self._redback_site_load = phase_power_net_sum + data2['Data']['PvPowerInstantaneouskW']
+        return
+        
     async def _convert_responses_to_battery_entities(self, data, data2, soc_data) -> None:
         batteryName = 'Unknown'
         batteryId = 1
         cabinetId = 1
         id_temp = data['Data']['Nodes'][0]['StaticData']['Id']
         id_temp = id_temp[-4:] + 'bat'
         id_temp = id_temp.lower()
@@ -835,44 +874,64 @@
         dataDict = {'value': data2['Data']['Battery']['NumberOfModules'],'entity_name': 'battery_no_of_modules', 'device_id': id_temp, 'device_type': 'battery'}
         self._redback_entities.append(dataDict)
         
         dataDict = {'value':(data['Data']['StaticData']['SiteDetails']['BatteryCapacitykWh'] * data2['Data']['BatterySoCInstantaneous0to1'] ),'entity_name': 'battery_currently_stored_kwh', 'device_id': id_temp, 'device_type': 'battery'}
         self._redback_entities.append(dataDict)
         dataDict = {'value':  round(data['Data']['StaticData']['SiteDetails']['BatteryCapacitykWh'] * (data2['Data']['BatterySoCInstantaneous0to1']- soc_data['Data']['MinSoC0to1']),2),'entity_name': 'battery_currently_usable_kwh', 'device_id': id_temp, 'device_type': 'battery'}
         self._redback_entities.append(dataDict)
+        battery_current_a = 0
+        battery_power_kw = 0
         for battery in data['Data']['Nodes'][0]['StaticData']['BatteryModels']:
             if battery != 'Unknown':
                 batteryName = battery
                 dataDict = {'value': batteryName,'entity_name': f'battery_{batteryId}_model', 'device_id': id_temp, 'device_type': 'battery'}
                 self._redback_entities.append(dataDict)
             else:
                 dataDict = {'value': batteryName,'entity_name': f'battery_{batteryId}_model', 'device_id': id_temp, 'device_type': 'battery'}
                 self._redback_entities.append(dataDict)
             battery_temp_value = data2['Data']['Battery']['Modules'][batteryId-1]['CurrentNegativeIsChargingA']
-            battery_temp_name= f'battery_{batteryId}_current_negative_in_charging_a'
+            battery_current_a += battery_temp_value
+            battery_temp_name= f'battery_{batteryId}_current_negative_is_charging_a'
             dataDict = {'value': battery_temp_value,'entity_name': battery_temp_name, 'device_id': id_temp, 'device_type': 'battery'}
             self._redback_entities.append(dataDict)
+            
             battery_temp_value = data2['Data']['Battery']['Modules'][batteryId-1]['VoltageV']
             battery_temp_name= f'battery_{batteryId}_voltage_v'
             dataDict = {'value': battery_temp_value,'entity_name': battery_temp_name, 'device_id': id_temp, 'device_type': 'battery'}
             self._redback_entities.append(dataDict)
-            battery_temp_value = data2['Data']['Battery']['Modules'][batteryId-1]['VoltageV']
+            
+            battery_temp_value = data2['Data']['Battery']['Modules'][batteryId-1]['PowerNegativeIsChargingkW']
+            battery_power_kw += battery_temp_value
             battery_temp_name= f'battery_{batteryId}_power_negative_is_charging_kw'
             dataDict = {'value': battery_temp_value,'entity_name': battery_temp_name, 'device_id': id_temp, 'device_type': 'battery'}
             self._redback_entities.append(dataDict)
-            battery_temp_value = data2['Data']['Battery']['Modules'][batteryId-1]['PowerNegativeIsChargingkW']
+            
+            battery_temp_value = data2['Data']['Battery']['Modules'][batteryId-1]['SoC0To1']
             battery_temp_name= f'battery_{batteryId}_soc_0to1'
             dataDict = {'value': battery_temp_value,'entity_name': battery_temp_name, 'device_id': id_temp, 'device_type': 'battery'}
             self._redback_entities.append(dataDict)
             batteryId += 1
+            
+        dataDict = {'value': battery_current_a,'entity_name': 'battery_current_negative_is_charging_a', 'device_id': id_temp, 'device_type': 'battery'}
+        self._redback_entities.append(dataDict)
         
         for cabinet in data2['Data']['Battery']['Cabinets']:
-            cabinet_temp_name = f'battery_cabinet_{cabinetId}_id'
+            cabinet_temp_name = f'battery_cabinet_{cabinetId}_temperature_c'
             dataDict = {'value': cabinet['TemperatureC'],'entity_name': cabinet_temp_name, 'device_id': id_temp, 'device_type': 'battery'}
             self._redback_entities.append(dataDict)
             cabinet_temp_name = f'battery_cabinet_{cabinetId}_fan_state'
             dataDict = {'value': cabinet['FanState'],'entity_name': cabinet_temp_name, 'device_id': id_temp, 'device_type': 'battery'}
             self._redback_entities.append(dataDict)
             cabinetId += 1
-            
+        
+        self._redback_site_load += data2['Data']['BatteryPowerNegativeIsChargingkW']
+        return
+    
+    async def _add_site_load_to_entities(self, site_load_data, data):
+        id_temp = data['Data']['Nodes'][0]['StaticData']['Id']
+        id_temp = id_temp[-4:] + 'inv'
+        id_temp = id_temp.lower()
+        dataDict = {'value': round(site_load_data,3),'entity_name': 'inverter_site_load_instantaneous_kw', 'device_id': id_temp, 'device_type': 'inverter'}
+        self._redback_entities.append(dataDict)
+        return
```

### Comparing `redbacktechpy-2024.5.1b7/src/redbacktechpy/str_enum.py` & `redbacktechpy-2024.5.1b8/src/redbacktechpy/str_enum.py`

 * *Files identical despite different names*

### Comparing `redbacktechpy-2024.5.1b7/src/redbacktechpy.egg-info/PKG-INFO` & `redbacktechpy-2024.5.1b8/src/redbacktechpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redbacktechpy
-Version: 2024.5.1b7
+Version: 2024.5.1b8
 Summary: Python Module to support Home Asssistant integration with Redback Technologies Smart Hybrid Inverter
 Author-email: Chris Abberley <unlisted@gmail.com>
 Project-URL: Homepage, https://github.com/cabberley/redbacktechpy
 Project-URL: Issues, https://github.com/cabberley/redbacktechpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

