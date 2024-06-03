# Comparing `tmp/bus_user-0.3.7.tar.gz` & `tmp/bus_user-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bus_user-0.3.7.tar", last modified: Mon Jun  3 11:23:34 2024, max compression
+gzip compressed data, was "bus_user-0.3.8.tar", last modified: Mon Jun  3 11:26:44 2024, max compression
```

## Comparing `bus_user-0.3.7.tar` & `bus_user-0.3.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-06-03 11:23:34.149025 bus_user-0.3.7/
--rw-rw-rw-   0        0        0     1082 2023-12-11 08:31:15.000000 bus_user-0.3.7/LICENSE
--rw-rw-rw-   0        0        0     4233 2024-06-03 11:23:34.149025 bus_user-0.3.7/PKG-INFO
--rw-rw-rw-   0        0        0     3268 2024-06-03 09:53:46.000000 bus_user-0.3.7/README.md
-drwxrwxrwx   0        0        0        0 2024-06-03 11:23:34.142597 bus_user-0.3.7/bus_user/
--rw-rw-rw-   0        0        0     2074 2024-06-03 07:24:45.000000 bus_user-0.3.7/bus_user/__init__.py
--rw-rw-rw-   0        0        0     3366 2023-12-14 12:44:59.000000 bus_user-0.3.7/bus_user/history.py
--rw-rw-rw-   0        0        0     3761 2024-05-24 09:30:08.000000 bus_user-0.3.7/bus_user/i2c_client.py
--rw-rw-rw-   0        0        0     2158 2024-05-24 09:19:18.000000 bus_user-0.3.7/bus_user/line_parser.py
--rw-rw-rw-   0        0        0    44785 2024-06-03 09:52:45.000000 bus_user-0.3.7/bus_user/serial_client.py
--rw-rw-rw-   0        0        0      711 2024-06-03 08:38:51.000000 bus_user-0.3.7/bus_user/serial_derivatives.py
--rw-rw-rw-   0        0        0    18547 2024-05-31 07:59:53.000000 bus_user-0.3.7/bus_user/serial_server.py
-drwxrwxrwx   0        0        0        0 2024-06-03 11:23:34.148026 bus_user-0.3.7/bus_user.egg-info/
--rw-rw-rw-   0        0        0     4233 2024-06-03 11:23:34.000000 bus_user-0.3.7/bus_user.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      335 2024-06-03 11:23:34.000000 bus_user-0.3.7/bus_user.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-03 11:23:34.000000 bus_user-0.3.7/bus_user.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-06-03 11:23:34.000000 bus_user-0.3.7/bus_user.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-06-03 11:23:34.150025 bus_user-0.3.7/setup.cfg
--rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 bus_user-0.3.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 11:26:44.449041 bus_user-0.3.8/
+-rw-rw-rw-   0        0        0     1082 2023-12-11 08:31:15.000000 bus_user-0.3.8/LICENSE
+-rw-rw-rw-   0        0        0     4233 2024-06-03 11:26:44.448041 bus_user-0.3.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3268 2024-06-03 11:26:08.000000 bus_user-0.3.8/README.md
+drwxrwxrwx   0        0        0        0 2024-06-03 11:26:44.440901 bus_user-0.3.8/bus_user/
+-rw-rw-rw-   0        0        0     2217 2024-06-03 11:26:08.000000 bus_user-0.3.8/bus_user/__init__.py
+-rw-rw-rw-   0        0        0     3366 2023-12-14 12:44:59.000000 bus_user-0.3.8/bus_user/history.py
+-rw-rw-rw-   0        0        0     3761 2024-05-24 09:30:08.000000 bus_user-0.3.8/bus_user/i2c_client.py
+-rw-rw-rw-   0        0        0     2158 2024-05-24 09:19:18.000000 bus_user-0.3.8/bus_user/line_parser.py
+-rw-rw-rw-   0        0        0    44785 2024-06-03 09:52:45.000000 bus_user-0.3.8/bus_user/serial_client.py
+-rw-rw-rw-   0        0        0      711 2024-06-03 08:38:51.000000 bus_user-0.3.8/bus_user/serial_derivatives.py
+-rw-rw-rw-   0        0        0    18547 2024-05-31 07:59:53.000000 bus_user-0.3.8/bus_user/serial_server.py
+drwxrwxrwx   0        0        0        0 2024-06-03 11:26:44.448041 bus_user-0.3.8/bus_user.egg-info/
+-rw-rw-rw-   0        0        0     4233 2024-06-03 11:26:44.000000 bus_user-0.3.8/bus_user.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      335 2024-06-03 11:26:44.000000 bus_user-0.3.8/bus_user.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 11:26:44.000000 bus_user-0.3.8/bus_user.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-06-03 11:26:44.000000 bus_user-0.3.8/bus_user.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-03 11:26:44.450106 bus_user-0.3.8/setup.cfg
+-rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 bus_user-0.3.8/setup.py
```

### Comparing `bus_user-0.3.7/LICENSE` & `bus_user-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `bus_user-0.3.7/PKG-INFO` & `bus_user-0.3.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bus_user
-Version: 0.3.7
+Version: 0.3.8
 Summary: work with equipment over buses like Serial/i2c/... as client and server
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/bus_user
 Keywords: serial,serial bus,pyserial,serial port,com port,comport,rs232,UART,TTL,serial client,serial server,serial emulator,i2c
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,15 +16,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# bus_user (v0.3.7)
+# bus_user (v0.3.8)
 
 ## DESCRIPTION_SHORT
 work with equipment over buses like Serial/i2c/... as client and server
 
 ## DESCRIPTION_LONG
 ###
 NOTE: IT SEEMS THIS IS OLD DATA! see tests for actual usage!
```

