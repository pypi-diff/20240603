# Comparing `tmp/pyiArduinoI2Cmotor-0.0.2.tar.gz` & `tmp/pyiArduinoI2Cmotor-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyiArduinoI2Cmotor-0.0.2.tar", last modified: Wed Dec 23 18:23:33 2020, max compression
+gzip compressed data, was "pyiArduinoI2Cmotor-0.0.4.tar", last modified: Mon Jun  3 11:54:56 2024, max compression
```

## Comparing `pyiArduinoI2Cmotor-0.0.2.tar` & `pyiArduinoI2Cmotor-0.0.4.tar`

### file list

```diff
@@ -1,62 +1,69 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2020-12-23 18:23:33.000000 pyiArduinoI2Cmotor-0.0.2/
--rw-r--r--   0 pi        (1000) pi        (1000)     2433 2020-12-23 18:23:33.000000 pyiArduinoI2Cmotor-0.0.2/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)       21 2020-12-18 19:22:37.000000 pyiArduinoI2Cmotor-0.0.2/README
--rw-r--r--   0 pi        (1000) pi        (1000)     1870 2020-12-18 19:22:37.000000 pyiArduinoI2Cmotor-0.0.2/README.md
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2020-12-23 18:23:33.000000 pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/
--rw-r--r--   0 pi        (1000) pi        (1000)       28 2020-12-18 19:22:37.000000 pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/__init__.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2020-12-23 18:23:33.000000 pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/cpp/
--rw-------   0 pi        (1000) pi        (1000)     6715 2020-12-23 01:12:04.000000 pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/cpp/Car.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)     9719 2020-12-23 00:38:56.000000 pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/cpp/FindDevices.cpp
--rw-------   0 pi        (1000) pi        (1000)     3178 2020-12-23 01:13:57.000000 pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/cpp/FindMagnet.cpp
--rw-------   0 pi        (1000) pi        (1000)     2297 2020-12-23 01:13:49.000000 pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/cpp/FindMaxSpeed.cpp
--rw-------   0 pi        (1000) pi        (1000)     3146 2020-12-23 01:13:40.000000 pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/cpp/FindReducer.cpp
--rw-------   0 pi        (1000) pi        (1000)     2804 2020-12-23 01:13:32.000000 pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/cpp/GetError.cpp
--rw-------   0 pi        (1000) pi        (1000)     5051 2020-12-23 01:14:04.000000 pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/cpp/GetInfo.cpp
--rw-------   0 pi        (1000) pi        (1000)     2780 2020-12-23 01:14:09.000000 pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/cpp/GetSpeedM_S.cpp
--rw-------   0 pi        (1000) pi        (1000)     2032 2020-12-23 01:14:14.000000 pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/cpp/GetSpeedPWM.cpp
--rw-------   0 pi        (1000) pi        (1000)     2632 2020-12-23 01:14:18.000000 pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/cpp/GetSpeedRPM.cpp
--rw-------   0 pi        (1000) pi        (1000)     2226 2020-12-23 01:10:56.000000 pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/cpp/GetStop.cpp
--rw-------   0 pi        (1000) pi        (1000)     3847 2020-12-23 01:14:53.000000 pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/cpp/GetSum.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)     1400 2020-12-23 00:38:56.000000 pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/cpp/NewAddress.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)      517 2020-12-23 14:01:28.000000 pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/cpp/Serial.h
--rw-------   0 pi        (1000) pi        (1000)     2476 2020-12-23 01:14:26.000000 pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/cpp/SetDirection.cpp
--rw-------   0 pi        (1000) pi        (1000)     3342 2020-12-23 01:14:30.000000 pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/cpp/SetError.cpp
--rw-------   0 pi        (1000) pi        (1000)     4219 2020-12-23 01:14:39.000000 pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/cpp/SetSpeedM_S.cpp
--rw-------   0 pi        (1000) pi        (1000)     2333 2020-12-23 01:14:44.000000 pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/cpp/SetSpeedM_S_Stop.cpp
--rw-------   0 pi        (1000) pi        (1000)     3712 2020-12-23 01:14:47.000000 pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/cpp/SetSpeedPWM.cpp
--rw-------   0 pi        (1000) pi        (1000)     2317 2020-12-23 01:13:26.000000 pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/cpp/SetSpeedPWM_Stop.cpp
--rw-------   0 pi        (1000) pi        (1000)     3791 2020-12-23 01:13:13.000000 pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/cpp/SetSpeedRPM.cpp
--rw-------   0 pi        (1000) pi        (1000)     2332 2020-12-23 01:12:34.000000 pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/cpp/SetSpeedRPM_Stop.cpp
--rw-------   0 pi        (1000) pi        (1000)     3039 2020-12-23 01:12:24.000000 pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/cpp/SetStopNeutral.cpp
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2020-12-23 18:23:33.000000 pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/examples/
--rw-r--r--   0 pi        (1000) pi        (1000)     6091 2020-12-23 16:05:31.000000 pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/examples/Car.py
--rw-r--r--   0 pi        (1000) pi        (1000)     6131 2020-12-23 14:51:48.000000 pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/examples/FindDevices.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2835 2020-12-23 18:04:51.000000 pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/examples/FindMagnet.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2138 2020-12-23 16:13:02.000000 pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/examples/FindMaxSpeed.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2923 2020-12-23 16:15:22.000000 pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/examples/FindReducer.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2358 2020-12-23 16:18:53.000000 pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/examples/GetError.py
--rw-r--r--   0 pi        (1000) pi        (1000)     3597 2020-12-23 16:37:15.000000 pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/examples/GetInfo.py
--rw-r--r--   0 pi        (1000) pi        (1000)     1654 2020-12-23 17:03:00.000000 pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/examples/GetSpeedM_S.py
--rw-r--r--   0 pi        (1000) pi        (1000)     1868 2020-12-23 17:04:31.000000 pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/examples/GetSpeedPWM.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2363 2020-12-23 17:07:28.000000 pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/examples/GetSpeedRPM.py
--rw-r--r--   0 pi        (1000) pi        (1000)     1727 2020-12-23 17:24:08.000000 pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/examples/GetStop.py
--rw-r--r--   0 pi        (1000) pi        (1000)     3403 2020-12-23 17:25:10.000000 pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/examples/GetSum.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2191 2020-12-23 17:26:08.000000 pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/examples/SetDirection.py
--rw-r--r--   0 pi        (1000) pi        (1000)     3075 2020-12-23 18:19:42.000000 pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/examples/SetError.py
--rw-r--r--   0 pi        (1000) pi        (1000)     3828 2020-12-23 17:27:42.000000 pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/examples/SetSpeedM_S.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2015 2020-12-23 17:28:03.000000 pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/examples/SetSpeedM_S_Stop.py
--rw-r--r--   0 pi        (1000) pi        (1000)     3326 2020-12-23 17:28:28.000000 pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/examples/SetSpeedPWM.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2004 2020-12-23 17:28:56.000000 pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/examples/SetSpeedPWM_Stop.py
--rw-r--r--   0 pi        (1000) pi        (1000)     3507 2020-12-23 17:29:15.000000 pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/examples/SetSpeedRPM.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2017 2020-12-23 17:31:49.000000 pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/examples/SetSpeedRPM_Stop.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2470 2020-12-23 18:07:18.000000 pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/examples/SetStopNeutral.py
--rw-r--r--   0 pi        (1000) pi        (1000)     1257 2020-12-23 14:51:48.000000 pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/examples/newAddress.py
--rw-------   0 pi        (1000) pi        (1000)    64301 2020-12-22 23:47:46.000000 pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/iarduino_I2C_Motor.cpp
--rw-------   0 pi        (1000) pi        (1000)    27500 2020-12-22 23:45:23.000000 pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/iarduino_I2C_Motor.h
--rw-r--r--   0 pi        (1000) pi        (1000)     1422 2020-12-23 18:01:07.000000 pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/iarduino_I2C_Motor.pxd
--rw-r--r--   0 pi        (1000) pi        (1000)    11391 2020-12-23 14:02:19.000000 pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/iarduino_I2C_PI.h
--rw-r--r--   0 pi        (1000) pi        (1000)   326825 2020-12-23 18:22:01.000000 pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/pyiArduinoI2Cmotor.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)     6319 2020-12-23 18:21:18.000000 pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/pyiArduinoI2Cmotor.pyx
--rw-r--r--   0 pi        (1000) pi        (1000)      131 2020-12-18 19:22:37.000000 pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/setup.py
--rw-r--r--   0 pi        (1000) pi        (1000)       40 2020-12-14 16:18:30.000000 pyiArduinoI2Cmotor-0.0.2/setup.cfg
--rw-r--r--   0 pi        (1000) pi        (1000)      718 2020-12-23 18:23:31.000000 pyiArduinoI2Cmotor-0.0.2/setup.py
+drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-06-03 11:54:56.929996 pyiArduinoI2Cmotor-0.0.4/
+-rw-r--r--   0 dron      (1000) dron      (1000)     3291 2024-03-29 13:35:14.000000 pyiArduinoI2Cmotor-0.0.4/LICENSE
+-rw-r--r--   0 dron      (1000) dron      (1000)       83 2024-03-29 13:35:14.000000 pyiArduinoI2Cmotor-0.0.4/MANIFEST.in
+-rw-r--r--   0 dron      (1000) dron      (1000)     2168 2024-06-03 11:54:56.929996 pyiArduinoI2Cmotor-0.0.4/PKG-INFO
+-rw-r--r--   0 dron      (1000) dron      (1000)       21 2024-03-29 13:35:14.000000 pyiArduinoI2Cmotor-0.0.4/README
+-rw-r--r--   0 dron      (1000) dron      (1000)     1870 2024-03-29 13:35:14.000000 pyiArduinoI2Cmotor-0.0.4/README.md
+drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-06-03 11:54:56.901997 pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/
+-rw-r--r--   0 dron      (1000) dron      (1000)       28 2024-03-29 13:35:14.000000 pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/__init__.py
+drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-06-03 11:54:56.917997 pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/cpp/
+-rw-r--r--   0 dron      (1000) dron      (1000)     6715 2024-03-29 13:35:14.000000 pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/cpp/Car.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     9719 2024-03-29 13:35:14.000000 pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/cpp/FindDevices.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     3178 2024-03-29 13:35:14.000000 pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/cpp/FindMagnet.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     2297 2024-03-29 13:35:14.000000 pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/cpp/FindMaxSpeed.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     3146 2024-03-29 13:35:14.000000 pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/cpp/FindReducer.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     2804 2024-03-29 13:35:14.000000 pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/cpp/GetError.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     5051 2024-03-29 13:35:14.000000 pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/cpp/GetInfo.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     2780 2024-03-29 13:35:14.000000 pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/cpp/GetSpeedM_S.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     2032 2024-03-29 13:35:14.000000 pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/cpp/GetSpeedPWM.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     2632 2024-03-29 13:35:14.000000 pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/cpp/GetSpeedRPM.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     2226 2024-03-29 13:35:14.000000 pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/cpp/GetStop.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     3847 2024-03-29 13:35:14.000000 pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/cpp/GetSum.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     1400 2024-03-29 13:35:14.000000 pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/cpp/NewAddress.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)      517 2024-03-29 13:35:14.000000 pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/cpp/Serial.h
+-rw-r--r--   0 dron      (1000) dron      (1000)     2476 2024-03-29 13:35:14.000000 pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/cpp/SetDirection.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     3342 2024-03-29 13:35:14.000000 pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/cpp/SetError.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     4219 2024-03-29 13:35:14.000000 pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/cpp/SetSpeedM_S.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     2333 2024-03-29 13:35:14.000000 pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/cpp/SetSpeedM_S_Stop.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     3712 2024-03-29 13:35:14.000000 pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/cpp/SetSpeedPWM.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     2317 2024-03-29 13:35:14.000000 pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/cpp/SetSpeedPWM_Stop.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     3791 2024-03-29 13:35:14.000000 pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/cpp/SetSpeedRPM.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     2332 2024-03-29 13:35:14.000000 pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/cpp/SetSpeedRPM_Stop.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     3039 2024-03-29 13:35:14.000000 pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/cpp/SetStopNeutral.cpp
+drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-06-03 11:54:56.929996 pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/examples/
+-rw-r--r--   0 dron      (1000) dron      (1000)     6101 2024-03-29 13:35:14.000000 pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/examples/Car.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     6131 2024-03-29 13:35:14.000000 pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/examples/FindDevices.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     2837 2024-03-29 13:35:14.000000 pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/examples/FindMagnet.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     2037 2024-03-29 13:35:14.000000 pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/examples/FindMaxSpeed.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     2925 2024-03-29 13:35:14.000000 pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/examples/FindReducer.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     2362 2024-03-29 13:35:14.000000 pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/examples/GetError.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     3597 2024-03-29 13:35:14.000000 pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/examples/GetInfo.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     1654 2024-03-29 13:35:14.000000 pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/examples/GetSpeedM_S.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     1709 2024-03-29 13:35:14.000000 pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/examples/GetSpeedPWM.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     2204 2024-03-29 13:35:14.000000 pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/examples/GetSpeedRPM.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     1731 2024-03-29 13:35:14.000000 pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/examples/GetStop.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     3408 2024-03-29 13:35:14.000000 pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/examples/GetSum.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     1993 2024-03-29 13:35:14.000000 pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/examples/SetDirection.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     3079 2024-03-29 13:35:14.000000 pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/examples/SetError.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     3773 2024-03-29 13:35:14.000000 pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/examples/SetSpeedM_S.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     1958 2024-03-29 13:35:14.000000 pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/examples/SetSpeedM_S_Stop.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     3274 2024-03-29 13:35:14.000000 pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/examples/SetSpeedPWM.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     1891 2024-03-29 13:35:14.000000 pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/examples/SetSpeedPWM_Stop.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     3453 2024-03-29 13:35:14.000000 pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/examples/SetSpeedRPM.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     1906 2024-03-29 13:35:14.000000 pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/examples/SetSpeedRPM_Stop.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     2470 2024-03-29 13:35:14.000000 pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/examples/SetStopNeutral.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     1257 2024-03-29 13:35:14.000000 pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/examples/newAddress.py
+-rw-r--r--   0 dron      (1000) dron      (1000)    64301 2024-03-29 13:35:14.000000 pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/iarduino_I2C_Motor.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)    27500 2024-03-29 13:35:14.000000 pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/iarduino_I2C_Motor.h
+-rw-r--r--   0 dron      (1000) dron      (1000)     1422 2024-03-29 13:35:14.000000 pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/iarduino_I2C_Motor.pxd
+-rw-r--r--   0 dron      (1000) dron      (1000)    11391 2024-03-29 13:35:14.000000 pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/iarduino_I2C_PI.h
+-rw-r--r--   0 dron      (1000) dron      (1000)   685675 2024-06-03 11:48:38.000000 pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/pyiArduinoI2Cmotor.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     6319 2024-03-29 13:35:14.000000 pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/pyiArduinoI2Cmotor.pyx
+-rw-r--r--   0 dron      (1000) dron      (1000)      131 2024-03-29 13:35:14.000000 pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/setup.py
+drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-06-03 11:54:56.905997 pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor.egg-info/
+-rw-r--r--   0 dron      (1000) dron      (1000)     2168 2024-06-03 11:54:56.000000 pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor.egg-info/PKG-INFO
+-rw-r--r--   0 dron      (1000) dron      (1000)     2345 2024-06-03 11:54:56.000000 pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor.egg-info/SOURCES.txt
+-rw-r--r--   0 dron      (1000) dron      (1000)        1 2024-06-03 11:54:56.000000 pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor.egg-info/dependency_links.txt
+-rw-r--r--   0 dron      (1000) dron      (1000)       19 2024-06-03 11:54:56.000000 pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor.egg-info/top_level.txt
+-rw-r--r--   0 dron      (1000) dron      (1000)       79 2024-06-03 11:54:56.933996 pyiArduinoI2Cmotor-0.0.4/setup.cfg
+-rw-r--r--   0 dron      (1000) dron      (1000)      718 2024-06-03 11:51:53.000000 pyiArduinoI2Cmotor-0.0.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyiArduinoI2Cmotor-0.0.2/PKG-INFO` & `pyiArduinoI2Cmotor-0.0.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pyiArduinoI2Cmotor
-Version: 0.0.2
+Version: 0.0.4
 Summary: iarduino.ru module for Raspberry Pi
 Home-page: http://github.com/tremaru/pyiArduinoI2Cmotor
 Author: iarduino.ru
 Author-email: shop@iarduino.ru
 License: MIT
