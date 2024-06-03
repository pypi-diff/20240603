# Comparing `tmp/redbacktechpy-2024.5.1b6.tar.gz` & `tmp/redbacktechpy-2024.5.1b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redbacktechpy-2024.5.1b6.tar", last modified: Sat Jun  1 22:34:16 2024, max compression
+gzip compressed data, was "redbacktechpy-2024.5.1b7.tar", last modified: Sun Jun  2 19:55:16 2024, max compression
```

## Comparing `redbacktechpy-2024.5.1b6.tar` & `redbacktechpy-2024.5.1b7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:34:16.122722 redbacktechpy-2024.5.1b6/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-01 22:34:11.000000 redbacktechpy-2024.5.1b6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-06-01 22:34:16.122722 redbacktechpy-2024.5.1b6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-06-01 22:34:11.000000 redbacktechpy-2024.5.1b6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 22:34:16.122722 redbacktechpy-2024.5.1b6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:34:16.122722 redbacktechpy-2024.5.1b6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:34:16.122722 redbacktechpy-2024.5.1b6/src/redbacktechpy/
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-06-01 22:34:11.000000 redbacktechpy-2024.5.1b6/src/redbacktechpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-06-01 22:34:11.000000 redbacktechpy-2024.5.1b6/src/redbacktechpy/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-06-01 22:34:11.000000 redbacktechpy-2024.5.1b6/src/redbacktechpy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-06-01 22:34:11.000000 redbacktechpy-2024.5.1b6/src/redbacktechpy/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    50889 2024-06-01 22:34:11.000000 redbacktechpy-2024.5.1b6/src/redbacktechpy/redbacktech_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-06-01 22:34:11.000000 redbacktechpy-2024.5.1b6/src/redbacktechpy/str_enum.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:34:16.122722 redbacktechpy-2024.5.1b6/src/redbacktechpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-06-01 22:34:16.000000 redbacktechpy-2024.5.1b6/src/redbacktechpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-06-01 22:34:16.000000 redbacktechpy-2024.5.1b6/src/redbacktechpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 22:34:16.000000 redbacktechpy-2024.5.1b6/src/redbacktechpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-06-01 22:34:16.000000 redbacktechpy-2024.5.1b6/src/redbacktechpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-06-01 22:34:16.000000 redbacktechpy-2024.5.1b6/src/redbacktechpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:55:16.008871 redbacktechpy-2024.5.1b7/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-02 19:55:11.000000 redbacktechpy-2024.5.1b7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-06-02 19:55:16.008871 redbacktechpy-2024.5.1b7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-06-02 19:55:11.000000 redbacktechpy-2024.5.1b7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 19:55:16.008871 redbacktechpy-2024.5.1b7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:55:16.004871 redbacktechpy-2024.5.1b7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:55:16.008871 redbacktechpy-2024.5.1b7/src/redbacktechpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-06-02 19:55:11.000000 redbacktechpy-2024.5.1b7/src/redbacktechpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-06-02 19:55:11.000000 redbacktechpy-2024.5.1b7/src/redbacktechpy/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-06-02 19:55:11.000000 redbacktechpy-2024.5.1b7/src/redbacktechpy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-06-02 19:55:11.000000 redbacktechpy-2024.5.1b7/src/redbacktechpy/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51810 2024-06-02 19:55:11.000000 redbacktechpy-2024.5.1b7/src/redbacktechpy/redbacktech_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-06-02 19:55:11.000000 redbacktechpy-2024.5.1b7/src/redbacktechpy/str_enum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:55:16.008871 redbacktechpy-2024.5.1b7/src/redbacktechpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-06-02 19:55:16.000000 redbacktechpy-2024.5.1b7/src/redbacktechpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-06-02 19:55:16.000000 redbacktechpy-2024.5.1b7/src/redbacktechpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 19:55:16.000000 redbacktechpy-2024.5.1b7/src/redbacktechpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-06-02 19:55:16.000000 redbacktechpy-2024.5.1b7/src/redbacktechpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-06-02 19:55:16.000000 redbacktechpy-2024.5.1b7/src/redbacktechpy.egg-info/top_level.txt
```

### Comparing `redbacktechpy-2024.5.1b6/LICENSE` & `redbacktechpy-2024.5.1b7/LICENSE`

 * *Files identical despite different names*

### Comparing `redbacktechpy-2024.5.1b6/PKG-INFO` & `redbacktechpy-2024.5.1b7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redbacktechpy
-Version: 2024.5.1b6
+Version: 2024.5.1b7
 Summary: Python Module to support Home Asssistant integration with Redback Technologies Smart Hybrid Inverter
 Author-email: Chris Abberley <unlisted@gmail.com>
 Project-URL: Homepage, https://github.com/cabberley/redbacktechpy
 Project-URL: Issues, https://github.com/cabberley/redbacktechpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `redbacktechpy-2024.5.1b6/pyproject.toml` & `redbacktechpy-2024.5.1b7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "redbacktechpy"
