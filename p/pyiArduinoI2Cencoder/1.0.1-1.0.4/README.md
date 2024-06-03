# Comparing `tmp/pyiArduinoI2Cencoder-1.0.1.tar.gz` & `tmp/pyiArduinoI2Cencoder-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyiArduinoI2Cencoder-1.0.1.tar", last modified: Fri Feb 14 11:28:22 2020, max compression
+gzip compressed data, was "pyiArduinoI2Cencoder-1.0.4.tar", last modified: Mon Jun  3 11:54:51 2024, max compression
```

## Comparing `pyiArduinoI2Cencoder-1.0.1.tar` & `pyiArduinoI2Cencoder-1.0.4.tar`

### file list

```diff
@@ -1,61 +1,69 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2020-02-14 11:28:22.000000 pyiArduinoI2Cencoder-1.0.1/
--rw-r--r--   0 pi        (1000) pi        (1000)     2451 2020-02-14 11:28:22.000000 pyiArduinoI2Cencoder-1.0.1/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)       23 2020-02-12 08:39:23.000000 pyiArduinoI2Cencoder-1.0.1/README
--rw-r--r--   0 pi        (1000) pi        (1000)     1884 2020-02-12 08:39:23.000000 pyiArduinoI2Cencoder-1.0.1/README.md
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2020-02-14 11:28:22.000000 pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/
--rw-r--r--   0 pi        (1000) pi        (1000)       30 2020-02-12 08:39:23.000000 pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/__init__.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2020-02-14 11:28:22.000000 pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/cpp/
--rw-------   0 pi        (1000) pi        (1000)      850 2020-02-13 09:32:48.000000 pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/cpp/EncTurn.cpp
--rw-------   0 pi        (1000) pi        (1000)     1152 2020-02-13 09:50:08.000000 pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/cpp/EncTurnLeftRight.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)     9696 2020-02-13 09:51:49.000000 pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/cpp/FindDevices.cpp
--rw-------   0 pi        (1000) pi        (1000)      868 2020-02-13 09:54:18.000000 pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/cpp/KeyChanged.cpp
--rw-------   0 pi        (1000) pi        (1000)     1278 2020-02-13 09:58:53.000000 pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/cpp/KeyHold.cpp
--rw-------   0 pi        (1000) pi        (1000)      738 2020-02-13 09:32:48.000000 pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/cpp/KeyPressed.cpp
--rw-------   0 pi        (1000) pi        (1000)      922 2020-02-13 09:55:05.000000 pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/cpp/KeyPushed.cpp
--rw-------   0 pi        (1000) pi        (1000)      995 2020-02-13 09:32:48.000000 pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/cpp/KeyReleased.cpp
--rw-------   0 pi        (1000) pi        (1000)      910 2020-02-13 09:32:48.000000 pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/cpp/KeyTimePressed.cpp
--rw-------   0 pi        (1000) pi        (1000)      855 2020-02-13 09:32:48.000000 pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/cpp/KeyTrigger.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)     1496 2020-02-13 09:32:48.000000 pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/cpp/NewAddress.cpp
--rw-------   0 pi        (1000) pi        (1000)      949 2020-02-13 12:22:32.000000 pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/cpp/PinModeDAC.cpp
--rw-------   0 pi        (1000) pi        (1000)      997 2020-02-13 10:09:15.000000 pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/cpp/PinModeFrequency.cpp
--rw-------   0 pi        (1000) pi        (1000)      784 2020-02-13 10:19:14.000000 pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/cpp/PinModeKey.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)      729 2020-02-13 10:24:14.000000 pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/cpp/PinModeOff.cpp
--rw-------   0 pi        (1000) pi        (1000)     1017 2020-02-13 10:30:17.000000 pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/cpp/PinModePWM.cpp
--rw-------   0 pi        (1000) pi        (1000)     1260 2020-02-13 12:05:54.000000 pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/cpp/PinModePWMlog.cpp
--rw-------   0 pi        (1000) pi        (1000)     1375 2020-02-13 12:14:35.000000 pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/cpp/PinModeServo.cpp
--rw-------   0 pi        (1000) pi        (1000)      837 2020-02-13 12:24:54.000000 pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/cpp/PinModeTrigger.cpp
--rw-------   0 pi        (1000) pi        (1000)      961 2020-02-13 12:45:09.000000 pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/cpp/PositionGet.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)      869 2020-02-13 13:13:02.000000 pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/cpp/PositionReset.cpp
--rw-------   0 pi        (1000) pi        (1000)      844 2020-02-13 13:20:56.000000 pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/cpp/PositionSettings.cpp
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2020-02-14 11:28:22.000000 pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/examples/
--rw-r--r--   0 pi        (1000) pi        (1000)      734 2020-02-13 13:43:17.000000 pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/examples/EncTurn.py
--rw-r--r--   0 pi        (1000) pi        (1000)     1196 2020-02-13 13:43:45.000000 pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/examples/EncTurnLeftRight.py
--rw-r--r--   0 pi        (1000) pi        (1000)     5580 2020-02-13 10:00:30.000000 pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/examples/FindDevices.py
--rw-r--r--   0 pi        (1000) pi        (1000)      833 2020-02-13 13:44:24.000000 pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/examples/KeyChanged.py
--rw-r--r--   0 pi        (1000) pi        (1000)      954 2020-02-13 13:45:32.000000 pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/examples/KeyHold.py
--rw-r--r--   0 pi        (1000) pi        (1000)      646 2020-02-13 09:35:53.000000 pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/examples/KeyPressed.py
--rw-r--r--   0 pi        (1000) pi        (1000)      796 2020-02-13 13:46:17.000000 pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/examples/KeyPushed.py
--rw-r--r--   0 pi        (1000) pi        (1000)      743 2020-02-13 13:46:59.000000 pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/examples/KeyReleased.py
--rw-r--r--   0 pi        (1000) pi        (1000)      819 2020-02-13 13:49:36.000000 pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/examples/KeyTimePressed.py
--rw-r--r--   0 pi        (1000) pi        (1000)      741 2020-02-13 09:34:03.000000 pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/examples/KeyTrigger.py
--rw-r--r--   0 pi        (1000) pi        (1000)      871 2020-02-13 09:34:03.000000 pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/examples/PinModeDAC.py
--rw-r--r--   0 pi        (1000) pi        (1000)      917 2020-02-13 10:12:27.000000 pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/examples/PinModeFrequency.py
--rw-r--r--   0 pi        (1000) pi        (1000)      745 2020-02-13 10:21:36.000000 pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/examples/PinModeKey.py
--rw-r--r--   0 pi        (1000) pi        (1000)      690 2020-02-13 10:26:17.000000 pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/examples/PinModeOff.py
--rw-r--r--   0 pi        (1000) pi        (1000)      944 2020-02-13 10:32:41.000000 pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/examples/PinModePWM.py
--rw-r--r--   0 pi        (1000) pi        (1000)     1191 2020-02-13 12:05:36.000000 pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/examples/PinModePWMlog.py
--rw-r--r--   0 pi        (1000) pi        (1000)     1301 2020-02-13 12:21:39.000000 pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/examples/PinModeServo.py
--rw-r--r--   0 pi        (1000) pi        (1000)      782 2020-02-13 12:26:46.000000 pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/examples/PinModeTrigger.py
--rw-r--r--   0 pi        (1000) pi        (1000)      923 2020-02-13 13:51:01.000000 pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/examples/PositionGet.py
--rw-r--r--   0 pi        (1000) pi        (1000)      920 2020-02-13 17:23:02.000000 pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/examples/PositionReset.py
--rw-r--r--   0 pi        (1000) pi        (1000)      767 2020-02-13 13:34:03.000000 pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/examples/PositionSettings.py
--rw-r--r--   0 pi        (1000) pi        (1000)     1400 2020-02-13 14:29:58.000000 pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/examples/newAddress.py
--rwx------   0 pi        (1000) pi        (1000)    40567 2020-02-13 14:01:18.000000 pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/iarduino_I2C_Encoder.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)    42370 2020-02-12 12:33:35.000000 pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/iarduino_I2C_Encoder.h
--rw-r--r--   0 pi        (1000) pi        (1000)      831 2020-02-12 12:33:02.000000 pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/iarduino_I2C_Encoder.pxd
--rwxr-xr-x   0 pi        (1000) pi        (1000)     9051 2020-02-14 08:52:54.000000 pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/iarduino_I2C_PI.h
--rw-r--r--   0 pi        (1000) pi        (1000)   282955 2020-02-14 11:25:18.000000 pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/pyiArduinoI2Cencoder.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)     5478 2020-02-14 11:24:58.000000 pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/pyiArduinoI2Cencoder.pyx
--rw-r--r--   0 pi        (1000) pi        (1000)      133 2020-02-12 08:39:23.000000 pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/setup.py
--rw-r--r--   0 pi        (1000) pi        (1000)       40 2020-02-12 08:39:23.000000 pyiArduinoI2Cencoder-1.0.1/setup.cfg
--rw-r--r--   0 pi        (1000) pi        (1000)      728 2020-02-14 11:27:29.000000 pyiArduinoI2Cencoder-1.0.1/setup.py
+drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-06-03 11:54:51.562069 pyiArduinoI2Cencoder-1.0.4/
+-rw-r--r--   0 dron      (1000) dron      (1000)     3291 2024-03-29 13:35:22.000000 pyiArduinoI2Cencoder-1.0.4/LICENSE
+-rw-r--r--   0 dron      (1000) dron      (1000)       85 2024-03-29 13:35:22.000000 pyiArduinoI2Cencoder-1.0.4/MANIFEST.in
+-rw-r--r--   0 dron      (1000) dron      (1000)     2186 2024-06-03 11:54:51.562069 pyiArduinoI2Cencoder-1.0.4/PKG-INFO
+-rw-r--r--   0 dron      (1000) dron      (1000)       23 2024-03-29 13:35:22.000000 pyiArduinoI2Cencoder-1.0.4/README
+-rw-r--r--   0 dron      (1000) dron      (1000)     1884 2024-03-29 13:35:22.000000 pyiArduinoI2Cencoder-1.0.4/README.md
+drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-06-03 11:54:51.534070 pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/
+-rw-r--r--   0 dron      (1000) dron      (1000)       30 2024-03-29 13:35:22.000000 pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/__init__.py
+drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-06-03 11:54:51.550069 pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/cpp/
+-rw-r--r--   0 dron      (1000) dron      (1000)      850 2024-03-29 13:35:22.000000 pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/cpp/EncTurn.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     1152 2024-03-29 13:35:22.000000 pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/cpp/EncTurnLeftRight.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     9696 2024-03-29 13:35:22.000000 pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/cpp/FindDevices.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)      868 2024-03-29 13:35:22.000000 pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/cpp/KeyChanged.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     1278 2024-03-29 13:35:22.000000 pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/cpp/KeyHold.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)      738 2024-03-29 13:35:22.000000 pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/cpp/KeyPressed.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)      922 2024-03-29 13:35:22.000000 pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/cpp/KeyPushed.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)      995 2024-03-29 13:35:22.000000 pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/cpp/KeyReleased.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)      910 2024-03-29 13:35:22.000000 pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/cpp/KeyTimePressed.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)      855 2024-03-29 13:35:22.000000 pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/cpp/KeyTrigger.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     1496 2024-03-29 13:35:22.000000 pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/cpp/NewAddress.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)      949 2024-03-29 13:35:22.000000 pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/cpp/PinModeDAC.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)      997 2024-03-29 13:35:22.000000 pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/cpp/PinModeFrequency.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)      784 2024-03-29 13:35:22.000000 pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/cpp/PinModeKey.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)      729 2024-03-29 13:35:22.000000 pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/cpp/PinModeOff.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     1017 2024-03-29 13:35:22.000000 pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/cpp/PinModePWM.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     1260 2024-03-29 13:35:22.000000 pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/cpp/PinModePWMlog.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     1375 2024-03-29 13:35:22.000000 pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/cpp/PinModeServo.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)      837 2024-03-29 13:35:22.000000 pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/cpp/PinModeTrigger.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)      961 2024-03-29 13:35:22.000000 pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/cpp/PositionGet.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)      869 2024-03-29 13:35:22.000000 pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/cpp/PositionReset.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)      844 2024-03-29 13:35:22.000000 pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/cpp/PositionSettings.cpp
+drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-06-03 11:54:51.562069 pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/examples/
+-rw-r--r--   0 dron      (1000) dron      (1000)      732 2024-03-29 13:35:22.000000 pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/examples/EncTurn.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     1194 2024-03-29 13:35:22.000000 pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/examples/EncTurnLeftRight.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     5580 2024-03-29 13:35:22.000000 pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/examples/FindDevices.py
+-rw-r--r--   0 dron      (1000) dron      (1000)      831 2024-03-29 13:35:22.000000 pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/examples/KeyChanged.py
+-rw-r--r--   0 dron      (1000) dron      (1000)      952 2024-03-29 13:35:22.000000 pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/examples/KeyHold.py
+-rw-r--r--   0 dron      (1000) dron      (1000)      644 2024-03-29 13:35:22.000000 pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/examples/KeyPressed.py
+-rw-r--r--   0 dron      (1000) dron      (1000)      794 2024-03-29 13:35:22.000000 pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/examples/KeyPushed.py
+-rw-r--r--   0 dron      (1000) dron      (1000)      741 2024-03-29 13:35:22.000000 pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/examples/KeyReleased.py
+-rw-r--r--   0 dron      (1000) dron      (1000)      817 2024-03-29 13:35:22.000000 pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/examples/KeyTimePressed.py
+-rw-r--r--   0 dron      (1000) dron      (1000)      739 2024-03-29 13:35:22.000000 pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/examples/KeyTrigger.py
+-rw-r--r--   0 dron      (1000) dron      (1000)      797 2024-03-29 13:35:22.000000 pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/examples/PinModeDAC.py
+-rw-r--r--   0 dron      (1000) dron      (1000)      843 2024-03-29 13:35:22.000000 pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/examples/PinModeFrequency.py
+-rw-r--r--   0 dron      (1000) dron      (1000)      668 2024-03-29 13:35:22.000000 pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/examples/PinModeKey.py
+-rw-r--r--   0 dron      (1000) dron      (1000)      613 2024-03-29 13:35:22.000000 pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/examples/PinModeOff.py
+-rw-r--r--   0 dron      (1000) dron      (1000)      867 2024-03-29 13:35:22.000000 pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/examples/PinModePWM.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     1114 2024-03-29 13:35:22.000000 pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/examples/PinModePWMlog.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     1224 2024-03-29 13:35:22.000000 pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/examples/PinModeServo.py
+-rw-r--r--   0 dron      (1000) dron      (1000)      705 2024-03-29 13:35:22.000000 pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/examples/PinModeTrigger.py
+-rw-r--r--   0 dron      (1000) dron      (1000)      846 2024-03-29 13:35:22.000000 pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/examples/PositionGet.py
+-rw-r--r--   0 dron      (1000) dron      (1000)      918 2024-03-29 13:35:22.000000 pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/examples/PositionReset.py
+-rw-r--r--   0 dron      (1000) dron      (1000)      692 2024-03-29 13:35:22.000000 pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/examples/PositionSettings.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     2638 2024-03-29 13:35:22.000000 pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/examples/ServoCalProc.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     1398 2024-03-29 13:35:22.000000 pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/examples/newAddress.py
+-rwxr-xr-x   0 dron      (1000) dron      (1000)    40567 2024-03-29 13:35:22.000000 pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/iarduino_I2C_Encoder.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)    42370 2024-03-29 13:35:22.000000 pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/iarduino_I2C_Encoder.h
+-rw-r--r--   0 dron      (1000) dron      (1000)      831 2024-03-29 13:35:22.000000 pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/iarduino_I2C_Encoder.pxd
+-rwxr-xr-x   0 dron      (1000) dron      (1000)     9051 2024-03-29 13:35:22.000000 pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/iarduino_I2C_PI.h
+-rw-r--r--   0 dron      (1000) dron      (1000)   557650 2024-06-03 11:47:48.000000 pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/pyiArduinoI2Cencoder.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     5478 2024-03-29 13:35:22.000000 pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/pyiArduinoI2Cencoder.pyx
+-rw-r--r--   0 dron      (1000) dron      (1000)      133 2024-03-29 13:35:22.000000 pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/setup.py
+drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-06-03 11:54:51.538070 pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder.egg-info/
+-rw-r--r--   0 dron      (1000) dron      (1000)     2186 2024-06-03 11:54:51.000000 pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder.egg-info/PKG-INFO
+-rw-r--r--   0 dron      (1000) dron      (1000)     2515 2024-06-03 11:54:51.000000 pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder.egg-info/SOURCES.txt
+-rw-r--r--   0 dron      (1000) dron      (1000)        1 2024-06-03 11:54:51.000000 pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder.egg-info/dependency_links.txt
+-rw-r--r--   0 dron      (1000) dron      (1000)       21 2024-06-03 11:54:51.000000 pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder.egg-info/top_level.txt
+-rw-r--r--   0 dron      (1000) dron      (1000)       79 2024-06-03 11:54:51.562069 pyiArduinoI2Cencoder-1.0.4/setup.cfg
+-rw-r--r--   0 dron      (1000) dron      (1000)      728 2024-06-03 11:51:46.000000 pyiArduinoI2Cencoder-1.0.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyiArduinoI2Cencoder-1.0.1/PKG-INFO` & `pyiArduinoI2Cencoder-1.0.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pyiArduinoI2Cencoder
-Version: 1.0.1
+Version: 1.0.4
 Summary: iarduino.ru module for Raspberry Pi
 Home-page: http://github.com/tremaru/pyiArduinoI2Cencoder
 Author: iarduino.ru
 Author-email: shop@iarduino.ru
 License: MIT
