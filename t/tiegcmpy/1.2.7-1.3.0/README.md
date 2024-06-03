# Comparing `tmp/tiegcmpy-1.2.7.tar.gz` & `tmp/tiegcmpy-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiegcmpy-1.2.7.tar", last modified: Tue Apr 23 17:14:56 2024, max compression
+gzip compressed data, was "tiegcmpy-1.3.0.tar", last modified: Mon Jun  3 06:52:35 2024, max compression
```

## Comparing `tiegcmpy-1.2.7.tar` & `tiegcmpy-1.3.0.tar`

### file list

```diff
@@ -1,24 +1,21 @@
-drwxr-xr-x   0 nikhilr  (42271) ncar      (1000)        0 2024-04-23 17:14:56.166971 tiegcmpy-1.2.7/
--rw-r--r--   0 nikhilr  (42271) ncar      (1000)    16517 2024-04-23 17:14:56.166030 tiegcmpy-1.2.7/PKG-INFO
--rw-r--r--   0 nikhilr  (42271) ncar      (1000)    16164 2023-12-19 19:29:40.000000 tiegcmpy-1.2.7/README.md
--rw-r--r--   0 nikhilr  (42271) ncar      (1000)       38 2024-04-23 17:14:56.167057 tiegcmpy-1.2.7/setup.cfg
--rw-r--r--   0 nikhilr  (42271) ncar      (1000)      810 2024-04-23 17:13:28.000000 tiegcmpy-1.2.7/setup.py
-drwxr-xr-x   0 nikhilr  (42271) ncar      (1000)        0 2024-04-23 17:14:54.035626 tiegcmpy-1.2.7/src/
-drwxr-xr-x   0 nikhilr  (42271) ncar      (1000)        0 2024-04-23 17:14:56.097859 tiegcmpy-1.2.7/src/tiegcmpy/
--rw-r--r--   0 nikhilr  (42271) ncar      (1000)      280 2023-12-19 18:21:34.000000 tiegcmpy-1.2.7/src/tiegcmpy/__init__.py
--rw-r--r--   0 nikhilr  (42271) ncar      (1000)     1984 2023-10-18 21:02:51.000000 tiegcmpy-1.2.7/src/tiegcmpy/convert_units.py
--rwxr-xr-x   0 nikhilr  (42271) ncar      (1000)    42106 2023-12-06 02:37:57.000000 tiegcmpy-1.2.7/src/tiegcmpy/data_parse copy.py
--rwxr-xr-x   0 nikhilr  (42271) ncar      (1000)    51281 2024-04-21 22:58:17.000000 tiegcmpy-1.2.7/src/tiegcmpy/data_parse.py
--rwxr-xr-x   0 nikhilr  (42271) ncar      (1000)    43845 2023-12-04 20:38:48.000000 tiegcmpy-1.2.7/src/tiegcmpy/data_parse_old.py
--rwxr-xr-x   0 nikhilr  (42271) ncar      (1000)    16097 2023-12-19 20:29:36.000000 tiegcmpy-1.2.7/src/tiegcmpy/getoptions.py
--rw-r--r--   0 nikhilr  (42271) ncar      (1000)      683 2023-12-19 18:20:02.000000 tiegcmpy-1.2.7/src/tiegcmpy/io.py
--rwxr-xr-x   0 nikhilr  (42271) ncar      (1000)     7391 2023-12-19 20:00:08.000000 tiegcmpy-1.2.7/src/tiegcmpy/main.py
--rwxr-xr-x   0 nikhilr  (42271) ncar      (1000)    35239 2023-12-05 15:26:08.000000 tiegcmpy-1.2.7/src/tiegcmpy/plot_gen copy.py
--rwxr-xr-x   0 nikhilr  (42271) ncar      (1000)    45099 2024-04-23 13:59:20.000000 tiegcmpy-1.2.7/src/tiegcmpy/plot_gen.py
-drwxr-xr-x   0 nikhilr  (42271) ncar      (1000)        0 2024-04-23 17:14:56.165511 tiegcmpy-1.2.7/src/tiegcmpy.egg-info/
--rw-r--r--   0 nikhilr  (42271) ncar      (1000)    16517 2024-04-23 17:14:52.000000 tiegcmpy-1.2.7/src/tiegcmpy.egg-info/PKG-INFO
--rw-r--r--   0 nikhilr  (42271) ncar      (1000)      503 2024-04-23 17:14:52.000000 tiegcmpy-1.2.7/src/tiegcmpy.egg-info/SOURCES.txt
--rw-r--r--   0 nikhilr  (42271) ncar      (1000)        1 2024-04-23 17:14:52.000000 tiegcmpy-1.2.7/src/tiegcmpy.egg-info/dependency_links.txt
--rw-r--r--   0 nikhilr  (42271) ncar      (1000)       86 2024-04-23 17:14:52.000000 tiegcmpy-1.2.7/src/tiegcmpy.egg-info/entry_points.txt
--rw-r--r--   0 nikhilr  (42271) ncar      (1000)       32 2024-04-23 17:14:52.000000 tiegcmpy-1.2.7/src/tiegcmpy.egg-info/requires.txt
--rw-r--r--   0 nikhilr  (42271) ncar      (1000)        9 2024-04-23 17:14:52.000000 tiegcmpy-1.2.7/src/tiegcmpy.egg-info/top_level.txt
+drwxr-xr-x   0 nikhilr  (42271) ncar      (1000)        0 2024-06-03 06:52:35.143052 tiegcmpy-1.3.0/
+-rw-r--r--   0 nikhilr  (42271) ncar      (1000)      515 2024-06-03 06:52:35.142447 tiegcmpy-1.3.0/PKG-INFO
+-rw-r--r--   0 nikhilr  (42271) ncar      (1000)      163 2024-06-03 06:52:11.000000 tiegcmpy-1.3.0/README.md
+-rw-r--r--   0 nikhilr  (42271) ncar      (1000)       38 2024-06-03 06:52:35.143120 tiegcmpy-1.3.0/setup.cfg
+-rw-r--r--   0 nikhilr  (42271) ncar      (1000)      810 2024-06-03 06:52:31.000000 tiegcmpy-1.3.0/setup.py
+drwxr-xr-x   0 nikhilr  (42271) ncar      (1000)        0 2024-06-03 06:52:35.134781 tiegcmpy-1.3.0/src/
+drwxr-xr-x   0 nikhilr  (42271) ncar      (1000)        0 2024-06-03 06:52:35.137702 tiegcmpy-1.3.0/src/tiegcmpy/
+-rw-r--r--   0 nikhilr  (42271) ncar      (1000)      312 2024-06-03 06:00:35.000000 tiegcmpy-1.3.0/src/tiegcmpy/__init__.py
+-rw-r--r--   0 nikhilr  (42271) ncar      (1000)     1984 2024-06-03 04:10:25.000000 tiegcmpy-1.3.0/src/tiegcmpy/convert_units.py
+-rwxr-xr-x   0 nikhilr  (42271) ncar      (1000)    53125 2024-06-03 06:00:22.000000 tiegcmpy-1.3.0/src/tiegcmpy/data_parse.py
+-rwxr-xr-x   0 nikhilr  (42271) ncar      (1000)    16097 2024-06-03 04:10:25.000000 tiegcmpy-1.3.0/src/tiegcmpy/getoptions.py
+-rw-r--r--   0 nikhilr  (42271) ncar      (1000)      683 2024-06-03 04:10:25.000000 tiegcmpy-1.3.0/src/tiegcmpy/io.py
+-rwxr-xr-x   0 nikhilr  (42271) ncar      (1000)     7391 2024-06-03 04:10:25.000000 tiegcmpy-1.3.0/src/tiegcmpy/main.py
+-rwxr-xr-x   0 nikhilr  (42271) ncar      (1000)    44716 2024-06-03 06:17:35.000000 tiegcmpy-1.3.0/src/tiegcmpy/plot_gen.py
+drwxr-xr-x   0 nikhilr  (42271) ncar      (1000)        0 2024-06-03 06:52:35.141198 tiegcmpy-1.3.0/src/tiegcmpy.egg-info/
+-rw-r--r--   0 nikhilr  (42271) ncar      (1000)      515 2024-06-03 06:52:35.138484 tiegcmpy-1.3.0/src/tiegcmpy.egg-info/PKG-INFO
+-rw-r--r--   0 nikhilr  (42271) ncar      (1000)      410 2024-06-03 06:52:35.139079 tiegcmpy-1.3.0/src/tiegcmpy.egg-info/SOURCES.txt
+-rw-r--r--   0 nikhilr  (42271) ncar      (1000)        1 2024-06-03 06:52:35.139584 tiegcmpy-1.3.0/src/tiegcmpy.egg-info/dependency_links.txt
+-rw-r--r--   0 nikhilr  (42271) ncar      (1000)       86 2024-06-03 06:52:35.140211 tiegcmpy-1.3.0/src/tiegcmpy.egg-info/entry_points.txt
+-rw-r--r--   0 nikhilr  (42271) ncar      (1000)       32 2024-06-03 06:52:35.140668 tiegcmpy-1.3.0/src/tiegcmpy.egg-info/requires.txt
+-rw-r--r--   0 nikhilr  (42271) ncar      (1000)        9 2024-06-03 06:52:35.141293 tiegcmpy-1.3.0/src/tiegcmpy.egg-info/top_level.txt
```

### Comparing `tiegcmpy-1.2.7/setup.py` & `tiegcmpy-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='tiegcmpy',
-    version='1.2.7',
+    version='1.3.0',
     author = "Nikhil Rao",
     author_email = "nikhilr@ucar.edu",
     description='A Python3 post processing tool for TIE-GCM',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/NCAR/tiegcm', 
     python_requires='>=3.8',
```

### Comparing `tiegcmpy-1.2.7/src/tiegcmpy/convert_units.py` & `tiegcmpy-1.3.0/src/tiegcmpy/convert_units.py`

 * *Files identical despite different names*

### Comparing `tiegcmpy-1.2.7/src/tiegcmpy/data_parse copy.py` & `tiegcmpy-1.3.0/src/tiegcmpy/data_parse.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,38 +5,38 @@
 from .convert_units import convert_units
 
 
 
 
 def time_list(datasets):
     """
-    Reads all the datasets and reutrns the timestamps listed in there.
-    
-    Args:
-    - datasets (xarray): The loaded dataset opened using xarray.
+    Compiles and returns a list of all timestamps present in the provided datasets. 
+    This function is particularly useful for aggregating time data from multiple sources.
+
+    Parameters:
+    - datasets (list of tuples): Each tuple in the list contains an xarray dataset and its corresponding filename. 
+      The function will iterate through each dataset to gather timestamps.
 
     Returns:
-    - timestamps (array): An array of numpy datimetime64 timestamps for all the time entries in the datasets.
+    - timestamps (list of np.datetime64): A list containing all the datetime64 timestamps found in the datasets.
     """
     
     # Extract timestamps from each file
     timestamps = []
     for ds, filename in datasets:
         file = str(filename)
         for timestamp in ds['time'].values:
-            #mtime=str(get_mtime(ds,timestamp))
-            #timestamps.append((str(timestamp),mtime,file))
             timestamps.append(timestamp)
     return timestamps
 
 def var_list(datasets):
     """
     Reads all the datasets and reutrns the variables listed in there.
     
-    Args:
+    Parameters:
     - datasets (xarray): The loaded dataset opened using xarray.
 
     Returns:
     - variables (array): An array of variable entries in the datasets.
     """
     
     unique_variables = set()
@@ -45,42 +45,149 @@
         # Convert the current dataset's variables to a set
         current_variables = set(ds.data_vars)
         # Union the current variables with the existing unique variables
         unique_variables = unique_variables.union(current_variables)
     variables = sorted(unique_variables)
     return variables    
 
-def var_time (datasets, variable_name, selected_time, selected_unit=None):
+def level_list(datasets):
+    """
+    Reads all the datasets and returns the unique lev and ilev entries in sorted order.
+    
+    Parameters:
+    - datasets (list of tuples): A list of tuples, where each tuple contains an xarray dataset and its filename.
+
+    Returns:
+    - lev_ilevs (list): A sorted list of unique lev and ilev entries from the datasets.
+    """
+    
+    unique_levels = set()
+
+    for ds, filename in datasets:
+        # Get lev and ilev values and add them to the set
+        levs = ds.lev.values
+        ilevs = ds.ilev.values
+        unique_levels.update(levs)
+        unique_levels.update(ilevs)
+
+    # Convert the set to a sorted list
+    lev_ilevs = sorted(unique_levels)
+    return lev_ilevs
+
+def lon_list(datasets):
+    """
+    Reads all the datasets and returns the unique longitude (lon) entries in sorted order.
+    
+    Parameters:
+    - datasets (list of tuples): A list of tuples, where each tuple contains an xarray dataset and its filename.
+
+    Returns:
+    - lons (list): A sorted list of unique longitude entries from the datasets.
+    """
+    
+    unique_lons = set()
+
+    for ds, filename in datasets:
+        # Get longitude values and add them to the set
+        lons = ds.lon.values
+        unique_lons.update(lons)
+
+    # Convert the set to a sorted list
+    lons = sorted(unique_lons)
+    return lons
+
+def lat_list(datasets):
+    """
+    Reads all the datasets and returns the unique latitude (lat) entries in sorted order.
+    
+    Parameters:
+    - datasets (list of tuples): A list of tuples, where each tuple contains an xarray dataset and its filename.
+
+    Returns:
+    - lats (list): A sorted list of unique latitude entries from the datasets.
+    """
+    
+    unique_lats = set()
+
+    for ds, filename in datasets:
+        # Get latitude values and add them to the set
+        lats = ds.lat.values
+        unique_lats.update(lats)
+
+    # Convert the set to a sorted list
+    lats = sorted(unique_lats)
+    return lats
+
+def arr_var (datasets, variable_name, time, selected_unit=None, plot_mode = False):
+    """
+    Extracts and processes data for a given variable at a specific time from multiple datasets. 
+    It also handles unit conversion and provides additional information if needed for plotting.
+
+    Args:
+    - datasets (list of tuples): Each tuple contains an xarray dataset and its filename. The function will search each dataset for the specified time and variable.
+    - variable_name (str): The name of the variable to be extracted.
+    - time (np.datetime64/str): The specific time for which data is to be extracted.
+    - selected_unit (str, optional): The desired unit for the variable. If None, the original unit is used.
+    - plot_mode (bool, optional): If True, the function returns additional data useful for plotting.
+
+    Returns:
+    - If plot_mode is False, returns only the variable values as a numpy array.
+    - If plot_mode is True, returns a tuple containing:
+        - variable_values (numpy array): The extracted variable values.
+        - levs_ilevs (numpy array): The corresponding level or ilevel values.
+        - variable_unit (str): The unit of the variable after conversion (if applicable).
+        - variable_long_name (str): The long descriptive name of the variable.
+        - selected_ut (float): Universal Time value in hours for the specified time.
+        - selected_mtime (array): Model time array corresponding to the specified time.
+        - filename (str): The name of the dataset file from which data is extracted.
+    """
     for ds, filenames in datasets:
-        if selected_time in ds['time'].values:
+        if time in ds['time'].values:
             # Extract variable attributes
             variable_unit = ds[variable_name].attrs.get('units', 'N/A')
+            if variable_unit == 'cm/s' and selected_unit == None:
+                selected_unit = 'm/s'
             variable_long_name = ds[variable_name].attrs.get('long_name', 'N/A')
-            selected_ut = ds['ut'].sel(time=selected_time).values.item() / (1e9 * 3600)
-            selected_mtime = get_mtime(ds,selected_time)
+            selected_ut = ds['ut'].sel(time=time).values.item() / (1e9 * 3600)
+            selected_mtime = get_mtime(ds,time)
             filename = filenames
-            data = ds[variable_name].sel(time=selected_time)
+            data = ds[variable_name].sel(time=time)
 
             not_all_nan_indices = ~np.isnan(data.values).all(axis=1)
             variable_values = data.values[not_all_nan_indices, :]
 
             if selected_unit != None:
                 variable_values ,variable_unit  = convert_units (variable_values, variable_unit, selected_unit)
                 
 
             try:
                 levs_ilevs = data.lev.values[not_all_nan_indices]
             except:
                 levs_ilevs = data.ilev.values[not_all_nan_indices]
 
-            return(variable_values, levs_ilevs, variable_unit, variable_long_name, selected_ut, selected_mtime, filename)
-    print(f"{selected_time} not found.")
+            if plot_mode == True:
+                return(variable_values, levs_ilevs, variable_unit, variable_long_name, selected_ut, selected_mtime, filename)
+            else:
+                return variable_values
+    print(f"{time} not found.")
     return None
 
 def check_var_dims(ds, variable_name):
+    """
+    Checks the dimensions of a given variable in a dataset to determine if it includes specific dimensions ('lev' or 'ilev').
+
+    Args:
+    - ds (xarray): The dataset in which the variable's dimensions are to be checked.
+    - variable_name (str): The name of the variable for which dimensions are being checked.
+
+    Returns:
+    - str: Returns 'lev' if the variable includes the 'lev' dimension, 'ilev' if it includes the 'ilev' dimension, 
+           'Variable not found in dataset' if the variable does not exist in the dataset, and None if neither 'lev' nor 'ilev' are dimensions of the variable.
+    """
+
     # Check if the variable exists in the dataset
     if variable_name in ds:
         # Get the dimensions of the variable
         var_dims = ds[variable_name].dims
 
         # Check for 'lev' and 'ilev' in dimensions
         if 'lev' in var_dims:
@@ -88,253 +195,302 @@
         elif 'ilev' in var_dims:
             return 'ilev'
         else:
             return None
     else:
         return 'Variable not found in dataset'
 
-def arr_lev_lon (datasets, variable_name, selected_time, selected_lat, selected_unit= None, plot_mode = False):
+def arr_lev_lon (datasets, variable_name, time, selected_lat, selected_unit= None, plot_mode = False):
     """
-    Extract data from the dataset based on the given variable name, timestamp, and lev value.
+    Extracts and processes data from the dataset based on a specific variable, time, and latitude.
     
-    Args:
+    Parameters:
     - datasets (xarray): The loaded dataset opened using xarray.
     - variable_name (str): Name of the variable to extract.
-    - selected_time (str): Timestamp to filter the data.
-    - selected_lev (float): Level value to filter the data.
+    - time (str/numpy.datetime64): Timestamp to filter the data.
+    - selected_lat (float): Latitude value to filter the data.
+    - selected_unit (str, optional): Desired unit to convert the data to. If None, uses the original unit.
+    - plot_mode (bool, optional): If True, returns additional information for plotting.
     
     Returns:
-    - variable_values (xarray): An xarray object of variable values for the given timestamp and latitude.
-    - lons (xarray): An xarray object of longitude values.
-    - levs_ilevs (xarray): An xarray object of selected lev or ilev values.
-    - variable_unit (str): Unit of the variable.
-    - variable_long_name (str): Long name of the variable.
-    - selected_ut (float): UT value in hours for selected_time.
-    - selected_mtime (array): An array containing Day, Hour, Min of the model run
+    - If plot_mode is False: An xarray object containing the variable values for the specified time and latitude.
+    - If plot_mode is True: A tuple containing:
+        - variable_values (xarray): Array of variable values for the specified time and latitude.
+        - lons (xarray): Array of longitude values corresponding to the variable values.
+        - levs_ilevs (xarray): Array of level or ilevel values where data is not NaN.
+        - selected_lat (float): The latitude value used for data selection.
+        - variable_unit (str): Unit of the variable after conversion (if applicable).
+        - variable_long_name (str): Long descriptive name of the variable.
+        - selected_ut (float): Universal Time value in hours for the specified time.
+        - selected_mtime (array): Array containing Day, Hour, Min of the model run.
+        - filename (str): Name of the dataset file from which data is extracted.
     """
     
     
-    # Load the dataset using xarray
-    #ds = xr.open_dataset(dataset)   
+
+    # Convert time from string to numpy datetime64 format
+    if isinstance(time, str):
+        time = np.datetime64(time, 'ns')
+
+    # Iterate over datasets to find the matching time and extract relevant data
     for ds, filenames in datasets:
-        if selected_time in ds['time'].values:
-            # Extract variable attributes
+        if time in ds['time'].values:
+            # Extracting variable attributes and time information
             variable_unit = ds[variable_name].attrs.get('units', 'N/A')
+            if variable_unit == 'cm/s' and selected_unit == None:
+                selected_unit = 'm/s'
             variable_long_name = ds[variable_name].attrs.get('long_name', 'N/A')
-            selected_ut = ds['ut'].sel(time=selected_time).values.item() / (1e9 * 3600)
-            selected_mtime = get_mtime(ds,selected_time)
+            selected_ut = ds['ut'].sel(time=time).values.item() / (1e9 * 3600)
+            selected_mtime = get_mtime(ds,time)
             filename = filenames
+            # Data selection based on latitude
             if selected_lat == "mean":
-                # if selected_lon is "mean", then we calculate the mean over all longitudes.
-                data = ds[variable_name].sel(time=selected_time).mean(dim='lat')
+                # Averaging over all latitudes
+                data = ds[variable_name].sel(time=time).mean(dim='lat')
             else:
-                data = ds[variable_name].sel(time=selected_time, lat=selected_lat, method='nearest')
+                # Nearest latitude selection
+                data = ds[variable_name].sel(time=time, lat=selected_lat, method='nearest')
             lons = data.lon.values
 
+            # Filtering non-NaN data
             not_all_nan_indices = ~np.isnan(data.values).all(axis=1)
             variable_values = data.values[not_all_nan_indices, :]
 
+            # Unit conversion if a different unit is specified
             if selected_unit != None:
-                variable_values ,variable_unit  = convert_units (variable_values, variable_unit, selected_unit)
-                
+                variable_values, variable_unit = convert_units(variable_values, variable_unit, selected_unit)
 
+            # Extracting level or ilevel values
             try:
                 levs_ilevs = data.lev.values[not_all_nan_indices]
             except:
                 levs_ilevs = data.ilev.values[not_all_nan_indices]
-  
+
+            # Conditional return based on plot_mode
             if plot_mode == True:    
                 return variable_values, lons, levs_ilevs, selected_lat, variable_unit, variable_long_name, selected_ut, selected_mtime, filename
             else:
                 return variable_values
-    print(f"{selected_time} not found.")
+
+    # Handling cases where the specified time is not found in the dataset
+    print(f"{time} not found.")
     return None
 
 
 
-def arr_lat_lon(datasets, variable_name, selected_time, selected_lev_ilev = None, selected_unit = None, plot_mode = False):
+def arr_lat_lon(datasets, variable_name, time, selected_lev_ilev = None, selected_unit = None, plot_mode = False):
+    """
+    Extracts data from the dataset based on the specified variable, time, and level (lev/ilev).
+
+    Parameters:
+    - datasets (xarray): The loaded dataset/s using xarray.
+    - variable_name (str): Name of the variable to extract.
+    - time (str/numpy.datetime64): Timestamp to filter the data.
+    - selected_lev_ilev (float/str, optional): Level value to filter the data. If 'mean', calculates the mean over all levels.
+    - selected_unit (str, optional): Desired unit to convert the data to. If None, uses the original unit.
+    - plot_mode (bool, optional): If True, returns additional information for plotting.
+
+    Returns:
+    - If plot_mode is False: An xarray object containing the variable values for the specified time and level.
+    - If plot_mode is True: A tuple containing:
+        - variable_values (xarray): Array of variable values for the specified time and level.
+        - selected_lev_ilev (float/str): The level value used for data selection.
+        - lats (xarray): Array of latitude values corresponding to the variable values.
+        - lons (xarray): Array of longitude values corresponding to the variable values.
+        - variable_unit (str): Unit of the variable after conversion (if applicable).
+        - variable_long_name (str): Long descriptive name of the variable.
+        - selected_ut (float): Universal Time value in hours for the specified time.
+        - selected_mtime (array): Array containing Day, Hour, Min of the model run.
+        - filename (str): Name of the dataset file from which data is extracted.
+    """
     if selected_lev_ilev != None:
         selected_lev_ilev = float(selected_lev_ilev)
-    if isinstance(selected_time, str):
-        selected_time = np.datetime64(selected_time, 'ns')
+    if isinstance(time, str):
+        time = np.datetime64(time, 'ns')
     first_pass = True
     for ds, filenames in datasets:
         if first_pass == True:
             lev_ilev = check_var_dims(ds, variable_name)
         if lev_ilev == 'lev':
             first_pass == False
-            if selected_time in ds['time'].values:
+            if time in ds['time'].values:
                 if 'lev' not in ds[variable_name].dims:
                     raise ValueError("The variable "+variable_name+" doesn't use the dimensions 'lat', 'lon', 'lev'")
                     return 0
 
                 # Extract variable attributes
                 variable_unit = ds[variable_name].attrs.get('units', 'N/A')
+                if variable_unit == 'cm/s' and selected_unit == None:
+                    selected_unit = 'm/s'
                 variable_long_name = ds[variable_name].attrs.get('long_name', 'N/A')
-                selected_ut = ds['ut'].sel(time=selected_time).values.item() / (1e9 * 3600)
-                selected_mtime = get_mtime(ds,selected_time)
+                selected_ut = ds['ut'].sel(time=time).values.item() / (1e9 * 3600)
+                selected_mtime = get_mtime(ds,time)
                 filename = filenames
 
 
                 if selected_lev_ilev == "mean":
                     # if selected_lon is "mean", then we calculate the mean over all longitudes.
-                    data = ds[variable_name].sel(time=selected_time).mean(dim='lev')
+                    data = ds[variable_name].sel(time=time).mean(dim='lev')
                     lons = data.lon.values
                     lats = data.lat.values
                     variable_values = data.values
                     if selected_unit != None:
                         variable_values ,variable_unit  = convert_units (variable_values, variable_unit, selected_unit)
                         
                 else:
-                    # Extract the data for the given selected_time and lev
+                    # Extract the data for the given time and lev
                     if selected_lev_ilev in ds['lev'].values:
-                        data = ds[variable_name].sel(time=selected_time, lev=selected_lev_ilev)
+                        data = ds[variable_name].sel(time=time, lev=selected_lev_ilev)
                         lons = data.lon.values
                         lats = data.lat.values
                         variable_values = data.values
                         if selected_unit != None:
                             variable_values ,variable_unit  = convert_units (variable_values, variable_unit, selected_unit)
                             
                     else:
                         print(f"The lev {selected_lev_ilev} isn't in the listed valid values.")
                         lev_max = ds['lev'].max().values.item()
                         lev_min = ds['lev'].min().values.item()
                         if selected_lev_ilev > lev_max:
                             print(f"Using maximun valid lev {lev_max}")
                             selected_lev_ilev = lev_max
-                            data = ds[variable_name].sel(time=selected_time, lev=selected_lev_ilev)
+                            data = ds[variable_name].sel(time=time, lev=selected_lev_ilev)
                             lons = data.lon.values
                             lats = data.lat.values
                             variable_values = data.values
                             if selected_unit != None:
                                 variable_values ,variable_unit  = convert_units (variable_values, variable_unit, selected_unit)
                         elif selected_lev_ilev < lev_min:
                             print(f"Using minimum valid lev {lev_min}")
                             selected_lev_ilev = lev_min
-                            data = ds[variable_name].sel(time=selected_time, lev=selected_lev_ilev)
+                            data = ds[variable_name].sel(time=time, lev=selected_lev_ilev)
                             lons = data.lon.values
                             lats = data.lat.values
                             variable_values = data.values
                             if selected_unit != None:
                                 variable_values ,variable_unit  = convert_units (variable_values, variable_unit, selected_unit)
                         else:
                             sorted_levs = sorted(ds['lev'].values, key=lambda x: abs(x - selected_lev_ilev))
                             closest_lev1 = sorted_levs[0]
                             closest_lev2 = sorted_levs[1]
                             print(f"Averaging from the closest valid levs: {closest_lev1} and {closest_lev2}")
                             # Extract data for the two closest lev values using .sel()
-                            data1 = ds[variable_name].sel(time=selected_time, lev=closest_lev1)
+                            data1 = ds[variable_name].sel(time=time, lev=closest_lev1)
                             lons = data1.lon.values
                             lats = data1.lat.values
                             variable_values_1 = data1.values
 
-                            data2 = ds[variable_name].sel(time=selected_time, lev=closest_lev2)
+                            data2 = ds[variable_name].sel(time=time, lev=closest_lev2)
                             variable_values_2 = data2.values
                             # Return the averaged data
                             variable_values = (variable_values_1 + variable_values_2) / 2
                             if selected_unit != None:
-                                variable_values , selected_unit  = convert_units (variable_values, variable_unit, selected_unit)
+                                variable_values , variable_unit  = convert_units (variable_values, variable_unit, selected_unit)
                 if plot_mode == True:    
                     return variable_values, selected_lev_ilev, lats, lons, variable_unit, variable_long_name, selected_ut, selected_mtime, filename
                 else:
                     return variable_values
 
         elif lev_ilev == 'ilev':
             first_pass == False
-            if selected_time in ds['time'].values:
+            if time in ds['time'].values:
                 if 'ilev' not in ds[variable_name].dims:
                     raise ValueError("The variable "+variable_name+" doesn't use the dimensions 'lat', 'lon', 'ilev'")
                     return 0
                             
                 # Extract variable attributes
                 variable_unit = ds[variable_name].attrs.get('units', 'N/A')