-version = "2024.05.1b6"
+version = "2024.05.1b7"
 authors = [
   { name="Chris Abberley", email="unlisted@gmail.com" },
 ]
 description = "Python Module to support Home Asssistant integration with Redback Technologies Smart Hybrid Inverter"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE.txt"}
```

### Comparing `redbacktechpy-2024.5.1b6/src/redbacktechpy/__init__.py` & `redbacktechpy-2024.5.1b7/src/redbacktechpy/__init__.py`

 * *Files identical despite different names*

### Comparing `redbacktechpy-2024.5.1b6/src/redbacktechpy/constants.py` & `redbacktechpy-2024.5.1b7/src/redbacktechpy/constants.py`

 * *Files identical despite different names*

### Comparing `redbacktechpy-2024.5.1b6/src/redbacktechpy/model.py` & `redbacktechpy-2024.5.1b7/src/redbacktechpy/model.py`

 * *Files identical despite different names*

### Comparing `redbacktechpy-2024.5.1b6/src/redbacktechpy/redbacktech_client.py` & `redbacktechpy-2024.5.1b7/src/redbacktechpy/redbacktech_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -295,26 +295,26 @@
             #Get the device info if it needs to be refreshed
             self._serial_numbers = await self.get_inverter_list()
             device_info = False
         
         for serial_number in self._serial_numbers:
             response1 = await self.get_static_by_serial(serial_number)
             response2 = await self.get_dynamic_by_serial(serial_number)
-            self._flatInverters = await self._convert_static_by_serial_to_inverter_list(response1, response2)
-            self._redback_devices.append(self._flatInverters)  ###
+            #self._flatInverters = await self._convert_static_by_serial_to_inverter_list(response1, response2)
+            #self._redback_devices.append(self._flatInverters)  ###
             await self._convert_responses_to_inverter_entities(response1, response2)
             await self._create_device_info_inverter(response1)
             #print(self._flatInverters['serial_number'])
             #response = await self.create_dynamic_info()
             if response1['Data']['Nodes'][0]['StaticData']['BatteryCount'] > 0:
                 soc_data = await self.get_config_by_serial(response1['Data']['Nodes'][0]['StaticData']['Id'])
-                self._flatBatterys = await self._convert_static_by_serial_to_battery_list(response1, response2, soc_data)
+                #self._flatBatterys = await self._convert_static_by_serial_to_battery_list(response1, response2, soc_data)
                 await self._convert_responses_to_battery_entities(response1, response2, soc_data)
                 await self._create_device_info_battery(response1)
-                self._redback_devices.append(self._flatBatterys)
+                #self._redback_devices.append(self._flatBatterys)
         self._device_info_refresh_time = datetime.now() + timedelta(seconds=DEVICEINFOREFRESH)
         return 
     
     async def create_dynamic_info(self) -> None:
 
         self._serial_numbers = await self.get_inverter_list()
         self._dynamic_data = []