-Description: [![](https://iarduino.ru/img/logo.svg)](https://iarduino.ru)[![](https://wiki.iarduino.ru/img/git-shop.svg?3)](https://iarduino.ru) [![](https://wiki.iarduino.ru/img/git-wiki.svg?2)](https://wiki.iarduino.ru) [![](https://wiki.iarduino.ru/img/git-lesson.svg?2)](https://lesson.iarduino.ru)[![](https://wiki.iarduino.ru/img/git-forum.svg?2)](http://forum.trema.ru)
-        
-        # pyiArduinoI2Cencoder
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
-        `sudo pip3 install pyiArduinoI2Cencoder`
-        
-        Самостоятельная сборка из исходников:
-        
-        `git clone https://github.com/tremaru/pyiArduinoI2Cencoder.git && cd pyiArduinoI2Cencoder/pyiArduinoI2Cencoder && python3 setup.py build_ext --inplace`
-        
-        Примеры для Python находятся в папке `pyiArduinoI2Cencoder/examples`
-        
-        Примеры для С++ находятся в папке `pyiArduinoI2Cencoder/cpp`. Так же в этой папке лежит *Makefile* для сборки
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
+# pyiArduinoI2Cencoder
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
+`sudo pip3 install pyiArduinoI2Cencoder`
+
+Самостоятельная сборка из исходников:
+
+`git clone https://github.com/tremaru/pyiArduinoI2Cencoder.git && cd pyiArduinoI2Cencoder/pyiArduinoI2Cencoder && python3 setup.py build_ext --inplace`
+
+Примеры для Python находятся в папке `pyiArduinoI2Cencoder/examples`
+
+Примеры для С++ находятся в папке `pyiArduinoI2Cencoder/cpp`. Так же в этой папке лежит *Makefile* для сборки
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

### Comparing `pyiArduinoI2Cencoder-1.0.1/README.md` & `pyiArduinoI2Cencoder-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/cpp/EncTurn.cpp` & `pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/cpp/EncTurn.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/cpp/EncTurnLeftRight.cpp` & `pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/cpp/EncTurnLeftRight.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/cpp/FindDevices.cpp` & `pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/cpp/FindDevices.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/cpp/KeyChanged.cpp` & `pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/cpp/KeyChanged.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/cpp/KeyHold.cpp` & `pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/cpp/KeyHold.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/cpp/KeyPressed.cpp` & `pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/cpp/KeyPressed.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/cpp/KeyPushed.cpp` & `pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/cpp/KeyPushed.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/cpp/KeyReleased.cpp` & `pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/cpp/KeyReleased.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/cpp/KeyTimePressed.cpp` & `pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/cpp/KeyTimePressed.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/cpp/KeyTrigger.cpp` & `pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/cpp/KeyTrigger.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/cpp/NewAddress.cpp` & `pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/cpp/NewAddress.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/cpp/PinModeDAC.cpp` & `pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/cpp/PinModeDAC.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/cpp/PinModeFrequency.cpp` & `pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/cpp/PinModeFrequency.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/cpp/PinModeKey.cpp` & `pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/cpp/PinModeKey.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/cpp/PinModeOff.cpp` & `pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/cpp/PinModeOff.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/cpp/PinModePWM.cpp` & `pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/cpp/PinModePWM.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/cpp/PinModePWMlog.cpp` & `pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/cpp/PinModePWMlog.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/cpp/PinModeServo.cpp` & `pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/cpp/PinModeServo.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/cpp/PinModeTrigger.cpp` & `pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/cpp/PinModeTrigger.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/cpp/PositionGet.cpp` & `pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/cpp/PositionGet.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/cpp/PositionReset.cpp` & `pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/cpp/PositionReset.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/cpp/PositionSettings.cpp` & `pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/cpp/PositionSettings.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/examples/EncTurn.py` & `pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/examples/EncTurn.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # ПРИМЕР ЧТЕНИЯ ТАКТОВ ПОВОРОТА ЭНКОДЕРА:
 
 from time import sleep
 
 # Подключаем библиотеку для работы с энкодером I2C-flash.
 from pyiArduinoI2Cencoder import *
-# Инстанциируем объект, указывая адрес модуля на шине I2C.
+# Инстанцируем объект, указывая адрес модуля на шине I2C.
 enc = pyiArduinoI2Cencoder(0x09)
 
 print("Вращайте барабан!")
 
 while True:
     # Считываем такты поворота энкодера:
     turn = enc.getEncoder(ENC_TURN)
```

### Comparing `pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/examples/EncTurnLeftRight.py` & `pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/examples/EncTurnLeftRight.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # В данном примере считываются такты поворотов энкодера,
 # отдельно вправо и отдельно влево.
 
 from time import sleep
 
 # Подключаем библиотеку для работы с энкодером I2C-flash.
 from pyiArduinoI2Cencoder import *
-# Инстанциируем объект, указывая адрес модуля на шине I2C.
+# Инстанцируем объект, указывая адрес модуля на шине I2C.
 enc = pyiArduinoI2Cencoder(0x09)
 
 print("Вращайте барабан!")
 
 while True:
 
     # Определяем переменные для чтения количества тактов поворота энкодера.
```

### Comparing `pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/examples/FindDevices.py` & `pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/examples/FindDevices.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/examples/KeyChanged.py` & `pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/examples/KeyChanged.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # В stdout будет выводится сообщения при
 # каждом нажатии и отпускании кнопки.
 
 from time import sleep
 
 # Подключаем библиотеку для работы с энкодером I2C-flash.
 from pyiArduinoI2Cencoder import *
-# Инстанциируем объект, указывая адрес модуля на шине I2C.
+# Инстанцируем объект, указывая адрес модуля на шине I2C.
 enc = pyiArduinoI2Cencoder(0x09)
 
 print("Нажмите на вал")
 
 while True:
     # Фиксируем смену состояния кнопки:
     # Если состояние кнопки изменилось, то ...
```

### Comparing `pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/examples/KeyHold.py` & `pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/examples/KeyHold.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Если кнопка удерживается дольше фиксированного времени,
 # в stdout выводится "ON".
 
 from time import sleep
 
 # Подключаем библиотеку для работы с энкодером I2C-flash.
 from pyiArduinoI2Cencoder import *
-# Инстанциируем объект, указывая адрес модуля на шине I2C.
+# Инстанцируем объект, указывая адрес модуля на шине I2C.
 enc = pyiArduinoI2Cencoder(0x09)
 
 print("Удерживайте кноку вала")
 
 while True:
     # f = enc.getButton(KEY_HOLD_05)  # Считываем удержание дольше 0,5 сек
     f = enc.getButton(KEY_HOLD_10)    # Считываем удержание дольше 1,0 сек
```

### Comparing `pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/examples/KeyPressed.py` & `pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/examples/KeyPressed.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #   ПРИМЕР РАБОТЫ С КНОПКОЙ ЭНКОДЕРА:
 # В stdout выводится состояние кнопки
 # энкодера на момент запуска сценария
 
 # Подключаем библиотеку для работы с энкодером I2C-flash.
 from pyiArduinoI2Cencoder import *
-# Инстанциируем объект, указывая адрес модуля на шине I2C.
+# Инстанцируем объект, указывая адрес модуля на шине I2C.
 enc = pyiArduinoI2Cencoder(0x09)
 
 # Считываем состояние кнопки энкодера в переменную f.
 f = enc.getButton(KEY_PRESSED)
 
 if not f:
     print("OFF")
```

### Comparing `pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/examples/KeyPushed.py` & `pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/examples/KeyPushed.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #   ДАННЫЙ ПРИМЕР ФИКСИРУЕТ НАЖАТИЕ КНОПКИ:
 # При каждом нажатии кнопки, будет выводится
 # сообщение в stdout
 
 from time import sleep
 # Подключаем библиотеку для работы с энкодером I2C-flash.
 from pyiArduinoI2Cencoder import *
-# Инстанциируем объект, указывая адрес модуля на шине I2C.
+# Инстанцируем объект, указывая адрес модуля на шине I2C.
 enc = pyiArduinoI2Cencoder(0x09)
 
 print("Нажмите на вал")
 
 while True:
     #  Фиксируем событие нажатия кнопки:
     # Если кнопка энкодера нажимается, то ...
```

### Comparing `pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/examples/KeyReleased.py` & `pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/examples/KeyReleased.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #   ДАННЫЙ ПРИМЕР ФИКСИРУЕТ ОТПУСКАНИЕ КНОПКИ:
 # При каждом отпускании кнопки, будет выводится
 # сообщение в stdout
 
 from time import sleep
 # Подключаем библиотеку для работы с энкодером I2C-flash.
 from pyiArduinoI2Cencoder import *
-# Инстанциируем объект, указывая адрес модуля на шине I2C.
+# Инстанцируем объект, указывая адрес модуля на шине I2C.
 enc = pyiArduinoI2Cencoder(0x09)
 
 print("Нажмите на вал")
 
 while True:
 
     # Если кнопка энкодера отпускается, то ...
```

### Comparing `pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/examples/KeyTimePressed.py` & `pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/examples/KeyTimePressed.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #   ДАННЫЙ ПРИМЕР ФИКСИРУЕТ УДЕРЖАНИЕ КНОПКИ:
 # В stdout будет вывоится время удержания кнопки
 
 from time import sleep
 # Подключаем библиотеку для работы с энкодером I2C-flash.
 from pyiArduinoI2Cencoder import *
 
-# Инстанциируем объект, указывая адрес модуля на шине I2C.
+# Инстанцируем объект, указывая адрес модуля на шине I2C.
 enc = pyiArduinoI2Cencoder(0x09)
 
 print("Удерживайте вал нажатым")
 
 while True:
     # Считываем время удержания кнопки (в миллисекундах)
     # Максимально фиксируемое время удержания: 25,5 секунд.
```

### Comparing `pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/examples/KeyTrigger.py` & `pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/examples/KeyTrigger.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #   ПРИМЕР РАБОТЫ С КНОПОЧНЫМ ПЕРЕКЛЮЧАТЕЛЕМ:
 # При каждом нажатии на кнопку булева переменная
 # будет менять своё значение на противоположное
 
 from time import sleep
 # Подключаем библиотеку для работы с энкодером I2C-flash.
 from pyiArduinoI2Cencoder import *
-# Инстанциируем объект, указывая адрес модуля на шине I2C.
+# Инстанцируем объект, указывая адрес модуля на шине I2C.
 enc = pyiArduinoI2Cencoder(0x09)
 
 while True:
     # Считываем состояние кнопочного переключателя энкодера
     t = bool(enc.getButton(KEY_TRIGGER))
     print(t)
     sleep(.1)
```

### Comparing `pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/examples/PinModeDAC.py` & `pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/examples/PinModeDAC.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 #   ПРИМЕР НАСТРОЙКИ ВЫХОДА В АНАЛОГОВЫЙ РЕЖИМ:
 # Режимы работы выхода модуля энергонезависимы
 # (сохраняются и после отключения питания).
 
 # Подключаем библиотеку для работы с энкодером I2C-flash.
 from pyiArduinoI2Cencoder import *
 
-# Инстанциируем объект, указывая адрес модуля на шине I2C.
+# Инстанцируем объект, указывая адрес модуля на шине I2C.
 enc = pyiArduinoI2Cencoder(0x09)
 
-# Инициируем работу с энкодером.
-enc.begin()
-
 # Указываем выводу модуля работать как аналоговый выход,
 # напряжение которого меняется от 0 до 3.3В
 # за 2 полных оборота вала энкодера.
 enc.setPinOut(ENC_PIN_MODE_DAC, 2)
```

### Comparing `pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/examples/PinModeFrequency.py` & `pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/examples/PinModeFrequency.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 # НАСТРОЙКА ВЫХОДА В ШИМ С УКАЗАННОЙ ЧАСТОТОЙ:
 # Режимы работы выхода модуля энергонезависимы
 # (сохраняются и после отключения питания).
 
 # Подключаем библиотеку для работы с энкодером I2C-flash.
 from pyiArduinoI2Cencoder import *
 
-# Инстанциируем объект, указывая адрес модуля на шине I2C.
+# Инстанцируем объект, указывая адрес модуля на шине I2C.
 enc = pyiArduinoI2Cencoder(0x09)
 
-# Инициируем работу с энкодером.
-enc.begin()
-
 # Указываем выводу модуля работать как выход с ШИМ на частоте 5 кГц,
 # коэффициент заполнения которого меняется от 0% до 100%
 # за 3 полных оборота вала энкодера.
 enc.setPinOut(ENC_PIN_MODE_PWM, 3, 5000)
```

### Comparing `pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/examples/PinModeKey.py` & `pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/examples/PositionGet.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,25 @@
-#   ПРИМЕР НАСТРОЙКИ ВЫХОДА В РЕЖИМ КНОПКИ:
-# Режимы работы выхода модуля энергонезависимы
-# (сохраняются и после отключения питания).
+#   ПРИМЕР ЧТЕНИЯ ТЕКУЩЕЙ ПОЗИЦИИ ВАЛА ЭНКОДЕРА:
+# Зная точную позицию Вала энкодера, работа
+# с модулем похожа на работу с потенциометром.
+
+from time import sleep
 
 # Подключаем библиотеку для работы с энкодером I2C-flash.
 from pyiArduinoI2Cencoder import *
 
-# Инстанциируем объект, указывая адрес модуля на шине I2C.
+# Инстанцируем объект, указывая адрес модуля на шине I2C.
 enc = pyiArduinoI2Cencoder(0x09)
 
-# Инициируем работу с энкодером.
-enc.begin()
+# Указываем считать до 2 полных оборотов.
+enc.setPosSettings(2)
+
+print("Вращайте вал!")
+
+while True:
+
+    p = enc.getPosition()
+    # Выводим текущую позицию вала энкодера.
+    print(p)
+
+    sleep(.5)
 
-# Указываем выводу модуля работать как выход кнопки энкодера.
-enc.setPinOut(ENC_PIN_MODE_KEY)
```

### Comparing `pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/examples/PinModePWM.py` & `pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/examples/PinModePWM.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 # ПРИМЕР НАСТРОЙКИ ВЫХОДА В РЕЖИМ ШИМ:
 # Режимы работы выхода модуля энергонезависимы
 # (сохраняются и после отключения питания).
 
 # Подключаем библиотеку для работы с энкодером I2C-flash.
 from pyiArduinoI2Cencoder import *
 
-# Инстанциируем объект, указывая адрес модуля на шине I2C.
+# Инстанцируем объект, указывая адрес модуля на шине I2C.
 enc = pyiArduinoI2Cencoder(0x09)
 
 # Инициируем работу с энкодером.
-enc.begin()
-
-# Инициируем работу с энкодером.
 # Указываем выводу модуля работать как выход с ШИМ,
 # коэффициент заполнения которого меняется от 0% до 100%
 # за 2 полных оборота вала энкодера.
 enc.setPinOut(ENC_PIN_MODE_PWM, 2)
```

### Comparing `pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/examples/PinModePWMlog.py` & `pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/examples/PinModePWMlog.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,18 +2,15 @@
 # Режимы работы выхода модуля энергонезависимы
 # (сохраняются и после отключения питания).
 # Логарифмический ШИМ лучше подходит для управления
 # светодиодами, чем обычный (линейный) ШИМ.
 
 # Подключаем библиотеку для работы с энкодером I2C-flash.
 from pyiArduinoI2Cencoder import *
-# Инстанциируем объект, указывая адрес модуля на шине I2C.
+# Инстанцируем объект, указывая адрес модуля на шине I2C.
 enc = pyiArduinoI2Cencoder(0x09)
 
-# Инициируем работу с энкодером.
-enc.begin()
-
 #   Инициируем работу с энкодером.
 #   Указываем выводу модуля работать как выход с логарифмической ШИМ,
 #   коэффициент заполнения которого меняется от 0% до 100%
 #   за 2 полных оборота вала энкодера.
 enc.setPinOut(ENC_PIN_MODE_PWM_LOG, 2)
```

### Comparing `pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/examples/PinModeServo.py` & `pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/examples/PinModeServo.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 #   ПРИМЕР НАСТРОЙКИ ВЫХОДА В РЕЖИМ СЕРВО:
 # Режимы работы выхода модуля энергонезависимы
 # (сохраняются и после отключения питания).
 
 # Подключаем библиотеку для работы с энкодером I2C-flash.
 from pyiArduinoI2Cencoder import *
 
-# Инстанциируем объект, указывая адрес модуля на шине I2C.
+# Инстанцируем объект, указывая адрес модуля на шине I2C.
 enc = pyiArduinoI2Cencoder(0x09)
 
-# Инициируем работу с энкодером.
-enc.begin()
-
 """Задаём границы поворота сервопривода, указав ширину
 импульсов в мкс для минимального и максимального угла.
 Как найти ширину импульсов для функции setServoLimit()
 рассказано в примере "Установка ограничений поворота вала сервопривода"
 на странице https://wiki.iarduino.ru/page/potentiometer-i2c/i"""
 # enc.setServoLimit(450, 2450)
```

### Comparing `pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/examples/PinModeTrigger.py` & `pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/examples/PinModeTrigger.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 #   ПРИМЕР НАСТРОЙКИ ВЫХОДА В РЕЖИМ ПЕРЕКЛЮЧАТЕЛ:
 # Режимы работы выхода модуля энергонезависимы
 # (сохраняются и после отключения питания).
 
 # Подключаем библиотеку для работы с энкодером I2C-flash.
 from pyiArduinoI2Cencoder import *
 
-# Инстанциируем объект, указывая адрес модуля на шине I2C.
+# Инстанцируем объект, указывая адрес модуля на шине I2C.
 enc = pyiArduinoI2Cencoder(0x09)
 
-# Инициируем работу с энкодером.
-enc.begin()
-
 # Указываем выводу модуля работать
 # как кнопочный переключатель (триггер).
 enc.setPinOut(ENC_PIN_MODE_TRG)
```

### Comparing `pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/examples/PositionGet.py` & `pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/examples/PositionReset.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,29 @@
-#   ПРИМЕР ЧТЕНИЯ ТЕКУЩЕЙ ПОЗИЦИИ ВАЛА ЭНКОДЕРА:
-# Зная точную позицию Вала энкодера, работа
-# с модулем похожа на работу с потенциометром.
+# ПРИМЕР СБРОСА ТЕКУЩЕЙ ПОЗИЦИИ ВАЛА ЭНКОДЕРА:
 
 from time import sleep
 
 # Подключаем библиотеку для работы с энкодером I2C-flash.
 from pyiArduinoI2Cencoder import *
 
-# Инстанциируем объект, указывая адрес модуля на шине I2C.
+# Инстанцируем объект, указывая адрес модуля на шине I2C.
 enc = pyiArduinoI2Cencoder(0x09)
+enc.invEncoder(True)
+f = False;
 
-# Инициируем работу с энкодером.
-enc.begin()
-
-# Указываем считать до 2 полных оборотов.
-enc.setPosSettings(2)
-
-print("Вращайте вал!")
+print("Вращайте вал по часовой стрелке, затем нажмите на вал")
 
 while True:
-
-    p = enc.getPosition()
     # Выводим текущую позицию вала энкодера.
-    print(p)
+    p = enc.getPosition()
+    if p > 0:
+        f = True;
+
+    if f:
+        print(p)
 
-    sleep(.5)
+    # Если нажата кнопка энкодера
+    if enc.getButton(KEY_PUSHED):
+        # Сбрасываем позицию вала в 0:
+        enc.resPosition()
 
+    sleep(.1)
```

### Comparing `pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/examples/PositionSettings.py` & `pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/examples/PositionSettings.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 # ПРИМЕР НАСТРОЙКИ ПОКАЗАНИЙ ПОЗИЦИИ ВАЛА:
 
 from time import sleep
 
 # Подключаем библиотеку для работы с энкодером I2C-flash.
 from pyiArduinoI2Cencoder import *
 
-# Инстанциируем объект, указывая адрес модуля на шине I2C.
+# Инстанцируем объект, указывая адрес модуля на шине I2C.
 enc = pyiArduinoI2Cencoder(0x09)
 
-# Инициируем работу с энкодером.
-enc.begin()
 # Указываем считать до 5 полных оборотов, без отрицательных значений.
 enc.setPosSettings(5, False)
 
 while True:
 
     p = enc.getPosition()
     # Выводим текущую позицию вала энкодера.
```

### Comparing `pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/examples/newAddress.py` & `pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/examples/newAddress.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # ПРИМЕР СМЕНЫ АДРЕСА МОДУЛЯ:
 
 # Подключаем библиотеку для работы с датчиком температуры и влажности
 from pyiArduinoI2Cencoder import *
 import sys
 
-# Инстанциируем объект module для работы с функциями и методами библиотеки pyiArduinoI2Cencoder.
+# Инстанцируем объект module для работы с функциями и методами библиотеки pyiArduinoI2Cencoder.
 # Если при объявлении объекта указать адрес, например, module(0x0B),
 # то пример будет работать с тем модулем, адрес которого был указан.
 module = pyiArduinoI2Cencoder(None, NO_BEGIN)
 
 # Если сценарию не были переданы аргументы
 if len(sys.argv) < 2:
     # Назначаем модулю адрес (0x07 < адрес < 0x7F).
```

### Comparing `pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/iarduino_I2C_Encoder.cpp` & `pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/iarduino_I2C_Encoder.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/iarduino_I2C_Encoder.h` & `pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/iarduino_I2C_Encoder.h`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/iarduino_I2C_Encoder.pxd` & `pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/iarduino_I2C_Encoder.pxd`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/iarduino_I2C_PI.h` & `pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/iarduino_I2C_PI.h`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cencoder-1.0.1/pyiArduinoI2Cencoder/pyiArduinoI2Cencoder.pyx` & `pyiArduinoI2Cencoder-1.0.4/pyiArduinoI2Cencoder/pyiArduinoI2Cencoder.pyx`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cencoder-1.0.1/setup.py` & `pyiArduinoI2Cencoder-1.0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from distutils.extension import Extension
 
 def readme():
     with open('README.md') as readme:
         return readme.read()
 
 setup(name='pyiArduinoI2Cencoder',
-    version='1.0.1',
+    version='1.0.4',
     description='iarduino.ru module for Raspberry Pi',
     long_description=readme(),
     classifiers=[
         'Programming Language :: Python :: 3',
     ],
     url='http://github.com/tremaru/pyiArduinoI2Cencoder',
     author='iarduino.ru',
```