+                if variable_unit == 'cm/s' and selected_unit == None:
+                    selected_unit = 'm/s'
                 variable_long_name = ds[variable_name].attrs.get('long_name', 'N/A')
-                selected_ut = ds['ut'].sel(time=selected_time).values.item() / (1e9 * 3600)
-                selected_mtime=get_mtime(ds,selected_time)
+                selected_ut = ds['ut'].sel(time=time).values.item() / (1e9 * 3600)
+                selected_mtime=get_mtime(ds,time)
                 filename = filenames
 
                 if selected_lev_ilev == "mean":
                     # if selected_lon is "mean", then we calculate the mean over all longitudes.
-                    data = ds[variable_name].sel(time=selected_time).mean(dim='lev')
+                    data = ds[variable_name].sel(time=time).mean(dim='lev')
                     lons = data.lon.values
                     lats = data.lat.values
                     variable_values = data.values
                     if selected_unit != None:
                         variable_values ,variable_unit  = convert_units (variable_values, variable_unit, selected_unit)
                         
                 else:
-                    # Extract the data for the given selected_time and lev
+                    # Extract the data for the given time and lev
                     if selected_lev_ilev in ds['ilev'].values:
-                        data = ds[variable_name].sel(time=selected_time, ilev=selected_lev_ilev)
+                        data = ds[variable_name].sel(time=time, ilev=selected_lev_ilev)
                         lons = data.lon.values
                         lats = data.lat.values
                         variable_values = data.values
                         if selected_unit != None:
                             variable_values ,variable_unit  = convert_units (variable_values, variable_unit, selected_unit)
                             
                     else:
                         
                         print(f"The ilev {selected_lev_ilev} isn't in the listed valid values.")
                         ilev_max = ds['ilev'].max().values.item()
                         ilev_min = ds['ilev'].min().values.item()
                         if selected_lev_ilev > ilev_max:
                             print(f"Using maximun valid ilev {ilev_max}")
                             selected_lev_ilev = ilev_max
-                            data = ds[variable_name].sel(time=selected_time, ilev=selected_lev_ilev)
+                            data = ds[variable_name].sel(time=time, ilev=selected_lev_ilev)
                             lons = data.lon.values
                             lats = data.lat.values
                             variable_values = data.values
                             if selected_unit != None:
                                 variable_values ,variable_unit  = convert_units (variable_values, variable_unit, selected_unit)
                         elif selected_lev_ilev < ilev_min:
                             print(f"Using minimum valid ilev {ilev_min}")
                             selected_lev_ilev = ilev_min
-                            data = ds[variable_name].sel(time=selected_time, ilev=selected_lev_ilev)
+                            data = ds[variable_name].sel(time=time, ilev=selected_lev_ilev)
                             lons = data.lon.values
                             lats = data.lat.values
                             variable_values = data.values
                             if selected_unit != None:
                                 variable_values ,variable_unit  = convert_units (variable_values, variable_unit, selected_unit)
                         else:
                             sorted_levs = sorted(ds['ilev'].values, key=lambda x: abs(x - selected_lev_ilev))
                             closest_lev1 = sorted_levs[0]
                             closest_lev2 = sorted_levs[1]
                             print(f"Averaging from the closest valid ilevs: {closest_lev1} and {closest_lev2}")
                             # Extract data for the two closest lev values using .sel()
-                            data1 = ds[variable_name].sel(time=selected_time, ilev=closest_lev1)
+                            data1 = ds[variable_name].sel(time=time, ilev=closest_lev1)
                             lons = data1.lon.values
                             lats = data1.lat.values
                             variable_values_1 = data1.values
 
-                            data2 = ds[variable_name].sel(time=selected_time, ilev=closest_lev2)
+                            data2 = ds[variable_name].sel(time=time, ilev=closest_lev2)
                             variable_values_2 = data2.values
                             # Return the averaged data
                             variable_values = (variable_values_1 + variable_values_2) / 2
                             if selected_unit != None:
                                 variable_values ,variable_unit  = convert_units (variable_values, variable_unit, selected_unit)
                             
                 if plot_mode == True:    
                     return variable_values, selected_lev_ilev, lats, lons, variable_unit, variable_long_name, selected_ut, selected_mtime, filename
                 else:
                     return variable_values
 
         elif lev_ilev == None:
             first_pass == False
             selected_lev_ilev = None
-            if selected_time in ds['time'].values:
+            if time in ds['time'].values:
 
                 # Extract variable attributes
                 variable_unit = ds[variable_name].attrs.get('units', 'N/A')
+                if variable_unit == 'cm/s' and selected_unit == None:
+                    selected_unit = 'm/s'
                 variable_long_name = ds[variable_name].attrs.get('long_name', 'N/A')
-                selected_ut = ds['ut'].sel(time=selected_time).values.item() / (1e9 * 3600)
-                selected_mtime = get_mtime(ds,selected_time)
+                selected_ut = ds['ut'].sel(time=time).values.item() / (1e9 * 3600)
+                selected_mtime = get_mtime(ds,time)
                 filename = filenames
 
-                # Extract the data for the given selected_time and lev
-                data = ds[variable_name].sel(time=selected_time)
+                # Extract the data for the given time and lev
+                data = ds[variable_name].sel(time=time)
                 lons = data.lon.values
                 lats = data.lat.values
                 variable_values = data.values
                 if selected_unit != None:
                     variable_values ,variable_unit  = convert_units (variable_values, variable_unit, selected_unit)
                 
                 
@@ -342,112 +498,122 @@
                     return variable_values, selected_lev_ilev, lats, lons, variable_unit, variable_long_name, selected_ut, selected_mtime, filename
                 else:
                     return variable_values
 
 
 
     
-def arr_lev_var(datasets, variable_name, selected_time, selected_lat, selected_lon, selected_unit= None, plot_mode = False):
+def arr_lev_var(datasets, variable_name, time, selected_lat, selected_lon, selected_unit= None, plot_mode = False):
     """
     Extracts data from the dataset for a given variable name, latitude, longitude, and time.
-    
+
     Parameters:
-    - ds (xarray): The loaded dataset opened using xarray.
+    - datasets (xarray): The loaded dataset opened using xarray.
     - variable_name (str): Name of the variable to retrieve.
-        - valid variables: ['TN', 'UN', 'VN', 'O2', 'O1', 'N4S', 'NO', 'HE', 'AR', 'OP', 'N2D','TI', 'TE', 'O2P', 'TN_NM', 
-                            'UN_NM', 'VN_NM', 'O2_NM', 'O1_NM', 'N4S_NM', 'NO_NM', 'OP_NM', 'HE_NM', 'AR_NM', 'NE', 'OMEGA', 
-                            'Z', 'POTEN']  
-    - selected_time (str): Timestamp to filter the data.
+    - time (str): Timestamp to filter the data.
     - selected_lat (float): Latitude value.
     - selected_lon (float): Longitude value.
-    - selected_time (int): Index of the time dimension.
+    - selected_unit (str, optional): Desired unit to convert the data to. If None, uses the original unit.
+    - plot_mode (bool, optional): If True, returns additional information for plotting.
     
     Returns:
-    - variable_values (xarray):  An xarray object of variable values for the given timestamp and lev.
-    - levs_ilevs (xarray): An xarray object of selected lev or ilev values.
-    - variable_unit (str): Unit of the variable.
-    - variable_long_name (str): Long name of the variable.
-    - selected_ut (float): UT value in hours for selected_time.
-    - selected_mtime (array): An array containing Day, Hour, Min of the model run.
+    - If plot_mode is True: A tuple containing:
+        - variable_values (xarray): Array of variable values for the specified time and latitude/longitude.
+        - levs_ilevs (xarray): Array of level or ilevel values where data is not NaN.
+        - variable_unit (str): Unit of the variable after conversion (if applicable).
+        - variable_long_name (str): Long descriptive name of the variable.
+        - selected_ut (float): Universal Time value in hours for the specified time.
+        - selected_mtime (array): Array containing Day, Hour, Min of the model run.
+        - filename (str): Name of the dataset file from which data is extracted.
+    - If plot_mode is False: An xarray object containing the variable values.
     """
     
     
     for ds, filenames in datasets:
-        if selected_time in ds['time'].values:
+        if time in ds['time'].values:
 
             if selected_lon == "mean" and selected_lat == "mean":
                 # if selected_lon is "mean", then we calculate the mean over all longitudes.
-                data = ds[variable_name].sel(time=selected_time).mean(dim=['lon', 'lat'])
+                data = ds[variable_name].sel(time=time).mean(dim=['lon', 'lat'])
             elif selected_lon == "mean":
-                data = ds[variable_name].sel(time=selected_time, lat=selected_lat, method="nearest").mean(dim='lon')  #look into method nearest
+                data = ds[variable_name].sel(time=time, lat=selected_lat, method="nearest").mean(dim='lon')  #look into method nearest
             elif selected_lat == "mean":
-                data = ds[variable_name].sel(time=selected_time, lon=selected_lon).mean(dim='lat')
+                data = ds[variable_name].sel(time=time, lon=selected_lon).mean(dim='lat')
             else:
-                data = ds[variable_name].sel(time=selected_time, lat=selected_lat, lon=selected_lon, method="nearest")
+                data = ds[variable_name].sel(time=time, lat=selected_lat, lon=selected_lon, method="nearest")
 
 
             variable_unit = ds[variable_name].attrs.get('units', 'N/A')
+            if variable_unit == 'cm/s' and selected_unit == None:
+                selected_unit = 'm/s'
             variable_long_name = ds[variable_name].attrs.get('long_name', 'N/A')
-            selected_ut = ds['ut'].sel(time=selected_time).values.item() / (1e9 * 3600)
-            selected_mtime=get_mtime(ds,selected_time)
+            selected_ut = ds['ut'].sel(time=time).values.item() / (1e9 * 3600)
+            selected_mtime=get_mtime(ds,time)
             filename = filenames
             valid_indices = ~np.isnan(data.values)
             variable_values = data.values[valid_indices]
             if selected_unit != None:
                 variable_values ,variable_unit  = convert_units (variable_values, variable_unit, selected_unit)
                 
             try:
                 levs_ilevs = ds['lev'].values[valid_indices]
             except:
                 levs_ilevs = ds['ilev'].values[valid_indices]
             if plot_mode == True:
                 return variable_values , levs_ilevs, variable_unit, variable_long_name, selected_ut, selected_mtime, filename
             else:
                 return variable_values 
-    print(f"{selected_time} not found.")
+    print(f"{time} not found.")
     return None
 
 
 
 
-def arr_lev_lat (datasets, variable_name, selected_time, selected_lon, selected_unit=None, plot_mode = False):
+def arr_lev_lat (datasets, variable_name, time, selected_lon, selected_unit=None, plot_mode = False):
     """
-    Extract data from the dataset based on the given variable name, timestamp, and lev value.
-    
-    Args:
-    - ds (xarray): The loaded dataset opened using xarray.
+    Extracts data from a dataset based on the specified variable name, timestamp, and longitude.
+
+    Parameters:
+    - datasets (xarray): The loaded dataset opened using xarray.
     - variable_name (str): Name of the variable to extract.
-        - valid variables: ['TN', 'UN', 'VN', 'O2', 'O1', 'N2', 'NO', 'N4S', 'HE', 'TE', 'TI', 'O2P', 'OP', 'QJOULE']    
-    - selected_time (str): Timestamp to filter the data.
-    - selected_lon (float): Longitude to filter the data.
-    
+    - time (str/numpy.datetime64): Timestamp to filter the data.
+    - selected_lon (float/str): Longitude to filter the data, or 'mean' for averaging over all longitudes.
+    - selected_unit (str, optional): Desired unit to convert the data to. If None, uses the original unit.
+    - plot_mode (bool, optional): If True, returns additional information for plotting.
+
     Returns:
-    - variable_values (xarray): An xarray object of variable values for the given timestamp and latitude.
-    - lats (xarray): An xarray object of latgitude values.
-    - levs_ilevs (xarray): An xarray object of selected lev or ilev values.
-    - variable_unit (str): Unit of the variable.
-    - variable_long_name (str): Long name of the variable.
-    - selected_ut (float): UT value in hours for selected_time.
-    - selected_mtime (array): An array containing Day, Hour, Min of the model run
+    - If plot_mode is False: An xarray object containing the variable values for the specified time and longitude.
+    - If plot_mode is True: A tuple containing:
+        - variable_values (xarray): Array of variable values for the specified time and longitude.
+        - lats (xarray): Array of latitude values corresponding to the variable values.
+        - levs_ilevs (xarray): Array of level or ilevel values where data is not NaN.
+        - variable_unit (str): Unit of the variable after conversion (if applicable).
+        - variable_long_name (str): Long descriptive name of the variable.
+        - selected_ut (float): Universal Time value in hours for the specified time.
+        - selected_mtime (array): Array containing Day, Hour, Min of the model run.
+        - filename (str): Name of the dataset file from which data is extracted.
     """
-    
+    if isinstance(time, str):
+        time = np.datetime64(time, 'ns')
     for ds, filenames in datasets:
-        if selected_time in ds['time'].values:
+        if time in ds['time'].values:
             # Extract variable attributes
             variable_unit = ds[variable_name].attrs.get('units', 'N/A')
+            if variable_unit == 'cm/s' and selected_unit == None:
+                selected_unit = 'm/s'
             variable_long_name = ds[variable_name].attrs.get('long_name', 'N/A')
-            selected_ut = ds['ut'].sel(time=selected_time).values.item() / (1e9 * 3600)
-            selected_mtime = get_mtime(ds,selected_time)
+            selected_ut = ds['ut'].sel(time=time).values.item() / (1e9 * 3600)
+            selected_mtime = get_mtime(ds,time)
             filename = filenames
             if selected_lon == "mean":
                 # if selected_lon is "mean", then we calculate the mean over all longitudes.
-                data = ds[variable_name].sel(time=selected_time).mean(dim='lon')
+                data = ds[variable_name].sel(time=time).mean(dim='lon')
             else:
                 selected_lon = float(selected_lon)
-                data = ds[variable_name].sel(time=selected_time, lon=selected_lon, method='nearest')
+                data = ds[variable_name].sel(time=time, lon=selected_lon, method='nearest')
             lats = data.lat.values
 
             not_all_nan_indices = ~np.isnan(data.values).all(axis=1)
             variable_values = data.values[not_all_nan_indices, :]
             if selected_unit != None:
                 variable_values ,variable_unit  = convert_units (variable_values, variable_unit, selected_unit)
                 
@@ -455,66 +621,101 @@
                 levs_ilevs = data.lev.values[not_all_nan_indices]
             except AttributeError:
                 levs_ilevs = data.ilev.values[not_all_nan_indices]
             if plot_mode == True:
                 return variable_values, lats, levs_ilevs, selected_lon, variable_unit, variable_long_name, selected_ut, selected_mtime,filename
             else:
                 return variable_values
