# Comparing `tmp/pyiArduinoI2Cjoystick-1.0.0.tar.gz` & `tmp/pyiArduinoI2Cjoystick-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyiArduinoI2Cjoystick-1.0.0.tar", last modified: Fri May 22 13:52:37 2020, max compression
+gzip compressed data, was "pyiArduinoI2Cjoystick-1.0.2.tar", last modified: Mon Jun  3 11:54:55 2024, max compression
```

## Comparing `pyiArduinoI2Cjoystick-1.0.0.tar` & `pyiArduinoI2Cjoystick-1.0.2.tar`

### file list

```diff
@@ -1,39 +1,47 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2020-05-22 13:52:37.000000 pyiArduinoI2Cjoystick-1.0.0/
--rw-r--r--   0 pi        (1000) pi        (1000)     2460 2020-05-22 13:52:37.000000 pyiArduinoI2Cjoystick-1.0.0/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)       24 2020-05-20 13:59:52.000000 pyiArduinoI2Cjoystick-1.0.0/README
--rw-r--r--   0 pi        (1000) pi        (1000)     1891 2020-05-20 13:59:52.000000 pyiArduinoI2Cjoystick-1.0.0/README.md
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2020-05-22 13:52:37.000000 pyiArduinoI2Cjoystick-1.0.0/pyiArduinoI2Cjoystick/
--rw-r--r--   0 pi        (1000) pi        (1000)       31 2020-05-20 13:59:52.000000 pyiArduinoI2Cjoystick-1.0.0/pyiArduinoI2Cjoystick/__init__.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2020-05-22 13:52:37.000000 pyiArduinoI2Cjoystick-1.0.0/pyiArduinoI2Cjoystick/cpp/
--rw-------   0 pi        (1000) pi        (1000)     9502 2020-05-21 16:22:15.000000 pyiArduinoI2Cjoystick-1.0.0/pyiArduinoI2Cjoystick/cpp/Calibration.cpp
--rw-------   0 pi        (1000) pi        (1000)     2827 2020-05-21 16:50:22.000000 pyiArduinoI2Cjoystick-1.0.0/pyiArduinoI2Cjoystick/cpp/CalibrationManual.cpp
--rw-------   0 pi        (1000) pi        (1000)     2688 2020-05-22 09:12:27.000000 pyiArduinoI2Cjoystick-1.0.0/pyiArduinoI2Cjoystick/cpp/ChangeAxisDir.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)    11329 2020-05-20 14:20:06.000000 pyiArduinoI2Cjoystick-1.0.0/pyiArduinoI2Cjoystick/cpp/FindDevices.cpp
--rw-------   0 pi        (1000) pi        (1000)     3075 2020-05-22 09:25:08.000000 pyiArduinoI2Cjoystick-1.0.0/pyiArduinoI2Cjoystick/cpp/GetADC.cpp
--rw-------   0 pi        (1000) pi        (1000)     7330 2020-05-22 13:34:02.000000 pyiArduinoI2Cjoystick-1.0.0/pyiArduinoI2Cjoystick/cpp/GetDirection.cpp
--rw-------   0 pi        (1000) pi        (1000)     2657 2020-05-22 09:42:58.000000 pyiArduinoI2Cjoystick-1.0.0/pyiArduinoI2Cjoystick/cpp/GetPosition.cpp
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2020-05-22 13:52:37.000000 pyiArduinoI2Cjoystick-1.0.0/pyiArduinoI2Cjoystick/cpp/Includes/
--rw-r--r--   0 pi        (1000) pi        (1000)    17035 2020-05-21 14:30:00.000000 pyiArduinoI2Cjoystick-1.0.0/pyiArduinoI2Cjoystick/cpp/Includes/WString.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)     9967 2020-05-21 14:30:00.000000 pyiArduinoI2Cjoystick-1.0.0/pyiArduinoI2Cjoystick/cpp/Includes/WString.h
--rw-r--r--   0 pi        (1000) pi        (1000)     1091 2020-05-21 14:31:56.000000 pyiArduinoI2Cjoystick-1.0.0/pyiArduinoI2Cjoystick/cpp/Includes/dtostrf.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)     1004 2020-05-21 14:31:56.000000 pyiArduinoI2Cjoystick-1.0.0/pyiArduinoI2Cjoystick/cpp/Includes/dtostrf.h
--rw-r--r--   0 pi        (1000) pi        (1000)     2917 2020-05-21 14:31:34.000000 pyiArduinoI2Cjoystick-1.0.0/pyiArduinoI2Cjoystick/cpp/Includes/itoa.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)     1253 2020-05-21 14:31:34.000000 pyiArduinoI2Cjoystick-1.0.0/pyiArduinoI2Cjoystick/cpp/Includes/itoa.h
--rw-r--r--   0 pi        (1000) pi        (1000)     1498 2020-05-20 13:59:52.000000 pyiArduinoI2Cjoystick-1.0.0/pyiArduinoI2Cjoystick/cpp/NewAddress.cpp
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2020-05-22 13:52:37.000000 pyiArduinoI2Cjoystick-1.0.0/pyiArduinoI2Cjoystick/examples/
--rwxr-xr-x   0 pi        (1000) pi        (1000)     5649 2020-05-22 12:18:34.000000 pyiArduinoI2Cjoystick-1.0.0/pyiArduinoI2Cjoystick/examples/Calibration.py
--rwxr-xr-x   0 pi        (1000) pi        (1000)     1985 2020-05-22 11:10:46.000000 pyiArduinoI2Cjoystick-1.0.0/pyiArduinoI2Cjoystick/examples/CalibrationManual.py
--rwxr-xr-x   0 pi        (1000) pi        (1000)     1967 2020-05-22 12:34:34.000000 pyiArduinoI2Cjoystick-1.0.0/pyiArduinoI2Cjoystick/examples/ChangeAxisDir.py
--rwxr-xr-x   0 pi        (1000) pi        (1000)     5902 2020-05-22 12:35:39.000000 pyiArduinoI2Cjoystick-1.0.0/pyiArduinoI2Cjoystick/examples/FindDevices.py
--rwxr-xr-x   0 pi        (1000) pi        (1000)     1584 2020-05-22 13:26:29.000000 pyiArduinoI2Cjoystick-1.0.0/pyiArduinoI2Cjoystick/examples/GetADC.py
--rwxr-xr-x   0 pi        (1000) pi        (1000)     1617 2020-05-22 13:26:26.000000 pyiArduinoI2Cjoystick-1.0.0/pyiArduinoI2Cjoystick/examples/GetPosition.py
--rwxr-xr-x   0 pi        (1000) pi        (1000)     1414 2020-05-22 12:37:38.000000 pyiArduinoI2Cjoystick-1.0.0/pyiArduinoI2Cjoystick/examples/newAddress.py
--rwx------   0 pi        (1000) pi        (1000)    40327 2020-05-21 13:56:46.000000 pyiArduinoI2Cjoystick-1.0.0/pyiArduinoI2Cjoystick/iarduino_I2C_Joystick.cpp
--rwx------   0 pi        (1000) pi        (1000)    23496 2020-05-21 13:56:36.000000 pyiArduinoI2Cjoystick-1.0.0/pyiArduinoI2Cjoystick/iarduino_I2C_Joystick.h
--rw-r--r--   0 pi        (1000) pi        (1000)     1322 2020-05-21 13:52:41.000000 pyiArduinoI2Cjoystick-1.0.0/pyiArduinoI2Cjoystick/iarduino_I2C_Joystick.pxd
--rwxr-xr-x   0 pi        (1000) pi        (1000)    11805 2020-05-20 13:57:49.000000 pyiArduinoI2Cjoystick-1.0.0/pyiArduinoI2Cjoystick/iarduino_I2C_PI.h
--rw-r--r--   0 pi        (1000) pi        (1000)   289095 2020-05-22 08:54:07.000000 pyiArduinoI2Cjoystick-1.0.0/pyiArduinoI2Cjoystick/pyiArduinoI2Cjoystick.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)     5561 2020-05-22 08:53:56.000000 pyiArduinoI2Cjoystick-1.0.0/pyiArduinoI2Cjoystick/pyiArduinoI2Cjoystick.pyx
--rw-r--r--   0 pi        (1000) pi        (1000)      134 2020-05-20 13:59:52.000000 pyiArduinoI2Cjoystick-1.0.0/pyiArduinoI2Cjoystick/setup.py
--rw-r--r--   0 pi        (1000) pi        (1000)       40 2020-05-20 13:57:49.000000 pyiArduinoI2Cjoystick-1.0.0/setup.cfg
--rw-r--r--   0 pi        (1000) pi        (1000)      733 2020-05-22 13:52:32.000000 pyiArduinoI2Cjoystick-1.0.0/setup.py
+drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-06-03 11:54:55.150020 pyiArduinoI2Cjoystick-1.0.2/
+-rw-r--r--   0 dron      (1000) dron      (1000)     3291 2024-03-29 13:35:18.000000 pyiArduinoI2Cjoystick-1.0.2/LICENSE
+-rw-r--r--   0 dron      (1000) dron      (1000)       86 2024-03-29 13:35:18.000000 pyiArduinoI2Cjoystick-1.0.2/MANIFEST.in
+-rw-r--r--   0 dron      (1000) dron      (1000)     2195 2024-06-03 11:54:55.150020 pyiArduinoI2Cjoystick-1.0.2/PKG-INFO
+-rw-r--r--   0 dron      (1000) dron      (1000)       24 2024-03-29 13:35:18.000000 pyiArduinoI2Cjoystick-1.0.2/README
+-rw-r--r--   0 dron      (1000) dron      (1000)     1891 2024-03-29 13:35:18.000000 pyiArduinoI2Cjoystick-1.0.2/README.md
+drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-06-03 11:54:55.134021 pyiArduinoI2Cjoystick-1.0.2/pyiArduinoI2Cjoystick/
+-rw-r--r--   0 dron      (1000) dron      (1000)       31 2024-03-29 13:35:18.000000 pyiArduinoI2Cjoystick-1.0.2/pyiArduinoI2Cjoystick/__init__.py
+drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-06-03 11:54:55.142021 pyiArduinoI2Cjoystick-1.0.2/pyiArduinoI2Cjoystick/cpp/
+-rw-r--r--   0 dron      (1000) dron      (1000)     9502 2024-03-29 13:35:18.000000 pyiArduinoI2Cjoystick-1.0.2/pyiArduinoI2Cjoystick/cpp/Calibration.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     2827 2024-03-29 13:35:18.000000 pyiArduinoI2Cjoystick-1.0.2/pyiArduinoI2Cjoystick/cpp/CalibrationManual.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     2688 2024-03-29 13:35:18.000000 pyiArduinoI2Cjoystick-1.0.2/pyiArduinoI2Cjoystick/cpp/ChangeAxisDir.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)    11329 2024-03-29 13:35:18.000000 pyiArduinoI2Cjoystick-1.0.2/pyiArduinoI2Cjoystick/cpp/FindDevices.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     3075 2024-03-29 13:35:18.000000 pyiArduinoI2Cjoystick-1.0.2/pyiArduinoI2Cjoystick/cpp/GetADC.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     7330 2024-03-29 13:35:18.000000 pyiArduinoI2Cjoystick-1.0.2/pyiArduinoI2Cjoystick/cpp/GetDirection.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     2657 2024-03-29 13:35:18.000000 pyiArduinoI2Cjoystick-1.0.2/pyiArduinoI2Cjoystick/cpp/GetPosition.cpp
+drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-06-03 11:54:55.146021 pyiArduinoI2Cjoystick-1.0.2/pyiArduinoI2Cjoystick/cpp/Includes/
+-rw-r--r--   0 dron      (1000) dron      (1000)    17035 2024-03-29 13:35:18.000000 pyiArduinoI2Cjoystick-1.0.2/pyiArduinoI2Cjoystick/cpp/Includes/WString.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     9967 2024-03-29 13:35:18.000000 pyiArduinoI2Cjoystick-1.0.2/pyiArduinoI2Cjoystick/cpp/Includes/WString.h
+-rw-r--r--   0 dron      (1000) dron      (1000)     1091 2024-03-29 13:35:18.000000 pyiArduinoI2Cjoystick-1.0.2/pyiArduinoI2Cjoystick/cpp/Includes/dtostrf.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     1004 2024-03-29 13:35:18.000000 pyiArduinoI2Cjoystick-1.0.2/pyiArduinoI2Cjoystick/cpp/Includes/dtostrf.h
+-rw-r--r--   0 dron      (1000) dron      (1000)     2917 2024-03-29 13:35:18.000000 pyiArduinoI2Cjoystick-1.0.2/pyiArduinoI2Cjoystick/cpp/Includes/itoa.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     1253 2024-03-29 13:35:18.000000 pyiArduinoI2Cjoystick-1.0.2/pyiArduinoI2Cjoystick/cpp/Includes/itoa.h
+-rw-r--r--   0 dron      (1000) dron      (1000)     1498 2024-03-29 13:35:18.000000 pyiArduinoI2Cjoystick-1.0.2/pyiArduinoI2Cjoystick/cpp/NewAddress.cpp
+drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-06-03 11:54:55.150020 pyiArduinoI2Cjoystick-1.0.2/pyiArduinoI2Cjoystick/examples/
+-rwxr-xr-x   0 dron      (1000) dron      (1000)     5649 2024-03-29 13:35:18.000000 pyiArduinoI2Cjoystick-1.0.2/pyiArduinoI2Cjoystick/examples/Calibration.py
+-rwxr-xr-x   0 dron      (1000) dron      (1000)     1985 2024-03-29 13:35:18.000000 pyiArduinoI2Cjoystick-1.0.2/pyiArduinoI2Cjoystick/examples/CalibrationManual.py
+-rwxr-xr-x   0 dron      (1000) dron      (1000)     1967 2024-03-29 13:35:18.000000 pyiArduinoI2Cjoystick-1.0.2/pyiArduinoI2Cjoystick/examples/ChangeAxisDir.py
+-rwxr-xr-x   0 dron      (1000) dron      (1000)     4204 2024-03-29 13:35:18.000000 pyiArduinoI2Cjoystick-1.0.2/pyiArduinoI2Cjoystick/examples/FindDevices.py
+-rwxr-xr-x   0 dron      (1000) dron      (1000)     1584 2024-03-29 13:35:18.000000 pyiArduinoI2Cjoystick-1.0.2/pyiArduinoI2Cjoystick/examples/GetADC.py
+-rwxr-xr-x   0 dron      (1000) dron      (1000)      955 2024-03-29 13:35:18.000000 pyiArduinoI2Cjoystick-1.0.2/pyiArduinoI2Cjoystick/examples/GetDirection.py
+-rwxr-xr-x   0 dron      (1000) dron      (1000)     1617 2024-03-29 13:35:18.000000 pyiArduinoI2Cjoystick-1.0.2/pyiArduinoI2Cjoystick/examples/GetPosition.py
+-rwxr-xr-x   0 dron      (1000) dron      (1000)     1373 2024-03-29 13:35:18.000000 pyiArduinoI2Cjoystick-1.0.2/pyiArduinoI2Cjoystick/examples/newAddress.py
+-rwxr-xr-x   0 dron      (1000) dron      (1000)    40327 2024-03-29 13:35:18.000000 pyiArduinoI2Cjoystick-1.0.2/pyiArduinoI2Cjoystick/iarduino_I2C_Joystick.cpp
+-rwxr-xr-x   0 dron      (1000) dron      (1000)    23496 2024-03-29 13:35:18.000000 pyiArduinoI2Cjoystick-1.0.2/pyiArduinoI2Cjoystick/iarduino_I2C_Joystick.h
+-rw-r--r--   0 dron      (1000) dron      (1000)     1322 2024-03-29 13:35:18.000000 pyiArduinoI2Cjoystick-1.0.2/pyiArduinoI2Cjoystick/iarduino_I2C_Joystick.pxd
+-rwxr-xr-x   0 dron      (1000) dron      (1000)    11805 2024-03-29 13:35:18.000000 pyiArduinoI2Cjoystick-1.0.2/pyiArduinoI2Cjoystick/iarduino_I2C_PI.h
+-rw-r--r--   0 dron      (1000) dron      (1000)   560779 2024-06-03 11:48:22.000000 pyiArduinoI2Cjoystick-1.0.2/pyiArduinoI2Cjoystick/pyiArduinoI2Cjoystick.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     5561 2024-03-29 13:35:18.000000 pyiArduinoI2Cjoystick-1.0.2/pyiArduinoI2Cjoystick/pyiArduinoI2Cjoystick.pyx
+-rw-r--r--   0 dron      (1000) dron      (1000)      134 2024-03-29 13:35:18.000000 pyiArduinoI2Cjoystick-1.0.2/pyiArduinoI2Cjoystick/setup.py
+drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-06-03 11:54:55.138021 pyiArduinoI2Cjoystick-1.0.2/pyiArduinoI2Cjoystick.egg-info/
+-rw-r--r--   0 dron      (1000) dron      (1000)     2195 2024-06-03 11:54:54.000000 pyiArduinoI2Cjoystick-1.0.2/pyiArduinoI2Cjoystick.egg-info/PKG-INFO
+-rw-r--r--   0 dron      (1000) dron      (1000)     1558 2024-06-03 11:54:55.000000 pyiArduinoI2Cjoystick-1.0.2/pyiArduinoI2Cjoystick.egg-info/SOURCES.txt
+-rw-r--r--   0 dron      (1000) dron      (1000)        1 2024-06-03 11:54:54.000000 pyiArduinoI2Cjoystick-1.0.2/pyiArduinoI2Cjoystick.egg-info/dependency_links.txt
+-rw-r--r--   0 dron      (1000) dron      (1000)       22 2024-06-03 11:54:54.000000 pyiArduinoI2Cjoystick-1.0.2/pyiArduinoI2Cjoystick.egg-info/top_level.txt
+-rw-r--r--   0 dron      (1000) dron      (1000)       79 2024-06-03 11:54:55.150020 pyiArduinoI2Cjoystick-1.0.2/setup.cfg
+-rw-r--r--   0 dron      (1000) dron      (1000)      733 2024-06-03 11:51:51.000000 pyiArduinoI2Cjoystick-1.0.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyiArduinoI2Cjoystick-1.0.0/PKG-INFO` & `pyiArduinoI2Cjoystick-1.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pyiArduinoI2Cjoystick
-Version: 1.0.0
+Version: 1.0.2
 Summary: iarduino.ru module for Raspberry Pi
 Home-page: http://github.com/tremaru/pyiArduinoI2Cjoystick
 Author: iarduino.ru
 Author-email: shop@iarduino.ru
 License: MIT
