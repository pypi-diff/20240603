# Comparing `tmp/redbacktechpy-2024.5.1b8.tar.gz` & `tmp/redbacktechpy-2024.5.1b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redbacktechpy-2024.5.1b8.tar", last modified: Mon Jun  3 03:10:04 2024, max compression
+gzip compressed data, was "redbacktechpy-2024.5.1b9.tar", last modified: Mon Jun  3 04:55:01 2024, max compression
```

## Comparing `redbacktechpy-2024.5.1b8.tar` & `redbacktechpy-2024.5.1b9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 03:10:04.901004 redbacktechpy-2024.5.1b8/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-03 03:09:55.000000 redbacktechpy-2024.5.1b8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-06-03 03:10:04.901004 redbacktechpy-2024.5.1b8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-06-03 03:09:55.000000 redbacktechpy-2024.5.1b8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 03:10:04.901004 redbacktechpy-2024.5.1b8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 03:10:04.897004 redbacktechpy-2024.5.1b8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 03:10:04.901004 redbacktechpy-2024.5.1b8/src/redbacktechpy/
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-06-03 03:09:55.000000 redbacktechpy-2024.5.1b8/src/redbacktechpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-06-03 03:09:55.000000 redbacktechpy-2024.5.1b8/src/redbacktechpy/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-06-03 03:09:55.000000 redbacktechpy-2024.5.1b8/src/redbacktechpy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-06-03 03:09:55.000000 redbacktechpy-2024.5.1b8/src/redbacktechpy/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    55598 2024-06-03 03:09:55.000000 redbacktechpy-2024.5.1b8/src/redbacktechpy/redbacktech_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-06-03 03:09:55.000000 redbacktechpy-2024.5.1b8/src/redbacktechpy/str_enum.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 03:10:04.901004 redbacktechpy-2024.5.1b8/src/redbacktechpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-06-03 03:10:04.000000 redbacktechpy-2024.5.1b8/src/redbacktechpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-06-03 03:10:04.000000 redbacktechpy-2024.5.1b8/src/redbacktechpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 03:10:04.000000 redbacktechpy-2024.5.1b8/src/redbacktechpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-06-03 03:10:04.000000 redbacktechpy-2024.5.1b8/src/redbacktechpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-06-03 03:10:04.000000 redbacktechpy-2024.5.1b8/src/redbacktechpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 04:55:01.196709 redbacktechpy-2024.5.1b9/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-03 04:54:56.000000 redbacktechpy-2024.5.1b9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-06-03 04:55:01.196709 redbacktechpy-2024.5.1b9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-06-03 04:54:56.000000 redbacktechpy-2024.5.1b9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 04:55:01.196709 redbacktechpy-2024.5.1b9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 04:55:01.192709 redbacktechpy-2024.5.1b9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 04:55:01.196709 redbacktechpy-2024.5.1b9/src/redbacktechpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-06-03 04:54:56.000000 redbacktechpy-2024.5.1b9/src/redbacktechpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-06-03 04:54:56.000000 redbacktechpy-2024.5.1b9/src/redbacktechpy/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-06-03 04:54:56.000000 redbacktechpy-2024.5.1b9/src/redbacktechpy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-06-03 04:54:56.000000 redbacktechpy-2024.5.1b9/src/redbacktechpy/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55678 2024-06-03 04:54:56.000000 redbacktechpy-2024.5.1b9/src/redbacktechpy/redbacktech_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-06-03 04:54:56.000000 redbacktechpy-2024.5.1b9/src/redbacktechpy/str_enum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 04:55:01.196709 redbacktechpy-2024.5.1b9/src/redbacktechpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-06-03 04:55:01.000000 redbacktechpy-2024.5.1b9/src/redbacktechpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-06-03 04:55:01.000000 redbacktechpy-2024.5.1b9/src/redbacktechpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 04:55:01.000000 redbacktechpy-2024.5.1b9/src/redbacktechpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-06-03 04:55:01.000000 redbacktechpy-2024.5.1b9/src/redbacktechpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-06-03 04:55:01.000000 redbacktechpy-2024.5.1b9/src/redbacktechpy.egg-info/top_level.txt
```

### Comparing `redbacktechpy-2024.5.1b8/LICENSE` & `redbacktechpy-2024.5.1b9/LICENSE`

 * *Files identical despite different names*

### Comparing `redbacktechpy-2024.5.1b8/PKG-INFO` & `redbacktechpy-2024.5.1b9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redbacktechpy
-Version: 2024.5.1b8
+Version: 2024.5.1b9
 Summary: Python Module to support Home Asssistant integration with Redback Technologies Smart Hybrid Inverter
 Author-email: Chris Abberley <unlisted@gmail.com>
 Project-URL: Homepage, https://github.com/cabberley/redbacktechpy
 Project-URL: Issues, https://github.com/cabberley/redbacktechpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `redbacktechpy-2024.5.1b8/pyproject.toml` & `redbacktechpy-2024.5.1b9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "redbacktechpy"
