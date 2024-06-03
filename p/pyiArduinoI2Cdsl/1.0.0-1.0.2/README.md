# Comparing `tmp/pyiArduinoI2Cdsl-1.0.0.tar.gz` & `tmp/pyiArduinoI2Cdsl-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyiArduinoI2Cdsl-1.0.0.tar", last modified: Tue Feb  4 12:18:12 2020, max compression
+gzip compressed data, was "pyiArduinoI2Cdsl-1.0.2.tar", last modified: Mon Jun  3 11:54:49 2024, max compression
```

## Comparing `pyiArduinoI2Cdsl-1.0.0.tar` & `pyiArduinoI2Cdsl-1.0.2.tar`

### file list

```diff
@@ -1,25 +1,32 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2020-02-04 12:18:12.000000 pyiArduinoI2Cdsl-1.0.0/
--rw-r--r--   0 pi        (1000) pi        (1000)     2415 2020-02-04 12:18:12.000000 pyiArduinoI2Cdsl-1.0.0/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)       19 2020-02-03 10:30:35.000000 pyiArduinoI2Cdsl-1.0.0/README
--rw-r--r--   0 pi        (1000) pi        (1000)     1856 2020-02-03 10:30:35.000000 pyiArduinoI2Cdsl-1.0.0/README.md
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2020-02-04 12:18:12.000000 pyiArduinoI2Cdsl-1.0.0/pyiArduinoI2Cdsl/
--rw-r--r--   0 pi        (1000) pi        (1000)       26 2020-02-03 10:30:35.000000 pyiArduinoI2Cdsl-1.0.0/pyiArduinoI2Cdsl/__init__.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2020-02-04 12:18:12.000000 pyiArduinoI2Cdsl-1.0.0/pyiArduinoI2Cdsl/cpp/
--rw-r--r--   0 pi        (1000) pi        (1000)     9722 2020-02-03 08:55:28.000000 pyiArduinoI2Cdsl-1.0.0/pyiArduinoI2Cdsl/cpp/FindDevices.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)     1490 2020-02-03 11:16:03.000000 pyiArduinoI2Cdsl-1.0.0/pyiArduinoI2Cdsl/cpp/NewAddress.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)     2154 2020-02-04 11:48:18.000000 pyiArduinoI2Cdsl-1.0.0/pyiArduinoI2Cdsl/cpp/getAll.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)     2028 2020-02-04 11:51:44.000000 pyiArduinoI2Cdsl-1.0.0/pyiArduinoI2Cdsl/cpp/getLuxChanged.cpp
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2020-02-04 12:18:12.000000 pyiArduinoI2Cdsl-1.0.0/pyiArduinoI2Cdsl/examples/
--rw-r--r--   0 pi        (1000) pi        (1000)     5581 2020-02-03 09:05:20.000000 pyiArduinoI2Cdsl-1.0.0/pyiArduinoI2Cdsl/examples/FindDevices.py
--rw-r--r--   0 pi        (1000) pi        (1000)     1255 2020-02-04 12:16:13.000000 pyiArduinoI2Cdsl-1.0.0/pyiArduinoI2Cdsl/examples/getAll.py
--rw-r--r--   0 pi        (1000) pi        (1000)     1207 2020-02-04 12:14:51.000000 pyiArduinoI2Cdsl-1.0.0/pyiArduinoI2Cdsl/examples/getLuxChanged.py
--rw-r--r--   0 pi        (1000) pi        (1000)     1380 2020-02-03 10:30:35.000000 pyiArduinoI2Cdsl-1.0.0/pyiArduinoI2Cdsl/examples/newAddress.py
--rw-r--r--   0 pi        (1000) pi        (1000)    33715 2020-02-03 10:38:01.000000 pyiArduinoI2Cdsl-1.0.0/pyiArduinoI2Cdsl/iarduino_I2C_DSL.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)    18032 2020-02-03 11:27:54.000000 pyiArduinoI2Cdsl-1.0.0/pyiArduinoI2Cdsl/iarduino_I2C_DSL.h
--rw-r--r--   0 pi        (1000) pi        (1000)      584 2020-02-03 11:24:15.000000 pyiArduinoI2Cdsl-1.0.0/pyiArduinoI2Cdsl/iarduino_I2C_DSL.pxd
--rwxr-xr-x   0 pi        (1000) pi        (1000)    11361 2020-02-03 11:22:47.000000 pyiArduinoI2Cdsl-1.0.0/pyiArduinoI2Cdsl/iarduino_I2C_PI.h
--rw-r--r--   0 pi        (1000) pi        (1000)   200064 2020-02-03 11:27:58.000000 pyiArduinoI2Cdsl-1.0.0/pyiArduinoI2Cdsl/pyiArduinoI2Cdsl.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)     3083 2020-02-03 11:25:28.000000 pyiArduinoI2Cdsl-1.0.0/pyiArduinoI2Cdsl/pyiArduinoI2Cdsl.pyx
--rw-r--r--   0 pi        (1000) pi        (1000)      129 2020-02-03 10:30:35.000000 pyiArduinoI2Cdsl-1.0.0/pyiArduinoI2Cdsl/setup.py
--rw-r--r--   0 pi        (1000) pi        (1000)       40 2020-02-03 08:55:28.000000 pyiArduinoI2Cdsl-1.0.0/setup.cfg
--rw-r--r--   0 pi        (1000) pi        (1000)      708 2020-02-04 12:18:02.000000 pyiArduinoI2Cdsl-1.0.0/setup.py
+drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-06-03 11:54:49.826093 pyiArduinoI2Cdsl-1.0.2/
+-rw-r--r--   0 dron      (1000) dron      (1000)     3289 2024-03-29 13:35:24.000000 pyiArduinoI2Cdsl-1.0.2/LICENSE
+-rw-r--r--   0 dron      (1000) dron      (1000)       81 2024-03-29 13:35:24.000000 pyiArduinoI2Cdsl-1.0.2/MANIFEST.in
+-rw-r--r--   0 dron      (1000) dron      (1000)     2150 2024-06-03 11:54:49.826093 pyiArduinoI2Cdsl-1.0.2/PKG-INFO
+-rw-r--r--   0 dron      (1000) dron      (1000)       19 2024-03-29 13:35:24.000000 pyiArduinoI2Cdsl-1.0.2/README
+-rw-r--r--   0 dron      (1000) dron      (1000)     1856 2024-03-29 13:35:24.000000 pyiArduinoI2Cdsl-1.0.2/README.md
+drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-06-03 11:54:49.818093 pyiArduinoI2Cdsl-1.0.2/pyiArduinoI2Cdsl/
+-rw-r--r--   0 dron      (1000) dron      (1000)       26 2024-03-29 13:35:24.000000 pyiArduinoI2Cdsl-1.0.2/pyiArduinoI2Cdsl/__init__.py
+drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-06-03 11:54:49.822093 pyiArduinoI2Cdsl-1.0.2/pyiArduinoI2Cdsl/cpp/
+-rw-r--r--   0 dron      (1000) dron      (1000)     9722 2024-03-29 13:35:24.000000 pyiArduinoI2Cdsl-1.0.2/pyiArduinoI2Cdsl/cpp/FindDevices.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     1490 2024-03-29 13:35:24.000000 pyiArduinoI2Cdsl-1.0.2/pyiArduinoI2Cdsl/cpp/NewAddress.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     2154 2024-03-29 13:35:24.000000 pyiArduinoI2Cdsl-1.0.2/pyiArduinoI2Cdsl/cpp/getAll.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     2028 2024-03-29 13:35:24.000000 pyiArduinoI2Cdsl-1.0.2/pyiArduinoI2Cdsl/cpp/getLuxChanged.cpp
+drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-06-03 11:54:49.826093 pyiArduinoI2Cdsl-1.0.2/pyiArduinoI2Cdsl/examples/
+-rw-r--r--   0 dron      (1000) dron      (1000)     5581 2024-03-29 13:35:24.000000 pyiArduinoI2Cdsl-1.0.2/pyiArduinoI2Cdsl/examples/FindDevices.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     1255 2024-03-29 13:35:24.000000 pyiArduinoI2Cdsl-1.0.2/pyiArduinoI2Cdsl/examples/getAll.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     1207 2024-03-29 13:35:24.000000 pyiArduinoI2Cdsl-1.0.2/pyiArduinoI2Cdsl/examples/getLuxChanged.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     1380 2024-03-29 13:35:24.000000 pyiArduinoI2Cdsl-1.0.2/pyiArduinoI2Cdsl/examples/newAddress.py
+-rw-r--r--   0 dron      (1000) dron      (1000)    33715 2024-03-29 13:35:24.000000 pyiArduinoI2Cdsl-1.0.2/pyiArduinoI2Cdsl/iarduino_I2C_DSL.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)    18032 2024-03-29 13:35:24.000000 pyiArduinoI2Cdsl-1.0.2/pyiArduinoI2Cdsl/iarduino_I2C_DSL.h
+-rw-r--r--   0 dron      (1000) dron      (1000)      584 2024-03-29 13:35:24.000000 pyiArduinoI2Cdsl-1.0.2/pyiArduinoI2Cdsl/iarduino_I2C_DSL.pxd
+-rwxr-xr-x   0 dron      (1000) dron      (1000)    11361 2024-03-29 13:35:24.000000 pyiArduinoI2Cdsl-1.0.2/pyiArduinoI2Cdsl/iarduino_I2C_PI.h
+-rw-r--r--   0 dron      (1000) dron      (1000)   427755 2024-06-03 11:45:48.000000 pyiArduinoI2Cdsl-1.0.2/pyiArduinoI2Cdsl/pyiArduinoI2Cdsl.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     3083 2024-03-29 13:35:24.000000 pyiArduinoI2Cdsl-1.0.2/pyiArduinoI2Cdsl/pyiArduinoI2Cdsl.pyx
+-rw-r--r--   0 dron      (1000) dron      (1000)      129 2024-03-29 13:35:24.000000 pyiArduinoI2Cdsl-1.0.2/pyiArduinoI2Cdsl/setup.py
+drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-06-03 11:54:49.822093 pyiArduinoI2Cdsl-1.0.2/pyiArduinoI2Cdsl.egg-info/
+-rw-r--r--   0 dron      (1000) dron      (1000)     2150 2024-06-03 11:54:49.000000 pyiArduinoI2Cdsl-1.0.2/pyiArduinoI2Cdsl.egg-info/PKG-INFO
+-rw-r--r--   0 dron      (1000) dron      (1000)      797 2024-06-03 11:54:49.000000 pyiArduinoI2Cdsl-1.0.2/pyiArduinoI2Cdsl.egg-info/SOURCES.txt
+-rw-r--r--   0 dron      (1000) dron      (1000)        1 2024-06-03 11:54:49.000000 pyiArduinoI2Cdsl-1.0.2/pyiArduinoI2Cdsl.egg-info/dependency_links.txt
+-rw-r--r--   0 dron      (1000) dron      (1000)       17 2024-06-03 11:54:49.000000 pyiArduinoI2Cdsl-1.0.2/pyiArduinoI2Cdsl.egg-info/top_level.txt
+-rw-r--r--   0 dron      (1000) dron      (1000)       79 2024-06-03 11:54:49.826093 pyiArduinoI2Cdsl-1.0.2/setup.cfg
+-rw-r--r--   0 dron      (1000) dron      (1000)      708 2024-06-03 11:51:43.000000 pyiArduinoI2Cdsl-1.0.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyiArduinoI2Cdsl-1.0.0/PKG-INFO` & `pyiArduinoI2Cdsl-1.0.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pyiArduinoI2Cdsl
-Version: 1.0.0
+Version: 1.0.2
 Summary: iarduino.ru module for Raspberry Pi
 Home-page: http://github.com/tremaru/pyiArduinoI2Cdsl
 Author: iarduino.ru
 Author-email: shop@iarduino.ru
 License: MIT