-    print(f"{selected_time} not found.")
+    print(f"{time} not found.")
     return None
 
 
 
 def arr_lev_time (datasets, variable_name, selected_lat, selected_lon, selected_unit = None, plot_mode = False):
     """
-    Extract data from the dataset based on the given variable name, timestamp, and lev value.
+    This function extracts and processes data from multiple datasets based on specified parameters. It focuses on extracting 
+    data across different levels and times for a given latitude and longitude.
+
+    Parameters:
+    - datasets (list of tuples): A list of tuples where each tuple contains an xarray dataset and its filename.
+    - variable_name (str): The name of the variable to be extracted from the dataset.
+    - selected_lat (float/str): The latitude value or 'mean' to average over all latitudes.
+    - selected_lon (float/str): The longitude value or 'mean' to average over all longitudes.
+    - selected_unit (str, optional): The desired unit for the variable. If None, the original unit is used.
+    - plot_mode (bool, optional): If True, the function returns additional data useful for plotting.
     
-    Args:
-    - ds (xarray): The loaded dataset opened using xarray.
-    - variable_name (str): Name of the variable to extract.
-        - valid variables: ['TN', 'UN', 'VN', 'O2', 'O1', 'N4S', 'NO', 'HE', 'AR', 'OP', 'N2D','TI', 'TE', 'O2P', 'TN_NM', 
-                            'UN_NM', 'VN_NM', 'O2_NM', 'O1_NM', 'N4S_NM', 'NO_NM', 'OP_NM', 'HE_NM', 'AR_NM', 'NE', 'OMEGA', 
-                            'Z', 'POTEN'] 
-    - selected_lat (str): Latitude to filter the data.
-    - selected_lon (float): Longitude to filter the data.
-    
-    Returns:
-    - variable_values (xarray): An xarray object of variable values for the given timestamp and latitude.
-    - levs_ilevs (xarray): An xarray object of selected lev or ilev values.
-    - mtime_values (xarray): An xarray object of mtime arrays.
-    - variable_unit (str): Unit of the variable.
-    - variable_long_name (str): Long name of the variable.
-    - selected_ut (float): UT value in hours for selected_time.
-    - selected_mtime (array): An array containing Day, Hour, Min of the model run
+    Returns:
+    - If plot_mode is False, returns a numpy array of variable values concatenated across datasets.
+    - If plot_mode is True, returns a tuple containing:
+        - variable_values_all (numpy array): Concatenated variable values.
+        - levs_ilevs (numpy array): Corresponding level or ilevel values.
+        - mtime_values (list): List of model times.
+        - selected_lon (float/str): The longitude used for data selection.
+        - variable_unit (str): The unit of the variable after conversion (if applicable).
+        - variable_long_name (str): The long descriptive name of the variable.
     """
-    
-    selected_lon = float(selected_lon)
-    
+
+    try:
+        selected_lon = float(selected_lon)
+    except:
+        selected_lon = selected_lon
+    if selected_lon == 180:
+            selected_lon = -180
     variable_values_all = []
     combined_mtime = []
     levs_ilevs_all = []
-    
+    avg_info_print = 0
     for ds, filenames in datasets:
         variable_unit = ds[variable_name].attrs.get('units', 'N/A')
+        if variable_unit == 'cm/s' and selected_unit == None:
+            selected_unit = 'm/s'
         variable_long_name = ds[variable_name].attrs.get('long_name', 'N/A')
         mtime_values = ds['mtime'].values
         if selected_lon == "mean" and selected_lat == "mean":
-
-            # if selected_lon is "mean", then we calculate the mean over all longitudes.
+            # if selected_lon is "mean", then we calculate the mean over all longitudes. This doesn't work fix
             data = ds[variable_name].mean(dim=['lon', 'lat'])
+            variable_values = data.T 
         elif selected_lon == "mean":
-            data = ds[variable_name].sel(lat=selected_lat).mean(dim='lon')
-
+            if selected_lat in ds['lat'].values:
+                data = ds[variable_name].sel(lat=selected_lat).mean(dim='lon')
+                variable_values = data.T 
+            else:
+                sorted_lats = sorted(ds['lat'].values, key=lambda x: abs(x - selected_lat))
+                closest_lat1 = sorted_lats[0]
+                closest_lat2 = sorted_lats[1]
+                if avg_info_print == 0:
+                    print(f"The lat {selected_lat} isn't in the listed valid values.")
+                    print(f"Averaging from the closest valid levs: {closest_lat1} and {closest_lat2}")
+                    avg_info_print = 1
+                data1 = ds[variable_name].sel(lat=closest_lat1, method='nearest').mean(dim='lon')
+                variable_values_1 = data1.T 
+                data2 = ds[variable_name].sel(lat=closest_lat2, method='nearest').mean(dim='lon')
+                variable_values_2 = data2.T 
+                variable_values = (variable_values_1 + variable_values_2) / 2
         elif selected_lat == "mean":
-            data = ds[variable_name].sel(lon=selected_lon).mean(dim='lat')
+            if selected_lon in ds['lon'].values:
+                data = ds[variable_name].sel(lon=selected_lon).mean(dim='lat')
+                variable_values = data.T 
+            else:
+                sorted_lons = sorted(ds['lat'].values, key=lambda x: abs(x - selected_lon))
+                closest_lon1 = sorted_lons[0]
+                closest_lon2 = sorted_lons[1]
+                if avg_info_print == 0:
+                    print(f"The lon {selected_lon} isn't in the listed valid values.")
+                    print(f"Averaging from the closest valid levs: {closest_lon1} and {closest_lon2}")
+                    avg_info_print = 1
+                data1 = ds[variable_name].sel(lon=closest_lon1, method='nearest').mean(dim='lat')
+                variable_values_1 = data1.T 
+                data2 = ds[variable_name].sel(lon=closest_lon2, method='nearest').mean(dim='lat')
+                variable_values_2 = data2.T 
+                variable_values = (variable_values_1 + variable_values_2) / 2
         else:
-            #data = ds[variable_name].sel(time=selected_time, lat=selected_lat, lon=selected_lon, method="nearest")    
+            #data = ds[variable_name].sel(time=time, lat=selected_lat, lon=selected_lon, method="nearest")    
             data = ds[variable_name].sel(lat=selected_lat, lon=selected_lon, method='nearest')
-
-        variable_values = data.T 
+            variable_values = data.T 
         try:
             levs_ilevs = data.lev.values
         except:
             levs_ilevs = data.ilev.values
     
         # Adjusting levs_ilevs to match the shape of variable_values
         levs_ilevs = levs_ilevs[:variable_values.shape[0]]
@@ -539,37 +740,60 @@
 
     if plot_mode == True:
         return variable_values_all, levs_ilevs, mtime_values, selected_lon, variable_unit, variable_long_name
     else:
         return variable_values_all
 
 def arr_lat_time(datasets, variable_name, selected_lon,selected_lev_ilev = None, selected_unit = None, plot_mode = False):
+    """
+    Extracts and processes data from the dataset based on the specified variable name, longitude, and level/ilev.
+    
+    Parameters:
+    - datasets (list of tuples): Each tuple contains an xarray dataset and its filename.
+    - variable_name (str): The name of the variable to extract.
+    - selected_lon (float/str): Longitude value or 'mean' to average over all longitudes.
+    - selected_lev_ilev (float/str/None): Level or intermediate level value or 'mean' for averaging, or None if not applicable.
+    - selected_unit (str, optional): The desired unit for the variable. If None, the original unit is used.
+    - plot_mode (bool, optional): If True, returns additional data useful for plotting.
     
+    Returns:
+    - If plot_mode is False, returns a numpy array of variable values concatenated across datasets.
+    - If plot_mode is True, returns a tuple containing:
+        - variable_values_all (numpy array): Concatenated variable values.
+        - lats (numpy array): Latitude values corresponding to the variable values.
+        - mtime_values (list): List of model times.
+        - selected_lon (float/str): The longitude used for data selection.
+        - variable_unit (str): The unit of the variable after conversion (if applicable).
+        - variable_long_name (str): The long descriptive name of the variable.
+        - filename (str): Name of the dataset file from which data is extracted.
+    """
     if selected_lev_ilev != 'mean' and selected_lev_ilev != None:
         selected_lev_ilev = float(selected_lev_ilev)
     if selected_lon !='mean':
         selected_lon = float(selected_lon)
     first_pass = True
     variable_values_all = []
     combined_mtime = []
     lats_all = []
     avg_info_print = 0
+
     for ds, filenames in datasets:
         if first_pass == True:
             lev_ilev = check_var_dims(ds, variable_name)
         if lev_ilev == 'lev':
             first_pass == False            
             if 'lev' not in ds[variable_name].dims:
                 raise ValueError("The variable "+variable_name+" doesn't use the dimensions 'lat', 'lon', 'lev'")
                 return 0
             variable_unit = ds[variable_name].attrs.get('units', 'N/A')
+            if variable_unit == 'cm/s' and selected_unit == None:
+                selected_unit = 'm/s'
             variable_long_name = ds[variable_name].attrs.get('long_name', 'N/A')
             mtime_values = ds['mtime'].values
             filename = filenames
-
             if selected_lon == 'mean' and selected_lev_ilev == 'mean':
                 data = ds[variable_name].sel(method='nearest').mean(dim=['lev', 'lon'])
                 variable_values = data.T 
                 lats = data.lat.values    
                 lats_all = lats_all[:variable_values.shape[0]]
             if selected_lon =='mean' and selected_lev_ilev != 'mean':
                 if selected_lev_ilev in ds['lev'].values:
@@ -618,23 +842,23 @@
                     data2 = ds[variable_name].sel(lev=closest_lev2, lon=selected_lon, method='nearest')
                     variable_values_2 = data2.T 
                     variable_values = (variable_values_1 + variable_values_2) / 2
             variable_values_all.append(variable_values)
             combined_mtime.extend(mtime_values)
             lats_all.append(lats)
         
-
         elif lev_ilev == 'ilev':
             first_pass == False
-            
             avg_info_print = 0
             if 'ilev' not in ds[variable_name].dims:
                 raise ValueError("The variable "+variable_name+" doesn't use the dimensions 'lat', 'lon', 'ilev'")
                 return 0
             variable_unit = ds[variable_name].attrs.get('units', 'N/A')
+            if variable_unit == 'cm/s' and selected_unit == None:
+                selected_unit = 'm/s'
             variable_long_name = ds[variable_name].attrs.get('long_name', 'N/A')
             mtime_values = ds['mtime'].values
             filename = filenames
             
             if selected_lon == 'mean' and selected_lev_ilev == 'mean':
                 data = ds[variable_name].sel(method='nearest').mean(dim=['ilev', 'lon'])
                 variable_values = data.T 
@@ -695,14 +919,16 @@
 
         elif lev_ilev == None:
             first_pass == False
             selected_lev_ilev = None
 
             avg_info_print = 0
             variable_unit = ds[variable_name].attrs.get('units', 'N/A')
+            if variable_unit == 'cm/s' and selected_unit == None:
+                selected_unit = 'm/s'
             variable_long_name = ds[variable_name].attrs.get('long_name', 'N/A')
             mtime_values = ds['mtime'].values
             filename = filenames
 
             if selected_lon =='mean':
                 data = ds[variable_name].sel(method='nearest').mean(dim='lon')
                 variable_values = data.T 
@@ -715,81 +941,86 @@
                 lats_all = lats_all[:variable_values.shape[0]]
             
 
             variable_values_all.append(variable_values)
             combined_mtime.extend(mtime_values)
             lats_all.append(lats)
             
-            # Concatenate data along the time dimension
-        variable_values_all = np.concatenate(variable_values_all, axis=1)
-        if selected_unit != None:
-            variable_values_all ,variable_unit  = convert_units (variable_values_all, variable_unit, selected_unit)
-            
-        mtime_values = combined_mtime
+    # Concatenate data along the time dimension
+    variable_values_all = np.concatenate(variable_values_all, axis=1)
+    if selected_unit != None:
+        variable_values_all ,variable_unit  = convert_units (variable_values_all, variable_unit, selected_unit)
         
-        if plot_mode == True:    
-            return variable_values_all, lats, mtime_values, selected_lon, variable_unit, variable_long_name, filename
-        else:
-            return variable_values_all
+    mtime_values = combined_mtime
+    if plot_mode == True:    
+        return variable_values_all, lats, mtime_values, selected_lon, variable_unit, variable_long_name, filename
+    else:
+        return variable_values_all
 
 
 
-def calc_avg_ht(datasets, selected_time, selected_lev_ilev):
+def calc_avg_ht(datasets, time, selected_lev_ilev):
     """
     Compute the average Z value for a given set of lat, lon, and lev from a dataset.
     
     Parameters:
     - ds (xarray): The loaded dataset opened using xarray.
-    - selected_time (str): Timestamp to filter the data.
+    - time (str): Timestamp to filter the data.
     - selected_lev_ilev (float): The level for which to retrieve data.
     
     Returns:
     - float: The average ZG value for the given conditions.
     """
-    
+    if isinstance(time, str):
+        time = np.datetime64(time, 'ns')
     
     for ds, filenames in datasets:
-        if selected_time in ds['time'].values:
+        if time in ds['time'].values:
             if selected_lev_ilev in ds['ilev'].values:
-                heights = ds['ZG'].sel(time=selected_time, ilev=selected_lev_ilev).values
+                heights = ds['ZG'].sel(time=time, ilev=selected_lev_ilev).values
             else:
                 sorted_levs = sorted(ds['ilev'].values, key=lambda x: abs(x - selected_lev_ilev))
                 closest_lev1 = sorted_levs[0]
                 closest_lev2 = sorted_levs[1]
 
                 # Extract data for the two closest lev values using .sel()
-                data1 = ds['ZG'].sel(time=selected_time, ilev=closest_lev1).values
-                data2 = ds['ZG'].sel(time=selected_time, ilev=closest_lev2).values
+                data1 = ds['ZG'].sel(time=time, ilev=closest_lev1).values
+                data2 = ds['ZG'].sel(time=time, ilev=closest_lev2).values
                 
                 # Return the averaged data
                 heights = (data1 + data2) / 2
             avg_ht= round(heights.mean()/ 100000, 2)
-    return avg_ht
+            return avg_ht
+    return 0
 
 def min_max(variable_values):
-    """Find the minimum and maximum values of varval from the 2D array
+    """
+    Find the minimum and maximum values of varval from the 2D array
     
     Parameters:
     - variable_values (xarray): A list of variable values.
     
     Returns:
     - min_val (float): Minimum value of the variable in the array.
     - max_val (float): Maximum value of the variable in the array.
     """
     
     return np.nanmin(variable_values), np.nanmax(variable_values)
 
 def get_time(datasets, mtime):
     """