-version = "2024.05.1b8"
+version = "2024.05.1b9"
 authors = [
   { name="Chris Abberley", email="unlisted@gmail.com" },
 ]
 description = "Python Module to support Home Asssistant integration with Redback Technologies Smart Hybrid Inverter"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE.txt"}
```

### Comparing `redbacktechpy-2024.5.1b8/src/redbacktechpy/__init__.py` & `redbacktechpy-2024.5.1b9/src/redbacktechpy/__init__.py`

 * *Files identical despite different names*

### Comparing `redbacktechpy-2024.5.1b8/src/redbacktechpy/constants.py` & `redbacktechpy-2024.5.1b9/src/redbacktechpy/constants.py`

 * *Files identical despite different names*

### Comparing `redbacktechpy-2024.5.1b8/src/redbacktechpy/model.py` & `redbacktechpy-2024.5.1b9/src/redbacktechpy/model.py`

 * *Files identical despite different names*

### Comparing `redbacktechpy-2024.5.1b8/src/redbacktechpy/redbacktech_client.py` & `redbacktechpy-2024.5.1b9/src/redbacktechpy/redbacktech_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -420,15 +420,15 @@
         dataDict['firmware_version'] = data['Data']['Nodes'][0]['StaticData']['FirmwareVersion']
         for battery in data['Data']['Nodes'][0]['StaticData']['BatteryModels']:
             if battery != 'Unknown':
                 batteryName = battery
                 dataDict[f'battery_{batteryId}_model'] = batteryName
             else:
                 dataDict[f'battery_{batteryId}_model'] = batteryName
-            dataDict[f'battery_{batteryId}_current_negative_in_charging_a'] = data2['Data']['Battery']['Modules'][batteryId-1]['CurrentNegativeIsChargingA']
+            dataDict[f'battery_{batteryId}_current_negative_is_charging_a'] = data2['Data']['Battery']['Modules'][batteryId-1]['CurrentNegativeIsChargingA']
             dataDict[f'battery_{batteryId}_voltage_v'] =  data2['Data']['Battery']['Modules'][batteryId-1]['VoltageV']
             dataDict[f'battery_{batteryId}_power_negative_is_charging_kw'] =  data2['Data']['Battery']['Modules'][batteryId-1]['PowerNegativeIsChargingkW']
             dataDict[f'battery_{batteryId}_soc_0to1'] =  data2['Data']['Battery']['Modules'][batteryId-1]['SoC0To1']
             batteryId += 1
         for cabinet in data2['Data']['Battery']['Cabinets']:
             dataDict[f'battery_cabinet_{cabinetId}_temperature_c'] = cabinet['TemperatureC']
             dataDict[f'battery_cabinet_{cabinetId}_fan_state'] = cabinet['FanState']
@@ -436,15 +436,15 @@
         dataDict['inverter_serial_number'] = data['Data']['Nodes'][0]['StaticData']['Id']
         dataDict['timestamp_utc'] = data2['Data']['TimestampUtc']
         dataDict['battery_soc_instantaneous_0to1'] = data2['Data']['BatterySoCInstantaneous0to1']
         dataDict['battery_power_negative_is_charging_kw'] = data2['Data']['BatteryPowerNegativeIsChargingkW']
         dataDict['battery_charge_all_time_energy_kwh'] = data2['Data']['BatteryChargeAllTimeEnergykWh']
         dataDict['battery_discharge_all_time_energy_kwh'] = data2['Data']['BatteryDischargeAllTimeEnergykWh']
         dataDict['status'] = data2['Data']['Status']
-        dataDict['battery_current_negative_in_charging_a'] = data2['Data']['Battery']['CurrentNegativeIsChargingA']
+        dataDict['battery_current_negative_is_charging_a'] = data2['Data']['Battery']['CurrentNegativeIsChargingA']
         dataDict['battery_voltage_v'] = data2['Data']['Battery']['VoltageV']
         dataDict['battery_voltage_type'] = data2['Data']['Battery']['VoltageType']
         dataDict['battery_no_of_modules'] = data2['Data']['Battery']['NumberOfModules']
         
         dataDict['battery_currently_stored_kwh'] = (data['Data']['StaticData']['SiteDetails']['BatteryCapacitykWh'] * data2['Data']['BatterySoCInstantaneous0to1'] )
         dataDict['battery_currently_usable_kwh'] = round(data['Data']['StaticData']['SiteDetails']['BatteryCapacitykWh'] * (data2['Data']['BatterySoCInstantaneous0to1']- soc_data['Data']['MinSoC0to1']),2)
         return dataDict
