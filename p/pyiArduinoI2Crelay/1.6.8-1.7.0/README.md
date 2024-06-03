# Comparing `tmp/pyiArduinoI2Crelay-1.6.8.tar.gz` & `tmp/pyiArduinoI2Crelay-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyiArduinoI2Crelay-1.6.8.tar", last modified: Mon Aug 12 15:48:16 2019, max compression
+gzip compressed data, was "pyiArduinoI2Crelay-1.7.0.tar", last modified: Mon Jun  3 11:55:00 2024, max compression
```

## Comparing `pyiArduinoI2Crelay-1.6.8.tar` & `pyiArduinoI2Crelay-1.7.0.tar`

### file list

```diff
@@ -1,32 +1,27 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2019-08-12 15:48:16.000000 pyiArduinoI2Crelay-1.6.8/
--rw-r--r--   0 pi        (1000) pi        (1000)     1348 2019-08-12 15:48:16.000000 pyiArduinoI2Crelay-1.6.8/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      977 2019-08-06 11:18:40.000000 pyiArduinoI2Crelay-1.6.8/README.md
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2019-08-12 15:48:16.000000 pyiArduinoI2Crelay-1.6.8/pyiArduinoI2Crelay/
--rw-r--r--   0 pi        (1000) pi        (1000)       28 2019-08-06 11:18:40.000000 pyiArduinoI2Crelay-1.6.8/pyiArduinoI2Crelay/__init__.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2019-08-12 15:48:16.000000 pyiArduinoI2Crelay-1.6.8/pyiArduinoI2Crelay/cpp/
--rw-r--r--   0 pi        (1000) pi        (1000)     4015 2019-08-08 11:24:35.000000 pyiArduinoI2Crelay-1.6.8/pyiArduinoI2Crelay/cpp/detectionModule.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)     3070 2019-08-08 11:26:53.000000 pyiArduinoI2Crelay-1.6.8/pyiArduinoI2Crelay/cpp/digitalRead.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)     2643 2019-08-08 11:25:14.000000 pyiArduinoI2Crelay-1.6.8/pyiArduinoI2Crelay/cpp/digitalWrite.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)     5119 2019-08-08 11:25:30.000000 pyiArduinoI2Crelay-1.6.8/pyiArduinoI2Crelay/cpp/newAddress.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)     2607 2019-08-08 11:25:42.000000 pyiArduinoI2Crelay-1.6.8/pyiArduinoI2Crelay/cpp/reset.cpp
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2019-08-12 15:48:16.000000 pyiArduinoI2Crelay-1.6.8/pyiArduinoI2Crelay/examples/
--rw-r--r--   0 pi        (1000) pi        (1000)     1393 2019-08-09 14:04:51.000000 pyiArduinoI2Crelay-1.6.8/pyiArduinoI2Crelay/examples/analogRead.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2449 2019-08-09 14:04:51.000000 pyiArduinoI2Crelay-1.6.8/pyiArduinoI2Crelay/examples/analogWrite.py
--rw-r--r--   0 pi        (1000) pi        (1000)     4077 2019-08-12 14:35:30.000000 pyiArduinoI2Crelay-1.6.8/pyiArduinoI2Crelay/examples/currentProtection.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2503 2019-08-09 14:45:15.000000 pyiArduinoI2Crelay-1.6.8/pyiArduinoI2Crelay/examples/currentRead.py
--rw-r--r--   0 pi        (1000) pi        (1000)     3049 2019-08-12 14:26:59.000000 pyiArduinoI2Crelay-1.6.8/pyiArduinoI2Crelay/examples/currentWrite.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2885 2019-08-12 14:52:37.000000 pyiArduinoI2Crelay-1.6.8/pyiArduinoI2Crelay/examples/detectionModule.py
--rw-r--r--   0 pi        (1000) pi        (1000)     1964 2019-08-06 11:18:40.000000 pyiArduinoI2Crelay-1.6.8/pyiArduinoI2Crelay/examples/digitalRead.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2098 2019-08-12 14:54:05.000000 pyiArduinoI2Crelay-1.6.8/pyiArduinoI2Crelay/examples/digitalWrite.py
--rw-r--r--   0 pi        (1000) pi        (1000)     1846 2019-08-09 14:04:51.000000 pyiArduinoI2Crelay-1.6.8/pyiArduinoI2Crelay/examples/freqPWM.py
--rw-r--r--   0 pi        (1000) pi        (1000)     4159 2019-08-12 15:11:52.000000 pyiArduinoI2Crelay-1.6.8/pyiArduinoI2Crelay/examples/newAddress.py
--rw-r--r--   0 pi        (1000) pi        (1000)     1177 2019-08-06 11:18:40.000000 pyiArduinoI2Crelay-1.6.8/pyiArduinoI2Crelay/examples/reset.py
--rwx------   0 pi        (1000) pi        (1000)    48746 2019-08-08 12:56:59.000000 pyiArduinoI2Crelay-1.6.8/pyiArduinoI2Crelay/iarduino_I2C_Relay.cpp
--rwx------   0 pi        (1000) pi        (1000)    48337 2019-08-08 12:53:00.000000 pyiArduinoI2Crelay-1.6.8/pyiArduinoI2Crelay/iarduino_I2C_Relay.h
--rw-r--r--   0 pi        (1000) pi        (1000)     1300 2019-08-09 13:59:51.000000 pyiArduinoI2Crelay-1.6.8/pyiArduinoI2Crelay/iarduino_I2C_Relay.pxd
--rwxr-xr-x   0 pi        (1000) pi        (1000)    12156 2019-08-08 13:26:55.000000 pyiArduinoI2Crelay-1.6.8/pyiArduinoI2Crelay/iarduino_I2C_Relay_PI.h
--rw-r--r--   0 pi        (1000) pi        (1000)   264509 2019-08-09 14:00:10.000000 pyiArduinoI2Crelay-1.6.8/pyiArduinoI2Crelay/pyiArduinoI2Crelay.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)     3668 2019-08-09 13:59:53.000000 pyiArduinoI2Crelay-1.6.8/pyiArduinoI2Crelay/pyiArduinoI2Crelay.pyx
--rw-r--r--   0 pi        (1000) pi        (1000)      131 2019-08-06 11:18:40.000000 pyiArduinoI2Crelay-1.6.8/pyiArduinoI2Crelay/setup.py
--rw-r--r--   0 pi        (1000) pi        (1000)       40 2019-08-06 11:18:40.000000 pyiArduinoI2Crelay-1.6.8/setup.cfg
--rw-r--r--   0 pi        (1000) pi        (1000)      808 2019-08-12 15:48:09.000000 pyiArduinoI2Crelay-1.6.8/setup.py
+drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-06-03 11:55:00.453949 pyiArduinoI2Crelay-1.7.0/
+-rw-r--r--   0 dron      (1000) dron      (1000)     3289 2024-03-29 13:35:28.000000 pyiArduinoI2Crelay-1.7.0/LICENSE
+-rw-r--r--   0 dron      (1000) dron      (1000)       82 2024-03-29 13:35:28.000000 pyiArduinoI2Crelay-1.7.0/MANIFEST.in
+-rw-r--r--   0 dron      (1000) dron      (1000)     3313 2024-06-03 11:55:00.453949 pyiArduinoI2Crelay-1.7.0/PKG-INFO
+-rw-r--r--   0 dron      (1000) dron      (1000)     2954 2024-03-29 13:35:28.000000 pyiArduinoI2Crelay-1.7.0/README.md
+drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-06-03 11:55:00.445949 pyiArduinoI2Crelay-1.7.0/pyiArduinoI2Crelay/
+drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-06-03 11:55:00.453949 pyiArduinoI2Crelay-1.7.0/pyiArduinoI2Crelay/cpp/
+-rw-r--r--   0 dron      (1000) dron      (1000)     4015 2024-03-29 13:35:28.000000 pyiArduinoI2Crelay-1.7.0/pyiArduinoI2Crelay/cpp/detectionModule.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     3070 2024-03-29 13:35:28.000000 pyiArduinoI2Crelay-1.7.0/pyiArduinoI2Crelay/cpp/digitalRead.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     2643 2024-03-29 13:35:28.000000 pyiArduinoI2Crelay-1.7.0/pyiArduinoI2Crelay/cpp/digitalWrite.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     5119 2024-03-29 13:35:28.000000 pyiArduinoI2Crelay-1.7.0/pyiArduinoI2Crelay/cpp/newAddress.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     2607 2024-03-29 13:35:28.000000 pyiArduinoI2Crelay-1.7.0/pyiArduinoI2Crelay/cpp/reset.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     4308 2024-03-29 13:35:28.000000 pyiArduinoI2Crelay-1.7.0/pyiArduinoI2Crelay/cpp/watchDogTimer.cpp
+-rwxr-xr-x   0 dron      (1000) dron      (1000)    48746 2024-03-29 13:35:28.000000 pyiArduinoI2Crelay-1.7.0/pyiArduinoI2Crelay/iarduino_I2C_Relay.cpp
+-rwxr-xr-x   0 dron      (1000) dron      (1000)    48337 2024-03-29 13:35:28.000000 pyiArduinoI2Crelay-1.7.0/pyiArduinoI2Crelay/iarduino_I2C_Relay.h
+-rw-r--r--   0 dron      (1000) dron      (1000)     1300 2024-03-29 13:35:28.000000 pyiArduinoI2Crelay-1.7.0/pyiArduinoI2Crelay/iarduino_I2C_Relay.pxd
+-rwxr-xr-x   0 dron      (1000) dron      (1000)    12156 2024-03-29 13:35:28.000000 pyiArduinoI2Crelay-1.7.0/pyiArduinoI2Crelay/iarduino_I2C_Relay_PI.h
+-rw-r--r--   0 dron      (1000) dron      (1000)   567936 2024-06-03 11:49:11.000000 pyiArduinoI2Crelay-1.7.0/pyiArduinoI2Crelay/pyiArduinoI2Crelay.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     3668 2024-03-29 13:35:28.000000 pyiArduinoI2Crelay-1.7.0/pyiArduinoI2Crelay/pyiArduinoI2Crelay.pyx
+drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-06-03 11:55:00.449949 pyiArduinoI2Crelay-1.7.0/pyiArduinoI2Crelay.egg-info/
+-rw-r--r--   0 dron      (1000) dron      (1000)     3313 2024-06-03 11:55:00.000000 pyiArduinoI2Crelay-1.7.0/pyiArduinoI2Crelay.egg-info/PKG-INFO
+-rw-r--r--   0 dron      (1000) dron      (1000)      742 2024-06-03 11:55:00.000000 pyiArduinoI2Crelay-1.7.0/pyiArduinoI2Crelay.egg-info/SOURCES.txt
+-rw-r--r--   0 dron      (1000) dron      (1000)        1 2024-06-03 11:55:00.000000 pyiArduinoI2Crelay-1.7.0/pyiArduinoI2Crelay.egg-info/dependency_links.txt
+-rw-r--r--   0 dron      (1000) dron      (1000)        1 2024-03-29 14:05:07.000000 pyiArduinoI2Crelay-1.7.0/pyiArduinoI2Crelay.egg-info/not-zip-safe
+-rw-r--r--   0 dron      (1000) dron      (1000)       19 2024-06-03 11:55:00.000000 pyiArduinoI2Crelay-1.7.0/pyiArduinoI2Crelay.egg-info/top_level.txt
+-rw-r--r--   0 dron      (1000) dron      (1000)       79 2024-06-03 11:55:00.453949 pyiArduinoI2Crelay-1.7.0/setup.cfg
+-rw-r--r--   0 dron      (1000) dron      (1000)      808 2024-06-03 11:52:04.000000 pyiArduinoI2Crelay-1.7.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyiArduinoI2Crelay-1.6.8/pyiArduinoI2Crelay/cpp/detectionModule.cpp` & `pyiArduinoI2Crelay-1.7.0/pyiArduinoI2Crelay/cpp/detectionModule.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Crelay-1.6.8/pyiArduinoI2Crelay/cpp/digitalRead.cpp` & `pyiArduinoI2Crelay-1.7.0/pyiArduinoI2Crelay/cpp/digitalRead.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Crelay-1.6.8/pyiArduinoI2Crelay/cpp/digitalWrite.cpp` & `pyiArduinoI2Crelay-1.7.0/pyiArduinoI2Crelay/cpp/digitalWrite.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Crelay-1.6.8/pyiArduinoI2Crelay/cpp/newAddress.cpp` & `pyiArduinoI2Crelay-1.7.0/pyiArduinoI2Crelay/cpp/newAddress.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Crelay-1.6.8/pyiArduinoI2Crelay/cpp/reset.cpp` & `pyiArduinoI2Crelay-1.7.0/pyiArduinoI2Crelay/cpp/reset.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Crelay-1.6.8/pyiArduinoI2Crelay/iarduino_I2C_Relay.cpp` & `pyiArduinoI2Crelay-1.7.0/pyiArduinoI2Crelay/iarduino_I2C_Relay.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Crelay-1.6.8/pyiArduinoI2Crelay/iarduino_I2C_Relay.h` & `pyiArduinoI2Crelay-1.7.0/pyiArduinoI2Crelay/iarduino_I2C_Relay.h`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Crelay-1.6.8/pyiArduinoI2Crelay/iarduino_I2C_Relay.pxd` & `pyiArduinoI2Crelay-1.7.0/pyiArduinoI2Crelay/iarduino_I2C_Relay.pxd`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Crelay-1.6.8/pyiArduinoI2Crelay/iarduino_I2C_Relay_PI.h` & `pyiArduinoI2Crelay-1.7.0/pyiArduinoI2Crelay/iarduino_I2C_Relay_PI.h`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Crelay-1.6.8/pyiArduinoI2Crelay/pyiArduinoI2Crelay.pyx` & `pyiArduinoI2Crelay-1.7.0/pyiArduinoI2Crelay/pyiArduinoI2Crelay.pyx`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Crelay-1.6.8/setup.py` & `pyiArduinoI2Crelay-1.7.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from distutils.core import setup
 from distutils.extension import Extension
 
 with open("README.md", "r") as readme:
     long_description = readme.read()
 
 setup(name='pyiArduinoI2Crelay',
-    version='1.6.8',
+    version='1.7.0',
     description='iarduino.ru module for Raspberry Pi',
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         'Programming Language :: Python :: 3',
     ],
     url='http://github.com/tremaru/pyiArduinoI2Crelay',
```