-    This function takes a dataset and mtime as parameters, searches for the time value 
-    in the dataset corresponding to mtime, and returns the np.datetime64 time value.
-    
-    :param dataset: xarray Dataset object
-    :param mtime: List of integers representing [day, hour, minute]
-    :return: np.datetime64 object representing the corresponding time value
+    Searches for a specific time in a dataset based on the provided model time (mtime) and returns the corresponding 
+    np.datetime64 time value. It iterates through multiple datasets to find a match.
+
+    Args:
+    - datasets (list of tuples): Each tuple contains an xarray dataset and its filename. The function will search each dataset for the time value.
+    - mtime (list of int): Model time represented as a list of integers in the format [day, hour, minute].
+
+    Returns:
+    - np.datetime64: The corresponding datetime value in the dataset for the given mtime. Returns None if no match is found.
     """
     for ds, filenames in datasets:
         # Convert mtime to numpy array for comparison
         mtime_array = np.array(mtime)
         
         # Find the index where mtime matches in the dataset
         idx = np.where(np.all(ds['mtime'].values == mtime_array, axis=1))[0]
@@ -798,74 +1029,36 @@
             continue  # Return None if no matching time is found
         
         # Get the corresponding datetime64 value from the time variable
         time = ds['time'].values[idx][0]
         
         return time
 
-def get_mtime(ds, selected_time):
-    """Find the mtime array for the corresponding selected time.
-    
+def get_mtime(ds, time):
+    """
+    Finds and returns the model time (mtime) array that corresponds to a specific time in a dataset. 
+    The mtime is an array representing [Day, Hour, Min].
+
     Parameters:
-    - ds (xarray): The loaded dataset opened using xarray.
-    - selected_time (str): Timestamp to filter the data.
-    
+    - ds (xarray): The dataset opened using xarray, containing time and mtime data.
+    - time (str/numpy.datetime64): The timestamp for which the corresponding mtime is to be found.
+
     Returns:
-    - array: mtime array containing [Day,Hour,Min].
+    - array: The mtime array containing [Day, Hour, Min] for the given timestamp. 
+             Returns None if no corresponding mtime is found.
     """
     # Convert input string to numpy datetime64 format
     
 
     # Extract time and mtime variables from the dataset
     time_variable = ds['time'].values
     mtime_variable = ds['mtime'].values
 
     # Find the index corresponding to the input time
-    index = np.where(time_variable == selected_time)
+    index = np.where(time_variable == time)
 
     # Extract and return the corresponding mtime value
     if index[0].size > 0:
         return mtime_variable[index[0][0]]
     else:
         return None
 
-
-def get_avg_ht_arr(ds, time, lat, lon):
-    """
-    Extracts ZG values for a given time, latitude, and longitude.
-    
-    Args:
-    - time (str): Desired time in the format 'YYYY-MM-DDTHH:MM:SS'
-    - lat (float): Desired latitude value
-    - lon (float): Desired longitude value
-    - dataset (xarray.Dataset): The dataset containing the ZG values. Default is the loaded dataset.
-    
-    Returns:
-    - list: A list of lists where each inner list contains [ilev_val, ZG_val]
-    """
-
-    #ds = xr.open_dataset(dataset)
-    # Extract the ZG values for the specified time, latitude, and longitude
-    selected_zg = ds['ZG'].sel(time=time, lat=lat, lon=lon)
-
-    # Convert the values from cm to km
-    selected_zg_km = selected_zg / 100000  # 1 km = 100000 cm
-    
-    # Extract the ilev values for the same selection
-    ilev_values = selected_zg['ilev'].values
-
-    # Combine the ilev and ZG values into a single list
-    combined_values = list(zip(ilev_values, selected_zg_km.values))
-
-    averaged_array = []
-    
-    # Iterate over the zg_array and calculate the average for consecutive values
-    for i in range(len(combined_values) - 1):
-        avg_lev = (combined_values[i][0] + combined_values[i+1][0]) / 2
-        avg_zg = (combined_values[i][1] + combined_values[i+1][1]) / 2
-        averaged_array.append((avg_lev, avg_zg))
-    averaged_array.append((7.25, float('nan')))
-    zg_values_array = [item[1] for item in averaged_array]
-
-    return zg_values_array
-
-    #return combined_values
```

### Comparing `tiegcmpy-1.2.7/src/tiegcmpy/getoptions.py` & `tiegcmpy-1.3.0/src/tiegcmpy/getoptions.py`

 * *Files identical despite different names*

### Comparing `tiegcmpy-1.2.7/src/tiegcmpy/io.py` & `tiegcmpy-1.3.0/src/tiegcmpy/io.py`

 * *Files identical despite different names*

### Comparing `tiegcmpy-1.2.7/src/tiegcmpy/main.py` & `tiegcmpy-1.3.0/src/tiegcmpy/main.py`

 * *Files identical despite different names*

### Comparing `tiegcmpy-1.2.7/src/tiegcmpy/plot_gen copy.py` & `tiegcmpy-1.3.0/src/tiegcmpy/plot_gen.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 import sys
 import numpy as np
 import matplotlib.pyplot as plt
-from .data_parse import lat_lon_lev, lat_lon_ilev,lat_lon, calc_avg_ht, min_max, lev_ilev_var, lev_ilev_lon, lev_ilev_lat,lev_ilev_time, lat_time_lev,lat_time_ilev, lat_time, get_time
+from .data_parse import arr_lat_lon,arr_lev_var,arr_lev_lon, arr_lev_lat,arr_lev_time,arr_lat_time, calc_avg_ht, min_max, get_time
 import cartopy.crs as ccrs
 import cartopy.feature as cfeature
+from cartopy.feature.nightshade import Nightshade
+from datetime import datetime, timezone
+import matplotlib.ticker as mticker
+import math
 
 def longitude_to_local_time(longitude):
     """
     Convert longitude to local time.
     
     Parameters:
         - longitude (float): Longitude value.
@@ -48,69 +52,76 @@
     Sets color scheme for plots.
     
     Parameters:
         - variable_name (str): The name of the variable with latitude, longitude, ilev dimensions.
     
     Returns:
         - cmap_color (str): Color scheme of the countour map.
-        - contour_color (str): Color scheme of conutour lines.
+        - line_color (str): Color scheme of conutour lines.
     """
     #
     # Setting type of variable 
     #
     density_type = ['NE', 'DEN', 'O2', 'O1', 'N2', 'NO', 'N4S', 'HE']
     temp_type = ['TN', 'TE', 'TI', 'QJOULE']
     wind_type = ['WN', 'UI_ExB', 'VI_ExB', 'WI_ExB', 'UN', 'VN']
     #
     # Color scheme for density type variables
     #
     if variable_name in density_type:
         cmap_color = 'viridis'
-        contour_color = 'white'
+        line_color = 'white'
     #
     # Color scheme for temprature type variables
     #
     elif variable_name in temp_type:
         cmap_color = 'inferno'
-        contour_color = 'white'
+        line_color = 'white'
     #
     # Color scheme for wind type variables
     #
     elif variable_name in wind_type:
         cmap_color = 'bwr'
-        contour_color = 'black'
+        line_color = 'black'
     #
     # Color scheme for all other types of variables
     #
     else:
         cmap_color = 'viridis'
-        contour_color = 'white'
-    return cmap_color, contour_color
+        line_color = 'white'
+    return cmap_color, line_color
 
-def plt_lat_lon(datasets, variable_name, time= None, mtime=None, level = None,  variable_unit = None, contour_intervals = None, contour_value = None, coastlines=False, latitude_minimum = None, latitude_maximum = None, longitude_minimum = None, longitude_maximum = None, localtime_minimum = None, localtime_maximum = None ):
+
+
+def plt_lat_lon(datasets, variable_name, time= None, mtime=None, level = None,  variable_unit = None, contour_intervals = None, contour_value = None,symmetric_interval= False, cmap_color = None, line_color = 'white', coastlines=False, nightshade=False, gm_equator=False, latitude_minimum = None, latitude_maximum = None, longitude_minimum = None, longitude_maximum = None, localtime_minimum = None, localtime_maximum = None ):
 
     """
     Generates a Latitude vs Longitude contour plot for a variable.
     
     Parameters:
         datasets (xarray): The loaded dataset/s using xarray.
-        variable_name (str): The name of the variable with latitude, longitude, ilev dimensions.
-        time (np.datetime64, optional): The selected time e.g., '2022-01-01T12:00:00'.
-        mtime (array, optional): The selected time as a list e.g., [1, 12, 0] for 1st day, 12 hours, 0 mins.
+        variable_name (str): The name of the variable with latitude, longitude, and lev/ilev dimensions.
+        time (np.datetime64, optional): The selected time, e.g., '2022-01-01T12:00:00'.
+        mtime (array, optional): The selected time as a list, e.g., [1, 12, 0] for 1st day, 12 hours, 0 mins.
         level (float, optional): The selected lev/ilev value.
         variable_unit (str, optional): The desired unit of the variable.
         contour_intervals (int, optional): The number of contour intervals. Defaults to 20.
         contour_value (int, optional): The value between each contour interval.
+        symmetric_interval (bool, optional): If True, the contour intervals will be symmetric around zero. Defaults to False.
+        cmap_color (str, optional): The color map of the contour. Defaults to 'viridis' for Density, 'inferno' for Temp, 'bwr' for Wind, 'viridis' for undefined.
+        line_color (str, optional): The color for all lines in the plot. Defaults to 'white'.
         coastlines (bool, optional): Shows coastlines on the plot. Defaults to False.
+        nightshade (bool, optional): Shows nightshade on the plot. Defaults to False.
+        gm_equator (bool, optional): Shows geomagnetic equator on the plot. Defaults to False.
         latitude_minimum (float, optional): Minimum latitude to slice plots. Defaults to -87.5.
         latitude_maximum (float, optional): Maximum latitude to slice plots. Defaults to 87.5.
         longitude_minimum (float, optional): Minimum longitude to slice plots. Defaults to -180.
         longitude_maximum (float, optional): Maximum longitude to slice plots. Defaults to 175.
-        localtime_minimum (float, optional): Minimum localtime to slice plots.
-        localtime_maximum (float, optional): Maximum localtime to slice plots.
+        localtime_minimum (float, optional): Minimum local time to slice plots. Defaults to None.
+        localtime_maximum (float, optional): Maximum local time to slice plots. Defaults to None.
     
     Returns:
         Contour plot.
     """
     # Printing Execution data
     if time == None:
         time = get_time(datasets, mtime)
@@ -118,152 +129,177 @@
         longitude_minimum = local_time_to_longitude(localtime_minimum)
     if localtime_maximum != None:
         longitude_maximum = local_time_to_longitude(localtime_maximum)
     if contour_intervals == None:
         contour_intervals = 20
     print("---------------["+variable_name+"]---["+str(time)+"]---["+str(level)+"]---------------")
     # Generate 2D arrays, extract variable_unit
-    
+    '''
     if level != None:
         try:
             data, level,  unique_lats, unique_lons, variable_unit, variable_long_name, selected_ut, selected_mtime, filename =lat_lon_lev(datasets, variable_name, time, level, variable_unit)
         except ValueError:
             data, level,  unique_lats, unique_lons, variable_unit, variable_long_name, selected_ut, selected_mtime, filename =lat_lon_ilev(datasets, variable_name, time, level, variable_unit)
         if level != 'mean':
             avg_ht=calc_avg_ht(datasets, time,level)
     else:
         data, unique_lats, unique_lons, variable_unit, variable_long_name, selected_ut, selected_mtime, filename =lat_lon(datasets, variable_name, time)
-    
+    '''
+    if isinstance(time, str):
+        time = np.datetime64(time, 'ns')
+
+    variable_values, level,  unique_lats, unique_lons, variable_unit, variable_long_name, selected_ut, selected_mtime, filename =arr_lat_lon(datasets, variable_name, time, selected_lev_ilev = level, selected_unit = variable_unit, plot_mode = True)
+    if level != 'mean' and level != None:
+            avg_ht=calc_avg_ht(datasets, time,level)
     if latitude_minimum == None:
         latitude_minimum = np.nanmin(unique_lats)
     if latitude_maximum == None:
         latitude_maximum = np.nanmax(unique_lats)
     if longitude_minimum == None:
         longitude_minimum = np.nanmin(unique_lons)
     if longitude_maximum == None:   
         longitude_maximum = np.nanmax(unique_lons)
 
-    min_val, max_val = min_max(data)
+    min_val, max_val = min_max(variable_values)
     selected_day=selected_mtime[0]
     selected_hour=selected_mtime[1]
     selected_min=selected_mtime[2]
 
-    cmap_color, contour_color = color_scheme(variable_name)
+    if cmap_color == None:
+        cmap_color, line_color = color_scheme(variable_name)
     # Extract values, latitudes, and longitudes from the array
     if contour_value is not None:
         contour_levels = np.arange(min_val, max_val + contour_value, contour_value)
-    else:
+        interval_value = contour_value
+    elif symmetric_interval == False:
         contour_levels = np.linspace(min_val, max_val, contour_intervals)