### Comparing `bus_user-0.3.7/README.md` & `bus_user-0.3.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# bus_user (v0.3.7)
+# bus_user (v0.3.8)
 
 ## DESCRIPTION_SHORT
 work with equipment over buses like Serial/i2c/... as client and server
 
 ## DESCRIPTION_LONG
 ###
 NOTE: IT SEEMS THIS IS OLD DATA! see tests for actual usage!
```

### Comparing `bus_user-0.3.7/bus_user/__init__.py` & `bus_user-0.3.8/bus_user/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,14 +18,18 @@
 # )
 # ---------------------------------------------------------------------------------------------------------------------
 from .history import HistoryIO
 from .line_parser import LineParsed
 from .serial_client import (
     # BASE
     SerialClient,
+    SerialClient_FirstFree,
+    SerialClient_FirstFree_Shorted,
+    SerialClient_FirstFree_Paired,
+    SerialClient_FirstFree_AnswerValid,
 
     # AUX
 
     # TYPES
     TYPE__ADDRESS,
     TYPE__RW_ANSWER,
```

### Comparing `bus_user-0.3.7/bus_user/history.py` & `bus_user-0.3.8/bus_user/history.py`

 * *Files identical despite different names*

### Comparing `bus_user-0.3.7/bus_user/i2c_client.py` & `bus_user-0.3.8/bus_user/i2c_client.py`

 * *Files identical despite different names*

### Comparing `bus_user-0.3.7/bus_user/line_parser.py` & `bus_user-0.3.8/bus_user/line_parser.py`

 * *Files identical despite different names*

### Comparing `bus_user-0.3.7/bus_user/serial_client.py` & `bus_user-0.3.8/bus_user/serial_client.py`

 * *Files identical despite different names*

### Comparing `bus_user-0.3.7/bus_user/serial_derivatives.py` & `bus_user-0.3.8/bus_user/serial_derivatives.py`

 * *Files identical despite different names*

### Comparing `bus_user-0.3.7/bus_user/serial_server.py` & `bus_user-0.3.8/bus_user/serial_server.py`

 * *Files identical despite different names*

### Comparing `bus_user-0.3.7/bus_user.egg-info/PKG-INFO` & `bus_user-0.3.8/bus_user.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bus_user
-Version: 0.3.7
+Version: 0.3.8
 Summary: work with equipment over buses like Serial/i2c/... as client and server
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/bus_user
 Keywords: serial,serial bus,pyserial,serial port,com port,comport,rs232,UART,TTL,serial client,serial server,serial emulator,i2c
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,15 +16,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# bus_user (v0.3.7)
+# bus_user (v0.3.8)
 
 ## DESCRIPTION_SHORT
 work with equipment over buses like Serial/i2c/... as client and server
 
 ## DESCRIPTION_LONG
 ###
 NOTE: IT SEEMS THIS IS OLD DATA! see tests for actual usage!
```

### Comparing `bus_user-0.3.7/setup.py` & `bus_user-0.3.8/setup.py`

 * *Files identical despite different names*