@@ -687,60 +687,69 @@
         self._redback_entities.append(dataDict)
         dataDict = {'value': data['Data']['StaticData']['SiteDetails']['InverterMaxExportPowerkW'],'entity_name': 'inverter_max_export_power_kw', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
         dataDict = {'value': data['Data']['StaticData']['SiteDetails']['InverterMaxImportPowerkW'],'entity_name': 'inverter_max_import_power_kw', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
         dataDict = {'value': data['Data']['StaticData']['CommissioningDate'],'entity_name': 'commissioning_date', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data['Data']['Nodes'][0]['StaticData']['ModelName'],'entity_name': 'model_name', 'device_id': id_temp, 'device_type': 'inverter'}
-        self._redback_entities.append(dataDict)
+        #dataDict = {'value': data['Data']['Nodes'][0]['StaticData']['ModelName'],'entity_name': 'model_name', 'device_id': id_temp, 'device_type': 'inverter'}
+        #self._redback_entities.append(dataDict)
         dataDict = {'value': data['Data']['StaticData']['NMI'],'entity_name': 'nmi', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
         dataDict = {'value': data['Data']['StaticData']['Id'],'entity_name': 'site_id', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
         dataDict = {'value': data['Data']['StaticData']['Type'],'entity_name': 'inverter_site_type', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
         dataDict = {'value': data['Data']['Nodes'][0]['StaticData']['BatteryCount'],'entity_name': 'battery_count', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
         dataDict = {'value': data['Data']['Nodes'][0]['StaticData']['SoftwareVersion'],'entity_name': 'software_version', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
         dataDict = {'value': data['Data']['Nodes'][0]['StaticData']['FirmwareVersion'],'entity_name': 'firmware_version', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data['Data']['Nodes'][0]['StaticData']['Id'],'entity_name': 'inverter_serial_number', 'device_id': id_temp, 'device_type': 'inverter'}
-        self._redback_entities.append(dataDict)
+        #dataDict = {'value': data['Data']['Nodes'][0]['StaticData']['Id'],'entity_name': 'inverter_serial_number', 'device_id': id_temp, 'device_type': 'inverter'}
+        #self._redback_entities.append(dataDict)
         dataDict = {'value': data2['Data']['TimestampUtc'],'entity_name': 'timestamp_utc', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
         dataDict = {'value': data2['Data']['FrequencyInstantaneousHz'],'entity_name': 'frequency_instantaneous', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
         dataDict = {'value': data2['Data']['PvPowerInstantaneouskW'],'entity_name': 'pv_power_instantaneous_kw', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
         dataDict = {'value': data2['Data']['InverterTemperatureC'],'entity_name': 'inverter_temperature_c', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
         dataDict = {'value': data2['Data']['PvAllTimeEnergykWh'],'entity_name': 'pv_all_time_energy_kwh', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data2['Data']['ExportAllTimeEnergykWh'],'entity_name': 'export_all_time_energy_kwh', 'device_id': id_temp, 'device_type': 'inverter'}
+        if data2['Data']['ExportAllTimeEnergykWh'] != None:
+            dataDict = {'value': (data2['Data']['ExportAllTimeEnergykWh'])/1000,'entity_name': 'export_all_time_energy_mwh', 'device_id': id_temp, 'device_type': 'inverter'}
+        else:
+            dataDict = {'value': data2['Data']['ExportAllTimeEnergykWh'],'entity_name': 'export_all_time_energy_mwh', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data2['Data']['ImportAllTimeEnergykWh'],'entity_name': 'import_all_time_energy_kwh', 'device_id': id_temp, 'device_type': 'inverter'}
+        if data2['Data']['ImportAllTimeEnergykWh'] != None:
+            dataDict = {'value': (data2['Data']['ImportAllTimeEnergykWh'])/1000,'entity_name': 'import_all_time_energy_mwh', 'device_id': id_temp, 'device_type': 'inverter'}
+        else:
+            dataDict = {'value': data2['Data']['ImportAllTimeEnergykWh'],'entity_name': 'import_all_time_energy_mwh', 'device_id': id_temp, 'device_type': 'inverter'}  
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data2['Data']['LoadAllTimeEnergykWh'],'entity_name': 'load_all_time_energy_kwh', 'device_id': id_temp, 'device_type': 'inverter'}
+        if data2['Data']['LoadAllTimeEnergykWh'] != None:
+            dataDict = {'value': (data2['Data']['LoadAllTimeEnergykWh'])/1000,'entity_name': 'load_all_time_energy_mwh', 'device_id': id_temp, 'device_type': 'inverter'}   
+        else:
+            dataDict = {'value': data2['Data']['LoadAllTimeEnergykWh'],'entity_name': 'load_all_time_energy_mwh', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
         dataDict = {'value': data2['Data']['Status'],'entity_name': 'status', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
         dataDict = {'value': data2['Data']['Inverters'][0]['PowerMode']['InverterMode'],'entity_name': 'power_mode_inverter_mode', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
         dataDict = {'value': data2['Data']['Inverters'][0]['PowerMode']['PowerW'],'entity_name': 'power_mode_power_w', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
         for pv in data2['Data']['PVs']:
-            entity_name_temp = f'pv_{pvId}_current_a'
+            entity_name_temp = f'mppt_{pvId}_current_a'
             dataDict = {'value': pv['CurrentA'],'entity_name': entity_name_temp, 'device_id': id_temp, 'device_type': 'inverter'}
             self._redback_entities.append(dataDict)
-            entity_name_temp = f'pv_{pvId}_voltage_v'
+            entity_name_temp = f'mppt_{pvId}_voltage_v'
             dataDict = {'value': pv['VoltageV'],'entity_name': entity_name_temp, 'device_id': id_temp, 'device_type': 'inverter'}
             self._redback_entities.append(dataDict)
-            entity_name_temp = f'pv_{pvId}_power_kw'
+            entity_name_temp = f'mppt_{pvId}_power_kw'
             dataDict = {'value': pv['PowerkW'],'entity_name': entity_name_temp, 'device_id': id_temp, 'device_type': 'inverter'}
             self._redback_entities.append(dataDict)
             pvId += 1
         for phase in data2['Data']['Phases']:  
             phaseAlpha=phase['Id']
             entity_name_temp = f'inverter_phase_{phaseAlpha}_active_exported_power_instantaneous_kw'
             dataDict = {'value': phase['ActiveExportedPowerInstantaneouskW'],'entity_name': entity_name_temp, 'device_id': id_temp, 'device_type': 'inverter'}
@@ -761,18 +770,14 @@
     async def _convert_responses_to_battery_entities(self, data, data2, soc_data) -> None:
         batteryName = 'Unknown'
         batteryId = 1
         cabinetId = 1
         id_temp = data['Data']['Nodes'][0]['StaticData']['Id']
         id_temp = id_temp[-4:] + 'bat'
         id_temp = id_temp.lower()
-        dataDict = {'value': data['Data']['Nodes'][0]['StaticData']['Id'],'entity_name': 'serial_number', 'device_id': id_temp, 'device_type': 'battery'}
-        self._redback_entities.append(dataDict)
-        dataDict = {'value': data['Data']['Nodes'][0]['StaticData']['ModelName'],'entity_name': 'model', 'device_id': id_temp, 'device_type': 'battery'}
-        self._redback_entities.append(dataDict)
         dataDict = {'value': soc_data['Data']['MinSoC0to1'],'entity_name': 'min_soc_0_to_1', 'device_id': id_temp, 'device_type': 'battery'}
         self._redback_entities.append(dataDict)
         dataDict = {'value': soc_data['Data']['MinOffgridSoC0to1'],'entity_name': 'min_Offgrid_soc_0_to_1', 'device_id': id_temp, 'device_type': 'battery'}
         self._redback_entities.append(dataDict)
         dataDict = {'value': data['Data']['StaticData']['Location']['Latitude'],'entity_name': 'latitude', 'device_id': id_temp, 'device_type': 'battery'}
         self._redback_entities.append(dataDict)
         dataDict = {'value': data['Data']['StaticData']['Location']['Longitude'],'entity_name': 'longitude', 'device_id': id_temp, 'device_type': 'battery'}
@@ -805,17 +810,23 @@
         self._redback_entities.append(dataDict)
         dataDict = {'value': data2['Data']['TimestampUtc'],'entity_name': 'timestamp_utc', 'device_id': id_temp, 'device_type': 'battery'}
         self._redback_entities.append(dataDict)
         dataDict = {'value': data2['Data']['BatterySoCInstantaneous0to1'],'entity_name': 'battery_soc_instantaneous_0to1', 'device_id': id_temp, 'device_type': 'battery'}
         self._redback_entities.append(dataDict)
         dataDict = {'value': data2['Data']['BatteryPowerNegativeIsChargingkW'],'entity_name': 'battery_power_negative_is_charging_kw', 'device_id': id_temp, 'device_type': 'battery'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data2['Data']['BatteryChargeAllTimeEnergykWh'],'entity_name': 'battery_charge_all_time_energy_kwh', 'device_id': id_temp, 'device_type': 'battery'}
+        if data2['Data']['BatteryChargeAllTimeEnergykWh'] != None:
+            dataDict = {'value': (data2['Data']['BatteryChargeAllTimeEnergykWh'])/1000,'entity_name': 'battery_charge_all_time_energy_mwh', 'device_id': id_temp, 'device_type': 'battery'}
+        else:
+            dataDict = {'value': data2['Data']['BatteryChargeAllTimeEnergykWh'],'entity_name': 'battery_charge_all_time_energy_mwh', 'device_id': id_temp, 'device_type': 'battery'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data2['Data']['BatteryDischargeAllTimeEnergykWh'],'entity_name': 'battery_discharge_all_time_energy_kwh', 'device_id': id_temp, 'device_type': 'battery'}
+        if data2['Data']['BatteryDischargeAllTimeEnergykWh'] != None:
+            dataDict = {'value': (data2['Data']['BatteryDischargeAllTimeEnergykWh'])/1000,'entity_name': 'battery_discharge_all_time_energy_mwh', 'device_id': id_temp, 'device_type': 'battery'}
+        else:
+            dataDict = {'value': data2['Data']['BatteryDischargeAllTimeEnergykWh'],'entity_name': 'battery_discharge_all_time_energy_mwh', 'device_id': id_temp, 'device_type': 'battery'}
         self._redback_entities.append(dataDict)
         dataDict = {'value': data2['Data']['Status'],'entity_name': 'status', 'device_id': id_temp, 'device_type': 'battery'}
         self._redback_entities.append(dataDict)
         dataDict = {'value': data2['Data']['Battery']['CurrentNegativeIsChargingA'],'entity_name': 'battery_current_negative_in_charging_a', 'device_id': id_temp, 'device_type': 'battery'}
         self._redback_entities.append(dataDict)
         dataDict = {'value': data2['Data']['Battery']['VoltageV'],'entity_name': 'battery_voltage_v', 'device_id': id_temp, 'device_type': 'battery'}
         self._redback_entities.append(dataDict)
```

### Comparing `redbacktechpy-2024.5.1b6/src/redbacktechpy/str_enum.py` & `redbacktechpy-2024.5.1b7/src/redbacktechpy/str_enum.py`

 * *Files identical despite different names*

### Comparing `redbacktechpy-2024.5.1b6/src/redbacktechpy.egg-info/PKG-INFO` & `redbacktechpy-2024.5.1b7/src/redbacktechpy.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redbacktechpy
-Version: 2024.5.1b6
+Version: 2024.5.1b7
 Summary: Python Module to support Home Asssistant integration with Redback Technologies Smart Hybrid Inverter
 Author-email: Chris Abberley <unlisted@gmail.com>
 Project-URL: Homepage, https://github.com/cabberley/redbacktechpy
 Project-URL: Issues, https://github.com/cabberley/redbacktechpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

