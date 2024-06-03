# Comparing `tmp/nrf_regtool-5.3.0.tar.gz` & `tmp/nrf_regtool-5.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nrf_regtool-5.3.0.tar", last modified: Tue May 21 17:48:37 2024, max compression
+gzip compressed data, was "nrf_regtool-5.3.1.tar", last modified: Mon Jun  3 13:59:37 2024, max compression
```

## Comparing `nrf_regtool-5.3.0.tar` & `nrf_regtool-5.3.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 joni-l    (1000) joni-l    (1000)        0 2024-05-21 17:48:37.559389 nrf_regtool-5.3.0/
--rw-r--r--   0 joni-l    (1000) joni-l    (1000)    11358 2022-12-07 09:09:13.000000 nrf_regtool-5.3.0/LICENSE
--rw-r--r--   0 joni-l    (1000) joni-l    (1000)    13630 2024-05-21 17:48:37.559389 nrf_regtool-5.3.0/PKG-INFO
-drwxr-xr-x   0 joni-l    (1000) joni-l    (1000)        0 2024-05-21 17:48:37.559389 nrf_regtool-5.3.0/nrf_regtool.egg-info/
--rw-r--r--   0 joni-l    (1000) joni-l    (1000)    13630 2024-05-21 17:48:37.000000 nrf_regtool-5.3.0/nrf_regtool.egg-info/PKG-INFO
--rw-r--r--   0 joni-l    (1000) joni-l    (1000)      542 2024-05-21 17:48:37.000000 nrf_regtool-5.3.0/nrf_regtool.egg-info/SOURCES.txt
--rw-r--r--   0 joni-l    (1000) joni-l    (1000)        1 2024-05-21 17:48:37.000000 nrf_regtool-5.3.0/nrf_regtool.egg-info/dependency_links.txt
--rw-r--r--   0 joni-l    (1000) joni-l    (1000)       65 2024-05-21 17:48:37.000000 nrf_regtool-5.3.0/nrf_regtool.egg-info/entry_points.txt
--rw-r--r--   0 joni-l    (1000) joni-l    (1000)       74 2024-05-21 17:48:37.000000 nrf_regtool-5.3.0/nrf_regtool.egg-info/requires.txt
--rw-r--r--   0 joni-l    (1000) joni-l    (1000)       11 2024-05-21 17:48:37.000000 nrf_regtool-5.3.0/nrf_regtool.egg-info/top_level.txt
-drwxr-xr-x   0 joni-l    (1000) joni-l    (1000)        0 2024-05-21 17:48:37.559389 nrf_regtool-5.3.0/nrfregtool/
--rw-r--r--   0 joni-l    (1000) joni-l    (1000)     1565 2024-05-21 12:29:39.000000 nrf_regtool-5.3.0/nrfregtool/__init__.py
--rw-r--r--   0 joni-l    (1000) joni-l    (1000)      626 2023-06-15 07:04:14.000000 nrf_regtool-5.3.0/nrfregtool/__main__.py
--rw-r--r--   0 joni-l    (1000) joni-l    (1000)    17162 2024-05-21 12:29:39.000000 nrf_regtool-5.3.0/nrfregtool/bicr.py
--rw-r--r--   0 joni-l    (1000) joni-l    (1000)    18606 2024-05-21 12:29:39.000000 nrf_regtool-5.3.0/nrfregtool/cli.py
--rw-r--r--   0 joni-l    (1000) joni-l    (1000)    10576 2024-05-21 17:45:26.000000 nrf_regtool-5.3.0/nrfregtool/common.py
--rw-r--r--   0 joni-l    (1000) joni-l    (1000)    25372 2024-05-21 12:29:39.000000 nrf_regtool-5.3.0/nrfregtool/core.py
--rw-r--r--   0 joni-l    (1000) joni-l    (1000)    11195 2024-05-21 17:45:26.000000 nrf_regtool-5.3.0/nrfregtool/ctrlsel.py
--rw-r--r--   0 joni-l    (1000) joni-l    (1000)      906 2024-05-21 12:29:39.000000 nrf_regtool-5.3.0/nrfregtool/main.py
--rw-r--r--   0 joni-l    (1000) joni-l    (1000)    15737 2024-05-21 12:29:39.000000 nrf_regtool-5.3.0/nrfregtool/parsed_dt.py
-drwxr-xr-x   0 joni-l    (1000) joni-l    (1000)        0 2024-05-21 17:48:37.559389 nrf_regtool-5.3.0/nrfregtool/resources/
--rw-r--r--   0 joni-l    (1000) joni-l    (1000)        0 2024-04-28 12:59:50.000000 nrf_regtool-5.3.0/nrfregtool/resources/__init__.py
--rw-r--r--   0 joni-l    (1000) joni-l    (1000)    24086 2023-06-14 07:15:13.000000 nrf_regtool-5.3.0/nrfregtool/resources/uicrextended.svd
--rw-r--r--   0 joni-l    (1000) joni-l    (1000)    73290 2024-05-21 17:45:26.000000 nrf_regtool-5.3.0/nrfregtool/uicr.py
--rw-r--r--   0 joni-l    (1000) joni-l    (1000)      987 2024-05-21 12:29:39.000000 nrf_regtool-5.3.0/pyproject.toml
-drwxr-xr-x   0 joni-l    (1000) joni-l    (1000)        0 2024-05-21 17:48:37.559389 nrf_regtool-5.3.0/scripts/
--rw-r--r--   0 joni-l    (1000) joni-l    (1000)       74 2024-04-28 12:59:50.000000 nrf_regtool-5.3.0/scripts/requirements-base.txt
--rw-r--r--   0 joni-l    (1000) joni-l    (1000)       38 2024-05-21 17:48:37.559389 nrf_regtool-5.3.0/setup.cfg
+drwxr-xr-x   0 joni-l    (1000) joni-l    (1000)        0 2024-06-03 13:59:37.256099 nrf_regtool-5.3.1/
+-rw-r--r--   0 joni-l    (1000) joni-l    (1000)    11358 2022-12-07 09:09:13.000000 nrf_regtool-5.3.1/LICENSE
+-rw-r--r--   0 joni-l    (1000) joni-l    (1000)    13630 2024-06-03 13:59:37.256099 nrf_regtool-5.3.1/PKG-INFO
+drwxr-xr-x   0 joni-l    (1000) joni-l    (1000)        0 2024-06-03 13:59:37.256099 nrf_regtool-5.3.1/nrf_regtool.egg-info/
+-rw-r--r--   0 joni-l    (1000) joni-l    (1000)    13630 2024-06-03 13:59:37.000000 nrf_regtool-5.3.1/nrf_regtool.egg-info/PKG-INFO
+-rw-r--r--   0 joni-l    (1000) joni-l    (1000)      542 2024-06-03 13:59:37.000000 nrf_regtool-5.3.1/nrf_regtool.egg-info/SOURCES.txt
+-rw-r--r--   0 joni-l    (1000) joni-l    (1000)        1 2024-06-03 13:59:37.000000 nrf_regtool-5.3.1/nrf_regtool.egg-info/dependency_links.txt
+-rw-r--r--   0 joni-l    (1000) joni-l    (1000)       65 2024-06-03 13:59:37.000000 nrf_regtool-5.3.1/nrf_regtool.egg-info/entry_points.txt
+-rw-r--r--   0 joni-l    (1000) joni-l    (1000)       74 2024-06-03 13:59:37.000000 nrf_regtool-5.3.1/nrf_regtool.egg-info/requires.txt
+-rw-r--r--   0 joni-l    (1000) joni-l    (1000)       11 2024-06-03 13:59:37.000000 nrf_regtool-5.3.1/nrf_regtool.egg-info/top_level.txt
+drwxr-xr-x   0 joni-l    (1000) joni-l    (1000)        0 2024-06-03 13:59:37.256099 nrf_regtool-5.3.1/nrfregtool/
+-rw-r--r--   0 joni-l    (1000) joni-l    (1000)     1565 2024-05-21 12:29:39.000000 nrf_regtool-5.3.1/nrfregtool/__init__.py
+-rw-r--r--   0 joni-l    (1000) joni-l    (1000)      626 2023-06-15 07:04:14.000000 nrf_regtool-5.3.1/nrfregtool/__main__.py
+-rw-r--r--   0 joni-l    (1000) joni-l    (1000)    17162 2024-05-21 12:29:39.000000 nrf_regtool-5.3.1/nrfregtool/bicr.py
+-rw-r--r--   0 joni-l    (1000) joni-l    (1000)    18606 2024-05-21 12:29:39.000000 nrf_regtool-5.3.1/nrfregtool/cli.py
+-rw-r--r--   0 joni-l    (1000) joni-l    (1000)    10576 2024-05-21 17:45:26.000000 nrf_regtool-5.3.1/nrfregtool/common.py
+-rw-r--r--   0 joni-l    (1000) joni-l    (1000)    25372 2024-05-21 12:29:39.000000 nrf_regtool-5.3.1/nrfregtool/core.py
+-rw-r--r--   0 joni-l    (1000) joni-l    (1000)    11162 2024-06-03 13:37:31.000000 nrf_regtool-5.3.1/nrfregtool/ctrlsel.py
+-rw-r--r--   0 joni-l    (1000) joni-l    (1000)      906 2024-05-21 12:29:39.000000 nrf_regtool-5.3.1/nrfregtool/main.py
+-rw-r--r--   0 joni-l    (1000) joni-l    (1000)    15737 2024-05-21 12:29:39.000000 nrf_regtool-5.3.1/nrfregtool/parsed_dt.py
+drwxr-xr-x   0 joni-l    (1000) joni-l    (1000)        0 2024-06-03 13:59:37.256099 nrf_regtool-5.3.1/nrfregtool/resources/
+-rw-r--r--   0 joni-l    (1000) joni-l    (1000)        0 2024-04-28 12:59:50.000000 nrf_regtool-5.3.1/nrfregtool/resources/__init__.py
+-rw-r--r--   0 joni-l    (1000) joni-l    (1000)    24086 2023-06-14 07:15:13.000000 nrf_regtool-5.3.1/nrfregtool/resources/uicrextended.svd
+-rw-r--r--   0 joni-l    (1000) joni-l    (1000)    73290 2024-05-21 17:45:26.000000 nrf_regtool-5.3.1/nrfregtool/uicr.py
+-rw-r--r--   0 joni-l    (1000) joni-l    (1000)      987 2024-05-21 12:29:39.000000 nrf_regtool-5.3.1/pyproject.toml
+drwxr-xr-x   0 joni-l    (1000) joni-l    (1000)        0 2024-06-03 13:59:37.256099 nrf_regtool-5.3.1/scripts/
+-rw-r--r--   0 joni-l    (1000) joni-l    (1000)       74 2024-04-28 12:59:50.000000 nrf_regtool-5.3.1/scripts/requirements-base.txt
+-rw-r--r--   0 joni-l    (1000) joni-l    (1000)       38 2024-06-03 13:59:37.256099 nrf_regtool-5.3.1/setup.cfg
```

### Comparing `nrf_regtool-5.3.0/LICENSE` & `nrf_regtool-5.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nrf_regtool-5.3.0/PKG-INFO` & `nrf_regtool-5.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nrf-regtool
-Version: 5.3.0
+Version: 5.3.1
 Summary: Generate files of register content for memory-mapped peripherals.
 Author: Nordic Semiconductor ASA
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `nrf_regtool-5.3.0/nrf_regtool.egg-info/PKG-INFO` & `nrf_regtool-5.3.1/nrf_regtool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nrf-regtool
-Version: 5.3.0
+Version: 5.3.1
 Summary: Generate files of register content for memory-mapped peripherals.
 Author: Nordic Semiconductor ASA
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `nrf_regtool-5.3.0/nrf_regtool.egg-info/SOURCES.txt` & `nrf_regtool-5.3.1/nrf_regtool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nrf_regtool-5.3.0/nrfregtool/__init__.py` & `nrf_regtool-5.3.1/nrfregtool/__init__.py`

 * *Files identical despite different names*

### Comparing `nrf_regtool-5.3.0/nrfregtool/__main__.py` & `nrf_regtool-5.3.1/nrfregtool/__main__.py`

 * *Files identical despite different names*

### Comparing `nrf_regtool-5.3.0/nrfregtool/bicr.py` & `nrf_regtool-5.3.1/nrfregtool/bicr.py`

 * *Files identical despite different names*

### Comparing `nrf_regtool-5.3.0/nrfregtool/cli.py` & `nrf_regtool-5.3.1/nrfregtool/cli.py`

 * *Files identical despite different names*

### Comparing `nrf_regtool-5.3.0/nrfregtool/common.py` & `nrf_regtool-5.3.1/nrfregtool/common.py`

 * *Files identical despite different names*

### Comparing `nrf_regtool-5.3.0/nrfregtool/core.py` & `nrf_regtool-5.3.1/nrfregtool/core.py`

 * *Files identical despite different names*

### Comparing `nrf_regtool-5.3.0/nrfregtool/ctrlsel.py` & `nrf_regtool-5.3.1/nrfregtool/ctrlsel.py`

 * *Files 2% similar despite different names*

```diff
@@ -216,18 +216,19 @@
         NrfPsel(fun=NRF_FUN_EXMIF_DQ1, port=6, pin=5): Ctrlsel.EXMIF_RADIO_SERIAL1,
         NrfPsel(fun=NRF_FUN_EXMIF_DQ6, port=6, pin=6): Ctrlsel.EXMIF_RADIO_SERIAL1,
         NrfPsel(fun=NRF_FUN_EXMIF_DQ0, port=6, pin=7): Ctrlsel.EXMIF_RADIO_SERIAL1,
         NrfPsel(fun=NRF_FUN_EXMIF_DQ5, port=6, pin=8): Ctrlsel.EXMIF_RADIO_SERIAL1,
         NrfPsel(fun=NRF_FUN_EXMIF_DQ3, port=6, pin=9): Ctrlsel.EXMIF_RADIO_SERIAL1,
         NrfPsel(fun=NRF_FUN_EXMIF_DQ2, port=6, pin=10): Ctrlsel.EXMIF_RADIO_SERIAL1,
         NrfPsel(fun=NRF_FUN_EXMIF_DQ4, port=6, pin=11): Ctrlsel.EXMIF_RADIO_SERIAL1,
