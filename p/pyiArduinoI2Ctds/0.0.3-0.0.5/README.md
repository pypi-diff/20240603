# Comparing `tmp/pyiArduinoI2Ctds-0.0.3.tar.gz` & `tmp/pyiArduinoI2Ctds-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyiArduinoI2Ctds-0.0.3.tar", last modified: Wed Apr  6 07:41:05 2022, max compression
+gzip compressed data, was "pyiArduinoI2Ctds-0.0.5.tar", last modified: Mon Jun  3 11:55:03 2024, max compression
```

## Comparing `pyiArduinoI2Ctds-0.0.3.tar` & `pyiArduinoI2Ctds-0.0.5.tar`

### file list

```diff
@@ -1,30 +1,37 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2022-04-06 07:41:05.000000 pyiArduinoI2Ctds-0.0.3/
--rw-r--r--   0 pi        (1000) pi        (1000)     2695 2022-04-06 07:41:05.000000 pyiArduinoI2Ctds-0.0.3/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)       19 2021-09-08 13:20:04.000000 pyiArduinoI2Ctds-0.0.3/README
--rw-r--r--   0 pi        (1000) pi        (1000)     2136 2021-12-28 15:27:20.000000 pyiArduinoI2Ctds-0.0.3/README.md
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2022-04-06 07:41:05.000000 pyiArduinoI2Ctds-0.0.3/pyiArduinoI2Ctds/
--rw-r--r--   0 pi        (1000) pi        (1000)       26 2021-09-08 13:20:04.000000 pyiArduinoI2Ctds-0.0.3/pyiArduinoI2Ctds/__init__.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2022-04-06 07:41:05.000000 pyiArduinoI2Ctds-0.0.3/pyiArduinoI2Ctds/cpp/
--rw-r--r--   0 pi        (1000) pi        (1000)     9722 2021-12-28 13:29:14.000000 pyiArduinoI2Ctds-0.0.3/pyiArduinoI2Ctds/cpp/FindDevices.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)     1488 2021-12-28 13:28:58.000000 pyiArduinoI2Ctds-0.0.3/pyiArduinoI2Ctds/cpp/NewAddress.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)      580 2021-12-28 14:53:49.000000 pyiArduinoI2Ctds-0.0.3/pyiArduinoI2Ctds/cpp/Serial.h
--rw-r--r--   0 pi        (1000) pi        (1000)     2716 2021-12-28 14:51:01.000000 pyiArduinoI2Ctds-0.0.3/pyiArduinoI2Ctds/cpp/getData.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)     3475 2021-12-28 14:59:14.000000 pyiArduinoI2Ctds-0.0.3/pyiArduinoI2Ctds/cpp/getSettings.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)       80 2021-12-28 14:53:40.000000 pyiArduinoI2Ctds-0.0.3/pyiArduinoI2Ctds/cpp/main.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)     3671 2021-12-28 14:54:51.000000 pyiArduinoI2Ctds-0.0.3/pyiArduinoI2Ctds/cpp/setCalibration.cpp
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2022-04-06 07:41:05.000000 pyiArduinoI2Ctds-0.0.3/pyiArduinoI2Ctds/examples/
--rw-r--r--   0 pi        (1000) pi        (1000)     7782 2021-12-28 16:44:29.000000 pyiArduinoI2Ctds-0.0.3/pyiArduinoI2Ctds/examples/FindDevices.py
--rw-r--r--   0 pi        (1000) pi        (1000)     1938 2021-12-28 15:11:04.000000 pyiArduinoI2Ctds-0.0.3/pyiArduinoI2Ctds/examples/getData.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2479 2021-12-28 15:02:16.000000 pyiArduinoI2Ctds-0.0.3/pyiArduinoI2Ctds/examples/getSettings.py
--rw-r--r--   0 pi        (1000) pi        (1000)     1380 2021-09-08 13:20:04.000000 pyiArduinoI2Ctds-0.0.3/pyiArduinoI2Ctds/examples/newAddress.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2797 2021-12-28 15:16:00.000000 pyiArduinoI2Ctds-0.0.3/pyiArduinoI2Ctds/examples/setCalibration.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2007 2021-12-28 15:16:58.000000 pyiArduinoI2Ctds-0.0.3/pyiArduinoI2Ctds/examples/setSettings.py
--rwxr-xr-x   0 pi        (1000) pi        (1000)    10971 2021-12-29 08:13:42.000000 pyiArduinoI2Ctds-0.0.3/pyiArduinoI2Ctds/iarduino_I2C_PI.h
--rw-r--r--   0 pi        (1000) pi        (1000)    51023 2022-04-06 07:36:18.000000 pyiArduinoI2Ctds-0.0.3/pyiArduinoI2Ctds/iarduino_I2C_TDS.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)    18193 2022-04-06 07:37:14.000000 pyiArduinoI2Ctds-0.0.3/pyiArduinoI2Ctds/iarduino_I2C_TDS.h
--rw-r--r--   0 pi        (1000) pi        (1000)     1361 2022-04-06 07:37:42.000000 pyiArduinoI2Ctds-0.0.3/pyiArduinoI2Ctds/iarduino_I2C_TDS.pxd
--rw-r--r--   0 pi        (1000) pi        (1000)   285035 2022-04-06 07:38:45.000000 pyiArduinoI2Ctds-0.0.3/pyiArduinoI2Ctds/pyiArduinoI2Ctds.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)     4691 2022-04-06 07:38:26.000000 pyiArduinoI2Ctds-0.0.3/pyiArduinoI2Ctds/pyiArduinoI2Ctds.pyx
--rw-r--r--   0 pi        (1000) pi        (1000)      129 2021-09-08 13:20:04.000000 pyiArduinoI2Ctds-0.0.3/pyiArduinoI2Ctds/setup.py
--rw-r--r--   0 pi        (1000) pi        (1000)       40 2021-09-08 13:20:04.000000 pyiArduinoI2Ctds-0.0.3/setup.cfg
--rw-r--r--   0 pi        (1000) pi        (1000)      708 2022-04-06 07:41:01.000000 pyiArduinoI2Ctds-0.0.3/setup.py
+drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-06-03 11:55:03.913902 pyiArduinoI2Ctds-0.0.5/
+-rw-r--r--   0 dron      (1000) dron      (1000)     3291 2024-03-29 13:35:06.000000 pyiArduinoI2Ctds-0.0.5/LICENSE
+-rw-r--r--   0 dron      (1000) dron      (1000)       81 2024-03-29 13:35:06.000000 pyiArduinoI2Ctds-0.0.5/MANIFEST.in
+-rw-r--r--   0 dron      (1000) dron      (1000)     2430 2024-06-03 11:55:03.917902 pyiArduinoI2Ctds-0.0.5/PKG-INFO
+-rw-r--r--   0 dron      (1000) dron      (1000)       19 2024-03-29 13:35:06.000000 pyiArduinoI2Ctds-0.0.5/README
+-rw-r--r--   0 dron      (1000) dron      (1000)     2136 2024-03-29 13:35:06.000000 pyiArduinoI2Ctds-0.0.5/README.md
+drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-06-03 11:55:03.905902 pyiArduinoI2Ctds-0.0.5/pyiArduinoI2Ctds/
+-rw-r--r--   0 dron      (1000) dron      (1000)       26 2024-03-29 13:35:06.000000 pyiArduinoI2Ctds-0.0.5/pyiArduinoI2Ctds/__init__.py
+drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-06-03 11:55:03.909902 pyiArduinoI2Ctds-0.0.5/pyiArduinoI2Ctds/cpp/
+-rw-r--r--   0 dron      (1000) dron      (1000)     9722 2024-03-29 13:35:06.000000 pyiArduinoI2Ctds-0.0.5/pyiArduinoI2Ctds/cpp/FindDevices.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     1488 2024-03-29 13:35:06.000000 pyiArduinoI2Ctds-0.0.5/pyiArduinoI2Ctds/cpp/NewAddress.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)      580 2024-03-29 13:35:06.000000 pyiArduinoI2Ctds-0.0.5/pyiArduinoI2Ctds/cpp/Serial.h
+-rw-r--r--   0 dron      (1000) dron      (1000)     2716 2024-03-29 13:35:06.000000 pyiArduinoI2Ctds-0.0.5/pyiArduinoI2Ctds/cpp/getData.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     3475 2024-03-29 13:35:06.000000 pyiArduinoI2Ctds-0.0.5/pyiArduinoI2Ctds/cpp/getSettings.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)       80 2024-03-29 13:35:06.000000 pyiArduinoI2Ctds-0.0.5/pyiArduinoI2Ctds/cpp/main.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     3671 2024-03-29 13:35:06.000000 pyiArduinoI2Ctds-0.0.5/pyiArduinoI2Ctds/cpp/setCalibration.cpp
+drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-06-03 11:55:03.913902 pyiArduinoI2Ctds-0.0.5/pyiArduinoI2Ctds/examples/
+-rw-r--r--   0 dron      (1000) dron      (1000)     7782 2024-03-29 13:35:06.000000 pyiArduinoI2Ctds-0.0.5/pyiArduinoI2Ctds/examples/FindDevices.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     1938 2024-03-29 13:35:06.000000 pyiArduinoI2Ctds-0.0.5/pyiArduinoI2Ctds/examples/getData.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     2479 2024-03-29 13:35:06.000000 pyiArduinoI2Ctds-0.0.5/pyiArduinoI2Ctds/examples/getSettings.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     1380 2024-03-29 13:35:06.000000 pyiArduinoI2Ctds-0.0.5/pyiArduinoI2Ctds/examples/newAddress.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     2797 2024-03-29 13:35:06.000000 pyiArduinoI2Ctds-0.0.5/pyiArduinoI2Ctds/examples/setCalibration.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     2007 2024-03-29 13:35:06.000000 pyiArduinoI2Ctds-0.0.5/pyiArduinoI2Ctds/examples/setSettings.py
+-rwxr-xr-x   0 dron      (1000) dron      (1000)    10971 2024-03-29 13:35:06.000000 pyiArduinoI2Ctds-0.0.5/pyiArduinoI2Ctds/iarduino_I2C_PI.h
+-rw-r--r--   0 dron      (1000) dron      (1000)    51023 2024-03-29 13:35:06.000000 pyiArduinoI2Ctds-0.0.5/pyiArduinoI2Ctds/iarduino_I2C_TDS.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)    18193 2024-03-29 13:35:06.000000 pyiArduinoI2Ctds-0.0.5/pyiArduinoI2Ctds/iarduino_I2C_TDS.h
+-rw-r--r--   0 dron      (1000) dron      (1000)     1361 2024-03-29 13:35:06.000000 pyiArduinoI2Ctds-0.0.5/pyiArduinoI2Ctds/iarduino_I2C_TDS.pxd
+-rw-r--r--   0 dron      (1000) dron      (1000)   610434 2024-06-03 11:49:38.000000 pyiArduinoI2Ctds-0.0.5/pyiArduinoI2Ctds/pyiArduinoI2Ctds.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     4691 2024-03-29 13:35:06.000000 pyiArduinoI2Ctds-0.0.5/pyiArduinoI2Ctds/pyiArduinoI2Ctds.pyx
+-rw-r--r--   0 dron      (1000) dron      (1000)      129 2024-03-29 13:35:06.000000 pyiArduinoI2Ctds-0.0.5/pyiArduinoI2Ctds/setup.py
+drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-06-03 11:55:03.905902 pyiArduinoI2Ctds-0.0.5/pyiArduinoI2Ctds.egg-info/
+-rw-r--r--   0 dron      (1000) dron      (1000)     2430 2024-06-03 11:55:03.000000 pyiArduinoI2Ctds-0.0.5/pyiArduinoI2Ctds.egg-info/PKG-INFO
+-rw-r--r--   0 dron      (1000) dron      (1000)      980 2024-06-03 11:55:03.000000 pyiArduinoI2Ctds-0.0.5/pyiArduinoI2Ctds.egg-info/SOURCES.txt
+-rw-r--r--   0 dron      (1000) dron      (1000)        1 2024-06-03 11:55:03.000000 pyiArduinoI2Ctds-0.0.5/pyiArduinoI2Ctds.egg-info/dependency_links.txt
+-rw-r--r--   0 dron      (1000) dron      (1000)       17 2024-06-03 11:55:03.000000 pyiArduinoI2Ctds-0.0.5/pyiArduinoI2Ctds.egg-info/top_level.txt
+-rw-r--r--   0 dron      (1000) dron      (1000)       79 2024-06-03 11:55:03.917902 pyiArduinoI2Ctds-0.0.5/setup.cfg
+-rw-r--r--   0 dron      (1000) dron      (1000)      708 2024-06-03 11:52:14.000000 pyiArduinoI2Ctds-0.0.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyiArduinoI2Ctds-0.0.3/PKG-INFO` & `pyiArduinoI2Ctds-0.0.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pyiArduinoI2Ctds
-Version: 0.0.3
+Version: 0.0.5
 Summary: iarduino.ru module for Raspberry Pi
 Home-page: http://github.com/tremaru/pyiArduinoI2Ctds
 Author: iarduino.ru
 Author-email: shop@iarduino.ru
 License: MIT