-Description: [![](https://iarduino.ru/img/logo.svg)](https://iarduino.ru)[![](https://wiki.iarduino.ru/img/git-shop.svg?3)](https://iarduino.ru) [![](https://wiki.iarduino.ru/img/git-wiki.svg?2)](https://wiki.iarduino.ru) [![](https://wiki.iarduino.ru/img/git-lesson.svg?2)](https://lesson.iarduino.ru)[![](https://wiki.iarduino.ru/img/git-forum.svg?2)](http://forum.trema.ru)
-        
-        # pyiArduinoI2Cdsl
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
-        `sudo pip3 install pyiArduinoI2Cdsl`
-        
-        Самостоятельная сборка из исходников:
-        
-        `git clone https://github.com/tremaru/pyiArduinoI2Cdsl.git && cd pyiArduinoI2Cdsl/pyiArduinoI2Cdsl && python3 setup.py build_ext --inplace`
-        
-        Примеры для Python находятся в папке `pyiArduinoI2Cdsl/examples`
-        
-        Примеры для С++ находятся в папке `pyiArduinoI2Cdsl/cpp`. Так же в этой папке лежит *Makefile* для сборки
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
+# pyiArduinoI2Cdsl
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
+`sudo pip3 install pyiArduinoI2Cdsl`
+
+Самостоятельная сборка из исходников:
+
+`git clone https://github.com/tremaru/pyiArduinoI2Cdsl.git && cd pyiArduinoI2Cdsl/pyiArduinoI2Cdsl && python3 setup.py build_ext --inplace`
+
+Примеры для Python находятся в папке `pyiArduinoI2Cdsl/examples`
+
+Примеры для С++ находятся в папке `pyiArduinoI2Cdsl/cpp`. Так же в этой папке лежит *Makefile* для сборки
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

### Comparing `pyiArduinoI2Cdsl-1.0.0/README.md` & `pyiArduinoI2Cdsl-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cdsl-1.0.0/pyiArduinoI2Cdsl/cpp/FindDevices.cpp` & `pyiArduinoI2Cdsl-1.0.2/pyiArduinoI2Cdsl/cpp/FindDevices.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cdsl-1.0.0/pyiArduinoI2Cdsl/cpp/NewAddress.cpp` & `pyiArduinoI2Cdsl-1.0.2/pyiArduinoI2Cdsl/cpp/NewAddress.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cdsl-1.0.0/pyiArduinoI2Cdsl/cpp/getAll.cpp` & `pyiArduinoI2Cdsl-1.0.2/pyiArduinoI2Cdsl/cpp/getAll.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cdsl-1.0.0/pyiArduinoI2Cdsl/cpp/getLuxChanged.cpp` & `pyiArduinoI2Cdsl-1.0.2/pyiArduinoI2Cdsl/cpp/getLuxChanged.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cdsl-1.0.0/pyiArduinoI2Cdsl/examples/FindDevices.py` & `pyiArduinoI2Cdsl-1.0.2/pyiArduinoI2Cdsl/examples/FindDevices.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cdsl-1.0.0/pyiArduinoI2Cdsl/examples/getAll.py` & `pyiArduinoI2Cdsl-1.0.2/pyiArduinoI2Cdsl/examples/getAll.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cdsl-1.0.0/pyiArduinoI2Cdsl/examples/getLuxChanged.py` & `pyiArduinoI2Cdsl-1.0.2/pyiArduinoI2Cdsl/examples/getLuxChanged.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cdsl-1.0.0/pyiArduinoI2Cdsl/examples/newAddress.py` & `pyiArduinoI2Cdsl-1.0.2/pyiArduinoI2Cdsl/examples/newAddress.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cdsl-1.0.0/pyiArduinoI2Cdsl/iarduino_I2C_DSL.cpp` & `pyiArduinoI2Cdsl-1.0.2/pyiArduinoI2Cdsl/iarduino_I2C_DSL.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cdsl-1.0.0/pyiArduinoI2Cdsl/iarduino_I2C_DSL.h` & `pyiArduinoI2Cdsl-1.0.2/pyiArduinoI2Cdsl/iarduino_I2C_DSL.h`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cdsl-1.0.0/pyiArduinoI2Cdsl/iarduino_I2C_DSL.pxd` & `pyiArduinoI2Cdsl-1.0.2/pyiArduinoI2Cdsl/iarduino_I2C_DSL.pxd`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cdsl-1.0.0/pyiArduinoI2Cdsl/iarduino_I2C_PI.h` & `pyiArduinoI2Cdsl-1.0.2/pyiArduinoI2Cdsl/iarduino_I2C_PI.h`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cdsl-1.0.0/pyiArduinoI2Cdsl/pyiArduinoI2Cdsl.pyx` & `pyiArduinoI2Cdsl-1.0.2/pyiArduinoI2Cdsl/pyiArduinoI2Cdsl.pyx`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cdsl-1.0.0/setup.py` & `pyiArduinoI2Cdsl-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from distutils.extension import Extension
 
 def readme():
     with open('README.md') as readme:
         return readme.read()
 
 setup(name='pyiArduinoI2Cdsl',
-    version='1.0.0',
+    version='1.0.2',
     description='iarduino.ru module for Raspberry Pi',
     long_description=readme(),
     classifiers=[
         'Programming Language :: Python :: 3',
     ],
     url='http://github.com/tremaru/pyiArduinoI2Cdsl',
     author='iarduino.ru',
```

