# Comparing `tmp/pyiArduinoI2Cph-0.0.3.tar.gz` & `tmp/pyiArduinoI2Cph-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyiArduinoI2Cph-0.0.3.tar", last modified: Wed Apr  6 07:31:32 2022, max compression
+gzip compressed data, was "pyiArduinoI2Cph-0.0.5.tar", last modified: Mon Jun  3 11:54:58 2024, max compression
```

## Comparing `pyiArduinoI2Cph-0.0.3.tar` & `pyiArduinoI2Cph-0.0.5.tar`

### file list

```diff
@@ -1,30 +1,37 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2022-04-06 07:31:32.000000 pyiArduinoI2Cph-0.0.3/
--rw-r--r--   0 pi        (1000) pi        (1000)     2704 2022-04-06 07:31:32.000000 pyiArduinoI2Cph-0.0.3/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)       18 2021-09-08 13:18:41.000000 pyiArduinoI2Cph-0.0.3/README
--rw-r--r--   0 pi        (1000) pi        (1000)     2147 2021-12-23 16:23:07.000000 pyiArduinoI2Cph-0.0.3/README.md
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2022-04-06 07:31:32.000000 pyiArduinoI2Cph-0.0.3/pyiArduinoI2Cph/
--rw-r--r--   0 pi        (1000) pi        (1000)       25 2021-09-08 13:18:41.000000 pyiArduinoI2Cph-0.0.3/pyiArduinoI2Cph/__init__.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2022-04-06 07:31:32.000000 pyiArduinoI2Cph-0.0.3/pyiArduinoI2Cph/cpp/
--rw-r--r--   0 pi        (1000) pi        (1000)     9722 2021-09-08 13:18:41.000000 pyiArduinoI2Cph-0.0.3/pyiArduinoI2Cph/cpp/FindDevices.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)     1486 2021-09-08 13:18:41.000000 pyiArduinoI2Cph-0.0.3/pyiArduinoI2Cph/cpp/NewAddress.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)      517 2021-09-15 06:59:06.000000 pyiArduinoI2Cph-0.0.3/pyiArduinoI2Cph/cpp/Serial.h
--rw-r--r--   0 pi        (1000) pi        (1000)     1476 2021-09-15 07:03:22.000000 pyiArduinoI2Cph-0.0.3/pyiArduinoI2Cph/cpp/getData.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)     2076 2021-12-22 15:46:44.000000 pyiArduinoI2Cph-0.0.3/pyiArduinoI2Cph/cpp/getFunction.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)     2288 2021-12-22 15:50:11.000000 pyiArduinoI2Cph-0.0.3/pyiArduinoI2Cph/cpp/getSettings.cpp
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2022-04-06 07:31:32.000000 pyiArduinoI2Cph-0.0.3/pyiArduinoI2Cph/examples/
--rw-r--r--   0 pi        (1000) pi        (1000)     7782 2021-09-14 12:15:31.000000 pyiArduinoI2Cph-0.0.3/pyiArduinoI2Cph/examples/FindDevices.py
--rw-r--r--   0 pi        (1000) pi        (1000)      638 2022-04-06 07:14:28.000000 pyiArduinoI2Cph-0.0.3/pyiArduinoI2Cph/examples/getData.py
--rw-r--r--   0 pi        (1000) pi        (1000)     1203 2021-12-22 16:05:50.000000 pyiArduinoI2Cph-0.0.3/pyiArduinoI2Cph/examples/getFunction.py
--rw-r--r--   0 pi        (1000) pi        (1000)     1793 2021-12-22 16:07:58.000000 pyiArduinoI2Cph-0.0.3/pyiArduinoI2Cph/examples/getSettings.py
--rw-r--r--   0 pi        (1000) pi        (1000)     1377 2021-09-08 13:18:41.000000 pyiArduinoI2Cph-0.0.3/pyiArduinoI2Cph/examples/newAddress.py
--rw-r--r--   0 pi        (1000) pi        (1000)     1278 2021-12-23 13:11:37.000000 pyiArduinoI2Cph-0.0.3/pyiArduinoI2Cph/examples/setCalibration.py
--rw-r--r--   0 pi        (1000) pi        (1000)      848 2021-12-24 10:53:00.000000 pyiArduinoI2Cph-0.0.3/pyiArduinoI2Cph/examples/setSettings.py
--rw-r--r--   0 pi        (1000) pi        (1000)    10952 2021-09-15 07:08:26.000000 pyiArduinoI2Cph-0.0.3/pyiArduinoI2Cph/iarduino_I2C_PI.h
--rw-r--r--   0 pi        (1000) pi        (1000)    39188 2022-04-06 07:18:48.000000 pyiArduinoI2Cph-0.0.3/pyiArduinoI2Cph/iarduino_I2C_pH.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)    21075 2022-04-06 07:17:54.000000 pyiArduinoI2Cph-0.0.3/pyiArduinoI2Cph/iarduino_I2C_pH.h
--rw-r--r--   0 pi        (1000) pi        (1000)      849 2022-04-06 07:20:05.000000 pyiArduinoI2Cph-0.0.3/pyiArduinoI2Cph/iarduino_I2C_pH.pxd
--rw-r--r--   0 pi        (1000) pi        (1000)   233939 2022-04-06 07:21:38.000000 pyiArduinoI2Cph-0.0.3/pyiArduinoI2Cph/pyiArduinoI2Cph.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)     4046 2022-04-06 07:21:05.000000 pyiArduinoI2Cph-0.0.3/pyiArduinoI2Cph/pyiArduinoI2Cph.pyx
--rw-r--r--   0 pi        (1000) pi        (1000)      128 2021-09-08 13:18:41.000000 pyiArduinoI2Cph-0.0.3/pyiArduinoI2Cph/setup.py
--rw-r--r--   0 pi        (1000) pi        (1000)       40 2021-09-08 13:18:41.000000 pyiArduinoI2Cph-0.0.3/setup.cfg
--rw-r--r--   0 pi        (1000) pi        (1000)      703 2022-04-06 07:31:26.000000 pyiArduinoI2Cph-0.0.3/setup.py
+drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-06-03 11:54:58.725972 pyiArduinoI2Cph-0.0.5/
+-rw-r--r--   0 dron      (1000) dron      (1000)     3291 2024-03-29 13:35:08.000000 pyiArduinoI2Cph-0.0.5/LICENSE
+-rw-r--r--   0 dron      (1000) dron      (1000)       80 2024-03-29 13:35:08.000000 pyiArduinoI2Cph-0.0.5/MANIFEST.in
+-rw-r--r--   0 dron      (1000) dron      (1000)     2439 2024-06-03 11:54:58.725972 pyiArduinoI2Cph-0.0.5/PKG-INFO
+-rw-r--r--   0 dron      (1000) dron      (1000)       18 2024-03-29 13:35:08.000000 pyiArduinoI2Cph-0.0.5/README
+-rw-r--r--   0 dron      (1000) dron      (1000)     2147 2024-03-29 13:35:08.000000 pyiArduinoI2Cph-0.0.5/README.md
+drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-06-03 11:54:58.717972 pyiArduinoI2Cph-0.0.5/pyiArduinoI2Cph/
+-rw-r--r--   0 dron      (1000) dron      (1000)       25 2024-03-29 13:35:08.000000 pyiArduinoI2Cph-0.0.5/pyiArduinoI2Cph/__init__.py
+drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-06-03 11:54:58.721972 pyiArduinoI2Cph-0.0.5/pyiArduinoI2Cph/cpp/
+-rw-r--r--   0 dron      (1000) dron      (1000)     9722 2024-03-29 13:35:08.000000 pyiArduinoI2Cph-0.0.5/pyiArduinoI2Cph/cpp/FindDevices.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     1486 2024-03-29 13:35:08.000000 pyiArduinoI2Cph-0.0.5/pyiArduinoI2Cph/cpp/NewAddress.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)      517 2024-03-29 13:35:08.000000 pyiArduinoI2Cph-0.0.5/pyiArduinoI2Cph/cpp/Serial.h
+-rw-r--r--   0 dron      (1000) dron      (1000)     1476 2024-03-29 13:35:08.000000 pyiArduinoI2Cph-0.0.5/pyiArduinoI2Cph/cpp/getData.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     2076 2024-03-29 13:35:08.000000 pyiArduinoI2Cph-0.0.5/pyiArduinoI2Cph/cpp/getFunction.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     2288 2024-03-29 13:35:08.000000 pyiArduinoI2Cph-0.0.5/pyiArduinoI2Cph/cpp/getSettings.cpp
+drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-06-03 11:54:58.725972 pyiArduinoI2Cph-0.0.5/pyiArduinoI2Cph/examples/
+-rw-r--r--   0 dron      (1000) dron      (1000)     7782 2024-03-29 13:35:08.000000 pyiArduinoI2Cph-0.0.5/pyiArduinoI2Cph/examples/FindDevices.py
+-rw-r--r--   0 dron      (1000) dron      (1000)      638 2024-03-29 13:35:08.000000 pyiArduinoI2Cph-0.0.5/pyiArduinoI2Cph/examples/getData.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     1203 2024-03-29 13:35:08.000000 pyiArduinoI2Cph-0.0.5/pyiArduinoI2Cph/examples/getFunction.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     1793 2024-03-29 13:35:08.000000 pyiArduinoI2Cph-0.0.5/pyiArduinoI2Cph/examples/getSettings.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     1377 2024-03-29 13:35:08.000000 pyiArduinoI2Cph-0.0.5/pyiArduinoI2Cph/examples/newAddress.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     1278 2024-03-29 13:35:08.000000 pyiArduinoI2Cph-0.0.5/pyiArduinoI2Cph/examples/setCalibration.py
+-rw-r--r--   0 dron      (1000) dron      (1000)      848 2024-03-29 13:35:08.000000 pyiArduinoI2Cph-0.0.5/pyiArduinoI2Cph/examples/setSettings.py
+-rw-r--r--   0 dron      (1000) dron      (1000)    10952 2024-03-29 13:35:08.000000 pyiArduinoI2Cph-0.0.5/pyiArduinoI2Cph/iarduino_I2C_PI.h
+-rw-r--r--   0 dron      (1000) dron      (1000)    39188 2024-03-29 13:35:08.000000 pyiArduinoI2Cph-0.0.5/pyiArduinoI2Cph/iarduino_I2C_pH.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)    21075 2024-03-29 13:35:08.000000 pyiArduinoI2Cph-0.0.5/pyiArduinoI2Cph/iarduino_I2C_pH.h
+-rw-r--r--   0 dron      (1000) dron      (1000)      849 2024-03-29 13:35:08.000000 pyiArduinoI2Cph-0.0.5/pyiArduinoI2Cph/iarduino_I2C_pH.pxd
+-rw-r--r--   0 dron      (1000) dron      (1000)   508568 2024-06-03 11:48:57.000000 pyiArduinoI2Cph-0.0.5/pyiArduinoI2Cph/pyiArduinoI2Cph.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     4046 2024-03-29 13:35:08.000000 pyiArduinoI2Cph-0.0.5/pyiArduinoI2Cph/pyiArduinoI2Cph.pyx
+-rw-r--r--   0 dron      (1000) dron      (1000)      128 2024-03-29 13:35:08.000000 pyiArduinoI2Cph-0.0.5/pyiArduinoI2Cph/setup.py
+drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-06-03 11:54:58.717972 pyiArduinoI2Cph-0.0.5/pyiArduinoI2Cph.egg-info/
+-rw-r--r--   0 dron      (1000) dron      (1000)     2439 2024-06-03 11:54:58.000000 pyiArduinoI2Cph-0.0.5/pyiArduinoI2Cph.egg-info/PKG-INFO
+-rw-r--r--   0 dron      (1000) dron      (1000)      958 2024-06-03 11:54:58.000000 pyiArduinoI2Cph-0.0.5/pyiArduinoI2Cph.egg-info/SOURCES.txt
+-rw-r--r--   0 dron      (1000) dron      (1000)        1 2024-06-03 11:54:58.000000 pyiArduinoI2Cph-0.0.5/pyiArduinoI2Cph.egg-info/dependency_links.txt
+-rw-r--r--   0 dron      (1000) dron      (1000)       16 2024-06-03 11:54:58.000000 pyiArduinoI2Cph-0.0.5/pyiArduinoI2Cph.egg-info/top_level.txt
+-rw-r--r--   0 dron      (1000) dron      (1000)       79 2024-06-03 11:54:58.729972 pyiArduinoI2Cph-0.0.5/setup.cfg
+-rw-r--r--   0 dron      (1000) dron      (1000)      703 2024-06-03 11:51:55.000000 pyiArduinoI2Cph-0.0.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyiArduinoI2Cph-0.0.3/PKG-INFO` & `pyiArduinoI2Cph-0.0.5/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,32 @@
-Metadata-Version: 1.1
-Name: pyiArduinoI2Cph
-Version: 0.0.3
-Summary: iarduino.ru module for Raspberry Pi
-Home-page: http://github.com/tremaru/pyiArduinoI2Cph
-Author: iarduino.ru
-Author-email: shop@iarduino.ru
-License: MIT
-Description: [![](https://iarduino.ru/img/logo.svg)](https://iarduino.ru)[![](https://wiki.iarduino.ru/img/git-shop.svg?3)](https://iarduino.ru) [![](https://wiki.iarduino.ru/img/git-wiki.svg?2)](https://wiki.iarduino.ru) [![](https://wiki.iarduino.ru/img/git-lesson.svg?2)](https://lesson.iarduino.ru)[![](https://wiki.iarduino.ru/img/git-forum.svg?2)](http://forum.trema.ru)
-        
-        # pyiArduinoI2Cph
-        
-        **Данная библилотека (модуль для Python3) позволяет управлять электронными модулями (устройствами) [Trema модуль pH-метр](https://iarduino.ru/shop/Sensory-Datchiki/datchik-kislotnosti-zhidkosti-ph-metr-flash-i2c.html) от iArduino.ru по шине I2C на Raspberry Pi.**
-        
-        Подробнее про датчик читайте в нашей [Wiki](https://wiki.iarduino.ru/page/ph-i2c-raspberry)
-        
-        ## Установка ##
-        
-        [Статья на сайте iarduino.ru](https://wiki.iarduino.ru/page/raspberry-python-modules/)
-        
-        Установка из репозиториев PyPI в терминале Raspberry:
-        
-        `sudo pip3 install pyiArduinoI2Cph`
-        
-        Самостоятельная сборка из исходников:
-        
-        `git clone https://github.com/tremaru/pyiArduinoI2Cph.git && cd pyiArduinoI2Cph/pyiArduinoI2Cph && python3 setup.py build_ext --inplace`
-        
-        Примеры для Python находятся в папке `pyiArduinoI2Cph/examples`
-        
-        Примеры для С++ находятся в папке `pyiArduinoI2Cph/cpp`. Так же в этой папке лежит *Makefile* для сборки
-        из исходников. Можно собрать сразу все примеры командой:
-        `make all` или `make`
-        Для сборки конкретного примера: `make "название примера"`
-        Например:
-        `make getData`
-        Для удаления собранных исполняемых файлов:
-        `make clean`
-        
-        **This is a Python3 module for Raspberry Pi. It can work with [Trema module pH-meter, Flash-I2C](https://iarduino.ru/shop/Sensory-Datchiki/datchik-kislotnosti-zhidkosti-ph-metr-flash-i2c.html) by iarduino.ru**
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
+[![](https://iarduino.ru/img/logo.svg)](https://iarduino.ru)[![](https://wiki.iarduino.ru/img/git-shop.svg?3)](https://iarduino.ru) [![](https://wiki.iarduino.ru/img/git-wiki.svg?2)](https://wiki.iarduino.ru) [![](https://wiki.iarduino.ru/img/git-lesson.svg?2)](https://lesson.iarduino.ru)[![](https://wiki.iarduino.ru/img/git-forum.svg?2)](http://forum.trema.ru)
+
+# pyiArduinoI2Cph
+
+**Данная библилотека (модуль для Python3) позволяет управлять электронными модулями (устройствами) [Trema модуль pH-метр](https://iarduino.ru/shop/Sensory-Datchiki/datchik-kislotnosti-zhidkosti-ph-metr-flash-i2c.html) от iArduino.ru по шине I2C на Raspberry Pi.**
+
+Подробнее про датчик читайте в нашей [Wiki](https://wiki.iarduino.ru/page/ph-i2c-raspberry)
+
+## Установка ##
+
+[Статья на сайте iarduino.ru](https://wiki.iarduino.ru/page/raspberry-python-modules/)
+
+Установка из репозиториев PyPI в терминале Raspberry:
+
+`sudo pip3 install pyiArduinoI2Cph`
+
+Самостоятельная сборка из исходников:
+
+`git clone https://github.com/tremaru/pyiArduinoI2Cph.git && cd pyiArduinoI2Cph/pyiArduinoI2Cph && python3 setup.py build_ext --inplace`
+
+Примеры для Python находятся в папке `pyiArduinoI2Cph/examples`
+
+Примеры для С++ находятся в папке `pyiArduinoI2Cph/cpp`. Так же в этой папке лежит *Makefile* для сборки
+из исходников. Можно собрать сразу все примеры командой:
+`make all` или `make`
+Для сборки конкретного примера: `make "название примера"`
+Например:
+`make getData`
+Для удаления собранных исполняемых файлов:
+`make clean`
+
+**This is a Python3 module for Raspberry Pi. It can work with [Trema module pH-meter, Flash-I2C](https://iarduino.ru/shop/Sensory-Datchiki/datchik-kislotnosti-zhidkosti-ph-metr-flash-i2c.html) by iarduino.ru**
```

### Comparing `pyiArduinoI2Cph-0.0.3/README.md` & `pyiArduinoI2Cph-0.0.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: pyiArduinoI2Cph
+Version: 0.0.5
+Summary: iarduino.ru module for Raspberry Pi
+Home-page: http://github.com/tremaru/pyiArduinoI2Cph
+Author: iarduino.ru
+Author-email: shop@iarduino.ru
+License: MIT
+Classifier: Programming Language :: Python :: 3
+License-File: LICENSE
+
 [![](https://iarduino.ru/img/logo.svg)](https://iarduino.ru)[![](https://wiki.iarduino.ru/img/git-shop.svg?3)](https://iarduino.ru) [![](https://wiki.iarduino.ru/img/git-wiki.svg?2)](https://wiki.iarduino.ru) [![](https://wiki.iarduino.ru/img/git-lesson.svg?2)](https://lesson.iarduino.ru)[![](https://wiki.iarduino.ru/img/git-forum.svg?2)](http://forum.trema.ru)
 
 # pyiArduinoI2Cph
 
 **Данная библилотека (модуль для Python3) позволяет управлять электронными модулями (устройствами) [Trema модуль pH-метр](https://iarduino.ru/shop/Sensory-Datchiki/datchik-kislotnosti-zhidkosti-ph-metr-flash-i2c.html) от iArduino.ru по шине I2C на Raspberry Pi.**
 
 Подробнее про датчик читайте в нашей [Wiki](https://wiki.iarduino.ru/page/ph-i2c-raspberry)
```

### Comparing `pyiArduinoI2Cph-0.0.3/pyiArduinoI2Cph/cpp/FindDevices.cpp` & `pyiArduinoI2Cph-0.0.5/pyiArduinoI2Cph/cpp/FindDevices.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cph-0.0.3/pyiArduinoI2Cph/cpp/NewAddress.cpp` & `pyiArduinoI2Cph-0.0.5/pyiArduinoI2Cph/cpp/NewAddress.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cph-0.0.3/pyiArduinoI2Cph/cpp/Serial.h` & `pyiArduinoI2Cph-0.0.5/pyiArduinoI2Cph/cpp/Serial.h`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cph-0.0.3/pyiArduinoI2Cph/cpp/getData.cpp` & `pyiArduinoI2Cph-0.0.5/pyiArduinoI2Cph/cpp/getData.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cph-0.0.3/pyiArduinoI2Cph/cpp/getFunction.cpp` & `pyiArduinoI2Cph-0.0.5/pyiArduinoI2Cph/cpp/getFunction.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cph-0.0.3/pyiArduinoI2Cph/cpp/getSettings.cpp` & `pyiArduinoI2Cph-0.0.5/pyiArduinoI2Cph/cpp/getSettings.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cph-0.0.3/pyiArduinoI2Cph/examples/FindDevices.py` & `pyiArduinoI2Cph-0.0.5/pyiArduinoI2Cph/examples/FindDevices.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cph-0.0.3/pyiArduinoI2Cph/examples/getData.py` & `pyiArduinoI2Cph-0.0.5/pyiArduinoI2Cph/examples/getData.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cph-0.0.3/pyiArduinoI2Cph/examples/getFunction.py` & `pyiArduinoI2Cph-0.0.5/pyiArduinoI2Cph/examples/getFunction.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cph-0.0.3/pyiArduinoI2Cph/examples/getSettings.py` & `pyiArduinoI2Cph-0.0.5/pyiArduinoI2Cph/examples/getSettings.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cph-0.0.3/pyiArduinoI2Cph/examples/newAddress.py` & `pyiArduinoI2Cph-0.0.5/pyiArduinoI2Cph/examples/newAddress.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cph-0.0.3/pyiArduinoI2Cph/examples/setCalibration.py` & `pyiArduinoI2Cph-0.0.5/pyiArduinoI2Cph/examples/setCalibration.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cph-0.0.3/pyiArduinoI2Cph/examples/setSettings.py` & `pyiArduinoI2Cph-0.0.5/pyiArduinoI2Cph/examples/setSettings.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cph-0.0.3/pyiArduinoI2Cph/iarduino_I2C_PI.h` & `pyiArduinoI2Cph-0.0.5/pyiArduinoI2Cph/iarduino_I2C_PI.h`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cph-0.0.3/pyiArduinoI2Cph/iarduino_I2C_pH.cpp` & `pyiArduinoI2Cph-0.0.5/pyiArduinoI2Cph/iarduino_I2C_pH.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cph-0.0.3/pyiArduinoI2Cph/iarduino_I2C_pH.h` & `pyiArduinoI2Cph-0.0.5/pyiArduinoI2Cph/iarduino_I2C_pH.h`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cph-0.0.3/pyiArduinoI2Cph/iarduino_I2C_pH.pxd` & `pyiArduinoI2Cph-0.0.5/pyiArduinoI2Cph/iarduino_I2C_pH.pxd`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cph-0.0.3/pyiArduinoI2Cph/pyiArduinoI2Cph.pyx` & `pyiArduinoI2Cph-0.0.5/pyiArduinoI2Cph/pyiArduinoI2Cph.pyx`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cph-0.0.3/setup.py` & `pyiArduinoI2Cph-0.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from distutils.extension import Extension
 
 def readme():
     with open('README.md') as readme:
         return readme.read()
 
 setup(name='pyiArduinoI2Cph',
-    version='0.0.3',
+    version='0.0.5',
     description='iarduino.ru module for Raspberry Pi',
     long_description=readme(),
     classifiers=[
         'Programming Language :: Python :: 3',
     ],
     url='http://github.com/tremaru/pyiArduinoI2Cph',
     author='iarduino.ru',
```

