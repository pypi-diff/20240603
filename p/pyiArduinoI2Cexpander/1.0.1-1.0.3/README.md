# Comparing `tmp/pyiArduinoI2Cexpander-1.0.1.tar.gz` & `tmp/pyiArduinoI2Cexpander-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyiArduinoI2Cexpander-1.0.1.tar", last modified: Fri Apr 12 09:19:34 2024, max compression
+gzip compressed data, was "pyiArduinoI2Cexpander-1.0.3.tar", last modified: Mon Jun  3 11:54:53 2024, max compression
```

## Comparing `pyiArduinoI2Cexpander-1.0.1.tar` & `pyiArduinoI2Cexpander-1.0.3.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-04-12 09:19:34.586280 pyiArduinoI2Cexpander-1.0.1/
--rw-r--r--   0 dron      (1000) dron      (1000)     3289 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/LICENSE
--rw-r--r--   0 dron      (1000) dron      (1000)       86 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/MANIFEST.in
--rw-r--r--   0 dron      (1000) dron      (1000)     2223 2024-04-12 09:19:34.586280 pyiArduinoI2Cexpander-1.0.1/PKG-INFO
--rw-r--r--   0 dron      (1000) dron      (1000)     1919 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/README.md
-drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-04-12 09:19:34.562280 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/
--rw-r--r--   0 dron      (1000) dron      (1000)       31 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/__init__.py
-drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-04-12 09:19:34.574280 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/
--rw-r--r--   0 dron      (1000) dron      (1000)     9722 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/FindDevices.cpp
--rw-r--r--   0 dron      (1000) dron      (1000)     3315 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/NewAddress.cpp
--rw-r--r--   0 dron      (1000) dron      (1000)     3614 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/analogAveraging.cpp
--rw-r--r--   0 dron      (1000) dron      (1000)     3292 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/analogRead.cpp
--rw-r--r--   0 dron      (1000) dron      (1000)     4184 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/analogWrite.cpp
--rw-r--r--   0 dron      (1000) dron      (1000)     3219 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/digitalRead.cpp
--rw-r--r--   0 dron      (1000) dron      (1000)     2831 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/digitalWrite.cpp
--rw-r--r--   0 dron      (1000) dron      (1000)     6401 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/freqPWM.cpp
--rw-r--r--   0 dron      (1000) dron      (1000)     2319 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/getVersion.cpp
--rw-r--r--   0 dron      (1000) dron      (1000)     4127 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/levelRead.cpp
--rw-r--r--   0 dron      (1000) dron      (1000)     6781 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/pinMode.cpp
--rw-r--r--   0 dron      (1000) dron      (1000)     6499 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/pinOutScheme.cpp
--rw-r--r--   0 dron      (1000) dron      (1000)     4624 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/pinPull.cpp
--rw-r--r--   0 dron      (1000) dron      (1000)     2963 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/reset.cpp
--rw-r--r--   0 dron      (1000) dron      (1000)     7301 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/servoAttach.cpp
--rw-r--r--   0 dron      (1000) dron      (1000)     3860 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/servoWrite.cpp
--rw-r--r--   0 dron      (1000) dron      (1000)     4522 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/servoWriteMicroseconds.cpp
-drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-04-12 09:19:34.586280 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/
--rw-r--r--   0 dron      (1000) dron      (1000)     5583 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/FindDevices.py
--rw-r--r--   0 dron      (1000) dron      (1000)     4084 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/NewAddress.py
--rw-r--r--   0 dron      (1000) dron      (1000)     2514 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/analogAveraging.py
--rw-r--r--   0 dron      (1000) dron      (1000)     2324 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/analogRead.py
--rw-r--r--   0 dron      (1000) dron      (1000)     3309 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/analogWrite.py
--rw-r--r--   0 dron      (1000) dron      (1000)     2192 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/digitalRead.py
--rw-r--r--   0 dron      (1000) dron      (1000)     1791 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/digitalWrite.py
--rw-r--r--   0 dron      (1000) dron      (1000)     4827 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/freqPWM.py
--rw-r--r--   0 dron      (1000) dron      (1000)     1313 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/getVersion.py
--rw-r--r--   0 dron      (1000) dron      (1000)     2844 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/levelRead.py
--rw-r--r--   0 dron      (1000) dron      (1000)     6438 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/pinMode.py
--rw-r--r--   0 dron      (1000) dron      (1000)     5360 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/pinOutScheme.py
--rw-r--r--   0 dron      (1000) dron      (1000)     3334 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/pinPull.py
--rw-r--r--   0 dron      (1000) dron      (1000)     2199 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/reset.py
--rw-r--r--   0 dron      (1000) dron      (1000)     6066 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/servoAttach.py
--rw-r--r--   0 dron      (1000) dron      (1000)     2787 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/servoWrite.py
--rw-r--r--   0 dron      (1000) dron      (1000)     3199 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/servoWriteMicroseconds.py
--rw-r--r--   0 dron      (1000) dron      (1000)    54927 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/iarduino_I2C_Expander.cpp
--rw-r--r--   0 dron      (1000) dron      (1000)    21194 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/iarduino_I2C_Expander.h
--rw-r--r--   0 dron      (1000) dron      (1000)     1106 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/iarduino_I2C_Expander.pxd
--rwxr-xr-x   0 dron      (1000) dron      (1000)    12628 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/iarduino_I2C_Expander_PI.h
--rw-r--r--   0 dron      (1000) dron      (1000)   622689 2024-04-12 06:59:39.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/pyiArduinoI2Cexpander.cpp
--rw-r--r--   0 dron      (1000) dron      (1000)     5123 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/pyiArduinoI2Cexpander.pyx
--rw-r--r--   0 dron      (1000) dron      (1000)      134 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/setup.py
-drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-04-12 09:19:34.566280 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander.egg-info/
--rw-r--r--   0 dron      (1000) dron      (1000)     2223 2024-04-12 09:19:34.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander.egg-info/PKG-INFO
--rw-r--r--   0 dron      (1000) dron      (1000)     2062 2024-04-12 09:19:34.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander.egg-info/SOURCES.txt
--rw-r--r--   0 dron      (1000) dron      (1000)        1 2024-04-12 09:19:34.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander.egg-info/dependency_links.txt
--rw-r--r--   0 dron      (1000) dron      (1000)       22 2024-04-12 09:19:34.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander.egg-info/top_level.txt
--rw-r--r--   0 dron      (1000) dron      (1000)       79 2024-04-12 09:19:34.586280 pyiArduinoI2Cexpander-1.0.1/setup.cfg
--rw-r--r--   0 dron      (1000) dron      (1000)      772 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/setup.py
+drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-06-03 11:54:53.334045 pyiArduinoI2Cexpander-1.0.3/
+-rw-r--r--   0 dron      (1000) dron      (1000)     3289 2024-03-29 13:35:26.000000 pyiArduinoI2Cexpander-1.0.3/LICENSE
+-rw-r--r--   0 dron      (1000) dron      (1000)       86 2024-03-29 13:35:26.000000 pyiArduinoI2Cexpander-1.0.3/MANIFEST.in
+-rw-r--r--   0 dron      (1000) dron      (1000)     2223 2024-06-03 11:54:53.334045 pyiArduinoI2Cexpander-1.0.3/PKG-INFO
+-rw-r--r--   0 dron      (1000) dron      (1000)     1919 2024-03-29 13:35:26.000000 pyiArduinoI2Cexpander-1.0.3/README.md
+drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-06-03 11:54:53.310046 pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/
+-rw-r--r--   0 dron      (1000) dron      (1000)       31 2024-03-29 13:35:26.000000 pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/__init__.py
+drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-06-03 11:54:53.322045 pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/cpp/
+-rw-r--r--   0 dron      (1000) dron      (1000)     9722 2024-03-29 13:35:26.000000 pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/cpp/FindDevices.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     3315 2024-03-29 13:35:26.000000 pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/cpp/NewAddress.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     3614 2024-03-29 13:35:26.000000 pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/cpp/analogAveraging.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     3292 2024-03-29 13:35:26.000000 pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/cpp/analogRead.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     4184 2024-03-29 13:35:26.000000 pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/cpp/analogWrite.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     3219 2024-03-29 13:35:26.000000 pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/cpp/digitalRead.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     2831 2024-03-29 13:35:26.000000 pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/cpp/digitalWrite.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     6401 2024-03-29 13:35:26.000000 pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/cpp/freqPWM.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     2319 2024-03-29 13:35:26.000000 pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/cpp/getVersion.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     4127 2024-03-29 13:35:26.000000 pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/cpp/levelRead.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     6781 2024-03-29 13:35:26.000000 pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/cpp/pinMode.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     6499 2024-03-29 13:35:26.000000 pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/cpp/pinOutScheme.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     4624 2024-03-29 13:35:26.000000 pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/cpp/pinPull.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     2963 2024-03-29 13:35:26.000000 pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/cpp/reset.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     7301 2024-03-29 13:35:26.000000 pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/cpp/servoAttach.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     3860 2024-03-29 13:35:26.000000 pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/cpp/servoWrite.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     4522 2024-03-29 13:35:26.000000 pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/cpp/servoWriteMicroseconds.cpp
+drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-06-03 11:54:53.334045 pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/examples/
+-rw-r--r--   0 dron      (1000) dron      (1000)     5583 2024-03-29 13:35:26.000000 pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/examples/FindDevices.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     4084 2024-03-29 13:35:26.000000 pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/examples/NewAddress.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     2514 2024-03-29 13:35:26.000000 pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/examples/analogAveraging.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     2324 2024-03-29 13:35:26.000000 pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/examples/analogRead.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     3309 2024-03-29 13:35:26.000000 pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/examples/analogWrite.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     2192 2024-03-29 13:35:26.000000 pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/examples/digitalRead.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     1791 2024-03-29 13:35:26.000000 pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/examples/digitalWrite.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     4827 2024-03-29 13:35:26.000000 pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/examples/freqPWM.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     1313 2024-03-29 13:35:26.000000 pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/examples/getVersion.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     2844 2024-03-29 13:35:26.000000 pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/examples/levelRead.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     6438 2024-03-29 13:35:26.000000 pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/examples/pinMode.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     5360 2024-03-29 13:35:26.000000 pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/examples/pinOutScheme.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     3334 2024-03-29 13:35:26.000000 pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/examples/pinPull.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     2199 2024-03-29 13:35:26.000000 pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/examples/reset.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     6066 2024-03-29 13:35:26.000000 pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/examples/servoAttach.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     2787 2024-03-29 13:35:26.000000 pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/examples/servoWrite.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     3199 2024-03-29 13:35:26.000000 pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/examples/servoWriteMicroseconds.py
+-rw-r--r--   0 dron      (1000) dron      (1000)    54927 2024-03-29 13:35:26.000000 pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/iarduino_I2C_Expander.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)    21194 2024-03-29 13:35:26.000000 pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/iarduino_I2C_Expander.h
+-rw-r--r--   0 dron      (1000) dron      (1000)     1106 2024-03-29 13:35:26.000000 pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/iarduino_I2C_Expander.pxd
+-rwxr-xr-x   0 dron      (1000) dron      (1000)    12628 2024-03-29 13:35:26.000000 pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/iarduino_I2C_Expander_PI.h
+-rw-r--r--   0 dron      (1000) dron      (1000)   622689 2024-06-03 11:48:04.000000 pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/pyiArduinoI2Cexpander.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     5123 2024-03-29 13:35:26.000000 pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/pyiArduinoI2Cexpander.pyx
+-rw-r--r--   0 dron      (1000) dron      (1000)      134 2024-03-29 13:35:26.000000 pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/setup.py
+drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-06-03 11:54:53.314046 pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander.egg-info/
+-rw-r--r--   0 dron      (1000) dron      (1000)     2223 2024-06-03 11:54:52.000000 pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander.egg-info/PKG-INFO
+-rw-r--r--   0 dron      (1000) dron      (1000)     2062 2024-06-03 11:54:53.000000 pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander.egg-info/SOURCES.txt
+-rw-r--r--   0 dron      (1000) dron      (1000)        1 2024-06-03 11:54:52.000000 pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander.egg-info/dependency_links.txt
+-rw-r--r--   0 dron      (1000) dron      (1000)       22 2024-06-03 11:54:52.000000 pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander.egg-info/top_level.txt
+-rw-r--r--   0 dron      (1000) dron      (1000)       79 2024-06-03 11:54:53.334045 pyiArduinoI2Cexpander-1.0.3/setup.cfg
+-rw-r--r--   0 dron      (1000) dron      (1000)      772 2024-06-03 11:51:48.000000 pyiArduinoI2Cexpander-1.0.3/setup.py
```

### Comparing `pyiArduinoI2Cexpander-1.0.1/LICENSE` & `pyiArduinoI2Cexpander-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-1.0.1/PKG-INFO` & `pyiArduinoI2Cexpander-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiArduinoI2Cexpander
-Version: 1.0.1
+Version: 1.0.3
 Summary: iarduino.ru module for Raspberry Pi
 Home-page: http://github.com/tremaru/pyiArduinoI2Cexpander
 Author: iarduino.ru
 Author-email: shop@iarduino.ru
 License: MIT
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
```

### Comparing `pyiArduinoI2Cexpander-1.0.1/README.md` & `pyiArduinoI2Cexpander-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/FindDevices.cpp` & `pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/cpp/FindDevices.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/NewAddress.cpp` & `pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/cpp/NewAddress.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/analogAveraging.cpp` & `pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/cpp/analogAveraging.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/analogRead.cpp` & `pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/cpp/analogRead.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/analogWrite.cpp` & `pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/cpp/analogWrite.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/digitalRead.cpp` & `pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/cpp/digitalRead.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/digitalWrite.cpp` & `pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/cpp/digitalWrite.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/freqPWM.cpp` & `pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/cpp/freqPWM.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/getVersion.cpp` & `pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/cpp/getVersion.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/levelRead.cpp` & `pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/cpp/levelRead.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/pinMode.cpp` & `pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/cpp/pinMode.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/pinOutScheme.cpp` & `pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/cpp/pinOutScheme.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/pinPull.cpp` & `pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/cpp/pinPull.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/reset.cpp` & `pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/cpp/reset.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/servoAttach.cpp` & `pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/cpp/servoAttach.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/servoWrite.cpp` & `pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/cpp/servoWrite.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/servoWriteMicroseconds.cpp` & `pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/cpp/servoWriteMicroseconds.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/FindDevices.py` & `pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/examples/FindDevices.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/NewAddress.py` & `pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/examples/NewAddress.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/analogAveraging.py` & `pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/examples/analogAveraging.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/analogRead.py` & `pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/examples/analogRead.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/analogWrite.py` & `pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/examples/analogWrite.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/digitalRead.py` & `pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/examples/digitalRead.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/digitalWrite.py` & `pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/examples/digitalWrite.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/freqPWM.py` & `pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/examples/freqPWM.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/getVersion.py` & `pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/examples/getVersion.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/levelRead.py` & `pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/examples/levelRead.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/pinMode.py` & `pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/examples/pinMode.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/pinOutScheme.py` & `pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/examples/pinOutScheme.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/pinPull.py` & `pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/examples/pinPull.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/reset.py` & `pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/examples/reset.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/servoAttach.py` & `pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/examples/servoAttach.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/servoWrite.py` & `pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/examples/servoWrite.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/servoWriteMicroseconds.py` & `pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/examples/servoWriteMicroseconds.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/iarduino_I2C_Expander.cpp` & `pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/iarduino_I2C_Expander.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/iarduino_I2C_Expander.h` & `pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/iarduino_I2C_Expander.h`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/iarduino_I2C_Expander.pxd` & `pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/iarduino_I2C_Expander.pxd`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/iarduino_I2C_Expander_PI.h` & `pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/iarduino_I2C_Expander_PI.h`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/pyiArduinoI2Cexpander.cpp` & `pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/pyiArduinoI2Cexpander.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/pyiArduinoI2Cexpander.pyx` & `pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander/pyiArduinoI2Cexpander.pyx`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander.egg-info/PKG-INFO` & `pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiArduinoI2Cexpander
-Version: 1.0.1
+Version: 1.0.3
 Summary: iarduino.ru module for Raspberry Pi
 Home-page: http://github.com/tremaru/pyiArduinoI2Cexpander
 Author: iarduino.ru
 Author-email: shop@iarduino.ru
 License: MIT
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
```

### Comparing `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander.egg-info/SOURCES.txt` & `pyiArduinoI2Cexpander-1.0.3/pyiArduinoI2Cexpander.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-1.0.1/setup.py` & `pyiArduinoI2Cexpander-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from distutils.extension import Extension
 
 def readme():
     with open('README.md') as readme:
         return readme.read()
 
 setup(name='pyiArduinoI2Cexpander',
-    version='1.0.1',
+    version='1.0.3',
     description='iarduino.ru module for Raspberry Pi',
     long_description=readme(),
     classifiers=[
         'Programming Language :: Python :: 3',
     ],
     url='http://github.com/tremaru/pyiArduinoI2Cexpander',
     author='iarduino.ru',
```