-Description: [![](https://iarduino.ru/img/logo.svg)](https://iarduino.ru)[![](https://wiki.iarduino.ru/img/git-shop.svg?3)](https://iarduino.ru) [![](https://wiki.iarduino.ru/img/git-wiki.svg?2)](https://wiki.iarduino.ru) [![](https://wiki.iarduino.ru/img/git-lesson.svg?2)](https://lesson.iarduino.ru)[![](https://wiki.iarduino.ru/img/git-forum.svg?2)](http://forum.trema.ru)
-        
-        # pyiArduinoI2Ctds
-        
-        **Данная библилотека (модуль для Python3) позволяет управлять электронными модулями (устройствами) [Солемер для воды с щупом TDS и EC-метр , FLASH-I2C](https://iarduino.ru/shop/Sensory-Datchiki/solemer-tds-ec-flash-i2c.html) от iArduino.ru по шине I2C на Raspberry Pi.**
-        
-        Подробнее про датчик читайте в нашей [Wiki](https://wiki.iarduino.ru/page/TDS-EC-i2c-raspberry/)
-        
-        ## Установка ##
-        
-        [Статья на сайте iarduino.ru](https://wiki.iarduino.ru/page/raspberry-python-modules/)
-        
-        Установка из репозиториев PyPI в терминале Raspberry:
-        
-        `sudo pip3 install pyiArduinoI2Ctds`
-        
-        Самостоятельная сборка из исходников:
-        
-        `git clone https://github.com/tremaru/pyiArduinoI2Ctds.git && cd pyiArduinoI2Ctds/pyiArduinoI2Ctds && python3 setup.py build_ext --inplace`
-        
-        Примеры для Python находятся в папке `pyiArduinoI2Ctds/examples`
-        
-        Примеры для С++ находятся в папке `pyiArduinoI2Ctds/cpp`. Так же в этой папке лежит *Makefile* для сборки
-        из исходников. Можно собрать сразу все примеры командой:
-        `make all` или `make`
-        Для сборки конкретного примера: `make "название примера"`
-        Например:
-        `make getData`
-        Для удаления собранных исполняемых файлов:
-        `make clean`
-        
-        **This is a Python3 module for Raspberry Pi. It requieres hardware module <https://iarduino.ru/shop/Sensory-Datchiki/solemer-tds-ec-flash-i2c.html> by iarduino.ru**
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
+License-File: LICENSE
+
+[![](https://iarduino.ru/img/logo.svg)](https://iarduino.ru)[![](https://wiki.iarduino.ru/img/git-shop.svg?3)](https://iarduino.ru) [![](https://wiki.iarduino.ru/img/git-wiki.svg?2)](https://wiki.iarduino.ru) [![](https://wiki.iarduino.ru/img/git-lesson.svg?2)](https://lesson.iarduino.ru)[![](https://wiki.iarduino.ru/img/git-forum.svg?2)](http://forum.trema.ru)
+
+# pyiArduinoI2Ctds
+
+**Данная библилотека (модуль для Python3) позволяет управлять электронными модулями (устройствами) [Солемер для воды с щупом TDS и EC-метр , FLASH-I2C](https://iarduino.ru/shop/Sensory-Datchiki/solemer-tds-ec-flash-i2c.html) от iArduino.ru по шине I2C на Raspberry Pi.**
+
+Подробнее про датчик читайте в нашей [Wiki](https://wiki.iarduino.ru/page/TDS-EC-i2c-raspberry/)
+
+## Установка ##
+
+[Статья на сайте iarduino.ru](https://wiki.iarduino.ru/page/raspberry-python-modules/)
+
+Установка из репозиториев PyPI в терминале Raspberry:
+
+`sudo pip3 install pyiArduinoI2Ctds`
+
+Самостоятельная сборка из исходников:
+
+`git clone https://github.com/tremaru/pyiArduinoI2Ctds.git && cd pyiArduinoI2Ctds/pyiArduinoI2Ctds && python3 setup.py build_ext --inplace`
+
+Примеры для Python находятся в папке `pyiArduinoI2Ctds/examples`
+
+Примеры для С++ находятся в папке `pyiArduinoI2Ctds/cpp`. Так же в этой папке лежит *Makefile* для сборки
+из исходников. Можно собрать сразу все примеры командой:
+`make all` или `make`
+Для сборки конкретного примера: `make "название примера"`
+Например:
+`make getData`
+Для удаления собранных исполняемых файлов:
+`make clean`
+
+**This is a Python3 module for Raspberry Pi. It requieres hardware module <https://iarduino.ru/shop/Sensory-Datchiki/solemer-tds-ec-flash-i2c.html> by iarduino.ru**
```

### Comparing `pyiArduinoI2Ctds-0.0.3/README.md` & `pyiArduinoI2Ctds-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Ctds-0.0.3/pyiArduinoI2Ctds/cpp/FindDevices.cpp` & `pyiArduinoI2Ctds-0.0.5/pyiArduinoI2Ctds/cpp/FindDevices.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Ctds-0.0.3/pyiArduinoI2Ctds/cpp/NewAddress.cpp` & `pyiArduinoI2Ctds-0.0.5/pyiArduinoI2Ctds/cpp/NewAddress.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Ctds-0.0.3/pyiArduinoI2Ctds/cpp/Serial.h` & `pyiArduinoI2Ctds-0.0.5/pyiArduinoI2Ctds/cpp/Serial.h`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Ctds-0.0.3/pyiArduinoI2Ctds/cpp/getData.cpp` & `pyiArduinoI2Ctds-0.0.5/pyiArduinoI2Ctds/cpp/getData.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Ctds-0.0.3/pyiArduinoI2Ctds/cpp/getSettings.cpp` & `pyiArduinoI2Ctds-0.0.5/pyiArduinoI2Ctds/cpp/getSettings.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Ctds-0.0.3/pyiArduinoI2Ctds/cpp/setCalibration.cpp` & `pyiArduinoI2Ctds-0.0.5/pyiArduinoI2Ctds/cpp/setCalibration.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Ctds-0.0.3/pyiArduinoI2Ctds/examples/FindDevices.py` & `pyiArduinoI2Ctds-0.0.5/pyiArduinoI2Ctds/examples/FindDevices.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Ctds-0.0.3/pyiArduinoI2Ctds/examples/getData.py` & `pyiArduinoI2Ctds-0.0.5/pyiArduinoI2Ctds/examples/getData.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Ctds-0.0.3/pyiArduinoI2Ctds/examples/getSettings.py` & `pyiArduinoI2Ctds-0.0.5/pyiArduinoI2Ctds/examples/getSettings.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Ctds-0.0.3/pyiArduinoI2Ctds/examples/newAddress.py` & `pyiArduinoI2Ctds-0.0.5/pyiArduinoI2Ctds/examples/newAddress.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Ctds-0.0.3/pyiArduinoI2Ctds/examples/setCalibration.py` & `pyiArduinoI2Ctds-0.0.5/pyiArduinoI2Ctds/examples/setCalibration.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Ctds-0.0.3/pyiArduinoI2Ctds/examples/setSettings.py` & `pyiArduinoI2Ctds-0.0.5/pyiArduinoI2Ctds/examples/setSettings.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Ctds-0.0.3/pyiArduinoI2Ctds/iarduino_I2C_PI.h` & `pyiArduinoI2Ctds-0.0.5/pyiArduinoI2Ctds/iarduino_I2C_PI.h`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Ctds-0.0.3/pyiArduinoI2Ctds/iarduino_I2C_TDS.cpp` & `pyiArduinoI2Ctds-0.0.5/pyiArduinoI2Ctds/iarduino_I2C_TDS.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Ctds-0.0.3/pyiArduinoI2Ctds/iarduino_I2C_TDS.h` & `pyiArduinoI2Ctds-0.0.5/pyiArduinoI2Ctds/iarduino_I2C_TDS.h`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Ctds-0.0.3/pyiArduinoI2Ctds/iarduino_I2C_TDS.pxd` & `pyiArduinoI2Ctds-0.0.5/pyiArduinoI2Ctds/iarduino_I2C_TDS.pxd`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Ctds-0.0.3/pyiArduinoI2Ctds/pyiArduinoI2Ctds.pyx` & `pyiArduinoI2Ctds-0.0.5/pyiArduinoI2Ctds/pyiArduinoI2Ctds.pyx`

 * *Files identical despite different names*