-Description: [![](https://iarduino.ru/img/logo.svg)](https://iarduino.ru)[![](https://wiki.iarduino.ru/img/git-shop.svg?3)](https://iarduino.ru) [![](https://wiki.iarduino.ru/img/git-wiki.svg?2)](https://wiki.iarduino.ru) [![](https://wiki.iarduino.ru/img/git-lesson.svg?2)](https://lesson.iarduino.ru)[![](https://wiki.iarduino.ru/img/git-forum.svg?2)](http://forum.trema.ru)
-        
-        # pyiArduinoI2Cjoystick
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
-        `sudo pip3 install pyiArduinoI2Cjoystick`
-        
-        Самостоятельная сборка из исходников:
-        
-        `git clone https://github.com/tremaru/pyiArduinoI2Cjoystick.git && cd pyiArduinoI2Cjoystick/pyiArduinoI2Cjoystick && python3 setup.py build_ext --inplace`
-        
-        Примеры для Python находятся в папке `pyiArduinoI2Cjoystick/examples`
-        
-        Примеры для С++ находятся в папке `pyiArduinoI2Cjoystick/cpp`. Так же в этой папке лежит *Makefile* для сборки
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
+# pyiArduinoI2Cjoystick
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
+`sudo pip3 install pyiArduinoI2Cjoystick`
+
+Самостоятельная сборка из исходников:
+
+`git clone https://github.com/tremaru/pyiArduinoI2Cjoystick.git && cd pyiArduinoI2Cjoystick/pyiArduinoI2Cjoystick && python3 setup.py build_ext --inplace`
+
+Примеры для Python находятся в папке `pyiArduinoI2Cjoystick/examples`
+
+Примеры для С++ находятся в папке `pyiArduinoI2Cjoystick/cpp`. Так же в этой папке лежит *Makefile* для сборки
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

### Comparing `pyiArduinoI2Cjoystick-1.0.0/README.md` & `pyiArduinoI2Cjoystick-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cjoystick-1.0.0/pyiArduinoI2Cjoystick/cpp/Calibration.cpp` & `pyiArduinoI2Cjoystick-1.0.2/pyiArduinoI2Cjoystick/cpp/Calibration.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cjoystick-1.0.0/pyiArduinoI2Cjoystick/cpp/CalibrationManual.cpp` & `pyiArduinoI2Cjoystick-1.0.2/pyiArduinoI2Cjoystick/cpp/CalibrationManual.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cjoystick-1.0.0/pyiArduinoI2Cjoystick/cpp/ChangeAxisDir.cpp` & `pyiArduinoI2Cjoystick-1.0.2/pyiArduinoI2Cjoystick/cpp/ChangeAxisDir.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cjoystick-1.0.0/pyiArduinoI2Cjoystick/cpp/FindDevices.cpp` & `pyiArduinoI2Cjoystick-1.0.2/pyiArduinoI2Cjoystick/cpp/FindDevices.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cjoystick-1.0.0/pyiArduinoI2Cjoystick/cpp/GetADC.cpp` & `pyiArduinoI2Cjoystick-1.0.2/pyiArduinoI2Cjoystick/cpp/GetADC.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cjoystick-1.0.0/pyiArduinoI2Cjoystick/cpp/GetDirection.cpp` & `pyiArduinoI2Cjoystick-1.0.2/pyiArduinoI2Cjoystick/cpp/GetDirection.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cjoystick-1.0.0/pyiArduinoI2Cjoystick/cpp/GetPosition.cpp` & `pyiArduinoI2Cjoystick-1.0.2/pyiArduinoI2Cjoystick/cpp/GetPosition.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cjoystick-1.0.0/pyiArduinoI2Cjoystick/cpp/Includes/WString.cpp` & `pyiArduinoI2Cjoystick-1.0.2/pyiArduinoI2Cjoystick/cpp/Includes/WString.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cjoystick-1.0.0/pyiArduinoI2Cjoystick/cpp/Includes/WString.h` & `pyiArduinoI2Cjoystick-1.0.2/pyiArduinoI2Cjoystick/cpp/Includes/WString.h`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cjoystick-1.0.0/pyiArduinoI2Cjoystick/cpp/Includes/dtostrf.cpp` & `pyiArduinoI2Cjoystick-1.0.2/pyiArduinoI2Cjoystick/cpp/Includes/dtostrf.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cjoystick-1.0.0/pyiArduinoI2Cjoystick/cpp/Includes/dtostrf.h` & `pyiArduinoI2Cjoystick-1.0.2/pyiArduinoI2Cjoystick/cpp/Includes/dtostrf.h`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cjoystick-1.0.0/pyiArduinoI2Cjoystick/cpp/Includes/itoa.cpp` & `pyiArduinoI2Cjoystick-1.0.2/pyiArduinoI2Cjoystick/cpp/Includes/itoa.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cjoystick-1.0.0/pyiArduinoI2Cjoystick/cpp/Includes/itoa.h` & `pyiArduinoI2Cjoystick-1.0.2/pyiArduinoI2Cjoystick/cpp/Includes/itoa.h`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cjoystick-1.0.0/pyiArduinoI2Cjoystick/cpp/NewAddress.cpp` & `pyiArduinoI2Cjoystick-1.0.2/pyiArduinoI2Cjoystick/cpp/NewAddress.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cjoystick-1.0.0/pyiArduinoI2Cjoystick/examples/Calibration.py` & `pyiArduinoI2Cjoystick-1.0.2/pyiArduinoI2Cjoystick/examples/Calibration.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cjoystick-1.0.0/pyiArduinoI2Cjoystick/examples/CalibrationManual.py` & `pyiArduinoI2Cjoystick-1.0.2/pyiArduinoI2Cjoystick/examples/CalibrationManual.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cjoystick-1.0.0/pyiArduinoI2Cjoystick/examples/ChangeAxisDir.py` & `pyiArduinoI2Cjoystick-1.0.2/pyiArduinoI2Cjoystick/examples/ChangeAxisDir.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cjoystick-1.0.0/pyiArduinoI2Cjoystick/examples/FindDevices.py` & `pyiArduinoI2Cjoystick-1.0.2/pyiArduinoI2Cjoystick/examples/FindDevices.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 #!/usr/bin/python3
 # Данный пример ищет модули на шине и выводит информацию о них.
                                             #
 import smbus                                # Подключаем модуль шины smbus(i2c)
-choices = {                                 # Создаём список устройств
-    0x01: "кнопкой",                            # Если значение 1, значит это кнопка.
-    0x02: "светодиодом",                        # Если значение 2, значит это RGB светодиод.
-    0x03: "потенциометром",                     # Если значение 3, значит это потенциометр.
-    0x04: "звукоизлучателем",                   # Если значение 4, значит это звукоизлучатель.
-    0x05: "датчиком SHT",                       # Если значение 5, значит это датчик владности и температуры.
-    0x06: "датчиком света",                     # Если значение 6, значит это датчик света.
-    0x07: "расширителем выводов",               # Если значение 7, значит это датчик света.
-    0x08: "LED матрицей",                       # Если значение 8, значит это светодиодная матрица.
-    0x09: "Энкодером",                          # Если значение 9, значит это энкодер.
-    0x0A: "реле на 2 канала",                   # Если значение A, значит это электромеханическое реле на 2 канала.
-    0x0B: "реле на 4 канала",                   # Если значение B, значит это твердотельное реле на 4 канала.
-    0x0C: "силовым ключём 4 N",                 # Если значение C, значит это силовой ключ на 4 N-канала.
-    0x0D: "силовым ключём 4 P",                 # Если значение D, значит это силовой ключ на 4 P-канала.
-    0x0E: "силовым ключём 4 N",                 # Если значение E, значит это силовой ключ на 4 N-канала, с измерением тока.
-    0x0F: "силовым ключём 4 P",                 # Если значение F, значит это силовой ключ на 4 P-канала, с измерением тока.
+choices = {                                 # Создаём словарь устройств
+    0x01: "кнопкой",
+    0x02: "светодиодом",
+    0x03: "потенциометром",
+    0x04: "звукоизлучателем",
+    0x05: "датчиком SHT",
+    0x06: "датчиком света",
+    0x07: "расширителем выводов",
+    0x08: "LED матрицей",
+    0x09: "Энкодером",
+    0x0A: "реле на 2 канала",
+    0x0B: "реле на 4 канала",
+    0x0C: "силовым ключём 4 N",
+    0x0D: "силовым ключём 4 P",
+    0x0E: "силовым ключём 4 N",
+    0x0F: "силовым ключём 4 P",
     0x10: "бампер с датчиками линий",
     0x11: "джойстик",
     0x12: "LCD конвертер в I2C",
     0x13: "клавиатура",
     0x14: "мотор-редуктор с драйвером",
     0x15: "реле на 1 канал",
     0x16: "LED индикатор на 4 разряда",
```

### Comparing `pyiArduinoI2Cjoystick-1.0.0/pyiArduinoI2Cjoystick/examples/GetADC.py` & `pyiArduinoI2Cjoystick-1.0.2/pyiArduinoI2Cjoystick/examples/GetADC.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cjoystick-1.0.0/pyiArduinoI2Cjoystick/examples/GetPosition.py` & `pyiArduinoI2Cjoystick-1.0.2/pyiArduinoI2Cjoystick/examples/GetPosition.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cjoystick-1.0.0/pyiArduinoI2Cjoystick/examples/newAddress.py` & `pyiArduinoI2Cjoystick-1.0.2/pyiArduinoI2Cjoystick/examples/newAddress.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/python3
 # ПРИМЕР СМЕНЫ АДРЕСА МОДУЛЯ:
 
-# Подключаем библиотеку для работы с датчиком температуры и влажности
+# Подключаем библиотеку для работы с джойстиком
 from pyiArduinoI2Cjoystick import *
 import sys
 
 # Объявляем объект module для работы с функциями и методами библиотеки pyiArduinoI2Cjoystick.
 # Если при объявлении объекта указать адрес, например, module(0x0B),
 # то пример будет работать с тем модулем, адрес которого был указан.
 module = pyiArduinoI2Cjoystick(None, NO_BEGIN)
```

### Comparing `pyiArduinoI2Cjoystick-1.0.0/pyiArduinoI2Cjoystick/iarduino_I2C_Joystick.cpp` & `pyiArduinoI2Cjoystick-1.0.2/pyiArduinoI2Cjoystick/iarduino_I2C_Joystick.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cjoystick-1.0.0/pyiArduinoI2Cjoystick/iarduino_I2C_Joystick.h` & `pyiArduinoI2Cjoystick-1.0.2/pyiArduinoI2Cjoystick/iarduino_I2C_Joystick.h`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cjoystick-1.0.0/pyiArduinoI2Cjoystick/iarduino_I2C_Joystick.pxd` & `pyiArduinoI2Cjoystick-1.0.2/pyiArduinoI2Cjoystick/iarduino_I2C_Joystick.pxd`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cjoystick-1.0.0/pyiArduinoI2Cjoystick/iarduino_I2C_PI.h` & `pyiArduinoI2Cjoystick-1.0.2/pyiArduinoI2Cjoystick/iarduino_I2C_PI.h`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cjoystick-1.0.0/pyiArduinoI2Cjoystick/pyiArduinoI2Cjoystick.pyx` & `pyiArduinoI2Cjoystick-1.0.2/pyiArduinoI2Cjoystick/pyiArduinoI2Cjoystick.pyx`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cjoystick-1.0.0/setup.py` & `pyiArduinoI2Cjoystick-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from distutils.extension import Extension
 
 def readme():
     with open('README.md') as readme:
         return readme.read()
 
 setup(name='pyiArduinoI2Cjoystick',
-    version='1.0.0',
+    version='1.0.2',
     description='iarduino.ru module for Raspberry Pi',
     long_description=readme(),
     classifiers=[
         'Programming Language :: Python :: 3',
     ],
     url='http://github.com/tremaru/pyiArduinoI2Cjoystick',
     author='iarduino.ru',
```

