# Comparing `tmp/pyiArduinoI2Csht-1.0.0.tar.gz` & `tmp/pyiArduinoI2Csht-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyiArduinoI2Csht-1.0.0.tar", last modified: Mon Dec  2 10:11:28 2019, max compression
+gzip compressed data, was "pyiArduinoI2Csht-1.0.2.tar", last modified: Mon Jun  3 11:55:02 2024, max compression
```

## Comparing `pyiArduinoI2Csht-1.0.0.tar` & `pyiArduinoI2Csht-1.0.2.tar`

### file list

```diff
@@ -1,21 +1,34 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2019-12-02 10:11:28.000000 pyiArduinoI2Csht-1.0.0/
--rw-r--r--   0 pi        (1000) pi        (1000)     2763 2019-12-02 10:11:28.000000 pyiArduinoI2Csht-1.0.0/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)       19 2019-11-27 13:17:35.000000 pyiArduinoI2Csht-1.0.0/README
--rw-r--r--   0 pi        (1000) pi        (1000)     2204 2019-11-28 13:54:16.000000 pyiArduinoI2Csht-1.0.0/README.md
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2019-12-02 10:11:28.000000 pyiArduinoI2Csht-1.0.0/pyiArduinoI2Csht/
--rw-r--r--   0 pi        (1000) pi        (1000)       26 2019-11-27 13:38:45.000000 pyiArduinoI2Csht-1.0.0/pyiArduinoI2Csht/__init__.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2019-12-02 10:11:28.000000 pyiArduinoI2Csht-1.0.0/pyiArduinoI2Csht/examples/
--rw-r--r--   0 pi        (1000) pi        (1000)     5581 2019-11-28 11:47:45.000000 pyiArduinoI2Csht-1.0.0/pyiArduinoI2Csht/examples/FindDevices.py
--rw-r--r--   0 pi        (1000) pi        (1000)      952 2019-11-28 11:22:58.000000 pyiArduinoI2Csht-1.0.0/pyiArduinoI2Csht/examples/getAll.py
--rw-r--r--   0 pi        (1000) pi        (1000)     1906 2019-11-28 11:11:02.000000 pyiArduinoI2Csht-1.0.0/pyiArduinoI2Csht/examples/getAllChanged.py
--rw-r--r--   0 pi        (1000) pi        (1000)     1345 2019-11-28 11:40:25.000000 pyiArduinoI2Csht-1.0.0/pyiArduinoI2Csht/examples/newAddress.py
--rw-r--r--   0 pi        (1000) pi        (1000)     1052 2019-11-28 11:45:51.000000 pyiArduinoI2Csht-1.0.0/pyiArduinoI2Csht/examples/setPeriod.py
--rwxr-xr-x   0 pi        (1000) pi        (1000)    13219 2019-11-28 08:33:27.000000 pyiArduinoI2Csht-1.0.0/pyiArduinoI2Csht/iarduino_I2C_PI.h
--rw-r--r--   0 pi        (1000) pi        (1000)    24463 2019-11-27 13:10:03.000000 pyiArduinoI2Csht-1.0.0/pyiArduinoI2Csht/iarduino_I2C_SHT.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)    13596 2019-11-28 10:09:13.000000 pyiArduinoI2Csht-1.0.0/pyiArduinoI2Csht/iarduino_I2C_SHT.h
--rw-r--r--   0 pi        (1000) pi        (1000)      565 2019-11-27 15:00:46.000000 pyiArduinoI2Csht-1.0.0/pyiArduinoI2Csht/iarduino_I2C_SHT.pxd
--rw-r--r--   0 pi        (1000) pi        (1000)   202809 2019-11-27 15:00:58.000000 pyiArduinoI2Csht-1.0.0/pyiArduinoI2Csht/pyiArduinoI2Csht.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)     3190 2019-11-27 15:00:45.000000 pyiArduinoI2Csht-1.0.0/pyiArduinoI2Csht/pyiArduinoI2Csht.pyx
--rw-r--r--   0 pi        (1000) pi        (1000)      129 2019-11-27 13:40:15.000000 pyiArduinoI2Csht-1.0.0/pyiArduinoI2Csht/setup.py
--rw-r--r--   0 pi        (1000) pi        (1000)       40 2019-11-27 13:13:29.000000 pyiArduinoI2Csht-1.0.0/setup.cfg
--rw-r--r--   0 pi        (1000) pi        (1000)      747 2019-12-02 10:07:37.000000 pyiArduinoI2Csht-1.0.0/setup.py
+drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-06-03 11:55:02.177925 pyiArduinoI2Csht-1.0.2/
+-rw-r--r--   0 dron      (1000) dron      (1000)     3289 2024-03-29 13:35:20.000000 pyiArduinoI2Csht-1.0.2/LICENSE
+-rw-r--r--   0 dron      (1000) dron      (1000)       81 2024-03-29 13:35:20.000000 pyiArduinoI2Csht-1.0.2/MANIFEST.in
+-rw-r--r--   0 dron      (1000) dron      (1000)     2498 2024-06-03 11:55:02.177925 pyiArduinoI2Csht-1.0.2/PKG-INFO
+-rw-r--r--   0 dron      (1000) dron      (1000)       19 2024-03-29 13:35:20.000000 pyiArduinoI2Csht-1.0.2/README
+-rw-r--r--   0 dron      (1000) dron      (1000)     2204 2024-03-29 13:35:20.000000 pyiArduinoI2Csht-1.0.2/README.md
+drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-06-03 11:55:02.169926 pyiArduinoI2Csht-1.0.2/pyiArduinoI2Csht/
+-rw-r--r--   0 dron      (1000) dron      (1000)       26 2024-03-29 13:35:20.000000 pyiArduinoI2Csht-1.0.2/pyiArduinoI2Csht/__init__.py
+drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-06-03 11:55:02.173925 pyiArduinoI2Csht-1.0.2/pyiArduinoI2Csht/cpp/
+-rw-r--r--   0 dron      (1000) dron      (1000)     9722 2024-03-29 13:35:20.000000 pyiArduinoI2Csht-1.0.2/pyiArduinoI2Csht/cpp/FindDevices.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     1473 2024-03-29 13:35:20.000000 pyiArduinoI2Csht-1.0.2/pyiArduinoI2Csht/cpp/NewAddress.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)      499 2024-03-29 13:35:20.000000 pyiArduinoI2Csht-1.0.2/pyiArduinoI2Csht/cpp/getAll.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)      741 2024-03-29 13:35:20.000000 pyiArduinoI2Csht-1.0.2/pyiArduinoI2Csht/cpp/getAllChanged.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)      454 2024-03-29 13:35:20.000000 pyiArduinoI2Csht-1.0.2/pyiArduinoI2Csht/cpp/setPeriod.cpp
+drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-06-03 11:55:02.177925 pyiArduinoI2Csht-1.0.2/pyiArduinoI2Csht/examples/
+-rw-r--r--   0 dron      (1000) dron      (1000)     5581 2024-03-29 13:35:20.000000 pyiArduinoI2Csht-1.0.2/pyiArduinoI2Csht/examples/FindDevices.py
+-rw-r--r--   0 dron      (1000) dron      (1000)      952 2024-03-29 13:35:20.000000 pyiArduinoI2Csht-1.0.2/pyiArduinoI2Csht/examples/getAll.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     1900 2024-03-29 13:35:20.000000 pyiArduinoI2Csht-1.0.2/pyiArduinoI2Csht/examples/getAllChanged.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     1359 2024-03-29 13:35:20.000000 pyiArduinoI2Csht-1.0.2/pyiArduinoI2Csht/examples/newAddress.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     1057 2024-03-29 13:35:20.000000 pyiArduinoI2Csht-1.0.2/pyiArduinoI2Csht/examples/setPeriod.py
+-rwxr-xr-x   0 dron      (1000) dron      (1000)    13219 2024-03-29 13:35:20.000000 pyiArduinoI2Csht-1.0.2/pyiArduinoI2Csht/iarduino_I2C_PI.h
+-rw-r--r--   0 dron      (1000) dron      (1000)    24463 2024-03-29 13:35:20.000000 pyiArduinoI2Csht-1.0.2/pyiArduinoI2Csht/iarduino_I2C_SHT.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)    13596 2024-03-29 13:35:20.000000 pyiArduinoI2Csht-1.0.2/pyiArduinoI2Csht/iarduino_I2C_SHT.h
+-rw-r--r--   0 dron      (1000) dron      (1000)      565 2024-03-29 13:35:20.000000 pyiArduinoI2Csht-1.0.2/pyiArduinoI2Csht/iarduino_I2C_SHT.pxd
+-rw-r--r--   0 dron      (1000) dron      (1000)   436189 2024-06-03 11:49:26.000000 pyiArduinoI2Csht-1.0.2/pyiArduinoI2Csht/pyiArduinoI2Csht.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     3190 2024-03-29 13:35:20.000000 pyiArduinoI2Csht-1.0.2/pyiArduinoI2Csht/pyiArduinoI2Csht.pyx
+-rw-r--r--   0 dron      (1000) dron      (1000)      129 2024-03-29 13:35:20.000000 pyiArduinoI2Csht-1.0.2/pyiArduinoI2Csht/setup.py
+drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-06-03 11:55:02.173925 pyiArduinoI2Csht-1.0.2/pyiArduinoI2Csht.egg-info/
+-rw-r--r--   0 dron      (1000) dron      (1000)     2498 2024-06-03 11:55:01.000000 pyiArduinoI2Csht-1.0.2/pyiArduinoI2Csht.egg-info/PKG-INFO
+-rw-r--r--   0 dron      (1000) dron      (1000)      871 2024-06-03 11:55:02.000000 pyiArduinoI2Csht-1.0.2/pyiArduinoI2Csht.egg-info/SOURCES.txt
+-rw-r--r--   0 dron      (1000) dron      (1000)        1 2024-06-03 11:55:01.000000 pyiArduinoI2Csht-1.0.2/pyiArduinoI2Csht.egg-info/dependency_links.txt
+-rw-r--r--   0 dron      (1000) dron      (1000)       17 2024-06-03 11:55:01.000000 pyiArduinoI2Csht-1.0.2/pyiArduinoI2Csht.egg-info/top_level.txt
+-rw-r--r--   0 dron      (1000) dron      (1000)       79 2024-06-03 11:55:02.181925 pyiArduinoI2Csht-1.0.2/setup.cfg
+-rw-r--r--   0 dron      (1000) dron      (1000)      747 2024-06-03 11:52:07.000000 pyiArduinoI2Csht-1.0.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyiArduinoI2Csht-1.0.0/PKG-INFO` & `pyiArduinoI2Csht-1.0.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,32 @@
-Metadata-Version: 1.1
-Name: pyiArduinoI2Csht
-Version: 1.0.0
-Summary: iarduino.ru module for Raspberry Pi
-Home-page: http://github.com/tremaru/pyiArduinoI2Csht
-Author: iarduino.ru
-Author-email: shop@iarduino.ru
-License: MIT
-Description: [![](https://iarduino.ru/img/logo.svg)](https://iarduino.ru)[![](https://wiki.iarduino.ru/img/git-shop.svg?3)](https://iarduino.ru) [![](https://wiki.iarduino.ru/img/git-wiki.svg?2)](https://wiki.iarduino.ru) [![](https://wiki.iarduino.ru/img/git-lesson.svg?2)](https://lesson.iarduino.ru)[![](https://wiki.iarduino.ru/img/git-forum.svg?2)](http://forum.trema.ru)
-        
-        # pyiArduinoI2Csht
-        
-        **Данная библилотека (модуль для Python3) позволяет управлять электронными модулями (устройствами) [Цифровой датчик температуры и влажности](https://iarduino.ru/shop/Sensory-Datchiki/datchik-temperatury-i-vlazhnosti-i2c-trema-modul-v2-0.html) от iArduino.ru по шине I2C на Raspberry Pi.**
-        
-        Подробнее про датчик читайте в нашей [Wiki](https://wiki.iarduino.ru/page/SHT-trema-i2c/#h3_5)
-        
-        ## Установка ##
-        
-        [Статья на сайте iarduino.ru](https://wiki.iarduino.ru/page/raspberry-python-modules/)
-        
-        Установка из репозиториев PyPI в терминале Raspberry:
-        
-        `sudo pip3 install pyiArduinoI2Csht`
-        
-        Самостоятельная сборка из исходников:
-        
-        `git clone https://github.com/tremaru/pyiArduinoI2Csht.git && cd pyiArduinoI2Csht/pyiArduinoI2Csht && python3 setup.py build_ext --inplace`
-        
-        Примеры для Python находятся в папке `pyiArduinoI2Csht/examples`
-        
-        Примеры для С++ находятся в папке `pyiArduinoI2Csht/cpp`. Так же в этой папке лежит *Makefile* для сборки
-        из исходников. Можно собрать сразу все примеры командой:
-        `make all` или `make`
-        Для сборки конкретного примера: `make "название примера"`
-        Например:
-        `make reset`
-        Для удаления собранных исполняемых файлов:
-        `make clean`
-        
-        **This is a Python3 module for Raspberry Pi. It can work with [Digital tempreture sensor](https://iarduino.ru/shop/Sensory-Datchiki/datchik-temperatury-i-vlazhnosti-i2c-trema-modul-v2-0.html) by iarduino.ru**
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
+[![](https://iarduino.ru/img/logo.svg)](https://iarduino.ru)[![](https://wiki.iarduino.ru/img/git-shop.svg?3)](https://iarduino.ru) [![](https://wiki.iarduino.ru/img/git-wiki.svg?2)](https://wiki.iarduino.ru) [![](https://wiki.iarduino.ru/img/git-lesson.svg?2)](https://lesson.iarduino.ru)[![](https://wiki.iarduino.ru/img/git-forum.svg?2)](http://forum.trema.ru)
+
+# pyiArduinoI2Csht
+
+**Данная библилотека (модуль для Python3) позволяет управлять электронными модулями (устройствами) [Цифровой датчик температуры и влажности](https://iarduino.ru/shop/Sensory-Datchiki/datchik-temperatury-i-vlazhnosti-i2c-trema-modul-v2-0.html) от iArduino.ru по шине I2C на Raspberry Pi.**
+
+Подробнее про датчик читайте в нашей [Wiki](https://wiki.iarduino.ru/page/SHT-trema-i2c/#h3_5)
+
+## Установка ##
+
+[Статья на сайте iarduino.ru](https://wiki.iarduino.ru/page/raspberry-python-modules/)
+
+Установка из репозиториев PyPI в терминале Raspberry:
+
+`sudo pip3 install pyiArduinoI2Csht`
+
+Самостоятельная сборка из исходников:
+
+`git clone https://github.com/tremaru/pyiArduinoI2Csht.git && cd pyiArduinoI2Csht/pyiArduinoI2Csht && python3 setup.py build_ext --inplace`
+
+Примеры для Python находятся в папке `pyiArduinoI2Csht/examples`
+
+Примеры для С++ находятся в папке `pyiArduinoI2Csht/cpp`. Так же в этой папке лежит *Makefile* для сборки
+из исходников. Можно собрать сразу все примеры командой:
+`make all` или `make`
+Для сборки конкретного примера: `make "название примера"`
+Например:
+`make reset`
+Для удаления собранных исполняемых файлов:
+`make clean`
+
+**This is a Python3 module for Raspberry Pi. It can work with [Digital tempreture sensor](https://iarduino.ru/shop/Sensory-Datchiki/datchik-temperatury-i-vlazhnosti-i2c-trema-modul-v2-0.html) by iarduino.ru**
```

### Comparing `pyiArduinoI2Csht-1.0.0/README.md` & `pyiArduinoI2Csht-1.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: pyiArduinoI2Csht
+Version: 1.0.2
+Summary: iarduino.ru module for Raspberry Pi
+Home-page: http://github.com/tremaru/pyiArduinoI2Csht
+Author: iarduino.ru
+Author-email: shop@iarduino.ru
+License: MIT
+Classifier: Programming Language :: Python :: 3
+License-File: LICENSE
+
 [![](https://iarduino.ru/img/logo.svg)](https://iarduino.ru)[![](https://wiki.iarduino.ru/img/git-shop.svg?3)](https://iarduino.ru) [![](https://wiki.iarduino.ru/img/git-wiki.svg?2)](https://wiki.iarduino.ru) [![](https://wiki.iarduino.ru/img/git-lesson.svg?2)](https://lesson.iarduino.ru)[![](https://wiki.iarduino.ru/img/git-forum.svg?2)](http://forum.trema.ru)
 
 # pyiArduinoI2Csht
 
 **Данная библилотека (модуль для Python3) позволяет управлять электронными модулями (устройствами) [Цифровой датчик температуры и влажности](https://iarduino.ru/shop/Sensory-Datchiki/datchik-temperatury-i-vlazhnosti-i2c-trema-modul-v2-0.html) от iArduino.ru по шине I2C на Raspberry Pi.**
 
 Подробнее про датчик читайте в нашей [Wiki](https://wiki.iarduino.ru/page/SHT-trema-i2c/#h3_5)
```

### Comparing `pyiArduinoI2Csht-1.0.0/pyiArduinoI2Csht/examples/FindDevices.py` & `pyiArduinoI2Csht-1.0.2/pyiArduinoI2Csht/examples/FindDevices.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Csht-1.0.0/pyiArduinoI2Csht/examples/getAll.py` & `pyiArduinoI2Csht-1.0.2/pyiArduinoI2Csht/examples/getAll.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Csht-1.0.0/pyiArduinoI2Csht/examples/getAllChanged.py` & `pyiArduinoI2Csht-1.0.2/pyiArduinoI2Csht/examples/getAllChanged.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,31 +6,31 @@
 
 # Объявляем объект sht для работы с функциями и методами библиотеки pyiArduinoI2Csht.
 # Если при объявлении объекта указать адрес, например, sht(0xBB), то пример будет
 # работать с тем модулем, адрес которого был указан.
 sht = pyiArduinoI2Csht()
 
 # Указываем фиксировать изменение температуры окружающей среды более чем на 0.1°С.
-sht.setTemChange( 0.1 )
+sht.setTemChange(0.1)
 
 # Указываем фиксировать изменение влажности воздуха более чем на 1%.
-sht.setHumChange( 1.0 )
+sht.setHumChange(1.0)
 
 while True:
 
     # Если температура окружающей среды изменилась более чем
     # на значение указанное в функции setTemChange(), то ...
     if sht.getTemChanged():
 
         # Выводим текущую температуру окружающей среды, от -40 до +125°С.
-        print("Температура = ")
-        print( sht.getTem() )
-        print(" °С.\r\n")
+        print("Температура = %.1f" %
+               sht.getTem(),
+              "°С.")
 
     # Если влажность воздуха изменилась более чем на значение указанное в функции setHumChange(), то ...
     if sht.getHumChanged():
 
         # Выводим текущую влажность воздуха, от 0 до 100%.
-        print("Влажность = ")
-        print( sht.getHum() )
-        print(" %.\r\n")
+        print("Влажность = %.1f" %
+               sht.getHum(),
+              "%.")
     sleep(0.1)
```

### Comparing `pyiArduinoI2Csht-1.0.0/pyiArduinoI2Csht/examples/newAddress.py` & `pyiArduinoI2Csht-1.0.2/pyiArduinoI2Csht/examples/newAddress.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Подключаем библиотеку для работы с датчиком температуры и влажности
 from pyiArduinoI2Csht import *
 import sys
 
 # Объявляем объект sht для работы с функциями и методами библиотеки pyiArduinoI2Csht.
 # Если при объявлении объекта указать адрес, например, sht(0xBB),
 # то пример будет работать с тем модулем, адрес которого был указан.
-sht = pyiArduinoI2Csht()
+sht = pyiArduinoI2Csht(None, NO_BEGIN)
 
 # Если сценарию не были переданы аргументы
 if len(sys.argv) < 2:
     # Назначаем модулю адрес (0x07 < адрес < 0x7F).
     newAddress = 0x09
 
 # Иначе
```

### Comparing `pyiArduinoI2Csht-1.0.0/pyiArduinoI2Csht/examples/setPeriod.py` & `pyiArduinoI2Csht-1.0.2/pyiArduinoI2Csht/examples/setPeriod.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # ЗАДАНИЕ ПЕРИОДА ОБНОВЛЕНИЯ ПОКАЗАНИЙ ДАТЧИКОВ:
 
 # Подключаем библиотеку для работы с датчиком температуры и влажности I2C-flash (Sensor Humidity and Temperature).
 from pyiArduinoI2Csht import *
 from time import sleep
 
 # Объявляем объект sht для работы с функциями и методами библиотеки pyiArduinoI2Csht.
-# Если при объявлении объекта указать адрес, например, sht(0xBB),
+# Если при объявлении объекта указать адрес, например, sht(0x09),
 # то пример будет работать с тем модулем, адрес которого был указан.
 sht = pyiArduinoI2Csht()
 
 # Указываем модулю обновлять показания датчиков каждые две секунды.
 sht.setPeriod(2.0)
 
 while True:
     # Выводим текущую температуру и влажность
-    print("t="+str(sht.getTem())+"°C, ")
-    print("RH="+str(sht.getHum())+"%%")
+    print("t = %.1f" % sht.getTem(),"°C,",
+          "RH = %.1f" % sht.getHum(),"%%")
     sleep(.1)
```

### Comparing `pyiArduinoI2Csht-1.0.0/pyiArduinoI2Csht/iarduino_I2C_PI.h` & `pyiArduinoI2Csht-1.0.2/pyiArduinoI2Csht/iarduino_I2C_PI.h`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Csht-1.0.0/pyiArduinoI2Csht/iarduino_I2C_SHT.cpp` & `pyiArduinoI2Csht-1.0.2/pyiArduinoI2Csht/iarduino_I2C_SHT.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Csht-1.0.0/pyiArduinoI2Csht/iarduino_I2C_SHT.h` & `pyiArduinoI2Csht-1.0.2/pyiArduinoI2Csht/iarduino_I2C_SHT.h`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Csht-1.0.0/pyiArduinoI2Csht/iarduino_I2C_SHT.pxd` & `pyiArduinoI2Csht-1.0.2/pyiArduinoI2Csht/iarduino_I2C_SHT.pxd`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Csht-1.0.0/pyiArduinoI2Csht/pyiArduinoI2Csht.pyx` & `pyiArduinoI2Csht-1.0.2/pyiArduinoI2Csht/pyiArduinoI2Csht.pyx`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Csht-1.0.0/setup.py` & `pyiArduinoI2Csht-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from distutils.extension import Extension
 
 def readme():
     with open('README.md') as readme:
         return readme.read()
 
 setup(name='pyiArduinoI2Csht',
-    version='1.0.0',
+    version='1.0.2',
     description='iarduino.ru module for Raspberry Pi',
     long_description=readme(),
     classifiers=[
         'Programming Language :: Python :: 3',
     ],
     url='http://github.com/tremaru/pyiArduinoI2Csht',
     author='iarduino.ru',
```