-Description: [![](https://iarduino.ru/img/logo.svg)](https://iarduino.ru)[![](https://wiki.iarduino.ru/img/git-shop.svg?3)](https://iarduino.ru) [![](https://wiki.iarduino.ru/img/git-wiki.svg?2)](https://wiki.iarduino.ru) [![](https://wiki.iarduino.ru/img/git-lesson.svg?2)](https://lesson.iarduino.ru)[![](https://wiki.iarduino.ru/img/git-forum.svg?2)](http://forum.trema.ru)
-        
-        # pyiArduinoI2Cmotor
-        
-        **Данная библилотека (модуль для Python3) позволяет управлять электронными модулями (устройствами) []() от iArduino.ru по шине I2C на Raspberry Pi.**
-        
-        Подробнее про датчик читайте в нашей [Wiki]()
-        
-        ## Установка ##
-        
-        [Статья на сайте iarduino.ru](https://wiki.iarduino.ru/page/raspberry-python-modules/)
-        
-        Установка из репозиториев PyPI в терминале Raspberry:
-        
-        `sudo pip3 install pyiArduinoI2Cmotor`
-        
-        Самостоятельная сборка из исходников:
-        
-        `git clone https://github.com/tremaru/pyiArduinoI2Cmotor.git && cd pyiArduinoI2Cmotor/pyiArduinoI2Cmotor && python3 setup.py build_ext --inplace`
-        
-        Примеры для Python находятся в папке `pyiArduinoI2Cmotor/examples`
-        
-        Примеры для С++ находятся в папке `pyiArduinoI2Cmotor/cpp`. Так же в этой папке лежит *Makefile* для сборки
-        из исходников. Можно собрать сразу все примеры командой:
-        `make all` или `make`
-        Для сборки конкретного примера: `make "название примера"`
-        Например:
-        `make reset`
-        Для удаления собранных исполняемых файлов:
-        `make clean`
-        
-        **This is a Python3 module for Raspberry Pi. It can work with []() by iarduino.ru**
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
+License-File: LICENSE
+
+[![](https://iarduino.ru/img/logo.svg)](https://iarduino.ru)[![](https://wiki.iarduino.ru/img/git-shop.svg?3)](https://iarduino.ru) [![](https://wiki.iarduino.ru/img/git-wiki.svg?2)](https://wiki.iarduino.ru) [![](https://wiki.iarduino.ru/img/git-lesson.svg?2)](https://lesson.iarduino.ru)[![](https://wiki.iarduino.ru/img/git-forum.svg?2)](http://forum.trema.ru)
+
+# pyiArduinoI2Cmotor
+
+**Данная библилотека (модуль для Python3) позволяет управлять электронными модулями (устройствами) []() от iArduino.ru по шине I2C на Raspberry Pi.**
+
+Подробнее про датчик читайте в нашей [Wiki]()
+
+## Установка ##
+
+[Статья на сайте iarduino.ru](https://wiki.iarduino.ru/page/raspberry-python-modules/)
+
+Установка из репозиториев PyPI в терминале Raspberry:
+
+`sudo pip3 install pyiArduinoI2Cmotor`
+
+Самостоятельная сборка из исходников:
+
+`git clone https://github.com/tremaru/pyiArduinoI2Cmotor.git && cd pyiArduinoI2Cmotor/pyiArduinoI2Cmotor && python3 setup.py build_ext --inplace`
+
+Примеры для Python находятся в папке `pyiArduinoI2Cmotor/examples`
+
+Примеры для С++ находятся в папке `pyiArduinoI2Cmotor/cpp`. Так же в этой папке лежит *Makefile* для сборки
+из исходников. Можно собрать сразу все примеры командой:
+`make all` или `make`
+Для сборки конкретного примера: `make "название примера"`
+Например:
+`make reset`
+Для удаления собранных исполняемых файлов:
+`make clean`
+
+**This is a Python3 module for Raspberry Pi. It can work with []() by iarduino.ru**
```

### Comparing `pyiArduinoI2Cmotor-0.0.2/README.md` & `pyiArduinoI2Cmotor-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/cpp/Car.cpp` & `pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/cpp/Car.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/cpp/FindDevices.cpp` & `pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/cpp/FindDevices.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/cpp/FindMagnet.cpp` & `pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/cpp/FindMagnet.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/cpp/FindMaxSpeed.cpp` & `pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/cpp/FindMaxSpeed.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/cpp/FindReducer.cpp` & `pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/cpp/FindReducer.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/cpp/GetError.cpp` & `pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/cpp/GetError.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/cpp/GetInfo.cpp` & `pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/cpp/GetInfo.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/cpp/GetSpeedM_S.cpp` & `pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/cpp/GetSpeedM_S.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/cpp/GetSpeedPWM.cpp` & `pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/cpp/GetSpeedPWM.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/cpp/GetSpeedRPM.cpp` & `pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/cpp/GetSpeedRPM.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/cpp/GetStop.cpp` & `pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/cpp/GetStop.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/cpp/GetSum.cpp` & `pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/cpp/GetSum.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/cpp/NewAddress.cpp` & `pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/cpp/NewAddress.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/cpp/Serial.h` & `pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/cpp/Serial.h`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/cpp/SetDirection.cpp` & `pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/cpp/SetDirection.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/cpp/SetError.cpp` & `pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/cpp/SetError.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/cpp/SetSpeedM_S.cpp` & `pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/cpp/SetSpeedM_S.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/cpp/SetSpeedM_S_Stop.cpp` & `pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/cpp/SetSpeedM_S_Stop.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/cpp/SetSpeedPWM.cpp` & `pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/cpp/SetSpeedPWM.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/cpp/SetSpeedPWM_Stop.cpp` & `pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/cpp/SetSpeedPWM_Stop.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/cpp/SetSpeedRPM.cpp` & `pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/cpp/SetSpeedRPM.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/cpp/SetSpeedRPM_Stop.cpp` & `pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/cpp/SetSpeedRPM_Stop.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/cpp/SetStopNeutral.cpp` & `pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/cpp/SetStopNeutral.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/examples/Car.py` & `pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/examples/Car.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,24 +11,24 @@
 mot_L.radius = 12.2                                 #   Указываем радиус левого  колеса в мм (значение используется для движения на заданное растояние).
 mot_R.radius = 12.2                                 #   Указываем радиус правого колеса в мм (значение используется для движения на заданное растояние).
                                                     #
 while True:                                         #
 #  Движение вперёд:                                 #
     mot_L.setSpeed( 120, MOT_RPM)                   #   Указываем левому  мотору работать на скорости  120 об/мин, что соответствует 2 об/сек.
     mot_R.setSpeed( 120, MOT_RPM)                   #   Указываем правому мотору работать на скорости  120 об/мин, что соответствует 2 об/сек.
-    sleep(5)                                        #   Приостанавливаем выполнение скетча на 5 секунд. При этом моторы будут вращаться.
+    sleep(5)                                        #   Приостанавливаем выполнение скрипта на 5 секунд. При этом моторы будут вращаться.
 #  Движение вперёд с доворотом влево:               #
     mot_L.setSpeed(  60, MOT_RPM)                   #   Указываем левому  мотору работать на скорости   60 об/мин, что соответствует 1 об/сек.
     mot_R.setSpeed( 120, MOT_RPM)                   #   Указываем правому мотору работать на скорости  120 об/мин, что соответствует 2 об/сек.
-    sleep(5)                                        #   Приостанавливаем выполнение скетча на 5 секунд. При этом моторы будут вращаться.
+    sleep(5)                                        #   Приостанавливаем выполнение скрипта на 5 секунд. При этом моторы будут вращаться.
 #  Движение назад:                                  #
     mot_L.setSpeed(-120, MOT_RPM)                   #   Указываем левому  мотору работать на скорости -120 об/мин, что соответствует 2 об/сек в обратную сторону.
     mot_R.setSpeed(-120, MOT_RPM)                   #   Указываем правому мотору работать на скорости -120 об/мин, что соответствует 2 об/сек в обратную сторону.
-    sleep(5)                                        #   Приостанавливаем выполнение скетча на 5 секунд. При этом моторы будут вращаться.
+    sleep(5)                                        #   Приостанавливаем выполнение скрипта на 5 секунд. При этом моторы будут вращаться.
 #  Разворот на месте вправо:                        #
     mot_L.setSpeed( 120, MOT_RPM)                   #   Указываем левому  мотору работать на скорости  120 об/мин, что соответствует 2 об/сек.
     mot_R.setSpeed(-120, MOT_RPM)                   #   Указываем правому мотору работать на скорости -120 об/мин, что соответствует 2 об/сек в обратную сторону.
-    sleep(5)                                        #   Приостанавливаем выполнение скетча на 5 секунд. При этом моторы будут вращаться.
+    sleep(5)                                        #   Приостанавливаем выполнение скрипта на 5 секунд. При этом моторы будут вращаться.
 #  Движение вперёд на заданное растояние:           #
     mot_L.setSpeed( 200, MOT_RPM, 1.5, MOT_MET )    #   Указываем левому  мотору работать на скорости 200 об/мин с остановкой мотора через 1.5 м пройденого пути.
     mot_R.setSpeed( 200, MOT_RPM, 1.5, MOT_MET )    #   Указываем правому мотору работать на скорости 200 об/мин с остановкой мотора через 1.5 м пройденого пути.
-    sleep(20)                                       #   Приостанавливаем выполнение скетча на 20 секунд. За это время автомобиль точно успеет проехать 1.5 м (полтора метра) и остановиться.
+    sleep(20)                                       #   Приостанавливаем выполнение скрипта на 20 секунд. За это время автомобиль точно успеет проехать 1.5 м (полтора метра) и остановиться.
```

### Comparing `pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/examples/FindDevices.py` & `pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/examples/FindDevices.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/examples/FindMagnet.py` & `pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/examples/FindMagnet.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # ОПРЕДЕЛЕНИЕ РЕАЛЬНОГО КОЛИЧЕСТВА МАГНИТОВ:
 #  ВЫПОЛНИТЕ СЛЕДУЮЩИЕ ДЕЙСТВИЯ:
-#  После старта скетча, в мониторе будут появляться значения 0.00
+#  После старта скрипта, в мониторе будут появляться значения 0.00
 #  При вращении ротора мотора (в любую сторону), эти значения будут увеличиваться.
 #  Поверните вручную ротор мотора (на котором установлен кольцевой магнит) на 1 полный оборот.
 #  В результате кольцевой магнит обернётся один раз вокруг своей оси.
 #  В мониторе появится значение равное количеству магнитных полюсов магнита одной полярности.
 #  Для большей точности советуем повернуть ротор мотора 10 раз, и разделить полученное значение на 10.
 #  Ближайшее целое число и будет реальным количеством магнитных полюсов одной полярности.                                                   #
 from time import sleep
```

### Comparing `pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/examples/FindMaxSpeed.py` & `pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/examples/FindMaxSpeed.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # ПРИМЕР НАХОДИТ МАКСИМАЛЬНУЮ СКОРОСТЬ:     #
                                             #
 from pyiArduinoI2Cmotor import *            #   Подключаем библиотеку для работы с мотором I2C-flash.
 mot = pyiArduinoI2Cmotor(0x09)              #   Объявляем объект mot для работы с функциями и методами библиотеки pyiArduinoI2Cmotor, указывая адрес модуля на шине I2C.
                                             #   Если объявить объект без указания адреса (mot = pyiArduinoI2Cmotor ), то адрес будет найден автоматически.
-mot.begin()                                 #   Инициируем работу с мотором.
 mot.setSpeed( 100.0 , MOT_PWM )             #   Запускаем мотор на максимальной скорости (ШИМ=100%).
 result = 0                                  #   Определяем переменную для получения результата.
 cnt    = 1                                  #   Определяем счётчик отсутствия рекордов скорости.
 while cnt < 255:                            #   Выполняем цикл пока устанавливаются новые рекорды.
     cnt += 1
     s = mot.getSpeed(MOT_RPM)               #   Получаем текущее количество оборотов в минуту.
     if result < s:
```

### Comparing `pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/examples/FindReducer.py` & `pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/examples/FindReducer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # ОПРЕДЕЛЕНИЕ РЕАЛЬНОГО ПЕРЕДАТОЧНОГО ОТНОШЕНИЯ:    #
 #  ВЫПОЛНИТЕ СЛЕДУЮЩИЕ ДЕЙСТВИЯ:                    #
-#  После старта скетча, в мониторе будут появляться значения 0.00
+#  После старта скрипта, в мониторе будут появляться значения 0.00
 #  При вращении ротора мотора (в любую сторону), эти значения будут увеличиваться.
 #  Поворачивайте вручную ротор мотора до тех пор пока вал редуктора не повернётся на 1 полный оборот.
 #  В мониторе появится значение равное передаточному отношению редуктора. Оно может быть не целым!
 #  Для большей точности советуем поворачивать ротор мотора до тех пор, пока вал редуктора не повернётся 10 раз, и разделить полученное значение на 10.
                                                     #
 from pyiArduinoI2Cmotor import *                    #   Подключаем библиотеку для работы с мотором I2C-flash.
 mot = pyiArduinoI2Cmotor(0x09)                      #   Объявляем объект mot для работы с функциями и методами библиотеки pyiArduinoI2Cmotor, указывая адрес модуля на шине I2C.
```

### Comparing `pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/examples/GetError.py` & `pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/examples/GetError.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,12 +11,12 @@
         print("Набор заданной скорости.", end="")   #   Выводим сообщение.
 
         while(mot.getError()==MOT_ERR_SPD):         #   Пока сохраняется ошибка скорости.
             print(".", end = "")
             sleep(.1)                               #   Выводим точку с задержкой по времени.
 
     print("\r\nСкорость набрана.")
-    sleep(.5)                                       #   Приостанавливаем выполнение скетча на 500 миллисекунд.
+    sleep(.5)                                       #   Приостанавливаем выполнение скрипта на 500 миллисекунд.
     print("Останавливаем мотор.")                   #   Выводим сообщение.
     mot.setStop()                                   #   Останавливаем мотор.
     print("====================")                   #   Выводим разделитель.
-    sleep(.5)                                       #   Приостанавливаем выполнение скетча на 500 миллисекунд.
+    sleep(.5)                                       #   Приостанавливаем выполнение скрипта на 500 миллисекунд.
```

### Comparing `pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/examples/GetInfo.py` & `pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/examples/GetInfo.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/examples/GetSpeedM_S.py` & `pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/examples/GetSpeedM_S.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/examples/GetSpeedPWM.py` & `pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/examples/GetSpeedPWM.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 # ДАННЫЙ ПРИМЕР ИНФОРМИРУЕТ О ЗНАЧЕНИИ ШИМ:         #
                                                     #
 from pyiArduinoI2Cmotor import *                    #   Подключаем библиотеку для работы с мотором I2C-flash.
 mot = pyiArduinoI2Cmotor(0x09)                      #   Объявляем объект mot для работы с функциями и методами библиотеки pyiArduinoI2Cmotor, указывая адрес модуля на шине I2C.
                                                     #   Если объявить объект без указания адреса (mot = pyiArduinoI2Cmotor ), то адрес будет найден автоматически.
-mot.begin()                                         #   Инициируем работу с мотором.
-                                                    #
 while True:                                         #
     mot.setSpeed(50.0, MOT_PWM)                     #   Запускаем мотор установив ШИМ = 50% (ШИМ указывается в % 0 до ±100.0).
     print( mot.getSpeed(MOT_PWM) )                  #   Выводим установленное значение ШИМ.
-    sleep(5)                                        #   Приостанавливаем выполнение скетча на 5 секунд.
+    sleep(5)                                        #   Приостанавливаем выполнение скрипта на 5 секунд.
     mot.setSpeed(-50.0, MOT_PWM)                    #   Запускаем мотор установив ШИМ = -50% (ШИМ указывается в % 0 до ±100.0).
     print( mot.getSpeed(MOT_PWM) )                  #   Выводим установленное значение ШИМ.
-    sleep(5)                                        #   Приостанавливаем выполнение скетча на 5 секунд.
+    sleep(5)                                        #   Приостанавливаем выполнение скрипта на 5 секунд.
```

### Comparing `pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/examples/GetSpeedRPM.py` & `pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/examples/GetSpeedRPM.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 # ДАННЫЙ ПРИМЕР ИНФОРМИРУЕТ О НАБОРЕ СКОРОСТИ:
 
 from pyiArduinoI2Cmotor import *                    #   Подключаем библиотеку для работы с мотором I2C-flash.
 mot = pyiArduinoI2Cmotor(0x09)                      #   Объявляем объект mot для работы с функциями и методами библиотеки pyiArduinoI2Cmotor, указывая адрес модуля на шине I2C.
                                                     #   Если объявить объект без указания адреса (mot = pyiArduinoI2Cmotor ), то адрес будет найден автоматически.
-mot.begin()                                         #   Инициируем работу с мотором.
-                                                    #
 while True:                                         #
     print("Запускаем мотор 100 об/мин.")            #   Выводим сообщение о запуске мотора.
     mot.setSpeed(100, MOT_RPM)                      #   Запускаем мотор на скорости 100 об/мин.
     while mot.getError()==MOT_ERR_SPD:              #   Пока сохраняется ошибка скорости.
         print("Реальная скорость = ")               #   Выводим сообщение.
         print( mot.getSpeed(MOT_RPM) )              #   Выводим реальное значение скорости.
         print(" об/мин.\r\n")                       #   Выводим сообщение.
 
     print("Скорость набрана.")                      #   Выводим сообщение.
-    sleep(.5)                                       #   Приостанавливаем выполнение скетча на 500 миллисекунд.
+    sleep(.5)                                       #   Приостанавливаем выполнение скрипта на 500 миллисекунд.
     print("Останавливаем мотор.")                   #   Выводим сообщение.
     mot.setStop()                                   #   Останавливаем мотор.
     print("====================")                   #   Выводим разделитель.
-    sleep(.5)                                       #   Приостанавливаем выполнение скетча на 500 миллисекунд.
+    sleep(.5)                                       #   Приостанавливаем выполнение скрипта на 500 миллисекунд.
```

### Comparing `pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/examples/GetStop.py` & `pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/examples/GetStop.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,11 +6,11 @@
 mot.radius = 12.2                                   #   Указываем радиус колеса в мм.
                                                     #
 while True:                                         #
     mot.setSpeed(100, MOT_RPM, 0.5, MOT_MET)        #   Запускаем мотор на скорости 100 об/мин с остановкой мотора через 0.5 метра.
     while mot.getStop(MOT_MET):                     #   Если путь до остановки ещё не пройден.
         print( mot.getStop(MOT_MET) )               #   Выводим оставшееся расстояние до остановки.
         println(" m.")
-        sleep(.1)                                   #   Приостанавливаем выполнение скетча на 0.1 секунду.
+        sleep(.1)                                   #   Приостанавливаем выполнение скрипта на 0.1 секунду.
 
     print("-----------------")
-    sleep(1)                                        #   Приостанавливаем выполнение скетча на 1 секунду.
+    sleep(1)                                        #   Приостанавливаем выполнение скрипта на 1 секунду.
```

### Comparing `pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/examples/GetSum.py` & `pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/examples/GetSum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# ПРИМЕР ВЫВОДИТ КОЛИЧЕСТВО СОВЕРШЁННЫХ ОБОРОТОВ
+# ПРИМЕР ВЫВОДИТ КОЛИЧЕСТВО СОВЕРШЁННЫХ ОБОРОТОВ TODO
 
 from pyiArduinoI2Cmotor import *                    #   Подключаем библиотеку для работы с мотором I2C-flash.
 mot = pyiArduinoI2Cmotor(0x09)                      #   Объявляем объект mot для работы с функциями и методами библиотеки pyiArduinoI2Cmotor, указывая адрес модуля на шине I2C.
                                                     #   Если объявить объект без указания адреса (mot = pyiArduinoI2Cmotor ), то адрес будет найден автоматически.
 mot.radius = 12.2                                   #   Указываем радиус колеса в мм.
 mot.setSpeed(60, MOT_RPM)                           #   Запускаем мотор на скорости 60 об/мин.
                                                     #
```

### Comparing `pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/examples/SetDirection.py` & `pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/examples/SetDirection.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 # ПРИМЕР ВЫБОРА БОРТА УСТАНОВКИ (ЛЕВЫЙ/ПРАВЫЙ):
 
 from pyiArduinoI2Cmotor import *        #   Подключаем библиотеку для работы с мотором I2C-flash.
-mot = pyiArduinoI2Cmotor1(0x09)         #   Объявляем объект mot1 для работы с функциями и методами библиотеки pyiArduinoI2Cmotor, указывая адрес модуля на шине I2C.
-mot = pyiArduinoI2Cmotor2(0x0A)         #   Объявляем объект mot2 для работы с функциями и методами библиотеки pyiArduinoI2Cmotor, указывая адрес модуля на шине I2C.
+mot1 = pyiArduinoI2Cmotor(0x09)         #   Объявляем объект mot1 для работы с функциями и методами библиотеки pyiArduinoI2Cmotor, указывая адрес модуля на шине I2C.
+mot2 = pyiArduinoI2Cmotor(0x0A)         #   Объявляем объект mot2 для работы с функциями и методами библиотеки pyiArduinoI2Cmotor, указывая адрес модуля на шине I2C.
                                         #   При наличии нескольких моторов на шине I2C нельзя объявлять объект без указания адреса.
-mot1.begin()                            #   Инициируем работу с 1 мотором.
-mot2.begin()                            #   Инициируем работу с 2 мотором.
 mot1.setDirection(True)                 #   Задаём направление вращения для 1 мотора: по часовой стрелке при положительных скоростях и против при отрицательных.
 mot2.setDirection(False)                #   Задаём направление вращения для 2 мотора: против часовой стрелки при положительных скоростях и по при отрицательных.
                                                  #
 # Если моторы установлены по бокам подвижного    #
 # механизма (машине, танке, тракторе...), то для #
 # реализации поступательного движения механизма, #
 # моторы расположенные на противоположных бортах #
```

### Comparing `pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/examples/SetError.py` & `pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/examples/SetError.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,17 @@
                                                     #   Если объявить объект без указания адреса (mot = pyiArduinoI2Cmotor ), то адрес будет найден автоматически.
 mot.setError(10)                                    #   Задаём максимально допустимый процент отклонения заданной скорости от реальной, превышение которого приведёт к появлению ошибки.
                                                     #
                                                     #   Теперь функция getError() будет возвращать значение MOT_ERR_SPD если текущая скорость отличается от заданной более чем на 10%.
                                                     #   При том же значении будет включаться красный светодиод на плате модуля.
 while True:                                         #
     mot.setSpeed(100, MOT_RPM)                      #   Запускаем мотор на скорости 100 об/мин.
-    sleep(1)                                        #   Приостанавливаем выполнение скетча на 1 секунду.
+    sleep(1)                                        #   Приостанавливаем выполнение скрипта на 1 секунду.
     mot.setStop()                                   #   Останавливаем мотор.
-    sleep(.5)                                       #   Приостанавливаем выполнение скетча на 500 миллисекунд.
+    sleep(.5)                                       #   Приостанавливаем выполнение скрипта на 500 миллисекунд.
                                                     #
 #  По умолчанию, ошибка скорости возникает при   #   Значение заданное функцией mot.setError()
 #  отличии заданной скорости от реальной более   #   сохраняется в энергонезависимой памяти модуля.
 #  чем на 10 процентов. Измените данное значение #
 #  обратившись к функции mot.setError()  и       #
 #  обратите внимание на то как изменится         #
 #  длительность свечения красного светодиода     #   Для большей нагладности предлагаем изменить
```

### Comparing `pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/examples/SetSpeedM_S.py` & `pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/examples/SetSpeedM_S.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 # ПРИМЕР ЗАПУСКАЕТ МОТОР С УКАЗАНИЕМ СКОРОСТИ:
 
-from pyiArduinoI2Cmotor import *                    #   Подключаем библиотеку для работы с мотором I2C-flash.
-mot = pyiArduinoI2Cmotor(0x09)                      #   Объявляем объект mot для работы с функциями и методами библиотеки pyiArduinoI2Cmotor, указывая адрес модуля на шине I2C.
-                                                  #   Если объявить объект без указания адреса (mot = pyiArduinoI2Cmotor ), то адрес будет найден автоматически.
-mot.radius = 12.2                             #   Указываем радиус колеса в мм.
-                                                  #
-while True:                                      #
-    mot.setSpeed( 0.0766f, MOT_M_S)               #   Запускаем мотор на скорости  0.0766 м/сек, что соответствует   60 об/мин при радиусе колеса в 12,2 мм.
-    sleep(5)                                   #   Приостанавливаем выполнение  скетча на 5 секунд.
-    mot.setSpeed( 0.1532f, MOT_M_S)               #   Запускаем мотор на скорости  0.1532 м/сек, что соответствует  120 об/мин при радиусе колеса в 12,2 мм.
-    sleep(5)                                   #   Приостанавливаем выполнение  скетча на 5 секунд.
-    mot.setSpeed( 0.0766f, MOT_M_S)               #   Запускаем мотор на скорости  0.0766 м/сек, что соответствует   60 об/мин при радиусе колеса в 12,2 мм.
-    sleep(5)                                   #   Приостанавливаем выполнение  скетча на 5 секунд.
-    mot.setSpeed(       0, MOT_M_S)               #   Запускаем мотор на скорости       0 м/сек, что соответствует остановке мотора.
-    sleep(5)                                   #   Приостанавливаем выполнение  скетча на 5 секунд.
-    mot.setSpeed(-0.0766f, MOT_M_S)               #   Запускаем мотор на скорости -0.0766 м/сек, что соответствует  -60 об/мин при радиусе колеса в 12,2 мм.
-    sleep(5)                                   #   Приостанавливаем выполнение  скетча на 5 секунд.
-    mot.setSpeed(-0.1532f, MOT_M_S)               #   Запускаем мотор на скорости -0.1532 м/сек, что соответствует -120 об/мин при радиусе колеса в 12,2 мм.
-    sleep(5)                                   #   Приостанавливаем выполнение  скетча на 5 секунд.
-    mot.setSpeed(-0.0766f, MOT_M_S)               #   Запускаем мотор на скорости -0.0766 м/сек, что соответствует  -60 об/мин при радиусе колеса в 12,2 мм.
-    sleep(5)                                   #   Приостанавливаем выполнение  скетча на 5 секунд.
-    mot.setSpeed(       0, MOT_M_S)               #   Запускаем мотор на скорости       0 м/сек, что соответствует остановке мотора.
-    sleep(5)                                   #   Приостанавливаем выполнение  скетча на 5 секунд.
-}                                                 #
+from pyiArduinoI2Cmotor import *                #   Подключаем библиотеку для работы с мотором I2C-flash.
+mot = pyiArduinoI2Cmotor(0x09)                  #   Объявляем объект mot для работы с функциями и методами библиотеки pyiArduinoI2Cmotor, указывая адрес модуля на шине I2C.
+                                                #   Если объявить объект без указания адреса (mot = pyiArduinoI2Cmotor ), то адрес будет найден автоматически.
+mot.radius = 12.2                               #   Указываем радиус колеса в мм.
+                                                #
+while True:                                     #
+    mot.setSpeed( 0.0766, MOT_M_S)              #   Запускаем мотор на скорости  0.0766 м/сек, что соответствует   60 об/мин при радиусе колеса в 12,2 мм.
+    sleep(5)                                    #   Приостанавливаем выполнение  скрипта на 5 секунд.
+    mot.setSpeed( 0.1532, MOT_M_S)              #   Запускаем мотор на скорости  0.1532 м/сек, что соответствует  120 об/мин при радиусе колеса в 12,2 мм.
+    sleep(5)                                    #   Приостанавливаем выполнение  скрипта на 5 секунд.
+    mot.setSpeed( 0.0766, MOT_M_S)              #   Запускаем мотор на скорости  0.0766 м/сек, что соответствует   60 об/мин при радиусе колеса в 12,2 мм.
+    sleep(5)                                    #   Приостанавливаем выполнение  скрипта на 5 секунд.
+    mot.setSpeed(       0, MOT_M_S)             #   Запускаем мотор на скорости       0 м/сек, что соответствует остановке мотора.
+    sleep(5)                                    #   Приостанавливаем выполнение  скрипта на 5 секунд.
+    mot.setSpeed(-0.0766, MOT_M_S)              #   Запускаем мотор на скорости -0.0766 м/сек, что соответствует  -60 об/мин при радиусе колеса в 12,2 мм.
+    sleep(5)                                    #   Приостанавливаем выполнение  скрипта на 5 секунд.
+    mot.setSpeed(-0.1532, MOT_M_S)              #   Запускаем мотор на скорости -0.1532 м/сек, что соответствует -120 об/мин при радиусе колеса в 12,2 мм.
+    sleep(5)                                    #   Приостанавливаем выполнение  скрипта на 5 секунд.
+    mot.setSpeed(-0.0766, MOT_M_S)              #   Запускаем мотор на скорости -0.0766 м/сек, что соответствует  -60 об/мин при радиусе колеса в 12,2 мм.
+    sleep(5)                                    #   Приостанавливаем выполнение  скрипта на 5 секунд.
+    mot.setSpeed(       0, MOT_M_S)             #   Запускаем мотор на скорости       0 м/сек, что соответствует остановке мотора.
+    sleep(5)                                    #   Приостанавливаем выполнение  скрипта на 5 секунд.
```

### Comparing `pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/examples/SetSpeedM_S_Stop.py` & `pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/examples/SetSpeedM_S_Stop.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-# ПРИМЕР ЗАПУСКАЕТ МОТОР С УСЛОВИЕМ ОСТАНОВКИ:   #
-                                                  #
+# ПРИМЕР ЗАПУСКАЕТ МОТОР С УСЛОВИЕМ ОСТАНОВКИ:  #
+                                                #
 from pyiArduinoI2Cmotor import *                #   Подключаем библиотеку для работы с мотором I2C-flash.
-mot = pyiArduinoI2Cmotor(0x09)                      #   Объявляем объект mot для работы с функциями и методами библиотеки pyiArduinoI2Cmotor, указывая адрес модуля на шине I2C.
-                                                  #   Если объявить объект без указания адреса (mot = pyiArduinoI2Cmotor ), то адрес будет найден автоматически.
-mot.radius = 12.2                             #   Указываем радиус колеса в мм.
-                                                  #
-while True:                                      #
-    mot.setSpeed(0.07, MOT_M_S, 0.1, MOT_MET)    #   Запускаем мотор на скорости 0.07 м/сек с остановкой мотора через 0.1 метра.
-    sleep(10)                                  #   Приостанавливаем выполнение скетча на 10 секунд.
-    mot.setSpeed(0.07, MOT_M_S,   3, MOT_REV)    #   Запускаем мотор на скорости 0.07 м/сек с остановкой мотора через 3 полных оборота.
-    sleep(10)                                  #   Приостанавливаем выполнение скетча на 10 секунд.
-    mot.setSpeed(0.07, MOT_M_S,   2, MOT_SEC)    #   Запускаем мотор на скорости 0.07 м/сек с остановкой мотора через 2 секунды.
-    sleep(10)                                  #   Приостанавливаем выполнение скетча на 10 секунд.
-}                                                 #
-
+mot = pyiArduinoI2Cmotor(0x09)                  #   Объявляем объект mot для работы с функциями и методами библиотеки pyiArduinoI2Cmotor, указывая адрес модуля на шине I2C.
+                                                #   Если объявить объект без указания адреса (mot = pyiArduinoI2Cmotor ), то адрес будет найден автоматически.
+mot.radius = 12.2                               #   Указываем радиус колеса в мм.
+                                                #
+while True:                                     #
+    mot.setSpeed(0.07, MOT_M_S, 0.1, MOT_MET)   #   Запускаем мотор на скорости 0.07 м/сек с остановкой мотора через 0.1 метра.
+    sleep(10)                                   #   Приостанавливаем выполнение скрипта на 10 секунд.
+    mot.setSpeed(0.07, MOT_M_S,   3, MOT_REV)   #   Запускаем мотор на скорости 0.07 м/сек с остановкой мотора через 3 полных оборота.
+    sleep(10)                                   #   Приостанавливаем выполнение скрипта на 10 секунд.
+    mot.setSpeed(0.07, MOT_M_S,   2, MOT_SEC)   #   Запускаем мотор на скорости 0.07 м/сек с остановкой мотора через 2 секунды.
+    sleep(10)                                   #   Приостанавливаем выполнение скрипта на 10 секунд.
```

### Comparing `pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/examples/SetSpeedPWM.py` & `pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/examples/SetSpeedPWM.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-# ДАННЫЙ ПРИМЕР ЗАПУСКАЕТ МОТОР С УКАЗАНИЕМ ШИМ: #
-                                                  #
+# ДАННЫЙ ПРИМЕР ЗАПУСКАЕТ МОТОР С УКАЗАНИЕМ ШИМ:
+
 from pyiArduinoI2Cmotor import *                #   Подключаем библиотеку для работы с мотором I2C-flash.
-mot = pyiArduinoI2Cmotor(0x09)                      #   Объявляем объект mot для работы с функциями и методами библиотеки pyiArduinoI2Cmotor, указывая адрес модуля на шине I2C.
-                                                  #   Если объявить объект без указания адреса (mot = pyiArduinoI2Cmotor ), то адрес будет найден автоматически.
-while True:                                      #
-    mot.setSpeed(  50.0, MOT_PWM)                 #   Запускаем мотор установив ШИМ =   50% (ШИМ указывается в % 0 до ±100.0).
-    sleep(5)                                   #   Приостанавливаем выполнение скетча на 5 секунд.
-    mot.setSpeed( 100.0, MOT_PWM)                 #   Запускаем мотор установив ШИМ =  100% (ШИМ указывается в % 0 до ±100.0).
-    sleep(5)                                   #   Приостанавливаем выполнение скетча на 5 секунд.
-    mot.setSpeed(  50.0, MOT_PWM)                 #   Запускаем мотор установив ШИМ =   50% (ШИМ указывается в % 0 до ±100.0).
-    sleep(5)                                   #   Приостанавливаем выполнение скетча на 5 секунд.
-    mot.setSpeed(     0, MOT_PWM)                 #   Запускаем мотор установив ШИМ =    0% что соответствует остановке мотора.
-    sleep(5)                                   #   Приостанавливаем выполнение скетча на 5 секунд.
-    mot.setSpeed( -50.0, MOT_PWM)                 #   Запускаем мотор установив ШИМ =  -50% (ШИМ указывается в % 0 до ±100.0).
-    sleep(5)                                   #   Приостанавливаем выполнение скетча на 5 секунд.
-    mot.setSpeed(-100.0, MOT_PWM)                 #   Запускаем мотор установив ШИМ = -100% (ШИМ указывается в % 0 до ±100.0).
-    sleep(5)                                   #   Приостанавливаем выполнение скетча на 5 секунд.
-    mot.setSpeed( -50.0, MOT_PWM)                 #   Запускаем мотор установив ШИМ =  -50% (ШИМ указывается в % 0 до ±100.0).
-    sleep(5)                                   #   Приостанавливаем выполнение скетча на 5 секунд.
-    mot.setSpeed(     0, MOT_PWM)                 #   Запускаем мотор установив ШИМ =    0% что соответствует остановке мотора.
-    sleep(5)                                   #   Приостанавливаем выполнение скетча на 5 секунд.
+mot = pyiArduinoI2Cmotor(0x09)                  #   Объявляем объект mot для работы с функциями и методами библиотеки pyiArduinoI2Cmotor, указывая адрес модуля на шине I2C.
+                                                #   Если объявить объект без указания адреса (mot = pyiArduinoI2Cmotor ), то адрес будет найден автоматически.
+while True:                                     #
+    mot.setSpeed(  50.0, MOT_PWM)               #   Запускаем мотор установив ШИМ =   50% (ШИМ указывается в % 0 до ±100.0).
+    sleep(5)                                    #   Приостанавливаем выполнение скрипта на 5 секунд.
+    mot.setSpeed( 100.0, MOT_PWM)               #   Запускаем мотор установив ШИМ =  100% (ШИМ указывается в % 0 до ±100.0).
+    sleep(5)                                    #   Приостанавливаем выполнение скрипта на 5 секунд.
+    mot.setSpeed(  50.0, MOT_PWM)               #   Запускаем мотор установив ШИМ =   50% (ШИМ указывается в % 0 до ±100.0).
+    sleep(5)                                    #   Приостанавливаем выполнение скрипта на 5 секунд.
+    mot.setSpeed(     0, MOT_PWM)               #   Запускаем мотор установив ШИМ =    0% что соответствует остановке мотора.
+    sleep(5)                                    #   Приостанавливаем выполнение скрипта на 5 секунд.
+    mot.setSpeed( -50.0, MOT_PWM)               #   Запускаем мотор установив ШИМ =  -50% (ШИМ указывается в % 0 до ±100.0).
+    sleep(5)                                    #   Приостанавливаем выполнение скрипта на 5 секунд.
+    mot.setSpeed(-100.0, MOT_PWM)               #   Запускаем мотор установив ШИМ = -100% (ШИМ указывается в % 0 до ±100.0).
+    sleep(5)                                    #   Приостанавливаем выполнение скрипта на 5 секунд.
+    mot.setSpeed( -50.0, MOT_PWM)               #   Запускаем мотор установив ШИМ =  -50% (ШИМ указывается в % 0 до ±100.0).
+    sleep(5)                                    #   Приостанавливаем выполнение скрипта на 5 секунд.
+    mot.setSpeed(     0, MOT_PWM)               #   Запускаем мотор установив ШИМ =    0% что соответствует остановке мотора.
+    sleep(5)                                    #   Приостанавливаем выполнение скрипта на 5 секунд.
```

### Comparing `pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/examples/SetSpeedPWM_Stop.py` & `pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/examples/SetSpeedPWM_Stop.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-# ПРИМЕР ЗАПУСКАЕТ МОТОР С УСЛОВИЕМ ОСТАНОВКИ:   #
-                                                  #
+# ПРИМЕР ЗАПУСКАЕТ МОТОР С УСЛОВИЕМ ОСТАНОВКИ:
+
 from pyiArduinoI2Cmotor import *                #   Подключаем библиотеку для работы с мотором I2C-flash.
-mot = pyiArduinoI2Cmotor(0x09)                      #   Объявляем объект mot для работы с функциями и методами библиотеки pyiArduinoI2Cmotor, указывая адрес модуля на шине I2C.
-                                                  #   Если объявить объект без указания адреса (mot = pyiArduinoI2Cmotor ), то адрес будет найден автоматически.
+mot = pyiArduinoI2Cmotor(0x09)                  #   Объявляем объект mot для работы с функциями и методами библиотеки pyiArduinoI2Cmotor, указывая адрес модуля на шине I2C.
+                                                #   Если объявить объект без указания адреса (mot = pyiArduinoI2Cmotor ), то адрес будет найден автоматически.
 mot.radius = 12.2                               #   Указываем радиус колеса в мм.
-                                                  #
-while True:                                      #
-    mot.setSpeed(50.0, MOT_PWM, 0.1, MOT_MET)     #   Запускаем мотор установив ШИМ = 50% с остановкой мотора через 0.1 метра.
-    sleep(10)                                  #   Приостанавливаем выполнение скетча на 10 секунд.
-    mot.setSpeed(50.0, MOT_PWM,   3, MOT_REV)     #   Запускаем мотор установив ШИМ = 50% с остановкой мотора через 3 полных оборота.
-    sleep(10)                                  #   Приостанавливаем выполнение скетча на 10 секунд.
-    mot.setSpeed(50.0, MOT_PWM,   2, MOT_SEC)     #   Запускаем мотор установив ШИМ = 50% с остановкой мотора через 2 секунды.
-    sleep(10)                                  #   Приостанавливаем выполнение скетча на 10 секунд.
-}                                                 #
+                                                #
+while True:                                     #
+    mot.setSpeed(50.0, MOT_PWM, 0.1, MOT_MET)   #   Запускаем мотор установив ШИМ = 50% с остановкой мотора через 0.1 метра.
+    sleep(10)                                   #   Приостанавливаем выполнение скрипта на 10 секунд.
+    mot.setSpeed(50.0, MOT_PWM,   3, MOT_REV)   #   Запускаем мотор установив ШИМ = 50% с остановкой мотора через 3 полных оборота.
+    sleep(10)                                   #   Приостанавливаем выполнение скрипта на 10 секунд.
+    mot.setSpeed(50.0, MOT_PWM,   2, MOT_SEC)   #   Запускаем мотор установив ШИМ = 50% с остановкой мотора через 2 секунды.
+    sleep(10)                                   #   Приостанавливаем выполнение скрипта на 10 секунд.
```

### Comparing `pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/examples/SetSpeedRPM.py` & `pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/examples/SetSpeedRPM.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-# ПРИМЕР ЗАПУСКАЕТ МОТОР С УКАЗАНИЕМ СКОРОСТИ:   #
-                                                  #
+# ПРИМЕР ЗАПУСКАЕТ МОТОР С УКАЗАНИЕМ СКОРОСТИ:
+
 from pyiArduinoI2Cmotor import *                #   Подключаем библиотеку для работы с мотором I2C-flash.
-mot = pyiArduinoI2Cmotor(0x09)                      #   Объявляем объект mot для работы с функциями и методами библиотеки pyiArduinoI2Cmotor, указывая адрес модуля на шине I2C.
-                                                  #   Если объявить объект без указания адреса (mot = pyiArduinoI2Cmotor ), то адрес будет найден автоматически.
-mot.begin()                                   #   Инициируем работу с мотором.
-                                                  #
-while True:                                      #
-    mot.setSpeed(  60, MOT_RPM)                   #   Запускаем мотор на скорости   60 об/мин, что соответствует 1 об/сек.
-    sleep(5)                                   #   Приостанавливаем выполнение скетча на 5 секунд.
-    mot.setSpeed( 120, MOT_RPM)                   #   Запускаем мотор на скорости  120 об/мин, что соответствует 2 об/сек.
-    sleep(5)                                   #   Приостанавливаем выполнение скетча на 5 секунд.
-    mot.setSpeed(  60, MOT_RPM)                   #   Запускаем мотор на скорости   60 об/мин, что соответствует 1 об/сек.
-    sleep(5)                                   #   Приостанавливаем выполнение скетча на 5 секунд.
-    mot.setSpeed(   0, MOT_RPM)                   #   Запускаем мотор на скорости    0 об/мин, что соответствует остановке мотора.
-    sleep(5)                                   #   Приостанавливаем выполнение скетча на 5 секунд.
-    mot.setSpeed( -60, MOT_RPM)                   #   Запускаем мотор на скорости  -60 об/мин, что соответствует -1 об/сек.
-    sleep(5)                                   #   Приостанавливаем выполнение скетча на 5 секунд.
-    mot.setSpeed(-120, MOT_RPM)                   #   Запускаем мотор на скорости -120 об/мин, что соответствует -2 об/сек.
-    sleep(5)                                   #   Приостанавливаем выполнение скетча на 5 секунд.
-    mot.setSpeed( -60, MOT_RPM)                   #   Запускаем мотор на скорости  -60 об/мин, что соответствует -1 об/сек.
-    sleep(5)                                   #   Приостанавливаем выполнение скетча на 5 секунд.
-    mot.setSpeed(   0, MOT_RPM)                   #   Запускаем мотор на скорости    0 об/мин, что соответствует остановке мотора.
-    sleep(5)                                   #   Приостанавливаем выполнение скетча на 5 секунд.
+mot = pyiArduinoI2Cmotor(0x09)                  #   Объявляем объект mot для работы с функциями и методами библиотеки pyiArduinoI2Cmotor, указывая адрес модуля на шине I2C.
+                                                #   Если объявить объект без указания адреса (mot = pyiArduinoI2Cmotor ), то адрес будет найден автоматически.
+mot.begin()                                     #   Инициируем работу с мотором.
+                                                #
+while True:                                     #
+    mot.setSpeed(  60, MOT_RPM)                 #   Запускаем мотор на скорости   60 об/мин, что соответствует 1 об/сек.
+    sleep(5)                                    #   Приостанавливаем выполнение скрипта на 5 секунд.
+    mot.setSpeed( 120, MOT_RPM)                 #   Запускаем мотор на скорости  120 об/мин, что соответствует 2 об/сек.
+    sleep(5)                                    #   Приостанавливаем выполнение скрипта на 5 секунд.
+    mot.setSpeed(  60, MOT_RPM)                 #   Запускаем мотор на скорости   60 об/мин, что соответствует 1 об/сек.
+    sleep(5)                                    #   Приостанавливаем выполнение скрипта на 5 секунд.
+    mot.setSpeed(   0, MOT_RPM)                 #   Запускаем мотор на скорости    0 об/мин, что соответствует остановке мотора.
+    sleep(5)                                    #   Приостанавливаем выполнение скрипта на 5 секунд.
+    mot.setSpeed( -60, MOT_RPM)                 #   Запускаем мотор на скорости  -60 об/мин, что соответствует -1 об/сек.
+    sleep(5)                                    #   Приостанавливаем выполнение скрипта на 5 секунд.
+    mot.setSpeed(-120, MOT_RPM)                 #   Запускаем мотор на скорости -120 об/мин, что соответствует -2 об/сек.
+    sleep(5)                                    #   Приостанавливаем выполнение скрипта на 5 секунд.
+    mot.setSpeed( -60, MOT_RPM)                 #   Запускаем мотор на скорости  -60 об/мин, что соответствует -1 об/сек.
+    sleep(5)                                    #   Приостанавливаем выполнение скрипта на 5 секунд.
+    mot.setSpeed(   0, MOT_RPM)                 #   Запускаем мотор на скорости    0 об/мин, что соответствует остановке мотора.
+    sleep(5)                                    #   Приостанавливаем выполнение скрипта на 5 секунд.
```

### Comparing `pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/examples/SetSpeedRPM_Stop.py` & `pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/examples/SetSpeedRPM_Stop.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-# ПРИМЕР ЗАПУСКАЕТ МОТОР С УСЛОВИЕМ ОСТАНОВКИ:   #
-                                                  #
+# ПРИМЕР ЗАПУСКАЕТ МОТОР С УСЛОВИЕМ ОСТАНОВКИ:
+
 from pyiArduinoI2Cmotor import *                #   Подключаем библиотеку для работы с мотором I2C-flash.
-mot = pyiArduinoI2Cmotor(0x09)                      #   Объявляем объект mot для работы с функциями и методами библиотеки pyiArduinoI2Cmotor, указывая адрес модуля на шине I2C.
-                                                  #   Если объявить объект без указания адреса (mot = pyiArduinoI2Cmotor ), то адрес будет найден автоматически.
-mot.radius = 12.2                             #   Указываем радиус колеса в мм.
-                                                  #
-while True:                                      #
-    mot.setSpeed(60, MOT_RPM, 0.1, MOT_MET)       #   Запускаем мотор на скорости 60 об/мин с остановкой мотора через 0.1 метра.
-    sleep(10)                                  #   Приостанавливаем выполнение скетча на 10 секунд.
-    mot.setSpeed(60, MOT_RPM,   3, MOT_REV)       #   Запускаем мотор на скорости 60 об/мин с остановкой мотора через 3 полных оборота.
-    sleep(10)                                  #   Приостанавливаем выполнение скетча на 10 секунд.
-    mot.setSpeed(60, MOT_RPM,   2, MOT_SEC)       #   Запускаем мотор на скорости 60 об/мин с остановкой мотора через 2 секунды.
-    sleep(10)                                  #   Приостанавливаем выполнение скетча на 10 секунд.
-}                                                 #
+mot = pyiArduinoI2Cmotor(0x09)                  #   Объявляем объект mot для работы с функциями и методами библиотеки pyiArduinoI2Cmotor, указывая адрес модуля на шине I2C.
+                                                #   Если объявить объект без указания адреса (mot = pyiArduinoI2Cmotor ), то адрес будет найден автоматически.
+mot.radius = 12.2                               #   Указываем радиус колеса в мм.
+                                                #
+while True:                                     #
+    mot.setSpeed(60, MOT_RPM, 0.1, MOT_MET)     #   Запускаем мотор на скорости 60 об/мин с остановкой мотора через 0.1 метра.
+    sleep(10)                                   #   Приостанавливаем выполнение скрипта на 10 секунд.
+    mot.setSpeed(60, MOT_RPM,   3, MOT_REV)     #   Запускаем мотор на скорости 60 об/мин с остановкой мотора через 3 полных оборота.
+    sleep(10)                                   #   Приостанавливаем выполнение скрипта на 10 секунд.
+    mot.setSpeed(60, MOT_RPM,   2, MOT_SEC)     #   Запускаем мотор на скорости 60 об/мин с остановкой мотора через 2 секунды.
+    sleep(10)                                   #   Приостанавливаем выполнение скрипта на 10 секунд.
```

### Comparing `pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/examples/SetStopNeutral.py` & `pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/examples/SetStopNeutral.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/examples/newAddress.py` & `pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/examples/newAddress.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/iarduino_I2C_Motor.cpp` & `pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/iarduino_I2C_Motor.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/iarduino_I2C_Motor.h` & `pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/iarduino_I2C_Motor.h`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/iarduino_I2C_Motor.pxd` & `pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/iarduino_I2C_Motor.pxd`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/iarduino_I2C_PI.h` & `pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/iarduino_I2C_PI.h`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cmotor-0.0.2/pyiArduinoI2Cmotor/pyiArduinoI2Cmotor.pyx` & `pyiArduinoI2Cmotor-0.0.4/pyiArduinoI2Cmotor/pyiArduinoI2Cmotor.pyx`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cmotor-0.0.2/setup.py` & `pyiArduinoI2Cmotor-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from distutils.extension import Extension
 
 def readme():
     with open('README.md') as readme:
         return readme.read()
 
 setup(name='pyiArduinoI2Cmotor',
-    version='0.0.2',
+    version='0.0.4',
     description='iarduino.ru module for Raspberry Pi',
     long_description=readme(),
     classifiers=[
         'Programming Language :: Python :: 3',
     ],
     url='http://github.com/tremaru/pyiArduinoI2Cmotor',
     author='iarduino.ru',
```

