# Comparing `tmp/pylake-0.1.6.tar.gz` & `tmp/pylake-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylake-0.1.6.tar", last modified: Tue Apr 23 13:13:07 2024, max compression
+gzip compressed data, was "pylake-0.1.7.tar", last modified: Mon Jun  3 13:52:10 2024, max compression
```

## Comparing `pylake-0.1.6.tar` & `pylake-0.1.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 13:13:07.693514 pylake-0.1.6/
--rw-rw-rw-   0        0        0     1410 2024-04-23 13:13:07.691520 pylake-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     1079 2024-04-23 13:00:55.000000 pylake-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-23 13:13:07.674907 pylake-0.1.6/pylake/
--rw-rw-rw-   0        0        0       56 2024-04-23 13:00:55.000000 pylake-0.1.6/pylake/__init__.py
--rw-rw-rw-   0        0        0     6237 2024-04-23 13:00:55.000000 pylake-0.1.6/pylake/functions.py
--rw-rw-rw-   0        0        0     1555 2024-04-23 13:00:55.000000 pylake-0.1.6/pylake/functions_meta.py
--rw-rw-rw-   0        0        0    30692 2024-04-23 13:00:55.000000 pylake-0.1.6/pylake/pylake.py
--rw-rw-rw-   0        0        0    25005 2024-04-23 13:00:55.000000 pylake-0.1.6/pylake/pylake_metabolizer.py
-drwxrwxrwx   0        0        0        0 2024-04-23 13:13:07.686539 pylake-0.1.6/pylake.egg-info/
--rw-rw-rw-   0        0        0     1410 2024-04-23 13:13:07.000000 pylake-0.1.6/pylake.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2024-04-23 13:13:07.000000 pylake-0.1.6/pylake.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 13:13:07.000000 pylake-0.1.6/pylake.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      100 2024-04-23 13:13:07.000000 pylake-0.1.6/pylake.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-23 13:13:07.000000 pylake-0.1.6/pylake.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-23 13:13:07.693514 pylake-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      813 2024-04-23 13:12:55.000000 pylake-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-23 13:13:07.689528 pylake-0.1.6/test/
--rw-rw-rw-   0        0        0     1425 2024-04-23 13:00:55.000000 pylake-0.1.6/test/test.py
+drwxrwxr-x   0 runnalja  (1000) runnalja  (1000)        0 2024-06-03 13:52:10.148461 pylake-0.1.7/
+-rw-rw-r--   0 runnalja  (1000) runnalja  (1000)     1354 2024-06-03 13:52:10.148461 pylake-0.1.7/PKG-INFO
+-rw-rw-r--   0 runnalja  (1000) runnalja  (1000)     1035 2024-06-03 13:50:00.000000 pylake-0.1.7/README.md
+drwxrwxr-x   0 runnalja  (1000) runnalja  (1000)        0 2024-06-03 13:52:10.148461 pylake-0.1.7/pylake/
+-rw-rw-r--   0 runnalja  (1000) runnalja  (1000)       55 2024-06-03 13:50:00.000000 pylake-0.1.7/pylake/__init__.py
+-rw-rw-r--   0 runnalja  (1000) runnalja  (1000)     6050 2024-06-03 13:50:00.000000 pylake-0.1.7/pylake/functions.py
+-rw-rw-r--   0 runnalja  (1000) runnalja  (1000)     1503 2024-06-03 13:50:00.000000 pylake-0.1.7/pylake/functions_meta.py
+-rw-rw-r--   0 runnalja  (1000) runnalja  (1000)    30400 2024-06-03 13:50:00.000000 pylake-0.1.7/pylake/pylake.py
+-rw-rw-r--   0 runnalja  (1000) runnalja  (1000)    24353 2024-06-03 13:50:00.000000 pylake-0.1.7/pylake/pylake_metabolizer.py
+drwxrwxr-x   0 runnalja  (1000) runnalja  (1000)        0 2024-06-03 13:52:10.148461 pylake-0.1.7/pylake.egg-info/
+-rw-rw-r--   0 runnalja  (1000) runnalja  (1000)     1354 2024-06-03 13:52:10.000000 pylake-0.1.7/pylake.egg-info/PKG-INFO
+-rw-rw-r--   0 runnalja  (1000) runnalja  (1000)      290 2024-06-03 13:52:10.000000 pylake-0.1.7/pylake.egg-info/SOURCES.txt
+-rw-rw-r--   0 runnalja  (1000) runnalja  (1000)        1 2024-06-03 13:52:10.000000 pylake-0.1.7/pylake.egg-info/dependency_links.txt
+-rw-rw-r--   0 runnalja  (1000) runnalja  (1000)      100 2024-06-03 13:52:10.000000 pylake-0.1.7/pylake.egg-info/requires.txt
+-rw-rw-r--   0 runnalja  (1000) runnalja  (1000)        7 2024-06-03 13:52:10.000000 pylake-0.1.7/pylake.egg-info/top_level.txt
+-rw-rw-r--   0 runnalja  (1000) runnalja  (1000)       38 2024-06-03 13:52:10.148461 pylake-0.1.7/setup.cfg
+-rw-rw-r--   0 runnalja  (1000) runnalja  (1000)      784 2024-06-03 13:50:00.000000 pylake-0.1.7/setup.py
+drwxrwxr-x   0 runnalja  (1000) runnalja  (1000)        0 2024-06-03 13:52:10.148461 pylake-0.1.7/test/
+-rw-rw-r--   0 runnalja  (1000) runnalja  (1000)     1398 2024-06-03 13:50:00.000000 pylake-0.1.7/test/test.py
```

### Comparing `pylake-0.1.6/PKG-INFO` & `pylake-0.1.7/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-Metadata-Version: 2.1
-Name: pylake
-Version: 0.1.6
-Summary: pylake
-Home-page: https://github.com/eawag-surface-waters-research/PyLake
-Author: Hugo Cruz
-Author-email: <huggcruzz@gmail.com>
-License: MIT
-Keywords: python,pylake,Lake analyzer,environmental data,Physical properties
-Description-Content-Type: text/markdown
-
-# PyLake
-
-This work present methods used to compute meaningful physical properties in aquatic sciences.
-
-The methods are based on Xarray. 
-Multi-dimensional large time-series array are compatible if an xarray is passed as input.
-
-Algorithms and documentation are sometimes inspired by LakeAnalyzer in R (https://github.com/GLEON/rLakeAnalyzer)
-
-Implemented methods:
-* Thermocline
-* Mixed layer
-* Metalimnion extent (epilimnion and hypolimnion depth)
-* Wedderburn Number
-* Schmidt stability
-* Heat content
-* Seiche periode
-* Lake Number
-* Brunt-Vaisala frequency
-* Average layer temperature
-* Monin-Obhukov 
-
-## Installation
-
-Pylake use Dask which require a python version >=3.8
-
-`pip install pylake`
-
-## Usage
-
-
-Have a look in the notebooks, an example is provided
-
-```python
-import pylake
-import numpy as np
-
-Temp = np.array([14.3,14,12.1,10,9.7,9.5,6,5])
-depth = np.array([1,2,3,4,5,6,7,8])
-epilimnion, hypolimnion = pylake.metalimnion(temp, depth)
-```
-
- ## Work in progress
- Warning messages
- Lake metabolizer is being implemented. 
+Metadata-Version: 2.1
+Name: pylake
+Version: 0.1.7
+Summary: pylake
+Home-page: https://github.com/eawag-surface-waters-research/pylake
+Author: Hugo Cruz
+Author-email: <huggcruzz@gmail.com>
+License: MIT
+Keywords: python,pylake,Lake analyzer,environmental data,Physical properties
+Description-Content-Type: text/markdown
+
+# PyLake
+
+This work present methods used to compute meaningful physical properties in aquatic sciences.
+
+The methods are based on Xarray. 
+Multi-dimensional large time-series array are compatible if an xarray is passed as input.
+
+Algorithms and documentation are sometimes inspired by LakeAnalyzer in R (https://github.com/GLEON/rLakeAnalyzer)
+
+Implemented methods:
+* Thermocline
+* Mixed layer
+* Metalimnion extent (epilimnion and hypolimnion depth)
+* Wedderburn Number
+* Schmidt stability
+* Heat content
+* Seiche periode
+* Lake Number
+* Brunt-Vaisala frequency
+* Average layer temperature
+* Monin-Obhukov 
+
+## Installation
+
+Pylake use Dask which require a python version >=3.8
+
+`pip install pylake`
+
+## Usage
+
+
+Have a look in the notebooks, an example is provided
+
+```python
+import pylake
+import numpy as np
+
+Temp = np.array([14.3,14,12.1,10,9.7,9.5,6,5])
+depth = np.array([1,2,3,4,5,6,7,8])
+epilimnion, hypolimnion = pylake.metalimnion(temp, depth)
+```
+
+ ## Work in progress
+ Warning messages
+ Lake metabolizer is being implemented.
```

### Comparing `pylake-0.1.6/README.md` & `pylake-0.1.7/README.md`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-# PyLake
-
-This work present methods used to compute meaningful physical properties in aquatic sciences.
-
-The methods are based on Xarray. 
-Multi-dimensional large time-series array are compatible if an xarray is passed as input.
-
-Algorithms and documentation are sometimes inspired by LakeAnalyzer in R (https://github.com/GLEON/rLakeAnalyzer)
-
-Implemented methods:
-* Thermocline
-* Mixed layer
-* Metalimnion extent (epilimnion and hypolimnion depth)
-* Wedderburn Number
-* Schmidt stability
-* Heat content
-* Seiche periode
-* Lake Number
-* Brunt-Vaisala frequency
-* Average layer temperature
-* Monin-Obhukov 
-
-## Installation
-
-Pylake use Dask which require a python version >=3.8
-
-`pip install pylake`
-
-## Usage
-
-
-Have a look in the notebooks, an example is provided
-
-```python
-import pylake
-import numpy as np
-
-Temp = np.array([14.3,14,12.1,10,9.7,9.5,6,5])
-depth = np.array([1,2,3,4,5,6,7,8])
-epilimnion, hypolimnion = pylake.metalimnion(temp, depth)
-```
-
- ## Work in progress
- Warning messages
+# PyLake
+
+This work present methods used to compute meaningful physical properties in aquatic sciences.
+
+The methods are based on Xarray. 
+Multi-dimensional large time-series array are compatible if an xarray is passed as input.
+
+Algorithms and documentation are sometimes inspired by LakeAnalyzer in R (https://github.com/GLEON/rLakeAnalyzer)
+
+Implemented methods:
+* Thermocline
+* Mixed layer
+* Metalimnion extent (epilimnion and hypolimnion depth)
+* Wedderburn Number
+* Schmidt stability
+* Heat content
+* Seiche periode
+* Lake Number
+* Brunt-Vaisala frequency
+* Average layer temperature
+* Monin-Obhukov 
+
+## Installation
+
+Pylake use Dask which require a python version >=3.8
+
+`pip install pylake`
+
+## Usage
+
+
+Have a look in the notebooks, an example is provided
+
+```python
+import pylake
+import numpy as np
+
+Temp = np.array([14.3,14,12.1,10,9.7,9.5,6,5])
+depth = np.array([1,2,3,4,5,6,7,8])
+epilimnion, hypolimnion = pylake.metalimnion(temp, depth)
+```
+
+ ## Work in progress
+ Warning messages
  Lake metabolizer is being implemented.
```

### Comparing `pylake-0.1.6/pylake/functions.py` & `pylake-0.1.7/pylake/functions.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,187 +1,187 @@
-import numpy as np
-import xarray as xr
-import warnings 
-
-def control(Temp, depths):
-    #Too chronophage and not so usefull
-    #if np.isnan(Temp).all:
-    #    warnings.warn("Could not deduce thermocline with only nan vector")
-    #    return np.nan
-    if Temp.shape[1]<3:
-        warnings.warn("Could not deduce thermocline with less than 3 measurements")
-        return np.nan
-    elif len(depths)!=len(np.unique(depths)):
-        warnings.warn("depths must be unique")
-        return np.nan
-    else:
-        return 1
-
-def to_xarray(Temp, depths, time=None):
-    if (type(Temp)==np.ndarray)or(type(Temp)==list):
-        Temp = format_Temp(depths, Temp)
-        if time is not None:
-            coords = {'time':time,'depth':depths}
-        else:
-            coords = {'time':list(range(0,Temp.shape[0])),'depth':depths}
-
-        Temp = xr.DataArray(Temp, coords)
-    else:
-        depths = Temp["depth"].to_numpy()
-        Temp.load()
-    return Temp,depths
-    
-def smooth_1D(Temp, smooth):
-    from scipy.signal import savgol_filter
-    if type(smooth)==dict:
-        window_size = smooth.get("window_size",len(Temp)/10)
-        mode = smooth.get("method",'nearest')
-        order = smooth.get("order",3)
-    else:
-        window_size= round_up_to_odd(len(Temp)/10)
-        mode = 'nearest'
-        order = 3
-    new_Temp = savgol_filter(Temp, window_size, order, mode=mode)
-    return new_Temp
-
-def smooth_temp(Temp, depths, smooth):
-    from scipy.signal import savgol_filter
-    if type(smooth)==dict:
-        window_size = smooth.get("window_size",round_up_to_odd(len(depths)/10))
-        mode = smooth.get("method",'nearest')
-        order = smooth.get("order",3)
-    else:
-        window_size= round_up_to_odd(len(depths)/10)
-        mode = 'nearest'
-        order = 3
-    new_Temp = savgol_filter(Temp, window_size, order, mode=mode)
-    return new_Temp
-
-
-def weighted_method(depths, rho, z_idx):
-    '''
-    Estimate where the thermocline lies even between two temperature 
-    measurement depths, giving a potentially finer-scale estimate 
-    than usual techniques.
-
-    Parameters
-    -----------
-    depths: array_like
-        depth array
-    drho_dz: array_like 
-        density array 
-    z_idx: array_like
-        thermocline index corresponding to the depths 
-
-    Returns
-    -----------
-    weighted_thermoD: array_like
-        the adjusted weighted thermocline depth.
-    '''
-    if type(rho)==np.ndarray:
-        depths, rho, z_idx = list(map(np.asanyarray, (depths, rho, z_idx)))
-        rho = format_Temp(depths, rho)
-        coords = {'time':list(range(0,rho.shape[0])),'depth':depths}
-        rho = xr.DataArray(rho, coords)
-    else:
-        depths = rho.depth
-        rho.load()
-
-    drho_dz = rho.diff('depth')/rho.depth.diff('depth')
-
-    #Mask boundarie values
-    mask_up = z_idx==0
-    mask_down = (z_idx>=len(depths)-2)
-
-    #Change values for boundaries to avoid any bug on the indexation
-    z_masked = z_idx.copy()
-    z_masked = z_masked.where(~mask_up, z_masked+1)
-    z_masked = z_masked.where(~mask_down, z_masked-1)
-
-    #Weighted method 
-    hplus = (depths.isel(depth=z_masked) - depths.isel(depth=z_masked+2))/2
-    hminu = (depths.isel(depth=z_masked-1) - depths.isel(depth=z_masked+1))/2
-
-    drho = drho_dz.isel(depth=z_masked)
-    drho_plus = drho_dz.isel(depth=z_masked+1)
-    drho_minu = drho_dz.isel(depth=z_masked-1)
-
-    Dplus = hplus/(drho-drho_plus)
-    Dminu = hminu/(drho-drho_minu)
-
-    weighted_thermoD = depths[z_masked+1]*(Dplus/(Dminu+Dplus)) + depths[z_masked]*(Dminu/(Dminu+Dplus))
-    
-    mask_inf = (np.isinf(Dplus/(Dminu+Dplus))) & (np.isinf(Dminu/(Dminu+Dplus)))
-
-    #Restablish correct values for boundaries
-    weighted_thermoD = weighted_thermoD.where(~mask_up, (depths[0]+depths[1])/2 )
-    weighted_thermoD =  weighted_thermoD.where(~mask_down, (depths[-1]+depths[-2])/2)
-    weighted_thermoD = weighted_thermoD.where(~mask_inf, np.nan)
-    try:
-        weighted_thermoD = weighted_thermoD.drop_vars('depth')
-    except:
-        pass
-    return weighted_thermoD
-
-def check_bathy(Temp, bthA, bthD, depth):
-    #Check this with xarray
-    numD = Temp.shape[1]-1
-    if max(bthD) > depth[numD]:
-        Temp  = np.append(Temp,Temp[:,numD])
-        depth = np.append(depth,max(bthD))
-    elif max(bthD)<depth[numD]:
-        bthD = np.append(bthD,depth[numD])
-        bthA = np.append(bthA, 0)
-    if min(bthD)<depth[0]:
-        Temp = np.hstack((Temp[:,0].reshape(-1,1),Temp))
-        depth = np.append(np.min(bthD), depth)
-    return Temp,bthA,bthD,depth
-
-def T68conv(T90):
-    return T90 * 1.00024
-
-def dens0(t,s=0.2):
-    b = (8.24493e-1, -4.0899e-3, 7.6438e-5, -8.2467e-7, 5.3875e-9)
-    c = (-5.72466e-3, 1.0227e-4, -1.6546e-6)
-    d = 4.8314e-4
-    T68 = T68conv(t)
-    out =  (smow(t) + (b[0] + (b[1] + (b[2] + (b[3] + b[4] * T68) * T68) *
-            T68) * T68) * s + (c[0] + (c[1] + c[2] * T68) * T68) * s *
-            s ** 0.5 + d * s ** 2)
-    return out
-
-def smow(t):
-    a = (999.842594, 6.793952e-2, -9.095290e-3, 1.001685e-4, -1.120083e-6, 6.536332e-9)
-    T68 = T68conv(t)
-    out= (a[0] + (a[1] + (a[2] + (a[3] + (a[4] + a[5] * T68) * T68) * T68) * T68) * T68)
-    return out    
-
-def format_Temp(depths, Temp):
-    if Temp.ndim==2:
-        if Temp.shape[0]==depths.shape[0]:
-            Temp = Temp.T
-    elif Temp.ndim==1:
-        Temp = Temp.reshape(-1,1).T
-    return Temp
-    
-def find_nearest_index(old_depths,SthermoD):
-    depth_index = np.argmin(np.abs(SthermoD-old_depths.reshape(-1,1)), axis=0)
-    return depth_index
-
-def find_nearest(old_depths,SthermoD):
-    depth_index = find_nearest_index(old_depths,SthermoD)
-    nearest_depth = old_depths[depth_index]
-    nearest_depth = set_nan(SthermoD,nearest_depth)
-    return nearest_depth
-
-def set_nan(vec1, vec2):
-    #If vec1 has NaN, set to NaN the values of vec2
-    NaN = np.isnan(vec1)
-    if any(NaN):
-        if len(NaN)==1:
-            vec2=np.array([np.nan])
-        else:
-            vec2[NaN] = np.nan
-    return vec2
-
-def round_up_to_odd(f):
-    return int(np.ceil(f) // 2 * 2 + 1)
+import numpy as np
+import xarray as xr
+import warnings 
+
+def control(Temp, depths):
+    #Too chronophage and not so usefull
+    #if np.isnan(Temp).all:
+    #    warnings.warn("Could not deduce thermocline with only nan vector")
+    #    return np.nan
+    if Temp.shape[1]<3:
+        warnings.warn("Could not deduce thermocline with less than 3 measurements")
+        return np.nan
+    elif len(depths)!=len(np.unique(depths)):
+        warnings.warn("depths must be unique")
+        return np.nan
+    else:
+        return 1
+
+def to_xarray(Temp, depths, time=None):
+    if (type(Temp)==np.ndarray)or(type(Temp)==list):
+        Temp = format_Temp(depths, Temp)
+        if time is not None:
+            coords = {'time':time,'depth':depths}
+        else:
+            coords = {'time':list(range(0,Temp.shape[0])),'depth':depths}
+
+        Temp = xr.DataArray(Temp, coords)
+    else:
+        depths = Temp["depth"].to_numpy()
+        Temp.load()
+    return Temp,depths
+    
+def smooth_1D(Temp, smooth):
+    from scipy.signal import savgol_filter
+    if type(smooth)==dict:
+        window_size = smooth.get("window_size",len(Temp)/10)
+        mode = smooth.get("method",'nearest')
+        order = smooth.get("order",3)
+    else:
+        window_size= round_up_to_odd(len(Temp)/10)
+        mode = 'nearest'
+        order = 3
+    new_Temp = savgol_filter(Temp, window_size, order, mode=mode)
+    return new_Temp
+
+def smooth_temp(Temp, depths, smooth):
+    from scipy.signal import savgol_filter
+    if type(smooth)==dict:
+        window_size = smooth.get("window_size",round_up_to_odd(len(depths)/10))
+        mode = smooth.get("method",'nearest')
+        order = smooth.get("order",3)
+    else:
+        window_size= round_up_to_odd(len(depths)/10)
+        mode = 'nearest'
+        order = 3
+    new_Temp = savgol_filter(Temp, window_size, order, mode=mode)
+    return new_Temp
+
+
+def weighted_method(depths, rho, z_idx):
+    '''
+    Estimate where the thermocline lies even between two temperature 
+    measurement depths, giving a potentially finer-scale estimate 
+    than usual techniques.
+
+    Parameters
+    -----------
+    depths: array_like
+        depth array
+    drho_dz: array_like 
+        density array 
+    z_idx: array_like
+        thermocline index corresponding to the depths 
+
+    Returns
+    -----------
+    weighted_thermoD: array_like
+        the adjusted weighted thermocline depth.
+    '''
+    if type(rho)==np.ndarray:
+        depths, rho, z_idx = list(map(np.asanyarray, (depths, rho, z_idx)))
+        rho = format_Temp(depths, rho)
+        coords = {'time':list(range(0,rho.shape[0])),'depth':depths}
+        rho = xr.DataArray(rho, coords)
+    else:
+        depths = rho.depth
+        rho.load()
+
+    drho_dz = rho.diff('depth')/rho.depth.diff('depth')
+
+    #Mask boundarie values
+    mask_up = z_idx==0
+    mask_down = (z_idx>=len(depths)-2)
+
+    #Change values for boundaries to avoid any bug on the indexation
+    z_masked = z_idx.copy()
+    z_masked = z_masked.where(~mask_up, z_masked+1)
+    z_masked = z_masked.where(~mask_down, z_masked-1)
+
+    #Weighted method 
+    hplus = (depths.isel(depth=z_masked) - depths.isel(depth=z_masked+2))/2
+    hminu = (depths.isel(depth=z_masked-1) - depths.isel(depth=z_masked+1))/2
+
+    drho = drho_dz.isel(depth=z_masked)
+    drho_plus = drho_dz.isel(depth=z_masked+1)
+    drho_minu = drho_dz.isel(depth=z_masked-1)
+
+    Dplus = hplus/(drho-drho_plus)
+    Dminu = hminu/(drho-drho_minu)
+
+    weighted_thermoD = depths[z_masked+1]*(Dplus/(Dminu+Dplus)) + depths[z_masked]*(Dminu/(Dminu+Dplus))
+    
+    mask_inf = (np.isinf(Dplus/(Dminu+Dplus))) & (np.isinf(Dminu/(Dminu+Dplus)))
+
+    #Restablish correct values for boundaries
+    weighted_thermoD = weighted_thermoD.where(~mask_up, (depths[0]+depths[1])/2 )
+    weighted_thermoD =  weighted_thermoD.where(~mask_down, (depths[-1]+depths[-2])/2)
+    weighted_thermoD = weighted_thermoD.where(~mask_inf, np.nan)
+    try:
+        weighted_thermoD = weighted_thermoD.drop_vars('depth')
+    except:
+        pass
+    return weighted_thermoD
+
+def check_bathy(Temp, bthA, bthD, depth):
+    #Check this with xarray
+    numD = Temp.shape[1]-1
+    if max(bthD) > depth[numD]:
+        Temp  = np.append(Temp,Temp[:,numD])
+        depth = np.append(depth,max(bthD))
+    elif max(bthD)<depth[numD]:
+        bthD = np.append(bthD,depth[numD])
+        bthA = np.append(bthA, 0)
+    if min(bthD)<depth[0]:
+        Temp = np.hstack((Temp[:,0].reshape(-1,1),Temp))
+        depth = np.append(np.min(bthD), depth)
+    return Temp,bthA,bthD,depth
+
+def T68conv(T90):
+    return T90 * 1.00024
+
+def dens0(t,s=0.2):
+    b = (8.24493e-1, -4.0899e-3, 7.6438e-5, -8.2467e-7, 5.3875e-9)
+    c = (-5.72466e-3, 1.0227e-4, -1.6546e-6)
+    d = 4.8314e-4
+    T68 = T68conv(t)
+    out =  (smow(t) + (b[0] + (b[1] + (b[2] + (b[3] + b[4] * T68) * T68) *
+            T68) * T68) * s + (c[0] + (c[1] + c[2] * T68) * T68) * s *
+            s ** 0.5 + d * s ** 2)
+    return out
+
+def smow(t):
+    a = (999.842594, 6.793952e-2, -9.095290e-3, 1.001685e-4, -1.120083e-6, 6.536332e-9)
+    T68 = T68conv(t)
+    out= (a[0] + (a[1] + (a[2] + (a[3] + (a[4] + a[5] * T68) * T68) * T68) * T68) * T68)
+    return out    
+
+def format_Temp(depths, Temp):
+    if Temp.ndim==2:
+        if Temp.shape[0]==depths.shape[0]:
+            Temp = Temp.T
+    elif Temp.ndim==1:
+        Temp = Temp.reshape(-1,1).T
+    return Temp
+    
+def find_nearest_index(old_depths,SthermoD):
+    depth_index = np.argmin(np.abs(SthermoD-old_depths.reshape(-1,1)), axis=0)
+    return depth_index
+
+def find_nearest(old_depths,SthermoD):
+    depth_index = find_nearest_index(old_depths,SthermoD)
+    nearest_depth = old_depths[depth_index]
+    nearest_depth = set_nan(SthermoD,nearest_depth)
+    return nearest_depth
+
+def set_nan(vec1, vec2):
+    #If vec1 has NaN, set to NaN the values of vec2
+    NaN = np.isnan(vec1)
+    if any(NaN):
+        if len(NaN)==1:
+            vec2=np.array([np.nan])
+        else:
+            vec2[NaN] = np.nan
+    return vec2
+
+def round_up_to_odd(f):
+    return int(np.ceil(f) // 2 * 2 + 1)
```

### Comparing `pylake-0.1.6/pylake/functions_meta.py` & `pylake-0.1.7/pylake/functions_meta.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-import numpy as np
-from .functions import *
-def xarray_from_input(func, locals, coords):
-    ds = xr.Dataset(coords=coords)
-    for var in func.__code__.co_varnames:
-        try:
-            ds[var]=('time', locals[var])
-        except:
-            try:
-                ds[var]=locals[var]
-            except:pass
-    return ds
-
-
-def getSchmidt(temperature, gas):
-    range_t = [4,35]
-    gases = {"He":[368,-16.75,0.374,-0.0036],
-	            "O2":[1568,-86.04,2.142,-0.0216],
-	            "CO2":[1742,-91.24,2.208,-0.0219],
-	            "CH4":[1824,-98.12,2.413,-0.0241],
-	            "SF6":[3255,-217.13,6.837,-0.0861],
-	            "N2O":[2105,-130.08,3.486,-0.0365],
-	            "Ar":[1799,-106.96,2.797,-0.0289],
-	            "N2":[1615,-92.15,2.349,-0.0240]}
-    A = gases[gas][0]
-    B = gases[gas][1]
-    C = gases[gas][2]
-    D = gases[gas][3]
-
-    Sc = A+B*temperature+C*temperature**2+D*temperature**3
-    return Sc
-
-def thermalExpFromTemp(Ts):
-    
-    V = 1       
-    dT = 0.001 
-    T1 = dens0(t=Ts, s=0.2)
-    T2 = dens0(t=Ts+dT, s=0.2)
-    V2 = T1/T2
-    dv_dT = (V2-V)/dT
-    alpha = dv_dT
-    return alpha
-
-def getKinematicVis(Ts):
-    # from Mays 2005, Water Resources Engineering
-    tempTable = np.arange(0,101,5)
-    # table in m2/s E-6
-    visTable = np.array([1.792,1.519,1.308,1.141,1.007,0.897,
-        0.804,0.727,0.661,0.605,0.556,0.513,0.477,0.444,
-        0.415,0.39,0.367,0.347,0.328,0.311,0.296])
-    v = np.interp(Ts, visTable, tempTable)
-    v = v*1e-6
+import numpy as np
+from .functions import *
+def xarray_from_input(func, locals, coords):
+    ds = xr.Dataset(coords=coords)
+    for var in func.__code__.co_varnames:
+        try:
+            ds[var]=('time', locals[var])
+        except:
+            try:
+                ds[var]=locals[var]
+            except:pass
+    return ds
+
+
+def getSchmidt(temperature, gas):
+    range_t = [4,35]
+    gases = {"He":[368,-16.75,0.374,-0.0036],
+	            "O2":[1568,-86.04,2.142,-0.0216],
+	            "CO2":[1742,-91.24,2.208,-0.0219],
+	            "CH4":[1824,-98.12,2.413,-0.0241],
+	            "SF6":[3255,-217.13,6.837,-0.0861],
+	            "N2O":[2105,-130.08,3.486,-0.0365],
+	            "Ar":[1799,-106.96,2.797,-0.0289],
+	            "N2":[1615,-92.15,2.349,-0.0240]}
+    A = gases[gas][0]
+    B = gases[gas][1]
+    C = gases[gas][2]
+    D = gases[gas][3]
+
+    Sc = A+B*temperature+C*temperature**2+D*temperature**3
+    return Sc
+
+def thermalExpFromTemp(Ts):
+    
+    V = 1       
+    dT = 0.001 
+    T1 = dens0(t=Ts, s=0.2)
+    T2 = dens0(t=Ts+dT, s=0.2)
+    V2 = T1/T2
+    dv_dT = (V2-V)/dT
+    alpha = dv_dT
+    return alpha
+
+def getKinematicVis(Ts):
+    # from Mays 2005, Water Resources Engineering
+    tempTable = np.arange(0,101,5)
+    # table in m2/s E-6
+    visTable = np.array([1.792,1.519,1.308,1.141,1.007,0.897,
+        0.804,0.727,0.661,0.605,0.556,0.513,0.477,0.444,
+        0.415,0.39,0.367,0.347,0.328,0.311,0.296])
+    v = np.interp(Ts, visTable, tempTable)
+    v = v*1e-6
     return(v)
```

### Comparing `pylake-0.1.6/pylake/pylake.py` & `pylake-0.1.7/pylake/pylake.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,789 +1,802 @@
-import numpy as np
-from .functions import *
-import seawater as sw
-from scipy.interpolate import interp1d
-import warnings
-from scipy.signal import find_peaks,savgol_filter
-import xarray as xr
-    
-def thermocline(Temp, depth=None, time=None, s=0.2, mixed_cutoff=1, smooth=False):
-    '''
-    Calculate the thermocline depth from one or various temperature profiles.
-    It uses the method of the maximum gradient, the results can be interpreted
-    as a diurnal thermocline (see pylake.seasonal_thermocline for the seasonal).
-
-    Method
-    ----------
-    The thermocline is calculated using the maximum gradient of density.
-    If the temperature profile have a variability in depth resolution, it is recommended 
-    to smooth the profile to avoid resolution influence on the algorithm.
-    Once the maximum gradient of density is found, a special technique to refine the 
-    thermocline depth is used and presented in (Read et al., 2011).
-
-    Parameters
-    ----------
-    Temp :  array_like
-        a numeric vector of water temperature in degrees C
-    depth : array_like
-        a numeric vector corresponding to the depth (in m) of the Temp
-    s : array_like, default : 0.2
-        Salinity of the water column in PSU
-    Smin : float, default: 0.1 °C/m
-        Optional parameter defining minimum density gradient for
-        thermocline.
-    mixed_cutoff : scalar, default: 1
-        The difference between the maximum and minimum of the
-        temperature profile should be higher than this cutoff.
-    smooth : bool, default: False
-        Smooth the curve following the scipy savgol filter (window size: 1/10 of the 
-        depth length, order:3, method=nearest)
-        Smoothing is recommended when the thermocline is located at a lower resolution 
-        sensors (sensors are more spaced at the thermocline)
-
-    Returns 
-    ----------
-    thermoD: array_like, scalar
-        thermocline depth (m)
-    thermoInd: array_like, scalar
-        thermocline index corresponding to the thermocline depth
-    
-    Examples
-    ----------
-    >>>     import pylake
-    ...     temp = temp = np.array([14.3,14,12.1,10,9.7,9.5,6,5])
-    ...     depth = depth = np.array([1,2,3,4,5,6,7,8])
-    ...     thermo, thermoInd = pylake.thermocline(temp,depth)
-    ...     print(f"thermocline depth: {thermo}\n")
-    ...     print(f"thermocline depth index: {thermoInd}\n")
-    ...     thermocline depth: 2.878790569183019
-    ...     thermocline depth index: 2
-    '''
-
-    Temp, depth = to_xarray(Temp, depth,time)
-
-    is_not_significant = Temp.max('depth')-Temp.min('depth')<mixed_cutoff
-    if smooth:
-        time = Temp.time
-        Temp = smooth_temp(Temp, depth, smooth)
-        Temp, depth = to_xarray(Temp, depth,time)
-
-    rhoVar = dens0(s=s,t=Temp)
-    drho_dz = rhoVar.diff('depth')/rhoVar.depth.diff('depth')
-    inf_mask = np.isinf(drho_dz)
-    drho_dz = drho_dz.where(~inf_mask, np.nan)
-    thermoInd = drho_dz.fillna(-999).argmax('depth')
-
-    thermoD = weighted_method(depth, rhoVar, thermoInd)
-
-    thermoInd = abs(thermoD-Temp.depth).fillna(999).argmin('depth')
-
-    thermoD = thermoD.where(~is_not_significant, np.nan)
-
-    if thermoD.size==1:
-        thermoD = thermoD.values.item()
-        thermoInd = thermoInd.data.item()
-    return thermoD, thermoInd
-
-
-
-def seasonal_thermocline(Temp, depth=None, time=None, s=0.2, mixed_cutoff=1, Smin=0.1, seasonal_smoothed=True, smooth=False):
-    '''
-    Calculate depth of the thermocline from a temperature profile.
-    
-    Method
-    ---------
-    The seasonal thermocline uses the find_peaks from scipy to find the first 
-    local maximum (higher than a certain threshold, based on Smin) starting 
-    from the bottom of the profile.
-    By default, if no peak is found, the seasonal thermocline is set equal to 
-    the diurnal thermocline. 
-    The same refining technique is used.
-    A savgol filter (special moving averaged filter) is used to smooth the data 
-    and discard extremums.
-    The seasonal is set to be more or equal to the diurnal thermocline.
-    Keep in mind that if the seasonal thermocline is often assimilated 
-    with the diurnal, with the exception that the seasonal is artificially smoothed.
-
-    Parameters
-    ----------
-    Temp :  array_like
-        a numeric vector of water temperature in degrees C
-    depth : array_like
-        a numeric vector corresponding to the depth of the temperature.
-        Depth is defined as positive, and is minimum at the surface. 
-    s : array_like, default : 0.2
-        Salinity of the water column in PSU
-    mixed_cutoff : scalar, default: 1
-        The difference between the maximum and minimum of the
-        temperature profile should be higher than this cutoff.
-    Smin : float, default: 0.1 °C/m
-        Optional parameter defining minimum density gradient for
-        thermocline. Threshold for the peak height of the scipy.signal.find_peaks(...).
-    seasonal_smoothed: bool, default: True
-        Smooth the seasonal thermocline on the entire time serie. The smooth depends on the time serie length.
-    smooth : bool, default: False
-        Smooth the curve following the scipy savgol filter (window size: 1/10 of the 
-        depth length, order:3, method=nearest)
-        Smoothing is recommended when the thermocline is located at a lower resolution 
-        sensors (sensors can be more spaced at the thermocline, resulting in a bias).
-    Returns 
-    ----------
-    thermoD: array_like
-        thermocline depth (m)
-    thermoInd: array_like
-        thermocline index corresponding to the thermocline depth
-    
-    Examples
-    ----------
-    >>>     import pylake
-    ...     temp = np.array([14.3,14,12.1,10,9.7,9.5,6,5])
-    ...     depth = np.array([1,2,3,4,5,6,7,8])
-    ...     Sthermo, SthermoInd = pylake.seasonal_thermocline(temp,depth)
-    ...     print(f"Seasonal thermocline depth: {Sthermo}\n")
-    ...     print(f"Seasonal thermocline depth index: {SthermoInd}\n")
-    ...     Seasonal thermocline depth: 6.510728817460102
-    ...     Seasonal thermocline depth index: 6
-    '''
-
-    Temp, depth = to_xarray(Temp, depth, time)
-    time = Temp.time
-    rhoVar = dens0(s=s,t=Temp)
-    drho_dz = rhoVar.diff('depth')/rhoVar.depth.diff('depth')
-
-    dRhoCut = Smin*np.ones(time.size)
-
-    thermoD, thermoInd = thermocline(Temp, depth, smooth=smooth, mixed_cutoff=mixed_cutoff)        
-
-    def process_peaks(arr, Smin, thermoInd):
-        #If no peak is found, set SthermoInd to thermoInd
-        arr = arr.copy()
-        locs, peaks = find_peaks(arr, height=Smin)
-        if (len(locs)and(~np.isnan(locs[-1]))):
-            SthermoInd = locs[-1].astype(int)
-        else:
-            SthermoInd = thermoInd
-        return SthermoInd
-
-    SthermoInd = xr.apply_ufunc(process_peaks, drho_dz, Smin, thermoInd, input_core_dims=[['depth'],[],[]],output_core_dims=[[]], vectorize=True)
-
-    SthermoD = weighted_method(depth, rhoVar, SthermoInd)
-
-    #Compare the seasonal and the diurnal thermocline, seasonal should be at higher depth than the diurnal, if not, both are set equal.
-    mask = (SthermoD<thermoD)
-    SthermoD = SthermoD.where(~mask, thermoD)
-    SthermoInd = SthermoInd.where(~mask, thermoInd)
-
-    SthermoInd = abs(SthermoD-Temp.depth).fillna(999).argmin('depth')
-
-    if len(SthermoD)!=1:
-        if seasonal_smoothed:
-            SthermoD = smooth_1D(SthermoD, seasonal_smoothed)
-            SthermoD = xr.DataArray(SthermoD, coords={'time':time})
-    else:
-        SthermoD = SthermoD.values.item()
-        SthermoInd = SthermoInd.values.item()
-    return SthermoD, SthermoInd
-
-
-def metalimnion(Temp, depth=None, slope=0.1, seasonal=False, mixed_cutoff=1, smooth=False, s=0.2):
-    '''
-    Calculates the top and bottom depth of the metalimnion in a stratified
-    lake. The metalimnion is defined as the water stratum in a stratified lake
-    with the steepest thermal gradient and is demarcated by the bottom of the
-    epilimnion and top of the hypolimnion.
-    
-    Method
-    ----------
-    
-    Parameters
-    ----------
-    Temp :  array_like
-        a numeric vector of water temperature in degrees C
-    depth : array_like
-        a numeric vector corresponding to the depth (in m) of the Temp
-        measurements. Depth is defined as positive, and is minimum at the surface. 
-    slope : scalar, str, default: 0.1
-        a numeric vector corresponding to the minimum slope. Can be set to "relative", if it's the case,
-        the threshold will be 10% of the max slope density gradient.
-    seasonal : bool, default: False
-        Calculates the metalimnion based on the seasonal thermocline if set to True.
-    mixed_cutoff : scalar, default: 1
-        A cutoff (deg C) where below this threshold, thermo.depth and meta.depth are 
-        not calculated (NaN is returned). Defaults to 1 deg C.
-    smooth : bool, default: False
-        Smooth the curve following the scipy savgol filter (window size: 1/5 of the 
-        depth length, order:3, method=nearest)
-        Smoothing is recommended when the thermocline is located at a lower resolution 
-        sensors (sensors are more spaced at the thermocline)
-    s : array_like, default : 0.2
-        Salinity of the water column in PSU
-    thermocline_output : bool, default : False
-        Return the calculated thermocline depth if set to True 
-
-    Returns 
-    ----------
-    epilimnion : array_like, scalar
-        A numeric vector of the epilimnion depth.
-        Returns the thermocline depth if no epilimnion depth is found
-    hypolimnion : array_like, scalar
-        A numeric vector of the hypolimnion depth.
-        Returns the thermocline depth if no hypolimnion depth is found
-    
-    See also
-    ----------
-    pylake.thermocline
-
-    Examples
-    ----------
-    >>>     import pylake
-    ...     temp = np.array([14.3,14,12.1,10,9.7,9.5,6,5])
-    ...     depth = np.array([1,2,3,4,5,6,7,8])
-    ...     epilimnion, hypolimnion = pylake.metalimnion(temp, depth)
-    ...     print(f"Epilimnion: {epilimnion} \n Hypolimnion: {hypolimnion}.")
-    Epilimnion: 2.5
-    Hypolimnion: 3.5
-
-    References
-    ----------
-    Wetzel, R. G. 2001. Limnology: Lake and River Ecosystems, 3rd ed. Academic Press.'''
-
-    Temp, depth = to_xarray(Temp, depth)
-    
-    if smooth:
-        time = Temp.time
-        Temp = smooth_temp(Temp, depth, smooth)
-        Temp, depth = to_xarray(Temp, depth, time)
-
-    if seasonal:
-        thermoD, thermoInd = seasonal_thermocline(Temp, depth, mixed_cutoff=mixed_cutoff, smooth=False)
-    else:
-        thermoD, thermoInd = thermocline(Temp, depth, mixed_cutoff=mixed_cutoff, smooth=False)
-
-    #thermoD, thermoInd = list(map(np.asanyarray, (thermoD, thermoInd)))
-    Temp["thermoInd"] = thermoInd
-    Temp["thermoD"] = thermoD
-
-    rhoVar = dens0(s=s,t=Temp)
-    drho_dz = rhoVar.diff('depth')/rhoVar.depth.diff('depth')
-    drho_dz["depth"] = [(a+b)/2 for a,b in zip(depth, depth[1:])]
-
-    drho_dz["thermoInd"] = abs(drho_dz["thermoD"]-drho_dz["depth"]).fillna(999).argmin('depth')
-    mark =  drho_dz["depth"]-drho_dz["thermoD"]
-
-    if slope=="relative":
-        slope = drho_dz.max('depth')/10
-
-    cond = drho_dz<slope
-
-    mark_value = mark.where(~cond)
-    e_mark = mark_value.where(mark_value<0)
-    h_mark = mark_value.where(mark_value>0)
-    
-    hyp_idx = h_mark.fillna(999).diff('depth').argmax('depth')
-    hyp_depth = h_mark.isel(depth=hyp_idx).depth
-
-    e_marked_rev = abs(e_mark)[::-1]
-    ep_idx_rev = e_marked_rev.fillna(999).diff('depth').argmax(dim='depth')
-    ep_depth = e_marked_rev.isel(depth=ep_idx_rev).depth
-
-    only_NaN_h_mark = (~np.isnan(h_mark)).sum('depth')>0
-    only_NaN_e_mark = (~np.isnan(e_mark)).sum('depth')>0
-    epi_depth = ep_depth.where(only_NaN_e_mark, ep_depth["thermoD"])
-    hypo_depth = hyp_depth.where(only_NaN_h_mark, hyp_depth["thermoD"])
-
-    hypo_depth_filt = hypo_depth.where(hypo_depth>hypo_depth["thermoD"],hypo_depth["thermoD"])
-    epi_depth_filt = epi_depth.where(epi_depth<epi_depth["thermoD"],epi_depth["thermoD"])
-    
-    if epi_depth_filt.size==1:
-        epi_depth_filt = epi_depth_filt.values.item()
-        hypo_depth_filt = hypo_depth_filt.data.item()
-    return epi_depth_filt, hypo_depth_filt
-
-def mixed_layer(Temp, depth=None, threshold=0.2):
-    '''
-    Calculates the mixed layer depth by using the difference temperature method.
-    The depth of the mixed layer is defined as the depth where the temperature difference with the temperature of the surface is greater than a threshold (default 0.1°C).
-    The algorithm does the difference of temperature from the surface to the bottom, reaching lower depth until it reaches a temperature difference lower than the threshold.
-    Surface Temperature might have NaNs. If it's the case, we take a deeper sensor (not more than 1m)
-
-    Parameters
-    -----------
-    depth : array_like 
-        depth vector (m)
-    Temp : array_like
-        Temperature matrix (degrees)
-    Threshold : scalar
-        threshold for the mixing layer detection
-
-    Returns
-    -----------
-    hML array_like
-        Mixed layer depth (m)
-    
-    Example
-    ----------
-    >>>    temp = np.array([14.3,14,12.1,10,9.7,9.5,6,5])
-    ...    depth = np.array([1,2,3,4,5,6,7,8])
-    ...    hML = pylake.mixed_layer(depth, wtr, threshold=0.1)
-    ...    print(hML)
-    '''
-    Temp, depth = to_xarray(Temp, depth)
-
-    T_surf = Temp.isel(depth=0)
-
-    #If surface sensor is NaN, check the second. Can be iterated until a certain depth.
-    NaN = np.where(np.isnan(T_surf))[0]
-    T_surf[NaN] = Temp.isel(time=NaN, depth=1)
-    
-    T_diff = T_surf-Temp.T-threshold
-
-    hML_idx = T_diff.where(T_diff>0).fillna(999).argmin('depth')
-    hML = Temp.depth.isel(depth=hML_idx)
-    if hML.size==1:
-        hML = hML.values.item()
-    return hML
-
-def wedderburn(delta_rho, metaT, uSt, AvHyp_rho, Lo=False, Ao=False, g=9.81):
-    ''' 
-    Wedderburn Number (Wn) is a dimensionless parameter measuring the balance
-    between wind stress and bouyancy force and is used to estimate the amount of
-    upwelling occuring in a lake.  When Wn is much greater than 1, the buoyancy
-    force is much greater than the wind stress and therefore there is a strong
-    vertical stratification with little horizontal variation in the
-    stratification. When Wn is much less than 1, the wind stress is much greater
-    than the bouyancy force and upwelling is likely occuring at the upwind end
-    of the lake. When Wn is near 1, the bouyance force and wind stress are
-    nearly equal and horizontal mixing is considered important
-
-    Parameters
-    ----------
-    delta_rho : array_like 
-        density difference between the epilimnion and the hypolimnion (kg/m3).
-    metaT : array_like:
-        thickness of the surface layer (m)
-    uSt : array_like
-        water friction velocity due to wind stress (m/s)
-    AvHyp_rho : array_like, scalar
-        average water density of the hypolimnion layer (kg/m3)
-    Lo : bool, scalar, default : False
-        fetch length in the direction of the wind (m). If Lo=False, calculate it based on Ao
-    Ao : bool, scalar, default : False
-        Lake surface (m2). Used to calculate Lo (if not given), assume the lake as a perfect circle.
-    g : scalar
-        gravity acceleration (m/s2)
-
-    Returns
-    ----------
-    Wedderburn Number
-    
-    Examples 
-    ----------
-    >>>    delta_rho = np.array([3.1,1.5])
-    ...    metaT = np.array([5.5,2.4])
-    ...    uSt = np.array([0.0028,0.0032])
-    ...    Ao = np.array([80300,120000])
-    ...    AvHyp_rho = np.array([999.31,999.1])
-    ...    pylake.wedderburn(delta_rho, metaT, uSt, AvHyp_rho, Ao=Ao)
-    array([367.22052925  21.19474286])
-
-    Equation
-    ----------   
-    W = (g*delta_rho*(h**2))/(pHyp*(uSt**2)*Lo)
-    where
-    g = gravity acceleration
-    delta_rho (kg/m3) = density difference beTempeen the epilimnion and the hypolimnion 
-    metaT (m)= thickness of the surface layer
-    uSt (m/s)= water friction velocity due to wind stress 
-    Lo = fetch length in the direction of the wind.
-
-    References
-    ----------
-    Read, J.S. et al., 2011. Derivation of lake mixing and stratification indices from high-resolution lake
-    buoy data. Environ. Model. Software 26, 1325–1336. https://doi.org/10.1016/j.
-    Imberger, J., Patterson, J.C., 1990. Physical limnology. Advances in Applied Mechanics 27, 353-370.
-    '''
-    #Must exist a better way to do this
-    try:
-        Lo_cond = len(Lo)
-    except:
-        Lo_cond = Lo
-    try:
-        Ao_cond = len(Ao)
-    except:
-        Ao_cond = Ao
-
-    if not Lo_cond:
-        if Ao_cond:
-            Lo = 2 * np.sqrt(Ao/np.pi);      #Length at thermocline depth
-        else:
-            warnings.warn("Please indicate either Lo or Ao")
-
-    go = g*delta_rho/AvHyp_rho
-    W = go*metaT**2/(uSt**2*Lo)
-    return W 
-
-def schmidt_stability(Temp, depth=None, time=None, bthA=None, bthD=None, sal = 0.2, g=9.81, dz=0.1):
-    '''
-    Schmidt stability, or the resistance to mechanical mixing due to the potential energy inherent in the stratification of the water column.
-
-    Parameters
-    -----------
-    Temp: array_like
-        water temperature in degrees C
-    depth:  array_like, default: None
-        depth of the Temp measurements (m)
-    bthA: array_like: 
-        cross sectional areas (m**2) corresponding to bthD depth
-    bthD: array_like
-        depth (m) which correspond to areal measures in bthA
-    sal: scalar,array_like, default: 0.2
-        Salinity in Practical Salinity Scale units
-    g: scalar, defaults: 9.81
-        gravity acceleration (m/s2)
-    dz: scalar, default: 0.1
-        depth resolution for the integral calculus
-    NaN_interp: bool, defaults : False
-        If NaN_interp=True, it will perform a linear interpolation to replace NaN values
-        The Schmidt stability calculation perform poorly if NaN are present.
-    
-    Returns
-    ----------
-        - Schmidt stability (J/m**2)
-
-    Example
-    ----------
-    >>>    bthA	=	np.array([1000,900,864,820,200,10])
-    ...    bthD	=	np.array([0,2.3,2.5,4.2,5.8,7]) 
-    ...    wtr	=	np.array([28,27,26.4,26,25.4,24,23.3])
-    ...    depth=   np.array([0,1,2,3,4,5,6])  
-    ...    pylake.schmidt_stability(wtr, depth, bthA, bthD, sal=.2, g=self.g)
-    array([21.20261732])
-
-    equation
-    ----------
-    g/A0 int(0,zmax, (zv-z)(rho_i-rho_v)A(z)dz)
-
-    '''
-    Temp, depth = to_xarray(Temp, depth, time)
-    Temp  = Temp.interpolate_na(dim='depth')
-
-    z0 = np.min(depth)
-    I0 = np.argmin(depth)
-    A0 = bthA[I0]
-    rhoL = dens0(t=Temp,s=sal)
-    
-    layerD = np.arange(z0, np.max(depth),dz)
-    layerP = rhoL.interp(depth=layerD)
-    layers = layerP.copy()
-    layerA = np.interp(layerD, bthD, bthA)
-    layers["A"]=('depth', layerA)
-    layers["D"] = layers.depth
-    layers["P"] = layerP
-    Zcv = (layers["D"]@layers["A"])/layers["A"].sum()
-    right_side = ((layers["D"]-Zcv) * layers["A"]) * dz * g / A0
-    St = layers["P"]@right_side
-    return St 
-
-def heat_content(Temp, bthA, bthD, depth=None, s=0.2):
-    '''
-    Calculates the heat content of the water column with temperature and hypsography
-    Heat content is the thermal energy in the water column, which is
-    calculated by multiplying the specific heat of water (J kg-1 K-1) by the
-    temperature and mass of the water in the lake.
-
-    Parameters
-    -----------
-    Temp: array_like: 
-        water temperature in degrees C
-    depth: array_like:
-        depth (in m) of the Temp measurements
-    bthA: array_like:
-        cross sectional areas (m^2) corresponding to bthD depth
-    bthD array_like:
-        depth (m) which correspond to areal measures in bthA
-
-    Returns
-    ---------
-        U: array_like
-            internal energy in Joules m-2
-
-    Example
-    ---------
-    >>>    bthA =np.array([1000,900,864,820,200,10])
-    ...    bthD=np.array([0,2.3,2.5,4.2,5.8,7])
-    ...    wtr	=np.array([28,27,26.4,26,25.4,24,23.3])
-    ...    depth	= np.array([0,1,2,3,4,5,6])
-    ...    lw.internal_energy(wtr, depth, bthA, bthD, s=0.2)
-    ...    520423172.7994813
-    '''
-    dz = 0.1
-    cw = 4186
-    Temp,depth = to_xarray(Temp, depth)
-    #Temp, bthA, bthD, depth = check_bathy(Temp, bthA, bthD, depth)
-    
-    Zo = min(depth)
-    Io = np.argmin(depth)
-    Ao = bthA[Io]
-
-    if Ao==0:
-        print("surface area cannot be zero, check bathymetric file")
-    
-    rhoL = dens0(s=s,t=Temp)
-    layerD = np.arange(Zo, np.max(depth),dz)
-    layerP = rhoL.interp(depth=layerD)
-    layerT = Temp.interp(depth=layerD)
-    layerA = np.interp(layerD, bthD, bthA)
-    layerP["layerA"] = ('depth', layerA)
-
-    v_i = layerP["layerA"]*dz
-    m_i = layerP*v_i
-    u_i = layerT*m_i*cw
-
-    U = u_i.sum('depth')/layerA[0]
-    return U 
-
-
-def seiche_period_1(depth, Zt, Lt, delta_rho, AvHyp_rho, g= 9.81) :
-    '''
-    Estimation of the Seiche periode based on: G. Monismith, 1985; Münnich, Wüest, & Imboden, 1992.
-
-    Parameters
-    -----------
-    depth: array_like:
-        depth (in m) of the Temp measurements
-    Zt: array_like, scalar
-        Thermocline depth 
-    At: scalar 
-        Surface at the thermocline depth 
-    delta_rho: scalar, array_like
-        Density difference between the epilimion and the hypolimnion 
-    AvHyp_rho: array_like, scalar
-        Average density of the hypolimnion
-    g: scalar, default: 9.81
-        gravity acceleration (m/s2)
-
-    Returns
-    ---------
-    T1: array_like, scalar
-        Mode-1 vertical seiche period (s)
-
-    example
-    ---------
-    >>>    bthA =np.array([1000,900,864,820,200,10])
-    ...    bthD=np.array([0,2.3,2.5,4.2,5.8,7])
-    ...    depth	= np.array([0,1,2,3,4,5,6])
-    ...    Zt = 4.5
-    ...    Lt = 4000
-    ...    delta_rho = 0.5
-    ...    AvHyp_rho = 997
-    ...    lw.seiche_period_1(depth, Zt, Lt, delta_rho, AvHyp_rho, g= 9.81)
-    ...    1445418 
-    '''
-    g_reduced = g*delta_rho/AvHyp_rho
-    Zd = depth[-1]
-    h2 = Zd-Zt
-    h1 = Zt
-    T1 = 2*Lt*np.sqrt((h1+h2)/(g_reduced*h1*h2))
-    return T1 
-
-def Lake_number(bthA, bthD, ustar, St, metaT, metaB, averageHypoDense, g=9.81):
-    '''
-    Description: The Lake Number, defined by Imberger and Patterson (1990), has been used to
-    describe processes relevant to the internal mixing of lakes induced by wind
-    forcings. Lower values of Lake Number represent a higher potential for
-    increased diapycnal mixing, which increases the vertical flux of mass and
-    energy across the metalimnion through the action of non-linear internal
-    waves. Lake Number is a dimensionless index.
-
-    Lake Number has been used, for example, to estimate the flux of oxygen
-    across the thermocline in a small lake (Robertson and Imberger, 1994), and
-    to explain the magnitude of the vertical flux of ammonium in a lake (Romero
-    et al., 1998).
-    In Imberger and Patterson (1990), Lake Number was defined as
-    Ln = (g * St * (zm - zT)) / (rho_0 * u*^2 * A0^3/2 * (zm - zg))
-    with all values referenced from the lake bottom, e.g.,
-    zm being the height of the water level, zT the height of metalimnion
-    and zg the height of center volume.
-    Our calculations assume that the reference is at the lake surface, therefore:
-    height of metalimnion becomes metalimnion depth (average of meta top and bot): 
-    (zm - zT) --> (metaT + metaB)/2 
-    height of center of volume depth becomes center of volume depth Zcv:
-    (zm - zg) --> Zcv
-    Further, we note that in that original work St was defined as
-    St = int (z - zg) A(z) rho(z) dz
-    and rLakeAnalyzer defines St as
-    St = g/A0 int (z - zg) rho(z) dz
-    Therefore, we calculate St_uC = St * Ao / g
-
-    Parameters
-    -----------
-    bthA: array_like:
-        a numeric vector of cross sectional areas (m2) corresponding to bthD depth, hypsographic areas
-    bthD: array_like:
-        a numeric vector of depth (m) which correspond to areal measures in bthA, hypsographic depth
-    uStar: array_like:
-        a numeric array of u* (m/s), water friction velocity due to wind stress
-    St: array_like
-        a numeric array of Schmidt stability (J/m2), as defined by Idso 1973
-    metaT: array_like
-        a numeric array of the top of the metalimnion depth (m from the surface)
-    metaB: array_like
-        a numeric array of the bottom of the metalimnion depth (m from the surface)
-    averageHypoDense: array_like:
-        a numeric array of the average density of the hypolimnion (kg/m3)
-    g: scalar, default: 9.81
-        gravity acceleration (m/s2)
-    Returns
-    -----------
-        Ln: A numeric vector of Lake Number [dimensionless]
-
-    Example
-    -----------
-    >>>    bthA =np.array([1000,900,864,820,200,10])
-    ...    bthD=np.array([0,2.3,2.5,4.2,5.8,7])
-    ...    uStar = np.array([0.0032,0.0024])
-    ...    St = np.array([140,153])
-    ...    metaT = np.array([1.34,1.54])
-    ...    metaB = np.array([4.32,4.33])
-    ...    averageHypoDense = np.array([999.3,999.32])
-    ...    lw.Lake_number(bthA, bthD, uStar, St, metaT,metaB,averageHypoDense,self.g)
-    ...    [472.30373072, 951.64555323]
-    references
-    -----------
-    Imberger, J., Patterson, J.C., 1990. Advances in Applied Mechanics 27, 303-475.
-    '''
-    dz	=	0.1
-    A0 = bthA[0]
-    Z0 = bthD[0]
-
-    layerD = np.arange(Z0, np.max(bthD),dz)
-    layerA = np.interp(layerD, bthD, bthA)
-    Zv = layerD*layerA*dz                    
-    Zcv = sum(Zv)/sum(layerA)/dz
-    St_uC = St*A0/g
-    Ln = g*St_uC*(metaT+metaB)/(2*averageHypoDense*ustar**2*A0**(3/2)*Zcv)
-    return Ln 
-
-def buoyancy_freq(Temp, depth=None, g=9.81):
-    '''
-    Description: Calculate the buoyancy frequency (Brunt-Vaisala frequency) for a temperature profile.
-
-    Parameters
-    ----------- 
-    Temp: array_like
-        A numeric vector of water temperature in degrees C
-    depth: array_like
-        a numeric vector corresponding to the depth (in m) of the Temp measurements
-    g: scalar, default: 9.81
-        gravity acceleration (m/s2)
-    
-    Returns
-    ----------
-    n2: array_like
-        a vector of buoyancy frequency in units \code{sec^-2}.
-    n2depth: array_like
-        Return value has attribute "depth" which define buoyancy frequency depth (which differ from supplied depth).
-    
-    Example
-    ----------
-    >>>     wtr = np.array([22.51, 22.42, 22.4, 22.4, 22.4, 22.36, 22.3, 22.21, 22.11, 21.23, 16.42,15.15, 14.24, 13.35, 10.94, 10.43, 10.36, 9.94, 9.45, 9.1, 8.91, 8.58, 8.43])
-    ...    depth = np.array([0, 0.5, 1, 1.5, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20])
-    ...    avg_depth, buoy_freq = lw.buoyancy_freq(wtr, depth, self.g)
-    ...    plt.pcolormesh(buoy_freq)
-    ... array([4.10503572e-04, 9.10051748e-05, 0.00000000e+00, 0.00000000e+00,
-        9.08868567e-05, 1.36034054e-04, 2.03383759e-04, 2.25040545e-04,
-        1.93749334e-03, 9.17368987e-03, 2.00052155e-03, 1.31951341e-03,
-        1.19625956e-03, 2.75490678e-03, 4.89153665e-04, 6.45127824e-05,
-        3.73658150e-04, 4.06586584e-04, 2.70840415e-04, 1.40129203e-04,
-        2.31752785e-04, 1.00430572e-04])
-    '''
-    Temp, depth = to_xarray(Temp,depth)
-    rho = dens0(s=0.2, t=Temp)
-    numdepth = len(depth)
-    rho_2 = rho.isel(depth=slice(0,numdepth-1))
-    drho_dz = rho.diff('depth')/Temp.depth.diff('depth')
-    rho_2["depth"] = drho_dz.depth
-    n2 = g/rho_2*drho_dz
-    n2["depth"] = [(a+b)/2 for a,b in zip(depth, depth[1:])]
-    n2 = n2.rename({"depth":"avg_depth"})
-    return n2 
-
-def Average_layer_temp(Temp, depth_ref, layer='top', depth=None):
-    '''
-    Perform the layer average temperature based on the thermocline depth 
-
-    Parameters
-    -----------
-    Temp: array_like, xarray: 
-        A dataset containing the temperature. Must be of the same dimensions than the thermocline depth.
-    depth_ref: array_like:
-        reference depth in which the averaged temperature above or under is calculated.
-    layer: str, default: 'top'
-        layer='top' will do the average temperature above the depth_ref
-        layer='bot' will do the average temperature under the depth_ref
-    depth: array_like
-        a numeric vector corresponding to the depth (in m) of the Temp measurements. Necessary if not using xarray
-
-    Returns
-    -----------
-    mean_temp: array_like
-        dataset with the mean layer temperature
-
-    Examples
-    -----------
-    >>> wtr = np.array([22.51, 22.42, 22.4, 22.4, 22.4, 22.36, 22.3, 22.21, 22.11, 21.23, 16.42,15.15, 14.24, 13.35, 10.94, 10.43, 10.36, 9.94, 9.45, 9.1, 8.91, 8.58, 8.43])
-    ... depth = np.array([0, 0.5, 1, 1.5, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20])
-    ... depth_ref = 9 
-    ... lw.Average_layer_temp(wtr, depth, depth_ref, top=True)
-    ... 21.70
-    ... lw.Average_layer_temp(wtr, depth, depth_ref, top=True)
-    ... 10.33
-    '''
-    Temp, depth = to_xarray(Temp,depth)
-
-    if layer=='top':
-        mask = (Temp.depth<depth_ref)
-    elif layer=='bot':
-        mask = (Temp.depth>depth_ref)
-    else:
-        warnings.warnings("Temperature average of the whole water column")
-        mean_temp = Temp.mean(dim="depth")
-        return mean_temp
-    masked_temp = Temp.where(mask)
-    mean_temp = masked_temp.mean(dim="depth")
-    return mean_temp
-
-def Surface_Buoyancy_Flux(swT,sHFturb0,rho0):
-    '''
-    Calculate the surface buyoancy flux
-
-    Parameters
-    -------------
-    swT: array_like, unit: °C
-        Surface water temperature in °C 
-    sHFturb0: array_like, unit: W/m2
-        Net Surface Heat Flux - Absorbed Shortwave Radiation 
-    rho0: array_like
-        Lake Surface Density kg/m3
-
-    returns
-    -------------
-    JB0: array_like
-        Surface buoyancy flux W/m2
-    '''
-    JB0 = sw.alpha(0.2,swT,0)*9.81/sw.cp(0.2,swT,0)*sHFturb0/rho0
-    return JB0
-
-def Monin_Obukhov(ustar, JB0):
-    '''
-    Calculate Monin-Obhukov length
-
-    Parameters
-    -------------
-    ustar: array_like, unit: m/s
-        Shear Velocity on water
-    JB0: array_like, unit: W/m2
-        Surface buoyancy flux 
-    '''
-    LMO = ustar**3/0.4/JB0
-    return LMO
+import numpy as np
+from .functions import *
+import seawater as sw
+from scipy.interpolate import interp1d
+import warnings
+from scipy.signal import find_peaks,savgol_filter
+import xarray as xr
+    
+def thermocline(Temp, depth=None, time=None, s=0.2, mixed_cutoff=1, smooth=False):
+    '''
+    Calculate the thermocline depth from one or various temperature profiles.
+    It uses the method of the maximum gradient, the results can be interpreted
+    as a diurnal thermocline (see pylake.seasonal_thermocline for the seasonal).
+
+    Method
+    ----------
+    The thermocline is calculated using the maximum gradient of density.
+    If the temperature profile have a variability in depth resolution, it is recommended 
+    to smooth the profile to avoid resolution influence on the algorithm.
+    Once the maximum gradient of density is found, a special technique to refine the 
+    thermocline depth is used and presented in (Read et al., 2011).
+
+    Parameters
+    ----------
+    Temp :  array_like
+        a numeric vector of water temperature in degrees C
+    depth : array_like
+        a numeric vector corresponding to the depth (in m) of the Temp
+    s : array_like, default : 0.2
+        Salinity of the water column in PSU
+    Smin : float, default: 0.1 °C/m
+        Optional parameter defining minimum density gradient for
+        thermocline.
+    mixed_cutoff : scalar, default: 1
+        The difference between the maximum and minimum of the
+        temperature profile should be higher than this cutoff.
+    smooth : bool, default: False
+        Smooth the curve following the scipy savgol filter (window size: 1/10 of the 
+        depth length, order:3, method=nearest)
+        Smoothing is recommended when the thermocline is located at a lower resolution 
+        sensors (sensors are more spaced at the thermocline)
+
+    Returns 
+    ----------
+    thermoD: array_like, scalar
+        thermocline depth (m)
+    thermoInd: array_like, scalar
+        thermocline index corresponding to the thermocline depth
+    
+    Examples
+    ----------
+    >>>     import pylake
+    ...     temp = temp = np.array([14.3,14,12.1,10,9.7,9.5,6,5])
+    ...     depth = depth = np.array([1,2,3,4,5,6,7,8])
+    ...     thermo, thermoInd = pylake.thermocline(temp,depth)
+    ...     print(f"thermocline depth: {thermo}\n")
+    ...     print(f"thermocline depth index: {thermoInd}\n")
+    ...     thermocline depth: 2.878790569183019
+    ...     thermocline depth index: 2
+    '''
+
+    Temp, depth = to_xarray(Temp, depth,time)
+
+    is_not_significant = Temp.max('depth')-Temp.min('depth')<mixed_cutoff
+    if smooth:
+        time = Temp.time
+        Temp = smooth_temp(Temp, depth, smooth)
+        Temp, depth = to_xarray(Temp, depth,time)
+
+    rhoVar = dens0(s=s,t=Temp)
+    drho_dz = rhoVar.diff('depth')/rhoVar.depth.diff('depth')
+    inf_mask = np.isinf(drho_dz)
+    drho_dz = drho_dz.where(~inf_mask, np.nan)
+    thermoInd = drho_dz.fillna(-999).argmax('depth')
+
+    thermoD = weighted_method(depth, rhoVar, thermoInd)
+
+    thermoInd = abs(thermoD-Temp.depth).fillna(999).argmin('depth')
+
+    thermoD = thermoD.where(~is_not_significant, np.nan)
+
+    if thermoD.size==1:
+        thermoD = thermoD.values.item()
+        thermoInd = thermoInd.data.item()
+    return thermoD, thermoInd
+
+
+
+def seasonal_thermocline(Temp, depth=None, time=None, s=0.2, mixed_cutoff=1, Smin=0.1, seasonal_smoothed=True, smooth=False):
+    '''
+    Calculate depth of the thermocline from a temperature profile.
+    
+    Method
+    ---------
+    The seasonal thermocline uses the find_peaks from scipy to find the first 
+    local maximum (higher than a certain threshold, based on Smin) starting 
+    from the bottom of the profile.
+    By default, if no peak is found, the seasonal thermocline is set equal to 
+    the diurnal thermocline. 
+    The same refining technique is used.
+    A savgol filter (special moving averaged filter) is used to smooth the data 
+    and discard extremums.
+    The seasonal is set to be more or equal to the diurnal thermocline.
+    Keep in mind that if the seasonal thermocline is often assimilated 
+    with the diurnal, with the exception that the seasonal is artificially smoothed.
+
+    Parameters
+    ----------
+    Temp :  array_like
+        a numeric vector of water temperature in degrees C
+    depth : array_like
+        a numeric vector corresponding to the depth of the temperature.
+        Depth is defined as positive, and is minimum at the surface. 
+    s : array_like, default : 0.2
+        Salinity of the water column in PSU
+    mixed_cutoff : scalar, default: 1
+        The difference between the maximum and minimum of the
+        temperature profile should be higher than this cutoff.
+    Smin : float, default: 0.1 °C/m
+        Optional parameter defining minimum density gradient for
+        thermocline. Threshold for the peak height of the scipy.signal.find_peaks(...).
+    seasonal_smoothed: bool, default: True
+        Smooth the seasonal thermocline on the entire time serie. The smooth depends on the time serie length.
+    smooth : bool, default: False
+        Smooth the curve following the scipy savgol filter (window size: 1/10 of the 
+        depth length, order:3, method=nearest)
+        Smoothing is recommended when the thermocline is located at a lower resolution 
+        sensors (sensors can be more spaced at the thermocline, resulting in a bias).
+    Returns 
+    ----------
+    thermoD: array_like
+        thermocline depth (m)
+    thermoInd: array_like
+        thermocline index corresponding to the thermocline depth
+    
+    Examples
+    ----------
+    >>>     import pylake
+    ...     temp = np.array([14.3,14,12.1,10,9.7,9.5,6,5])
+    ...     depth = np.array([1,2,3,4,5,6,7,8])
+    ...     Sthermo, SthermoInd = pylake.seasonal_thermocline(temp,depth)
+    ...     print(f"Seasonal thermocline depth: {Sthermo}\n")
+    ...     print(f"Seasonal thermocline depth index: {SthermoInd}\n")
+    ...     Seasonal thermocline depth: 6.510728817460102
+    ...     Seasonal thermocline depth index: 6
+    '''
+
+    Temp, depth = to_xarray(Temp, depth, time)
+    time = Temp.time
+    rhoVar = dens0(s=s,t=Temp)
+    drho_dz = rhoVar.diff('depth')/rhoVar.depth.diff('depth')
+
+    dRhoCut = Smin*np.ones(time.size)
+
+    thermoD, thermoInd = thermocline(Temp, depth, smooth=smooth, mixed_cutoff=mixed_cutoff)        
+
+    def process_peaks(arr, Smin, thermoInd):
+        #If no peak is found, set SthermoInd to thermoInd
+        arr = arr.copy()
+        locs, peaks = find_peaks(arr, height=Smin)
+        if (len(locs)and(~np.isnan(locs[-1]))):
+            SthermoInd = locs[-1].astype(int)
+        else:
+            SthermoInd = thermoInd
+        return SthermoInd
+
+    SthermoInd = xr.apply_ufunc(process_peaks, drho_dz, Smin, thermoInd, input_core_dims=[['depth'],[],[]],output_core_dims=[[]], vectorize=True)
+
+    SthermoD = weighted_method(depth, rhoVar, SthermoInd)
+
+    #Compare the seasonal and the diurnal thermocline, seasonal should be at higher depth than the diurnal, if not, both are set equal.
+    mask = (SthermoD<thermoD)
+    SthermoD = SthermoD.where(~mask, thermoD)
+    SthermoInd = SthermoInd.where(~mask, thermoInd)
+
+    SthermoInd = abs(SthermoD-Temp.depth).fillna(999).argmin('depth')
+
+    if len(SthermoD)!=1:
+        if seasonal_smoothed:
+            SthermoD = smooth_1D(SthermoD, seasonal_smoothed)
+            SthermoD = xr.DataArray(SthermoD, coords={'time':time})
+    else:
+        SthermoD = SthermoD.values.item()
+        SthermoInd = SthermoInd.values.item()
+    return SthermoD, SthermoInd
+
+
+def metalimnion(Temp, depth=None, slope=0.1, seasonal=False, mixed_cutoff=1, smooth=False, s=0.2):
+    '''
+    Calculates the top and bottom depth of the metalimnion in a stratified
+    lake. The metalimnion is defined as the water stratum in a stratified lake
+    with the steepest thermal gradient and is demarcated by the bottom of the
+    epilimnion and top of the hypolimnion.
+    
+    Method
+    ----------
+    
+    Parameters
+    ----------
+    Temp :  array_like
+        a numeric vector of water temperature in degrees C
+    depth : array_like
+        a numeric vector corresponding to the depth (in m) of the Temp
+        measurements. Depth is defined as positive, and is minimum at the surface. 
+    slope : scalar, str, default: 0.1
+        a numeric vector corresponding to the minimum slope. Can be set to "relative", if it's the case,
+        the threshold will be 10% of the max slope density gradient.
+    seasonal : bool, default: False
+        Calculates the metalimnion based on the seasonal thermocline if set to True.
+    mixed_cutoff : scalar, default: 1
+        A cutoff (deg C) where below this threshold, thermo.depth and meta.depth are 
+        not calculated (NaN is returned). Defaults to 1 deg C.
+    smooth : bool, default: False
+        Smooth the curve following the scipy savgol filter (window size: 1/5 of the 
+        depth length, order:3, method=nearest)
+        Smoothing is recommended when the thermocline is located at a lower resolution 
+        sensors (sensors are more spaced at the thermocline)
+    s : array_like, default : 0.2
+        Salinity of the water column in PSU
+    thermocline_output : bool, default : False
+        Return the calculated thermocline depth if set to True 
+
+    Returns 
+    ----------
+    epilimnion : array_like, scalar
+        A numeric vector of the epilimnion depth.
+        Returns the thermocline depth if no epilimnion depth is found
+    hypolimnion : array_like, scalar
+        A numeric vector of the hypolimnion depth.
+        Returns the thermocline depth if no hypolimnion depth is found
+    
+    See also
+    ----------
+    pylake.thermocline
+
+    Examples
+    ----------
+    >>>     import pylake
+    ...     temp = np.array([14.3,14,12.1,10,9.7,9.5,6,5])
+    ...     depth = np.array([1,2,3,4,5,6,7,8])
+    ...     epilimnion, hypolimnion = pylake.metalimnion(temp, depth)
+    ...     print(f"Epilimnion: {epilimnion} \n Hypolimnion: {hypolimnion}.")
+    Epilimnion: 2.5
+    Hypolimnion: 3.5
+
+    References
+    ----------
+    Wetzel, R. G. 2001. Limnology: Lake and River Ecosystems, 3rd ed. Academic Press.'''
+
+    Temp, depth = to_xarray(Temp, depth)
+    
+    if smooth:
+        time = Temp.time
+        Temp = smooth_temp(Temp, depth, smooth)
+        Temp, depth = to_xarray(Temp, depth, time)
+
+    if seasonal:
+        thermoD, thermoInd = seasonal_thermocline(Temp, depth, mixed_cutoff=mixed_cutoff, smooth=False)
+    else:
+        thermoD, thermoInd = thermocline(Temp, depth, mixed_cutoff=mixed_cutoff, smooth=False)
+
+    #thermoD, thermoInd = list(map(np.asanyarray, (thermoD, thermoInd)))
+    Temp["thermoInd"] = thermoInd
+    Temp["thermoD"] = thermoD
+
+    rhoVar = dens0(s=s,t=Temp)
+    drho_dz = rhoVar.diff('depth')/rhoVar.depth.diff('depth')
+    drho_dz["depth"] = [(a+b)/2 for a,b in zip(depth, depth[1:])]
+
+    drho_dz["thermoInd"] = abs(drho_dz["thermoD"]-drho_dz["depth"]).fillna(999).argmin('depth')
+    mark =  drho_dz["depth"]-drho_dz["thermoD"]
+
+    if slope=="relative":
+        slope = drho_dz.max('depth')/10
+
+    cond = drho_dz<slope
+
+    mark_value = mark.where(~cond)
+    e_mark = mark_value.where(mark_value<0)
+    h_mark = mark_value.where(mark_value>0)
+    
+    hyp_idx = h_mark.fillna(999).diff('depth').argmax('depth')
+    hyp_depth = h_mark.isel(depth=hyp_idx).depth
+
+    e_marked_rev = abs(e_mark)[::-1]
+    ep_idx_rev = e_marked_rev.fillna(999).diff('depth').argmax(dim='depth')
+    ep_depth = e_marked_rev.isel(depth=ep_idx_rev).depth
+
+    only_NaN_h_mark = (~np.isnan(h_mark)).sum('depth')>0
+    only_NaN_e_mark = (~np.isnan(e_mark)).sum('depth')>0
+    epi_depth = ep_depth.where(only_NaN_e_mark, ep_depth["thermoD"])
+    hypo_depth = hyp_depth.where(only_NaN_h_mark, hyp_depth["thermoD"])
+
+    hypo_depth_filt = hypo_depth.where(hypo_depth>hypo_depth["thermoD"],hypo_depth["thermoD"])
+    epi_depth_filt = epi_depth.where(epi_depth<epi_depth["thermoD"],epi_depth["thermoD"])
+    
+    if epi_depth_filt.size==1:
+        epi_depth_filt = epi_depth_filt.values.item()
+        hypo_depth_filt = hypo_depth_filt.data.item()
+    return epi_depth_filt, hypo_depth_filt
+
+def mixed_layer(Temp, depth=None, s=0.2, threshold=0.01):
+    '''
+    Calculates the mixed layer depth by using the density difference method.
+    The depth of the mixed layer is defined as the depth where the density difference with the density of the surface is greater than a threshold (default 0.01 kg/m3).
+    The algorithm does the difference of density from the surface to the bottom, reaching lower depth until it reaches a density difference lower than the threshold.
+    Surface density might have NaNs. If it's the case, we take a deeper sensor (not more than 1m)
+
+    Parameters
+    -----------
+    depth : array_like 
+        depth vector (m)
+    Temp : array_like
+        Temperature matrix (degrees)
+    s   : array_like
+        Salinity matrix (psu)
+    Threshold : scalar
+        threshold for the mixing layer detection
+
+    Returns
+    -----------
+    hML array_like
+        Mixed layer depth (m)
+    
+    Example
+    ----------
+    >>>    temp = np.array([14.3,14,12.1,10,9.7,9.5,6,5])
+    ...    depth = np.array([1,2,3,4,5,6,7,8])
+    ...    hML = pylake.mixed_layer(depth, wtr, threshold=0.1)
+    ...    print(hML)
+    '''
+    Temp, depth = to_xarray(Temp, depth)
+    rho = dens0(s=s,t=Temp)
+
+    rho_surf = rho.isel(depth=0)
+
+    #If surface sensor is NaN, check the second. Can be iterated until a certain depth.
+    NaN = np.where(np.isnan(rho_surf))[0]
+    rho_surf[NaN] = rho.isel(time=NaN, depth=1)
+    
+    rho_diff = rho.T - rho_surf - threshold
+
+    # Replace NaNs with 999 to indicate they don't fulfill the condition
+    rho_diff_filled = rho_diff.where(rho_diff > 0, other=999)
+
+    # Find the index of the minimum value along the depth dimension
+    hML_idx = rho_diff_filled.argmin('depth')
+
+    # Ensure hML_idx correctly handles the case where the condition is not met
+    if rho_diff_filled.isel(depth=hML_idx).values == 999:
+            hML_idx = len(rho.depth) - 1
+
+    # Get the depth corresponding to hML_idx
+    hML = rho.depth.isel(depth=hML_idx)
+    if hML.size == 1:
+            hML = hML.values.item()
+    return hML
+
+def wedderburn(delta_rho, metaT, uSt, AvHyp_rho, Lo=False, Ao=False, g=9.81):
+    ''' 
+    Wedderburn Number (Wn) is a dimensionless parameter measuring the balance
+    between wind stress and bouyancy force and is used to estimate the amount of
+    upwelling occuring in a lake.  When Wn is much greater than 1, the buoyancy
+    force is much greater than the wind stress and therefore there is a strong
+    vertical stratification with little horizontal variation in the
+    stratification. When Wn is much less than 1, the wind stress is much greater
+    than the bouyancy force and upwelling is likely occuring at the upwind end
+    of the lake. When Wn is near 1, the bouyance force and wind stress are
+    nearly equal and horizontal mixing is considered important
+
+    Parameters
+    ----------
+    delta_rho : array_like 
+        density difference between the epilimnion and the hypolimnion (kg/m3).
+    metaT : array_like:
+        thickness of the surface layer (m)
+    uSt : array_like
+        water friction velocity due to wind stress (m/s)
+    AvHyp_rho : array_like, scalar
+        average water density of the hypolimnion layer (kg/m3)
+    Lo : bool, scalar, default : False
+        fetch length in the direction of the wind (m). If Lo=False, calculate it based on Ao
+    Ao : bool, scalar, default : False
+        Lake surface (m2). Used to calculate Lo (if not given), assume the lake as a perfect circle.
+    g : scalar
+        gravity acceleration (m/s2)
+
+    Returns
+    ----------
+    Wedderburn Number
+    
+    Examples 
+    ----------
+    >>>    delta_rho = np.array([3.1,1.5])
+    ...    metaT = np.array([5.5,2.4])
+    ...    uSt = np.array([0.0028,0.0032])
+    ...    Ao = np.array([80300,120000])
+    ...    AvHyp_rho = np.array([999.31,999.1])
+    ...    pylake.wedderburn(delta_rho, metaT, uSt, AvHyp_rho, Ao=Ao)
+    array([367.22052925  21.19474286])
+
+    Equation
+    ----------   
+    W = (g*delta_rho*(h**2))/(pHyp*(uSt**2)*Lo)
+    where
+    g = gravity acceleration
+    delta_rho (kg/m3) = density difference beTempeen the epilimnion and the hypolimnion 
+    metaT (m)= thickness of the surface layer
+    uSt (m/s)= water friction velocity due to wind stress 
+    Lo = fetch length in the direction of the wind.
+
+    References
+    ----------
+    Read, J.S. et al., 2011. Derivation of lake mixing and stratification indices from high-resolution lake
+    buoy data. Environ. Model. Software 26, 1325–1336. https://doi.org/10.1016/j.
+    Imberger, J., Patterson, J.C., 1990. Physical limnology. Advances in Applied Mechanics 27, 353-370.
+    '''
+    #Must exist a better way to do this
+    try:
+        Lo_cond = len(Lo)
+    except:
+        Lo_cond = Lo
+    try:
+        Ao_cond = len(Ao)
+    except:
+        Ao_cond = Ao
+
+    if not Lo_cond:
+        if Ao_cond:
+            Lo = 2 * np.sqrt(Ao/np.pi);      #Length at thermocline depth
+        else:
+            warnings.warn("Please indicate either Lo or Ao")
+
+    go = g*delta_rho/AvHyp_rho
+    W = go*metaT**2/(uSt**2*Lo)
+    return W 
+
+def schmidt_stability(Temp, depth=None, time=None, bthA=None, bthD=None, sal = 0.2, g=9.81, dz=0.1):
+    '''
+    Schmidt stability, or the resistance to mechanical mixing due to the potential energy inherent in the stratification of the water column.
+
+    Parameters
+    -----------
+    Temp: array_like
+        water temperature in degrees C
+    depth:  array_like, default: None
+        depth of the Temp measurements (m)
+    bthA: array_like: 
+        cross sectional areas (m**2) corresponding to bthD depth
+    bthD: array_like
+        depth (m) which correspond to areal measures in bthA
+    sal: scalar,array_like, default: 0.2
+        Salinity in Practical Salinity Scale units
+    g: scalar, defaults: 9.81
+        gravity acceleration (m/s2)
+    dz: scalar, default: 0.1
+        depth resolution for the integral calculus
+    NaN_interp: bool, defaults : False
+        If NaN_interp=True, it will perform a linear interpolation to replace NaN values
+        The Schmidt stability calculation perform poorly if NaN are present.
+    
+    Returns
+    ----------
+        - Schmidt stability (J.m-2)
+
+    Example
+    ----------
+    >>>    bthA	=	np.array([1000,900,864,820,200,10])
+    ...    bthD	=	np.array([0,2.3,2.5,4.2,5.8,7]) 
+    ...    wtr	=	np.array([28,27,26.4,26,25.4,24,23.3])
+    ...    depth=   np.array([0,1,2,3,4,5,6])  
+    ...    pylake.schmidt_stability(wtr, depth, bthA, bthD, sal=.2, g=self.g)
+    array([21.20261732])
+
+    equation
+    ----------
+    g/A0 int(0,zmax, (zv-z)(rho_i-rho_v)A(z)dz)
+
+    '''
+    Temp, depth = to_xarray(Temp, depth, time)
+    Temp  = Temp.interpolate_na(dim='depth')
+
+    z0 = np.min(depth)
+    I0 = np.argmin(depth)
+    A0 = bthA[I0]
+    rhoL = dens0(t=Temp,s=sal)
+    
+    layerD = np.arange(z0, np.max(depth),dz)
+    layerP = rhoL.interp(depth=layerD)
+    layers = layerP.copy()
+    layerA = np.interp(layerD, bthD, bthA)
+    layers["A"]=('depth', layerA)
+    layers["D"] = layers.depth
+    layers["P"] = layerP
+    Zcv = (layers["D"]@layers["A"])/layers["A"].sum()
+    right_side = ((layers["D"]-Zcv) * layers["A"]) * dz * g / A0
+    St = layers["P"]@right_side
+    return St 
+
+def heat_content(Temp, bthA, bthD, depth=None, s=0.2):
+    '''
+    Calculates the heat content of the water column with temperature and hypsography
+    Heat content is the thermal energy in the water column, which is
+    calculated by multiplying the specific heat of water (J kg-1 K-1) by the
+    temperature and mass of the water in the lake.
+
+    Parameters
+    -----------
+    Temp: array_like: 
+        water temperature in degrees C
+    depth: array_like:
+        depth (in m) of the Temp measurements
+    bthA: array_like:
+        cross sectional areas (m^2) corresponding to bthD depth
+    bthD array_like:
+        depth (m) which correspond to areal measures in bthA
+
+    Returns
+    ---------
+        U: array_like
+            internal energy in Joules m-2
+
+    Example
+    ---------
+    >>>    bthA =np.array([1000,900,864,820,200,10])
+    ...    bthD=np.array([0,2.3,2.5,4.2,5.8,7])
+    ...    wtr	=np.array([28,27,26.4,26,25.4,24,23.3])
+    ...    depth	= np.array([0,1,2,3,4,5,6])
+    ...    lw.internal_energy(wtr, depth, bthA, bthD, s=0.2)
+    ...    520423172.7994813
+    '''
+    dz = 0.1
+    cw = 4186
+    Temp,depth = to_xarray(Temp, depth)
+    #Temp, bthA, bthD, depth = check_bathy(Temp, bthA, bthD, depth)
+    
+    Zo = min(depth)
+    Io = np.argmin(depth)
+    Ao = bthA[Io]
+
+    if Ao==0:
+        print("surface area cannot be zero, check bathymetric file")
+    
+    rhoL = dens0(s=s,t=Temp)
+    layerD = np.arange(Zo, np.max(depth),dz)
+    layerP = rhoL.interp(depth=layerD)
+    layerT = Temp.interp(depth=layerD)
+    layerA = np.interp(layerD, bthD, bthA)
+    layerP["layerA"] = ('depth', layerA)
+
+    v_i = layerP["layerA"]*dz
+    m_i = layerP*v_i
+    u_i = layerT*m_i*cw
+
+    U = u_i.sum('depth')/layerA[0]
+    return U 
+
+
+def seiche_period_1(depth, Zt, Lt, delta_rho, AvHyp_rho, g= 9.81) :
+    '''
+    Estimation of the Seiche periode based on: G. Monismith, 1985; Münnich, Wüest, & Imboden, 1992.
+
+    Parameters
+    -----------
+    depth: array_like:
+        depth (in m) of the Temp measurements
+    Zt: array_like, scalar
+        Thermocline depth 
+    At: scalar 
+        Surface at the thermocline depth 
+    delta_rho: scalar, array_like
+        Density difference between the epilimion and the hypolimnion 
+    AvHyp_rho: array_like, scalar
+        Average density of the hypolimnion
+    g: scalar, default: 9.81
+        gravity acceleration (m/s2)
+
+    Returns
+    ---------
+    T1: array_like, scalar
+        Mode-1 vertical seiche period (h)
+
+    example
+    ---------
+    >>>    bthA =np.array([1000,900,864,820,200,10])
+    ...    bthD=np.array([0,2.3,2.5,4.2,5.8,7])
+    ...    depth	= np.array([0,1,2,3,4,5,6])
+    ...    Zt = 4.5
+    ...    Lt = 4000
+    ...    delta_rho = 0.5
+    ...    AvHyp_rho = 997
+    ...    lw.seiche_period_1(depth, Zt, Lt, delta_rho, AvHyp_rho, g= 9.81)
+    ...    1445418 
+    '''
+    g_reduced = g*delta_rho/AvHyp_rho
+    Zd = depth[-1]
+    h2 = Zd-Zt
+    h1 = Zt
+    T1 = 2*Lt*np.sqrt((h1+h2)/(g_reduced*h1*h2))
+    return T1*60*60
+
+def Lake_number(bthA, bthD, ustar, St, metaT, metaB, averageHypoDense, g=9.81):
+    '''
+    Description: The Lake Number, defined by Imberger and Patterson (1990), has been used to
+    describe processes relevant to the internal mixing of lakes induced by wind
+    forcings. Lower values of Lake Number represent a higher potential for
+    increased diapycnal mixing, which increases the vertical flux of mass and
+    energy across the metalimnion through the action of non-linear internal
+    waves. Lake Number is a dimensionless index.
+
+    Lake Number has been used, for example, to estimate the flux of oxygen
+    across the thermocline in a small lake (Robertson and Imberger, 1994), and
+    to explain the magnitude of the vertical flux of ammonium in a lake (Romero
+    et al., 1998).
+    In Imberger and Patterson (1990), Lake Number was defined as
+    Ln = (g * St * (zm - zT)) / (rho_0 * u*^2 * A0^3/2 * (zm - zg))
+    with all values referenced from the lake bottom, e.g.,
+    zm being the height of the water level, zT the height of metalimnion
+    and zg the height of center volume.
+    Our calculations assume that the reference is at the lake surface, therefore:
+    height of metalimnion becomes metalimnion depth (average of meta top and bot): 
+    (zm - zT) --> (metaT + metaB)/2 
+    height of center of volume depth becomes center of volume depth Zcv:
+    (zm - zg) --> Zcv
+    Further, we note that in that original work St was defined as
+    St = int (z - zg) A(z) rho(z) dz
+    and rLakeAnalyzer defines St as
+    St = g/A0 int (z - zg) rho(z) dz
+    Therefore, we calculate St_uC = St * Ao / g
+
+    Parameters
+    -----------
+    bthA: array_like:
+        a numeric vector of cross sectional areas (m2) corresponding to bthD depth, hypsographic areas
+    bthD: array_like:
+        a numeric vector of depth (m) which correspond to areal measures in bthA, hypsographic depth
+    uStar: array_like:
+        a numeric array of u* (m/s), water friction velocity due to wind stress
+    St: array_like
+        a numeric array of Schmidt stability (J/m2), as defined by Idso 1973
+    metaT: array_like
+        a numeric array of the top of the metalimnion depth (m from the surface)
+    metaB: array_like
+        a numeric array of the bottom of the metalimnion depth (m from the surface)
+    averageHypoDense: array_like:
+        a numeric array of the average density of the hypolimnion (kg/m3)
+    g: scalar, default: 9.81
+        gravity acceleration (m/s2)
+    Returns
+    -----------
+        Ln: A numeric vector of Lake Number [dimensionless]
+
+    Example
+    -----------
+    >>>    bthA =np.array([1000,900,864,820,200,10])
+    ...    bthD=np.array([0,2.3,2.5,4.2,5.8,7])
+    ...    uStar = np.array([0.0032,0.0024])
+    ...    St = np.array([140,153])
+    ...    metaT = np.array([1.34,1.54])
+    ...    metaB = np.array([4.32,4.33])
+    ...    averageHypoDense = np.array([999.3,999.32])
+    ...    lw.Lake_number(bthA, bthD, uStar, St, metaT,metaB,averageHypoDense,self.g)
+    ...    [472.30373072, 951.64555323]
+    references
+    -----------
+    Imberger, J., Patterson, J.C., 1990. Advances in Applied Mechanics 27, 303-475.
+    '''
+    dz	=	0.1
+    A0 = bthA[0]
+    Z0 = bthD[0]
+
+    layerD = np.arange(Z0, np.max(bthD),dz)
+    layerA = np.interp(layerD, bthD, bthA)
+    Zv = layerD*layerA*dz                    
+    Zcv = sum(Zv)/sum(layerA)/dz
+    St_uC = St*A0/g
+    Ln = g*St_uC*(metaT+metaB)/(2*averageHypoDense*ustar**2*A0**(3/2)*Zcv)
+    return Ln 
+
+def buoyancy_freq(Temp, depth=None, g=9.81):
+    '''
+    Description: Calculate the buoyancy frequency (Brunt-Vaisala frequency) for a temperature profile.
+
+    Parameters
+    ----------- 
+    Temp: array_like
+        A numeric vector of water temperature in degrees C
+    depth: array_like
+        a numeric vector corresponding to the depth (in m) of the Temp measurements
+    g: scalar, default: 9.81
+        gravity acceleration (m/s2)
+    
+    Returns
+    ----------
+    n2: array_like
+        a vector of buoyancy frequency in units \code{sec^-2}.
+    n2depth: array_like
+        Return value has attribute "depth" which define buoyancy frequency depth (which differ from supplied depth).
+    
+    Example
+    ----------
+    >>>     wtr = np.array([22.51, 22.42, 22.4, 22.4, 22.4, 22.36, 22.3, 22.21, 22.11, 21.23, 16.42,15.15, 14.24, 13.35, 10.94, 10.43, 10.36, 9.94, 9.45, 9.1, 8.91, 8.58, 8.43])
+    ...    depth = np.array([0, 0.5, 1, 1.5, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20])
+    ...    avg_depth, buoy_freq = lw.buoyancy_freq(wtr, depth, self.g)
+    ...    plt.pcolormesh(buoy_freq)
+    ... array([4.10503572e-04, 9.10051748e-05, 0.00000000e+00, 0.00000000e+00,
+        9.08868567e-05, 1.36034054e-04, 2.03383759e-04, 2.25040545e-04,
+        1.93749334e-03, 9.17368987e-03, 2.00052155e-03, 1.31951341e-03,
+        1.19625956e-03, 2.75490678e-03, 4.89153665e-04, 6.45127824e-05,
+        3.73658150e-04, 4.06586584e-04, 2.70840415e-04, 1.40129203e-04,
+        2.31752785e-04, 1.00430572e-04])
+    '''
+    Temp, depth = to_xarray(Temp,depth)
+    rho = dens0(s=0.2, t=Temp)
+    numdepth = len(depth)
+    rho_2 = rho.isel(depth=slice(0,numdepth-1))
+    drho_dz = rho.diff('depth')/Temp.depth.diff('depth')
+    rho_2["depth"] = drho_dz.depth
+    n2 = g/rho_2*drho_dz
+    n2["depth"] = [(a+b)/2 for a,b in zip(depth, depth[1:])]
+    n2 = n2.rename({"depth":"avg_depth"})
+    return n2 
+
+def Average_layer_temp(Temp, depth_ref, layer='top', depth=None):
+    '''
+    Perform the layer average temperature based on the thermocline depth 
+
+    Parameters
+    -----------
+    Temp: array_like, xarray: 
+        A dataset containing the temperature. Must be of the same dimensions than the thermocline depth.
+    depth_ref: array_like:
+        reference depth in which the averaged temperature above or under is calculated.
+    layer: str, default: 'top'
+        layer='top' will do the average temperature above the depth_ref
+        layer='bot' will do the average temperature under the depth_ref
+    depth: array_like
+        a numeric vector corresponding to the depth (in m) of the Temp measurements. Necessary if not using xarray
+
+    Returns
+    -----------
+    mean_temp: array_like
+        dataset with the mean layer temperature
+
+    Examples
+    -----------
+    >>> wtr = np.array([22.51, 22.42, 22.4, 22.4, 22.4, 22.36, 22.3, 22.21, 22.11, 21.23, 16.42,15.15, 14.24, 13.35, 10.94, 10.43, 10.36, 9.94, 9.45, 9.1, 8.91, 8.58, 8.43])
+    ... depth = np.array([0, 0.5, 1, 1.5, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20])
+    ... depth_ref = 9 
+    ... lw.Average_layer_temp(wtr, depth, depth_ref, top=True)
+    ... 21.70
+    ... lw.Average_layer_temp(wtr, depth, depth_ref, top=True)
+    ... 10.33
+    '''
+    Temp, depth = to_xarray(Temp,depth)
+
+    if layer=='top':
+        mask = (Temp.depth<depth_ref)
+    elif layer=='bot':
+        mask = (Temp.depth>depth_ref)
+    else:
+        warnings.warnings("Temperature average of the whole water column")
+        mean_temp = Temp.mean(dim="depth")
+        return mean_temp
+    masked_temp = Temp.where(mask)
+    mean_temp = masked_temp.mean(dim="depth")
+    return mean_temp
+
+def Surface_Buoyancy_Flux(swT,sHFturb0,rho0):
+    '''
+    Calculate the surface buyoancy flux
+
+    Parameters
+    -------------
+    swT: array_like, unit: °C
+        Surface water temperature in °C 
+    sHFturb0: array_like, unit: W/m2
+        Net Surface Heat Flux - Absorbed Shortwave Radiation 
+    rho0: array_like
+        Lake Surface Density kg/m3
+
+    returns
+    -------------
+    JB0: array_like
+        Surface buoyancy flux W/m2
+    '''
+    JB0 = sw.alpha(0.2,swT,0)*9.81/sw.cp(0.2,swT,0)*sHFturb0/rho0
+    return JB0
+
+def Monin_Obukhov(ustar, JB0):
+    '''
+    Calculate Monin-Obhukov length
+
+    Parameters
+    -------------
+    ustar: array_like, unit: m/s
+        Shear Velocity on water
+    JB0: array_like, unit: W/m2
+        Surface buoyancy flux 
+    '''
+    LMO = ustar**3/0.4/JB0
+    return LMO
```

### Comparing `pylake-0.1.6/pylake/pylake_metabolizer.py` & `pylake-0.1.7/pylake/pylake_metabolizer.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,652 +1,652 @@
-from logging import warning
-from pickle import TRUE
-import pandas as pd 
-import xarray as xr
-import numpy as np 
-from .functions import *
-from .functions_meta import *
-import warnings
-
-def metab_bookkeep(do_obs, do_sat, k_gas, z_mix, irr, Datetime):
-    #May have a problem if multiple year data
-    Datetime, do_obs, do_sat, k_gas, z_mix, irr = list(map(np.asanyarray, (Datetime, do_obs, do_sat, k_gas, z_mix, irr)))
-    loc = locals()
-    dataset = xarray_from_input(metab_bookkeep, loc, coords = {'time':Datetime})
-    if type(dataset["time"][0].values)==np.ndarray:
-        dataset["time"] = pd.to_datetime(dataset["time"], unit='s')
-    ds_grouped = dataset.groupby("time.dayofyear")
-    R = []
-    NEP = []
-    GPP = []
-    DOY = []
-    TIME=[]
-    for group in list(ds_grouped):
-        ds = group[1]
-        doy = group[0]
-        TIME = np.append(TIME, ds["time"][0].values.astype(str)[:10])
-        DOY=np.append(DOY,doy)
-        
-        n = xr.ones_like(ds["do_sat"]).count()
-        
-        dayI = (ds["irr"]>0)
-        nightI = (ds["irr"]<=0)
-
-        delta_do = ds["do_obs"].diff('time')
-
-        gas_flux = (ds["do_sat"] - ds["do_obs"]) * (ds["k_gas"]/n) / ds["z_mix"]
-
-        delta_do_metab = delta_do - gas_flux
-        #gas flux is negative because DO is oversaturated. 
-        #Does this equation assumes under saturation ??
-        #Goal is to remove gas flux
-        #Here if gas flux < 0 means adding something to delta_do
-        
-        nep_day = delta_do_metab.where(dayI)
-        nep_night = delta_do_metab.where(nightI)
-        
-        R = np.append(R, nep_night.mean('time')*n) # should be negative
-        NEP = np.append(NEP, delta_do_metab.mean('time')*n) # can be positive or negative
-        GPP = np.append(GPP, nep_day.mean('time') * dayI.sum('time') - nep_night.mean('time') * dayI.sum('time')) # should be positive
-        if nep_night.mean('time')*n>0:
-            print(1)
-    metab=({"time": TIME, "GPP":GPP, "R":R, "NEP":NEP})
-    return metab
-
-
-def metab_ols(wtr, do_obs, do_sat, k_gas, z_mix, irr, Datetime):
-    from sklearn.linear_model import LinearRegression
-    #Format and get rid of NaNs
-    Datetime, do_obs, do_sat, k_gas, z_mix, irr = list(map(np.asanyarray, (Datetime, do_obs, do_sat, k_gas, z_mix, irr)))
-    mask_nan = ~np.isnan(wtr)&~np.isnan(do_obs)&~np.isnan(do_sat)&~np.isnan(k_gas)&~np.isnan(z_mix)&~np.isnan(irr)
-    do_obs, do_sat, k_gas, z_mix, irr, wtr = do_obs[mask_nan], do_sat[mask_nan], k_gas[mask_nan], z_mix[mask_nan], irr[mask_nan], wtr[mask_nan]
-
-    loc = locals()
-    dataset = xarray_from_input(metab_ols, loc, coords = {'time':Datetime})
-    ds_grouped = dataset.groupby("time.dayofyear")
-    R = []
-    NEP = []
-    GPP = []
-    DOY = []
-    for group in list(ds_grouped):
-        ds = group[1]
-        doy = group[0]
-        n = xr.ones_like(ds["do_sat"]).count()
-
-        do_diff = ds["do_obs"].diff('time')
-        inst_flux = (ds["k_gas"]/n) * (ds["do_sat"] - ds["do_obs"])  # positive is into the lake
-
-        # flux = (inst_flux[1:(n.obs-1)] + inst_flux[-1])/2
-        flux = inst_flux
-
-        noflux_do_diff = do_diff - flux/ds["z_mix"]
-
-        lntemp = np.log(ds["wtr"])
-
-        regr = LinearRegression()
-        df = pd.DataFrame({"noflux_do_diff":noflux_do_diff, "irr": ds["irr"][:-1], "lntemp":lntemp[:-1]})
-        X= df[['irr', 'lntemp']]
-        y = df["noflux_do_diff"] 
-        reg = regr.fit(X,y)
-        iota = reg.coef_[0]
-        rho = reg.coef_[1]
-
-        gpp = np.nanmean(iota*ds["irr"][:-1])*n
-        resp = np.nanmean(rho*lntemp[:-1])*n
-        nep = gpp + resp
-
-        GPP = np.append(GPP,gpp)
-        R = np.append(R,resp)
-        NEP = np.append(NEP, nep)
-        DOY=np.append(DOY,doy)
-
-    results = {"DOY": DOY, "GPP":GPP, "R":R, "NEP":NEP}
-    return(results)
-'''
-def metab_mle(do_obs, do_sat, k_gas, z_mix, irr, wtr, freq, error_type="OE"):
-    freq, do_obs, do_sat, k_gas, z_mix, irr = list(map(np.asanyarray, (freq, do_obs, do_sat, k_gas, z_mix, irr)))
-    mask_nan = ~np.isnan(wtr)&~np.isnan(do_obs)&~np.isnan(do_sat)&~np.isnan(k_gas)&~np.isnan(z_mix)&~np.isnan(irr)
-    do_obs, do_sat, k_gas, z_mix, irr, wtr = do_obs[mask_nan], do_sat[mask_nan], k_gas[mask_nan], z_mix[mask_nan], irr[mask_nan], wtr[mask_nan]
-    nobs = len(do_obs)
-
-    Q0 = ((np.diff(range(do_obs)) - np.mean(do_obs))^2 / len(do_obs))
-
-    guesses = np.array([1E-4, 1E-4, np.log(Q0)])
-
-    #We have a different number of fitted parameters depending on error type of the model
-    if(error_type=='OE'):
-        guesses = c(guesses, do_obs[1]) 
-
-        fit = optim(guesses, fn=mleNllOE, do_obs=do_obs, do_sat=do_sat, k_gas=(k_gas/freq), z_mix=z_mix, irr=irr, wtr=wtr)
-        
-        pars0 = fit$par
-        pars = c("gppCoeff"=pars0[1], "rCoeff"=pars0[2], "Q"=exp(pars0[3]), "nll"=fit$value, "doInit"=pars0[4])
-        
-    else if(error_type=='PE'):
-        guesses = c(guesses) 
-        
-        fit = optim(guesses, fn=mleNllPE, do_obs=do_obs, do_sat=do_sat, k_gas=(k_gas/freq), z_mix=z_mix, irr=irr, wtr=wtr)
-        
-        pars0 = fit$par
-        pars = c("gppCoeff"=pars0[1], "rCoeff"=pars0[2], "Q"=exp(pars0[3]), "nll"=fit$value)
-        
-    else:
-        stop("error.type must be either 'OE' or 'PE', Observation Error or Process Error respectively.")
-
-    # ====================================
-    # = Use fits to calculate metabolism =
-    # ====================================
-    GPP = mean(pars[1]*irr, na.rm=TRUE) * freq
-    R = mean(pars[2]*np.log(wtr), na.rm=TRUE) * freq
-
-    return(list("params"=pars, "metab"=c("GPP"=GPP,"R"=R,"NEP"=GPP+R)))
-    '''
-def o2_at_sat(temp, baro=None, altitude=0, salinity=.2, model='garcia-benson'):
-    #temp, baro, altitude, salinity = list(map(np.asanyarray, (temp, baro, altitude, salinity)))
-    # Conversion from mL/L (the usual output of the garcia, weiss, etc. equations)
-    # to mg/L per USGS memo 2011.03
-    mgL_mlL = 1.42905
-
-    # Correction for air pressure; incorportes effects of altitude & vapor pressure of water
-    mmHg_mb = 0.750061683 # conversion from mm Hg to millibars
-    if baro is None:
-        mmHg_inHg = 25.3970886 # conversion from inches Hg to mm Hg
-        standard_pressure_sea_level = 29.92126 # Pb, inches Hg
-        standard_temperature_sea_level = 15 + 273.15 # Tb, 15 C = 288.15 K
-        gravitational_acceleration = 9.80665 # g0, m/s**2
-        air_molar_mass = 0.0289644 # M, molar mass of Earth's air (kg/mol)
-        universal_gas_constant = 8.31447 #8.31432 # R*, N*m/(mol*K)
-
-        # estimate pressure by the barometric formula
-        baro = (1/mmHg_mb) * mmHg_inHg * standard_pressure_sea_level * \
-            np.exp( (-gravitational_acceleration * air_molar_mass * altitude) / (universal_gas_constant * standard_temperature_sea_level) )
-        baro = np.ones(len(temp))*baro
-    
-    # pressure correction per USGS memos 81.11 and 81.15. calculate u by Antoine equation.
-    u = 10 ** (8.10765 - 1750.286 / (235 + temp)) # u is vapor pressure of water; water temp is used as an approximation for water & air temp at the air-water boundary
-    press_corr = (baro*mmHg_mb - u) / (760 - u) # pressure correction is ratio of current to standard pressure after correcting for vapor pressure of water. 0.750061683 mmHg/mb
-
-    # Estimate O2 at saturation in mL/L by several models
-    if(model == 'garcia'):
-
-        Ts = np.log((298.15 - temp)/(273.15 + temp))
-
-        lnC = 2.00856 + 3.22400 *Ts + 3.99063*Ts**2 + 4.80299*Ts**3 + 9.78188e-1*Ts**4 + \
-        1.71069*Ts**5 - salinity*(6.24097e-3 + 6.93498e-3*Ts + 6.90358e-3*Ts**2 + 4.29155e-3*Ts**3) - 3.1168e-7*salinity**2
-
-        o2_sat = np.exp(lnC)
-
-    elif((model) == 'garcia-benson'):
-        
-        Ts = np.log((298.15 - temp)/(273.15 + temp))
-        
-        lnC = 2.00907 + 3.22014*Ts + 4.05010*Ts**2 + 4.94457*Ts**3 + -2.56847e-1*Ts**4 + \
-        3.88767*Ts**5 - salinity*(6.24523e-3 + 7.37614e-3*Ts + 1.03410e-2*Ts**2 + 8.17083e-3*Ts**3) - 4.88682e-7*salinity**2
-        
-        o2_sat = np.exp(lnC)
-        
-    elif((model) == 'weiss'):
-        tempk = temp + 273.15
-
-        lnC = -173.4292 + 249.6339 * (100 / tempk) + 143.3483 * \
-        np.log(tempk / 100) - 21.8492 * (tempk / 100) + \
-        salinity * (-0.033096 + 0.014259 * (tempk / 100) - 0.0017000 * (tempk / 100)**2)
-            
-        o2_sat = np.exp(lnC)
-
-
-    o2_sat = o2_sat * mgL_mlL * press_corr
-
-    return(o2_sat)
-
-def k_cole(wnd):
-    k600 = 2.07 + (0.215*(wnd**(1.7)))
-    k600 = k600*24/100 #units in m d-1
-    return k600
-
-def k_crusius(wnd, method='power'):
-    # -- References 
-    # CRUSIUS, JOHN, AND RIK WANNINKHOF. 2003
-    # Gas transfer velocities measured at low wind speed over a lake.
-    # Limnology and Oceanography. 48(3): 1010:1017.
-    U10 = wnd
-    if method=='constant':
-        mask = U10<3.7
-        k600 = 0.72*U10
-        k600[~mask] = 14*U10-17.9
-    elif method=='bilinear':
-        mask = U10<3.7
-        k600 = 0.72*U10
-        k600[~mask] = 4.33*U10-13.3
-    elif method =='power':
-        k600 = 0.228*U10**2.2+0.168 # units in cm h-1
-
-    k600 = k600*24/100
-    return k600
-
-def k_read(wnd_z, Qsen, Qlat, Cd, Kd, lat, A0, air_press, dateTime, Ts, hML, airT, wnd, RH, sw, lwnet, lwnet_mode=1, s=0.2):
-    #'@param wnd Numeric value of wind speed, (Units:m/s)
-    #'@param method Only for \link{k.crusius.base}. String of valid method . Either "constant", "bilinear", or "power"
-    #'@param wnd_z Height of wind measurement, (Units: m)
-    #'@param Kd Light attenuation coefficient (Units: m**-1)
-    #'@param lat Latitude, degrees north
-    #'@param A0 Lake area, m**2
-    #'@param air_press Atmospheric pressure, (Units: millibar)
-    #'@param dateTime datetime (Y-\%m-\%d \%H:\%M), (Format: \code{\link{POSIXct}})
-    #'@param Ts Numeric vector of surface water temperature, (Units(deg C)
-    #'@param hML Numeric vector of actively mixed layer depths. Must be the same length as the Ts parameter
-    #'@param airT Numeric value of air temperature, Units(deg C)
-    #'@param RH Numeric value of relative humidity, \%
-    #'@param sw Numeric value of short wave radiation, W m**-2
-    #'@param lwnet Numeric value net long wave radiation, W m**-2, 
-    # define constants used in function
-    wnd, Qsen, Qlat, Cd, Kd, air_press, dateTime, Ts, hML, airT, wnd, RH, sw, lwnet = list(map(np.asanyarray, (wnd, \
-        Qsen, Qlat, Cd, Kd, air_press, dateTime, Ts, hML, airT, wnd, RH, sw, lwnet)))
-    #if no net, convert it to net
-    if not lwnet_mode:
-        Tk = Ts+Kelvin # water temperature in Kelvin
-        LWo = S_B*emiss*Tk**4 # long wave out
-        lwnet = lwnet-LWo
-
-    Kelvin = 273.15 # temp mod for deg K   
-    emiss = 0.972 # emissivity;
-    S_B = 5.67E-8 # Stefan-Boltzman constant (?K is used)
-    vonK = 0.41 # von Karman  constant
-    dT = 0.5   # change in temp for mixed layer depth
-    C1 = 114.278 # from Soloviev et al. 2007
-    nu = 0.29 # proportionality constant from Zappa et al. 2007, lower bounds
-    KeCrit = 0.18     # constant for wave age = 20 (Soloviev et al. 2007)
-    albedo_SW = 0.07
-    swRat = 0.46 # percentage of SW radiation that penetrates the water column
-    g = 9.81 # gravity
-    C_w = 4186 # J kg-1 ?C-1 (Lenters et al. 2005)
-    mnWnd = 0.2 # minimum wind speed
-
-    # impose limit on wind speed
-    rpcI = wnd < mnWnd
-    wnd[rpcI] = mnWnd
-
-    # calculate sensible and latent heat fluxes
-    C_D = Cd # drag coefficient for momentum
-    E = Qlat # latent heat flux
-    H = Qsen # sensible heat flux
-
-    # calculate total heat flux
-    dUdt = sw*0.93 - E - H + lwnet
-    Qo = sw*(1-albedo_SW)*swRat
-
-    # calculate water density
-    rho_w = dens0(t=Ts, s=0.2)
-
-    # calculate u*
-    if (wnd_z != 10):
-        e1 = np.sqrt(C_D)
-        wnd = wnd/(1-e1/vonK*np.log(10/wnd_z))
-        
-    rhoAir = 1.2 #  air density
-    tau = C_D*wnd**2*rhoAir
-    uSt = np.sqrt(tau/rho_w)
-
-    # calculate the effective heat flux
-    q1 = 2-2*np.exp(hML*-Kd)
-    q2 = hML*Kd
-    q3 = np.exp(hML*-Kd)
-    H_star = dUdt-Qo*(q1/q2-q3) # Kim 1976
-
-    # calculate the thermal expansion coefficient 
-    tExp = thermalExpFromTemp(Ts)
-
-    # calculate buoyancy flux and w*
-    B1 = H_star*tExp*g
-    B2 = rho_w*C_w
-    Bflx = B1/B2
-    ltI = Bflx>0
-    if type(B1)==np.float64:
-        B1 = np.array(B1)
-    B1[ltI] = 0
-    divi = 1/3
-    w1 = -B1*hML
-    wSt = w1**divi
-
-    # calculate kinematic viscosiy
-    kinV = getKinematicVis(Ts)
-
-    KeDe = (kinV*g)
-    KeNm = uSt**3
-    Ke = KeNm/KeDe
-    tau = tau    # estimate of total tau (includes wave stress)
-    euPw = (1+Ke/KeCrit)  # tau_shear = tau/(1+Ke/Kecr)
-    tau_t = tau/euPw      # tau_shear, Soloviev
-    uTanS = tau_t/rho_w   
-    uTanS = uTanS**0.5
-
-    # calculate viscous sublayer
-    Sv = C1*kinV/uTanS
-    eu_N = uTanS**3      # e_u(0) = (tau_t/rho)**1.5/(vonK*Sv)
-    eu_D = vonK*Sv       # denominator
-    eu_0 = eu_N/eu_D    # in m2/s3
-    ew_0 = -1.0*B1       # buoyancy flux, but only when outward
-    e_0 = ew_0+eu_0     # e(0) from Soloviev (w/o wave effects)
-    K1 = e_0*kinV       # in units of m4/s4, want cm4/hr4
-    K2 = ew_0*kinV      # convective component (m4/s4)
-    K1 = K1*100**4*3600**4 # now in cm4/hr4  (Total)
-    K2 = K2*100**4*3600**4 # now in cm4/hr4  (Convective)
-    K600 = nu*600**(-0.5)*K1**(1/4)   # in cm/hr (Total)
-
-    #k600 = np.numeric(K600)
-    k600 = K600*24/100 #now in units in m d-1
-    return(k600)
-
-def k_heiskanen(wnd_z, Cd, Qlat, Qsen, Kd, air_press, dateTime, Ts, hML, airT, wnd, RH, sw, lwnet):
-
-    #Constants
-    S_B = 5.67E-8 # Stefan-Boltzman constant (K is used)
-    emiss = 0.972 # emissivity
-    Kelvin = 273.15 #conversion from C to Kelvin
-    albedo_SW = 0.07
-    vonK = 0.41 #von Karman constant
-    swRat = 0.46 # percentage of SW radiation that penetrates the water column
-    mnWnd = 0.2 # minimum wind speed
-    g = 9.81 # gravity
-    C_w = 4186 # J kg-1 ?C-1 (Lenters et al. 2005)
-
-    # impose limit on wind speed
-    rpcI = wnd < mnWnd
-    if type(wnd)==int:
-        wnd=np.array(wnd)
-    wnd[rpcI] = mnWnd
-
-
-    # calculate sensible and latent heat fluxes
-    #mm = calc.zeng(dateTime,Ts,airT,wnd,RH,air_press,wnd_z)
-    C_D = Cd # drag coefficient for momentum
-    E = Qlat # latent heat flux
-    H = Qsen # sensible heat flux
-
-    # calculate total heat flux
-    dUdt = sw*0.93 - E - H + lwnet
-    Qo = sw*(1-albedo_SW)*swRat
-
-    # calculate water density
-    rho_w = dens0(t=Ts, s=0.2)
-
-    # calculate u*
-    if (wnd_z != 10):
-        e1 = np.sqrt(C_D)
-        u10 = wnd/(1-e1/vonK*np.log(10/wnd_z))
-    else:
-        u10 = wnd
-
-
-    rhoAir = 1.2 #  air density
-    vonK = 0.41 # von Karman  constant
-    tau = C_D*u10**2*rhoAir
-    uSt = np.sqrt(tau/rho_w)
-
-    # calculate the effective heat flux
-    q1 = 2-2*np.exp(hML*-Kd)
-    q2 = hML*Kd
-    q3 = np.exp(hML*-Kd)
-    H_star = dUdt-Qo*(q1/q2-q3) # Kim 1976
-
-    # calculate the thermal expansion coefficient 
-    tExp = thermalExpFromTemp(Ts)
-
-    B1 = H_star*tExp*g #Imberger 1985: Effective heat flux * thermal expansion of water * gravity
-    B2 = rho_w*C_w # mean density of the water column * specific heat of water at constant pressure
-    Bflx = B1/B2
-
-    if Bflx<0:
-        wstar = (-Bflx*hML)**(1/3)#penetrative convective velocity Heiskanen 2014 (Imberger 1985)
-    else:
-        wstar = 0
-    Hk   = np.sqrt((0.00015*u10)**2 + (0.07*wstar)**2) 
-    Hk   = Hk*100*3600 # Heiskanen's K in cm/hr
-    Hk600 = Hk*600**(-0.5)
-    k600 = Hk600*24/100 #units in m d-1
-    return(k600)
-
-
-def k_macIntyre(wnd_z, Cd, Qlat, Qsen, Kd, air_press, dateTime, Ts, hML, airT, wnd, RH, sw, lwnet,
-                                params=np.array([1.2,0.4872,1.4784])):
-
-    #Constants
-    S_B = 5.67E-8 # Stefan-Boltzman constant (K is used)
-    emiss = 0.972 # emissivity;
-    Kelvin = 273.15 #conversion from C to Kelvin
-    albedo_SW = 0.07
-    vonK = 0.41 #von Karman constant
-    swRat = 0.46 # percentage of SW radiation that penetrates the water column
-    mnWnd = 0.2 # minimum wind speed
-    g = 9.81 # gravity
-    C_w = 4186 # J kg-1 ?C-1 (Lenters et al. 2005)
-
-    # impose limit on wind speed
-    rpcI = wnd < mnWnd
-    if type(wnd)==int:
-        wnd=np.array(wnd)
-    wnd[rpcI] = mnWnd
-
-
-    # calculate sensible and latent heat fluxes
-    C_D = Cd # drag coefficient for momentum
-    E = Qlat # latent heat flux
-    H = Qsen # sensible heat flux
-
-    # calculate total heat flux
-    dUdt = sw*0.93 - E - H + lwnet
-    Qo = sw*(1-albedo_SW)*swRat
-
-    # calculate water density
-    rho_w = dens0(t=Ts, s=0.2)
-
-    # calculate u*
-    if (wnd_z != 10):
-        e1 = np.sqrt(C_D)
-        u10 = wnd/(1-e1/vonK*np.log(10/wnd_z))
-    else:
-        u10 = wnd
-    
-
-    rhoAir = 1.2 #  air density
-    vonK = 0.41 # von Karman  constant
-    tau = C_D*u10**2*rhoAir
-    uSt = np.sqrt(tau/rho_w)
-
-    # calculate the effective heat flux
-    q1 = 2-2*np.exp(hML*-Kd)
-    q2 = hML*Kd
-    q3 = np.exp(hML*-Kd)
-    H_star = dUdt-Qo*(q1/q2-q3) # Kim 1976
-
-
-    # calculate the thermal expansion coefficient
-    tExp = thermalExpFromTemp(Ts)
-
-    B1 = H_star*tExp*g
-    B2 = rho_w*C_w
-    Bflx = B1/B2
-
-    # calculate kinematic viscosiy
-    kinV = getKinematicVis(Ts)
-    KeNm = uSt**3
-
-    #SmE   = 0.84*(-0.58*Bflx+1.76*KeNm/(vonK*hML))
-    SmE = params[0]*-Bflx+params[1]*KeNm/(vonK*hML) #change to two coefficients
-    if type(SmE)==np.float64:
-        SmE=np.array(SmE)
-    SmE[SmE<0] = 0    # set negative to 0
-    Sk   = SmE*kinV
-    Sk   = Sk*100**4*3600**4 # Sally's K now in cm4/h4
-    Sk600 = params[2]*600**(-0.5)*Sk**(1/4) # in cm/hr (Total)
-
-    k600 = Sk600 # why is this not already numeric?
-    k600 = k600*24/100 #units in m d-1
-    return k600
-
-def k_read_soloviev(wnd_z, Cd, Qlat, Qsen, Kd, lat, A0, air_press, dateTime, Ts, hML, airT, wnd, RH, sw, lwnet):
-    
-    wnd_z, Cd, Qlat, Qsen, Kd, lat, A0, air_press, dateTime, Ts, hML, airT, wnd, RH, sw, lwnet = list(map(np.asanyarray, (wnd_z,\
-         Cd, Qlat, Qsen, Kd, lat, A0, air_press, dateTime, Ts, hML, airT, wnd, RH, sw, lwnet)))
-    # define constants used in function
-    Kelvin = 273.15 # temp mod for deg K
-    emiss = 0.972 # emissivity;
-    S_B = 5.67E-8 # Stefan-Boltzman constant (?K is used)
-    vonK = 0.41 # von Karman  constant
-    dT = 0.5   # change in temp for mixed layer depth
-    C1 = 114.278 # from Soloviev et al. 2007
-    nu = 0.29 # proportionality constant from Zappa et al. 2007, lower bounds
-    KeCrit = 0.18     # constant for wave age = 20 (Soloviev et al. 2007)
-    albedo_SW = 0.07
-    swRat = 0.46 # percentage of SW radiation that penetrates the water column
-    g = 9.81 # gravity
-    C_w = 4186 # J kg-1 ?C-1 (Lenters et al. 2005)
-    mnWnd = 0.2 # minimum wind speed
-
-    # impose limit on wind speed
-    rpcI = wnd < mnWnd
-    wnd[rpcI] = mnWnd
-
-    # calculate sensible and latent heat fluxes
-    C_D = Cd # drag coefficient for momentum
-    E = Qlat # latent heat flux
-    H = Qsen # sensible heat flux
-
-    # calculate total heat flux
-    dUdt = sw*0.93 - E - H + lwnet
-    Qo = sw*(1-albedo_SW)*swRat #PAR
-
-    # calculate the effective heat flux
-    q1 = 2-2*np.exp(hML*-Kd)
-    q2 = hML*Kd
-    q3 = np.exp(hML*-Kd)
-    H_star = dUdt-Qo*(q1/q2-q3) #Effective surface heat flux Kim 1976
-
-    # calculate water density
-    rho_w = dens0(t=Ts, s=0.2)
-
-    # calculate u*
-    if (wnd_z != 10):
-        e1 = np.sqrt(C_D)
-        wnd = wnd/(1-e1/vonK*np.log(10/wnd_z))
-    
-    rhoAir = 1.2 #  air density
-    tau = C_D*wnd**2*rhoAir
-    uSt = np.sqrt(tau/rho_w)
-    uSta = np.sqrt(tau/rhoAir)  #friction velocity in air
-
-    # calculate the thermal expansion coefficient
-    tExp = thermalExpFromTemp(Ts)
-
-    # calculate buoyancy flux and w*
-    B1 = H_star*tExp*g #Hstar * coefficient of thermal expansion * gravity
-    B2 = rho_w*C_w
-    Bflx = B1/B2
-    
-    if type(Bflx)==np.float64:
-        Bflx = np.array(Bflx)
-    Bflx[Bflx>0] = 0
-
-    wSt = (-Bflx*hML)**1/3
-
-    # calculate kinematic viscosiy
-    kinV = getKinematicVis(Ts)
-    kinVa = getKinematicVis(airT)
-
-    KeDe = (kinV*g)
-    KeNm = uSt**3
-    Ke = KeNm/KeDe
-    tau = tau    # estimate of total tau (includes wave stress)
-    euPw = (1+Ke/KeCrit)  # tau_shear = tau/(1+Ke/Kecr) Ke is the Keulegan number
-    # Could calculate KeCrit (critical Keulegan number) from wave age
-    #KeCrit = (kinVa/kinV)*((rhoAir/rho_w)**1.5)*(Rbcr/Aw) # Eq1.16-Soloviev et al(2007)
-
-    tau_t = tau/euPw      # tau_t = tangential wind stress, tau = total wind stress
-    uTanS = tau_t/rho_w
-    uTanS = uTanS**0.5
-
-    # calculate viscous sublayer
-    Sv = C1*kinV/uTanS  # effective thickness of the aqueous viscous sublayer
-    eu_N = uTanS**3      # e_u(0) = (tau_t/rho)**1.5/(vonK*Sv)
-    eu_D = vonK*Sv      # denominator
-    eu_0 = eu_N/eu_D    # in m2/s3
-    ec_0 = -1.0*Bflx       # buoyancy flux, but only when outward
-
-    #ewave_0 turbulence due to wave breaking
-    A0 = A0/1e6 # convert surface area to km
-    Fetch = 2*np.sqrt(A0/np.pi) # fetch in km (assuming a conical lake)
-    Hs = 0.0163*(Fetch**0.5)*wnd # significant wave height - Woolf (2005)
-    Aw = (1/(2*np.pi))*(( (g*Hs*rhoAir)/(0.062*rho_w*
-            uSt**2))**(2/3)) # wave age - eqn 1.11 Soloviev et al. (2007)
-
-    W = 3.8e-6*wnd**3.4 # simplified whitecap fraction (Fariall et al. 2000)
-
-
-    Ap = 2.45*W*((1/(W**0.25))-1)
-    alphaW = 100 # p. 185 - Soloviev et al. (2007)
-    B = 16.6 # p. 185 - Soloviev et al. (2007)
-    Sq = 0.2 # p. 185 - Soloviev et al. (2007)
-    cT = 0.6 # p. 188 - Soloviev et al. (2007)
-    ewave_0 = ((Ap**4)*alphaW)*((3/(B*Sq))**0.5) * \
-                    (((Ke/KeCrit)**1.5)/((1+Ke/KeCrit)**1.5))* \
-                    (uSt*g*kinV)/(0.062*vonK*cT*((2*np.pi*Aw)**1.5)) * \
-                    (rhoAir/rho_w)
-
-    #------------------------------------
-    e_0 = ec_0+eu_0+ewave_0    # e(0) from Soloviev (w/o wave effects)
-    Kc = ec_0*kinV*100**4*3600**4      # convective component now in cm4/hr4  (Total)
-    Ku = eu_0*kinV*100**4*3600**4 # shear component now in cm4/hr4  (Total)
-    Kwave = ewave_0*kinV*100**4*3600**4 # wave component now in cm4/hr4  (Total)
-    Kall = e_0*kinV*100**4*3600**4       # turbulent kinetic energy now in cm4/hr4  (Total)
-
-    #Schmidt number could be calculated as temperature dependent
-    #Sc = 1568+(-86.04*Ts)+(2.142*Ts**2)+(-0.0216*Ts**3)
-    k600org = nu*600**(-0.5)*(Kc+Ku)**(1/4)   # in cm/hr (Total)
-    k600org = k600org*24/100 #now in units in m d-1
-
-    k600 = nu*600**(-0.5)*Kall**(1/4)   # in cm/hr (Total)
-    k600 = k600*24/100 #now in units in m d-1
-
-    # ---Breaking Wave Component, Author: R I Woolway, 2014-11-13 ---
-    # bubble mediated component - Woolf 1997
-    kbi = W*2450
-    beta_0 = 2.71*1e-2 # Ostwald gas solubility (Emerson and Hedges, 2008)
-    Sc = 1568+(-86.04*Ts)+(2.142*Ts**2)+(-0.0216*Ts**3) # Schmidt number
-    kbiii = (1+(1/(14*beta_0*Sc**(-0.5))**(1/1.2)))**1.2
-    kb = kbi/((beta_0*kbiii))
-    kb = kb*24/100 #units in m d-1
-    #----------------------------------------------------------------
-
-    k600b = k600+kb
-    #allks = pd.DataFrame(data =(Ku,Kc,Kwave,kb,k600org,k600,k600b), columns= ["shear","convective","wave","bubble","k600org","k600",'k600b'])
-    return k600b
-
-def k_vachon(wnd, A0, params=np.array([2.51,1.48,0.39])):
-    U10 = wnd  #This function uses just the wind speed it is supplied
-    k600 = params[0] + params[1]*U10 + params[2]*U10*np.log10(A0/1000000) # units in cm h-1
-    k600 = k600*24/100 #units in m d-1
-    return(k600)
-    
-
-def k600_2_kGAS(k600,temperature,gas="O2"):
-    #'@title Returns the gas exchange velocity for gas of interest w/ no unit conversions
-    #'@description 
-    #'Returns the gas exchange velocity for gas of interest w/ no unit conversions
-    #'@usage
-    #'k600.2.kGAS.base(k600,temperature,gas="O2")
-    #'
-    #'k600.2.kGAS(ts.data, gas="O2")
-    #'
-    #'@param ts.data Object of class data.frame with named columns datetime and k600 and wtr (water temp in deg C). Other columns are ignored
-    #'@param k600 k600 as vector array of numbers or single number
-    #'@param temperature Water temperature (deg C) as vector array of numbers or single number
-    #'@param gas gas for conversion, as string (e.g., 'CO2' or 'O2')
-    #'@return Numeric value of gas exchange velocity for gas
-    #'@author Jordan S. Read
-    #'@seealso \link{k.read} and \link{k.read.base} for functions that calculate k600 estimates
-    n	=	0.5
-    schmidt	=	getSchmidt(temperature,gas)
-    Sc600	=	schmidt/600
-
-    kGAS	=	k600*(Sc600**-n)
-    return(kGAS)
-
+from logging import warning
+from pickle import TRUE
+import pandas as pd 
+import xarray as xr
+import numpy as np 
+from .functions import *
+from .functions_meta import *
+import warnings
+
+def metab_bookkeep(do_obs, do_sat, k_gas, z_mix, irr, Datetime):
+    #May have a problem if multiple year data
+    Datetime, do_obs, do_sat, k_gas, z_mix, irr = list(map(np.asanyarray, (Datetime, do_obs, do_sat, k_gas, z_mix, irr)))
+    loc = locals()
+    dataset = xarray_from_input(metab_bookkeep, loc, coords = {'time':Datetime})
+    if type(dataset["time"][0].values)==np.ndarray:
+        dataset["time"] = pd.to_datetime(dataset["time"], unit='s')
+    ds_grouped = dataset.groupby("time.dayofyear")
+    R = []
+    NEP = []
+    GPP = []
+    DOY = []
+    TIME=[]
+    for group in list(ds_grouped):
+        ds = group[1]
+        doy = group[0]
+        TIME = np.append(TIME, ds["time"][0].values.astype(str)[:10])
+        DOY=np.append(DOY,doy)
+        
+        n = xr.ones_like(ds["do_sat"]).count()
+        
+        dayI = (ds["irr"]>0)
+        nightI = (ds["irr"]<=0)
+
+        delta_do = ds["do_obs"].diff('time')
+
+        gas_flux = (ds["do_sat"] - ds["do_obs"]) * (ds["k_gas"]/n) / ds["z_mix"]
+
+        delta_do_metab = delta_do - gas_flux
+        #gas flux is negative because DO is oversaturated. 
+        #Does this equation assumes under saturation ??
+        #Goal is to remove gas flux
+        #Here if gas flux < 0 means adding something to delta_do
+        
+        nep_day = delta_do_metab.where(dayI)
+        nep_night = delta_do_metab.where(nightI)
+        
+        R = np.append(R, nep_night.mean('time')*n) # should be negative
+        NEP = np.append(NEP, delta_do_metab.mean('time')*n) # can be positive or negative
+        GPP = np.append(GPP, nep_day.mean('time') * dayI.sum('time') - nep_night.mean('time') * dayI.sum('time')) # should be positive
+        if nep_night.mean('time')*n>0:
+            print(1)
+    metab=({"time": TIME, "GPP":GPP, "R":R, "NEP":NEP})
+    return metab
+
+
+def metab_ols(wtr, do_obs, do_sat, k_gas, z_mix, irr, Datetime):
+    from sklearn.linear_model import LinearRegression
+    #Format and get rid of NaNs
+    Datetime, do_obs, do_sat, k_gas, z_mix, irr = list(map(np.asanyarray, (Datetime, do_obs, do_sat, k_gas, z_mix, irr)))
+    mask_nan = ~np.isnan(wtr)&~np.isnan(do_obs)&~np.isnan(do_sat)&~np.isnan(k_gas)&~np.isnan(z_mix)&~np.isnan(irr)
+    do_obs, do_sat, k_gas, z_mix, irr, wtr = do_obs[mask_nan], do_sat[mask_nan], k_gas[mask_nan], z_mix[mask_nan], irr[mask_nan], wtr[mask_nan]
+
+    loc = locals()
+    dataset = xarray_from_input(metab_ols, loc, coords = {'time':Datetime})
+    ds_grouped = dataset.groupby("time.dayofyear")
+    R = []
+    NEP = []
+    GPP = []
+    DOY = []
+    for group in list(ds_grouped):
+        ds = group[1]
+        doy = group[0]
+        n = xr.ones_like(ds["do_sat"]).count()
+
+        do_diff = ds["do_obs"].diff('time')
+        inst_flux = (ds["k_gas"]/n) * (ds["do_sat"] - ds["do_obs"])  # positive is into the lake
+
+        # flux = (inst_flux[1:(n.obs-1)] + inst_flux[-1])/2
+        flux = inst_flux
+
+        noflux_do_diff = do_diff - flux/ds["z_mix"]
+
+        lntemp = np.log(ds["wtr"])
+
+        regr = LinearRegression()
+        df = pd.DataFrame({"noflux_do_diff":noflux_do_diff, "irr": ds["irr"][:-1], "lntemp":lntemp[:-1]})
+        X= df[['irr', 'lntemp']]
+        y = df["noflux_do_diff"] 
+        reg = regr.fit(X,y)
+        iota = reg.coef_[0]
+        rho = reg.coef_[1]
+
+        gpp = np.nanmean(iota*ds["irr"][:-1])*n
+        resp = np.nanmean(rho*lntemp[:-1])*n
+        nep = gpp + resp
+
+        GPP = np.append(GPP,gpp)
+        R = np.append(R,resp)
+        NEP = np.append(NEP, nep)
+        DOY=np.append(DOY,doy)
+
+    results = {"DOY": DOY, "GPP":GPP, "R":R, "NEP":NEP}
+    return(results)
+'''
+def metab_mle(do_obs, do_sat, k_gas, z_mix, irr, wtr, freq, error_type="OE"):
+    freq, do_obs, do_sat, k_gas, z_mix, irr = list(map(np.asanyarray, (freq, do_obs, do_sat, k_gas, z_mix, irr)))
+    mask_nan = ~np.isnan(wtr)&~np.isnan(do_obs)&~np.isnan(do_sat)&~np.isnan(k_gas)&~np.isnan(z_mix)&~np.isnan(irr)
+    do_obs, do_sat, k_gas, z_mix, irr, wtr = do_obs[mask_nan], do_sat[mask_nan], k_gas[mask_nan], z_mix[mask_nan], irr[mask_nan], wtr[mask_nan]
+    nobs = len(do_obs)
+
+    Q0 = ((np.diff(range(do_obs)) - np.mean(do_obs))^2 / len(do_obs))
+
+    guesses = np.array([1E-4, 1E-4, np.log(Q0)])
+
+    #We have a different number of fitted parameters depending on error type of the model
+    if(error_type=='OE'):
+        guesses = c(guesses, do_obs[1]) 
+
+        fit = optim(guesses, fn=mleNllOE, do_obs=do_obs, do_sat=do_sat, k_gas=(k_gas/freq), z_mix=z_mix, irr=irr, wtr=wtr)
+        
+        pars0 = fit$par
+        pars = c("gppCoeff"=pars0[1], "rCoeff"=pars0[2], "Q"=exp(pars0[3]), "nll"=fit$value, "doInit"=pars0[4])
+        
+    else if(error_type=='PE'):
+        guesses = c(guesses) 
+        
+        fit = optim(guesses, fn=mleNllPE, do_obs=do_obs, do_sat=do_sat, k_gas=(k_gas/freq), z_mix=z_mix, irr=irr, wtr=wtr)
+        
+        pars0 = fit$par
+        pars = c("gppCoeff"=pars0[1], "rCoeff"=pars0[2], "Q"=exp(pars0[3]), "nll"=fit$value)
+        
+    else:
+        stop("error.type must be either 'OE' or 'PE', Observation Error or Process Error respectively.")
+
+    # ====================================
+    # = Use fits to calculate metabolism =
+    # ====================================
+    GPP = mean(pars[1]*irr, na.rm=TRUE) * freq
+    R = mean(pars[2]*np.log(wtr), na.rm=TRUE) * freq
+
+    return(list("params"=pars, "metab"=c("GPP"=GPP,"R"=R,"NEP"=GPP+R)))
+    '''
+def o2_at_sat(temp, baro=None, altitude=0, salinity=.2, model='garcia-benson'):
+    #temp, baro, altitude, salinity = list(map(np.asanyarray, (temp, baro, altitude, salinity)))
+    # Conversion from mL/L (the usual output of the garcia, weiss, etc. equations)
+    # to mg/L per USGS memo 2011.03
+    mgL_mlL = 1.42905
+
+    # Correction for air pressure; incorportes effects of altitude & vapor pressure of water
+    mmHg_mb = 0.750061683 # conversion from mm Hg to millibars
+    if baro is None:
+        mmHg_inHg = 25.3970886 # conversion from inches Hg to mm Hg
+        standard_pressure_sea_level = 29.92126 # Pb, inches Hg
+        standard_temperature_sea_level = 15 + 273.15 # Tb, 15 C = 288.15 K
+        gravitational_acceleration = 9.80665 # g0, m/s**2
+        air_molar_mass = 0.0289644 # M, molar mass of Earth's air (kg/mol)
+        universal_gas_constant = 8.31447 #8.31432 # R*, N*m/(mol*K)
+
+        # estimate pressure by the barometric formula
+        baro = (1/mmHg_mb) * mmHg_inHg * standard_pressure_sea_level * \
+            np.exp( (-gravitational_acceleration * air_molar_mass * altitude) / (universal_gas_constant * standard_temperature_sea_level) )
+        baro = np.ones(len(temp))*baro
+    
+    # pressure correction per USGS memos 81.11 and 81.15. calculate u by Antoine equation.
+    u = 10 ** (8.10765 - 1750.286 / (235 + temp)) # u is vapor pressure of water; water temp is used as an approximation for water & air temp at the air-water boundary
+    press_corr = (baro*mmHg_mb - u) / (760 - u) # pressure correction is ratio of current to standard pressure after correcting for vapor pressure of water. 0.750061683 mmHg/mb
+
+    # Estimate O2 at saturation in mL/L by several models
+    if(model == 'garcia'):
+
+        Ts = np.log((298.15 - temp)/(273.15 + temp))
+
+        lnC = 2.00856 + 3.22400 *Ts + 3.99063*Ts**2 + 4.80299*Ts**3 + 9.78188e-1*Ts**4 + \
+        1.71069*Ts**5 - salinity*(6.24097e-3 + 6.93498e-3*Ts + 6.90358e-3*Ts**2 + 4.29155e-3*Ts**3) - 3.1168e-7*salinity**2
+
+        o2_sat = np.exp(lnC)
+
+    elif((model) == 'garcia-benson'):
+        
+        Ts = np.log((298.15 - temp)/(273.15 + temp))
+        
+        lnC = 2.00907 + 3.22014*Ts + 4.05010*Ts**2 + 4.94457*Ts**3 + -2.56847e-1*Ts**4 + \
+        3.88767*Ts**5 - salinity*(6.24523e-3 + 7.37614e-3*Ts + 1.03410e-2*Ts**2 + 8.17083e-3*Ts**3) - 4.88682e-7*salinity**2
+        
+        o2_sat = np.exp(lnC)
+        
+    elif((model) == 'weiss'):
+        tempk = temp + 273.15
+
+        lnC = -173.4292 + 249.6339 * (100 / tempk) + 143.3483 * \
+        np.log(tempk / 100) - 21.8492 * (tempk / 100) + \
+        salinity * (-0.033096 + 0.014259 * (tempk / 100) - 0.0017000 * (tempk / 100)**2)
+            
+        o2_sat = np.exp(lnC)
+
+
+    o2_sat = o2_sat * mgL_mlL * press_corr
+
+    return(o2_sat)
+
+def k_cole(wnd):
+    k600 = 2.07 + (0.215*(wnd**(1.7)))
+    k600 = k600*24/100 #units in m d-1
+    return k600
+
+def k_crusius(wnd, method='power'):
+    # -- References 
+    # CRUSIUS, JOHN, AND RIK WANNINKHOF. 2003
+    # Gas transfer velocities measured at low wind speed over a lake.
+    # Limnology and Oceanography. 48(3): 1010:1017.
+    U10 = wnd
+    if method=='constant':
+        mask = U10<3.7
+        k600 = 0.72*U10
+        k600[~mask] = 14*U10-17.9
+    elif method=='bilinear':
+        mask = U10<3.7
+        k600 = 0.72*U10
+        k600[~mask] = 4.33*U10-13.3
+    elif method =='power':
+        k600 = 0.228*U10**2.2+0.168 # units in cm h-1
+
+    k600 = k600*24/100
+    return k600
+
+def k_read(wnd_z, Qsen, Qlat, Cd, Kd, lat, A0, air_press, dateTime, Ts, hML, airT, wnd, RH, sw, lwnet, lwnet_mode=1, s=0.2):
+    #'@param wnd Numeric value of wind speed, (Units:m/s)
+    #'@param method Only for \link{k.crusius.base}. String of valid method . Either "constant", "bilinear", or "power"
+    #'@param wnd_z Height of wind measurement, (Units: m)
+    #'@param Kd Light attenuation coefficient (Units: m**-1)
+    #'@param lat Latitude, degrees north
+    #'@param A0 Lake area, m**2
+    #'@param air_press Atmospheric pressure, (Units: millibar)
+    #'@param dateTime datetime (Y-\%m-\%d \%H:\%M), (Format: \code{\link{POSIXct}})
+    #'@param Ts Numeric vector of surface water temperature, (Units(deg C)
+    #'@param hML Numeric vector of actively mixed layer depths. Must be the same length as the Ts parameter
+    #'@param airT Numeric value of air temperature, Units(deg C)
+    #'@param RH Numeric value of relative humidity, \%
+    #'@param sw Numeric value of short wave radiation, W m**-2
+    #'@param lwnet Numeric value net long wave radiation, W m**-2, 
+    # define constants used in function
+    wnd, Qsen, Qlat, Cd, Kd, air_press, dateTime, Ts, hML, airT, wnd, RH, sw, lwnet = list(map(np.asanyarray, (wnd, \
+        Qsen, Qlat, Cd, Kd, air_press, dateTime, Ts, hML, airT, wnd, RH, sw, lwnet)))
+    #if no net, convert it to net
+    if not lwnet_mode:
+        Tk = Ts+Kelvin # water temperature in Kelvin
+        LWo = S_B*emiss*Tk**4 # long wave out
+        lwnet = lwnet-LWo
+
+    Kelvin = 273.15 # temp mod for deg K   
+    emiss = 0.972 # emissivity;
+    S_B = 5.67E-8 # Stefan-Boltzman constant (?K is used)
+    vonK = 0.41 # von Karman  constant
+    dT = 0.5   # change in temp for mixed layer depth
+    C1 = 114.278 # from Soloviev et al. 2007
+    nu = 0.29 # proportionality constant from Zappa et al. 2007, lower bounds
+    KeCrit = 0.18     # constant for wave age = 20 (Soloviev et al. 2007)
+    albedo_SW = 0.07
+    swRat = 0.46 # percentage of SW radiation that penetrates the water column
+    g = 9.81 # gravity
+    C_w = 4186 # J kg-1 ?C-1 (Lenters et al. 2005)
+    mnWnd = 0.2 # minimum wind speed
+
+    # impose limit on wind speed
+    rpcI = wnd < mnWnd
+    wnd[rpcI] = mnWnd
+
+    # calculate sensible and latent heat fluxes
+    C_D = Cd # drag coefficient for momentum
+    E = Qlat # latent heat flux
+    H = Qsen # sensible heat flux
+
+    # calculate total heat flux
+    dUdt = sw*0.93 - E - H + lwnet
+    Qo = sw*(1-albedo_SW)*swRat
+
+    # calculate water density
+    rho_w = dens0(t=Ts, s=0.2)
+
+    # calculate u*
+    if (wnd_z != 10):
+        e1 = np.sqrt(C_D)
+        wnd = wnd/(1-e1/vonK*np.log(10/wnd_z))
+        
+    rhoAir = 1.2 #  air density
+    tau = C_D*wnd**2*rhoAir
+    uSt = np.sqrt(tau/rho_w)
+
+    # calculate the effective heat flux
+    q1 = 2-2*np.exp(hML*-Kd)
+    q2 = hML*Kd
+    q3 = np.exp(hML*-Kd)
+    H_star = dUdt-Qo*(q1/q2-q3) # Kim 1976
+
+    # calculate the thermal expansion coefficient 
+    tExp = thermalExpFromTemp(Ts)
+
+    # calculate buoyancy flux and w*
+    B1 = H_star*tExp*g
+    B2 = rho_w*C_w
+    Bflx = B1/B2
+    ltI = Bflx>0
+    if type(B1)==np.float64:
+        B1 = np.array(B1)
+    B1[ltI] = 0
+    divi = 1/3
+    w1 = -B1*hML
+    wSt = w1**divi
+
+    # calculate kinematic viscosiy
+    kinV = getKinematicVis(Ts)
+
+    KeDe = (kinV*g)
+    KeNm = uSt**3
+    Ke = KeNm/KeDe
+    tau = tau    # estimate of total tau (includes wave stress)
+    euPw = (1+Ke/KeCrit)  # tau_shear = tau/(1+Ke/Kecr)
+    tau_t = tau/euPw      # tau_shear, Soloviev
+    uTanS = tau_t/rho_w   
+    uTanS = uTanS**0.5
+
+    # calculate viscous sublayer
+    Sv = C1*kinV/uTanS
+    eu_N = uTanS**3      # e_u(0) = (tau_t/rho)**1.5/(vonK*Sv)
+    eu_D = vonK*Sv       # denominator
+    eu_0 = eu_N/eu_D    # in m2/s3
+    ew_0 = -1.0*B1       # buoyancy flux, but only when outward
+    e_0 = ew_0+eu_0     # e(0) from Soloviev (w/o wave effects)
+    K1 = e_0*kinV       # in units of m4/s4, want cm4/hr4
+    K2 = ew_0*kinV      # convective component (m4/s4)
+    K1 = K1*100**4*3600**4 # now in cm4/hr4  (Total)
+    K2 = K2*100**4*3600**4 # now in cm4/hr4  (Convective)
+    K600 = nu*600**(-0.5)*K1**(1/4)   # in cm/hr (Total)
+
+    #k600 = np.numeric(K600)
+    k600 = K600*24/100 #now in units in m d-1
+    return(k600)
+
+def k_heiskanen(wnd_z, Cd, Qlat, Qsen, Kd, air_press, dateTime, Ts, hML, airT, wnd, RH, sw, lwnet):
+
+    #Constants
+    S_B = 5.67E-8 # Stefan-Boltzman constant (K is used)
+    emiss = 0.972 # emissivity
+    Kelvin = 273.15 #conversion from C to Kelvin
+    albedo_SW = 0.07
+    vonK = 0.41 #von Karman constant
+    swRat = 0.46 # percentage of SW radiation that penetrates the water column
+    mnWnd = 0.2 # minimum wind speed
+    g = 9.81 # gravity
+    C_w = 4186 # J kg-1 ?C-1 (Lenters et al. 2005)
+
+    # impose limit on wind speed
+    rpcI = wnd < mnWnd
+    if type(wnd)==int:
+        wnd=np.array(wnd)
+    wnd[rpcI] = mnWnd
+
+
+    # calculate sensible and latent heat fluxes
+    #mm = calc.zeng(dateTime,Ts,airT,wnd,RH,air_press,wnd_z)
+    C_D = Cd # drag coefficient for momentum
+    E = Qlat # latent heat flux
+    H = Qsen # sensible heat flux
+
+    # calculate total heat flux
+    dUdt = sw*0.93 - E - H + lwnet
+    Qo = sw*(1-albedo_SW)*swRat
+
+    # calculate water density
+    rho_w = dens0(t=Ts, s=0.2)
+
+    # calculate u*
+    if (wnd_z != 10):
+        e1 = np.sqrt(C_D)
+        u10 = wnd/(1-e1/vonK*np.log(10/wnd_z))
+    else:
+        u10 = wnd
+
+
+    rhoAir = 1.2 #  air density
+    vonK = 0.41 # von Karman  constant
+    tau = C_D*u10**2*rhoAir
+    uSt = np.sqrt(tau/rho_w)
+
+    # calculate the effective heat flux
+    q1 = 2-2*np.exp(hML*-Kd)
+    q2 = hML*Kd
+    q3 = np.exp(hML*-Kd)
+    H_star = dUdt-Qo*(q1/q2-q3) # Kim 1976
+
+    # calculate the thermal expansion coefficient 
+    tExp = thermalExpFromTemp(Ts)
+
+    B1 = H_star*tExp*g #Imberger 1985: Effective heat flux * thermal expansion of water * gravity
+    B2 = rho_w*C_w # mean density of the water column * specific heat of water at constant pressure
+    Bflx = B1/B2
+
+    if Bflx<0:
+        wstar = (-Bflx*hML)**(1/3)#penetrative convective velocity Heiskanen 2014 (Imberger 1985)
+    else:
+        wstar = 0
+    Hk   = np.sqrt((0.00015*u10)**2 + (0.07*wstar)**2) 
+    Hk   = Hk*100*3600 # Heiskanen's K in cm/hr
+    Hk600 = Hk*600**(-0.5)
+    k600 = Hk600*24/100 #units in m d-1
+    return(k600)
+
+
+def k_macIntyre(wnd_z, Cd, Qlat, Qsen, Kd, air_press, dateTime, Ts, hML, airT, wnd, RH, sw, lwnet,
+                                params=np.array([1.2,0.4872,1.4784])):
+
+    #Constants
+    S_B = 5.67E-8 # Stefan-Boltzman constant (K is used)
+    emiss = 0.972 # emissivity;
+    Kelvin = 273.15 #conversion from C to Kelvin
+    albedo_SW = 0.07
+    vonK = 0.41 #von Karman constant
+    swRat = 0.46 # percentage of SW radiation that penetrates the water column
+    mnWnd = 0.2 # minimum wind speed
+    g = 9.81 # gravity
+    C_w = 4186 # J kg-1 ?C-1 (Lenters et al. 2005)
+
+    # impose limit on wind speed
+    rpcI = wnd < mnWnd
+    if type(wnd)==int:
+        wnd=np.array(wnd)
+    wnd[rpcI] = mnWnd
+
+
+    # calculate sensible and latent heat fluxes
+    C_D = Cd # drag coefficient for momentum
+    E = Qlat # latent heat flux
+    H = Qsen # sensible heat flux
+
+    # calculate total heat flux
+    dUdt = sw*0.93 - E - H + lwnet
+    Qo = sw*(1-albedo_SW)*swRat
+
+    # calculate water density
+    rho_w = dens0(t=Ts, s=0.2)
+
+    # calculate u*
+    if (wnd_z != 10):
+        e1 = np.sqrt(C_D)
+        u10 = wnd/(1-e1/vonK*np.log(10/wnd_z))
+    else:
+        u10 = wnd
+    
+
+    rhoAir = 1.2 #  air density
+    vonK = 0.41 # von Karman  constant
+    tau = C_D*u10**2*rhoAir
+    uSt = np.sqrt(tau/rho_w)
+
+    # calculate the effective heat flux
+    q1 = 2-2*np.exp(hML*-Kd)
+    q2 = hML*Kd
+    q3 = np.exp(hML*-Kd)
+    H_star = dUdt-Qo*(q1/q2-q3) # Kim 1976
+
+
+    # calculate the thermal expansion coefficient
+    tExp = thermalExpFromTemp(Ts)
+
+    B1 = H_star*tExp*g
+    B2 = rho_w*C_w
+    Bflx = B1/B2
+
+    # calculate kinematic viscosiy
+    kinV = getKinematicVis(Ts)
+    KeNm = uSt**3
+
+    #SmE   = 0.84*(-0.58*Bflx+1.76*KeNm/(vonK*hML))
+    SmE = params[0]*-Bflx+params[1]*KeNm/(vonK*hML) #change to two coefficients
+    if type(SmE)==np.float64:
+        SmE=np.array(SmE)
+    SmE[SmE<0] = 0    # set negative to 0
+    Sk   = SmE*kinV
+    Sk   = Sk*100**4*3600**4 # Sally's K now in cm4/h4
+    Sk600 = params[2]*600**(-0.5)*Sk**(1/4) # in cm/hr (Total)
+
+    k600 = Sk600 # why is this not already numeric?
+    k600 = k600*24/100 #units in m d-1
+    return k600
+
+def k_read_soloviev(wnd_z, Cd, Qlat, Qsen, Kd, lat, A0, air_press, dateTime, Ts, hML, airT, wnd, RH, sw, lwnet):
+    
+    wnd_z, Cd, Qlat, Qsen, Kd, lat, A0, air_press, dateTime, Ts, hML, airT, wnd, RH, sw, lwnet = list(map(np.asanyarray, (wnd_z,\
+         Cd, Qlat, Qsen, Kd, lat, A0, air_press, dateTime, Ts, hML, airT, wnd, RH, sw, lwnet)))
+    # define constants used in function
+    Kelvin = 273.15 # temp mod for deg K
+    emiss = 0.972 # emissivity;
+    S_B = 5.67E-8 # Stefan-Boltzman constant (?K is used)
+    vonK = 0.41 # von Karman  constant
+    dT = 0.5   # change in temp for mixed layer depth
+    C1 = 114.278 # from Soloviev et al. 2007
+    nu = 0.29 # proportionality constant from Zappa et al. 2007, lower bounds
+    KeCrit = 0.18     # constant for wave age = 20 (Soloviev et al. 2007)
+    albedo_SW = 0.07
+    swRat = 0.46 # percentage of SW radiation that penetrates the water column
+    g = 9.81 # gravity
+    C_w = 4186 # J kg-1 ?C-1 (Lenters et al. 2005)
+    mnWnd = 0.2 # minimum wind speed
+
+    # impose limit on wind speed
+    rpcI = wnd < mnWnd
+    wnd[rpcI] = mnWnd
+
+    # calculate sensible and latent heat fluxes
+    C_D = Cd # drag coefficient for momentum
+    E = Qlat # latent heat flux
+    H = Qsen # sensible heat flux
+
+    # calculate total heat flux
+    dUdt = sw*0.93 - E - H + lwnet
+    Qo = sw*(1-albedo_SW)*swRat #PAR
+
+    # calculate the effective heat flux
+    q1 = 2-2*np.exp(hML*-Kd)
+    q2 = hML*Kd
+    q3 = np.exp(hML*-Kd)
+    H_star = dUdt-Qo*(q1/q2-q3) #Effective surface heat flux Kim 1976
+
+    # calculate water density
+    rho_w = dens0(t=Ts, s=0.2)
+
+    # calculate u*
+    if (wnd_z != 10):
+        e1 = np.sqrt(C_D)
+        wnd = wnd/(1-e1/vonK*np.log(10/wnd_z))
+    
+    rhoAir = 1.2 #  air density
+    tau = C_D*wnd**2*rhoAir
+    uSt = np.sqrt(tau/rho_w)
+    uSta = np.sqrt(tau/rhoAir)  #friction velocity in air
+
+    # calculate the thermal expansion coefficient
+    tExp = thermalExpFromTemp(Ts)
+
+    # calculate buoyancy flux and w*
+    B1 = H_star*tExp*g #Hstar * coefficient of thermal expansion * gravity
+    B2 = rho_w*C_w
+    Bflx = B1/B2
+    
+    if type(Bflx)==np.float64:
+        Bflx = np.array(Bflx)
+    Bflx[Bflx>0] = 0
+
+    wSt = (-Bflx*hML)**1/3
+
+    # calculate kinematic viscosiy
+    kinV = getKinematicVis(Ts)
+    kinVa = getKinematicVis(airT)
+
+    KeDe = (kinV*g)
+    KeNm = uSt**3
+    Ke = KeNm/KeDe
+    tau = tau    # estimate of total tau (includes wave stress)
+    euPw = (1+Ke/KeCrit)  # tau_shear = tau/(1+Ke/Kecr) Ke is the Keulegan number
+    # Could calculate KeCrit (critical Keulegan number) from wave age
+    #KeCrit = (kinVa/kinV)*((rhoAir/rho_w)**1.5)*(Rbcr/Aw) # Eq1.16-Soloviev et al(2007)
+
+    tau_t = tau/euPw      # tau_t = tangential wind stress, tau = total wind stress
+    uTanS = tau_t/rho_w
+    uTanS = uTanS**0.5
+
+    # calculate viscous sublayer
+    Sv = C1*kinV/uTanS  # effective thickness of the aqueous viscous sublayer
+    eu_N = uTanS**3      # e_u(0) = (tau_t/rho)**1.5/(vonK*Sv)
+    eu_D = vonK*Sv      # denominator
+    eu_0 = eu_N/eu_D    # in m2/s3
+    ec_0 = -1.0*Bflx       # buoyancy flux, but only when outward
+
+    #ewave_0 turbulence due to wave breaking
+    A0 = A0/1e6 # convert surface area to km
+    Fetch = 2*np.sqrt(A0/np.pi) # fetch in km (assuming a conical lake)
+    Hs = 0.0163*(Fetch**0.5)*wnd # significant wave height - Woolf (2005)
+    Aw = (1/(2*np.pi))*(( (g*Hs*rhoAir)/(0.062*rho_w*
+            uSt**2))**(2/3)) # wave age - eqn 1.11 Soloviev et al. (2007)
+
+    W = 3.8e-6*wnd**3.4 # simplified whitecap fraction (Fariall et al. 2000)
+
+
+    Ap = 2.45*W*((1/(W**0.25))-1)
+    alphaW = 100 # p. 185 - Soloviev et al. (2007)
+    B = 16.6 # p. 185 - Soloviev et al. (2007)
+    Sq = 0.2 # p. 185 - Soloviev et al. (2007)
+    cT = 0.6 # p. 188 - Soloviev et al. (2007)
+    ewave_0 = ((Ap**4)*alphaW)*((3/(B*Sq))**0.5) * \
+                    (((Ke/KeCrit)**1.5)/((1+Ke/KeCrit)**1.5))* \
+                    (uSt*g*kinV)/(0.062*vonK*cT*((2*np.pi*Aw)**1.5)) * \
+                    (rhoAir/rho_w)
+
+    #------------------------------------
+    e_0 = ec_0+eu_0+ewave_0    # e(0) from Soloviev (w/o wave effects)
+    Kc = ec_0*kinV*100**4*3600**4      # convective component now in cm4/hr4  (Total)
+    Ku = eu_0*kinV*100**4*3600**4 # shear component now in cm4/hr4  (Total)
+    Kwave = ewave_0*kinV*100**4*3600**4 # wave component now in cm4/hr4  (Total)
+    Kall = e_0*kinV*100**4*3600**4       # turbulent kinetic energy now in cm4/hr4  (Total)
+
+    #Schmidt number could be calculated as temperature dependent
+    #Sc = 1568+(-86.04*Ts)+(2.142*Ts**2)+(-0.0216*Ts**3)
+    k600org = nu*600**(-0.5)*(Kc+Ku)**(1/4)   # in cm/hr (Total)
+    k600org = k600org*24/100 #now in units in m d-1
+
+    k600 = nu*600**(-0.5)*Kall**(1/4)   # in cm/hr (Total)
+    k600 = k600*24/100 #now in units in m d-1
+
+    # ---Breaking Wave Component, Author: R I Woolway, 2014-11-13 ---
+    # bubble mediated component - Woolf 1997
+    kbi = W*2450
+    beta_0 = 2.71*1e-2 # Ostwald gas solubility (Emerson and Hedges, 2008)
+    Sc = 1568+(-86.04*Ts)+(2.142*Ts**2)+(-0.0216*Ts**3) # Schmidt number
+    kbiii = (1+(1/(14*beta_0*Sc**(-0.5))**(1/1.2)))**1.2
+    kb = kbi/((beta_0*kbiii))
+    kb = kb*24/100 #units in m d-1
+    #----------------------------------------------------------------
+
+    k600b = k600+kb
+    #allks = pd.DataFrame(data =(Ku,Kc,Kwave,kb,k600org,k600,k600b), columns= ["shear","convective","wave","bubble","k600org","k600",'k600b'])
+    return k600b
+
+def k_vachon(wnd, A0, params=np.array([2.51,1.48,0.39])):
+    U10 = wnd  #This function uses just the wind speed it is supplied
+    k600 = params[0] + params[1]*U10 + params[2]*U10*np.log10(A0/1000000) # units in cm h-1
+    k600 = k600*24/100 #units in m d-1
+    return(k600)
+    
+
+def k600_2_kGAS(k600,temperature,gas="O2"):
+    #'@title Returns the gas exchange velocity for gas of interest w/ no unit conversions
+    #'@description 
+    #'Returns the gas exchange velocity for gas of interest w/ no unit conversions
+    #'@usage
+    #'k600.2.kGAS.base(k600,temperature,gas="O2")
+    #'
+    #'k600.2.kGAS(ts.data, gas="O2")
+    #'
+    #'@param ts.data Object of class data.frame with named columns datetime and k600 and wtr (water temp in deg C). Other columns are ignored
+    #'@param k600 k600 as vector array of numbers or single number
+    #'@param temperature Water temperature (deg C) as vector array of numbers or single number
+    #'@param gas gas for conversion, as string (e.g., 'CO2' or 'O2')
+    #'@return Numeric value of gas exchange velocity for gas
+    #'@author Jordan S. Read
+    #'@seealso \link{k.read} and \link{k.read.base} for functions that calculate k600 estimates
+    n	=	0.5
+    schmidt	=	getSchmidt(temperature,gas)
+    Sc600	=	schmidt/600
+
+    kGAS	=	k600*(Sc600**-n)
+    return(kGAS)
+
```

### Comparing `pylake-0.1.6/pylake.egg-info/PKG-INFO` & `pylake-0.1.7/pylake.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-Metadata-Version: 2.1
-Name: pylake
-Version: 0.1.6
-Summary: pylake
-Home-page: https://github.com/eawag-surface-waters-research/PyLake
-Author: Hugo Cruz
-Author-email: <huggcruzz@gmail.com>
-License: MIT
-Keywords: python,pylake,Lake analyzer,environmental data,Physical properties
-Description-Content-Type: text/markdown
-
-# PyLake
-
-This work present methods used to compute meaningful physical properties in aquatic sciences.
-
-The methods are based on Xarray. 
-Multi-dimensional large time-series array are compatible if an xarray is passed as input.
-
-Algorithms and documentation are sometimes inspired by LakeAnalyzer in R (https://github.com/GLEON/rLakeAnalyzer)
-
-Implemented methods:
-* Thermocline
-* Mixed layer
-* Metalimnion extent (epilimnion and hypolimnion depth)
-* Wedderburn Number
-* Schmidt stability
-* Heat content
-* Seiche periode
-* Lake Number
-* Brunt-Vaisala frequency
-* Average layer temperature
-* Monin-Obhukov 
-
-## Installation
-
-Pylake use Dask which require a python version >=3.8
-
-`pip install pylake`
-
-## Usage
-
-
-Have a look in the notebooks, an example is provided
-
-```python
-import pylake
-import numpy as np
-
-Temp = np.array([14.3,14,12.1,10,9.7,9.5,6,5])
-depth = np.array([1,2,3,4,5,6,7,8])
-epilimnion, hypolimnion = pylake.metalimnion(temp, depth)
-```
-
- ## Work in progress
- Warning messages
- Lake metabolizer is being implemented. 
+Metadata-Version: 2.1
+Name: pylake
+Version: 0.1.7
+Summary: pylake
+Home-page: https://github.com/eawag-surface-waters-research/pylake
+Author: Hugo Cruz
+Author-email: <huggcruzz@gmail.com>
+License: MIT
+Keywords: python,pylake,Lake analyzer,environmental data,Physical properties
+Description-Content-Type: text/markdown
+
+# PyLake
+
+This work present methods used to compute meaningful physical properties in aquatic sciences.
+
+The methods are based on Xarray. 
+Multi-dimensional large time-series array are compatible if an xarray is passed as input.
+
+Algorithms and documentation are sometimes inspired by LakeAnalyzer in R (https://github.com/GLEON/rLakeAnalyzer)
+
+Implemented methods:
+* Thermocline
+* Mixed layer
+* Metalimnion extent (epilimnion and hypolimnion depth)
+* Wedderburn Number
+* Schmidt stability
+* Heat content
+* Seiche periode
+* Lake Number
+* Brunt-Vaisala frequency
+* Average layer temperature
+* Monin-Obhukov 
+
+## Installation
+
+Pylake use Dask which require a python version >=3.8
+
+`pip install pylake`
+
+## Usage
+
+
+Have a look in the notebooks, an example is provided
+
+```python
+import pylake
+import numpy as np
+
+Temp = np.array([14.3,14,12.1,10,9.7,9.5,6,5])
+depth = np.array([1,2,3,4,5,6,7,8])
+epilimnion, hypolimnion = pylake.metalimnion(temp, depth)
+```
+
+ ## Work in progress
+ Warning messages
+ Lake metabolizer is being implemented.
```

### Comparing `pylake-0.1.6/setup.py` & `pylake-0.1.7/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-from setuptools import setup, find_packages
-
-with open('README.md') as f:
-    README = f.read()
-
-VERSION = '0.1.6'
-DESCRIPTION = 'pylake'
-
-setup(
-    name="pylake",
-    version=VERSION,
-    author="Hugo Cruz",
-    author_email="<huggcruzz@gmail.com>",
-    description=DESCRIPTION,
-    long_description=README,
-    long_description_content_type='text/markdown',
-    packages=find_packages(),
-    url='https://github.com/eawag-surface-waters-research/PyLake',
-    install_requires=[
-        'numpy>=1.19.5',
-        'pandas>=1.1.5',
-        'PyYAML>=6.0',
-        'scipy>=1.5.4',
-        'dask>=2022.02.1',
-        'xarray>=0.19.0',   
-        'seawater>=3.3.4'
-    ],
-    license="MIT",
-    keywords=['python', 'pylake', 'Lake analyzer', 'environmental data', 'Physical properties'],
+from setuptools import setup, find_packages
+
+with open('README.md') as f:
+    README = f.read()
+
+VERSION = '0.1.7'
+DESCRIPTION = 'pylake'
+
+setup(
+    name="pylake",
+    version=VERSION,
+    author="Hugo Cruz",
+    author_email="<huggcruzz@gmail.com>",
+    description=DESCRIPTION,
+    long_description=README,
+    long_description_content_type='text/markdown',
+    packages=find_packages(),
+    url='https://github.com/eawag-surface-waters-research/pylake',
+    install_requires=[
+        'numpy>=1.19.5',
+        'pandas>=1.1.5',
+        'PyYAML>=6.0',
+        'scipy>=1.5.4',
+        'dask>=2022.02.1',
+        'xarray>=0.19.0',   
+        'seawater>=3.3.4'
+    ],
+    license="MIT",
+    keywords=['python', 'pylake', 'Lake analyzer', 'environmental data', 'Physical properties'],
 )
```

### Comparing `pylake-0.1.6/test/test.py` & `pylake-0.1.7/test/test.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-import pylake
-import numpy as np
-import seawater as sw
-
-Temp = np.array([14.3,14,12.1,10,9.7,9.5,6,5])
-depth = np.array([1,2,3,4,5,6,7,8])
-
-thermoD, thermoInd = pylake.thermocline(Temp, depth)
-epilimnion, hypolimnion = pylake.metalimnion(Temp, depth)
-SthermoD, SthermoInd = pylake.seasonal_thermocline(Temp,depth)
-hML = pylake.mixed_layer(Temp,depth, threshold=0.4)
-n2 = pylake.buoyancy_freq(Temp, depth, g=9.81)
-avg_ep_T = pylake.Average_layer_temp(Temp, depth=depth, depth_ref=epilimnion, layer='top')
-avg_ep_rho = sw.dens0(s=0.2,t=avg_ep_T)
-avg_hyp_T = pylake.Average_layer_temp(Temp, depth=depth, depth_ref=hypolimnion, layer='bot')
-avg_hyp_rho = sw.dens0(s=0.2,t=avg_hyp_T)
-delta_rho = avg_hyp_rho-avg_ep_rho
-
-bthA = np.array([100,90,86,82,20,1])
-bthD = np.array([0,2.3,2.5,4.2,5.8,7])
-Lo = 50
-ustar = 0.5
-W = pylake.wedderburn(delta_rho, metaT=epilimnion, uSt=ustar, AvHyp_rho=avg_hyp_rho, Lo=Lo, g=9.81)
-Schmidt_stability = pylake.schmidt_stability(Temp, depth=depth, bthA=bthA, bthD=bthD, sal = 0.2, g=9.81, dz=0.1)
-heat_content = pylake.heat_content(Temp, bthA=bthA, bthD=bthD, depth=depth, s=0.2)
-seiche_period_1 = pylake.seiche_period_1(depth=depth, Zt=thermoD, Lt=Lo, delta_rho=delta_rho, AvHyp_rho=avg_hyp_rho, g= 9.81)
-Lake_number = pylake.Lake_number(bthA=bthA, bthD=bthD, ustar=ustar, St=Schmidt_stability, metaT=epilimnion, metaB=hypolimnion, averageHypoDense=avg_hyp_rho, g=9.81)
+import pylake
+import numpy as np
+import seawater as sw
+
+Temp = np.array([14.3,14,12.1,10,9.7,9.5,6,5])
+depth = np.array([1,2,3,4,5,6,7,8])
+
+thermoD, thermoInd = pylake.thermocline(Temp, depth)
+epilimnion, hypolimnion = pylake.metalimnion(Temp, depth)
+SthermoD, SthermoInd = pylake.seasonal_thermocline(Temp,depth)
+hML = pylake.mixed_layer(Temp,depth, threshold=0.4)
+n2 = pylake.buoyancy_freq(Temp, depth, g=9.81)
+avg_ep_T = pylake.Average_layer_temp(Temp, depth=depth, depth_ref=epilimnion, layer='top')
+avg_ep_rho = sw.dens0(s=0.2,t=avg_ep_T)
+avg_hyp_T = pylake.Average_layer_temp(Temp, depth=depth, depth_ref=hypolimnion, layer='bot')
+avg_hyp_rho = sw.dens0(s=0.2,t=avg_hyp_T)
+delta_rho = avg_hyp_rho-avg_ep_rho
+
+bthA = np.array([100,90,86,82,20,1])
+bthD = np.array([0,2.3,2.5,4.2,5.8,7])
+Lo = 50
+ustar = 0.5
+W = pylake.wedderburn(delta_rho, metaT=epilimnion, uSt=ustar, AvHyp_rho=avg_hyp_rho, Lo=Lo, g=9.81)
+Schmidt_stability = pylake.schmidt_stability(Temp, depth=depth, bthA=bthA, bthD=bthD, sal = 0.2, g=9.81, dz=0.1)
+heat_content = pylake.heat_content(Temp, bthA=bthA, bthD=bthD, depth=depth, s=0.2)
+seiche_period_1 = pylake.seiche_period_1(depth=depth, Zt=thermoD, Lt=Lo, delta_rho=delta_rho, AvHyp_rho=avg_hyp_rho, g= 9.81)
+Lake_number = pylake.Lake_number(bthA=bthA, bthD=bthD, ustar=ustar, St=Schmidt_stability, metaT=epilimnion, metaB=hypolimnion, averageHypoDense=avg_hyp_rho, g=9.81)
```