@@ -707,15 +707,15 @@
         self._redback_entities.append(dataDict)
         dataDict = {'value': data['Data']['Nodes'][0]['StaticData']['SoftwareVersion'],'entity_name': 'software_version', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
         dataDict = {'value': data['Data']['Nodes'][0]['StaticData']['FirmwareVersion'],'entity_name': 'firmware_version', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
         #dataDict = {'value': data['Data']['Nodes'][0]['StaticData']['Id'],'entity_name': 'inverter_serial_number', 'device_id': id_temp, 'device_type': 'inverter'}
         #self._redback_entities.append(dataDict)
-        dataDict = {'value': data2['Data']['TimestampUtc'],'entity_name': 'timestamp_utc', 'device_id': id_temp, 'device_type': 'inverter'}
+        dataDict = {'value': (data2['Data']['TimestampUtc']).replace('Z','+00:00'),'entity_name': 'timestamp_utc', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
         dataDict = {'value': data2['Data']['FrequencyInstantaneousHz'],'entity_name': 'frequency_instantaneous', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
         dataDict = {'value': data2['Data']['PvPowerInstantaneouskW'],'entity_name': 'pv_power_instantaneous_kw', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
         dataDict = {'value': data2['Data']['InverterTemperatureC'],'entity_name': 'inverter_temperature_c', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
@@ -809,17 +809,17 @@
     async def _convert_responses_to_battery_entities(self, data, data2, soc_data) -> None:
         batteryName = 'Unknown'
         batteryId = 1
         cabinetId = 1
         id_temp = data['Data']['Nodes'][0]['StaticData']['Id']
         id_temp = id_temp[-4:] + 'bat'
         id_temp = id_temp.lower()
-        dataDict = {'value': soc_data['Data']['MinSoC0to1'],'entity_name': 'min_soc_0_to_1', 'device_id': id_temp, 'device_type': 'battery'}
+        dataDict = {'value': (soc_data['Data']['MinSoC0to1'])*100,'entity_name': 'min_soc_0_to_1', 'device_id': id_temp, 'device_type': 'battery'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': soc_data['Data']['MinOffgridSoC0to1'],'entity_name': 'min_Offgrid_soc_0_to_1', 'device_id': id_temp, 'device_type': 'battery'}
+        dataDict = {'value': (soc_data['Data']['MinOffgridSoC0to1'])*100,'entity_name': 'min_Offgrid_soc_0_to_1', 'device_id': id_temp, 'device_type': 'battery'}
         self._redback_entities.append(dataDict)
         dataDict = {'value': data['Data']['StaticData']['Location']['Latitude'],'entity_name': 'latitude', 'device_id': id_temp, 'device_type': 'battery'}
         self._redback_entities.append(dataDict)
         dataDict = {'value': data['Data']['StaticData']['Location']['Longitude'],'entity_name': 'longitude', 'device_id': id_temp, 'device_type': 'battery'}
         self._redback_entities.append(dataDict)
         dataDict = {'value': data['Data']['StaticData']['SiteDetails']['BatteryMaxChargePowerkW'],'entity_name': 'battery_max_charge_power_kw', 'device_id': id_temp, 'device_type': 'battery'}
         self._redback_entities.append(dataDict)
@@ -843,33 +843,33 @@
         self._redback_entities.append(dataDict)
         dataDict = {'value': data['Data']['Nodes'][0]['StaticData']['SoftwareVersion'],'entity_name': 'software_version', 'device_id': id_temp, 'device_type': 'battery'}
         self._redback_entities.append(dataDict)
         dataDict = {'value': data['Data']['Nodes'][0]['StaticData']['FirmwareVersion'],'entity_name': 'firmware_version', 'device_id': id_temp, 'device_type': 'battery'}
         self._redback_entities.append(dataDict)
         dataDict = {'value': data['Data']['Nodes'][0]['StaticData']['Id'],'entity_name': 'inverter_serial_number', 'device_id': id_temp, 'device_type': 'battery'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data2['Data']['TimestampUtc'],'entity_name': 'timestamp_utc', 'device_id': id_temp, 'device_type': 'battery'}
+        dataDict = {'value': (data2['Data']['TimestampUtc']).replace('Z','+00:00'),'entity_name': 'timestamp_utc', 'device_id': id_temp, 'device_type': 'battery'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data2['Data']['BatterySoCInstantaneous0to1'],'entity_name': 'battery_soc_instantaneous_0to1', 'device_id': id_temp, 'device_type': 'battery'}
+        dataDict = {'value': (data2['Data']['BatterySoCInstantaneous0to1'])*100,'entity_name': 'battery_soc_instantaneous_0to1', 'device_id': id_temp, 'device_type': 'battery'}
         self._redback_entities.append(dataDict)
         dataDict = {'value': data2['Data']['BatteryPowerNegativeIsChargingkW'],'entity_name': 'battery_power_negative_is_charging_kw', 'device_id': id_temp, 'device_type': 'battery'}
         self._redback_entities.append(dataDict)
-        if data2['Data']['BatteryChargeAllTimeEnergykWh'] != None:
+        if data2['Data']['BatteryChargeAllTimeEnergykWh'] is not None:
             dataDict = {'value': (data2['Data']['BatteryChargeAllTimeEnergykWh'])/1000,'entity_name': 'battery_charge_all_time_energy_mwh', 'device_id': id_temp, 'device_type': 'battery'}
         else:
             dataDict = {'value': data2['Data']['BatteryChargeAllTimeEnergykWh'],'entity_name': 'battery_charge_all_time_energy_mwh', 'device_id': id_temp, 'device_type': 'battery'}
         self._redback_entities.append(dataDict)
-        if data2['Data']['BatteryDischargeAllTimeEnergykWh'] != None:
+        if data2['Data']['BatteryDischargeAllTimeEnergykWh'] is not None:
             dataDict = {'value': (data2['Data']['BatteryDischargeAllTimeEnergykWh'])/1000,'entity_name': 'battery_discharge_all_time_energy_mwh', 'device_id': id_temp, 'device_type': 'battery'}
         else:
             dataDict = {'value': data2['Data']['BatteryDischargeAllTimeEnergykWh'],'entity_name': 'battery_discharge_all_time_energy_mwh', 'device_id': id_temp, 'device_type': 'battery'}
         self._redback_entities.append(dataDict)
         dataDict = {'value': data2['Data']['Status'],'entity_name': 'status', 'device_id': id_temp, 'device_type': 'battery'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data2['Data']['Battery']['CurrentNegativeIsChargingA'],'entity_name': 'battery_current_negative_in_charging_a', 'device_id': id_temp, 'device_type': 'battery'}
+        dataDict = {'value': data2['Data']['Battery']['CurrentNegativeIsChargingA'],'entity_name': 'battery_current_negative_is_charging_a', 'device_id': id_temp, 'device_type': 'battery'}
         self._redback_entities.append(dataDict)
         dataDict = {'value': data2['Data']['Battery']['VoltageV'],'entity_name': 'battery_voltage_v', 'device_id': id_temp, 'device_type': 'battery'}
         self._redback_entities.append(dataDict)
         dataDict = {'value': data2['Data']['Battery']['VoltageType'],'entity_name': 'battery_voltage_type', 'device_id': id_temp, 'device_type': 'battery'}
         self._redback_entities.append(dataDict)
         dataDict = {'value': data2['Data']['Battery']['NumberOfModules'],'entity_name': 'battery_no_of_modules', 'device_id': id_temp, 'device_type': 'battery'}
         self._redback_entities.append(dataDict)
@@ -901,15 +901,15 @@
             
             battery_temp_value = data2['Data']['Battery']['Modules'][batteryId-1]['PowerNegativeIsChargingkW']
             battery_power_kw += battery_temp_value
             battery_temp_name= f'battery_{batteryId}_power_negative_is_charging_kw'
             dataDict = {'value': battery_temp_value,'entity_name': battery_temp_name, 'device_id': id_temp, 'device_type': 'battery'}
             self._redback_entities.append(dataDict)
             
-            battery_temp_value = data2['Data']['Battery']['Modules'][batteryId-1]['SoC0To1']
+            battery_temp_value = (data2['Data']['Battery']['Modules'][batteryId-1]['SoC0To1'])*100
             battery_temp_name= f'battery_{batteryId}_soc_0to1'
             dataDict = {'value': battery_temp_value,'entity_name': battery_temp_name, 'device_id': id_temp, 'device_type': 'battery'}
             self._redback_entities.append(dataDict)
             batteryId += 1
             
         dataDict = {'value': battery_current_a,'entity_name': 'battery_current_negative_is_charging_a', 'device_id': id_temp, 'device_type': 'battery'}
         self._redback_entities.append(dataDict)
```

### Comparing `redbacktechpy-2024.5.1b8/src/redbacktechpy/str_enum.py` & `redbacktechpy-2024.5.1b9/src/redbacktechpy/str_enum.py`

 * *Files identical despite different names*

### Comparing `redbacktechpy-2024.5.1b8/src/redbacktechpy.egg-info/PKG-INFO` & `redbacktechpy-2024.5.1b9/src/redbacktechpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redbacktechpy
-Version: 2024.5.1b8
+Version: 2024.5.1b9
 Summary: Python Module to support Home Asssistant integration with Redback Technologies Smart Hybrid Inverter
 Author-email: Chris Abberley <unlisted@gmail.com>
 Project-URL: Homepage, https://github.com/cabberley/redbacktechpy
 Project-URL: Issues, https://github.com/cabberley/redbacktechpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