-        NrfPsel(fun=NRF_FUN_EXMIF_CS0, port=6, pin=3): Ctrlsel.EXMIF_RADIO_SERIAL1,
-        GpiosProp(name="cs-gpios", port=6, pin=3): Ctrlsel.EXMIF_RADIO_SERIAL1,
-        NrfPsel(fun=NRF_FUN_EXMIF_CS1, port=6, pin=13): Ctrlsel.EXMIF_RADIO_SERIAL1,
-        GpiosProp(name="cs-gpios", port=6, pin=13): Ctrlsel.EXMIF_RADIO_SERIAL1,
+        # Ref: NCSDK-27559
+        NrfPsel(fun=NRF_FUN_EXMIF_CS0, port=6, pin=3): Ctrlsel.GPIO,
+        GpiosProp(name="cs-gpios", port=6, pin=3): Ctrlsel.GPIO,
+        NrfPsel(fun=NRF_FUN_EXMIF_CS1, port=6, pin=13): Ctrlsel.GPIO,
+        GpiosProp(name="cs-gpios", port=6, pin=13): Ctrlsel.GPIO,
     },
 }
 
 
 def dt_lookup_ctrlsel(
     src: Union[edtlib.PinCtrl, edtlib.Property],
     psel: Union[NrfPsel, Tuple[int, int]],
```

### Comparing `nrf_regtool-5.3.0/nrfregtool/main.py` & `nrf_regtool-5.3.1/nrfregtool/main.py`

 * *Files identical despite different names*

### Comparing `nrf_regtool-5.3.0/nrfregtool/parsed_dt.py` & `nrf_regtool-5.3.1/nrfregtool/parsed_dt.py`

 * *Files identical despite different names*

### Comparing `nrf_regtool-5.3.0/nrfregtool/resources/uicrextended.svd` & `nrf_regtool-5.3.1/nrfregtool/resources/uicrextended.svd`

 * *Files identical despite different names*

### Comparing `nrf_regtool-5.3.0/nrfregtool/uicr.py` & `nrf_regtool-5.3.1/nrfregtool/uicr.py`

 * *Files identical despite different names*

### Comparing `nrf_regtool-5.3.0/pyproject.toml` & `nrf_regtool-5.3.1/pyproject.toml`

 * *Files identical despite different names*