+        interval_value = (max_val - min_val) / (contour_intervals - 1)
+    elif symmetric_interval == True:
+        range_half = math.ceil(max(abs(min_val), abs(max_val))/10)*10
+        interval_value = range_half / (contour_intervals // 2)  # Divide by 2 to get intervals for one side
+        positive_levels = np.arange(interval_value, range_half + interval_value, interval_value)
+        negative_levels = -np.flip(positive_levels)  # Generate negative levels symmetrically
+        contour_levels = np.concatenate((negative_levels, [0], positive_levels))
+    if -180 in unique_lons:
+        lon_idx = np.where(unique_lons == -180)[0][-1]  # Get the index of the last occurrence of -180
+        unique_lons = np.append(unique_lons, 180)
+        variable_values = np.insert(variable_values, -1, variable_values[:, lon_idx], axis=1)
+
     # Generate contour plot
     
     interval_value = contour_value if contour_value else (max_val - min_val) / (contour_intervals - 1)
 
     # Generate contour plot
-    plot = plt.figure(figsize=(20, 12))
+    plot = plt.figure(figsize=(20, 9))
 
-
-    # Check if add_coastlines parameter is True
-    if coastlines:
-        # Create a GeoAxes instance with a specific projection
+    if coastlines == True or nightshade == True or gm_equator ==True:
+        subtitle_ht= 100
         ax = plt.axes(projection=ccrs.PlateCarree())
-        # Add coastlines to this GeoAxes instance
-        ax.add_feature(cfeature.COASTLINE, edgecolor='white', linewidth=3)
     else:
+        subtitle_ht= 115
         ax = plt.gca()
-
-    contour_filled = plt.contourf(unique_lons, unique_lats, data, cmap=cmap_color, levels=contour_levels)
-    contour_lines = plt.contour(unique_lons, unique_lats, data, colors=contour_color, linewidths=0.5, levels=contour_levels)
-    plt.clabel(contour_lines, inline=True, fontsize=16, colors=contour_color)
-    cbar = plt.colorbar(contour_filled, label=variable_name + " [" + variable_unit + "]")
+    # Check if add_coastlines parameter is True
+    if coastlines:
+        ax.add_feature(cfeature.COASTLINE, edgecolor=line_color, linewidth=3)
+    if nightshade:
+        ax.add_feature(Nightshade(datetime.fromtimestamp(time.astype('O')/1e9, tz=timezone.utc), alpha=0.4))
+    if gm_equator:
+        ax.plot(unique_lons, [0]*len(unique_lons), color=line_color, linestyle='--', transform=ccrs.Geodetic())
+    
+    
+    contour_filled = plt.contourf(unique_lons, unique_lats, variable_values, cmap=cmap_color, levels=contour_levels)
+    contour_lines = plt.contour(unique_lons, unique_lats, variable_values, colors=line_color, linewidths=0.5, levels=contour_levels)
+    plt.clabel(contour_lines, inline=True, fontsize=16, colors=line_color)
+    cbar = plt.colorbar(contour_filled, label=variable_name + " [" + variable_unit + "]",fraction=0.046, pad=0.04)
     cbar.set_label(variable_name + " [" + variable_unit + "]", size=28, labelpad=15)
     cbar.ax.tick_params(labelsize=18)
-    plt.title(variable_long_name + ' ' + variable_name + ' (' + variable_unit + ') ' + '\n\n', fontsize=36)
-    if level == 'mean':
-        plt.text(0, 110, 'UT=' + str(selected_ut) + '  ZP=' + str(level), ha='center', va='center', fontsize=28)
-    elif level != None:
-        plt.text(0, 110, 'UT=' + str(selected_ut) + '  ZP=' + str(level)+' AVG HT=' + str(avg_ht), ha='center', va='center', fontsize=28)
-    else:
-        plt.text(0, 110, 'UT=' + str(selected_ut), ha='center', va='center', fontsize=28)
-    plt.ylabel('Latitude', fontsize=28)
+    
+    
     plt.xlabel('Longitude (Deg)', fontsize=28)
     plt.xticks([value for value in unique_lons if value % 30 == 0],fontsize=18)
-    plt.yticks(fontsize=18)
+    plt.ylabel('Latitude (Deg)', fontsize=28)
+    plt.yticks(range(-90, 91, 30),fontsize=18)
     plt.xlim(longitude_minimum,longitude_maximum)
     plt.ylim(latitude_minimum,latitude_maximum)
 
     plt.tight_layout()
     
+    if coastlines == False and nightshade == False and gm_equator == False:
+        # Add Local Time secondary x-axis
+        ax2 = ax.twiny()
+        ax2.set_xlim(ax.get_xlim())
+        ax2_xticks = ax.get_xticks()
+        ax2.set_xticks(ax2_xticks)
+        ax2.set_xticklabels([str(int(longitude_to_local_time(longitude) % 24)) for longitude in ax2_xticks],fontsize=18)
+        ax2.set_xlabel('Local Time (Hrs)', labelpad=15, fontsize=28)
 
-    # Add Local Time secondary x-axis
-    #ax = plt.gca()
-    ax2 = ax.twiny()
-    ax2.set_xlim(ax.get_xlim())
-    ax2_xticks = ax.get_xticks()
-    ax2.set_xticks(ax2_xticks)
-    ax2.set_xticklabels([str(int(longitude_to_local_time(longitude) % 24)) for longitude in ax2_xticks],fontsize=18)
-    ax2.set_xlabel('Local Time (Hrs)', labelpad=15, fontsize=28)
+
+    # Add plot title
+    plt.title(variable_long_name + ' ' + variable_name + ' (' + variable_unit + ') ' + '\n\n', fontsize=36)
+    # Add plot subtitle
+    if level == 'mean':
+        plt.text(0, subtitle_ht, 'UT=' + str(selected_ut) + '  ZP=' + str(level), ha='center', va='center', fontsize=28)
+    elif level != None:
+        plt.text(0, subtitle_ht, 'UT=' + str(selected_ut) + '  ZP=' + str(level)+' AVG HT=' + str(avg_ht), ha='center', va='center', fontsize=28)
+    else:
+        plt.text(0, subtitle_ht, 'UT=' + str(selected_ut), ha='center', va='center', fontsize=28)
+    
 
     # Add subtext to the plot
     plt.text(-90, -115, "Min, Max = "+str("{:.2e}".format(min_val))+", "+str("{:.2e}".format(max_val)), ha='center', va='center',fontsize=28)
     plt.text(90, -115, "Contour Interval = "+str("{:.2e}".format(interval_value)), ha='center', va='center',fontsize=28)
-    plt.text(90, -125, "Day, Hour, Min = "+str(selected_day)+","+str(selected_hour)+","+str(selected_min), ha='center', va='center',fontsize=28)
-    plt.text(-90, -125, str(filename), ha='center', va='center',fontsize=28)
-
-    
-    #plot, ax = plt.subplots()
-    #plot, ax = plt.subplots()
-
-    
+    plt.text(0, -125, "Day, Hour, Min = "+str(selected_day)+","+str(selected_hour)+","+str(selected_min), ha='center', va='center',fontsize=28)
+    plt.text(0, -135, str(filename), ha='center', va='center',fontsize=28)
     
     return(plot)
 
 
 
 def plt_lev_var(datasets, variable_name, latitude, time= None, mtime=None, longitude = None, localtime = None, variable_unit = None, level_minimum = None, level_maximum = None):
     """
     Generates a Level vs Variable line plot for a given latitude.
     
     Parameters:
         datasets (xarray): The loaded dataset/s using xarray.
-        variable_name (str): The name of the variable with latitude, longitude, and ilev dimensions.
+        variable_name (str): The name of the variable with latitude, longitude, and lev/ilev dimensions.
         latitude (float): The specific latitude value for the plot.
         time (np.datetime64, optional): The selected time, e.g., '2022-01-01T12:00:00'.
         mtime (array, optional): The selected time as a list, e.g., [1, 12, 0] for 1st day, 12 hours, 0 mins.
         longitude (float, optional): The specific longitude value for the plot.
         localtime (float, optional): The specific local time value for the plot.
         variable_unit (str, optional): The desired unit of the variable.
-        level_minimum (float, optional): Minimum level value for the plot. Defaults to -8.
-        level_maximum (float, optional): Maximum level value for the plot. Defaults to 8.
+        level_minimum (float, optional): Minimum level value for the plot. Defaults to None.
+        level_maximum (float, optional): Maximum level value for the plot. Defaults to None.
     
     Returns:
         Line plot.
     """
     # Printing Execution data
     if time == None:
         time = get_time(datasets, mtime)
     if longitude == None:
         longitude = local_time_to_longitude(localtime)
     print("---------------["+variable_name+"]---["+str(time)+"]---["+str(latitude)+"]---["+str(longitude)+"]---------------")
+    if isinstance(time, str):
+        time = np.datetime64(time, 'ns')
 
-
-    variable_values , levs_ilevs, variable_unit, variable_long_name, selected_ut, selected_mtime, filename = lev_ilev_var(datasets, variable_name, time, latitude, longitude,  variable_unit)
+    variable_values , levs_ilevs, variable_unit, variable_long_name, selected_ut, selected_mtime, filename = arr_lev_var(datasets, variable_name, time, latitude, longitude,  variable_unit, plot_mode = True)
 
     if level_minimum == None:
         level_minimum = np.nanmin(levs_ilevs)
     if level_maximum == None:
         level_maximum = np.nanmax(levs_ilevs)
 
     min_val, max_val = min_max(variable_values)
     #print(min_val, max_val)
     selected_day=selected_mtime[0]
     selected_hour=selected_mtime[1]
     selected_min=selected_mtime[2]
 
 
-    #zg_values = get_avg_ht_arr(datasets, time, latitude, longitude)
     #print(len(zg_values))
 
     
     # Plotting
     
     plot = plt.figure(figsize=(22, 12))
     plt.plot(variable_values, levs_ilevs)
@@ -271,57 +307,53 @@
     plt.ylabel('LN(P0/P) (INTERFACES)', fontsize=28)
     plt.xticks(fontsize=18)  
     plt.yticks(fontsize=18) 
     plt.title(variable_long_name+' '+variable_name+' ('+variable_unit+') '+'\n\n',fontsize=36 )   
 
     plt.ylim(level_minimum, level_maximum)
 
-    '''
-    ax = plt.gca()
-    ax2 = ax.twinx()
-    ax2.plot(variable_values, zg_values, 'r--', alpha=0)  # Plot with alpha=0 to make it invisible
-    ax2.set_ylabel('Height (in km)', fontsize=28, labelpad=15, color='black')
-    ax2.tick_params(axis='y', labelcolor='black', labelsize=18)
-    
-    '''
+
 
     if longitude == 'mean' and latitude == 'mean':
-        plt.text(0.5, 1.08,'UT='+str(selected_ut) +"  LAT= Mean SLT= Mean", ha='center', va='center',fontsize=28, transform=plt.gca().transAxes) 
+        plt.text(0.5, 1.08,'UT='+str(selected_ut) +"  LAT= Mean LON= Mean", ha='center', va='center',fontsize=28, transform=plt.gca().transAxes) 
     elif longitude == 'mean':
-        plt.text(0.5, 1.08,'UT='+str(selected_ut) +'  LAT='+str(latitude)+" SLT= Mean", ha='center', va='center',fontsize=28, transform=plt.gca().transAxes) 
+        plt.text(0.5, 1.08,'UT='+str(selected_ut) +'  LAT='+str(latitude)+" LON= Mean", ha='center', va='center',fontsize=28, transform=plt.gca().transAxes) 
     elif latitude == 'mean':
-        plt.text(0.5, 1.08,'UT='+str(selected_ut) +'  LAT= Mean'+" SLT="+str(longitude_to_local_time(longitude))+"Hrs", ha='center', va='center',fontsize=28, transform=plt.gca().transAxes) 
+        plt.text(0.5, 1.08,'UT='+str(selected_ut) +'  LAT= Mean'+" LON="+str(longitude), ha='center', va='center',fontsize=28, transform=plt.gca().transAxes) 
     else:
-        plt.text(0.5, 1.08,'UT='+str(selected_ut) +'  LAT='+str(latitude)+" SLT="+str(longitude_to_local_time(longitude))+"Hrs", ha='center', va='center',fontsize=28, transform=plt.gca().transAxes) 
+        plt.text(0.5, 1.08,'UT='+str(selected_ut) +'  LAT='+str(latitude)+" LON="+str(longitude), ha='center', va='center',fontsize=28, transform=plt.gca().transAxes) 
     plt.text(0.5, -0.2, "Min, Max = "+str("{:.2e}".format(min_val))+", "+str("{:.2e}".format(max_val)), ha='center', va='center',fontsize=28, transform=plt.gca().transAxes) 
     plt.text(0.5, -0.25, "Day, Hour, Min = "+str(selected_day)+","+str(selected_hour)+","+str(selected_min), ha='center', va='center',fontsize=28, transform=plt.gca().transAxes)
     plt.text(0.5, -0.3, str(filename), ha='center', va='center',fontsize=28, transform=plt.gca().transAxes)
 
     return(plot)
 
 
-def plt_lev_lon(datasets, variable_name, latitude, time= None, mtime=None, variable_unit = None, contour_intervals = 20, contour_value = None,  level_minimum = None, level_maximum = None, longitude_minimum = None, longitude_maximum = None, localtime_minimum = None, localtime_maximum = None):
+def plt_lev_lon(datasets, variable_name, latitude, time= None, mtime=None, variable_unit = None, contour_intervals = 20, contour_value = None,symmetric_interval= False, cmap_color = None, line_color = 'white',  level_minimum = None, level_maximum = None, longitude_minimum = None, longitude_maximum = None, localtime_minimum = None, localtime_maximum = None):
     """
     Generates a Level vs Longitude contour plot for a given latitude.
     
     Parameters:
         datasets (xarray): The loaded dataset/s using xarray.
-        variable_name (str): The name of the variable with latitude, longitude, and ilev dimensions.
+        variable_name (str): The name of the variable with latitude, longitude, and lev/ilev dimensions.
         latitude (float): The specific latitude value for the plot.
         time (np.datetime64, optional): The selected time, e.g., '2022-01-01T12:00:00'.
         mtime (array, optional): The selected time as a list, e.g., [1, 12, 0] for 1st day, 12 hours, 0 mins.
         variable_unit (str, optional): The desired unit of the variable.
         contour_intervals (int, optional): The number of contour intervals. Defaults to 20.
         contour_value (int, optional): The value between each contour interval.
-        level_minimum (float, optional): Minimum level value for the plot. Defaults to -6.75.
-        level_maximum (float, optional): Maximum level value for the plot. Defaults to 6.75.
+        symmetric_interval (bool, optional): If True, the contour intervals will be symmetric around zero. Defaults to False.
+        cmap_color (str, optional): The color map of the contour. Defaults to 'viridis' for Density, 'inferno' for Temp, 'bwr' for Wind, 'viridis' for undefined.
+        line_color (str, optional): The color for all lines in the plot. Defaults to 'white'.
+        level_minimum (float, optional): Minimum level value for the plot. Defaults to None.
+        level_maximum (float, optional): Maximum level value for the plot. Defaults to None.
         longitude_minimum (float, optional): Minimum longitude value for the plot. Defaults to -180.
         longitude_maximum (float, optional): Maximum longitude value for the plot. Defaults to 175.
-        localtime_minimum (float, optional): Minimum localtime value for the plot.
-        localtime_maximum (float, optional): Maximum localtime value for the plot.
+        localtime_minimum (float, optional): Minimum local time value for the plot. Defaults to None.
+        localtime_maximum (float, optional): Maximum local time value for the plot. Defaults to None.
     
     Returns:
         Contour plot.
     """
     # Printing Execution data
     if time == None:
         time = get_time(datasets, mtime)
@@ -329,15 +361,15 @@
         longitude_minimum = local_time_to_longitude(localtime_minimum)
     if localtime_maximum != None:
         longitude_maximum = local_time_to_longitude(localtime_maximum)
     if contour_intervals == None:
         contour_intervals = 20    
     print("---------------["+variable_name+"]---["+str(time)+"]---["+str(latitude)+"]---------------")
     # Generate 2D arrays, extract variable_unit
-    variable_values, unique_lons, unique_levs,latitude, variable_unit, variable_long_name, selected_ut, selected_mtime, filename = lev_ilev_lon(datasets, variable_name, time, latitude, variable_unit)
+    variable_values, unique_lons, unique_levs,latitude, variable_unit, variable_long_name, selected_ut, selected_mtime, filename = arr_lev_lon(datasets, variable_name, time, latitude, variable_unit, plot_mode = True)
 
     if level_minimum == None:
         level_minimum = np.nanmin(unique_levs)
     if level_maximum == None:
         level_maximum = np.nanmax(unique_levs)
     if longitude_minimum == None:
         longitude_minimum = np.nanmin(unique_lons)
@@ -345,29 +377,39 @@
         longitude_maximum = np.nanmax(unique_lons)
 
     min_val, max_val = min_max(variable_values)
     selected_day=selected_mtime[0]
     selected_hour=selected_mtime[1]
     selected_min=selected_mtime[2]
 
-    cmap_color, contour_color = color_scheme(variable_name)
+    if cmap_color == None:
+        cmap_color, line_color = color_scheme(variable_name)
 
     if contour_value is not None:
         contour_levels = np.arange(min_val, max_val + contour_value, contour_value)
-    else:
+        interval_value = contour_value
+    elif symmetric_interval == False:
         contour_levels = np.linspace(min_val, max_val, contour_intervals)
-    # Generate contour plot
-    
-    interval_value = contour_value if contour_value else (max_val - min_val) / (contour_intervals - 1)
-
+        interval_value = (max_val - min_val) / (contour_intervals - 1)
+    elif symmetric_interval == True:
+        range_half = math.ceil(max(abs(min_val), abs(max_val))/10)*10
+        interval_value = range_half / (contour_intervals // 2)  # Divide by 2 to get intervals for one side
+        positive_levels = np.arange(interval_value, range_half + interval_value, interval_value)
+        negative_levels = -np.flip(positive_levels)  # Generate negative levels symmetrically
+        contour_levels = np.concatenate((negative_levels, [0], positive_levels))
+    if -180 in unique_lons:
+        lon_idx = np.where(unique_lons == -180)[0][-1]  # Get the index of the last occurrence of -180
+        unique_lons = np.append(unique_lons, 180)
+        variable_values = np.insert(variable_values, -1, variable_values[:, lon_idx], axis=1)
 
+    # Generate contour plot   
     plot=plt.figure(figsize=(24, 12))
     contour_filled = plt.contourf(unique_lons, unique_levs, variable_values, cmap= cmap_color, levels=contour_levels)
-    contour_lines = plt.contour(unique_lons, unique_levs, variable_values, colors=contour_color, linewidths=0.5, levels=contour_levels)
-    plt.clabel(contour_lines, inline=True, fontsize=16, colors=contour_color)
+    contour_lines = plt.contour(unique_lons, unique_levs, variable_values, colors=line_color, linewidths=0.5, levels=contour_levels)
+    plt.clabel(contour_lines, inline=True, fontsize=16, colors=line_color)
     cbar = plt.colorbar(contour_filled, label=variable_name+" ["+variable_unit+"]")
     cbar.set_label(variable_name+" ["+variable_unit+"]", size=28, labelpad=15)
     cbar.ax.tick_params(labelsize=18)
     plt.title(variable_long_name+' '+variable_name+' ('+variable_unit+') '+'\n\n',fontsize=36 )   
     if latitude == 'mean':
         plt.text(0.5, 1.18,'UT='+str(selected_ut) +' ZONAL MEANS', ha='center', va='center',fontsize=28, transform=plt.gca().transAxes) 
     else:
@@ -398,30 +440,33 @@
     #plot, ax = plt.subplots()
 
     
     
     return(plot)
 
 
-def plt_lev_lat(datasets, variable_name, time= None, mtime=None, longitude = None, localtime = None, variable_unit = None, contour_intervals = 20, contour_value = None, level_minimum = None, level_maximum = None, latitude_minimum = None,latitude_maximum = None):
+def plt_lev_lat(datasets, variable_name, time= None, mtime=None, longitude = None, localtime = None, variable_unit = None, contour_intervals = 20, contour_value = None,symmetric_interval= False, cmap_color = None, line_color = 'white', level_minimum = None, level_maximum = None, latitude_minimum = None,latitude_maximum = None):
     """
     Generates a Level vs Latitude contour plot for a specified time and/or longitude.
     
     Parameters:
         datasets (xarray): The loaded dataset/s using xarray.
-        variable_name (str): The name of the variable with latitude, longitude, and ilev dimensions.
+        variable_name (str): The name of the variable with latitude, longitude, and lev/ilev dimensions.
         time (np.datetime64, optional): The selected time, e.g., '2022-01-01T12:00:00'.
         mtime (array, optional): The selected time as a list, e.g., [1, 12, 0] for 1st day, 12 hours, 0 mins.
         longitude (float, optional): The specific longitude value for the plot.
         localtime (float, optional): The specific local time value for the plot.
         variable_unit (str, optional): The desired unit of the variable.
         contour_intervals (int, optional): The number of contour intervals. Defaults to 20.
         contour_value (int, optional): The value between each contour interval.
-        level_minimum (float, optional): Minimum level value for the plot. Defaults to -6.75.
-        level_maximum (float, optional): Maximum level value for the plot. Defaults to 6.75.
+        symmetric_interval (bool, optional): If True, the contour intervals will be symmetric around zero. Defaults to False.
+        cmap_color (str, optional): The color map of the contour. Defaults to 'viridis' for Density, 'inferno' for Temp, 'bwr' for Wind, 'viridis' for undefined.
+        line_color (str, optional): The color for all lines in the plot. Defaults to 'white'.
+        level_minimum (float, optional): Minimum level value for the plot. Defaults to None.
+        level_maximum (float, optional): Maximum level value for the plot. Defaults to None.
         latitude_minimum (float, optional): Minimum latitude value for the plot. Defaults to -87.5.
         latitude_maximum (float, optional): Maximum latitude value for the plot. Defaults to 87.5.
     
     Returns:
         Contour plot.
     """
     # Printing Execution data
@@ -429,15 +474,17 @@
         time = get_time(datasets, mtime)
     if longitude == None:
         longitude = local_time_to_longitude(localtime)
     if contour_intervals == None:
         contour_intervals = 20
     print("---------------["+variable_name+"]---["+str(time)+"]---["+str(longitude)+"]---------------")
     # Generate 2D arrays, extract variable_unit
-    variable_values, unique_lats, unique_levs,longitude, variable_unit, variable_long_name, selected_ut, selected_mtime, filename = lev_ilev_lat(datasets, variable_name, time, longitude,  variable_unit)
+    if isinstance(time, str):
+        time = np.datetime64(time, 'ns')
+    variable_values, unique_lats, unique_levs,longitude, variable_unit, variable_long_name, selected_ut, selected_mtime, filename = arr_lev_lat(datasets, variable_name, time, longitude,  variable_unit, plot_mode = True)
 
     if level_minimum == None:
         level_minimum = np.nanmin(unique_levs)
     if level_maximum == None:
         level_maximum = np.nanmax(unique_levs)
     if latitude_minimum == None:
         latitude_minimum = np.nanmin(unique_lats)
@@ -445,29 +492,39 @@
         latitude_maximum = np.nanmax(unique_lats)
 
     min_val, max_val = min_max(variable_values)
     selected_day=selected_mtime[0]
     selected_hour=selected_mtime[1]
     selected_min=selected_mtime[2]
 
-    cmap_color, contour_color = color_scheme(variable_name)
+    if cmap_color == None:
+        cmap_color, line_color = color_scheme(variable_name)
 
     if contour_value is not None:
         contour_levels = np.arange(min_val, max_val + contour_value, contour_value)
-    else:
+        interval_value = contour_value
+    elif symmetric_interval == False:
         contour_levels = np.linspace(min_val, max_val, contour_intervals)
+        interval_value = (max_val - min_val) / (contour_intervals - 1)
+    elif symmetric_interval == True:
+        range_half = math.ceil(max(abs(min_val), abs(max_val))/10)*10
+        interval_value = range_half / (contour_intervals // 2)  # Divide by 2 to get intervals for one side
+        positive_levels = np.arange(interval_value, range_half + interval_value, interval_value)
+        negative_levels = -np.flip(positive_levels)  # Generate negative levels symmetrically
+        contour_levels = np.concatenate((negative_levels, [0], positive_levels))
+
     
     
     interval_value = contour_value if contour_value else (max_val - min_val) / (contour_intervals - 1)
     
     # Generate contour plot
     plot=plt.figure(figsize=(24, 12))
     contour_filled = plt.contourf(unique_lats, unique_levs, variable_values, cmap= cmap_color, levels=contour_levels)
-    contour_lines = plt.contour(unique_lats, unique_levs, variable_values, colors=contour_color, linewidths=0.5, levels=contour_levels)
-    plt.clabel(contour_lines, inline=True, fontsize=16, colors=contour_color)
+    contour_lines = plt.contour(unique_lats, unique_levs, variable_values, colors=line_color, linewidths=0.5, levels=contour_levels)
+    plt.clabel(contour_lines, inline=True, fontsize=16, colors=line_color)
     cbar = plt.colorbar(contour_filled, label=variable_name+" ["+variable_unit+"]")
     cbar.set_label(variable_name+" ["+variable_unit+"]", size=28, labelpad=15)
     cbar.ax.tick_params(labelsize=18)
     plt.title(variable_long_name+' '+variable_name+' ('+variable_unit+') '+'\n\n',fontsize=36 )   
     if longitude == 'mean':
           plt.text(0.5, 1.08,'UT='+str(selected_ut) +' ZONAL MEANS', ha='center', va='center',fontsize=28, transform=plt.gca().transAxes) 
     else:
@@ -478,83 +535,124 @@
     plt.yticks(fontsize=18) 
     plt.xlim(latitude_minimum,latitude_maximum)
     plt.ylim(level_minimum,level_maximum)
     
     # Add subtext to the plot
     plt.text(0.25, -0.2, "Min, Max = "+str("{:.2e}".format(min_val))+", "+str("{:.2e}".format(max_val)), ha='center', va='center',fontsize=28, transform=plt.gca().transAxes)
     plt.text(0.75, -0.2, "Contour Interval = "+str("{:.2e}".format(interval_value)), ha='center', va='center',fontsize=28, transform=plt.gca().transAxes)
-    plt.text(0.75, -0.25, "Day, Hour, Min = "+str(selected_day)+","+str(selected_hour)+","+str(selected_min), ha='center', va='center',fontsize=28, transform=plt.gca().transAxes)
-    plt.text(0.25, -0.25, str(filename), ha='center', va='center',fontsize=28, transform=plt.gca().transAxes)
+    plt.text(0.50, -0.25, "Day, Hour, Min = "+str(selected_day)+","+str(selected_hour)+","+str(selected_min), ha='center', va='center',fontsize=28, transform=plt.gca().transAxes)
+    plt.text(0.50, -0.3, str(filename), ha='center', va='center',fontsize=28, transform=plt.gca().transAxes)
 
     
     #plot, ax = plt.subplots()
 
     
     
     return(plot)
 
 
 
 
-def plt_lev_time(datasets, variable_name, latitude, longitude = None, localtime = None, variable_unit = None, contour_intervals = 20, contour_value = None,  level_minimum = None, level_maximum = None):
+def plt_lev_time(datasets, variable_name, latitude, longitude = None, localtime = None, variable_unit = None, contour_intervals = 10, contour_value = None,symmetric_interval= False, cmap_color = None, line_color = 'white',  level_minimum = None, level_maximum = None, mtime_minimum=None, mtime_maximum=None):
     """
     Generates a Level vs Time contour plot for a specified latitude and/or longitude.
     
     Parameters:
         datasets (xarray): The loaded dataset/s using xarray.
         variable_name (str): The name of the variable with latitude, longitude, time, and ilev dimensions.
         latitude (float): The specific latitude value for the plot.
         longitude (float, optional): The specific longitude value for the plot.
         localtime (float, optional): The specific local time value for the plot.
         variable_unit (str, optional): The desired unit of the variable.
-        contour_intervals (int, optional): The number of contour intervals. Defaults to 20.
+        contour_intervals (int, optional): The number of contour intervals. Defaults to 10.
         contour_value (int, optional): The value between each contour interval.
-        level_minimum (float, optional): Minimum level value for the plot. Defaults to -6.75.
-        level_maximum (float, optional): Maximum level value for the plot. Defaults to 6.75.
+        symmetric_interval (bool, optional): If True, the contour intervals will be symmetric around zero. Defaults to False.
+        cmap_color (str, optional): The color map of the contour. Defaults to 'viridis' for Density, 'inferno' for Temp, 'bwr' for Wind, 'viridis' for undefined.
+        line_color (str, optional): The color for all lines in the plot. Defaults to 'white'.
+        level_minimum (float, optional): Minimum level value for the plot. Defaults to None.
+        level_maximum (float, optional): Maximum level value for the plot. Defaults to None.
+        mtime_minimum (float, optional): Minimum time value for the plot. Defaults to None.
+        mtime_maximum (float, optional): Maximum time value for the plot. Defaults to None.
     
     Returns:
         Contour plot.
     """
     if longitude is None:
         longitude = local_time_to_longitude(localtime)
     if contour_intervals == None:
         contour_intervals = 20
     #print(datasets)
-    variable_values_all, levs_ilevs, mtime_values, longitude, variable_unit, variable_long_name = lev_ilev_time(datasets, variable_name, latitude, longitude, variable_unit)
+    variable_values_all, levs_ilevs, mtime_values, longitude, variable_unit, variable_long_name = arr_lev_time(datasets, variable_name, latitude, longitude, variable_unit, plot_mode = True)
     
     if level_minimum == None:
         level_minimum = np.nanmin(levs_ilevs)
     if level_maximum == None:
         level_maximum = np.nanmax(levs_ilevs)
 
     print("---------------["+variable_name+"]---["+str(latitude)+"]---["+str(longitude)+"]---------------")
     
+
+
+    num_deleted_before = 0
+    num_deleted_after = 0
+
+    if mtime_minimum is not None and mtime_maximum is not None:
+        new_mtime_values = []
+        for t_mtime in mtime_values:
+            mtime_total_minutes = t_mtime[0] * 24 * 60 *60 + t_mtime[1] * 60 *60+ t_mtime[2] *60+ t_mtime[3]
+            mtime_min_total = mtime_minimum[0] * 24 * 60*60 + mtime_minimum[1] * 60 *60+ mtime_minimum[2]*60 + mtime_minimum[3]
+            mtime_max_total = mtime_maximum[0] * 24 * 60*60 + mtime_maximum[1] * 60 *60+ mtime_maximum[2]*60 + mtime_minimum[3]
+            if mtime_total_minutes >= mtime_min_total and mtime_total_minutes <= mtime_max_total:                
+                new_mtime_values.append(t_mtime)  
+            else:
+                if mtime_total_minutes < mtime_min_total:
+                    num_deleted_before += 1
+                elif mtime_total_minutes > mtime_max_total:
+                    num_deleted_after += 1
+        mtime_values = new_mtime_values
+        mtime_values_sorted = sorted(mtime_values, key=lambda x: (x[0], x[1], x[2], x[3]))
+        variable_values_all = variable_values_all[:, num_deleted_before:-num_deleted_after]
+
     min_val, max_val = np.nanmin(variable_values_all), np.nanmax(variable_values_all)
-    cmap_color, contour_color = color_scheme(variable_name)
+
+    if cmap_color == None:
+        cmap_color, line_color = color_scheme(variable_name)
 
     if contour_value is not None:
         contour_levels = np.arange(min_val, max_val + contour_value, contour_value)
-    else:
+        interval_value = contour_value
+    elif symmetric_interval == False:
         contour_levels = np.linspace(min_val, max_val, contour_intervals)
+        interval_value = (max_val - min_val) / (contour_intervals - 1)
+    elif symmetric_interval == True:
+        range_half = math.ceil(max(abs(min_val), abs(max_val))/10)*10
+        interval_value = range_half / (contour_intervals // 2)  # Divide by 2 to get intervals for one side
+        positive_levels = np.arange(interval_value, range_half + interval_value, interval_value)
+        negative_levels = -np.flip(positive_levels)  # Generate negative levels symmetrically
+        contour_levels = np.concatenate((negative_levels, [0], positive_levels))
+
     
     
     interval_value = contour_value if contour_value else (max_val - min_val) / (contour_intervals - 1)
     mtime_tuples = [tuple(entry) for entry in mtime_values]
     try:    # Modify this part to show both day and hour
         unique_times = sorted(list(set([(day, hour) for day, hour, _, _ in mtime_values])))
         time_indices = [i for i, (day, hour, _, _) in enumerate(mtime_tuples) if i == 0 or mtime_tuples[i-1][:2] != (day, hour)]
+        if len(time_indices) >24:
+            unique_times = sorted(list(set([day for day, _, _, _ in mtime_values])))
+            time_indices = [i for i, (day, _, _, _) in enumerate(mtime_values) if i == 0 or mtime_values[i-1][0] != day]
     except:
         unique_times = sorted(list(set([day for day, _, _ in mtime_values])))
         time_indices = [i for i, (day, _, _) in enumerate(mtime_values) if i == 0 or mtime_values[i-1][0] != day]
 
     plot=plt.figure(figsize=(20, 12))
     X, Y = np.meshgrid(range(len(mtime_values)), levs_ilevs)
     contour_filled = plt.contourf(X, Y, variable_values_all, cmap=cmap_color, levels=contour_levels)
-    contour_lines = plt.contour(X, Y, variable_values_all, colors=contour_color, linewidths=0.5, levels=contour_levels)
-    plt.clabel(contour_lines, inline=True, fontsize=16, colors=contour_color)
+    contour_lines = plt.contour(X, Y, variable_values_all, colors=line_color, linewidths=0.5, levels=contour_levels)
+    plt.clabel(contour_lines, inline=True, fontsize=16, colors=line_color)
     cbar = plt.colorbar(contour_filled, label=variable_name+" ["+variable_unit+"]")
     cbar.set_label(variable_name+" ["+variable_unit+"]", size=28, labelpad=15)
     cbar.ax.tick_params(labelsize=18)
     try:
         plt.xticks(time_indices, ["{}-{:02d}h".format(day, hour) for day, hour in unique_times], rotation=45)
         plt.xlabel("Model Time (Day-Hour) from "+str(unique_times[0])+" to "+str(unique_times[-1]), fontsize=28) 
     except:
@@ -568,29 +666,29 @@
     plt.xticks(fontsize=18)  
     plt.yticks(fontsize=18) 
     plt.ylim(level_minimum,level_maximum)
 
 
     # Add subtext to the plot
     if longitude == 'mean' and latitude == 'mean':
-        plt.text(0.5, 1.08,'  LAT= Mean SLT= Mean', ha='center', va='center',fontsize=28, transform=plt.gca().transAxes) 
+        plt.text(0.5, 1.08,'  LAT= Mean LON= Mean', ha='center', va='center',fontsize=28, transform=plt.gca().transAxes) 
     elif longitude == 'mean':
-        plt.text(0.5, 1.08,'  LAT='+str(latitude)+" SLT= Mean", ha='center', va='center',fontsize=28, transform=plt.gca().transAxes) 
+        plt.text(0.5, 1.08,'  LAT='+str(latitude)+" LON= Mean", ha='center', va='center',fontsize=28, transform=plt.gca().transAxes) 
     elif latitude == 'mean':
-        plt.text(0.5, 1.08,'  LAT= Mean'+" SLT="+str(longitude_to_local_time(longitude))+"Hrs", ha='center', va='center',fontsize=28, transform=plt.gca().transAxes) 
+        plt.text(0.5, 1.08,'  LAT= Mean'+" LON="+str(longitude), ha='center', va='center',fontsize=28, transform=plt.gca().transAxes) 
     else:
-        plt.text(0.5, 1.08,'  LAT='+str(latitude)+" SLT="+str(longitude_to_local_time(longitude))+"Hrs", ha='center', va='center',fontsize=28, transform=plt.gca().transAxes) 
+        plt.text(0.5, 1.08,'  LAT='+str(latitude)+" LON="+str(longitude), ha='center', va='center',fontsize=28, transform=plt.gca().transAxes) 
     plt.text(0.5, -0.2, "Min, Max = "+str("{:.2e}".format(min_val))+", "+str("{:.2e}".format(max_val)), ha='center', va='center',fontsize=28, transform=plt.gca().transAxes)
     plt.text(0.5, -0.25, "Contour Interval = "+str("{:.2e}".format(interval_value)), ha='center', va='center',fontsize=28, transform=plt.gca().transAxes)
-
+    plt.close(plot)
     return(plot)
 
 
 
-def plt_lat_time(datasets, variable_name, level = None, longitude = None, localtime = None,  variable_unit = None, contour_intervals = 10, contour_value = None, latitude_minimum = None,latitude_maximum = None):
+def plt_lat_time(datasets, variable_name, level = None, longitude = None, localtime = None,  variable_unit = None, contour_intervals = 10, contour_value = None,symmetric_interval= False, cmap_color = None, line_color = 'white', latitude_minimum = None,latitude_maximum = None, mtime_minimum=None, mtime_maximum=None):
     """
     Generates a Latitude vs Time contour plot for a specified level and/or longitude.
     
     Parameters:
         datasets (xarray): The loaded dataset/s using xarray.
         variable_name (str): The name of the variable with latitude, longitude, time, and ilev dimensions.
         level (float): The specific level value for the plot.
@@ -606,59 +704,85 @@
         Contour plot.
     """
     if longitude is None:
         longitude = local_time_to_longitude(localtime)
     if contour_intervals == None:
         contour_intervals = 20
     print("---------------["+variable_name+"]---["+str(level)+"]---["+str(longitude)+"]---------------")
-
+    '''
     if level != None: 
         try:
             variable_values_all, unique_lats, mtime_values, longitude, variable_unit, variable_long_name, filename = lat_time_lev(datasets, variable_name, level, longitude, variable_unit)
         except:
             variable_values_all, unique_lats, mtime_values, longitude, variable_unit, variable_long_name, filename = lat_time_ilev(datasets, variable_name, level, longitude, variable_unit)
     else:
         variable_values_all, unique_lats, mtime_values, longitude, variable_unit, variable_long_name, filename = lat_time(datasets, variable_name, longitude, variable_unit)
+    '''
+    variable_values_all, unique_lats, mtime_values, longitude, variable_unit, variable_long_name, filename = arr_lat_time(datasets, variable_name, longitude, level, variable_unit, plot_mode = True)
     # Assuming the levels are consistent across datasets, but using the minimum size for safety
-    
     if latitude_minimum == None:
         latitude_minimum = np.nanmin(unique_lats)
     if latitude_maximum == None:
         latitude_maximum = np.nanmax(unique_lats)
+    num_deleted_before = 0
+    num_deleted_after = 0
 
-    
-    
+    if mtime_minimum is not None and mtime_maximum is not None:
+        new_mtime_values = []
+        for t_mtime in mtime_values:
+            mtime_total_minutes = t_mtime[0] * 24 * 60 *60 + t_mtime[1] * 60 *60+ t_mtime[2] *60+ t_mtime[3]
+            mtime_min_total = mtime_minimum[0] * 24 * 60*60 + mtime_minimum[1] * 60 *60+ mtime_minimum[2]*60 + mtime_minimum[3]
+            mtime_max_total = mtime_maximum[0] * 24 * 60*60 + mtime_maximum[1] * 60 *60+ mtime_maximum[2]*60 + mtime_minimum[3]
+            if mtime_total_minutes >= mtime_min_total and mtime_total_minutes <= mtime_max_total:
+                new_mtime_values.append(t_mtime)   
+            else:
+                if mtime_total_minutes < mtime_min_total:
+                    num_deleted_before += 1
+                elif mtime_total_minutes > mtime_max_total:
+                    num_deleted_after += 1
+        mtime_values = new_mtime_values
+        mtime_values_sorted = sorted(mtime_values, key=lambda x: (x[0], x[1], x[2], x[3]))
+        variable_values_all = variable_values_all[:, num_deleted_before:-num_deleted_after]
     min_val, max_val = np.nanmin(variable_values_all), np.nanmax(variable_values_all)
     
-    cmap_color, contour_color = color_scheme(variable_name)
+    if cmap_color == None:
+        cmap_color, line_color = color_scheme(variable_name)
 
     if contour_value is not None:
         contour_levels = np.arange(min_val, max_val + contour_value, contour_value)
-    else:
+        interval_value = contour_value
+    elif symmetric_interval == False:
         contour_levels = np.linspace(min_val, max_val, contour_intervals)
-    
+        interval_value = (max_val - min_val) / (contour_intervals - 1)
+    elif symmetric_interval == True:
+        range_half = math.ceil(max(abs(min_val), abs(max_val))/10)*10
+        interval_value = range_half / (contour_intervals // 2)  # Divide by 2 to get intervals for one side
+        positive_levels = np.arange(interval_value, range_half + interval_value, interval_value)
+        negative_levels = -np.flip(positive_levels)  # Generate negative levels symmetrically
+        contour_levels = np.concatenate((negative_levels, [0], positive_levels))
+
     
     interval_value = contour_value if contour_value else (max_val - min_val) / (contour_intervals - 1)
 
     mtime_tuples = [tuple(entry) for entry in mtime_values]
     try:    # Modify this part to show both day and hour
         unique_times = sorted(list(set([(day, hour) for day, hour, _, _ in mtime_values])))
         time_indices = [i for i, (day, hour, _, _) in enumerate(mtime_tuples) if i == 0 or mtime_tuples[i-1][:2] != (day, hour)]
-        if len(time_indices) >=10:
+        if len(time_indices) >24:
             unique_times = sorted(list(set([day for day, _, _, _ in mtime_values])))
             time_indices = [i for i, (day, _, _, _) in enumerate(mtime_values) if i == 0 or mtime_values[i-1][0] != day]
     except:
         unique_times = sorted(list(set([day for day, _, _ in mtime_values])))
         time_indices = [i for i, (day, _, _) in enumerate(mtime_values) if i == 0 or mtime_values[i-1][0] != day]
 
     plot = plt.figure(figsize=(20, 12))
     X, Y = np.meshgrid(range(len(mtime_values)), unique_lats)
     contour_filled = plt.contourf(X, Y, variable_values_all, cmap=cmap_color, levels=contour_levels)
-    contour_lines = plt.contour(X, Y, variable_values_all, colors=contour_color, linewidths=0.5, levels=contour_levels)
-    plt.clabel(contour_lines, inline=True, fontsize=16, colors=contour_color)
+    contour_lines = plt.contour(X, Y, variable_values_all, colors=line_color, linewidths=0.5, levels=contour_levels)
+    plt.clabel(contour_lines, inline=True, fontsize=16, colors=line_color)
     cbar = plt.colorbar(contour_filled, label=variable_name + " [" + variable_unit + "]")
     cbar.set_label(variable_name + " [" + variable_unit + "]", size=28, labelpad=15)
     cbar.ax.tick_params(labelsize=18)
     try:
         plt.xticks(time_indices, ["{}-{:02d}h".format(day, hour) for day, hour in unique_times], rotation=45)
         plt.xlabel("Model Time (Day-Hour) from "+str(unique_times[0])+" to "+str(unique_times[-1]), fontsize=28) 
     except:
@@ -672,18 +796,18 @@
     plt.tight_layout()
     plt.xticks(fontsize=18)
     plt.yticks(fontsize=18)
     plt.ylim(latitude_minimum, latitude_maximum)
 
     # Add subtext to the plot
     if level == 'mean' and longitude == 'mean':
-        plt.text(0.5, 1.08, '  ZP= Mean SLT= Mean', ha='center', va='center', fontsize=28, transform=plt.gca().transAxes)
+        plt.text(0.5, 1.08, '  ZP= Mean LON= Mean', ha='center', va='center', fontsize=28, transform=plt.gca().transAxes)
     elif longitude == 'mean':
-        plt.text(0.5, 1.08, '  ZP=' + str(level) + " SLT= Mean", ha='center', va='center', fontsize=28, transform=plt.gca().transAxes)
+        plt.text(0.5, 1.08, '  ZP=' + str(level) + " LON= Mean", ha='center', va='center', fontsize=28, transform=plt.gca().transAxes)
     elif level == 'mean':
-        plt.text(0.5, 1.08, '  ZP= Mean' + " SLT=" + str(longitude_to_local_time(longitude)) + "Hrs", ha='center', va='center', fontsize=28, transform=plt.gca().transAxes)
+        plt.text(0.5, 1.08, '  ZP= Mean' + " LON=" + str(longitude), ha='center', va='center', fontsize=28, transform=plt.gca().transAxes)
     else:
-        plt.text(0.5, 1.08, '  ZP=' + str(level) + " SLT=" + str(longitude_to_local_time(longitude)) + "Hrs", ha='center', va='center', fontsize=28, transform=plt.gca().transAxes)
+        plt.text(0.5, 1.08, '  ZP=' + str(level) + " LON=" + str(longitude), ha='center', va='center', fontsize=28, transform=plt.gca().transAxes)
     plt.text(0.5, -0.2, "Min, Max = " + str("{:.2e}".format(min_val)) + ", " + str("{:.2e}".format(max_val)), ha='center', va='center', fontsize=28, transform=plt.gca().transAxes)
     plt.text(0.5, -0.25, "Contour Interval = " + str("{:.2e}".format(interval_value)), ha='center', va='center', fontsize=28, transform=plt.gca().transAxes)
     plt.close(plot)
     return plot
```

